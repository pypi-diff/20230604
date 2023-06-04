# Comparing `tmp/minimapi-0.0.5.tar.gz` & `tmp/minimapi-0.0.6.tar.gz`

## Comparing `minimapi-0.0.5.tar` & `minimapi-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 minimapi-0.0.5/build.sh
--rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 minimapi-0.0.5/minimapi.png
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/__init__.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/minimapi.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/sanitizer.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/auth_modules/bearer.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/auth_modules/ecdsa.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/auth_modules/jwt.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/auth_modules/none.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/date.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/email.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/number.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/password.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/pbkdf2.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/sha256.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/text.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/totp.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/data_types/url.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 minimapi-0.0.5/src/minimapi/database_connectors/pysondb.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 minimapi-0.0.5/LICENSE
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 minimapi-0.0.5/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 minimapi-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 minimapi-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 minimapi-0.0.6/build.sh
+-rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 minimapi-0.0.6/minimapi.png
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/__init__.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/minimapi.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/sanitizer.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/auth_modules/bearer.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/auth_modules/ecdsa.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/auth_modules/jwt.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/auth_modules/none.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/data_types/date.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/data_types/email.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/data_types/number.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/data_types/password.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/data_types/pbkdf2.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/data_types/sha256.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/data_types/text.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/data_types/totp.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/data_types/url.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 minimapi-0.0.6/src/minimapi/database_connectors/pysondb.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minimapi-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 minimapi-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 minimapi-0.0.6/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 minimapi-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 minimapi-0.0.6/PKG-INFO
```

### Comparing `minimapi-0.0.5/minimapi.png` & `minimapi-0.0.6/minimapi.png`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.5/src/minimapi/minimapi.py` & `minimapi-0.0.6/src/minimapi/minimapi.py`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.5/src/minimapi/sanitizer.py` & `minimapi-0.0.6/src/minimapi/sanitizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 					type_to_check = self.model[table][property]['type']
 					if 'tags' in self.model[table][property]:
 						
 						if 'encrypted' in self.model[table][property]['tags']:
 							type_to_check = 'text'
 						
 						if 'unlistable' in self.model[table][property]['tags'] and listing:
-							row[property] = '-'
+							row[property] = '•' if bool(result[property]) else ''
 							continue
 
 					if result[property] and not self.check_type(type_to_check, property, result[property]):
 						row[property] = None
 						
 					if type_to_check in self.types and hasattr(self.types[type_to_check], 'response_task') and result[property]:
 						row[property] = self.types[type_to_check].response_task(result[property])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `minimapi-0.0.5/src/minimapi/auth_modules/bearer.py` & `minimapi-0.0.6/src/minimapi/auth_modules/bearer.py`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.5/src/minimapi/auth_modules/ecdsa.py` & `minimapi-0.0.6/src/minimapi/auth_modules/ecdsa.py`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.5/src/minimapi/auth_modules/jwt.py` & `minimapi-0.0.6/src/minimapi/auth_modules/jwt.py`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.5/src/minimapi/data_types/pbkdf2.py` & `minimapi-0.0.6/src/minimapi/data_types/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.5/src/minimapi/database_connectors/pysondb.py` & `minimapi-0.0.6/src/minimapi/database_connectors/pysondb.py`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.5/LICENSE` & `minimapi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.5/README.md` & `minimapi-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `minimapi-0.0.5/pyproject.toml` & `minimapi-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "minimapi"
-version = "0.0.5"
+version = "0.0.6"
 description = "Easy and simple REST API from model"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'flask >= 2.2.0',
   'pysondb >= 1.6.7',
   'pyjwt >= 2.6.0',
```

### Comparing `minimapi-0.0.5/PKG-INFO` & `minimapi-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minimapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Easy and simple REST API from model
 Project-URL: Homepage, https://github.com/minimapi/minimapi
 Project-URL: Bug Tracker, https://github.com/minimapi/minimapi/issues
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
```

