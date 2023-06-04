# Comparing `tmp/cpp_linter_hooks-0.2.2-py3-none-any.whl.zip` & `tmp/cpp_linter_hooks-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6193 bytes, number of entries: 10
--rw-r--r--  2.0 unx      471 b- defN 22-Aug-14 03:19 cpp_linter_hooks/__init__.py
--rw-r--r--  2.0 unx     1044 b- defN 22-Aug-14 03:19 cpp_linter_hooks/clang_format.py
--rw-r--r--  2.0 unx      928 b- defN 22-Aug-14 03:19 cpp_linter_hooks/clang_tidy.py
--rw-r--r--  2.0 unx     1466 b- defN 22-Aug-14 03:19 cpp_linter_hooks/util.py
--rw-r--r--  2.0 unx     1067 b- defN 22-Aug-14 03:19 cpp_linter_hooks-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5454 b- defN 22-Aug-14 03:19 cpp_linter_hooks-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-14 03:19 cpp_linter_hooks-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      124 b- defN 22-Aug-14 03:19 cpp_linter_hooks-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 22-Aug-14 03:19 cpp_linter_hooks-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      876 b- defN 22-Aug-14 03:19 cpp_linter_hooks-0.2.2.dist-info/RECORD
-10 files, 11539 bytes uncompressed, 4677 bytes compressed:  59.5%
+Zip file size: 6330 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      471 b- defN 23-Jun-04 14:49 cpp_linter_hooks/__init__.py
+-rw-r--r--  2.0 unx     1044 b- defN 23-Jun-04 14:49 cpp_linter_hooks/clang_format.py
+-rw-r--r--  2.0 unx      928 b- defN 23-Jun-04 14:49 cpp_linter_hooks/clang_tidy.py
+-rw-r--r--  2.0 unx     1466 b- defN 23-Jun-04 14:49 cpp_linter_hooks/util.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Jun-04 14:49 cpp_linter_hooks-0.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5870 b- defN 23-Jun-04 14:49 cpp_linter_hooks-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 14:49 cpp_linter_hooks-0.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-04 14:49 cpp_linter_hooks-0.2.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-04 14:49 cpp_linter_hooks-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      876 b- defN 23-Jun-04 14:49 cpp_linter_hooks-0.2.4.dist-info/RECORD
+10 files, 11955 bytes uncompressed, 4814 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: cpp_linter_hooks/clang_tidy.py
 Comment: 
 
 Filename: cpp_linter_hooks/util.py
 Comment: 
 
-Filename: cpp_linter_hooks-0.2.2.dist-info/LICENSE
+Filename: cpp_linter_hooks-0.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: cpp_linter_hooks-0.2.2.dist-info/METADATA
+Filename: cpp_linter_hooks-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: cpp_linter_hooks-0.2.2.dist-info/WHEEL
+Filename: cpp_linter_hooks-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: cpp_linter_hooks-0.2.2.dist-info/entry_points.txt
+Filename: cpp_linter_hooks-0.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: cpp_linter_hooks-0.2.2.dist-info/top_level.txt
+Filename: cpp_linter_hooks-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: cpp_linter_hooks-0.2.2.dist-info/RECORD
+Filename: cpp_linter_hooks-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cpp_linter_hooks-0.2.2.dist-info/LICENSE` & `cpp_linter_hooks-0.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cpp_linter_hooks-0.2.2.dist-info/METADATA` & `cpp_linter_hooks-0.2.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp-linter-hooks
-Version: 0.2.2
+Version: 0.2.4
 Summary: Automatically check c/c++ with clang-format and clang-tidy
 Author-email: Peter Shen <xianpeng.shen@gmail.com>
 License: MIT License
 Project-URL: source, https://github.com/cpp-linter/cpp-linter-hooks
 Project-URL: tracker, https://github.com/cpp-linter/cpp-linter-hooks/issues
 Keywords: clang,clang-format,clang-tidy,pre-commit,pre-commit-hooks
 Classifier: Development Status :: 4 - Beta
@@ -15,19 +15,24 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: clang-tools (==0.8.0)
 
 # cpp-linter-hooks
 
-[![Test](https://github.com/cpp-linter/cpp-linter-hooks/actions/workflows/test.yml/badge.svg)](https://github.com/cpp-linter/cpp-linter-hooks/actions/workflows/test.yml)
+[![PyPI](https://img.shields.io/pypi/v/cpp-linter-hooks)](https://pypi.org/project/cpp-linter-hooks/)
 [![codecov](https://codecov.io/gh/cpp-linter/cpp-linter-hooks/branch/main/graph/badge.svg?token=L74Z3HZ4Y5)](https://codecov.io/gh/cpp-linter/cpp-linter-hooks)
+[![Test](https://github.com/cpp-linter/cpp-linter-hooks/actions/workflows/test.yml/badge.svg)](https://github.com/cpp-linter/cpp-linter-hooks/actions/workflows/test.yml)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+<!-- [![PyPI - Downloads](https://img.shields.io/pypi/dw/cpp-linter-hooks)](https://pypi.org/project/cpp-linter-hooks/) -->
+
 
 Using `clang-format` and `clang-tidy` hooks with [pre-commit](https://pre-commit.com/) to lint your C/C++ code.
 
 Highlight✨: No need to manually download and install `clang-format` or `clang-tidy` on your system.
 
 ## Usage
```

