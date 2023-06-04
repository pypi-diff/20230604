# Comparing `tmp/aquarium-python-api-2.0.0.tar.gz` & `tmp/aquarium-python-api-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquarium-python-api-2.0.0.tar", last modified: Sat Apr 15 09:32:25 2023, max compression
+gzip compressed data, was "dist/aquarium-python-api-2.0.1.tar", last modified: Sun Jun  4 09:16:07 2023, max compression
```

## Comparing `aquarium-python-api-2.0.0.tar` & `aquarium-python-api-2.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-04-15 09:32:25.028462 aquarium-python-api-2.0.0/
--rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.0/LICENSE.md
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-04-15 09:32:25.028681 aquarium-python-api-2.0.0/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.0/README.md
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-04-15 09:32:25.001463 aquarium-python-api-2.0.0/aquarium/
--rw-r--r--   0 yann       (501) staff       (20)      917 2021-02-01 10:01:21.000000 aquarium-python-api-2.0.0/aquarium/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)    12537 2023-04-15 09:11:35.000000 aquarium-python-api-2.0.0/aquarium/aquarium.py
--rw-r--r--   0 yann       (501) staff       (20)     3399 2022-11-09 16:10:59.000000 aquarium-python-api-2.0.0/aquarium/edge.py
--rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.0/aquarium/element.py
--rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.0/aquarium/entity.py
--rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.0/aquarium/exceptions.py
--rw-r--r--   0 yann       (501) staff       (20)    26536 2023-04-15 08:46:19.000000 aquarium-python-api-2.0.0/aquarium/item.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-04-15 09:32:25.023566 aquarium-python-api-2.0.0/aquarium/items/
--rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.0/aquarium/items/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.0/aquarium/items/asset.py
--rw-r--r--   0 yann       (501) staff       (20)     5092 2023-04-15 09:03:56.000000 aquarium-python-api-2.0.0/aquarium/items/organisation.py
--rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.0/aquarium/items/playlist.py
--rw-r--r--   0 yann       (501) staff       (20)     2278 2022-10-07 09:30:26.000000 aquarium-python-api-2.0.0/aquarium/items/project.py
--rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.0/aquarium/items/shot.py
--rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.0/aquarium/items/task.py
--rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.0/aquarium/items/template.py
--rw-r--r--   0 yann       (501) staff       (20)     4087 2022-11-05 08:59:00.000000 aquarium-python-api-2.0.0/aquarium/items/user.py
--rw-r--r--   0 yann       (501) staff       (20)     1653 2021-02-19 09:03:04.000000 aquarium-python-api-2.0.0/aquarium/items/usergroup.py
--rw-r--r--   0 yann       (501) staff       (20)     1870 2023-04-15 07:32:38.000000 aquarium-python-api-2.0.0/aquarium/tools.py
--rw-r--r--   0 yann       (501) staff       (20)     3823 2023-02-07 11:39:40.000000 aquarium-python-api-2.0.0/aquarium/utils.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-04-15 09:32:25.028041 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/
--rw-r--r--   0 yann       (501) staff       (20)     3238 2023-04-15 09:32:24.000000 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)      686 2023-04-15 09:32:24.000000 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yann       (501) staff       (20)        1 2023-04-15 09:32:24.000000 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yann       (501) staff       (20)      123 2023-04-15 09:32:24.000000 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/requires.txt
--rw-r--r--   0 yann       (501) staff       (20)        9 2023-04-15 09:32:24.000000 aquarium-python-api-2.0.0/aquarium_python_api.egg-info/top_level.txt
--rw-r--r--   0 yann       (501) staff       (20)     1280 2023-04-15 09:32:25.030188 aquarium-python-api-2.0.0/setup.cfg
--rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.0/setup.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-04 09:16:07.279075 aquarium-python-api-2.0.1/
+-rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.0.1/LICENSE.md
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-04 09:16:07.279320 aquarium-python-api-2.0.1/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.0.1/README.md
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-04 09:16:07.257981 aquarium-python-api-2.0.1/aquarium/
+-rw-r--r--   0 yann       (501) staff       (20)      917 2021-02-01 10:01:21.000000 aquarium-python-api-2.0.1/aquarium/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)    12537 2023-04-15 09:11:35.000000 aquarium-python-api-2.0.1/aquarium/aquarium.py
+-rw-r--r--   0 yann       (501) staff       (20)     3399 2022-11-09 16:10:59.000000 aquarium-python-api-2.0.1/aquarium/edge.py
+-rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.0.1/aquarium/element.py
+-rw-r--r--   0 yann       (501) staff       (20)     2899 2022-11-09 16:11:03.000000 aquarium-python-api-2.0.1/aquarium/entity.py
+-rw-r--r--   0 yann       (501) staff       (20)      941 2023-04-15 08:48:21.000000 aquarium-python-api-2.0.1/aquarium/exceptions.py
+-rw-r--r--   0 yann       (501) staff       (20)    26695 2023-06-04 09:10:20.000000 aquarium-python-api-2.0.1/aquarium/item.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-04 09:16:07.273574 aquarium-python-api-2.0.1/aquarium/items/
+-rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.0.1/aquarium/items/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)     6444 2022-10-24 12:24:48.000000 aquarium-python-api-2.0.1/aquarium/items/asset.py
+-rw-r--r--   0 yann       (501) staff       (20)     5092 2023-04-15 09:03:56.000000 aquarium-python-api-2.0.1/aquarium/items/organisation.py
+-rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.0.1/aquarium/items/playlist.py
+-rw-r--r--   0 yann       (501) staff       (20)     2307 2023-06-04 08:20:45.000000 aquarium-python-api-2.0.1/aquarium/items/project.py
+-rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.0.1/aquarium/items/shot.py
+-rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.0.1/aquarium/items/task.py
+-rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.0.1/aquarium/items/template.py
+-rw-r--r--   0 yann       (501) staff       (20)     4087 2022-11-05 08:59:00.000000 aquarium-python-api-2.0.1/aquarium/items/user.py
+-rw-r--r--   0 yann       (501) staff       (20)     1653 2021-02-19 09:03:04.000000 aquarium-python-api-2.0.1/aquarium/items/usergroup.py
+-rw-r--r--   0 yann       (501) staff       (20)     2232 2023-06-04 09:10:43.000000 aquarium-python-api-2.0.1/aquarium/tools.py
+-rw-r--r--   0 yann       (501) staff       (20)     3823 2023-06-04 09:15:02.000000 aquarium-python-api-2.0.1/aquarium/utils.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2023-06-04 09:16:07.278419 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/
+-rw-r--r--   0 yann       (501) staff       (20)     3238 2023-06-04 09:16:06.000000 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)      686 2023-06-04 09:16:06.000000 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yann       (501) staff       (20)        1 2023-06-04 09:16:06.000000 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yann       (501) staff       (20)      123 2023-06-04 09:16:06.000000 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/requires.txt
+-rw-r--r--   0 yann       (501) staff       (20)        9 2023-06-04 09:16:06.000000 aquarium-python-api-2.0.1/aquarium_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yann       (501) staff       (20)     1280 2023-06-04 09:16:07.280346 aquarium-python-api-2.0.1/setup.cfg
+-rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.0.1/setup.py
```

### Comparing `aquarium-python-api-2.0.0/LICENSE.md` & `aquarium-python-api-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/PKG-INFO` & `aquarium-python-api-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.0/README.md` & `aquarium-python-api-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/__init__.py` & `aquarium-python-api-2.0.1/aquarium/__init__.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/aquarium.py` & `aquarium-python-api-2.0.1/aquarium/aquarium.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/edge.py` & `aquarium-python-api-2.0.1/aquarium/edge.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/element.py` & `aquarium-python-api-2.0.1/aquarium/element.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/entity.py` & `aquarium-python-api-2.0.1/aquarium/entity.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/exceptions.py` & `aquarium-python-api-2.0.1/aquarium/exceptions.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/item.py` & `aquarium-python-api-2.0.1/aquarium/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 from . import URL_CONTENT_TYPE
 import json
 import re
 import os
 from .tools import to_string_url
+from .tools import jsonify
 from .entity import Entity
 from .exceptions import Deprecated
 import logging
 logger = logging.getLogger(__name__)
 
 
 class Item(Entity):
@@ -301,28 +302,40 @@
         :rtype:     list of :class:`~aquarium.item.Item` or subclass : :class:`~aquarium.items.asset.Asset` | :class:`~aquarium.items.project.Project` | :class:`~aquarium.items.shot.Shot` | :class:`~aquarium.items.task.Task` | :class:`~aquarium.items.template.Template` | :class:`~aquarium.items.user.User` | :class:`~aquarium.items.usergroup.Usergroup`
         """
         result = self.do_request(
             'GET', 'items/'+self._key+'/path/'+key, headers=URL_CONTENT_TYPE)
         result = [self.parent.cast(data) for data in result]
         return result
 
-    def get_permissions(self, filters={}, populate=False):
+    def get_permissions(self, sort=None, populate=False, offset=0, limit=50, depth=1, includeMembers=False):
         """
         Gets the permissions of the item
 
-        :param      filters:   The filters
-        :type       filters:   dictionary, optional
+
         :param      populate:  Populate with User object
         :type       populate:  boolean, optional
 
         :returns:   List of edge and user
         :rtype:     list
         """
-        result = self.do_request('GET', 'items/{0}/permissions?filters={1}&populate={2}'.format(
-            self._key, str(filters).replace("'", '"'), to_string_url(populate)), headers=URL_CONTENT_TYPE)
+        params = dict(
+            populate=populate,
+            offset=offset,
+            limit=limit,
+            depth=depth,
+            includeMembers=includeMembers
+        )
+
+        if sort != None:
+            params['sort'] = sort
+
+        jsonify(params)
+
+        result = self.do_request('GET', 'items/{0}/permissions'.format(
+            self._key), params=params)
         result = [self.parent.element(data) for data in result]
         return result
 
     def create_permission(self, participant_key, permissions, propagate = True):
         """
         Create a new permission on an item. It's like sharing an item to an existing user, usergroup or organisation.
```

### Comparing `aquarium-python-api-2.0.0/aquarium/items/asset.py` & `aquarium-python-api-2.0.1/aquarium/items/asset.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/items/organisation.py` & `aquarium-python-api-2.0.1/aquarium/items/organisation.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/items/playlist.py` & `aquarium-python-api-2.0.1/aquarium/items/playlist.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/items/project.py` & `aquarium-python-api-2.0.1/aquarium/items/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,20 +14,20 @@
         :param      show_all:  Add completed and trashed projects
         :type       show_all:  boolean, optional
 
         :returns:   List of Project class
         :rtype:     List of :class:`~aquarium.items.project.Project`
         """
         query = list()
-        query.append('# ($Project')
+        query.append('# $Project')
 
         if not show_all:
-            query.append('AND item.data.completion != 1 AND NOT <($Trash)- *)')
+            query.append('AND item.data.completion != 1 AND item.data.completion != -1 AND NOT (<($Trash)- *)')
 
-        query.append(') SORT item.data.name ASC')
+        query.append('SORT item.data.name ASC')
         result = self.parent.query(meshql=' '.join(query))
         result = [self.parent.cast(data) for data in result]
         return result
 
     def get_shots(self):
         """
         Gets all the shots of the project
```

### Comparing `aquarium-python-api-2.0.0/aquarium/items/task.py` & `aquarium-python-api-2.0.1/aquarium/items/task.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/items/template.py` & `aquarium-python-api-2.0.1/aquarium/items/template.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/items/user.py` & `aquarium-python-api-2.0.1/aquarium/items/user.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/items/usergroup.py` & `aquarium-python-api-2.0.1/aquarium/items/usergroup.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium/utils.py` & `aquarium-python-api-2.0.1/aquarium/utils.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/aquarium_python_api.egg-info/PKG-INFO` & `aquarium-python-api-2.0.1/aquarium_python_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.0.0/aquarium_python_api.egg-info/SOURCES.txt` & `aquarium-python-api-2.0.1/aquarium_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.0.0/setup.cfg` & `aquarium-python-api-2.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://docs.fatfish.app/dev/python/index.html
 project_urls = 
 	Documentation = https://docs.fatfish.app/dev/python/index.html
 	Source = https://github.com/fatfish-lab/aquarium-python-api
 	Aquarium = https://fatfi.sh/aquarium
-version = 2.0.0
+version = 2.0.1
 author = Fatfish Lab
 author_email = lab@fatfi.sh
 keywords = fatfish, lab, aquarium, studio, project, management, nodal, sdk, rest, cgi, vfx, api, python
 license = gpl-3.0
 license_file = LICENSE.md
 platform = any
 python_requires = '>=2.4'
```

