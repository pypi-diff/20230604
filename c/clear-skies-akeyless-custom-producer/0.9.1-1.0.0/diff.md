# Comparing `tmp/clear-skies-akeyless-custom-producer-0.9.1.tar.gz` & `tmp/clear_skies_akeyless_custom_producer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear-skies-akeyless-custom-producer-0.9.1.tar", last modified: Mon May 15 23:28:57 2023, max compression
+gzip compressed data, was "clear_skies_akeyless_custom_producer-1.0.0.tar", max compression
```

## Comparing `clear-skies-akeyless-custom-producer-0.9.1.tar` & `clear_skies_akeyless_custom_producer-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,10 @@
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1053 2023-05-10 15:19:24.000000 clear-skies-akeyless-custom-producer-0.9.1/LICENSE
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       25 2023-05-10 10:53:24.000000 clear-skies-akeyless-custom-producer-0.9.1/MANIFEST.in
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6920 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6259 2023-05-12 15:20:11.000000 clear-skies-akeyless-custom-producer-0.9.1/README.md
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/setup.cfg
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1415 2023-05-15 23:26:56.000000 clear-skies-akeyless-custom-producer-0.9.1/setup.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 23:28:57.180132 clear-skies-akeyless-custom-producer-0.9.1/src/
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6920 2023-05-15 23:28:57.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      604 2023-05-15 23:28:57.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/SOURCES.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2023-05-15 23:28:57.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/dependency_links.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       12 2023-05-15 23:28:57.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/requires.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       36 2023-05-15 23:28:57.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/top_level.txt
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       23 2023-05-10 10:54:42.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       30 2023-05-11 19:55:49.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10449 2023-05-15 23:26:29.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/no_input.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5948 2023-05-12 14:49:21.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/with_input.py
+-rw-r--r--   0        0        0     1053 2023-05-10 15:19:24.285335 clear_skies_akeyless_custom_producer-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6259 2023-05-12 15:20:11.769906 clear_skies_akeyless_custom_producer-1.0.0/README.md
+-rw-r--r--   0        0        0      664 2023-06-04 14:40:58.806745 clear_skies_akeyless_custom_producer-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-10 10:54:42.233306 clear_skies_akeyless_custom_producer-1.0.0/src/clearskies_akeyless_custom_producer/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-11 19:55:49.528090 clear_skies_akeyless_custom_producer-1.0.0/src/clearskies_akeyless_custom_producer/handlers/__init__.py
+-rw-r--r--   0        0        0     9756 2023-06-01 11:15:55.029296 clear_skies_akeyless_custom_producer-1.0.0/src/clearskies_akeyless_custom_producer/handlers/no_input.py
+-rw-r--r--   0        0        0     7392 2023-06-01 11:17:20.022617 clear_skies_akeyless_custom_producer-1.0.0/src/clearskies_akeyless_custom_producer/handlers/no_input_test.py
+-rw-r--r--   0        0        0     5948 2023-05-12 14:49:21.358575 clear_skies_akeyless_custom_producer-1.0.0/src/clearskies_akeyless_custom_producer/handlers/with_input.py
+-rwxr-xr-x   0        0        0      705 2023-05-10 10:53:24.580923 clear_skies_akeyless_custom_producer-1.0.0/src/test.py
+-rw-r--r--   0        0        0     7063 1970-01-01 00:00:00.000000 clear_skies_akeyless_custom_producer-1.0.0/PKG-INFO
```

### Comparing `clear-skies-akeyless-custom-producer-0.9.1/LICENSE` & `clear_skies_akeyless_custom_producer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clear-skies-akeyless-custom-producer-0.9.1/PKG-INFO` & `clear_skies_akeyless_custom_producer-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: clear-skies-akeyless-custom-producer
-Version: 0.9.1
+Version: 1.0.0
 Summary: clearskies handlers for hosting Akeyless custom producer endpoints
 Home-page: https://github.com/cmancone/clearskies-akeyless-custom-producer
+License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
-License: MIT
-Keywords: setuptools development
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: clear-skies (>=1.14.4,<2.0.0)
+Project-URL: Repository, https://github.com/cmancone/clearskies-akeyless-custom-producer
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # clearskies-akeyless-custom-producer
 
 Contains clearskies handlers that should make it very easy to create custom producers for Akeyless.
 
 There are a variety of ways to manage custom producers for Akeyless.  The strategy utilized in this library is aimed at creating a stateless set of producer endpoints.  This works because you can store a payload in the customer producer in Akeless, and then Akeyless will provide this to the custom producer endpoint when it calls them.  As a result, the custom producer endpoints make use of the data provided in the payload rather than storing any secrets themselves.  This dramatically simplifies management of the endpoints.  In addition, this removes the need to manage authentication and authorization.  The reason is because Akeyless will only call your endpoint and pass along the payload in the event that it received a properly authorized request.  Therefore, the payload will only be present for authorized users, and since the custom producer endpoints don't store any credentials on their own, they are incapable of fulfilling requests on their own without being called properly by Akeyless.
 
@@ -142,7 +143,8 @@
     }
 )
 ```
 
 # With Input
 
 Akeyless provides an option for allowing the client to pass additional input to the custom produccer which it can use when issuing credentials.  It's important to be very careful when processing user input in these cases, to ensure that users can't arbitrarily adjust the permissions of the generated credentials.  Still, if you want to allow users to impact the credential generation process, you can do that using the `WithInput` handler (which doesn't exist yet).
+
```

### Comparing `clear-skies-akeyless-custom-producer-0.9.1/README.md` & `clear_skies_akeyless_custom_producer-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/no_input.py` & `clear_skies_akeyless_custom_producer-1.0.0/src/clearskies_akeyless_custom_producer/handlers/no_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -131,16 +131,15 @@
         # we need to return a meaningful id if we are going to revoke at the end
         if self.configuration('can_revoke'):
             id_column_name = self.configuration('id_column_name')
             if id_column_name not in credentials:
                 raise ValueError(
                     f"Response from create callable did not include the required id column: '{id_column_name}'"
                 )
-            # this is stupid but I'm doing it - see the revoke function for reasons
-            credential_id = credentials[id_column_name].replace('_', 'ZZZZ----AAAA')
+            credential_id = credentials[id_column_name]
         else:
             credential_id = 'i_dont_need_an_id'
 
         return input_output.respond({
             'id': credential_id,
             'response': credentials,
         }, 200)
@@ -174,21 +173,15 @@
         except InputError as e:
             return self.error(input_output, e.errors, 400)
 
         errors = self._check_payload(payload)
         if errors:
             return self.input_errors(input_output, errors)
 
-        for raw_id in ids:
-            # Akeyless prepends some stuff to the id to make it unique, which we have to remove.
-            # They will stick some parts and separate things with an underscore.  We therefore want
-            # to split on an underscore and grab the part at the end.  This can cause trouble if the
-            # id itself contains an underscore.  To avoid this, the create function replaces underscores
-            # with a string that is very unlikely to exist in the actual id, so we have to reverse that.
-            id = raw_id.split('_')[-1].replace('ZZZZ----AAAA', '_')
+        for id in ids:
             self._di.call_function(
                 self.configuration('revoke_callable'),
                 **payload,
                 payload=payload,
                 id_to_delete=id,
             )
```

### Comparing `clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/with_input.py` & `clear_skies_akeyless_custom_producer-1.0.0/src/clearskies_akeyless_custom_producer/handlers/with_input.py`

 * *Files identical despite different names*

