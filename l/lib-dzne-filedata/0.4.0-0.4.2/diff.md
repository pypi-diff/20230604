# Comparing `tmp/lib-dzne-filedata-0.4.0.tar.gz` & `tmp/lib-dzne-filedata-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-filedata-0.4.0.tar", last modified: Mon May 29 12:33:02 2023, max compression
+gzip compressed data, was "lib-dzne-filedata-0.4.2.tar", last modified: Sun Jun  4 06:36:26 2023, max compression
```

## Comparing `lib-dzne-filedata-0.4.0.tar` & `lib-dzne-filedata-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:33:02.670066 lib-dzne-filedata-0.4.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.4.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 12:33:02.670066 lib-dzne-filedata-0.4.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.4.0/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      556 2023-05-29 12:32:04.000000 lib-dzne-filedata-0.4.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 12:33:02.670066 lib-dzne-filedata-0.4.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:33:02.666066 lib-dzne-filedata-0.4.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:33:02.666066 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata/
--rw-r--r--   0 base      (1001) base      (1001)     7233 2023-05-29 12:30:10.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:33:02.670066 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 12:33:02.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 12:33:02.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 12:33:02.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       36 2023-05-29 12:33:02.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 12:33:02.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-04 06:36:26.736199 lib-dzne-filedata-0.4.2/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.4.2/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-06-04 06:36:26.736199 lib-dzne-filedata-0.4.2/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.4.2/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      556 2023-06-04 06:24:01.000000 lib-dzne-filedata-0.4.2/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-04 06:36:26.736199 lib-dzne-filedata-0.4.2/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-04 06:36:26.736199 lib-dzne-filedata-0.4.2/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-04 06:36:26.736199 lib-dzne-filedata-0.4.2/src/lib_dzne_filedata/
+-rw-r--r--   0 base      (1001) base      (1001)     7509 2023-06-04 06:34:29.000000 lib-dzne-filedata-0.4.2/src/lib_dzne_filedata/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-04 06:36:26.736199 lib-dzne-filedata-0.4.2/src/lib_dzne_filedata.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-06-04 06:36:26.000000 lib-dzne-filedata-0.4.2/src/lib_dzne_filedata.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      300 2023-06-04 06:36:26.000000 lib-dzne-filedata-0.4.2/src/lib_dzne_filedata.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-04 06:36:26.000000 lib-dzne-filedata-0.4.2/src/lib_dzne_filedata.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       36 2023-06-04 06:36:26.000000 lib-dzne-filedata-0.4.2/src/lib_dzne_filedata.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-06-04 06:36:26.000000 lib-dzne-filedata-0.4.2/src/lib_dzne_filedata.egg-info/top_level.txt
```

### Comparing `lib-dzne-filedata-0.4.0/LICENSE` & `lib-dzne-filedata-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-filedata-0.4.0/PKG-INFO` & `lib-dzne-filedata-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.4.0
+Version: 0.4.2
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-filedata-0.4.0/pyproject.toml` & `lib-dzne-filedata-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-filedata"
-version = "0.4.0"
+version = "0.4.2"
 description = "Libary for filedata handling. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
 dependencies = [
     "tomli_w>=1.0.0",
-    "lib-dzne-math>=0.2.0",
+    "lib-dzne-math>=0.2.3",
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-filedata-0.4.0/src/lib_dzne_filedata/__init__.py` & `lib-dzne-filedata-0.4.2/src/lib_dzne_filedata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,43 +40,44 @@
             txtfile = _os.path.join(directory, "b"+TXTData.ext())
             self.save(file)
             _os.rename(file, txtfile)
             txtdata = TXTData.load(txtfile)
         return str(txtdata)
     @classmethod
     def from_str(cls, string, /):
-        txtdata = TXTData([string])
+        txtdata = TXTData.from_str(string)
         with _tmp.TemporaryDirectory() as directory:
             txtfile = _os.path.join(directory, "b"+TXTData.ext())
-            file = _os.path.join(directory, "a"+self.ext())
+            file = _os.path.join(directory, "a"+cls.ext())
             txtdata.save(txtfile)
             _os.rename(txtfile, file)
             return cls.load(file)
 
 
     @classmethod
     def file(cls, /, string):
         return _File(fileDataType=cls, string=string)
     @classmethod
     def ext(cls):
         return cls._ext
     @classmethod
     def check_ext(cls, /, file):
-        if cls._ext is None:
+        if cls._ext == _os.path.splitext(file)[1]:
             return
-        if cls._ext == _os.path.splitext(file):
-            return
-        raise ValueError()
+        raise ValueError(f"{file.__repr__()} has an illegal extension! ")
     @classmethod
     def load(cls, /, file, **kwargs):
         if file == "":
             ans = cls._default()
         else:
             cls.check_ext(file)
-            ans = cls._load(file=file, **kwargs)
+            try:
+                ans = cls._load(file=file, **kwargs)
+            except:
+                raise ValueError(f"Loading file {file.__repr__()} failed! ")
         return cls(ans)
     def save(self, /, file, *, overwrite=False, **kwargs):
         cls = type(self)
         if file == "":
             ans = type(self).drop()
         elif _os.path.exists(file) and not overwrite:
             raise FileExistsError(file)
@@ -98,27 +99,33 @@
     def default(cls):
         return cls.load("")
     @property
     def data(self):
         return type(self).clone_data(self._data)
     @data.setter
     def data(self, value):
-        self._data = type(self).clone_data(self._data)
+        self._data = type(self).clone_data(value)
 
 
 
 class TXTData(FileData):
     _ext = '.txt'
     def __str__(self):
         ans = ""
         for line in self._data:
             ans += line
             ans += '\n'
         return ans
     @classmethod
+    def from_str(cls, string, /):
+        string = str(string)
+        data = string.split('\n')
+        ans = cls(data)
+        return ans
+    @classmethod
     def _load(cls, /, file):
         ans = list()
         with open(file, 'r') as s:
             for line in s:
                 if not line.endswith('\n'):
                     raise ValueError()
                 ans.append(line[:-1])
@@ -158,15 +165,14 @@
         del target[keys[-1]]
     def __add__(self, other):
         if type(self) is not type(other):
             other = type(self)(other)
         return self._add(self, other)
     def __radd__(self, other):
         return self.__add__(other)
-
     @classmethod
     def _add(cls, *objs):
         ans = cls.default()
         for obj in objs:
             for k, v in obj.iteritems():
                 if ans.get(*k) is None:
                     ans[k] = v
@@ -205,15 +211,14 @@
             gen = data.items()
         else:
             yield (tuple(), data)
             return
         for k, v in gen:
             for keys, value in cls._iteritems(v):
                 yield ((k,) + keys), value
-
     @classmethod
     def clone_data(cls, data):
         if issubclass(type(data), cls):
             data = data._data
         if _na.isna(data):
             return float('nan')
         if type(data) in (str, int, bool, float):
```

### Comparing `lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/PKG-INFO` & `lib-dzne-filedata-0.4.2/src/lib_dzne_filedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.4.0
+Version: 0.4.2
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

