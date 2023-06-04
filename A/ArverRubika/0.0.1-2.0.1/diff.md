# Comparing `tmp/ArverRubika-0.0.1.tar.gz` & `tmp/ArverRubika-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ArverRubika-0.0.1.tar", last modified: Mon Apr 24 06:24:06 2023, max compression
+gzip compressed data, was "ArverRubika-2.0.1.tar", last modified: Sun Jun  4 16:15:29 2023, max compression
```

## Comparing `ArverRubika-0.0.1.tar` & `ArverRubika-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 06:24:06.707458 ArverRubika-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-24 06:24:06.443791 ArverRubika-0.0.1/ArverRubika/
-drwxrwxrwx   0        0        0        0 2023-04-24 06:24:06.614334 ArverRubika-0.0.1/ArverRubika/ArverMaker/
--rw-rw-rw-   0        0        0     2155 2023-04-24 04:46:38.000000 ArverRubika-0.0.1/ArverRubika/ArverMaker/__init__.py
--rw-rw-rw-   0        0        0     1388 2023-04-24 06:26:00.000000 ArverRubika-0.0.1/ArverRubika/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:24:06.679455 ArverRubika-0.0.1/ArverRubika/cryptos/
--rw-rw-rw-   0        0        0     1164 2023-04-21 03:31:00.000000 ArverRubika-0.0.1/ArverRubika/cryptos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:24:06.699457 ArverRubika-0.0.1/ArverRubika/servers/
--rw-rw-rw-   0        0        0      326 2023-04-21 03:38:24.000000 ArverRubika-0.0.1/ArverRubika/servers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:24:06.550641 ArverRubika-0.0.1/ArverRubika.egg-info/
--rw-rw-rw-   0        0        0      479 2023-04-24 06:24:02.000000 ArverRubika-0.0.1/ArverRubika.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-04-24 06:24:03.000000 ArverRubika-0.0.1/ArverRubika.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 06:24:02.000000 ArverRubika-0.0.1/ArverRubika.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-24 06:24:02.000000 ArverRubika-0.0.1/ArverRubika.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-24 06:24:02.000000 ArverRubika-0.0.1/ArverRubika.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      479 2023-04-24 06:24:06.704459 ArverRubika-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-24 06:24:06.708472 ArverRubika-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      888 2023-04-24 06:20:45.000000 ArverRubika-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 16:15:29.890447 ArverRubika-2.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-04 16:15:29.576714 ArverRubika-2.0.1/ArverRubika/
+drwxrwxrwx   0        0        0        0 2023-06-04 16:15:29.765038 ArverRubika-2.0.1/ArverRubika/ArverMaker/
+-rw-rw-rw-   0        0        0     2382 2023-06-04 14:43:20.000000 ArverRubika-2.0.1/ArverRubika/ArverMaker/__init__.py
+-rw-rw-rw-   0        0        0     3493 2023-06-04 14:43:20.000000 ArverRubika-2.0.1/ArverRubika/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 16:15:29.816926 ArverRubika-2.0.1/ArverRubika/cryptos/
+-rw-rw-rw-   0        0        0     1164 2023-06-04 14:43:20.000000 ArverRubika-2.0.1/ArverRubika/cryptos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 16:15:29.890447 ArverRubika-2.0.1/ArverRubika/servers/
+-rw-rw-rw-   0        0        0      326 2023-06-04 14:43:20.000000 ArverRubika-2.0.1/ArverRubika/servers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 16:15:29.765038 ArverRubika-2.0.1/ArverRubika.egg-info/
+-rw-rw-rw-   0        0        0      815 2023-06-04 16:15:29.000000 ArverRubika-2.0.1/ArverRubika.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-04 16:15:29.000000 ArverRubika-2.0.1/ArverRubika.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 16:15:29.000000 ArverRubika-2.0.1/ArverRubika.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-04 16:15:29.000000 ArverRubika-2.0.1/ArverRubika.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-04 16:15:29.000000 ArverRubika-2.0.1/ArverRubika.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-06-04 15:52:38.000000 ArverRubika-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0      815 2023-06-04 16:15:29.890447 ArverRubika-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-04 15:56:20.000000 ArverRubika-2.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 16:15:29.890447 ArverRubika-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2023-06-04 16:03:20.000000 ArverRubika-2.0.1/setup.py
```

### Comparing `ArverRubika-0.0.1/ArverRubika/ArverMaker/__init__.py` & `ArverRubika-2.0.1/ArverRubika/ArverMaker/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,20 +47,25 @@
             'POST',
             self.server,
             body = dumps(data).encode(),
             headers = {'Cookie': 'Arver Library'}
         )
         result = loads(self.crypto.decrypt(loads(result.data.decode('utf-8'))['data_enc']))
         if result['status'] == 'OK':
-            return result
+            if result == None:
+            	raise IndexError("Auth is Not True .!")
+            else:
+            	return result
         elif result['status'] in ['ERROR_GENERIC', 'ERROR_ACTION']:
             if result['status_det'] == 'INVALID_AUTH':
-                raise IndexError("Auth Not True .!")
+                raise IndexError("Auth is Not True .!")
+            elif result['status_det'] == 'NOT_REGISTERED':
+            	raise IndexError("Auth is Not True .!")
             else:
-                pass
+                return result
     def _upload(self, url, data, headers):
         while True:
             req = post(url=url, data=data, headers=headers)
             if req.status_code != 200:
                 "This file cannot be uploaded ! Trying to upload again ..."
                 continue
             return req.json()
```

### Comparing `ArverRubika-0.0.1/ArverRubika/cryptos/__init__.py` & `ArverRubika-2.0.1/ArverRubika/cryptos/__init__.py`

 * *Files identical despite different names*

### Comparing `ArverRubika-0.0.1/setup.py` & `ArverRubika-2.0.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from setuptools import setup, find_packages
 
+with open('README.md', 'r') as fl :
+    long_description = fl.read()
+
 setup(
         # the name must match the folder name 'verysimplemodule'
         name="ArverRubika", 
-        version='0.0.1',
+        version='2.0.1',
         author="Aboli Coder",
-        author_email="",
+        author_email="mirzaiabolfazl6@gmail.com",
         description='Coding the robot in Rubika in the easiest way !',
-        long_description='none',
+        long_description=long_description,
+        long_description_content_type= 'text/markdown',
         packages=find_packages(),
         
         # add any additional packages that 
         # needs to be installed along with your package.
         install_requires=["pycryptodome==3.16.0", "Pillow==9.4.0"], 
         
-        keywords=['python', 'rubel', 'Rubika', 'ArverRubika', 'robika', 'robot'],
+        keywords=['python', 'rubel', 'Rubika', 'ArverRubika', 'robika', 'robot', 'ArseinRubika', 'arsein', 'arver', 'Arver', 'pyrubi'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
+            "License :: OSI Approved :: MIT License",
             "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
         ]
 )
```

