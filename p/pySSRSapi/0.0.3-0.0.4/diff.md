# Comparing `tmp/pySSRSapi-0.0.3.tar.gz` & `tmp/pySSRSapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySSRSapi-0.0.3.tar", last modified: Sat Jun  3 22:43:53 2023, max compression
+gzip compressed data, was "pySSRSapi-0.0.4.tar", last modified: Sat Jun  3 23:26:58 2023, max compression
```

## Comparing `pySSRSapi-0.0.3.tar` & `pySSRSapi-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 22:43:53.631508 pySSRSapi-0.0.3/
--rw-r--r--   0 quaik8     (501) staff       (20)      532 2023-06-03 22:43:53.630801 pySSRSapi-0.0.3/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.3/README.md
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 22:43:53.626665 pySSRSapi-0.0.3/pySSRSapi/
--rw-r--r--   0 quaik8     (501) staff       (20)     8751 2023-06-03 22:43:05.000000 pySSRSapi-0.0.3/pySSRSapi/__init__.py
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 22:43:53.629965 pySSRSapi-0.0.3/pySSRSapi.egg-info/
--rw-r--r--   0 quaik8     (501) staff       (20)      532 2023-06-03 22:43:53.000000 pySSRSapi-0.0.3/pySSRSapi.egg-info/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-03 22:43:53.000000 pySSRSapi-0.0.3/pySSRSapi.egg-info/SOURCES.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-03 22:43:53.000000 pySSRSapi-0.0.3/pySSRSapi.egg-info/dependency_links.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-03 22:43:53.000000 pySSRSapi-0.0.3/pySSRSapi.egg-info/requires.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-03 22:43:53.000000 pySSRSapi-0.0.3/pySSRSapi.egg-info/top_level.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-03 22:43:53.631706 pySSRSapi-0.0.3/setup.cfg
--rw-r--r--   0 quaik8     (501) staff       (20)      800 2023-06-03 22:43:45.000000 pySSRSapi-0.0.3/setup.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 23:26:58.992402 pySSRSapi-0.0.4/
+-rw-r--r--   0 quaik8     (501) staff       (20)      532 2023-06-03 23:26:58.991965 pySSRSapi-0.0.4/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.4/README.md
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 23:26:58.986616 pySSRSapi-0.0.4/pySSRSapi/
+-rw-r--r--   0 quaik8     (501) staff       (20)     8926 2023-06-03 23:26:39.000000 pySSRSapi-0.0.4/pySSRSapi/__init__.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 23:26:58.991339 pySSRSapi-0.0.4/pySSRSapi.egg-info/
+-rw-r--r--   0 quaik8     (501) staff       (20)      532 2023-06-03 23:26:58.000000 pySSRSapi-0.0.4/pySSRSapi.egg-info/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-03 23:26:58.000000 pySSRSapi-0.0.4/pySSRSapi.egg-info/SOURCES.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-03 23:26:58.000000 pySSRSapi-0.0.4/pySSRSapi.egg-info/dependency_links.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-03 23:26:58.000000 pySSRSapi-0.0.4/pySSRSapi.egg-info/requires.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-03 23:26:58.000000 pySSRSapi-0.0.4/pySSRSapi.egg-info/top_level.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-03 23:26:58.992517 pySSRSapi-0.0.4/setup.cfg
+-rw-r--r--   0 quaik8     (501) staff       (20)      800 2023-06-03 23:26:50.000000 pySSRSapi-0.0.4/setup.py
```

### Comparing `pySSRSapi-0.0.3/PKG-INFO` & `pySSRSapi-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pySSRSapi-0.0.3/pySSRSapi/__init__.py` & `pySSRSapi-0.0.4/pySSRSapi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,23 @@
     
     def __repr__(self):
         return self.__str__()
     
     def to_json(self):
         return self.__str__()
     
+    def to_obj(self):
+        obj = {
+            'Username': self.Username,
+            'DisplayName': self.DisplayName
+        }
+        if self.Id != None:
+            obj.update({'Id': self.Id})
+        return obj
+    
     @staticmethod
     def from_json(json_dct):
         return User(
             json_dct['Id'],
             json_dct['Username'],
             json_dct['DisplayName']
         )
@@ -60,37 +69,35 @@
         return json.dumps(dict(self), ensure_ascii=False)
     
     def __repr__(self):
         return self.__str__()
     
     def to_json(self):
         return self.__str__()
+        
+    def to_obj(self):
+        obj = {
+            'Name': self.Name,
+            'Description': self.Description,
+            'Path': self.Path,
+            'ParentFolderId': self.ParentFolderId
+        }
+        if self.Id != None:
+            obj.update({'Id': self.Id})
+        return obj
     
     @staticmethod
     def from_json(json_dct):
         return Folder(
             json_dct['Id'],
             json_dct['Name'],
             json_dct['Description'],
             json_dct['Path'],
             json_dct['ParentFolderId']
         )
-        
-    def to_json(self):
-        json = {
-            'Name': self.Name,
-            'Description': self.Description,
-            'Path': self.Path,
-            'ParentFolderId': self.ParentFolderId
-        }
-        
-        if self.Id != None:
-            json.update({'Id': self.Id})
-        
-        return json
 
 class Datasource:
     def __init__(self, Id, Name: str, Description: str, Path: str, ParentFolderId: str, DataSourceType: str, ConnectionString: str, Content: str, ContentType: str = '', Size: int = 0):
         self.Id = Id
         self.Name = Name
         self.Description = Description
         self.Path = Path
@@ -120,46 +127,44 @@
     
     def __repr__(self):
         return self.__str__()
     
     def to_json(self):
         return self.__str__()
     
+    def to_obj(self):
+        obj = {
+            'Name': self.Name,
+            'Description': self.Description,
+            'Path': self.Path,
+            'ParentFolderId': self.ParentFolderId,
+            'DataSourceType': self.DataSourceType,
+            'ConnectionString': self.ConnectionString,
+            'Content': self.Content,
+            'ContentType': self.ContentType,
+            'Size': self.Size
+        }
+        if self.Id != None:
+            obj.update({'Id': self.Id})
+        return obj
+    
     @staticmethod
     def from_json(json_dct):
         return Datasource(
             json_dct['Id'],
             json_dct['Name'],
             json_dct['Description'],
             json_dct['Path'],
             json_dct['ParentFolderId'],
             json_dct['DataSourceType'],
             json_dct['ConnectionString'],
             json_dct['Content'],
             json_dct['ContentType'],
             json_dct['Size']
         )
-        
-    def to_json(self):
-        json = {
-            'Name': self.Name,
-            'Description': self.Description,
-            'Path': self.Path,
-            'ParentFolderId': self.ParentFolderId,
-            'DataSourceType': self.DataSourceType,
-            'ConnectionString': self.ConnectionString,
-            'Content': self.Content,
-            'ContentType': self.ContentType,
-            'Size': self.Size
-        }
-        
-        if self.Id != None:
-            json.update({'Id': self.Id})
-        
-        return json
 
 class Api:
     def __init__(self, url: str, user: str, password: str):
         self.url = url + EP_API
         self.basicAuth = HTTPBasicAuth(user, password)
         self.headers = {'Content-type': 'application/json;charset=UTF-8'}
```

### Comparing `pySSRSapi-0.0.3/pySSRSapi.egg-info/PKG-INFO` & `pySSRSapi-0.0.4/pySSRSapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pySSRSapi-0.0.3/setup.py` & `pySSRSapi-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pySSRSapi',
-    version='0.0.3',
+    version='0.0.4',
     description='Python SSRS API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='SSRS, API',
     author='quaik8',
     author_email='mail@example.com',
     url='https://pypi.org/project/pySSRSapi/',
```

