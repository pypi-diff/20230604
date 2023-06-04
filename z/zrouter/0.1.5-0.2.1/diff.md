# Comparing `tmp/zrouter-0.1.5.tar.gz` & `tmp/zrouter-0.2.1.tar.gz`

## Comparing `zrouter-0.1.5.tar` & `zrouter-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 zrouter-0.1.5/src/zrouter/__init__.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 zrouter-0.1.5/src/zrouter/decorator.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.1.5/src/zrouter/exception.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.1.5/LICENSE
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.1.5/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 zrouter-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zrouter-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 zrouter-0.2.1/src/zrouter/__init__.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 zrouter-0.2.1/src/zrouter/decorator.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.2.1/src/zrouter/exception.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.2.1/LICENSE
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.2.1/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 zrouter-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 zrouter-0.2.1/PKG-INFO
```

### Comparing `zrouter-0.1.5/src/zrouter/decorator.py` & `zrouter-0.2.1/src/zrouter/decorator.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.1.5/LICENSE` & `zrouter-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.1.5/PKG-INFO` & `zrouter-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: zrouter
-Version: 0.1.5
+Version: 0.2.1
 Summary: zen router library
 Project-URL: Homepage, https://github.com/inspirare6/zrouter
 Project-URL: Bug Tracker, https://github.com/inspirare6/zrouter/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: flask==2.2.2
+Requires-Dist: fastapi==0.95.2
 Requires-Dist: inspirare
 Description-Content-Type: text/markdown
 
 # ztime
 
 Zen time library.
```

