# Comparing `tmp/roco-0.1.0.tar.gz` & `tmp/roco-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roco-0.1.0.tar", max compression
+gzip compressed data, was "roco-0.1.1.tar", max compression
```

## Comparing `roco-0.1.0.tar` & `roco-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1676 2023-06-02 06:31:09.431216 roco-0.1.0/README.md
--rw-r--r--   0        0        0      448 2023-06-02 06:20:01.623968 roco-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-01 06:31:27.843640 roco-0.1.0/roco/__init__.py
--rw-r--r--   0        0        0      542 2023-06-02 06:20:07.871975 roco-0.1.0/roco/bin/cli.py
--rw-r--r--   0        0        0     1423 2023-06-02 05:51:24.730781 roco-0.1.0/roco/config.py
--rw-r--r--   0        0        0      572 2023-06-02 05:53:54.441615 roco-0.1.0/roco/main.py
--rw-r--r--   0        0        0      575 2023-06-02 05:04:45.847069 roco-0.1.0/roco/templates/runtime-config.js.jinja2
--rw-r--r--   0        0        0     2152 1970-01-01 00:00:00.000000 roco-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10231 2023-06-04 06:19:17.723918 roco-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1572 2023-06-04 06:19:17.723918 roco-0.1.1/README.md
+-rw-r--r--   0        0        0      718 2023-06-04 06:19:17.723918 roco-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-04 06:19:17.723918 roco-0.1.1/roco/__init__.py
+-rw-r--r--   0        0        0      542 2023-06-04 06:19:17.723918 roco-0.1.1/roco/bin/cli.py
+-rw-r--r--   0        0        0     1583 2023-06-04 06:19:17.723918 roco-0.1.1/roco/config.py
+-rw-r--r--   0        0        0      572 2023-06-04 06:19:17.723918 roco-0.1.1/roco/main.py
+-rw-r--r--   0        0        0      547 2023-06-04 06:19:17.723918 roco-0.1.1/roco/templates/runtime-config.js.jinja2
+-rw-r--r--   0        0        0     2316 1970-01-01 00:00:00.000000 roco-0.1.1/PKG-INFO
```

### Comparing `roco-0.1.0/README.md` & `roco-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # Roco - Runtime config generator
 
 Command line utility tool which prints to the standard output javascript valid 
 text generated from environment variables.
 
 For example, given following environment variables:
 
-    PAPERMERGE__AUTH__REDIRECT_URI=http://localhost:9000/callback
-    PAPERMERGE__AUTH__INTERNAL_TOKEN_URL=http://localhost:9000/api/token
     PAPERMERGE__AUTH__GOOGLE_CLIENT_ID=some-id.apps.googleusercontent.com
     PAPERMERGE__AUTH__GOOGLE_AUTHORIZE_URL=https://accounts.google.com/o/oauth2/auth
+    PAPERMERGE__AUTH__GOOGLE_REDIRECT_URI=http://localhost:11000/google/callback
 
 will result in the following text (valid javascript) as output:
 
     window.__PAPERMERGE_RUNTIME_CONFIG__ = {
       oauth2: {
-        internal_token_url: 'http://localhost:9000/api/token',
-        redirect_uri: 'http://localhost:9000/callback',
         google: {
           client_id: 'some-id.apps.googleusercontent.com',
           authorize_url: 'https://accounts.google.com/o/oauth2/auth',
+          redirect_uri: 'http://localhost:11000/google/callback',
           scope: 'openid email',
         },
       }
     };
 
 
 ## Install
@@ -46,14 +44,13 @@
     
     roco -s
 
 The above command will also show the env var prefix i.e. `PAPERMERGE__AUTH__`.
 
 Roco reads from following environment variables:
 
-* `PAPERMERGE__AUTH__REDIRECT_URI`
-* `PAPERMERGE__AUTH__INTERNAL_TOKEN_URL`
 * `PAPERMERGE__AUTH__GOOGLE_AUTHORIZE_URL`
 * `PAPERMERGE__AUTH__GOOGLE_CLIENT_ID`
+* `PAPERMERGE__AUTH__GOOGLE_REDIRECT_URI`
 * `PAPERMERGE__AUTH__GITHUB_AUTHORIZE_URL`
 * `PAPERMERGE__AUTH__GITHUB_CLIENT_ID`
-
+* `PAPERMERGE__AUTH__GITHUB_REDIRECT_URI`
```

### Comparing `roco-0.1.0/roco/bin/cli.py` & `roco-0.1.1/roco/bin/cli.py`

 * *Files identical despite different names*

### Comparing `roco-0.1.0/roco/config.py` & `roco-0.1.1/roco/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-from pydantic import BaseSettings, root_validator, validator
+from pydantic import BaseSettings, root_validator
 
 
 class Settings(BaseSettings):
 
-    internal_token_url: str | None = None
-    redirect_uri: str | None = None
-
     google_client_id: str | None = None
     google_authorize_url: str | None = None
+    google_redirect_uri: str | None = None
     google_scope: str = 'openid email'
 
     github_client_id: str | None = None
     github_authorize_url: str | None = None
+    github_redirect_uri: str | None = None
     github_scope: str = 'openid email'
 
-    # will be true if both `internal_token_url` and `redirect_uri`
-    # are non-empty
-    oauth2: bool = False
-
-    @validator("oauth2", always=True)
-    def validator_oauth2(cls, value, values):
-        """
-        oauth2 field will be True if both internal_token_url
-        and redirect_uri are non-empty
-        """
-        if values["internal_token_url"] and values["redirect_uri"]:
-            return True
-
-        return False
-
     @root_validator
     def check_google_params(cls, values):
-        two_values = [
+        three_values = [
             values.get('google_client_id'),
-            values.get('google_authorize_url')
+            values.get('google_authorize_url'),
+            values.get('google_redirect_uri')
         ]
-        count = len([v for v in two_values if v])
+        count = len([v for v in three_values if v])
 
-        if count not in (0, 2):
+        if count not in (0, 3):
             raise ValueError(
-                'google_client_id and google_authorize_url should be'
-                ' either both absent or both present'
+                'google_client_id, google_authorize_url and google_redirect_uri'
+                ' should be either all absent or all present'
             )
 
         return values
 
+    @root_validator
+    def check_github_params(cls, values):
+        three_values = [
+            values.get('github_client_id'),
+            values.get('github_authorize_url'),
+            values.get('github_redirect_uri')
+        ]
+        count = len([v for v in three_values if v])
+
+        if count not in (0, 3):
+            raise ValueError(
+                'github_client_id, github_authorize_url and github_redirect_uri'
+                ' should be either all absent or all present'
+            )
+
+        return values
 
     class Config:
         env_prefix = 'PAPERMERGE__AUTH__'
 
 
 def get_settings():
     return Settings()
```

### Comparing `roco-0.1.0/roco/main.py` & `roco-0.1.1/roco/main.py`

 * *Files identical despite different names*

### Comparing `roco-0.1.0/roco/templates/runtime-config.js.jinja2` & `roco-0.1.1/roco/templates/runtime-config.js.jinja2`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 window.__PAPERMERGE_RUNTIME_CONFIG__ = {
-  {%- if oauth2 %}
   oauth2: {
-    internal_token_url: '{{ internal_token_url }}',
-    redirect_uri: '{{ redirect_uri }}',
     {%- if google_client_id %}
     google: {
       client_id: '{{ google_client_id }}',
       authorize_url: '{{ google_authorize_url }}',
+      redirect_uri: '{{ google_redirect_uri }}',
       scope: '{{ google_scope }}',
     },
     {%- endif %}
     {%- if github_client_id %}
     github: {
       client_id: '{{ github_client_id }}',
       authorize_url: '{{ github_authorize_url }}',
+      redirect_uri: '{{ github_redirect_uri }}',
       scope: 'openid email',
     }
     {%- endif %}
   }
-  {%- endif %}
 };
```

### Comparing `roco-0.1.0/PKG-INFO` & `roco-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
 Name: roco
-Version: 0.1.0
+Version: 0.1.1
 Summary: Runtime Config Generator
+Home-page: https://github.com/papermerge/roco
+License: Apache 2.0
 Author: Eugen Ciur
 Author-email: eugen@papermerge.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Description-Content-Type: text/markdown
@@ -16,28 +22,26 @@
 # Roco - Runtime config generator
 
 Command line utility tool which prints to the standard output javascript valid 
 text generated from environment variables.
 
 For example, given following environment variables:
 
-    PAPERMERGE__AUTH__REDIRECT_URI=http://localhost:9000/callback
-    PAPERMERGE__AUTH__INTERNAL_TOKEN_URL=http://localhost:9000/api/token
     PAPERMERGE__AUTH__GOOGLE_CLIENT_ID=some-id.apps.googleusercontent.com
     PAPERMERGE__AUTH__GOOGLE_AUTHORIZE_URL=https://accounts.google.com/o/oauth2/auth
+    PAPERMERGE__AUTH__GOOGLE_REDIRECT_URI=http://localhost:11000/google/callback
 
 will result in the following text (valid javascript) as output:
 
     window.__PAPERMERGE_RUNTIME_CONFIG__ = {
       oauth2: {
-        internal_token_url: 'http://localhost:9000/api/token',
-        redirect_uri: 'http://localhost:9000/callback',
         google: {
           client_id: 'some-id.apps.googleusercontent.com',
           authorize_url: 'https://accounts.google.com/o/oauth2/auth',
+          redirect_uri: 'http://localhost:11000/google/callback',
           scope: 'openid email',
         },
       }
     };
 
 
 ## Install
@@ -61,15 +65,14 @@
     
     roco -s
 
 The above command will also show the env var prefix i.e. `PAPERMERGE__AUTH__`.
 
 Roco reads from following environment variables:
 
-* `PAPERMERGE__AUTH__REDIRECT_URI`
-* `PAPERMERGE__AUTH__INTERNAL_TOKEN_URL`
 * `PAPERMERGE__AUTH__GOOGLE_AUTHORIZE_URL`
 * `PAPERMERGE__AUTH__GOOGLE_CLIENT_ID`
+* `PAPERMERGE__AUTH__GOOGLE_REDIRECT_URI`
 * `PAPERMERGE__AUTH__GITHUB_AUTHORIZE_URL`
 * `PAPERMERGE__AUTH__GITHUB_CLIENT_ID`
-
+* `PAPERMERGE__AUTH__GITHUB_REDIRECT_URI`
```

