# Comparing `tmp/gerbil-api-wrapper-1.0.2.tar.gz` & `tmp/gerbil-api-wrapper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerbil-api-wrapper-1.0.2.tar", last modified: Tue Mar 21 07:26:26 2023, max compression
+gzip compressed data, was "gerbil-api-wrapper-1.0.3.tar", last modified: Sun Jun  4 16:34:02 2023, max compression
```

## Comparing `gerbil-api-wrapper-1.0.2.tar` & `gerbil-api-wrapper-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 07:26:26.496718 gerbil-api-wrapper-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-03-21 07:26:06.000000 gerbil-api-wrapper-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-21 07:26:26.496718 gerbil-api-wrapper-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-21 07:26:06.000000 gerbil-api-wrapper-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 07:26:26.492718 gerbil-api-wrapper-1.0.2/gerbil_api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 07:26:06.000000 gerbil-api-wrapper-1.0.2/gerbil_api_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-03-21 07:26:06.000000 gerbil-api-wrapper-1.0.2/gerbil_api_wrapper/gerbil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 07:26:26.492718 gerbil-api-wrapper-1.0.2/gerbil_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-21 07:26:26.000000 gerbil-api-wrapper-1.0.2/gerbil_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-21 07:26:26.000000 gerbil-api-wrapper-1.0.2/gerbil_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 07:26:26.000000 gerbil-api-wrapper-1.0.2/gerbil_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-21 07:26:26.000000 gerbil-api-wrapper-1.0.2/gerbil_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-21 07:26:26.000000 gerbil-api-wrapper-1.0.2/gerbil_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 07:26:26.496718 gerbil-api-wrapper-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-21 07:26:06.000000 gerbil-api-wrapper-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 07:26:26.496718 gerbil-api-wrapper-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 07:26:06.000000 gerbil-api-wrapper-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-21 07:26:06.000000 gerbil-api-wrapper-1.0.2/tests/test_gerbil_api_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:34:02.107424 gerbil-api-wrapper-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-06-04 16:33:33.000000 gerbil-api-wrapper-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-04 16:34:02.107424 gerbil-api-wrapper-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-04 16:33:33.000000 gerbil-api-wrapper-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:34:02.103423 gerbil-api-wrapper-1.0.3/gerbil_api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:33:33.000000 gerbil-api-wrapper-1.0.3/gerbil_api_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-06-04 16:33:33.000000 gerbil-api-wrapper-1.0.3/gerbil_api_wrapper/gerbil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:34:02.103423 gerbil-api-wrapper-1.0.3/gerbil_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-04 16:34:02.000000 gerbil-api-wrapper-1.0.3/gerbil_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-04 16:34:02.000000 gerbil-api-wrapper-1.0.3/gerbil_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:34:02.000000 gerbil-api-wrapper-1.0.3/gerbil_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-04 16:34:02.000000 gerbil-api-wrapper-1.0.3/gerbil_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-04 16:34:02.000000 gerbil-api-wrapper-1.0.3/gerbil_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 16:34:02.107424 gerbil-api-wrapper-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-04 16:33:33.000000 gerbil-api-wrapper-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:34:02.107424 gerbil-api-wrapper-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:33:33.000000 gerbil-api-wrapper-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-04 16:33:33.000000 gerbil-api-wrapper-1.0.3/tests/test_gerbil_api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-04 16:33:33.000000 gerbil-api-wrapper-1.0.3/tests/test_gerbil_api_wrapper_live.py
```

### Comparing `gerbil-api-wrapper-1.0.2/LICENSE` & `gerbil-api-wrapper-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gerbil-api-wrapper-1.0.2/PKG-INFO` & `gerbil-api-wrapper-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerbil-api-wrapper
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that provides wrapper functionality for the Gerbil Benchmark Service
 Home-page: https://github.com/heinpa/GerbilExperimentApiWrapper
 Author: Paul Heinze
 Author-email: paul.heinze@student.hs-anhalt.de
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,17 +31,20 @@
 
 Running an expeiment with a local test results file: 
 
 ```python
 from gerbil_api_wrapper.gerbil import Gerbil
 
 wrapper = Gerbil(
-    gold_standard_file="results_gold.json",
-    test_results_file="result_test.json",
-    language="en")
+    gold_standard_file="original_data/qald_9_plus_test_dbpedia.json",
+    test_results_file="original_data/qald_9_plus_test_dbpedia-test.json",
+    test_results_name="MyTestResults",
+    gold_standard_name="MyGoldStandard",
+    language="de"
+)
 ```
 
 Running an experiment with a live annotator: 
 
 ```python
 from gerbil_api_wrapper.gerbil import Gerbil
```

### Comparing `gerbil-api-wrapper-1.0.2/README.md` & `gerbil-api-wrapper-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -20,17 +20,20 @@
 
 Running an expeiment with a local test results file: 
 
 ```python
 from gerbil_api_wrapper.gerbil import Gerbil
 
 wrapper = Gerbil(
-    gold_standard_file="results_gold.json",
-    test_results_file="result_test.json",
-    language="en")
+    gold_standard_file="original_data/qald_9_plus_test_dbpedia.json",
+    test_results_file="original_data/qald_9_plus_test_dbpedia-test.json",
+    test_results_name="MyTestResults",
+    gold_standard_name="MyGoldStandard",
+    language="de"
+)
 ```
 
 Running an experiment with a live annotator: 
 
 ```python
 from gerbil_api_wrapper.gerbil import Gerbil
```

### Comparing `gerbil-api-wrapper-1.0.2/gerbil_api_wrapper/gerbil.py` & `gerbil-api-wrapper-1.0.3/gerbil_api_wrapper/gerbil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import requests
 import time
 from bs4 import BeautifulSoup
 import validators
 from pathlib import Path
 import logging
+from urllib.parse import urlparse
 
 
 logging.basicConfig(format="%(asctime)s - %(message)s", level=logging.INFO)
 
 
 class Gerbil:
 
@@ -20,18 +21,19 @@
 
     gold_standard_name = "GoldStandard"
     test_results_name = "TestResults"
 
     live_annotator_prefix = "NIFWS"
     uploaded_dataset_prefix = "NIFDS"
     dataset_reference_prefix = "AFDS"
-    anser_files_prefix = "AF"
+    answer_files_prefix = "AF"
 
-    upload_data_postfix = """experimentData={{"type":"QA","matching":"STRONG_ENTITY_MATCH","annotator":[{annotator}],"dataset":["{dataset}"],"answerFiles":[{answerFiles}],"questionLanguage":"{questionLanguage}"}}"""
+    upload_data_template = """experimentData={{"type":"QA","matching":"STRONG_ENTITY_MATCH","annotator":[{annotator}],"dataset":["{dataset}"],"answerFiles":[{answerFiles}],"questionLanguage":"{questionLanguage}"}}"""
 
+    check_for_another_experiments = False
 
     def __init__(self, language, gold_standard_file, **kwargs):
         """
         Parameters
         ---------
         gold_standard_file : str, required
             The path to a gold standard dataset
@@ -56,82 +58,83 @@
         self.test_results_file = kwargs.get('test_results_file')
         self.live_annotator_name = kwargs.get('live_annotator_name')
         self.live_annotator_url = kwargs.get('live_annotator_url')
 
         self.gold_standard_name = kwargs.get('gold_standard_name', self.gold_standard_name)
         self.test_results_name = kwargs.get('test_results_name', self.test_results_name)
 
+        self.check_for_another_experiments = kwargs.get('check_for_another_experiments', self.check_for_another_experiments)
+
         # upload files / set live annotator (prefer local files)
         self.upload_file(self.gold_standard_file, self.gold_standard_name, 'application/json')
-        
+
         # setup with local files
         if self.test_results_file:
             self.use_live_annotator = False
-            self.upload_file(self.test_results_file, self.test_results_name, 'application/json', self.gold_standard_file)
+            self.upload_file(self.test_results_file, self.test_results_name, 'application/json')
 
         # setup with live annotator
-        elif self.live_annotator_url:
+        if self.live_annotator_url:
             self.use_live_annotator = True
             self.set_live_annotator(self.live_annotator_name, self.live_annotator_url)
-        else:
+        elif not self.test_results_file and not self.live_annotator_url:
             raise Exception(f"Could not initialize GerbilBenchmarkService!"
                             + "Missing results file or live annotator.")
 
         # run experiment with set configuration
         self.experiment_id = self.upload_experiment_configuration()
         if self.is_url_valid(self.get_results_url()):
             logging.info(f"initialized GerbilExperimentApiWrapper with experiment: {self.get_experiment_url}{self.experiment_id}")
         else:
             raise Exception(f"Could not initialize GerbilBenchmarkService!"
                             + "The experiment did not return valid results.")
-        
+
 
     def is_url_valid(self, results_url):
         # basic validation of the result url
         if validators.url(results_url):
             return True
         else:
             return False
 
 
     def set_live_annotator(self, name, url):
         if self.is_url_valid(url):
-            self.annoator = f"{self.live_annotator_prefix}_{name}({url})"
-        else: 
+            self.annotator = f"{self.live_annotator_prefix}_{name}({url})"
+        else:
             raise Exception(f"Invalid annotator URL for annotator {name}: {url}")
 
-        
-    def upload_experiment_configuration(self):
 
-        execute_url = self.upload_configuration_url + self.upload_data_postfix.format(
-            dataset = f"{self.uploaded_dataset_prefix}_{self.gold_standard_name}({self.gold_standard_file})",
-            answerFiles = f"\"{self.anser_files_prefix}_{self.test_results_name}({self.test_results_file})(undefined)({self.dataset_reference_prefix}_{self.gold_standard_file})\"" 
-                if not self.use_live_annotator else "", 
-            annotator = f"\"{self.annoator}\"" if self.use_live_annotator else "",
+    def upload_experiment_configuration(self):
+        execute_url = self.upload_configuration_url + self.upload_data_template.format(
+            dataset = f"{self.uploaded_dataset_prefix}_{self.gold_standard_name}({self.gold_standard_name})",
+            answerFiles = f"\"{self.answer_files_prefix}_{self.test_results_name}({self.test_results_name})(undefined)({self.dataset_reference_prefix}_{self.gold_standard_name})\""
+                if not self.use_live_annotator else "",
+            annotator = f"\"{self.annotator}\"" if self.use_live_annotator else "",
             questionLanguage = self.language
         )
 
         logging.info(f"\nUpload experiment configuration: {execute_url}")
 
         cnt = 0
         while cnt < 5:
             try:
                 # check that no other experiment is running
-                if requests.get(self.check_running_url).text == '':
+                if not self.check_for_another_experiments or requests.get(self.check_running_url).text == '':
                     # execute reauest with experiment configuration
                     response = requests.get(execute_url)
                     if response.status_code == 200:
                         return response.text # return the experiment id 
                 else:
                     logging.info("another experiment is running, waiting for 60 seconds ...")
-                    cnt += 1 
+                    cnt += 1
                     time.sleep(60)
             except:
                 logging.info("request failed, retrying ...")
-                cnt += 1 
+                cnt += 1
         raise Exception(f"could not complete request after {cnt} attempts")
 
 
     def get_results_url(self):
         return self.get_experiment_url + self.experiment_id
 
 
@@ -139,47 +142,49 @@
         query_url = self.get_results_url()
         # extract json-ld from response content
         soup = BeautifulSoup(requests.get(query_url).text, "html.parser")
         data = [
             json.loads(x.string) for x in soup.find_all("script", type="application/ld+json")
         ]
         return data[0]
-        
 
-    def upload_file(self, file, name, type, multiselect=None):
+
+    def upload_file(self, file, name, type):
         """Upload gold starndard or test results file to be used in the experiment
 
         Parameters
         ----------
         file : str, required
-            The file path 
+            The file path
         name : str, required
             The name to be used in the experiment configuration
         type : str, required
             The application type for the file
         multiselect : bool, optional
             The path to the referenced gold standard file when uploading test results
         """
 
-        if len(file) > 100:
+        if len(name) > 100:
             raise Exception("File names must not exceed 100 characters!")
         # TODO: figure out how upload handles file paths
         # currently the server responds with 500, seeminly because it's out of space
         files = {
-            "file": (file, open(file, 'rb'), type)
+            "file": (name, open(file, 'rb'), type)
         }
         data = {
-            'name': name,
-            'multiselect': multiselect 
+            'name': name
+            # 'multiselect': multiselect
         }
         try:
             logging.info(f"\nRequest to: {self.file_upload_url}\n" + \
                          f"Data: {data}\n" + \
                          f"Files: {files}")
             request = requests.post(self.file_upload_url, data=data, files=files)
             response = request.json()
+            # store the response, mainly for test purposes
+            # TODO: change? 
             logging.info(f"Got response: {response} ({request.status_code})")
             if request.status_code != 200:
                 raise Exception(f"file upload not successful: {request.status_code}: {request.content}")
             else: return response
         except Exception as e:
             raise Exception(f"file upload not successful: {e}")
```

### Comparing `gerbil-api-wrapper-1.0.2/gerbil_api_wrapper.egg-info/PKG-INFO` & `gerbil-api-wrapper-1.0.3/gerbil_api_wrapper.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gerbil-api-wrapper
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that provides wrapper functionality for the Gerbil Benchmark Service
 Home-page: https://github.com/heinpa/GerbilExperimentApiWrapper
 Author: Paul Heinze
 Author-email: paul.heinze@student.hs-anhalt.de
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,17 +31,20 @@
 
 Running an expeiment with a local test results file: 
 
 ```python
 from gerbil_api_wrapper.gerbil import Gerbil
 
 wrapper = Gerbil(
-    gold_standard_file="results_gold.json",
-    test_results_file="result_test.json",
-    language="en")
+    gold_standard_file="original_data/qald_9_plus_test_dbpedia.json",
+    test_results_file="original_data/qald_9_plus_test_dbpedia-test.json",
+    test_results_name="MyTestResults",
+    gold_standard_name="MyGoldStandard",
+    language="de"
+)
 ```
 
 Running an experiment with a live annotator: 
 
 ```python
 from gerbil_api_wrapper.gerbil import Gerbil
```

### Comparing `gerbil-api-wrapper-1.0.2/setup.py` & `gerbil-api-wrapper-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     for req in reqs:
         names.append(req)
     return {'install_requires': names}
 
 
 setuptools.setup(
     name="gerbil-api-wrapper",
-    version="1.0.2",
+    version="1.0.3",
     author="Paul Heinze",
     author_email="paul.heinze@student.hs-anhalt.de",
     description="A package that provides wrapper functionality for the Gerbil Benchmark Service",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/heinpa/GerbilExperimentApiWrapper",
     packages=setuptools.find_packages(),
```

### Comparing `gerbil-api-wrapper-1.0.2/tests/test_gerbil_api_wrapper.py` & `gerbil-api-wrapper-1.0.3/tests/test_gerbil_api_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,21 @@
                     gold_standard_file=self.gold_standard_file, language=self.language,
                     test_results_file=self.test_results_file
                 )
                 assert wrapper.use_live_annotator == False
 
                 assert mocked_upload_file.call_count == 2
                 assert mocked_upload_file.call_args_list[0].args == (
-                    self.gold_standard_file, 
+                    self.gold_standard_file,
                     'GoldStandard',
                     'application/json')
                 assert mocked_upload_file.call_args_list[1].args == (
                     self.test_results_file,
                     'TestResults',
-                    'application/json',
-                    self.gold_standard_file)
+                    'application/json')
 
                 # assert values are stored in wrapper object
                 assert wrapper.gold_standard_file == self.gold_standard_file
                 assert wrapper.test_results_file == self.test_results_file
                 assert wrapper.language == self.language
 
                 # assert the configuration upload function was called
@@ -61,15 +60,15 @@
                     live_annotator_name=self.live_annotator_name,
                     live_annotator_url=self.live_annotator_url
                 )
                 assert wrapper.use_live_annotator == True
 
                 assert mocked_upload_file.call_count == 1
                 assert mocked_upload_file.call_args_list[0].args == (
-                    self.gold_standard_file, 
+                    self.gold_standard_file,
                     'GoldStandard',
                     'application/json')
 
                 # assert values are stored in wrapper object
                 assert wrapper.gold_standard_file == self.gold_standard_file
                 assert wrapper.live_annotator_name == self.live_annotator_name
                 assert wrapper.live_annotator_url == self.live_annotator_url
```

