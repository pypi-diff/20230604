# Comparing `tmp/streamlit-cognito-auth-1.1.1.tar.gz` & `tmp/streamlit-cognito-auth-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-cognito-auth-1.1.1.tar", last modified: Thu Apr  6 14:06:38 2023, max compression
+gzip compressed data, was "streamlit-cognito-auth-1.2.0.tar", last modified: Sun Jun  4 12:40:46 2023, max compression
```

## Comparing `streamlit-cognito-auth-1.1.1.tar` & `streamlit-cognito-auth-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 pop       (1001) pop       (1001)        0 2023-04-06 14:06:38.569018 streamlit-cognito-auth-1.1.1/
--rw-rw-r--   0 pop       (1001) pop       (1001)    11357 2023-04-06 08:51:35.000000 streamlit-cognito-auth-1.1.1/LICENSE
--rw-rw-r--   0 pop       (1001) pop       (1001)     4471 2023-04-06 14:06:38.569018 streamlit-cognito-auth-1.1.1/PKG-INFO
--rw-rw-r--   0 pop       (1001) pop       (1001)     3990 2023-04-06 13:57:28.000000 streamlit-cognito-auth-1.1.1/README.md
--rw-rw-r--   0 pop       (1001) pop       (1001)       38 2023-04-06 14:06:38.569018 streamlit-cognito-auth-1.1.1/setup.cfg
--rw-rw-r--   0 pop       (1001) pop       (1001)      870 2023-04-06 14:01:24.000000 streamlit-cognito-auth-1.1.1/setup.py
-drwxrwxr-x   0 pop       (1001) pop       (1001)        0 2023-04-06 14:06:38.565018 streamlit-cognito-auth-1.1.1/src/
-drwxrwxr-x   0 pop       (1001) pop       (1001)        0 2023-04-06 14:06:38.569018 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth/
--rw-rw-r--   0 pop       (1001) pop       (1001)       39 2023-04-06 08:51:35.000000 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth/__init__.py
--rw-rw-r--   0 pop       (1001) pop       (1001)     9854 2023-04-06 13:55:18.000000 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth/auth.py
--rw-rw-r--   0 pop       (1001) pop       (1001)      153 2023-04-06 08:51:35.000000 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth/exceptions.py
--rw-rw-r--   0 pop       (1001) pop       (1001)      540 2023-04-06 10:43:27.000000 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth/utils.py
-drwxrwxr-x   0 pop       (1001) pop       (1001)        0 2023-04-06 14:06:38.569018 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth.egg-info/
--rw-rw-r--   0 pop       (1001) pop       (1001)     4471 2023-04-06 14:06:38.000000 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth.egg-info/PKG-INFO
--rw-rw-r--   0 pop       (1001) pop       (1001)      426 2023-04-06 14:06:38.000000 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 pop       (1001) pop       (1001)        1 2023-04-06 14:06:38.000000 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 pop       (1001) pop       (1001)       89 2023-04-06 14:06:38.000000 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth.egg-info/requires.txt
--rw-rw-r--   0 pop       (1001) pop       (1001)       23 2023-04-06 14:06:38.000000 streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth.egg-info/top_level.txt
+drwxrwxr-x   0 pop       (1001) pop       (1001)        0 2023-06-04 12:40:46.203379 streamlit-cognito-auth-1.2.0/
+-rw-rw-r--   0 pop       (1001) pop       (1001)    11357 2023-04-06 08:51:35.000000 streamlit-cognito-auth-1.2.0/LICENSE
+-rw-rw-r--   0 pop       (1001) pop       (1001)     4471 2023-06-04 12:40:46.203379 streamlit-cognito-auth-1.2.0/PKG-INFO
+-rw-rw-r--   0 pop       (1001) pop       (1001)     3990 2023-06-04 12:22:23.000000 streamlit-cognito-auth-1.2.0/README.md
+-rw-rw-r--   0 pop       (1001) pop       (1001)       38 2023-06-04 12:40:46.203379 streamlit-cognito-auth-1.2.0/setup.cfg
+-rw-rw-r--   0 pop       (1001) pop       (1001)      870 2023-06-04 12:19:40.000000 streamlit-cognito-auth-1.2.0/setup.py
+drwxrwxr-x   0 pop       (1001) pop       (1001)        0 2023-06-04 12:40:46.195379 streamlit-cognito-auth-1.2.0/src/
+drwxrwxr-x   0 pop       (1001) pop       (1001)        0 2023-06-04 12:40:46.199379 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth/
+-rw-rw-r--   0 pop       (1001) pop       (1001)       39 2023-04-06 08:51:35.000000 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth/__init__.py
+-rw-rw-r--   0 pop       (1001) pop       (1001)    10115 2023-06-04 11:59:02.000000 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth/auth.py
+-rw-rw-r--   0 pop       (1001) pop       (1001)      153 2023-04-06 08:51:35.000000 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth/exceptions.py
+-rw-rw-r--   0 pop       (1001) pop       (1001)      540 2023-04-06 10:43:27.000000 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth/utils.py
+drwxrwxr-x   0 pop       (1001) pop       (1001)        0 2023-06-04 12:40:46.203379 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth.egg-info/
+-rw-rw-r--   0 pop       (1001) pop       (1001)     4471 2023-06-04 12:40:46.000000 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 pop       (1001) pop       (1001)      426 2023-06-04 12:40:46.000000 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 pop       (1001) pop       (1001)        1 2023-06-04 12:40:46.000000 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 pop       (1001) pop       (1001)       89 2023-06-04 12:40:46.000000 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth.egg-info/requires.txt
+-rw-rw-r--   0 pop       (1001) pop       (1001)       23 2023-06-04 12:40:46.000000 streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth.egg-info/top_level.txt
```

### Comparing `streamlit-cognito-auth-1.1.1/LICENSE` & `streamlit-cognito-auth-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-cognito-auth-1.1.1/PKG-INFO` & `streamlit-cognito-auth-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-cognito-auth
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Streamlit component for authenticating users with AWS Cognito
 Home-page: https://github.com/pop-srw/streamlit-cognito-auth
 Author: Sarawin Khemmachotikun
 Author-email: khemmachotikun.s@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -95,15 +95,15 @@
 
 - This package has been tested and known to work with Amazon Cognito pools that have an app client with a secret enabled and using the SRP protocol. Other configurations of Cognito pools may not be supported and have not been tested.
 - This package has been tested and known to work with python 3.8 in Linux environment. It may not work with other versions of python or other operating systems.
 
 ## Features
 
 - [x] Support for Cognito pools with app client secret
-- [ ] Support for Cognito pools without app client secret
+- [x] Support for Cognito pools without app client secret
 - [x] Support for "USER_SRP_AUTH" authentication flow
 - [ ] Support for "REFRESH_TOKEN_AUTH / REFRESH_TOKEN" authentication flow
 - [ ] Support for "USER_PASSWORD_AUTH" authentication flow
 - [x] Support for password reset for temporary password
 - [ ] Support for password reset with OTP
 
 ## Credits
```

### Comparing `streamlit-cognito-auth-1.1.1/README.md` & `streamlit-cognito-auth-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 - This package has been tested and known to work with Amazon Cognito pools that have an app client with a secret enabled and using the SRP protocol. Other configurations of Cognito pools may not be supported and have not been tested.
 - This package has been tested and known to work with python 3.8 in Linux environment. It may not work with other versions of python or other operating systems.
 
 ## Features
 
 - [x] Support for Cognito pools with app client secret
-- [ ] Support for Cognito pools without app client secret
+- [x] Support for Cognito pools without app client secret
 - [x] Support for "USER_SRP_AUTH" authentication flow
 - [ ] Support for "REFRESH_TOKEN_AUTH / REFRESH_TOKEN" authentication flow
 - [ ] Support for "USER_PASSWORD_AUTH" authentication flow
 - [x] Support for password reset for temporary password
 - [ ] Support for password reset with OTP
 
 ## Credits
```

### Comparing `streamlit-cognito-auth-1.1.1/setup.py` & `streamlit-cognito-auth-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="streamlit-cognito-auth",
-    version="1.1.1",
+    version="1.2.0",
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=[
         "boto3 >= 1.26.52",
         "pycognito >= 2022.12.0",
         "streamlit >= 1.17.0",
```

### Comparing `streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth/auth.py` & `streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from .utils import verify_access_token
 
 import pycognito
 from pycognito import AWSSRP
 
 
 class CognitoAuthenticator:
-    def __init__(self, pool_id, app_client_id, app_client_secret, boto_client=None):
+    def __init__(
+        self, pool_id, app_client_id, app_client_secret=None, boto_client=None
+    ):
         self.pool_region = pool_id.split("_")[0]
         self.client = boto_client or boto3.client(
             "cognito-idp", region_name=self.pool_region
         )
         self.pool_id = pool_id
         self.app_client_id = app_client_id
         self.app_client_secret = app_client_secret
@@ -95,22 +97,26 @@
         self.cookie_manager.set(
             "refresh_token",
             tokens["AuthenticationResult"]["RefreshToken"],
             key="set_refresh_token",
         )
 
     def _login(self, username, password):
-        aws_srp = AWSSRP(
-            client=self.client,
-            pool_id=self.pool_id,
-            client_id=self.app_client_id,
-            client_secret=self.app_client_secret,
-            username=username,
-            password=password,
-        )
+        aws_srp_args = {
+            "client": self.client,
+            "pool_id": self.pool_id,
+            "client_id": self.app_client_id,
+            "username": username,
+            "password": password,
+        }
+
+        if self.app_client_secret is not None:
+            aws_srp_args["client_secret"] = self.app_client_secret
+
+        aws_srp = AWSSRP(**aws_srp_args)
         try:
             tokens = aws_srp.authenticate_user()
             self._set_auth_cookies(tokens)
             return True
 
         except pycognito.exceptions.ForceChangePasswordException as e:
             self._set_reset_password_temp("x", username, password)
@@ -130,22 +136,26 @@
 
     def _reset_password(
         self,
         username,
         password,
         new_password,
     ):
-        aws_srp = AWSSRP(
-            client=self.client,
-            pool_id=self.pool_id,
-            client_id=self.app_client_id,
-            client_secret=self.app_client_secret,
-            username=username,
-            password=password,
-        )
+        aws_srp_args = {
+            "client": self.client,
+            "pool_id": self.pool_id,
+            "client_id": self.app_client_id,
+            "username": username,
+            "password": password,
+        }
+
+        if self.app_client_secret is not None:
+            aws_srp_args["client_secret"] = self.app_client_secret
+
+        aws_srp = AWSSRP(**aws_srp_args)
         try:
             tokens = aws_srp.set_new_password_challenge(new_password=new_password)
             self._set_auth_cookies(tokens)
             self._clear_reset_password_temp()
             return True
 
         except self.client.exceptions.NotAuthorizedException as e:
```

### Comparing `streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth/utils.py` & `streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit-cognito-auth-1.1.1/src/streamlit_cognito_auth.egg-info/PKG-INFO` & `streamlit-cognito-auth-1.2.0/src/streamlit_cognito_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-cognito-auth
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Streamlit component for authenticating users with AWS Cognito
 Home-page: https://github.com/pop-srw/streamlit-cognito-auth
 Author: Sarawin Khemmachotikun
 Author-email: khemmachotikun.s@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -95,15 +95,15 @@
 
 - This package has been tested and known to work with Amazon Cognito pools that have an app client with a secret enabled and using the SRP protocol. Other configurations of Cognito pools may not be supported and have not been tested.
 - This package has been tested and known to work with python 3.8 in Linux environment. It may not work with other versions of python or other operating systems.
 
 ## Features
 
 - [x] Support for Cognito pools with app client secret
-- [ ] Support for Cognito pools without app client secret
+- [x] Support for Cognito pools without app client secret
 - [x] Support for "USER_SRP_AUTH" authentication flow
 - [ ] Support for "REFRESH_TOKEN_AUTH / REFRESH_TOKEN" authentication flow
 - [ ] Support for "USER_PASSWORD_AUTH" authentication flow
 - [x] Support for password reset for temporary password
 - [ ] Support for password reset with OTP
 
 ## Credits
```

