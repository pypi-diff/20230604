# Comparing `tmp/asyncstdlib-3.9.1.tar.gz` & `tmp/asyncstdlib-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncstdlib-3.9.1.tar", last modified: Fri Mar  5 12:09:27 2021, max compression
+gzip compressed data, was "asyncstdlib-3.9.2.tar", last modified: Fri May 14 15:48:30 2021, max compression
```

## Comparing `asyncstdlib-3.9.1.tar` & `asyncstdlib-3.9.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      410 2019-12-12 07:32:51.249795 asyncstdlib-3.9.1/.coveragerc
--rw-r--r--   0        0        0     3387 2019-11-20 16:50:44.017648 asyncstdlib-3.9.1/.gitignore
--rw-r--r--   0        0        0      171 2019-11-22 16:36:36.853093 asyncstdlib-3.9.1/.readthedocs.yml
--rw-r--r--   0        0        0      668 2020-06-02 18:49:56.577235 asyncstdlib-3.9.1/.travis.yml
--rw-r--r--   0        0        0     1075 2020-01-10 17:27:50.616297 asyncstdlib-3.9.1/LICENSE
--rw-r--r--   0        0        0      994 2019-12-20 16:16:16.741047 asyncstdlib-3.9.1/README.rst
--rw-r--r--   0        0        0     1295 2021-03-05 12:08:42.684731 asyncstdlib-3.9.1/asyncstdlib/__init__.py
--rw-r--r--   0        0        0     3674 2021-02-24 18:36:26.351458 asyncstdlib-3.9.1/asyncstdlib/_core.py
--rw-r--r--   0        0        0    10467 2020-10-21 16:31:54.657115 asyncstdlib-3.9.1/asyncstdlib/_lrucache.py
--rw-r--r--   0        0        0      891 2020-03-19 20:18:44.928037 asyncstdlib-3.9.1/asyncstdlib/_utility.py
--rw-r--r--   0        0        0     9871 2021-03-05 11:42:18.545545 asyncstdlib-3.9.1/asyncstdlib/asynctools.py
--rw-r--r--   0        0        0    19212 2021-03-05 11:42:18.546442 asyncstdlib-3.9.1/asyncstdlib/builtins.py
--rw-r--r--   0        0        0    14943 2020-06-02 18:49:56.580733 asyncstdlib-3.9.1/asyncstdlib/contextlib.py
--rw-r--r--   0        0        0     5225 2020-10-21 16:31:54.659533 asyncstdlib-3.9.1/asyncstdlib/functools.py
--rw-r--r--   0        0        0    20974 2021-03-05 11:42:18.547316 asyncstdlib-3.9.1/asyncstdlib/itertools.py
--rw-r--r--   0        0        0      580 2019-09-20 16:00:47.755000 asyncstdlib-3.9.1/docs/Makefile
--rw-r--r--   0        0        0     4806 2021-03-05 11:42:18.548093 asyncstdlib-3.9.1/docs/conf.py
--rw-r--r--   0        0        0     5106 2020-12-01 11:45:33.218388 asyncstdlib-3.9.1/docs/index.rst
--rw-r--r--   0        0        0      787 2019-09-20 16:00:47.755000 asyncstdlib-3.9.1/docs/make.bat
--rw-r--r--   0        0        0      907 2021-03-05 12:05:52.821655 asyncstdlib-3.9.1/docs/source/api/asynctools.rst
--rw-r--r--   0        0        0     1889 2021-02-24 18:18:58.252821 asyncstdlib-3.9.1/docs/source/api/builtins.rst
--rw-r--r--   0        0        0     1612 2020-06-02 18:49:56.584119 asyncstdlib-3.9.1/docs/source/api/contextlib.rst
--rw-r--r--   0        0        0     3337 2020-10-27 14:55:22.220079 asyncstdlib-3.9.1/docs/source/api/functools.rst
--rw-r--r--   0        0        0     2031 2021-02-18 16:03:46.229534 asyncstdlib-3.9.1/docs/source/api/itertools.rst
--rw-r--r--   0        0        0      938 2020-07-23 08:25:15.028460 asyncstdlib-3.9.1/docs/source/glossary.rst
--rw-r--r--   0        0        0      912 2020-01-10 17:32:04.309227 asyncstdlib-3.9.1/pyproject.toml
--rw-r--r--   0        0        0      169 2019-11-20 21:22:45.358183 asyncstdlib-3.9.1/setup.cfg
--rw-r--r--   0        0        0        0 2019-11-18 22:50:14.886698 asyncstdlib-3.9.1/unittests/__init__.py
--rw-r--r--   0        0        0     5783 2021-02-24 17:09:14.113467 asyncstdlib-3.9.1/unittests/test_asynctools.py
--rw-r--r--   0        0        0     9231 2021-02-18 13:51:58.031025 asyncstdlib-3.9.1/unittests/test_builtins.py
--rw-r--r--   0        0        0     7509 2020-03-15 20:41:07.977279 asyncstdlib-3.9.1/unittests/test_contextlib.py
--rw-r--r--   0        0        0     8990 2020-10-21 16:31:54.662765 asyncstdlib-3.9.1/unittests/test_functools.py
--rw-r--r--   0        0        0     1250 2020-06-02 18:49:56.587443 asyncstdlib-3.9.1/unittests/test_helpers.py
--rw-r--r--   0        0        0     8701 2021-02-18 16:03:46.230664 asyncstdlib-3.9.1/unittests/test_itertools.py
--rw-r--r--   0        0        0     3264 2020-03-19 08:04:36.789109 asyncstdlib-3.9.1/unittests/utility.py
--rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 asyncstdlib-3.9.1/setup.py
--rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 asyncstdlib-3.9.1/PKG-INFO
+-rw-r--r--   0        0        0      410 2019-12-12 07:32:51.249795 asyncstdlib-3.9.2/.coveragerc
+-rw-r--r--   0        0        0     3387 2019-11-20 16:50:44.017648 asyncstdlib-3.9.2/.gitignore
+-rw-r--r--   0        0        0      171 2019-11-22 16:36:36.853093 asyncstdlib-3.9.2/.readthedocs.yml
+-rw-r--r--   0        0        0      668 2020-06-02 18:49:56.577235 asyncstdlib-3.9.2/.travis.yml
+-rw-r--r--   0        0        0     1075 2020-01-10 17:27:50.616297 asyncstdlib-3.9.2/LICENSE
+-rw-r--r--   0        0        0      994 2019-12-20 16:16:16.741047 asyncstdlib-3.9.2/README.rst
+-rw-r--r--   0        0        0     1295 2021-05-14 15:47:26.009637 asyncstdlib-3.9.2/asyncstdlib/__init__.py
+-rw-r--r--   0        0        0     3674 2021-02-24 18:36:26.351458 asyncstdlib-3.9.2/asyncstdlib/_core.py
+-rw-r--r--   0        0        0    10566 2021-05-14 15:47:18.052034 asyncstdlib-3.9.2/asyncstdlib/_lrucache.py
+-rw-r--r--   0        0        0      891 2020-03-19 20:18:44.928037 asyncstdlib-3.9.2/asyncstdlib/_utility.py
+-rw-r--r--   0        0        0     9971 2021-05-14 15:47:18.052365 asyncstdlib-3.9.2/asyncstdlib/asynctools.py
+-rw-r--r--   0        0        0    19212 2021-03-05 11:42:18.546442 asyncstdlib-3.9.2/asyncstdlib/builtins.py
+-rw-r--r--   0        0        0    15058 2021-05-14 15:47:18.052689 asyncstdlib-3.9.2/asyncstdlib/contextlib.py
+-rw-r--r--   0        0        0     5225 2020-10-21 16:31:54.659533 asyncstdlib-3.9.2/asyncstdlib/functools.py
+-rw-r--r--   0        0        0    20974 2021-03-05 11:42:18.547316 asyncstdlib-3.9.2/asyncstdlib/itertools.py
+-rw-r--r--   0        0        0      580 2019-09-20 16:00:47.755000 asyncstdlib-3.9.2/docs/Makefile
+-rw-r--r--   0        0        0     4806 2021-03-05 11:42:18.548093 asyncstdlib-3.9.2/docs/conf.py
+-rw-r--r--   0        0        0     5129 2021-05-14 15:47:18.052996 asyncstdlib-3.9.2/docs/index.rst
+-rw-r--r--   0        0        0      787 2019-09-20 16:00:47.755000 asyncstdlib-3.9.2/docs/make.bat
+-rw-r--r--   0        0        0      907 2021-03-05 12:05:52.821655 asyncstdlib-3.9.2/docs/source/api/asynctools.rst
+-rw-r--r--   0        0        0     1889 2021-02-24 18:18:58.252821 asyncstdlib-3.9.2/docs/source/api/builtins.rst
+-rw-r--r--   0        0        0     1612 2020-06-02 18:49:56.584119 asyncstdlib-3.9.2/docs/source/api/contextlib.rst
+-rw-r--r--   0        0        0     3337 2020-10-27 14:55:22.220079 asyncstdlib-3.9.2/docs/source/api/functools.rst
+-rw-r--r--   0        0        0     2031 2021-02-18 16:03:46.229534 asyncstdlib-3.9.2/docs/source/api/itertools.rst
+-rw-r--r--   0        0        0     4450 2021-05-14 15:47:18.053294 asyncstdlib-3.9.2/docs/source/contributing.rst
+-rw-r--r--   0        0        0      938 2020-07-23 08:25:15.028460 asyncstdlib-3.9.2/docs/source/glossary.rst
+-rw-r--r--   0        0        0      949 2021-05-14 15:47:18.053564 asyncstdlib-3.9.2/pyproject.toml
+-rw-r--r--   0        0        0      169 2019-11-20 21:22:45.358183 asyncstdlib-3.9.2/setup.cfg
+-rw-r--r--   0        0        0        0 2019-11-18 22:50:14.886698 asyncstdlib-3.9.2/unittests/__init__.py
+-rw-r--r--   0        0        0     5783 2021-02-24 17:09:14.113467 asyncstdlib-3.9.2/unittests/test_asynctools.py
+-rw-r--r--   0        0        0     9231 2021-02-18 13:51:58.031025 asyncstdlib-3.9.2/unittests/test_builtins.py
+-rw-r--r--   0        0        0     7509 2020-03-15 20:41:07.977279 asyncstdlib-3.9.2/unittests/test_contextlib.py
+-rw-r--r--   0        0        0     8990 2020-10-21 16:31:54.662765 asyncstdlib-3.9.2/unittests/test_functools.py
+-rw-r--r--   0        0        0     1250 2020-06-02 18:49:56.587443 asyncstdlib-3.9.2/unittests/test_helpers.py
+-rw-r--r--   0        0        0     8701 2021-02-18 16:03:46.230664 asyncstdlib-3.9.2/unittests/test_itertools.py
+-rw-r--r--   0        0        0     3264 2020-03-19 08:04:36.789109 asyncstdlib-3.9.2/unittests/utility.py
+-rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 asyncstdlib-3.9.2/setup.py
+-rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 asyncstdlib-3.9.2/PKG-INFO
```

### Comparing `asyncstdlib-3.9.1/.gitignore` & `asyncstdlib-3.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/.travis.yml` & `asyncstdlib-3.9.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/LICENSE` & `asyncstdlib-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/README.rst` & `asyncstdlib-3.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/asyncstdlib/__init__.py` & `asyncstdlib-3.9.2/asyncstdlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     tee,
     pairwise,
     zip_longest,
     groupby,
 )
 from .asynctools import borrow, scoped_iter, await_each, apply
 
-__version__ = "3.9.1"
+__version__ = "3.9.2"
 
 __all__ = [
     "anext",
     "zip",
     "map",
     "filter",
     "enumerate",
```

### Comparing `asyncstdlib-3.9.1/asyncstdlib/_core.py` & `asyncstdlib-3.9.2/asyncstdlib/_core.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/asyncstdlib/_lrucache.py` & `asyncstdlib-3.9.2/asyncstdlib/_lrucache.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,20 @@
     Optional,
     Tuple,
     Dict,
     Union,
 )
 from functools import update_wrapper
 from collections import OrderedDict
+import sys
 
-from typing_extensions import Protocol, TypedDict
+if sys.version_info[:2] >= (3, 8):
+    from typing import Protocol, TypedDict
+else:
+    from typing_extensions import Protocol, TypedDict
 
 from ._utility import public_module
 
 
 R = TypeVar("R")
```

### Comparing `asyncstdlib-3.9.1/asyncstdlib/_utility.py` & `asyncstdlib-3.9.2/asyncstdlib/_utility.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/asyncstdlib/asynctools.py` & `asyncstdlib-3.9.2/asyncstdlib/asynctools.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,20 @@
     Iterable,
     Awaitable,
     AsyncIterable,
     Callable,
     Any,
     overload,
 )
-from typing_extensions import AsyncContextManager
+import sys
+
+if sys.version_info[:2] >= (3, 8):
+    from typing import AsyncContextManager
+else:
+    from typing_extensions import AsyncContextManager
 
 from ._core import AnyIterable, aiter
 from .contextlib import nullcontext
 
 
 T = TypeVar("T")
 S = TypeVar("S")
```

### Comparing `asyncstdlib-3.9.1/asyncstdlib/builtins.py` & `asyncstdlib-3.9.2/asyncstdlib/builtins.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/asyncstdlib/contextlib.py` & `asyncstdlib-3.9.2/asyncstdlib/contextlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,24 @@
     AsyncGenerator,
     Callable,
     Optional,
     Union,
     Any,
     Awaitable,
 )
-from typing_extensions import Protocol, AsyncContextManager, ContextManager
 from functools import wraps
 from collections import deque
 from functools import partial
 import sys
 
+if sys.version_info[:2] >= (3, 8):
+    from typing import Protocol, AsyncContextManager, ContextManager
+else:
+    from typing_extensions import Protocol, AsyncContextManager, ContextManager
+
 from ._core import awaitify
 from ._utility import public_module, slot_get as _slot_get
 
 
 # typing.AsyncContextManager uses contextlib.AbstractAsyncContextManager if available,
 # and a custom implementation otherwise. No need to replicate it.
 AbstractContextManager = AsyncContextManager
```

### Comparing `asyncstdlib-3.9.1/asyncstdlib/functools.py` & `asyncstdlib-3.9.2/asyncstdlib/functools.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/asyncstdlib/itertools.py` & `asyncstdlib-3.9.2/asyncstdlib/itertools.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/docs/Makefile` & `asyncstdlib-3.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/docs/conf.py` & `asyncstdlib-3.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/docs/index.rst` & `asyncstdlib-3.9.2/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
    source/api/builtins
    source/api/functools
    source/api/contextlib
    source/api/itertools
    source/api/asynctools
    source/glossary
+   source/contributing
 
 The ``asyncstdlib`` library re-implements functions and classes of the Python
 standard library to make them compatible with ``async`` callables, iterables
 and context managers.
 It is fully agnostic to ``async`` event loops and seamlessly works with
 :py:mod:`asyncio`, third-party libraries such as :py:mod:`trio`, as well as
 any custom ``async`` event loop.
```

### Comparing `asyncstdlib-3.9.1/docs/make.bat` & `asyncstdlib-3.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/docs/source/api/asynctools.rst` & `asyncstdlib-3.9.2/docs/source/api/asynctools.rst`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/docs/source/api/builtins.rst` & `asyncstdlib-3.9.2/docs/source/api/builtins.rst`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/docs/source/api/contextlib.rst` & `asyncstdlib-3.9.2/docs/source/api/contextlib.rst`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/docs/source/api/functools.rst` & `asyncstdlib-3.9.2/docs/source/api/functools.rst`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/docs/source/api/itertools.rst` & `asyncstdlib-3.9.2/docs/source/api/itertools.rst`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/docs/source/glossary.rst` & `asyncstdlib-3.9.2/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/pyproject.toml` & `asyncstdlib-3.9.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
 ]
-requires = ["typing_extensions"]
+requires = ["typing_extensions; python_version<'3.8'"]
 
 [tool.flit.metadata.requires-extra]
 test = [
     "pytest >=4.3.0",
     "flake8",
     "flake8-bugbear",
     "black; implementation_name=='cpython'",
+    "coverage"
 ]
 doc = ["sphinx", "sphinxcontrib-contentui", "sphinxcontrib-trio"]
 
 [tool.flit.metadata.urls]
 Documentation = "https://asyncstdlib.readthedocs.io/en/latest/"
```

### Comparing `asyncstdlib-3.9.1/unittests/test_asynctools.py` & `asyncstdlib-3.9.2/unittests/test_asynctools.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/unittests/test_builtins.py` & `asyncstdlib-3.9.2/unittests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/unittests/test_contextlib.py` & `asyncstdlib-3.9.2/unittests/test_contextlib.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/unittests/test_functools.py` & `asyncstdlib-3.9.2/unittests/test_functools.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/unittests/test_helpers.py` & `asyncstdlib-3.9.2/unittests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/unittests/test_itertools.py` & `asyncstdlib-3.9.2/unittests/test_itertools.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/unittests/utility.py` & `asyncstdlib-3.9.2/unittests/utility.py`

 * *Files identical despite different names*

### Comparing `asyncstdlib-3.9.1/setup.py` & `asyncstdlib-3.9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,26 +5,23 @@
 
 packages = \
 ['asyncstdlib']
 
 package_data = \
 {'': ['*']}
 
-install_requires = \
-['typing_extensions']
-
 extras_require = \
-{'doc': ['sphinx', 'sphinxcontrib-contentui', 'sphinxcontrib-trio'],
- 'test': ['pytest >=4.3.0', 'flake8', 'flake8-bugbear'],
+{":python_version<'3.8'": ['typing_extensions'],
+ 'doc': ['sphinx', 'sphinxcontrib-contentui', 'sphinxcontrib-trio'],
+ 'test': ['pytest >=4.3.0', 'flake8', 'flake8-bugbear', 'coverage'],
  "test:implementation_name=='cpython'": ['black']}
 
 setup(name='asyncstdlib',
-      version='3.9.1',
+      version='3.9.2',
       description='The missing async toolbox',
       author='Max Fischer',
       author_email='maxfischer2781@gmail.com',
       url='https://github.com/maxfischer2781/asyncstdlib',
       packages=packages,
       package_data=package_data,
-      install_requires=install_requires,
       extras_require=extras_require,
      )
```

