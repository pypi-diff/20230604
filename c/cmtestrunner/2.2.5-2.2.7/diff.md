# Comparing `tmp/cmtestrunner-2.2.5.tar.gz` & `tmp/cmtestrunner-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmtestrunner-2.2.5.tar", last modified: Wed Feb 15 05:37:01 2023, max compression
+gzip compressed data, was "cmtestrunner-2.2.7.tar", last modified: Wed Feb 22 10:15:40 2023, max compression
```

## Comparing `cmtestrunner-2.2.5.tar` & `cmtestrunner-2.2.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-15 05:37:01.671802 cmtestrunner-2.2.5/
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)       96 2022-10-06 09:29:30.000000 cmtestrunner-2.2.5/MANIFEST.in
--rw-rw-r--   0 tasin     (1000) tasin     (1000)      250 2023-02-15 05:37:01.667802 cmtestrunner-2.2.5/PKG-INFO
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)      658 2022-10-06 09:29:30.000000 cmtestrunner-2.2.5/README.md
-drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-15 05:37:01.483802 cmtestrunner-2.2.5/cmtestrunner/
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)      512 2023-01-16 12:25:01.000000 cmtestrunner-2.2.5/cmtestrunner/__init__.py
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)     2885 2023-02-05 08:30:30.000000 cmtestrunner-2.2.5/cmtestrunner/json_traverser.py
-drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-15 05:37:01.499802 cmtestrunner-2.2.5/cmtestrunner/management/
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/__init__.py
-drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-15 05:37:01.543802 cmtestrunner-2.2.5/cmtestrunner/management/commands/
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/commands/__init__.py
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)     4450 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/commands/createtest.py
--rw-rw-r--   0 tasin     (1000) tasin     (1000)     1063 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/commands/createtestpool.py
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)     5120 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/commands/createunittest.py
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)     2018 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/commands/iwanttotest.py
-drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-15 05:37:01.603802 cmtestrunner-2.2.5/cmtestrunner/management/templates/
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)       29 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/templates/endpoints_template.txt
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)      362 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/templates/test_methods_template.txt
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)      189 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/templates/test_runner_template.txt
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)      512 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/templates/tests_template.txt
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)       80 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/templates/unit_test_import_template.txt
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)      515 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/management/templates/unit_test_method_template.txt
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)    18653 2023-02-14 07:33:51.000000 cmtestrunner-2.2.5/cmtestrunner/middleware.py
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)    12318 2023-02-05 08:30:21.000000 cmtestrunner-2.2.5/cmtestrunner/object_manager.py
--rw-rw-r--   0 tasin     (1000) tasin     (1000)        0 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/processor.py
-drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-15 05:37:01.667802 cmtestrunner-2.2.5/cmtestrunner/templates/
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)     1674 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/templates/exceptions.html
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)     2539 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/templates/modal.html
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)     5072 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/templates/report.html
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)     1588 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/templates/test_details.html
--rw-rw-r--   0 tasin     (1000) tasin     (1000)     1262 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/templates/test_pool.html
--rw-rw-r--   0 tasin     (1000) tasin     (1000)     1603 2022-10-06 09:37:36.000000 cmtestrunner-2.2.5/cmtestrunner/test.py
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)    16217 2023-02-15 05:36:32.000000 cmtestrunner-2.2.5/cmtestrunner/test_runner.py
--rw-rw-r--   0 tasin     (1000) tasin     (1000)        0 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner/verify_enigne.py
-drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-15 05:37:01.499802 cmtestrunner-2.2.5/cmtestrunner.egg-info/
--rwxrwxrwx   0 tasin     (1000) tasin     (1000)      250 2023-02-15 05:37:01.000000 cmtestrunner-2.2.5/cmtestrunner.egg-info/PKG-INFO
--rwxrwxrwx   0 tasin     (1000) tasin     (1000)     1285 2023-02-15 05:37:01.000000 cmtestrunner-2.2.5/cmtestrunner.egg-info/SOURCES.txt
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)        1 2023-02-15 05:37:01.000000 cmtestrunner-2.2.5/cmtestrunner.egg-info/dependency_links.txt
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)        1 2022-10-06 09:29:31.000000 cmtestrunner-2.2.5/cmtestrunner.egg-info/not-zip-safe
--rwxrwxrwx   0 tasin     (1000) tasin     (1000)       85 2023-02-15 05:37:01.000000 cmtestrunner-2.2.5/cmtestrunner.egg-info/requires.txt
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)       13 2023-02-15 05:37:01.000000 cmtestrunner-2.2.5/cmtestrunner.egg-info/top_level.txt
--rw-rw-r--   0 tasin     (1000) tasin     (1000)       38 2023-02-15 05:37:01.671802 cmtestrunner-2.2.5/setup.cfg
--rwxrwxr-x   0 tasin     (1000) tasin     (1000)      567 2023-02-15 05:36:54.000000 cmtestrunner-2.2.5/setup.py
+drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-22 10:15:39.999967 cmtestrunner-2.2.7/
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)       96 2022-10-06 09:29:30.000000 cmtestrunner-2.2.7/MANIFEST.in
+-rw-rw-r--   0 tasin     (1000) tasin     (1000)      250 2023-02-22 10:15:39.999967 cmtestrunner-2.2.7/PKG-INFO
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)      658 2022-10-06 09:29:30.000000 cmtestrunner-2.2.7/README.md
+drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-22 10:15:39.963967 cmtestrunner-2.2.7/cmtestrunner/
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)      512 2023-01-16 12:25:01.000000 cmtestrunner-2.2.7/cmtestrunner/__init__.py
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)     2885 2023-02-05 08:30:30.000000 cmtestrunner-2.2.7/cmtestrunner/json_traverser.py
+drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-22 10:15:39.971968 cmtestrunner-2.2.7/cmtestrunner/management/
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/__init__.py
+drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-22 10:15:39.987967 cmtestrunner-2.2.7/cmtestrunner/management/commands/
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/commands/__init__.py
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)     4450 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/commands/createtest.py
+-rw-rw-r--   0 tasin     (1000) tasin     (1000)     1063 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/commands/createtestpool.py
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)     5120 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/commands/createunittest.py
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)     2018 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/commands/iwanttotest.py
+drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-22 10:15:39.991967 cmtestrunner-2.2.7/cmtestrunner/management/templates/
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)       29 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/templates/endpoints_template.txt
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)      362 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/templates/test_methods_template.txt
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)      189 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/templates/test_runner_template.txt
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)      512 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/templates/tests_template.txt
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)       80 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/templates/unit_test_import_template.txt
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)      515 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/management/templates/unit_test_method_template.txt
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)    18653 2023-02-14 07:33:51.000000 cmtestrunner-2.2.7/cmtestrunner/middleware.py
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)    12318 2023-02-05 08:30:21.000000 cmtestrunner-2.2.7/cmtestrunner/object_manager.py
+-rw-rw-r--   0 tasin     (1000) tasin     (1000)        0 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/processor.py
+drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-22 10:15:39.995967 cmtestrunner-2.2.7/cmtestrunner/templates/
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)     1674 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/templates/exceptions.html
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)     2539 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/templates/modal.html
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)     5072 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/templates/report.html
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)     1588 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/templates/test_details.html
+-rw-rw-r--   0 tasin     (1000) tasin     (1000)     1262 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/templates/test_pool.html
+-rw-rw-r--   0 tasin     (1000) tasin     (1000)     1603 2022-10-06 09:37:36.000000 cmtestrunner-2.2.7/cmtestrunner/test.py
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)    16651 2023-02-22 10:12:23.000000 cmtestrunner-2.2.7/cmtestrunner/test_runner.py
+-rw-rw-r--   0 tasin     (1000) tasin     (1000)        0 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner/verify_enigne.py
+drwxrwxr-x   0 tasin     (1000) tasin     (1000)        0 2023-02-22 10:15:39.971968 cmtestrunner-2.2.7/cmtestrunner.egg-info/
+-rwxrwxrwx   0 tasin     (1000) tasin     (1000)      250 2023-02-22 10:15:39.000000 cmtestrunner-2.2.7/cmtestrunner.egg-info/PKG-INFO
+-rwxrwxrwx   0 tasin     (1000) tasin     (1000)     1285 2023-02-22 10:15:39.000000 cmtestrunner-2.2.7/cmtestrunner.egg-info/SOURCES.txt
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)        1 2023-02-22 10:15:39.000000 cmtestrunner-2.2.7/cmtestrunner.egg-info/dependency_links.txt
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)        1 2022-10-06 09:29:31.000000 cmtestrunner-2.2.7/cmtestrunner.egg-info/not-zip-safe
+-rwxrwxrwx   0 tasin     (1000) tasin     (1000)       82 2023-02-22 10:15:39.000000 cmtestrunner-2.2.7/cmtestrunner.egg-info/requires.txt
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)       13 2023-02-22 10:15:39.000000 cmtestrunner-2.2.7/cmtestrunner.egg-info/top_level.txt
+-rw-rw-r--   0 tasin     (1000) tasin     (1000)       38 2023-02-22 10:15:39.999967 cmtestrunner-2.2.7/setup.cfg
+-rwxrwxr-x   0 tasin     (1000) tasin     (1000)      564 2023-02-22 10:15:38.000000 cmtestrunner-2.2.7/setup.py
```

### Comparing `cmtestrunner-2.2.5/README.md` & `cmtestrunner-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/__init__.py` & `cmtestrunner-2.2.7/cmtestrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/json_traverser.py` & `cmtestrunner-2.2.7/cmtestrunner/json_traverser.py`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/management/commands/createtest.py` & `cmtestrunner-2.2.7/cmtestrunner/management/commands/createtest.py`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/management/commands/createtestpool.py` & `cmtestrunner-2.2.7/cmtestrunner/management/commands/createtestpool.py`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/management/commands/createunittest.py` & `cmtestrunner-2.2.7/cmtestrunner/management/commands/createunittest.py`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/management/commands/iwanttotest.py` & `cmtestrunner-2.2.7/cmtestrunner/management/commands/iwanttotest.py`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/management/templates/tests_template.txt` & `cmtestrunner-2.2.7/cmtestrunner/management/templates/tests_template.txt`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/management/templates/unit_test_method_template.txt` & `cmtestrunner-2.2.7/cmtestrunner/management/templates/unit_test_method_template.txt`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/middleware.py` & `cmtestrunner-2.2.7/cmtestrunner/middleware.py`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/object_manager.py` & `cmtestrunner-2.2.7/cmtestrunner/object_manager.py`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/templates/exceptions.html` & `cmtestrunner-2.2.7/cmtestrunner/templates/exceptions.html`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/templates/modal.html` & `cmtestrunner-2.2.7/cmtestrunner/templates/modal.html`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/templates/report.html` & `cmtestrunner-2.2.7/cmtestrunner/templates/report.html`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/templates/test_details.html` & `cmtestrunner-2.2.7/cmtestrunner/templates/test_details.html`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/templates/test_pool.html` & `cmtestrunner-2.2.7/cmtestrunner/templates/test_pool.html`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/test.py` & `cmtestrunner-2.2.7/cmtestrunner/test.py`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/cmtestrunner/test_runner.py` & `cmtestrunner-2.2.7/cmtestrunner/test_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
                             parse_snapshot, generate_analytics, get_test_endpoints,
                             Constants, mark_test_as_failed, form_endpoint, replace_context_var,
                             set_default_data_to_context, CustomDict, Context
                         )
 from unittest import TextTestRunner, TextTestResult
 from django.test.runner import DiscoverRunner
 import inspect
-import traceback
 from rest_framework.test import RequestsClient
 from django.conf import settings
 import requests
 import re
 import json
 import os
 import csv
@@ -216,33 +215,36 @@
         return TestRunner.client
     
 
     # see CONTRIBUTING.md for test data formats.
     def verify_test_result(self, exp_response, test_id, accept_lang):
         response_time = None
         response_status_code = None
-
+        exp_response['request_errors'] = None
+ 
         response_ = {}
         if self.response:
             response_time = self.response.get('response_time')
             response_status_code = self.response.get('status_code')
 
         
 
         exp_response_ = copy.deepcopy(exp_response)
+        if exp_response_.get('response'):
+            exp_response_.update(parse_snapshot(exp_response_.pop('response'), self.response))
 
         for key, value in exp_response_.items():
             if accept_lang != 'en':
                 exp_response[key] = self.format_expected_response(
                     exp_response[key], accept_lang)
-            if key == 'response':
-                exp_response.pop('response')
-                exp_response.update(parse_snapshot(value, self.response))   # there is a bug in this line, response may not be a dictionary always
-                response_.update(self.response)
-                continue
+            # if key == 'response':
+            #     exp_response.pop('response')
+            #     exp_response.update(parse_snapshot(value, self.response))   # there is a bug in this line, response may not be a dictionary always
+            #     response_.update(self.response)
+            #     continue
             exp_response[key] = value = parse_snapshot(value, self.response.get(key))
             response_[key] = self.response.get(key)
         exp_response = replace_context_var(exp_response)
         
         self.response = response_
 
         
@@ -296,14 +298,22 @@
         self.set_test_attributes(**kwargs)
         TestRunner.runtime_info['tests'].append(
             dict(name=self.test_name, status='running', total_tests=len(self.test_data), tests_executed=0, completion=0))
       
         with open(settings.TEST_PAYLOAD_PATH + '/data/yml/runtime_info.yml', 'w') as f:
             yaml.dump(dict(runtimeInfo=TestRunner.runtime_info), f)
         for each_test_data in self.test_data:
+            TestRunner.runtime_info['tests'][-1]['completion'] = round(TestRunner.runtime_info['tests'][-1]['tests_executed']/TestRunner.runtime_info['tests'][-1]['total_tests'] * 100, 2)
+            
+            
+            with open(settings.TEST_PAYLOAD_PATH + '/data/yml/runtime_info.yml', 'w') as f:
+                yaml.dump(dict(runtimeInfo=TestRunner.runtime_info), f)
+
+            TestRunner.runtime_info['tests'][-1]['tests_executed'] += 1
+
             self.set_test_vars(each_test_data)
 
             if self.request_body.get(
                     'accept_lang'
             ) and self.request_body.get('accept_lang') != self.accept_lang:
                 TestRunner.total_test_cases -= 1
                 continue
@@ -313,40 +323,39 @@
                 self.request_body.pop('reset_env')
         
             files = self.request_body.pop('files')
             self.request_body = replace_context_var(self.request_body)
             self.request_body['files'] = files
             set_custom_headers(TestRunner.client, replace_context_var(self.custom_headers))
             try:
-                
                 self.response = kwargs.get('test_method')(
                     client=TestRunner.client,
                     request_body=self.request_body,
                     accept_lang=self.accept_lang,
                     headers=self.custom_headers
                     )
                 
             except requests.exceptions.RequestException as e:
-                self.response = dict(errors=e)
+                # print('<><><><><><><><><><><><><><><><><><><><><>',traceback.format_exc())
+                # errors = self.get_error(self.error_info, self.exp_response)
+                self.response = dict(request_errors=e)
             except Exception as e:
+
+                # with self.subTest():
+                #     self.assertEqual(None, e, msg=errors)
                 Constants.EXCEPTIONS.append({
                     'test_method': self.test_method.__name__,
                     'details': e
                 })
                 raise Exception('Exception Occured: ' + str(e))
             
             with self.subTest():
                 TestRunner.total_test_cases += 1
                 self.verify_test_result(self.exp_response, self.test_id,
                                         self.accept_lang)
-                TestRunner.runtime_info['tests'][-1]['tests_executed'] += 1
-                TestRunner.runtime_info['tests'][-1]['completion'] = round(TestRunner.runtime_info['tests'][-1]['tests_executed']/TestRunner.runtime_info['tests'][-1]['total_tests'] * 100, 2)
-                
-                with open(settings.TEST_PAYLOAD_PATH + '/data/yml/runtime_info.yml', 'w') as f:
-                    yaml.dump(dict(runtimeInfo=TestRunner.runtime_info), f)
 
         TestRunner.runtime_info['tests'][-1]['status'] = 'completed'
         TestRunner.runtime_info['tests'][-1]['completion'] = 100
         with open(settings.TEST_PAYLOAD_PATH + '/data/yml/runtime_info.yml', 'w') as f:
             yaml.dump(dict(runtimeInfo=TestRunner.runtime_info), f)
 
     def execute_tests(self, **kwargs):
```

### Comparing `cmtestrunner-2.2.5/cmtestrunner.egg-info/SOURCES.txt` & `cmtestrunner-2.2.7/cmtestrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmtestrunner-2.2.5/setup.py` & `cmtestrunner-2.2.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 setuptools.setup(name='cmtestrunner',
-      version='2.2.5',
+      version='2.2.7',
       description='custom test runner for API test',
       author='Tasin Nawaz',
       author_email='tasin.buet@gmail.com',
       license='CM',
       url='https://github.com/tasin-megamind/cmtestrunner',
       packages=setuptools.find_packages(),
       include_package_data=True,
       install_requires=[
-          'django==2.0.6',
+          'django==2.2.6',
           'djangorestframework==3.8.2',
-          'PyYAML==3.12',
+          'PyYAML==6',
           'requests==2.20.1',
           'numpy>=1.14.1',
       ],
       zip_safe=False)
```

