# Comparing `tmp/mawk-0.1.3.tar.gz` & `tmp/mawk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mawk-0.1.3.tar", max compression
+gzip compressed data, was "mawk-0.1.4.tar", max compression
```

## Comparing `mawk-0.1.3.tar` & `mawk-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-05-17 23:10:37.697187 mawk-0.1.3/LICENSE
--rw-r--r--   0        0        0     2380 2023-05-17 23:10:37.701187 mawk-0.1.3/README.md
--rw-r--r--   0        0        0     3349 2023-05-17 23:10:37.701187 mawk-0.1.3/mawk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 23:10:37.701187 mawk-0.1.3/mawk/py.typed
--rw-r--r--   0        0        0      543 2023-05-17 23:10:37.701187 mawk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 mawk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-04 12:53:24.595502 mawk-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2380 2023-06-04 12:53:24.595502 mawk-0.1.4/README.md
+-rw-r--r--   0        0        0     3546 2023-06-04 12:53:24.595502 mawk-0.1.4/mawk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:53:24.595502 mawk-0.1.4/mawk/py.typed
+-rw-r--r--   0        0        0      543 2023-06-04 12:53:24.595502 mawk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 mawk-0.1.4/PKG-INFO
```

### Comparing `mawk-0.1.3/LICENSE` & `mawk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mawk-0.1.3/README.md` & `mawk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mawk-0.1.3/mawk/__init__.py` & `mawk-0.1.4/mawk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,22 +69,26 @@
     else:
         return f
 
 
 Rule = Callable[[str], list[str]]
 
 
-def run(rules: list[Rule], inp: str, exclusive=True, on_eof=None) -> str:
+def run(rules: list[Rule], inp: str, exclusive=True, on_begin=None, on_eof=None) -> str:
     """Takes a list of rules, being function from `str` to `list[str]`.
     The input string is split into lines, after which each line is fed
     through the list of rules. All the results are colected into a list
     of strings and then joined by newline.
     """
     lines = inp.splitlines()
     result = []
+
+    if on_begin:
+        result.extend(on_begin())
+
     for l in lines:
         for r in rules:
             v = r(l)
             if v is not None:
                 result.extend(v)
                 if exclusive:
                     break
@@ -102,14 +106,18 @@
     decorated methods."""
 
     def list_rules(self):
         members = (getattr(self, m) for m in dir(self) if m[0] != "_")
         rules = [m for m in members if hasattr(m, "_is_rule")]
         return sorted(rules, key=lambda r: r._is_rule)
 
+    def on_begin(self):
+        """This method gets called at the start of a scan."""
+        return []
+
     def on_eof(self):
         """This method gets called at the end of a scan."""
         return []
 
     def run(self, inp: str, exclusive=True) -> str:
         """Runs all rules in the class on input."""
-        return run(self.list_rules(), inp, exclusive, on_eof=self.on_eof)
+        return run(self.list_rules(), inp, exclusive, on_begin=self.on_begin, on_eof=self.on_eof)
```

### Comparing `mawk-0.1.3/pyproject.toml` & `mawk-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mawk"
-version = "0.1.3"
+version = "0.1.4"
 description = "A minimalist implementation of an Awk-like model in Python"
 authors = ["Johan Hidding <j.hidding@esciencecenter.nl>"]
 license = "Apache 2"
 readme = "README.md"
 repository = "https://github.com/jhidding/mawk"
 
 [tool.poetry.dependencies]
```

### Comparing `mawk-0.1.3/PKG-INFO` & `mawk-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mawk
-Version: 0.1.3
+Version: 0.1.4
 Summary: A minimalist implementation of an Awk-like model in Python
 Home-page: https://github.com/jhidding/mawk
 License: Apache 2
 Author: Johan Hidding
 Author-email: j.hidding@esciencecenter.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

