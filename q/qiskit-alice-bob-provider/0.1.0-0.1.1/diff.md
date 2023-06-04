# Comparing `tmp/qiskit_alice_bob_provider-0.1.0.tar.gz` & `tmp/qiskit_alice_bob_provider-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_alice_bob_provider-0.1.0.tar", last modified: Thu May 25 17:40:50 2023, max compression
+gzip compressed data, was "qiskit_alice_bob_provider-0.1.1.tar", last modified: Sun Jun  4 19:27:39 2023, max compression
```

## Comparing `qiskit_alice_bob_provider-0.1.0.tar` & `qiskit_alice_bob_provider-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-05-25 17:40:50.895440 qiskit_alice_bob_provider-0.1.0/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)    11342 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.0/LICENSE
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-05-25 17:40:50.895440 qiskit_alice_bob_provider-0.1.0/PKG-INFO
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1122 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/README.md
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2092 2023-05-25 17:40:45.000000 qiskit_alice_bob_provider-0.1.0/pyproject.toml
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-05-25 17:40:50.895440 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      822 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/__init__.py
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-05-25 17:40:50.895440 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/api/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      760 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/api/__init__.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     3136 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/api/client.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     4469 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/api/jobs.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1286 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/api/targets.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5005 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/backend.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1857 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/custom_instructions.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1039 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/errors.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     7882 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/job.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2324 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/provider.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5871 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/qir_to_qiskit.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5112 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/translation_plugin.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1086 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/utils.py
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-05-25 17:40:50.895440 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider.egg-info/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-05-25 17:40:50.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider.egg-info/PKG-INFO
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1033 2023-05-25 17:40:50.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider.egg-info/SOURCES.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)        1 2023-05-25 17:40:50.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider.egg-info/dependency_links.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      120 2023-05-25 17:40:50.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider.egg-info/entry_points.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      308 2023-05-25 17:40:50.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider.egg-info/requires.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       26 2023-05-25 17:40:50.000000 qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider.egg-info/top_level.txt
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       38 2023-05-25 17:40:50.895440 qiskit_alice_bob_provider-0.1.0/setup.cfg
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       69 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.0/setup.py
-drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-05-25 17:40:50.895440 qiskit_alice_bob_provider-0.1.0/tests/
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1372 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.0/tests/test_against_real_server.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     3963 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/tests/test_api.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5049 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/tests/test_backend.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      295 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/tests/test_provider.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1126 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/tests/test_qir_to_qiskit.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5606 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.0/tests/test_translation_plugin.py
--rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      444 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)    11342 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/LICENSE
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/PKG-INFO
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1122 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/README.md
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2108 2023-06-04 19:26:25.000000 qiskit_alice_bob_provider-0.1.1/pyproject.toml
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      822 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/__init__.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      760 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/__init__.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     3681 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/client.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     4469 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/jobs.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1286 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/targets.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5005 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/backend.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1857 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/custom_instructions.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1039 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/errors.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     7882 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/job.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2563 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/provider.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5871 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/qir_to_qiskit.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5112 2023-05-29 08:28:45.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/translation_plugin.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1086 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/utils.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     2245 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/PKG-INFO
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1033 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)        1 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      120 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/entry_points.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      317 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/requires.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       26 2023-06-04 19:27:39.000000 qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/top_level.txt
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       38 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/setup.cfg
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)       69 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/setup.py
+drwxr-xr-x   0 jdumazer  (1000) jdumazer  (1000)        0 2023-06-04 19:27:39.817076 qiskit_alice_bob_provider-0.1.1/tests/
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1372 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/tests/test_against_real_server.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5145 2023-06-04 19:24:55.000000 qiskit_alice_bob_provider-0.1.1/tests/test_api.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5049 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/tests/test_backend.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      295 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/tests/test_provider.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     1126 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/tests/test_qir_to_qiskit.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)     5606 2023-05-19 13:42:42.000000 qiskit_alice_bob_provider-0.1.1/tests/test_translation_plugin.py
+-rw-r--r--   0 jdumazer  (1000) jdumazer  (1000)      444 2023-05-25 14:34:56.000000 qiskit_alice_bob_provider-0.1.1/tests/test_utils.py
```

### Comparing `qiskit_alice_bob_provider-0.1.0/LICENSE` & `qiskit_alice_bob_provider-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/PKG-INFO` & `qiskit_alice_bob_provider-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_alice_bob_provider
-Version: 0.1.0
+Version: 0.1.1
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
```

### Comparing `qiskit_alice_bob_provider-0.1.0/README.md` & `qiskit_alice_bob_provider-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/pyproject.toml` & `qiskit_alice_bob_provider-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qiskit_alice_bob_provider"
 authors = [
     {name = "Alice & Bob Software Team"},
 ]
-version = "0.1.0"
+version = "0.1.1"
 description = "Provider for running Qiskit circuits on Alice & Bob QPUs and simulators"
 readme = "README.md"
 license = {text = "Apache 2.0"}
 keywords = ["Qiskit", "Alice & Bob", "Quantum", "SDK"]
 classifiers=[
     "Environment :: Console",
     "License :: OSI Approved :: Apache Software License",
@@ -28,15 +28,16 @@
     "Topic :: Scientific/Engineering :: Physics",
 ]
 urls = {Homepage = "https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider", "Alice & Bob" = "https://alice-bob.com/"}
 requires-python = ">=3.7"
 dependencies = [
     "requests",
     "qiskit-terra",
-    "qiskit-qir-alice-bob-fork"
+    "qiskit-qir-alice-bob-fork",
+    "tenacity"
 ]
 
 [project.optional-dependencies]
 dev = [
     "black==23.1.0",
     "codespell==2.2.2",
     "coverage==7.2.2",
```

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/__init__.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/api/__init__.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/api/client.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 
 import urllib.parse
 
 import requests
+from tenacity import (
+    retry,
+    retry_if_exception_type,
+    stop_after_attempt,
+    wait_fixed,
+)
 
 
 class AliceBobApiException(Exception):
     """Exception raised by the Aice & Bob API client"""
 
     def __init__(self, response: requests.Response) -> None:
         super().__init__(response.content.decode())
@@ -29,29 +35,42 @@
 
 class ApiClient:
     """Alice & Bob API client
 
     This wrapper adds authentication and the base URL to all requests.
     """
 
-    def __init__(self, api_key: str, url: str):
+    def __init__(
+        self,
+        api_key: str,
+        url: str,
+        retries: int = 5,
+        wait_between_retries_seconds: int = 1,
+    ):
         """
         Args:
             api_key (str): an API key provided by Alice & Bob
             url (str): the base URL of the API
         """
         self._url = url
         self._session = requests.Session()
         self._session.headers.update({'Authorization': f'Basic {api_key}'})
+        self._retries = retries
+        self._wait_between_retries_seconds = wait_between_retries_seconds
 
     def _request(
         self, method: str, endpoint: str, **kwargs
     ) -> requests.Response:
         url = urllib.parse.urljoin(self._url, endpoint)
-        resp = self._session.request(method=method, url=url, **kwargs)
+        resp = retry(
+            reraise=True,
+            wait=wait_fixed(self._wait_between_retries_seconds),
+            retry=retry_if_exception_type(requests.ConnectionError),
+            stop=stop_after_attempt(self._retries),
+        )(self._session.request)(method=method, url=url, **kwargs)
         try:
             resp.raise_for_status()
         except requests.HTTPError as e:
             raise AliceBobApiException(resp) from e
         return resp
 
     def get(self, endpoint: str, **kwargs) -> requests.Response:
```

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/api/jobs.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/jobs.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/api/targets.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/api/targets.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/backend.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/custom_instructions.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/custom_instructions.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/errors.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/job.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/job.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/provider.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,22 +23,33 @@
 from .api.targets import list_targets
 from .backend import AliceBobBackend
 
 
 class AliceBobProvider(ProviderV1):
     """Class listing and providing access to all Alice & Bob backends."""
 
-    def __init__(self, api_key: str, url: str = 'https://api.alice-bob.com/'):
+    def __init__(
+        self,
+        api_key: str,
+        url: str = 'https://api.alice-bob.com/',
+        retries: int = 5,
+        wait_between_retries_seconds: int = 1,
+    ):
         """
         Args:
             api_key (str): an API key for the Alice & Bob API
             url (str): Base URL of the Alice & Bob API.
                 Defaults to 'https://api.alice-bob.com/'.
         """
-        client = ApiClient(api_key=api_key, url=url)
+        client = ApiClient(
+            api_key=api_key,
+            url=url,
+            retries=retries,
+            wait_between_retries_seconds=wait_between_retries_seconds,
+        )
         self._backends = []
         for ab_target in list_targets(client):
             self._backends.append(AliceBobBackend(client, ab_target))
 
     def backends(
         self, name: Optional[str] = None, **kwargs
     ) -> List[BackendV2]:
```

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/qir_to_qiskit.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/qir_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/translation_plugin.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/translation_plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider/utils.py` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider.egg-info/PKG-INFO` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-alice-bob-provider
-Version: 0.1.0
+Version: 0.1.1
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
```

### Comparing `qiskit_alice_bob_provider-0.1.0/qiskit_alice_bob_provider.egg-info/SOURCES.txt` & `qiskit_alice_bob_provider-0.1.1/qiskit_alice_bob_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/tests/test_against_real_server.py` & `qiskit_alice_bob_provider-0.1.1/tests/test_against_real_server.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/tests/test_api.py` & `qiskit_alice_bob_provider-0.1.1/tests/test_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 
+import pytest
+import requests
 from requests_mock import ANY
 from requests_mock.mocker import Mocker
 
 from qiskit_alice_bob_provider.api import jobs, targets
 from qiskit_alice_bob_provider.api.client import ApiClient
 
 
@@ -102,7 +104,44 @@
     assert payload['inputParams'] == input_params
 
 
 def test_list_targets(requests_mock: Mocker) -> None:
     requests_mock.register_uri('GET', '/v1/targets/', json=[{}, {}])
     client = ApiClient(api_key='foo', url='https://api.alice-bob.com/')
     targets.list_targets(client)
+
+
+def test_connection_aborted(requests_mock: Mocker) -> None:
+    requests_mock.register_uri(
+        'GET', '/v1/targets/', exc=requests.ConnectionError
+    )
+    client = ApiClient(
+        api_key='foo',
+        url='https://api.alice-bob.com/',
+        wait_between_retries_seconds=0,
+    )
+    with pytest.raises(requests.ConnectionError):
+        targets.list_targets(client)
+    assert requests_mock.call_count == 5
+
+    requests_mock.register_uri('GET', '/v1/targets/', exc=requests.HTTPError)
+    client = ApiClient(
+        api_key='foo',
+        url='https://api.alice-bob.com/',
+        wait_between_retries_seconds=0,
+    )
+    with pytest.raises(requests.HTTPError):
+        targets.list_targets(client)
+    assert requests_mock.call_count == 5 + 1
+
+    requests_mock.register_uri(
+        'GET', '/v1/targets/', exc=requests.ConnectionError
+    )
+    client = ApiClient(
+        api_key='foo',
+        url='https://api.alice-bob.com/',
+        retries=4,
+        wait_between_retries_seconds=0,
+    )
+    with pytest.raises(requests.ConnectionError):
+        targets.list_targets(client)
+    assert requests_mock.call_count == 5 + 1 + 4
```

### Comparing `qiskit_alice_bob_provider-0.1.0/tests/test_backend.py` & `qiskit_alice_bob_provider-0.1.1/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/tests/test_qir_to_qiskit.py` & `qiskit_alice_bob_provider-0.1.1/tests/test_qir_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.1.0/tests/test_translation_plugin.py` & `qiskit_alice_bob_provider-0.1.1/tests/test_translation_plugin.py`

 * *Files identical despite different names*

