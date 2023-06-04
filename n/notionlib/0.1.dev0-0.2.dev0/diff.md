# Comparing `tmp/notionlib-0.1.dev0.tar.gz` & `tmp/notionlib-0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notionlib-0.1.dev0.tar", last modified: Thu Jul 14 22:16:12 2022, max compression
+gzip compressed data, was "notionlib-0.2.dev0.tar", last modified: Sun Jun  4 20:45:48 2023, max compression
```

## Comparing `notionlib-0.1.dev0.tar` & `notionlib-0.2.dev0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2022-07-14 22:16:12.804249 notionlib-0.1.dev0/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       52 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/AUTHORS
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       17 2022-07-14 21:45:57.000000 notionlib-0.1.dev0/BUGS.md
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       56 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/CHANGES.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1092 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/LICENSE
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      397 2022-07-14 21:45:57.000000 notionlib-0.1.dev0/MANIFEST.in
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     3792 2022-07-14 22:16:12.804249 notionlib-0.1.dev0/PKG-INFO
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      463 2022-07-14 21:45:57.000000 notionlib-0.1.dev0/PUBLISH_HOWTO.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     2901 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/README.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      228 2022-07-14 21:45:57.000000 notionlib-0.1.dev0/TODO.md
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2022-07-14 22:16:12.804249 notionlib-0.1.dev0/docs/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7618 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/docs/Makefile
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      287 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/docs/api.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      126 2022-07-14 21:45:57.000000 notionlib-0.1.dev0/docs/api_TODO_MODULE_NAME.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)    10912 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/docs/conf.py
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     5257 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/docs/developer.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      779 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/docs/index.rst
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      864 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/docs/init_sphinx.sh
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      207 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/docs/intro.rst
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7738 2022-07-14 22:06:12.000000 notionlib-0.1.dev0/docs/make.bat
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2022-07-14 22:16:12.804249 notionlib-0.1.dev0/notionlib/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1141 2022-07-14 22:12:45.000000 notionlib-0.1.dev0/notionlib/__init__.py
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)    19876 2022-07-14 15:59:19.000000 notionlib-0.1.dev0/notionlib/notion.py
-drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2022-07-14 22:16:12.804249 notionlib-0.1.dev0/notionlib.egg-info/
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     3792 2022-07-14 22:16:12.000000 notionlib-0.1.dev0/notionlib.egg-info/PKG-INFO
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      453 2022-07-14 22:16:12.000000 notionlib-0.1.dev0/notionlib.egg-info/SOURCES.txt
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)        1 2022-07-14 22:16:12.000000 notionlib-0.1.dev0/notionlib.egg-info/dependency_links.txt
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       10 2022-07-14 22:16:12.000000 notionlib-0.1.dev0/notionlib.egg-info/top_level.txt
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       84 2022-07-14 21:45:57.000000 notionlib-0.1.dev0/pyproject.toml
--rw-rw-r--   0 jeremie   (1010) jeremie   (1010)        0 2022-07-14 21:45:57.000000 notionlib-0.1.dev0/requirements.txt
--rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      946 2022-07-14 22:16:12.804249 notionlib-0.1.dev0/setup.cfg
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 20:45:48.138593 notionlib-0.2.dev0/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       52 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/AUTHORS
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       17 2022-07-14 21:45:57.000000 notionlib-0.2.dev0/BUGS.md
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       56 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/CHANGES.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1092 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/LICENSE
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      397 2022-07-14 21:45:57.000000 notionlib-0.2.dev0/MANIFEST.in
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     3822 2023-06-04 20:45:48.138593 notionlib-0.2.dev0/PKG-INFO
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      465 2023-06-04 20:37:53.000000 notionlib-0.2.dev0/PUBLISH_HOWTO.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     2901 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/README.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      228 2022-07-14 21:45:57.000000 notionlib-0.2.dev0/TODO.md
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 20:45:48.134592 notionlib-0.2.dev0/docs/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7618 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/Makefile
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      287 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/api.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      126 2022-07-14 21:45:57.000000 notionlib-0.2.dev0/docs/api_TODO_MODULE_NAME.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)    10912 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/conf.py
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     5257 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/developer.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      779 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/index.rst
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      864 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/init_sphinx.sh
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      207 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/intro.rst
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     7738 2022-07-14 22:06:12.000000 notionlib-0.2.dev0/docs/make.bat
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 20:45:48.138593 notionlib-0.2.dev0/notionlib/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     1177 2023-06-04 20:36:54.000000 notionlib-0.2.dev0/notionlib/__init__.py
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)    23555 2023-06-04 20:30:01.000000 notionlib-0.2.dev0/notionlib/notion.py
+drwxrwxr-x   0 jeremie   (1010) jeremie   (1010)        0 2023-06-04 20:45:48.138593 notionlib-0.2.dev0/notionlib.egg-info/
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)     3822 2023-06-04 20:45:48.000000 notionlib-0.2.dev0/notionlib.egg-info/PKG-INFO
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)      462 2023-06-04 20:45:48.000000 notionlib-0.2.dev0/notionlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)        1 2023-06-04 20:45:48.000000 notionlib-0.2.dev0/notionlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       10 2023-06-04 20:45:48.000000 notionlib-0.2.dev0/notionlib.egg-info/top_level.txt
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       76 2023-06-04 20:45:17.000000 notionlib-0.2.dev0/pyproject.toml
+-rw-rw-r--   0 jeremie   (1010) jeremie   (1010)       15 2022-07-24 14:13:07.000000 notionlib-0.2.dev0/requirements.txt
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)      946 2023-06-04 20:45:48.138593 notionlib-0.2.dev0/setup.cfg
+-rwxrwxr-x   0 jeremie   (1010) jeremie   (1010)     2922 2022-07-14 22:35:14.000000 notionlib-0.2.dev0/setup.py
```

### Comparing `notionlib-0.1.dev0/LICENSE` & `notionlib-0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `notionlib-0.1.dev0/PKG-INFO` & `notionlib-0.2.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: notionlib
-Version: 0.1.dev0
-Summary: An unofficial Python 3 client for Notion.so API
+Version: 0.2.dev0
+Summary: An unofficial Python 3 client for the Notion.so API
 Home-page: https://github.com/jdhp/notion-lib
+Download-URL: 
 Author: Jérémie DECOCK
 Author-email: jd.jdhp@gmail.com
+Maintainer: Jérémie DECOCK
+Maintainer-email: jd.jdhp@gmail.com
 Project-URL: Bug Tracker, https://github.com/jdhp/notion-lib/issues
-Keywords: notionlib
+Keywords: Gitlab
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.6
```

### Comparing `notionlib-0.1.dev0/README.rst` & `notionlib-0.2.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `notionlib-0.1.dev0/docs/Makefile` & `notionlib-0.2.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `notionlib-0.1.dev0/docs/conf.py` & `notionlib-0.2.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `notionlib-0.1.dev0/docs/developer.rst` & `notionlib-0.2.dev0/docs/developer.rst`

 * *Files identical despite different names*

### Comparing `notionlib-0.1.dev0/docs/index.rst` & `notionlib-0.2.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `notionlib-0.1.dev0/docs/init_sphinx.sh` & `notionlib-0.2.dev0/docs/init_sphinx.sh`

 * *Files identical despite different names*

### Comparing `notionlib-0.1.dev0/docs/make.bat` & `notionlib-0.2.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `notionlib-0.1.dev0/notionlib/__init__.py` & `notionlib-0.2.dev0/notionlib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ``<TAB>`` refers to the TAB key), or use ``notionlib.*get_version*?<ENTER>`` (where
 ``<ENTER>`` refers to the ENTER key) to narrow down the list.  To view the
 docstring for a function, use ``notionlib.get_version?<ENTER>`` (to view the
 docstring) and ``notionlib.get_version??<ENTER>`` (to view the source code).
 """
 
 import notionlib.notion
+from notionlib.notion import Notion
 
 # PEP0440 compatible formatted version, see:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # Generic release markers:
 # X.Y
 # X.Y.Z # For bugfix releases  
@@ -29,13 +30,13 @@
 # X.YbN # Beta release         
 # X.YrcN # Release Candidate   
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '0.1.dev0'
+__version__ = '0.2.dev0'
 
 def get_version():
     return __version__
 
 __all__ = ['TODO']
```

### Comparing `notionlib-0.1.dev0/notionlib/notion.py` & `notionlib-0.2.dev0/notionlib/notion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import datetime
 import json
 import os
 import pandas as pd
 import requests
 import urllib.request
+import time
+import warnings
 
 #PERSON_PROPERTY = "email"
 PERSON_PROPERTY = "id"
+SLEEP_ERROR_SEC = 1
 
 
 class Notion:
 
     def __init__(self, api_token):
         self.api_token = api_token
         #self.api_version = "2022-06-28" # Breaks everything!
@@ -69,15 +72,15 @@
 
         for k, v in resp.json()["properties"].items():
             value_dict[k] = self.parse_database_property_object(v)
 
         return value_dict
 
 
-    def query_a_database(self, notion_db_id, return_dataframe=False, ignored_properties=None, ignored_properties_type=None):
+    def query_a_database(self, notion_db_id, return_dataframe=False, ignored_properties=None, ignored_properties_type=None, timeout=60):
         """
         Gets a list of Pages contained in the database.
 
         https://developers.notion.com/reference/post-database-query
 
         Parameters
         ----------
@@ -118,43 +121,56 @@
         if ignored_properties is None:
             ignored_properties = []
         elif isinstance(ignored_properties, str):
             ignored_properties = [ignored_properties]
 
         has_more = True
         while has_more:
-            resp = requests.post(url, headers=self.request_header, data=json.dumps(requests_data_dict))
+            is_successful_request = False
+            retry = 10
+            while (is_successful_request==False) and (retry > 0):
+                resp = requests.post(url, headers=self.request_header, data=json.dumps(requests_data_dict, default=str), timeout=timeout)
 
-            if resp.status_code != 200:
+                if resp.status_code == 200:
+                    is_successful_request = True
+                else:
+                    err_msg = f"{datetime.datetime.now().isoformat()} Error {resp.status_code} ({resp.reason}) on {url} ; wait {SLEEP_ERROR_SEC} seconds before the next retry ({retry} remaining retries)"
+                    warnings.warn(err_msg)
+                    with open("errors.log", "a") as fd:
+                        print(err_msg, file=fd)
+                    time.sleep(SLEEP_ERROR_SEC)
+                    retry -= 1
+
+            if is_successful_request:
+                for page in resp.json()['results']:
+                    page_dict = {
+                        'page_id': page['id'],
+                        'created_time': datetime.datetime.strptime(page['created_time'], r"%Y-%m-%dT%H:%M:%S.000Z"),
+                        'created_by': page['created_by']['id'],
+                        'last_edited_time': datetime.datetime.strptime(page['last_edited_time'], r"%Y-%m-%dT%H:%M:%S.000Z"),
+                        'last_edited_by': page['last_edited_by']['id']
+                    }
+
+                    for property, property_dict in page["properties"].items():
+                        if (property not in ignored_properties) and (property_dict["type"] not in ignored_properties_type):
+                            if property not in RESERVED_PROPERTY_NAMES:
+                                page_dict[property] = self.parse_database_property_object(property_dict)
+                            else:
+                                raise ValueError(f'Property name "{property}" is reserved... Please rename this property in Notion.')    # TODO: it suck... Improve it!
+
+                    notion_page_dict_list.append(page_dict)
+            else:
                 # https://developers.notion.com/reference/post-database-query#errors
                 msg = os.linesep.join([
-                        resp.reason,
-                        "; ".join([f"{k}: {v}" for k, v in resp.json().items()]),
-                        json.dumps(requests_data_dict)
+                        f"Error {resp.status_code} ({resp.reason}) on {url}",
+                        #"; ".join([f"{k}: {v}" for k, v in resp.json().items()]),
+                        json.dumps(requests_data_dict, default=str)
                     ])
                 raise Exception(msg)
 
-            for page in resp.json()['results']:
-                page_dict = {
-                    'page_id': page['id'],
-                    'created_time': datetime.datetime.strptime(page['created_time'], r"%Y-%m-%dT%H:%M:%S.000Z"),
-                    'created_by': page['created_by']['id'],
-                    'last_edited_time': datetime.datetime.strptime(page['last_edited_time'], r"%Y-%m-%dT%H:%M:%S.000Z"),
-                    'last_edited_by': page['last_edited_by']['id']
-                }
-
-                for property, property_dict in page["properties"].items():
-                    if (property not in ignored_properties) and (property_dict["type"] not in ignored_properties_type):
-                        if property not in RESERVED_PROPERTY_NAMES:
-                            page_dict[property] = self.parse_database_property_object(property_dict)
-                        else:
-                            raise ValueError(f'Property name "{property}" is reserved... Please rename this property in Notion.')    # TODO: it suck... Improve it!
-
-                notion_page_dict_list.append(page_dict)
-
             has_more = resp.json()['has_more']
 
             if has_more:
                 requests_data_dict = {
                     "page_size": 100,
                     "start_cursor": resp.json()['next_cursor']
                 }
@@ -340,25 +356,45 @@
             # https://developers.notion.com/reference/property-item-object#checkbox-property-values
             value =  property_dict["checkbox"]
 
         elif property_dict["type"] == "url":
             # https://developers.notion.com/reference/property-item-object#url-property-values
             value =  property_dict["url"]
 
+        elif property_dict["type"] == "last_edited_time":
+            # https://developers.notion.com/reference/property-item-object#url-property-values
+            value = self.parse_notion_datetime_str(property_dict["last_edited_time"])
+
+        elif property_dict["type"] == "created_by":
+            # https://developers.notion.com/reference/property-item-object#created-by-property-values
+            value = property_dict["created_by"]["id"]
+            #if "person" in property_dict["created_by"]:
+            #    value = property_dict["created_by"]["person"]["email"]    # TODO : use ID instead !!!
+            #else:
+            #    value = None
+
+        elif property_dict["type"] == "created_time":
+            # https://developers.notion.com/reference/property-item-object#created-by-property-values
+            value = self.parse_notion_datetime_str(property_dict["created_time"])
+            #if "person" in property_dict["created_by"]:
+            #    value = property_dict["created_by"]["person"]["email"]    # TODO : use ID instead !!!
+            #else:
+            #    value = None
+
         else:
             raise Exception(f'Unknown property type "{property_dict["type"]}"')
 
         return value
 
 
     ###########################################################################
     # MAKE PAGES ##############################################################
     ###########################################################################
 
-    def create_a_page(self, notion_db_id, properties, verbose=False):
+    def create_a_page(self, notion_db_id, properties, verbose=False, timeout=60):
         # https://developers.notion.com/reference/post-page
 
         data_dict = {
             "parent": {
                 "database_id": notion_db_id
             },
             "properties": {}
@@ -368,30 +404,43 @@
             notion_property_type = notion_property_dict["type"]
             notion_property_value = notion_property_dict["value"]
             if notion_property_value is not None:
                 data_dict["properties"][notion_property_name] = self.make_property(type=notion_property_type, value=notion_property_value)
 
         url = f"https://api.notion.com/v1/pages"
 
-        resp = requests.post(url, headers=self.request_header, data=json.dumps(data_dict))
+        is_successful_request = False
+        retry = 10
+        while (is_successful_request==False) and (retry > 0):
+            resp = requests.post(url, headers=self.request_header, data=json.dumps(data_dict, default=str), timeout=timeout)
 
-        if resp.status_code != 200:
+            if resp.status_code == 200:
+                is_successful_request = True
+            else:
+                err_msg = f"{datetime.datetime.now().isoformat()} Error {resp.status_code} ({resp.reason}) on {url} ; wait {SLEEP_ERROR_SEC} seconds before the next retry ({retry} remaining retries)"
+                warnings.warn(err_msg)
+                with open("errors.log", "a") as fd:
+                    print(err_msg, file=fd)
+                time.sleep(SLEEP_ERROR_SEC)
+                retry -= 1
+
+        if not is_successful_request:
             # C.f. https://developers.notion.com/reference/post-page#errors
             if resp.status_code == 404:
                 raise Exception("The specified parent database or page does not exist, or if the integration does not have access to the parent")
             else:
                 msg = os.linesep.join([
                     resp.reason,
                     "; ".join([f"{k}: {v}" for k, v in resp.json().items()]),
-                    json.dumps(data_dict)
+                    json.dumps(data_dict, default=str)
                 ])
                 raise Exception(msg)
 
         if verbose:
-            print(json.dumps(resp.json(), sort_keys=False, indent=4))
+            print(json.dumps(resp.json(), default=str, sort_keys=False, indent=4))
         
         return resp.json()
 
 
     def update_a_page(self, notion_page_id, properties):
         # https://developers.notion.com/reference/patch-page
 
@@ -403,22 +452,35 @@
             notion_property_type = notion_property_dict["type"]
             notion_property_value = notion_property_dict["value"]
             if notion_property_value is not None:
                 data_dict["properties"][notion_property_name] = self.make_property(type=notion_property_type, value=notion_property_value)
 
         url = f"https://api.notion.com/v1/pages/{notion_page_id}"
 
-        resp = requests.patch(url, headers=self.request_header, data=json.dumps(data_dict))
+        is_successful_request = False
+        retry = 10
+        while (is_successful_request==False) and (retry > 0):
+            resp = requests.patch(url, headers=self.request_header, data=json.dumps(data_dict, default=str))
 
-        if resp.status_code != 200:
+            if resp.status_code == 200:
+                is_successful_request = True
+            else:
+                err_msg = f"{datetime.datetime.now().isoformat()} Error {resp.status_code} ({resp.reason}) on {url} ; wait {SLEEP_ERROR_SEC} seconds before the next retry ({retry} remaining retries)"
+                warnings.warn(err_msg)
+                with open("errors.log", "a") as fd:
+                    print(err_msg, file=fd)
+                time.sleep(SLEEP_ERROR_SEC)
+                retry -= 1
+
+        if not is_successful_request:
             # https://developers.notion.com/reference/patch-page#errors
             msg = os.linesep.join([
                     resp.reason,
                     "; ".join([f"{k}: {v}" for k, v in resp.json().items()]),
-                    json.dumps(data_dict)
+                    json.dumps(data_dict, default=str)
                 ])
             raise Exception(msg)
 
         return resp.json()
 
 
     def check_value_type(self, value, expected_types):
@@ -489,15 +551,21 @@
 
         elif type == "rollup":
             # https://developers.notion.com/reference/property-value-object#rollup-property-values
             raise NotImplementedError()  # TODO !!!
 
         elif type == "people":
             # https://developers.notion.com/reference/property-value-object#people-property-values
-            raise NotImplementedError()  # TODO !!!
+            self.check_value_type(value, (str, list, tuple))
+            if isinstance(value, str):
+                property_dict["people"] = [{"id": value}]
+            elif isinstance(value, list, tuple):
+                property_dict["people"] = []
+                for page_id in value:
+                    property_dict["relation"].append({"id": page_id})
 
         elif type == "files":
             # https://developers.notion.com/reference/property-value-object#files-property-values
             raise NotImplementedError()  # TODO !!!
 
         elif type == "checkbox":
             # https://developers.notion.com/reference/property-value-object#checkbox-property-values
```

### Comparing `notionlib-0.1.dev0/notionlib.egg-info/PKG-INFO` & `notionlib-0.2.dev0/notionlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: notionlib
-Version: 0.1.dev0
-Summary: An unofficial Python 3 client for Notion.so API
+Version: 0.2.dev0
+Summary: An unofficial Python 3 client for the Notion.so API
 Home-page: https://github.com/jdhp/notion-lib
+Download-URL: 
 Author: Jérémie DECOCK
 Author-email: jd.jdhp@gmail.com
+Maintainer: Jérémie DECOCK
+Maintainer-email: jd.jdhp@gmail.com
 Project-URL: Bug Tracker, https://github.com/jdhp/notion-lib/issues
-Keywords: notionlib
+Keywords: Gitlab
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.6
```

### Comparing `notionlib-0.1.dev0/setup.cfg` & `notionlib-0.2.dev0/setup.cfg`

 * *Files identical despite different names*

