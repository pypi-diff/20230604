# Comparing `tmp/authomize-rest-api-client-4.1.5.tar.gz` & `tmp/authomize-rest-api-client-4.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.1.5.tar", last modified: Wed May 31 13:11:24 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.1.6.tar", last modified: Sun Jun  4 13:30:06 2023, max compression
```

## Comparing `authomize-rest-api-client-4.1.5.tar` & `authomize-rest-api-client-4.1.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2194 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.742829 authomize-rest-api-client-4.1.5/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84288 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37380 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   200259 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89370 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-31 13:11:24.000000 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-31 13:11:24.000000 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 13:11:24.000000 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 13:11:24.000000 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-31 13:11:24.000000 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 13:11:08.000000 authomize-rest-api-client-4.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.089781 authomize-rest-api-client-4.1.6/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84288 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37380 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   200259 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89370 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-04 13:29:43.000000 authomize-rest-api-client-4.1.6/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-04 13:30:06.000000 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-06-04 13:30:06.000000 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 13:30:06.000000 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-04 13:30:06.000000 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-04 13:30:06.000000 authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-04 13:30:06.093781 authomize-rest-api-client-4.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-06-04 13:29:47.000000 authomize-rest-api-client-4.1.6/setup.py
```

### Comparing `authomize-rest-api-client-4.1.5/LICENSE.txt` & `authomize-rest-api-client-4.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/README.md` & `authomize-rest-api-client-4.1.6/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.1.6/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/base_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,31 +51,31 @@
                 'raw': response.content,
             }
         )
 
     def http_get(self, url, params=None):
         url = self.base_url + url
         response = self.session.get(url, params=params)
-        self._handle_response(response)
+        return self._handle_response(response)
 
     def http_post(self, url: str, body: Optional[str] = None):
         url = self.base_url + url
         response = self.session.post(
             url,
             headers={'Content-Type': 'application/json'},
             data=body,
         )
-        self._handle_response(response)
+        return self._handle_response(response)
 
     def http_patch(self, url: str, body: Optional[str] = None):
         url = self.base_url + url
         response = self.session.patch(
             url,
             headers={'Content-Type': 'application/json'},
             data=body,
         )
-        self._handle_response(response)
+        return self._handle_response(response)
 
     def http_delete(self, url: str, params=None):
         url = self.base_url + url
         response = self.session.delete(url, params=params)
-        self._handle_response(response)
+        return self._handle_response(response)
```

### Comparing `authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.1.6/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.1.6/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.1.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.1.6/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.5/setup.py` & `authomize-rest-api-client-4.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.1.5',
+        version='4.1.6',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

