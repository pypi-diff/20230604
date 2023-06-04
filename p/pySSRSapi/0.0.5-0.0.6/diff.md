# Comparing `tmp/pySSRSapi-0.0.5.tar.gz` & `tmp/pySSRSapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySSRSapi-0.0.5.tar", last modified: Sun Jun  4 19:50:33 2023, max compression
+gzip compressed data, was "pySSRSapi-0.0.6.tar", last modified: Sun Jun  4 21:45:30 2023, max compression
```

## Comparing `pySSRSapi-0.0.5.tar` & `pySSRSapi-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-04 19:50:33.351568 pySSRSapi-0.0.5/
--rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-04 19:50:33.351194 pySSRSapi-0.0.5/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.5/README.md
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-04 19:50:33.347018 pySSRSapi-0.0.5/pySSRSapi/
--rw-r--r--   0 quaik8     (501) staff       (20)     8922 2023-06-04 19:49:26.000000 pySSRSapi-0.0.5/pySSRSapi/__init__.py
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-04 19:50:33.350257 pySSRSapi-0.0.5/pySSRSapi.egg-info/
--rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-04 19:50:33.000000 pySSRSapi-0.0.5/pySSRSapi.egg-info/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-04 19:50:33.000000 pySSRSapi-0.0.5/pySSRSapi.egg-info/SOURCES.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-04 19:50:33.000000 pySSRSapi-0.0.5/pySSRSapi.egg-info/dependency_links.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-04 19:50:33.000000 pySSRSapi-0.0.5/pySSRSapi.egg-info/requires.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-04 19:50:33.000000 pySSRSapi-0.0.5/pySSRSapi.egg-info/top_level.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-04 19:50:33.351672 pySSRSapi-0.0.5/setup.cfg
--rw-r--r--   0 quaik8     (501) staff       (20)      791 2023-06-04 10:39:17.000000 pySSRSapi-0.0.5/setup.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-04 21:45:30.504766 pySSRSapi-0.0.6/
+-rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-04 21:45:30.504436 pySSRSapi-0.0.6/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.6/README.md
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-04 21:45:30.500290 pySSRSapi-0.0.6/pySSRSapi/
+-rw-r--r--   0 quaik8     (501) staff       (20)     9324 2023-06-04 21:44:56.000000 pySSRSapi-0.0.6/pySSRSapi/__init__.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-04 21:45:30.503459 pySSRSapi-0.0.6/pySSRSapi.egg-info/
+-rw-r--r--   0 quaik8     (501) staff       (20)      523 2023-06-04 21:45:30.000000 pySSRSapi-0.0.6/pySSRSapi.egg-info/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-04 21:45:30.000000 pySSRSapi-0.0.6/pySSRSapi.egg-info/SOURCES.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-04 21:45:30.000000 pySSRSapi-0.0.6/pySSRSapi.egg-info/dependency_links.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-04 21:45:30.000000 pySSRSapi-0.0.6/pySSRSapi.egg-info/requires.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-04 21:45:30.000000 pySSRSapi-0.0.6/pySSRSapi.egg-info/top_level.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-04 21:45:30.504859 pySSRSapi-0.0.6/setup.cfg
+-rw-r--r--   0 quaik8     (501) staff       (20)      791 2023-06-04 21:45:20.000000 pySSRSapi-0.0.6/setup.py
```

### Comparing `pySSRSapi-0.0.5/PKG-INFO` & `pySSRSapi-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pySSRSapi-0.0.5/pySSRSapi/__init__.py` & `pySSRSapi-0.0.6/pySSRSapi/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import base64
+# import base64
 import json
 import requests
 from requests.auth import HTTPBasicAuth
 
 EP_API = '/api/v2.0'
 EP_ME = '/me'
 EP_FOLDERS = '/folders'
-EP_REPORTS = '/reports'
 EP_DATASOURCES = '/datasources'
+EP_REPORTS = '/reports'
 
 class User:
     def __init__(self, Id: str, Username: str, DisplayName: str):
         self.Id = Id
         self.Username = Username
         self.DisplayName = DisplayName
         
@@ -161,104 +161,116 @@
             json_dct['ContentType'],
             json_dct['Size']
         )
 
 class Api:
     def __init__(self, url: str, user: str, password: str):
         self.url = url + EP_API
-        self.basicAuth = HTTPBasicAuth(user, password)
+        self.basic_auth = HTTPBasicAuth(user, password)
         self.headers = {'Content-type': 'application/json;charset=UTF-8'}
+        
+    # REQUESTS
+    def __getEndpointClass(self, endpoint: str):
+        if endpoint == EP_ME:
+            return User
+        elif endpoint == EP_FOLDERS:
+            return Folder
+        elif endpoint == EP_DATASOURCES:
+            return Datasource
+
+    def __get(self, endpoint: str, args: str = ''):
+        response = requests.get(self.url + endpoint + args, auth=self.basic_auth, headers=self.headers)
+        object_hook = self.__getEndpointClass(endpoint=endpoint).from_json
+        if response.status_code == 200:
+            response_obj = json.loads(response.content)
+            if 'value' in response_obj:
+                value = json.loads(response.content)['value']
+                return json.loads(json.dumps(value), object_hook=object_hook)
+            else:
+                return json.loads(response.content, object_hook=object_hook)
+        return False
+    
+    def __post(self, endpoint: str, data: Folder|Datasource, args: str = ''):
+        response = requests.post(self.url + endpoint + args, json=data.to_obj(), auth=self.basic_auth, headers=self.headers)
+        object_hook = self.__getEndpointClass(endpoint=endpoint).from_json
+        if response.status_code == 201:
+            return json.loads(response.content, object_hook=object_hook)
+        return False
     
     # USER
     def getUser(self):
-        response = requests.get(self.url + EP_ME, auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 200:
-            return json.loads(response.content, object_hook=User.from_json)
-        return False
+        return self.__get(endpoint=EP_ME)
     
     # FOLDER
     def getFolders(self):
-        response = requests.get(self.url + EP_FOLDERS, auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 200:
-            value = json.loads(response.content)['value']
-            return json.loads(json.dumps(value), object_hook=Folder.from_json)
-        return False
+        return self.__get(endpoint=EP_FOLDERS)
     
     def getFolderById(self, id: str):
-        response = requests.get(self.url + EP_FOLDERS + '(' + id + ')', auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 200:
-            return json.loads(response.content, object_hook=Folder.from_json)
-        return False
+        return self.__get(endpoint=EP_FOLDERS, args='(' + id + ')')
     
     def getFolderByName(self, name: str):
         folders = self.getFolders()
         for f in folders:
             if f.Name == name:
                 return f
         return False
     
     def getFolderByPath(self, path: str):
-        response = requests.get(self.url + EP_FOLDERS + "(Path='" + path + "')", auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 200:
-            return json.loads(response.content, object_hook=Folder.from_json)
-        return False
+        return self.__get(endpoint=EP_FOLDERS, args="(Path='" + path + "')")
     
     def getRootFolder(self):
         return self.getFolderByPath(path = '/')
     
     def addFolder(self, folder: Folder):
-        response = requests.post(self.url + EP_FOLDERS, json=folder, auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 201:
-            return json.loads(response.text, object_hook=Folder.from_json)
-        return False
+        return self.__post(endpoint=EP_FOLDERS, data=folder)
     
-    def editFolder(self, id: str, folder: Folder):
-        response = requests.patch(self.url + EP_FOLDERS + '(' + id + ')', json=folder, auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 204:
-            return self.getFolderById(id = id)
-        return False
+    # def editFolder(self, id: str, folder: Folder):
+    #     response = requests.patch(self.url + EP_FOLDERS + '(' + id + ')', json=folder, auth=self.basic_auth, headers=self.headers)
+    #     if response.status_code == 204:
+    #         return self.getFolderById(id = id)
+    #     return False
 
-    def deleteFolder(self, id: str):
-        response = requests.delete(self.url + EP_FOLDERS + '(' + id + ')', auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 204:
-            return True
-        return False
-    
-    # DATASOURCE
-    def getDatasources(self):
-        response = requests.get(self.url + EP_DATASOURCES, auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 200:
-            value = json.loads(response.content)['value']
-            return json.loads(json.dumps(value), object_hook=Datasource.from_json)
-        return False
+    # def deleteFolder(self, id: str):
+    #     response = requests.delete(self.url + EP_FOLDERS + '(' + id + ')', auth=self.basic_auth, headers=self.headers)
+    #     if response.status_code == 204:
+    #         return True
+    #     return False
+    
+    # # DATASOURCE
+    # def getDatasources(self):
+    #     response = requests.get(self.url + EP_DATASOURCES, auth=self.basic_auth, headers=self.headers)
+    #     if response.status_code == 200:
+    #         value = json.loads(response.content)['value']
+    #         return json.loads(json.dumps(value), object_hook=Datasource.from_json)
+    #     return False
 
-    def getDatasourceById(self, id: str):
-        response = requests.get(self.url + EP_DATASOURCES + '(' + id + ')', auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 200:
-            return json.loads(response.content, object_hook=Datasource.from_json)
-        return False
+    # def getDatasourceById(self, id: str):
+    #     response = requests.get(self.url + EP_DATASOURCES + '(' + id + ')', auth=self.basic_auth, headers=self.headers)
+    #     if response.status_code == 200:
+    #         return json.loads(response.content, object_hook=Datasource.from_json)
+    #     return False
 
-    def getDatasourceByPath(self, path: str):
-        response = requests.get(self.url + EP_DATASOURCES + "(Path='" + path + "')", auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 200:
-            return json.loads(response.content, object_hook=Datasource.from_json)
-        return False
-    
-    def addDatasource(self, datasource: Datasource):
-        response = requests.post(self.url + EP_DATASOURCES, json=datasource, auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 201:
-            return json.loads(response.text, object_hook=Datasource.from_json)
-        return False
-    
-    def deleteDatasource(self, id: str):
-        response = requests.delete(self.url + EP_DATASOURCES + '(' + id + ')', auth=self.basicAuth, headers=self.headers)
-        if response.status_code == 204:
-            return True
-        return False
-    
-    # REPORT
-    
-def getB64EncodedFile(path):
-    with open(path, 'rb') as f:
-        byte_content = f.read()
-    base64_bytes = base64.b64encode(byte_content)
-    return base64_bytes.decode('utf-8')
+    # def getDatasourceByPath(self, path: str):
+    #     response = requests.get(self.url + EP_DATASOURCES + "(Path='" + path + "')", auth=self.basic_auth, headers=self.headers)
+    #     if response.status_code == 200:
+    #         return json.loads(response.content, object_hook=Datasource.from_json)
+    #     return False
+    
+    # def addDatasource(self, datasource: Datasource):
+    #     response = requests.post(self.url + EP_DATASOURCES, json=datasource, auth=self.basic_auth, headers=self.headers)
+    #     if response.status_code == 201:
+    #         return json.loads(response.text, object_hook=Datasource.from_json)
+    #     return False
+    
+    # def deleteDatasource(self, id: str):
+    #     response = requests.delete(self.url + EP_DATASOURCES + '(' + id + ')', auth=self.basic_auth, headers=self.headers)
+    #     if response.status_code == 204:
+    #         return True
+    #     return False
+    
+    # # REPORT
+    
+# def getB64EncodedFile(path):
+#     with open(path, 'rb') as f:
+#         byte_content = f.read()
+#     base64_bytes = base64.b64encode(byte_content)
+#     return base64_bytes.decode('utf-8')
```

### Comparing `pySSRSapi-0.0.5/pySSRSapi.egg-info/PKG-INFO` & `pySSRSapi-0.0.6/pySSRSapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pySSRSapi-0.0.5/setup.py` & `pySSRSapi-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pySSRSapi',
-    version='0.0.5',
+    version='0.0.6',
     description='Python SSRS API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='SSRS, API',
     author='quaik8',
     author_email='mail@example.com',
     url='https://pypi.org/project/pySSRSapi/',
```

