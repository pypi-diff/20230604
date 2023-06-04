# Comparing `tmp/pe-0.3.2.tar.gz` & `tmp/pe-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-0.3.2.tar", last modified: Wed Oct  6 00:00:00 2021, max compression
+gzip compressed data, was "pe-0.4.0.tar", last modified: Sun Jun  4 20:10:15 2023, max compression
```

## Comparing `pe-0.3.2.tar` & `pe-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 00:00:00.371703 pe-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-10-05 23:59:49.000000 pe-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7552 2021-10-06 00:00:00.371703 pe-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6386 2021-10-05 23:59:49.000000 pe-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 00:00:00.367702 pe-0.3.2/pe/
--rw-r--r--   0 runner    (1001) docker     (121)      768 2021-10-05 23:59:49.000000 pe-0.3.2/pe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)  1096209 2021-10-05 23:59:59.000000 pe-0.3.2/pe/_cy_machine.c
--rw-r--r--   0 runner    (1001) docker     (121)    16281 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_cy_machine.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     3481 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_escape.py
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2645 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_grammar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_match.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8917 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)     7531 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    13790 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_py_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-10-05 23:59:49.000000 pe-0.3.2/pe/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2836 2021-10-05 23:59:49.000000 pe-0.3.2/pe/actions.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-10-05 23:59:49.000000 pe-0.3.2/pe/machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     4313 2021-10-05 23:59:49.000000 pe-0.3.2/pe/operators.py
--rw-r--r--   0 runner    (1001) docker     (121)    12515 2021-10-05 23:59:49.000000 pe-0.3.2/pe/packrat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 00:00:00.367702 pe-0.3.2/pe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7552 2021-10-06 00:00:00.000000 pe-0.3.2/pe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-10-06 00:00:00.000000 pe-0.3.2/pe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-06 00:00:00.000000 pe-0.3.2/pe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-06 00:00:00.000000 pe-0.3.2/pe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-10-06 00:00:00.000000 pe-0.3.2/pe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-05 23:59:49.000000 pe-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2021-10-06 00:00:00.371703 pe-0.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1069 2021-10-05 23:59:49.000000 pe-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 00:00:00.371703 pe-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-10-05 23:59:49.000000 pe-0.3.2/test/test__definition.py
--rw-r--r--   0 runner    (1001) docker     (121)     3156 2021-10-05 23:59:49.000000 pe-0.3.2/test/test__match.py
--rw-r--r--   0 runner    (1001) docker     (121)     5184 2021-10-05 23:59:49.000000 pe-0.3.2/test/test__optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3317 2021-10-05 23:59:49.000000 pe-0.3.2/test/test__parse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2021-10-05 23:59:49.000000 pe-0.3.2/test/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     6803 2021-10-05 23:59:49.000000 pe-0.3.2/test/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2021-10-05 23:59:49.000000 pe-0.3.2/test/test_pe.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2021-10-05 23:59:49.000000 pe-0.3.2/test/test_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:10:15.158856 pe-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-04 20:10:06.000000 pe-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-06-04 20:10:15.158856 pe-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-04 20:10:06.000000 pe-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:10:15.154855 pe-0.4.0/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-04 20:10:06.000000 pe-0.4.0/pe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1115685 2023-06-04 20:10:14.000000 pe-0.4.0/pe/_cy_machine.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_cy_machine.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_py_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-04 20:10:06.000000 pe-0.4.0/pe/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-04 20:10:06.000000 pe-0.4.0/pe/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-04 20:10:06.000000 pe-0.4.0/pe/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-06-04 20:10:06.000000 pe-0.4.0/pe/packrat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:10:15.154855 pe-0.4.0/pe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-06-04 20:10:15.000000 pe-0.4.0/pe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-04 20:10:15.000000 pe-0.4.0/pe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:10:15.000000 pe-0.4.0/pe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:10:15.000000 pe-0.4.0/pe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-04 20:10:15.000000 pe-0.4.0/pe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 20:10:06.000000 pe-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-04 20:10:15.158856 pe-0.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-06-04 20:10:06.000000 pe-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:10:15.158856 pe-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-04 20:10:06.000000 pe-0.4.0/test/test__definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-04 20:10:06.000000 pe-0.4.0/test/test__match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-04 20:10:06.000000 pe-0.4.0/test/test__optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-04 20:10:06.000000 pe-0.4.0/test/test__parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-04 20:10:06.000000 pe-0.4.0/test/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-04 20:10:06.000000 pe-0.4.0/test/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-04 20:10:06.000000 pe-0.4.0/test/test_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-04 20:10:06.000000 pe-0.4.0/test/test_regression.py
```

### Comparing `pe-0.3.2/LICENSE` & `pe-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/PKG-INFO` & `pe-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: pe
-Version: 0.3.2
+Version: 0.4.0
 Summary: Library for Parsing Expression Grammars (PEG)
 Home-page: https://github.com/goodmami/pe/
 Author: Michael Wayne Goodman
 Author-email: goodman.m.w@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/goodmami/pe/blob/main/docs/README.md
 Project-URL: Changelog, https://github.com/goodmami/pe/blob/main/CHANGELOG.md
 Keywords: peg,parsing,text
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/goodmami/pe/main/docs/_static/pe-logo.svg" alt="pe logo">
   <br>
@@ -243,9 +242,7 @@
 - [TatSu](https://tatsu.readthedocs.io/en/stable/) (Python)
 - [PEG.js](https://github.com/pegjs/pegjs) (Javascript)
 - [Pegged](https://github.com/PhilippeSigaud/Pegged) (D)
 - [pegen](https://github.com/gvanrossum/pegen) (Python / C)
 - [LPeg] (Lua)
 
 [LPeg]: http://www.inf.puc-rio.br/~roberto/lpeg/
-
-
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pe Version: 0.3.2 Summary: Library for Parsing
+Metadata-Version: 2.1 Name: pe Version: 0.4.0 Summary: Library for Parsing
 Expression Grammars (PEG) Home-page: https://github.com/goodmami/pe/ Author:
 Michael Wayne Goodman Author-email: goodman.m.w@gmail.com License: MIT Project-
 URL: Documentation, https://github.com/goodmami/pe/blob/main/docs/README.md
 Project-URL: Changelog, https://github.com/goodmami/pe/blob/main/CHANGELOG.md
-Keywords: peg,parsing,text Platform: UNKNOWN Classifier: Development Status ::
-4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Cython Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Text Processing Classifier:
-Topic :: Utilities Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE
+Keywords: peg,parsing,text Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Cython Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: Topic :: Text Processing Classifier: Topic :: Utilities
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE
                                   [pe logo]
                              Parsing Expressions
                      [PyPI_link] [Python Support] [tests]
 --- **pe** is a library for parsing expressions, including [parsing expression
 grammars] (PEGs). It aims to join the expressive power of parsing expressions
 with the familiarity of regular expressions. For example: ```python >>> import
 pe >>> pe.match(r'"-"? [0-9]+', '-38') # match an integer
```

### Comparing `pe-0.3.2/README.md` & `pe-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/__init__.py` & `pe-0.4.0/pe/__init__.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/_constants.py` & `pe-0.4.0/pe/_constants.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/_cy_machine.c` & `pe-0.4.0/pe/_cy_machine.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "pe._cy_machine",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -58,14 +58,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -86,26 +87,34 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -135,18 +144,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -158,61 +216,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -321,17 +390,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -437,35 +565,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -561,18 +689,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -589,16 +717,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -720,14 +850,15 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -1244,26 +1375,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1284,21 +1415,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
@@ -1482,14 +1621,17 @@
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* BuildPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
                                                 int prepend_sign, char padding_char);
 
+/* IncludeStringH.proto */
+#include <string.h>
+
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_enum____pyx_t_2pe_11_cy_machine_OpCode(enum __pyx_t_2pe_11_cy_machine_OpCode value, Py_ssize_t width, char padding_char, char format_char);
 
 /* SliceObject.proto */
 #define __Pyx_PyObject_DelSlice(obj, cstart, cstop, py_start, py_stop, py_slice, has_cstart, has_cstop, wraparound)\
     __Pyx_PyObject_SetSlice(obj, (PyObject*)NULL, cstart, cstop, py_start, py_stop, py_slice, has_cstart, has_cstop, wraparound)
 static CYTHON_INLINE int __Pyx_PyObject_SetSlice(
@@ -1590,17 +1732,14 @@
         PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
         int has_cstart, int has_cstop, int wraparound);
 
 /* PyObjectFormatAndDecref.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatSimpleAndDecref(PyObject* s, PyObject* f);
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FormatAndDecref(PyObject* s, PyObject* f);
 
-/* IncludeStringH.proto */
-#include <string.h>
-
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* None.proto */
@@ -1949,15 +2088,15 @@
 static const char __pyx_k_OPT[] = "OPT";
 static const char __pyx_k_PLS[] = "PLS";
 static const char __pyx_k_RGX[] = "RGX";
 static const char __pyx_k_RUL[] = "RUL";
 static const char __pyx_k_SEQ[] = "SEQ";
 static const char __pyx_k_STR[] = "STR";
 static const char __pyx_k_SYM[] = "SYM";
-static const char __pyx_k__43[] = "_";
+static const char __pyx_k__49[] = "_";
 static const char __pyx_k_and[] = "_and";
 static const char __pyx_k_bnd[] = "_bnd";
 static const char __pyx_k_cap[] = "_cap";
 static const char __pyx_k_chc[] = "_chc";
 static const char __pyx_k_cls[] = "_cls";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_dot[] = "_dot";
@@ -2118,20 +2257,20 @@
 static const char __pyx_k_pyx_unpickle_Scanner[] = "__pyx_unpickle_Scanner";
 static const char __pyx_k_pyx_unpickle__Parser[] = "__pyx_unpickle__Parser";
 static const char __pyx_k_init___locals_genexpr[] = "__init__.<locals>.genexpr";
 static const char __pyx_k_MachineParser___contains[] = "MachineParser.__contains__";
 static const char __pyx_k_pyx_unpickle_Instruction[] = "__pyx_unpickle_Instruction";
 static const char __pyx_k_pyx_unpickle_CharacterClass[] = "__pyx_unpickle_CharacterClass";
 static const char __pyx_k_PEG_Parsing_Machine_Inspired_by[] = "\nPEG Parsing Machine\n\nInspired by Medeiros and Ierusalimschy, 2008, \"A Parsing Machine for PEGs\"\n\n";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x1b[] = "Incompatible checksums (%s vs 0x1bd4b7a = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x2d[] = "Incompatible checksums (%s vs 0x2d3b4f6 = (action, capturing, marking, name, opcode, oploc, scanner))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x69[] = "Incompatible checksums (%s vs 0x69ecbea = (_regex))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x72[] = "Incompatible checksums (%s vs 0x72ab8af = (pi))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xd4[] = "Incompatible checksums (%s vs 0xd41d8cd = ())";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xf4[] = "Incompatible checksums (%s vs 0xf4951bf = (_x, _xlen))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0x2d3b4f6, 0x74ff7a4, 0x922105f) = (action, capturing, marking, name, opcode, oploc, scanner))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_3[] = "Incompatible checksums (0x%x vs (0x72ab8af, 0x85b42e1, 0xb02e5b6) = (pi))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_4[] = "Incompatible checksums (0x%x vs (0xf4951bf, 0xbcfcf82, 0x8b14fe1) = (_x, _xlen))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_5[] = "Incompatible checksums (0x%x vs (0x1bd4b7a, 0xb19f84c, 0x593b1c1) = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_6[] = "Incompatible checksums (0x%x vs (0x69ecbea, 0xe094a6e, 0x13156fa) = (_regex))";
 static PyObject *__pyx_n_s_AND;
 static PyObject *__pyx_n_s_Action;
 static PyObject *__pyx_n_s_Any;
 static PyObject *__pyx_n_s_BND;
 static PyObject *__pyx_n_s_Bind;
 static PyObject *__pyx_n_s_Binding;
 static PyObject *__pyx_n_s_CAP;
@@ -2142,20 +2281,20 @@
 static PyObject *__pyx_n_s_DOT;
 static PyObject *__pyx_n_s_Dict;
 static PyObject *__pyx_n_s_Dot;
 static PyObject *__pyx_n_s_Error;
 static PyObject *__pyx_n_s_Flag;
 static PyObject *__pyx_n_s_Grammar;
 static PyObject *__pyx_n_s_INLINE;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x1b;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x2d;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x69;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x72;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xd4;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xf4;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_5;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_6;
 static PyObject *__pyx_n_s_Index;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_n_s_Instruction;
 static PyObject *__pyx_n_s_IntEnum;
 static PyObject *__pyx_n_s_KeyError;
 static PyObject *__pyx_n_s_LIT;
 static PyObject *__pyx_n_s_List;
@@ -2187,15 +2326,15 @@
 static PyObject *__pyx_n_s_STR;
 static PyObject *__pyx_n_s_SYM;
 static PyObject *__pyx_n_s_Scanner;
 static PyObject *__pyx_n_s_Tuple;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_Union;
 static PyObject *__pyx_kp_u__2;
-static PyObject *__pyx_n_s__43;
+static PyObject *__pyx_n_s__49;
 static PyObject *__pyx_n_s_action;
 static PyObject *__pyx_n_s_and;
 static PyObject *__pyx_n_s_append;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_bnd;
 static PyObject *__pyx_n_s_cap;
 static PyObject *__pyx_n_s_captured_choice;
@@ -2410,25 +2549,40 @@
 static PyObject *__pyx_tp_new_2pe_11_cy_machine_Regex(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct____init__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_2_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
+static PyObject *__pyx_int_20010746;
 static PyObject *__pyx_int_29182842;
 static PyObject *__pyx_int_47428854;
+static PyObject *__pyx_int_93565377;
 static PyObject *__pyx_int_111070186;
 static PyObject *__pyx_int_120240303;
+static PyObject *__pyx_int_122681252;
+static PyObject *__pyx_int_140198625;
+static PyObject *__pyx_int_145838049;
+static PyObject *__pyx_int_153227359;
+static PyObject *__pyx_int_184739254;
+static PyObject *__pyx_int_186251340;
+static PyObject *__pyx_int_198168450;
 static PyObject *__pyx_int_222419149;
+static PyObject *__pyx_int_228825662;
+static PyObject *__pyx_int_235489902;
+static PyObject *__pyx_int_238750788;
 static PyObject *__pyx_int_256463295;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_slice_;
 static PyObject *__pyx_tuple__3;
+static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__21;
@@ -2438,26 +2592,26 @@
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__35;
 static PyObject *__pyx_tuple__37;
 static PyObject *__pyx_tuple__39;
 static PyObject *__pyx_tuple__41;
-static PyObject *__pyx_tuple__44;
-static PyObject *__pyx_tuple__46;
-static PyObject *__pyx_tuple__48;
+static PyObject *__pyx_tuple__43;
+static PyObject *__pyx_tuple__45;
+static PyObject *__pyx_tuple__47;
 static PyObject *__pyx_tuple__50;
 static PyObject *__pyx_tuple__52;
 static PyObject *__pyx_tuple__54;
 static PyObject *__pyx_tuple__56;
 static PyObject *__pyx_tuple__58;
 static PyObject *__pyx_tuple__60;
-static PyObject *__pyx_codeobj__4;
-static PyObject *__pyx_codeobj__6;
-static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_tuple__62;
+static PyObject *__pyx_tuple__64;
+static PyObject *__pyx_tuple__66;
 static PyObject *__pyx_codeobj__10;
 static PyObject *__pyx_codeobj__12;
 static PyObject *__pyx_codeobj__14;
 static PyObject *__pyx_codeobj__16;
 static PyObject *__pyx_codeobj__18;
 static PyObject *__pyx_codeobj__20;
 static PyObject *__pyx_codeobj__22;
@@ -2467,23 +2621,26 @@
 static PyObject *__pyx_codeobj__30;
 static PyObject *__pyx_codeobj__32;
 static PyObject *__pyx_codeobj__34;
 static PyObject *__pyx_codeobj__36;
 static PyObject *__pyx_codeobj__38;
 static PyObject *__pyx_codeobj__40;
 static PyObject *__pyx_codeobj__42;
-static PyObject *__pyx_codeobj__45;
-static PyObject *__pyx_codeobj__47;
-static PyObject *__pyx_codeobj__49;
+static PyObject *__pyx_codeobj__44;
+static PyObject *__pyx_codeobj__46;
+static PyObject *__pyx_codeobj__48;
 static PyObject *__pyx_codeobj__51;
 static PyObject *__pyx_codeobj__53;
 static PyObject *__pyx_codeobj__55;
 static PyObject *__pyx_codeobj__57;
 static PyObject *__pyx_codeobj__59;
 static PyObject *__pyx_codeobj__61;
+static PyObject *__pyx_codeobj__63;
+static PyObject *__pyx_codeobj__65;
+static PyObject *__pyx_codeobj__67;
 /* Late includes */
 
 /* "pe/_cy_machine.pyx":55
  * 
  * 
  * cdef State* push(             # <<<<<<<<<<<<<<
  *     int opidx,
@@ -3380,15 +3537,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Scanner, (type(self), 0xd41d8cd, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Scanner__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Scanner__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Scanner, (type(self), 0xd41d8cd, state)
@@ -4292,15 +4449,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 106, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -4658,15 +4815,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Instruction, (type(self), 0x2d3b4f6, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Instruction__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Instruction__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Instruction, (type(self), 0x2d3b4f6, state)
@@ -7955,15 +8112,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle__Parser, (type(self), 0x72ab8af, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle__Parser__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_2pe_11_cy_machine___pyx_unpickle__Parser__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle__Parser, (type(self), 0x72ab8af, state)
@@ -12277,15 +12434,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Dot, (type(self), 0xd41d8cd, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Dot__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Dot__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Dot, (type(self), 0xd41d8cd, state)
@@ -12790,15 +12947,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Literal, (type(self), 0xf4951bf, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Literal__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Literal__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Literal, (type(self), 0xf4951bf, state)
@@ -14233,15 +14390,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_CharacterClass, (type(self), 0x1bd4b7a, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_CharacterClass__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_CharacterClass__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_CharacterClass, (type(self), 0x1bd4b7a, state)
@@ -14814,15 +14971,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Regex, (type(self), 0x69ecbea, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Regex__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Regex__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Regex, (type(self), 0x69ecbea, state)
@@ -14926,151 +15083,155 @@
 }
 
 static PyObject *__pyx_pf_2pe_11_cy_machine_36__pyx_unpickle_Scanner(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Scanner", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xd41d8cd) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = Scanner.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Scanner.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = Scanner.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Scanner__set_state(<Scanner> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Scanner), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Scanner), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = Scanner.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Scanner__set_state(<Scanner> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Scanner.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Scanner__set_state(<Scanner> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Scanner__set_state(Scanner __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Scanner__set_state(((struct __pyx_obj_2pe_11_cy_machine_Scanner *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Scanner__set_state(((struct __pyx_obj_2pe_11_cy_machine_Scanner *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = Scanner.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Scanner__set_state(<Scanner> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -15090,18 +15251,18 @@
  * def __pyx_unpickle_Scanner(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("pe._cy_machine.__pyx_unpickle_Scanner", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -15304,151 +15465,155 @@
 }
 
 static PyObject *__pyx_pf_2pe_11_cy_machine_38__pyx_unpickle_Instruction(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Instruction", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x2d3b4f6:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x2d3b4f6, 0x74ff7a4, 0x922105f):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2d3b4f6 = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2d3b4f6, 0x74ff7a4, 0x922105f) = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x2d3b4f6) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__4, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x2d3b4f6:
+ *     if __pyx_checksum not in (0x2d3b4f6, 0x74ff7a4, 0x922105f):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2d3b4f6 = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2d3b4f6, 0x74ff7a4, 0x922105f) = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
  *     __pyx_result = Instruction.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x2d3b4f6:
+ *     if __pyx_checksum not in (0x2d3b4f6, 0x74ff7a4, 0x922105f):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2d3b4f6 = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2d3b4f6, 0x74ff7a4, 0x922105f) = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Instruction.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x2d, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x2d3b4f6:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x2d3b4f6, 0x74ff7a4, 0x922105f):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2d3b4f6 = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2d3b4f6, 0x74ff7a4, 0x922105f) = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2d3b4f6 = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2d3b4f6, 0x74ff7a4, 0x922105f) = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
  *     __pyx_result = Instruction.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Instruction__set_state(<Instruction> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2d3b4f6 = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2d3b4f6, 0x74ff7a4, 0x922105f) = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
  *     __pyx_result = Instruction.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Instruction__set_state(<Instruction> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Instruction.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Instruction__set_state(<Instruction> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Instruction__set_state(Instruction __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Instruction__set_state(((struct __pyx_obj_2pe_11_cy_machine_Instruction *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Instruction__set_state(((struct __pyx_obj_2pe_11_cy_machine_Instruction *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x2d3b4f6 = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x2d3b4f6, 0x74ff7a4, 0x922105f) = (action, capturing, marking, name, opcode, oploc, scanner))" % __pyx_checksum)
  *     __pyx_result = Instruction.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Instruction__set_state(<Instruction> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -15468,18 +15633,18 @@
  * def __pyx_unpickle_Instruction(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("pe._cy_machine.__pyx_unpickle_Instruction", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -15550,15 +15715,15 @@
   __pyx_v___pyx_result->marking = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->name);
   __Pyx_DECREF(__pyx_v___pyx_result->name);
   __pyx_v___pyx_result->name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
@@ -15763,151 +15928,155 @@
 }
 
 static PyObject *__pyx_pf_2pe_11_cy_machine_40__pyx_unpickle__Parser(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle__Parser", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x72ab8af:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x72ab8af, 0x85b42e1, 0xb02e5b6):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x72ab8af = (pi))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x72ab8af, 0x85b42e1, 0xb02e5b6) = (pi))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x72ab8af) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__5, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x72ab8af:
+ *     if __pyx_checksum not in (0x72ab8af, 0x85b42e1, 0xb02e5b6):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x72ab8af = (pi))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x72ab8af, 0x85b42e1, 0xb02e5b6) = (pi))" % __pyx_checksum)
  *     __pyx_result = _Parser.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x72ab8af:
+ *     if __pyx_checksum not in (0x72ab8af, 0x85b42e1, 0xb02e5b6):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x72ab8af = (pi))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x72ab8af, 0x85b42e1, 0xb02e5b6) = (pi))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = _Parser.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x72, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x72ab8af:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x72ab8af, 0x85b42e1, 0xb02e5b6):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x72ab8af = (pi))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x72ab8af, 0x85b42e1, 0xb02e5b6) = (pi))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x72ab8af = (pi))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x72ab8af, 0x85b42e1, 0xb02e5b6) = (pi))" % __pyx_checksum)
  *     __pyx_result = _Parser.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle__Parser__set_state(<_Parser> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine__Parser), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine__Parser), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x72ab8af = (pi))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x72ab8af, 0x85b42e1, 0xb02e5b6) = (pi))" % __pyx_checksum)
  *     __pyx_result = _Parser.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle__Parser__set_state(<_Parser> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = _Parser.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle__Parser__set_state(<_Parser> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle__Parser__set_state(_Parser __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_2pe_11_cy_machine___pyx_unpickle__Parser__set_state(((struct __pyx_obj_2pe_11_cy_machine__Parser *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_2pe_11_cy_machine___pyx_unpickle__Parser__set_state(((struct __pyx_obj_2pe_11_cy_machine__Parser *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x72ab8af = (pi))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x72ab8af, 0x85b42e1, 0xb02e5b6) = (pi))" % __pyx_checksum)
  *     __pyx_result = _Parser.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle__Parser__set_state(<_Parser> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -15927,18 +16096,18 @@
  * def __pyx_unpickle__Parser(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("pe._cy_machine.__pyx_unpickle__Parser", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -15978,15 +16147,15 @@
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (!(likely(PyList_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "list", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->pi);
   __Pyx_DECREF(__pyx_v___pyx_result->pi);
   __pyx_v___pyx_result->pi = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "(tree fragment)":13
@@ -16161,151 +16330,155 @@
 }
 
 static PyObject *__pyx_pf_2pe_11_cy_machine_42__pyx_unpickle_Dot(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Dot", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xd41d8cd) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = Dot.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xd41d8cd:
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Dot.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd41d8cd:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = Dot.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Dot__set_state(<Dot> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Dot), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Dot), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = Dot.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Dot__set_state(<Dot> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Dot.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Dot__set_state(<Dot> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Dot__set_state(Dot __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Dot__set_state(((struct __pyx_obj_2pe_11_cy_machine_Dot *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Dot__set_state(((struct __pyx_obj_2pe_11_cy_machine_Dot *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd41d8cd = ())" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
  *     __pyx_result = Dot.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Dot__set_state(<Dot> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -16325,18 +16498,18 @@
  * def __pyx_unpickle_Dot(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("pe._cy_machine.__pyx_unpickle_Dot", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -16539,151 +16712,155 @@
 }
 
 static PyObject *__pyx_pf_2pe_11_cy_machine_44__pyx_unpickle_Literal(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Literal", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf4951bf:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xf4951bf, 0xbcfcf82, 0x8b14fe1):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf4951bf = (_x, _xlen))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf4951bf, 0xbcfcf82, 0x8b14fe1) = (_x, _xlen))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xf4951bf) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__6, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf4951bf:
+ *     if __pyx_checksum not in (0xf4951bf, 0xbcfcf82, 0x8b14fe1):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf4951bf = (_x, _xlen))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf4951bf, 0xbcfcf82, 0x8b14fe1) = (_x, _xlen))" % __pyx_checksum)
  *     __pyx_result = Literal.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xf4951bf:
+ *     if __pyx_checksum not in (0xf4951bf, 0xbcfcf82, 0x8b14fe1):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf4951bf = (_x, _xlen))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf4951bf, 0xbcfcf82, 0x8b14fe1) = (_x, _xlen))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Literal.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xf4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xf4951bf:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xf4951bf, 0xbcfcf82, 0x8b14fe1):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf4951bf = (_x, _xlen))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf4951bf, 0xbcfcf82, 0x8b14fe1) = (_x, _xlen))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf4951bf = (_x, _xlen))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf4951bf, 0xbcfcf82, 0x8b14fe1) = (_x, _xlen))" % __pyx_checksum)
  *     __pyx_result = Literal.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Literal__set_state(<Literal> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Literal), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Literal), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf4951bf = (_x, _xlen))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf4951bf, 0xbcfcf82, 0x8b14fe1) = (_x, _xlen))" % __pyx_checksum)
  *     __pyx_result = Literal.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Literal__set_state(<Literal> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Literal.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Literal__set_state(<Literal> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Literal__set_state(Literal __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Literal__set_state(((struct __pyx_obj_2pe_11_cy_machine_Literal *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Literal__set_state(((struct __pyx_obj_2pe_11_cy_machine_Literal *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xf4951bf = (_x, _xlen))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xf4951bf, 0xbcfcf82, 0x8b14fe1) = (_x, _xlen))" % __pyx_checksum)
  *     __pyx_result = Literal.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Literal__set_state(<Literal> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -16703,18 +16880,18 @@
  * def __pyx_unpickle_Literal(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("pe._cy_machine.__pyx_unpickle_Literal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -16755,15 +16932,15 @@
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->_x);
   __Pyx_DECREF(__pyx_v___pyx_result->_x);
   __pyx_v___pyx_result->_x = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
@@ -16947,151 +17124,155 @@
 }
 
 static PyObject *__pyx_pf_2pe_11_cy_machine_46__pyx_unpickle_CharacterClass(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_CharacterClass", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x1bd4b7a:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x1bd4b7a, 0xb19f84c, 0x593b1c1):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x1bd4b7a = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1bd4b7a, 0xb19f84c, 0x593b1c1) = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x1bd4b7a) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__7, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x1bd4b7a:
+ *     if __pyx_checksum not in (0x1bd4b7a, 0xb19f84c, 0x593b1c1):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x1bd4b7a = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1bd4b7a, 0xb19f84c, 0x593b1c1) = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
  *     __pyx_result = CharacterClass.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x1bd4b7a:
+ *     if __pyx_checksum not in (0x1bd4b7a, 0xb19f84c, 0x593b1c1):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x1bd4b7a = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1bd4b7a, 0xb19f84c, 0x593b1c1) = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = CharacterClass.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x1b, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_5, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x1bd4b7a:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x1bd4b7a, 0xb19f84c, 0x593b1c1):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x1bd4b7a = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1bd4b7a, 0xb19f84c, 0x593b1c1) = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x1bd4b7a = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1bd4b7a, 0xb19f84c, 0x593b1c1) = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
  *     __pyx_result = CharacterClass.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_CharacterClass__set_state(<CharacterClass> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_CharacterClass), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_CharacterClass), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x1bd4b7a = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1bd4b7a, 0xb19f84c, 0x593b1c1) = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
  *     __pyx_result = CharacterClass.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_CharacterClass__set_state(<CharacterClass> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = CharacterClass.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_CharacterClass__set_state(<CharacterClass> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_CharacterClass__set_state(CharacterClass __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_CharacterClass__set_state(((struct __pyx_obj_2pe_11_cy_machine_CharacterClass *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_CharacterClass__set_state(((struct __pyx_obj_2pe_11_cy_machine_CharacterClass *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x1bd4b7a = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x1bd4b7a, 0xb19f84c, 0x593b1c1) = (_chars, _negate, _rangelen, _ranges, maxcount, mincount))" % __pyx_checksum)
  *     __pyx_result = CharacterClass.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_CharacterClass__set_state(<CharacterClass> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -17111,18 +17292,18 @@
  * def __pyx_unpickle_CharacterClass(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("pe._cy_machine.__pyx_unpickle_CharacterClass", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -17163,15 +17344,15 @@
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->_chars);
   __Pyx_DECREF(__pyx_v___pyx_result->_chars);
   __pyx_v___pyx_result->_chars = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
@@ -17193,15 +17374,15 @@
   __pyx_v___pyx_result->_rangelen = __pyx_t_3;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->_ranges);
   __Pyx_DECREF(__pyx_v___pyx_result->_ranges);
   __pyx_v___pyx_result->_ranges = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
@@ -17394,151 +17575,155 @@
 }
 
 static PyObject *__pyx_pf_2pe_11_cy_machine_48__pyx_unpickle_Regex(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Regex", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x69ecbea:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x69ecbea, 0xe094a6e, 0x13156fa):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x69ecbea = (_regex))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x69ecbea, 0xe094a6e, 0x13156fa) = (_regex))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x69ecbea) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__8, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x69ecbea:
+ *     if __pyx_checksum not in (0x69ecbea, 0xe094a6e, 0x13156fa):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x69ecbea = (_regex))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x69ecbea, 0xe094a6e, 0x13156fa) = (_regex))" % __pyx_checksum)
  *     __pyx_result = Regex.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x69ecbea:
+ *     if __pyx_checksum not in (0x69ecbea, 0xe094a6e, 0x13156fa):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x69ecbea = (_regex))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x69ecbea, 0xe094a6e, 0x13156fa) = (_regex))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Regex.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x69, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_6, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x69ecbea:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x69ecbea, 0xe094a6e, 0x13156fa):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x69ecbea = (_regex))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x69ecbea, 0xe094a6e, 0x13156fa) = (_regex))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x69ecbea = (_regex))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x69ecbea, 0xe094a6e, 0x13156fa) = (_regex))" % __pyx_checksum)
  *     __pyx_result = Regex.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Regex__set_state(<Regex> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Regex), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Regex), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x69ecbea = (_regex))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x69ecbea, 0xe094a6e, 0x13156fa) = (_regex))" % __pyx_checksum)
  *     __pyx_result = Regex.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Regex__set_state(<Regex> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Regex.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Regex__set_state(<Regex> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Regex__set_state(Regex __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Regex__set_state(((struct __pyx_obj_2pe_11_cy_machine_Regex *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_2pe_11_cy_machine___pyx_unpickle_Regex__set_state(((struct __pyx_obj_2pe_11_cy_machine_Regex *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x69ecbea = (_regex))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x69ecbea, 0xe094a6e, 0x13156fa) = (_regex))" % __pyx_checksum)
  *     __pyx_result = Regex.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Regex__set_state(<Regex> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -17558,18 +17743,18 @@
  * def __pyx_unpickle_Regex(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("pe._cy_machine.__pyx_unpickle_Regex", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -17796,20 +17981,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine_Instruction(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_2pe_11_cy_machine_Instruction *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
@@ -18031,20 +18219,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine__Parser __pyx_vtable_2pe_11_cy_machine__Parser;
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine__Parser(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_2pe_11_cy_machine__Parser *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -18153,20 +18344,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_Dot __pyx_vtable_2pe_11_cy_machine_Dot;
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine_Dot(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_2pe_11_cy_machine_Dot *p;
   PyObject *o = __pyx_tp_new_2pe_11_cy_machine_Scanner(t, a, k);
   if (unlikely(!o)) return 0;
@@ -18238,20 +18432,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_Literal __pyx_vtable_2pe_11_cy_machine_Literal;
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine_Literal(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_2pe_11_cy_machine_Literal *p;
   PyObject *o = __pyx_tp_new_2pe_11_cy_machine_Scanner(t, a, k);
   if (unlikely(!o)) return 0;
@@ -18335,20 +18532,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_CharacterClass __pyx_vtable_2pe_11_cy_machine_CharacterClass;
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine_CharacterClass(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_2pe_11_cy_machine_CharacterClass *p;
   PyObject *o = __pyx_tp_new_2pe_11_cy_machine_Scanner(t, a, k);
   if (unlikely(!o)) return 0;
@@ -18468,20 +18668,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_Regex __pyx_vtable_2pe_11_cy_machine_Regex;
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine_Regex(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_2pe_11_cy_machine_Regex *p;
   PyObject *o = __pyx_tp_new_2pe_11_cy_machine_Scanner(t, a, k);
   if (unlikely(!o)) return 0;
@@ -18496,18 +18699,15 @@
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_regex);
-  #if CYTHON_USE_TYPE_SLOTS
-  if (PyType_IS_GC(Py_TYPE(o)->tp_base))
-  #endif
-  PyObject_GC_Track(o);
+  if (PyType_IS_GC(__pyx_ptype_2pe_11_cy_machine_Scanner)) PyObject_GC_Track(o);
   __pyx_tp_dealloc_2pe_11_cy_machine_Scanner(o);
 }
 
 static int __pyx_tp_traverse_2pe_11_cy_machine_Regex(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_2pe_11_cy_machine_Regex *p = (struct __pyx_obj_2pe_11_cy_machine_Regex *)o;
   e = ((likely(__pyx_ptype_2pe_11_cy_machine_Scanner)) ? ((__pyx_ptype_2pe_11_cy_machine_Scanner->tp_traverse) ? __pyx_ptype_2pe_11_cy_machine_Scanner->tp_traverse(o, v, a) : 0) : __Pyx_call_next_tp_traverse(o, v, a, __pyx_tp_traverse_2pe_11_cy_machine_Regex)); if (e) return e;
@@ -18590,20 +18790,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct____init__ *__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct____init__[8];
 static int __pyx_freecount_2pe_11_cy_machine___pyx_scope_struct____init__ = 0;
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct____init__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -18705,20 +18908,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr *__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_1_genexpr = 0;
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -18819,20 +19025,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr *__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_2_genexpr[8];
 static int __pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_2_genexpr = 0;
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_2_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
@@ -18933,20 +19142,23 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -19005,20 +19217,20 @@
   {&__pyx_n_s_DOT, __pyx_k_DOT, sizeof(__pyx_k_DOT), 0, 0, 1, 1},
   {&__pyx_n_s_Dict, __pyx_k_Dict, sizeof(__pyx_k_Dict), 0, 0, 1, 1},
   {&__pyx_n_s_Dot, __pyx_k_Dot, sizeof(__pyx_k_Dot), 0, 0, 1, 1},
   {&__pyx_n_s_Error, __pyx_k_Error, sizeof(__pyx_k_Error), 0, 0, 1, 1},
   {&__pyx_n_s_Flag, __pyx_k_Flag, sizeof(__pyx_k_Flag), 0, 0, 1, 1},
   {&__pyx_n_s_Grammar, __pyx_k_Grammar, sizeof(__pyx_k_Grammar), 0, 0, 1, 1},
   {&__pyx_n_s_INLINE, __pyx_k_INLINE, sizeof(__pyx_k_INLINE), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x1b, __pyx_k_Incompatible_checksums_s_vs_0x1b, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x1b), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x2d, __pyx_k_Incompatible_checksums_s_vs_0x2d, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x2d), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x69, __pyx_k_Incompatible_checksums_s_vs_0x69, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x69), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x72, __pyx_k_Incompatible_checksums_s_vs_0x72, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x72), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_k_Incompatible_checksums_s_vs_0xd4, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xd4), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xf4, __pyx_k_Incompatible_checksums_s_vs_0xf4, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xf4), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_k_Incompatible_checksums_0x_x_vs_0_3, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_3), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4, __pyx_k_Incompatible_checksums_0x_x_vs_0_4, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_4), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_5, __pyx_k_Incompatible_checksums_0x_x_vs_0_5, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_5), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_6, __pyx_k_Incompatible_checksums_0x_x_vs_0_6, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_6), 0, 0, 1, 0},
   {&__pyx_n_s_Index, __pyx_k_Index, sizeof(__pyx_k_Index), 0, 0, 1, 1},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_n_s_Instruction, __pyx_k_Instruction, sizeof(__pyx_k_Instruction), 0, 0, 1, 1},
   {&__pyx_n_s_IntEnum, __pyx_k_IntEnum, sizeof(__pyx_k_IntEnum), 0, 0, 1, 1},
   {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
   {&__pyx_n_s_LIT, __pyx_k_LIT, sizeof(__pyx_k_LIT), 0, 0, 1, 1},
   {&__pyx_n_s_List, __pyx_k_List, sizeof(__pyx_k_List), 0, 0, 1, 1},
@@ -19050,15 +19262,15 @@
   {&__pyx_n_s_STR, __pyx_k_STR, sizeof(__pyx_k_STR), 0, 0, 1, 1},
   {&__pyx_n_s_SYM, __pyx_k_SYM, sizeof(__pyx_k_SYM), 0, 0, 1, 1},
   {&__pyx_n_s_Scanner, __pyx_k_Scanner, sizeof(__pyx_k_Scanner), 0, 0, 1, 1},
   {&__pyx_n_s_Tuple, __pyx_k_Tuple, sizeof(__pyx_k_Tuple), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_Union, __pyx_k_Union, sizeof(__pyx_k_Union), 0, 0, 1, 1},
   {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-  {&__pyx_n_s__43, __pyx_k__43, sizeof(__pyx_k__43), 0, 0, 1, 1},
+  {&__pyx_n_s__49, __pyx_k__49, sizeof(__pyx_k__49), 0, 0, 1, 1},
   {&__pyx_n_s_action, __pyx_k_action, sizeof(__pyx_k_action), 0, 0, 1, 1},
   {&__pyx_n_s_and, __pyx_k_and, sizeof(__pyx_k_and), 0, 0, 1, 1},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_bnd, __pyx_k_bnd, sizeof(__pyx_k_bnd), 0, 0, 1, 1},
   {&__pyx_n_s_cap, __pyx_k_cap, sizeof(__pyx_k_cap), 0, 0, 1, 1},
   {&__pyx_n_s_captured_choice, __pyx_k_captured_choice, sizeof(__pyx_k_captured_choice), 0, 0, 1, 1},
@@ -19215,328 +19427,366 @@
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])
  */
   __pyx_slice_ = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice_);
   __Pyx_GIVEREF(__pyx_slice_);
 
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd41d8cd, 0xe3b0c44, 0xda39a3e) = ())" % __pyx_checksum)
+ */
+  __pyx_tuple__3 = PyTuple_Pack(3, __pyx_int_222419149, __pyx_int_238750788, __pyx_int_228825662); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_47428854, __pyx_int_122681252, __pyx_int_153227359); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_int_120240303, __pyx_int_140198625, __pyx_int_184739254); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__6 = PyTuple_Pack(3, __pyx_int_256463295, __pyx_int_198168450, __pyx_int_145838049); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple__7 = PyTuple_Pack(3, __pyx_int_29182842, __pyx_int_186251340, __pyx_int_93565377); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_111070186, __pyx_int_235489902, __pyx_int_20010746); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+
   /* "pe/_cy_machine.pyx":132
  * class MachineParser(Parser):
  * 
  *     def __init__(self, grammar: Grammar,             # <<<<<<<<<<<<<<
  *                  flags: Flag = Flag.NONE):
  *         super().__init__(grammar, flags=flags)
  */
-  __pyx_tuple__3 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_grammar, __pyx_n_s_flags, __pyx_n_s_pi, __pyx_n_s_index_2); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 132, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_init, 132, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_grammar, __pyx_n_s_flags, __pyx_n_s_pi, __pyx_n_s_index_2); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_init, 132, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 132, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":149
  * 
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         return self.grammar.start
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_start, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_start, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 149, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":152
  *         return self.grammar.start
  * 
  *     def __contains__(self, name: str) -> bool:             # <<<<<<<<<<<<<<
  *         return name in self._index
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_name); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_contains, 152, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_name); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_contains, 152, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 152, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":155
  *         return name in self._index
  * 
  *     def match(self,             # <<<<<<<<<<<<<<
  *               str s,
  *               int pos = 0,
  */
-  __pyx_tuple__9 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_s, __pyx_n_s_pos, __pyx_n_s_flags, __pyx_n_s_memo, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_idx, __pyx_n_s_end); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 155, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(4, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_match, 155, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_s, __pyx_n_s_pos, __pyx_n_s_flags, __pyx_n_s_memo, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_idx, __pyx_n_s_end); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(4, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_match, 155, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 155, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":330
  * 
  * 
  * def _make_program(grammar) -> Tuple[_Program, _Index]:             # <<<<<<<<<<<<<<
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  */
-  __pyx_tuple__11 = PyTuple_Pack(6, __pyx_n_s_grammar, __pyx_n_s_index_2, __pyx_n_s_pis, __pyx_n_s_name, __pyx_n_s_pis_2, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 330, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_make_program, 330, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(6, __pyx_n_s_grammar, __pyx_n_s_index_2, __pyx_n_s_pis, __pyx_n_s_name, __pyx_n_s_pis_2, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_make_program, 330, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 330, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":352
  * 
  * 
  * def _dot(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Dot())]
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 352, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_dot, 352, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_dot, 352, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 352, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":356
  * 
  * 
  * def _lit(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]
  * 
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 356, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_lit, 356, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_lit, 356, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 356, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":360
  * 
  * 
  * def _cls(defn, mincount=1, maxcount=1):             # <<<<<<<<<<<<<<
  *     cclass = CharacterClass(
  *         defn.args[0],
  */
-  __pyx_tuple__17 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_maxcount, __pyx_n_s_cclass); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 360, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cls, 360, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_maxcount, __pyx_n_s_cclass); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cls, 360, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 360, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":370
  * 
  * 
  * def _rgx(defn):             # <<<<<<<<<<<<<<
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  */
-  __pyx_tuple__19 = PyTuple_Pack(3, __pyx_n_s_defn, __pyx_n_s_pat, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 370, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rgx, 370, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(3, __pyx_n_s_defn, __pyx_n_s_pat, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rgx, 370, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 370, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":375
  * 
  * 
  * def _opt(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 375, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_opt, 375, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_opt, 375, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 375, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":382
  * 
  * 
  * def _str(defn): return _rpt(defn, 0)             # <<<<<<<<<<<<<<
  * def _pls(defn): return _rpt(defn, 1)
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 382, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_str, 382, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_str, 382, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 382, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":383
  * 
  * def _str(defn): return _rpt(defn, 0)
  * def _pls(defn): return _rpt(defn, 1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 383, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_pls, 383, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_pls, 383, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 383, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":386
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
-  __pyx_tuple__27 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 386, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rpt, 386, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rpt, 386, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 386, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":408
  * 
  * 
  * def _sym(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(CALL, name=defn.args[0])]
  * 
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 408, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_sym, 408, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_sym, 408, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 408, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":412
  * 
  * 
  * def _and(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_tuple__31 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 412, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_and, 412, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_and, 412, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 412, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":420
  * 
  * 
  * def _not(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_tuple__33 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_not, 420, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_not, 420, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 420, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":427
  * 
  * 
  * def _cap(defn):             # <<<<<<<<<<<<<<
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  */
-  __pyx_tuple__35 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_captured_choice, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 427, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cap, 427, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_captured_choice, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cap, 427, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 427, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":446
  * 
  * 
  * def _bnd(defn):             # <<<<<<<<<<<<<<
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))
  * 
  */
-  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 446, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_bnd, 446, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_bnd, 446, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 446, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":450
  * 
  * 
  * def _seq(defn):             # <<<<<<<<<<<<<<
  *     head = [pi
  *             for d in defn.args[0][:-1]
  */
-  __pyx_tuple__39 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_head, __pyx_n_s_tail, __pyx_n_s_d, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 450, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__39);
-  __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_seq, 450, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_head, __pyx_n_s_tail, __pyx_n_s_d, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__45);
+  __Pyx_GIVEREF(__pyx_tuple__45);
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_seq, 450, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 450, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":458
  * 
  * 
  * def _chc(defn):             # <<<<<<<<<<<<<<
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  */
-  __pyx_tuple__41 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_pis, __pyx_n_s_pi, __pyx_n_s_pi_2, __pyx_n_s_d); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 458, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__41);
-  __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_chc, 458, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_pis, __pyx_n_s_pi, __pyx_n_s_pi_2, __pyx_n_s_d); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__47);
+  __Pyx_GIVEREF(__pyx_tuple__47);
+  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_chc, 458, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 458, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":469
  * 
  * 
  * def _rul(defn):             # <<<<<<<<<<<<<<
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  */
-  __pyx_tuple__44 = PyTuple_Pack(6, __pyx_n_s_defn, __pyx_n_s_subdefn, __pyx_n_s_action, __pyx_n_s__43, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 469, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__44);
-  __Pyx_GIVEREF(__pyx_tuple__44);
-  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rul, 469, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_tuple__50 = PyTuple_Pack(6, __pyx_n_s_defn, __pyx_n_s_subdefn, __pyx_n_s_action, __pyx_n_s__49, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__50);
+  __Pyx_GIVEREF(__pyx_tuple__50);
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rul, 469, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 469, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":506
  * 
  * 
  * def _parsing_instructions(defn):  # noqa: C901             # <<<<<<<<<<<<<<
  *     try:
  *         return _op_map[defn.op](defn)
  */
-  __pyx_tuple__46 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 506, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__46);
-  __Pyx_GIVEREF(__pyx_tuple__46);
-  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_parsing_instructions, 506, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__52);
+  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_parsing_instructions, 506, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 506, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Scanner(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__48 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__48);
-  __Pyx_GIVEREF(__pyx_tuple__48);
-  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Scanner, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__50 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__50);
-  __Pyx_GIVEREF(__pyx_tuple__50);
-  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Instruction, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__52 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__52);
-  __Pyx_GIVEREF(__pyx_tuple__52);
-  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle__Parser, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__54 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__54);
   __Pyx_GIVEREF(__pyx_tuple__54);
-  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Dot, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Scanner, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__56 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__56);
   __Pyx_GIVEREF(__pyx_tuple__56);
-  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Literal, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Instruction, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__58 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__58);
   __Pyx_GIVEREF(__pyx_tuple__58);
-  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CharacterClass, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle__Parser, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__60 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__60);
   __Pyx_GIVEREF(__pyx_tuple__60);
-  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Regex, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Dot, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__62 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__62);
+  __Pyx_GIVEREF(__pyx_tuple__62);
+  __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__62, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Literal, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__64 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__64);
+  __Pyx_GIVEREF(__pyx_tuple__64);
+  __pyx_codeobj__65 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CharacterClass, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__65)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__66 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__66);
+  __Pyx_GIVEREF(__pyx_tuple__66);
+  __pyx_codeobj__67 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Regex, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__67)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 2, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_20010746 = PyInt_FromLong(20010746L); if (unlikely(!__pyx_int_20010746)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_29182842 = PyInt_FromLong(29182842L); if (unlikely(!__pyx_int_29182842)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_47428854 = PyInt_FromLong(47428854L); if (unlikely(!__pyx_int_47428854)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_93565377 = PyInt_FromLong(93565377L); if (unlikely(!__pyx_int_93565377)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_111070186 = PyInt_FromLong(111070186L); if (unlikely(!__pyx_int_111070186)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_120240303 = PyInt_FromLong(120240303L); if (unlikely(!__pyx_int_120240303)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_122681252 = PyInt_FromLong(122681252L); if (unlikely(!__pyx_int_122681252)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_140198625 = PyInt_FromLong(140198625L); if (unlikely(!__pyx_int_140198625)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_145838049 = PyInt_FromLong(145838049L); if (unlikely(!__pyx_int_145838049)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_153227359 = PyInt_FromLong(153227359L); if (unlikely(!__pyx_int_153227359)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_184739254 = PyInt_FromLong(184739254L); if (unlikely(!__pyx_int_184739254)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_186251340 = PyInt_FromLong(186251340L); if (unlikely(!__pyx_int_186251340)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_198168450 = PyInt_FromLong(198168450L); if (unlikely(!__pyx_int_198168450)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_222419149 = PyInt_FromLong(222419149L); if (unlikely(!__pyx_int_222419149)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_228825662 = PyInt_FromLong(228825662L); if (unlikely(!__pyx_int_228825662)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_235489902 = PyInt_FromLong(235489902L); if (unlikely(!__pyx_int_235489902)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_int_238750788 = PyInt_FromLong(238750788L); if (unlikely(!__pyx_int_238750788)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_256463295 = PyInt_FromLong(256463295L); if (unlikely(!__pyx_int_256463295)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -19901,15 +20151,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 2, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 2, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 2, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 2, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pe___cy_machine) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
@@ -20346,15 +20596,15 @@
   /* "pe/_cy_machine.pyx":132
  * class MachineParser(Parser):
  * 
  *     def __init__(self, grammar: Grammar,             # <<<<<<<<<<<<<<
  *                  flags: Flag = Flag.NONE):
  *         super().__init__(grammar, flags=flags)
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_1__init__, 0, __pyx_n_s_MachineParser___init, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_1__init__, 0, __pyx_n_s_MachineParser___init, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_t_6);
   PyList_Append(__pyx_t_4, __pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_6);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_6, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 132, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":133
@@ -20381,15 +20631,15 @@
   /* "pe/_cy_machine.pyx":149
  * 
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         return self.grammar.start
  * 
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_3start, 0, __pyx_n_s_MachineParser_start, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_3start, 0, __pyx_n_s_MachineParser_start, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
   /* "pe/_cy_machine.pyx":148
  *         self._index = index
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def start(self):
@@ -20408,15 +20658,15 @@
  *         return name in self._index
  * 
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_name, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_5__contains__, 0, __pyx_n_s_MachineParser___contains, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_5__contains__, 0, __pyx_n_s_MachineParser___contains, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_contains, __pyx_t_6) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "pe/_cy_machine.pyx":155
@@ -20462,15 +20712,15 @@
   /* "pe/_cy_machine.pyx":155
  *         return name in self._index
  * 
  *     def match(self,             # <<<<<<<<<<<<<<
  *               str s,
  *               int pos = 0,
  */
-  __pyx_t_8 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_7match, 0, __pyx_n_s_MachineParser_match, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_7match, 0, __pyx_n_s_MachineParser_match, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_8, sizeof(__pyx_defaults1), 1)) __PYX_ERR(0, 155, __pyx_L1_error)
 
   /* "pe/_cy_machine.pyx":158
  *               str s,
  *               int pos = 0,
  *               flags: Flag = Flag.NONE) -> Union[Match, None]:             # <<<<<<<<<<<<<<
@@ -21667,28 +21917,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -22116,18 +22366,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
@@ -22212,15 +22460,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -22342,15 +22590,15 @@
         uval = NULL;
         if (uoffset > 0) {
             prepend_sign = !!prepend_sign;
             if (uoffset > prepend_sign) {
                 padding = PyUnicode_FromOrdinal(padding_char);
                 if (likely(padding) && uoffset > prepend_sign + 1) {
                     PyObject *tmp;
-                    PyObject *repeat = PyInt_FromSize_t(uoffset - prepend_sign);
+                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
                     if (unlikely(!repeat)) goto done_or_error;
                     tmp = PyNumber_Multiply(padding, repeat);
                     Py_DECREF(repeat);
                     Py_DECREF(padding);
                     padding = tmp;
                 }
                 if (unlikely(!padding)) goto done_or_error;
@@ -22376,25 +22624,14 @@
         Py_XDECREF(sign);
     }
 #endif
     return uval;
 }
 
 /* CIntToPyUnicode */
-#ifdef _MSC_VER
-    #ifndef _MSC_STDINT_H_
-        #if _MSC_VER < 1300
-           typedef unsigned short    uint16_t;
-        #else
-           typedef unsigned __int16  uint16_t;
-        #endif
-    #endif
-#else
-   #include <stdint.h>
-#endif
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_enum____pyx_t_2pe_11_cy_machine_OpCode(enum __pyx_t_2pe_11_cy_machine_OpCode value, Py_ssize_t width, char padding_char, char format_char) {
     char digits[sizeof(enum __pyx_t_2pe_11_cy_machine_OpCode)*3+2];
     char *dpos, *end = digits + sizeof(enum __pyx_t_2pe_11_cy_machine_OpCode)*3+2;
     const char *hex_digits = DIGITS_HEX;
     Py_ssize_t length, ulength;
     int prepend_sign, last_one_off;
     enum __pyx_t_2pe_11_cy_machine_OpCode remaining;
@@ -22417,22 +22654,22 @@
     do {
         int digit_pos;
         switch (format_char) {
         case 'o':
             digit_pos = abs((int)(remaining % (8*8)));
             remaining = (enum __pyx_t_2pe_11_cy_machine_OpCode) (remaining / (8*8));
             dpos -= 2;
-            *(uint16_t*)dpos = ((const uint16_t*)DIGIT_PAIRS_8)[digit_pos];
+            memcpy(dpos, DIGIT_PAIRS_8 + digit_pos * 2, 2);
             last_one_off = (digit_pos < 8);
             break;
         case 'd':
             digit_pos = abs((int)(remaining % (10*10)));
             remaining = (enum __pyx_t_2pe_11_cy_machine_OpCode) (remaining / (10*10));
             dpos -= 2;
-            *(uint16_t*)dpos = ((const uint16_t*)DIGIT_PAIRS_10)[digit_pos];
+            memcpy(dpos, DIGIT_PAIRS_10 + digit_pos * 2, 2);
             last_one_off = (digit_pos < 10);
             break;
         case 'x':
             *(--dpos) = hex_digits[abs((int)(remaining % 16))];
             remaining = (enum __pyx_t_2pe_11_cy_machine_OpCode) (remaining / 16);
             break;
         default:
@@ -22651,15 +22888,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -22952,15 +23189,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -23335,25 +23572,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
+#if CYTHON_USE_PYTYPE_LOOKUP
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
+#else
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
+#endif
+    if (getstate) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
 #endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -23390,14 +23645,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -23974,14 +24231,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -24042,20 +24307,26 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
@@ -24185,15 +24456,15 @@
 #endif
     }
     return 0;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -24215,15 +24486,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -24309,41 +24580,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -24354,34 +24632,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -24579,15 +24872,15 @@
                         } else if (8 * sizeof(enum __pyx_t_2pe_11_cy_machine_OpCode) >= 4 * PyLong_SHIFT) {
                             return (enum __pyx_t_2pe_11_cy_machine_OpCode) (((((((((enum __pyx_t_2pe_11_cy_machine_OpCode)digits[3]) << PyLong_SHIFT) | (enum __pyx_t_2pe_11_cy_machine_OpCode)digits[2]) << PyLong_SHIFT) | (enum __pyx_t_2pe_11_cy_machine_OpCode)digits[1]) << PyLong_SHIFT) | (enum __pyx_t_2pe_11_cy_machine_OpCode)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24813,15 +25106,15 @@
                         } else if (8 * sizeof(short) >= 4 * PyLong_SHIFT) {
                             return (short) (((((((((short)digits[3]) << PyLong_SHIFT) | (short)digits[2]) << PyLong_SHIFT) | (short)digits[1]) << PyLong_SHIFT) | (short)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25047,15 +25340,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25243,15 +25536,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25520,14 +25813,20 @@
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CoroutineBase */
 #include <structmember.h>
 #include <frameobject.h>
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 #define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
 static int __Pyx_PyGen__FetchStopIterationValue(CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject **pvalue) {
     PyObject *et, *ev, *tb;
     PyObject *value = NULL;
     __Pyx_ErrFetch(&et, &ev, &tb);
     if (!et) {
         Py_XDECREF(tb);
@@ -25691,17 +25990,21 @@
     exc_state = &self->gi_exc_state;
     if (exc_state->exc_type) {
         #if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_PYSTON
         #else
         if (exc_state->exc_traceback) {
             PyTracebackObject *tb = (PyTracebackObject *) exc_state->exc_traceback;
             PyFrameObject *f = tb->tb_frame;
-            Py_XINCREF(tstate->frame);
             assert(f->f_back == NULL);
+            #if PY_VERSION_HEX >= 0x030B00A1
+            f->f_back = PyThreadState_GetFrame(tstate);
+            #else
+            Py_XINCREF(tstate->frame);
             f->f_back = tstate->frame;
+            #endif
         }
         #endif
     }
 #if CYTHON_USE_EXC_INFO_STACK
     exc_state->previous_item = tstate->exc_info;
     tstate->exc_info = exc_state;
 #else
@@ -26481,38 +26784,66 @@
 #endif
     0,
 #if CYTHON_USE_TP_FINALIZE
     __Pyx_Coroutine_del,
 #elif PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
     if (unlikely(!__pyx_GeneratorType)) {
         return -1;
     }
     return 0;
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -26762,14 +27093,31 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `pe-0.3.2/pe/_cy_machine.pyx` & `pe-0.4.0/pe/_cy_machine.pyx`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/_debug.py` & `pe-0.4.0/pe/_debug.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/_definition.py` & `pe-0.4.0/pe/_definition.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/_errors.py` & `pe-0.4.0/pe/_errors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 
+from typing import Optional
+
+
 class Error(Exception):
     """Exception raised for invalid parsing expressions."""
 
 
 class GrammarWarning(Warning):
     pass
 
@@ -10,31 +13,31 @@
 class GrammarError(Error):
     pass
 
 
 class ParseError(Error):
 
     def __init__(self,
-                 message: str = None,
-                 filename: str = None,
-                 lineno: int = None,
-                 offset: int = None,
-                 text: str = None):
+                 message: Optional[str] = None,
+                 filename: Optional[str] = None,
+                 lineno: Optional[int] = None,
+                 offset: Optional[int] = None,
+                 text: Optional[str] = None):
         self.message = message
         self.filename = filename
         self.lineno = lineno
         self.offset = offset
         self.text = text
 
     @classmethod
     def from_pos(cls,
                  pos: int,
                  text: str,
-                 message: str = None,
-                 filename: str = None):
+                 message: Optional[str] = None,
+                 filename: Optional[str] = None):
         """Instantiate from a full *text* and a file position *pos*"""
 
         # this method should work for \n and \r\n newline sequences, which
         # I assume covers all potential users
         try:
             start = text.rindex('\n', 0, pos) + 1
         except ValueError:
```

### Comparing `pe-0.3.2/pe/_escape.py` & `pe-0.4.0/pe/_escape.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/_functions.py` & `pe-0.4.0/pe/_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 
-from typing import Union, Dict, Callable
+from typing import Union, Dict, Callable, Optional
 
+from pe.actions import Action
 from pe._constants import Flag
 from pe._errors import Error
 from pe._parser import Parser
 from pe._grammar import Grammar
 from pe._parse import loads
 
+_FuncMap = Dict[str, Union[Action, Callable]]
+
 
 def compile(source: Union[str, Grammar],
-            actions: Dict[str, Callable] = None,
+            actions: Optional[_FuncMap] = None,
             parser: str = 'packrat',
             flags: Flag = Flag.OPTIMIZE) -> Parser:
     """Compile the parsing expression or grammar in *source*."""
     parsername = parser.lower()
     if parsername == 'packrat':
         from pe.packrat import PackratParser as parser_class
     elif parsername == 'machine':
@@ -43,15 +46,15 @@
         print(p.modified_grammar)
 
     return p
 
 
 def match(pattern: str,
           string: str,
-          actions: Dict[str, Callable] = None,
+          actions: Optional[_FuncMap] = None,
           parser: str = 'packrat',
           flags: Flag = Flag.MEMOIZE):
     """Compile *pattern* and match *string* against it.
 
     Example:
         >>> import pe
         >>> pe.match(r'"-"? [1-9] [0-9]*', '-12345').group()
```

### Comparing `pe-0.3.2/pe/_grammar.py` & `pe-0.4.0/pe/_grammar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 
-from typing import Dict, Callable
+from typing import Union, Dict, Callable, Optional
 
+from pe.actions import Action
 from pe._constants import Operator
 from pe._errors import Error
 from pe._definition import Definition
 from pe.operators import Rule, Nonterminal
 
+_FuncMap = Dict[str, Union[Action, Callable]]
+
 
 class Grammar:
     """A parsing expression grammar definition."""
 
     def __init__(self,
-                 definitions: Dict[str, Definition] = None,
-                 actions: Dict[str, Callable] = None,
+                 definitions: Optional[Dict[str, Definition]] = None,
+                 actions: Optional[_FuncMap] = None,
                  start: str = 'Start'):
         self.definitions: Dict[str, Definition] = dict(definitions or [])
         self.actions = actions or {}
         self.start = start
         self._finalize()
 
     def __repr__(self):
```

### Comparing `pe-0.3.2/pe/_match.py` & `pe-0.4.0/pe/_match.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/_optimize.py` & `pe-0.4.0/pe/_optimize.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/_parse.py` & `pe-0.4.0/pe/_parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   EndOfLine  <- '\r\n' / '\n' / '\r'
   EndOfFile  <- !.
 """
 
 from typing import Tuple, Dict, cast
 
 import pe
-from pe._errors import Error
+from pe._errors import Error, ParseError, GrammarError
 from pe._definition import Definition
 from pe._grammar import Grammar
 from pe.operators import (
     Dot,
     Literal,
     Class,
     Nonterminal,
@@ -242,15 +242,21 @@
 )
 
 _parser = PackratParser(PEG)
 
 
 def loads(source: str) -> Tuple[str, Dict[str, Definition]]:
     """Parse the PEG at *source* and return a list of definitions."""
-    m = _parser.match(source, flags=pe.STRICT | pe.MEMOIZE)
+    if not source.strip():
+        raise GrammarError("empty grammar")
+    try:
+        m = _parser.match(source, flags=pe.STRICT | pe.MEMOIZE)
+    except ParseError as exc:
+        raise GrammarError("invalid grammar") from exc
+
     if not m:
         raise Error('invalid grammar')
     defs = m.value()
     if isinstance(defs, Definition):
         start = 'Start'
         defmap = {'Start': defs}
     else:
```

### Comparing `pe-0.3.2/pe/_parser.py` & `pe-0.4.0/pe/_parser.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/_py_machine.py` & `pe-0.4.0/pe/_py_machine.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/actions.py` & `pe-0.4.0/pe/actions.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/pe/operators.py` & `pe-0.4.0/pe/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
 
 def Bind(expression: _Def, name: str):
     assert isinstance(name, str)
     return Definition(BND, (_validate(expression), name))
 
 
-def Rule(expression: _Def, action: Callable, name: str = ANONYMOUS):
+def Rule(expression: _Def, action: Union[Action, Callable], name: str = ANONYMOUS):
     if action and not isinstance(action, Action):
         action = Call(action)
     return Definition(RUL, (_validate(expression), action, name))
 
 
 def Debug(expression: _Def):
     return Definition(DBG, (_validate(expression),))
```

### Comparing `pe-0.3.2/pe/packrat.py` & `pe-0.4.0/pe/packrat.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Packrat Parsing
 
 """
 
 # NOTE: attempting to use exceptions instead of FAIL codes resulted in
 # almost a 2x slowdown, so it's probably not a good idea
 
-from typing import (Union, List, Dict, Callable, Iterable, Any)
+from typing import List, Dict, Callable, Iterable, Any, Optional
 from collections import defaultdict
 import re
 import inspect
 
 from pe._constants import (
     FAIL,
     MAX_MEMO_SIZE,
@@ -56,16 +56,16 @@
 
     def __contains__(self, name: str) -> bool:
         return name in self._exprs
 
     def match(self,
               s: str,
               pos: int = 0,
-              flags: Flag = Flag.MEMOIZE | Flag.STRICT) -> Union[Match, None]:
-        memo: Union[Memo, None] = None
+              flags: Flag = Flag.MEMOIZE | Flag.STRICT) -> Optional[Match]:
+        memo: Optional[Memo] = None
         if flags & Flag.MEMOIZE:
             memo = defaultdict(dict)
 
         end, args, kwargs = self._exprs[self.start](s, pos, memo)
 
         if end < 0:
             if flags & Flag.STRICT:
@@ -341,16 +341,16 @@
     A grammar rule is a named expression with an optional action.
 
     The *name* field is more relevant for the grammar than the rule
     itself, but it helps with debugging.
     """
     def __init__(self,
                  name: str,
-                 expression: _Matcher = None,
-                 action: Action = None):
+                 expression: Optional[_Matcher] = None,
+                 action: Optional[Action] = None):
         self.name = name
         self.expression = expression
         self.action = action
 
     def __call__(self, s: str, pos: int, memo: Memo) -> RawMatch:
         expression = self.expression
```

### Comparing `pe-0.3.2/pe.egg-info/PKG-INFO` & `pe-0.4.0/pe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: pe
-Version: 0.3.2
+Version: 0.4.0
 Summary: Library for Parsing Expression Grammars (PEG)
 Home-page: https://github.com/goodmami/pe/
 Author: Michael Wayne Goodman
 Author-email: goodman.m.w@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/goodmami/pe/blob/main/docs/README.md
 Project-URL: Changelog, https://github.com/goodmami/pe/blob/main/CHANGELOG.md
 Keywords: peg,parsing,text
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/goodmami/pe/main/docs/_static/pe-logo.svg" alt="pe logo">
   <br>
@@ -243,9 +242,7 @@
 - [TatSu](https://tatsu.readthedocs.io/en/stable/) (Python)
 - [PEG.js](https://github.com/pegjs/pegjs) (Javascript)
 - [Pegged](https://github.com/PhilippeSigaud/Pegged) (D)
 - [pegen](https://github.com/gvanrossum/pegen) (Python / C)
 - [LPeg] (Lua)
 
 [LPeg]: http://www.inf.puc-rio.br/~roberto/lpeg/
-
-
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pe Version: 0.3.2 Summary: Library for Parsing
+Metadata-Version: 2.1 Name: pe Version: 0.4.0 Summary: Library for Parsing
 Expression Grammars (PEG) Home-page: https://github.com/goodmami/pe/ Author:
 Michael Wayne Goodman Author-email: goodman.m.w@gmail.com License: MIT Project-
 URL: Documentation, https://github.com/goodmami/pe/blob/main/docs/README.md
 Project-URL: Changelog, https://github.com/goodmami/pe/blob/main/CHANGELOG.md
-Keywords: peg,parsing,text Platform: UNKNOWN Classifier: Development Status ::
-4 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Cython Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Text Processing Classifier:
-Topic :: Utilities Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE
+Keywords: peg,parsing,text Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Cython Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: Topic :: Text Processing Classifier: Topic :: Utilities
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE
                                   [pe logo]
                              Parsing Expressions
                      [PyPI_link] [Python Support] [tests]
 --- **pe** is a library for parsing expressions, including [parsing expression
 grammars] (PEGs). It aims to join the expressive power of parsing expressions
 with the familiarity of regular expressions. For example: ```python >>> import
 pe >>> pe.match(r'"-"? [0-9]+', '-38') # match an integer
```

### Comparing `pe-0.3.2/pe.egg-info/SOURCES.txt` & `pe-0.4.0/pe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/setup.cfg` & `pe-0.4.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 [metadata]
 name = pe
+version = attr: pe.__version__
 description = Library for Parsing Expression Grammars (PEG)
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 keywords = peg, parsing, text
 author = Michael Wayne Goodman
 author_email = goodman.m.w@gmail.com
 url = https://github.com/goodmami/pe/
-requires_python = ">=3.6"
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Cython
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Text Processing
 	Topic :: Utilities
 project_urls = 
 	Documentation = https://github.com/goodmami/pe/blob/main/docs/README.md
 	Changelog = https://github.com/goodmami/pe/blob/main/CHANGELOG.md
 
 [options]
-python_requires = >= 3.6
+python_requires = >= 3.8
 zip_safe = False
 packages = pe
 test_suite = test
 setup_requires = 
-	setuptools >=46.4.0
+	setuptools >= 67.8
 	Cython ~= 0.29
 tests_require = 
 	pytest
 
 [flake8]
 max-line-length = 88
 exclude = .git, __pycache__, test/, build/, dist/
```

### Comparing `pe-0.3.2/setup.py` & `pe-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/test/test__match.py` & `pe-0.4.0/test/test__match.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/test/test__optimize.py` & `pe-0.4.0/test/test__optimize.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/test/test__parse.py` & `pe-0.4.0/test/test__parse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import pytest
 
+from pe._errors import GrammarError
 from pe.operators import (
     Dot,
     Literal,
     Class,
     Sequence,
     Choice,
     Optional,
@@ -114,7 +116,16 @@
     assert loads('A <- "a" B <- "b"') == ('A', {'A': Literal('a'),
                                                 'B': Literal('b')})
     assert loads('''
         A   <- "a" Bee
         Bee <- "b"
     ''') == ('A', {'A': Sequence('a', Nonterminal('Bee')),
                    'Bee': Literal('b')})
+
+
+def test_loads_error():
+    with pytest.raises(GrammarError):
+        loads('')
+    with pytest.raises(GrammarError):
+        loads('A <- +"a"')
+    with pytest.raises(GrammarError):
+        loads('A <- "a"+*')
```

### Comparing `pe-0.3.2/test/test_operators.py` & `pe-0.4.0/test/test_operators.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/test/test_parsers.py` & `pe-0.4.0/test/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/test/test_pe.py` & `pe-0.4.0/test/test_pe.py`

 * *Files identical despite different names*

### Comparing `pe-0.3.2/test/test_regression.py` & `pe-0.4.0/test/test_regression.py`

 * *Files identical despite different names*

