# Comparing `tmp/bovine_herd-0.2.5.tar.gz` & `tmp/bovine_herd-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_herd-0.2.5.tar", max compression
+gzip compressed data, was "bovine_herd-0.2.6.tar", max compression
```

## Comparing `bovine_herd-0.2.5.tar` & `bovine_herd-0.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1345 2023-05-28 14:52:06.773617 bovine_herd-0.2.5/README.md
--rw-r--r--   0        0        0     1513 2023-05-28 14:52:06.773617 bovine_herd-0.2.5/bovine_herd/__init__.py
--rw-r--r--   0        0        0      275 2023-05-28 14:52:06.773617 bovine_herd-0.2.5/bovine_herd/server/__init__.py
--rw-r--r--   0        0        0     1466 2023-05-28 14:52:06.773617 bovine_herd-0.2.5/bovine_herd/server/activitypub.py
--rw-r--r--   0        0        0     4986 2023-05-28 14:52:06.773617 bovine_herd-0.2.5/bovine_herd/server/endpoints.py
--rw-r--r--   0        0        0     2000 2023-05-28 14:52:06.773617 bovine_herd-0.2.5/bovine_herd/server/wellknown.py
--rw-r--r--   0        0        0      521 2023-05-28 14:52:06.773617 bovine_herd-0.2.5/bovine_herd/utils/__init__.py
--rw-r--r--   0        0        0     1084 2023-05-28 14:52:06.777617 bovine_herd-0.2.5/bovine_herd/utils/test/__init__.py
--rw-r--r--   0        0        0      274 2023-05-28 14:52:06.777617 bovine_herd-0.2.5/bovine_herd/utils/test_utils.py
--rw-r--r--   0        0        0       23 2023-05-28 14:52:06.777617 bovine_herd-0.2.5/bovine_herd/version.py
--rw-r--r--   0        0        0      875 2023-05-28 14:52:15.973751 bovine_herd-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 bovine_herd-0.2.5/setup.py
--rw-r--r--   0        0        0     2197 1970-01-01 00:00:00.000000 bovine_herd-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1243 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/README.md
+-rw-r--r--   0        0        0     1513 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/__init__.py
+-rw-r--r--   0        0        0      275 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/server/__init__.py
+-rw-r--r--   0        0        0     1466 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/server/activitypub.py
+-rw-r--r--   0        0        0     4986 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/server/endpoints.py
+-rw-r--r--   0        0        0     2015 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/server/wellknown.py
+-rw-r--r--   0        0        0      521 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/utils/__init__.py
+-rw-r--r--   0        0        0     1084 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/utils/test/__init__.py
+-rw-r--r--   0        0        0      274 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/utils/test_utils.py
+-rw-r--r--   0        0        0       23 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/version.py
+-rw-r--r--   0        0        0      875 2023-06-04 18:36:21.134507 bovine_herd-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 bovine_herd-0.2.6/setup.py
+-rw-r--r--   0        0        0     2095 1970-01-01 00:00:00.000000 bovine_herd-0.2.6/PKG-INFO
```

### Comparing `bovine_herd-0.2.5/README.md` & `bovine_herd-0.2.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 hypercorn bovine_herd:app
 ```
 
 This will start `bovine_herd` using an sqlite3 database.
 
 ## Interacting with the fediverse
 
-Assume that you alias `$DOMAIN` so that it redirects to the above server, e.g. via....
-
-Then by running
+Assume that you alias `$DOMAIN` so that it redirects to the above server. Then by running
 
 ```bash
 pip install bovine_tool
 python -mbovine_tool.register --domain $DOMAIN moocow
 ```
 
 you create a new account for __moocow__. This command returns its bovine name, which will be of the form `moocow + uuid4()`, e.g. `moocow_09c80006-483c-4826-b48c-cf5134b4e898`. By running:
@@ -35,8 +33,7 @@
 ```
 
 ## Configuration
 
 The default database connection is "sqlite://bovine.sqlite3". This can be overwridden with the environment variable "BOVINE_DB_URL".
 
 - `BOVINE_REDIS` represents how to reach redis, e.g. `redis://localhost`. If not set, redis is not used. Redis is necessary when using more than one worker.
-- `BOVINE_LOGFILE` gives the path of the log file. When not present bovine.log is used.
```

### Comparing `bovine_herd-0.2.5/bovine_herd/__init__.py` & `bovine_herd-0.2.6/bovine_herd/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.5/bovine_herd/server/activitypub.py` & `bovine_herd-0.2.6/bovine_herd/server/activitypub.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.5/bovine_herd/server/endpoints.py` & `bovine_herd-0.2.6/bovine_herd/server/endpoints.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.5/bovine_herd/server/wellknown.py` & `bovine_herd-0.2.6/bovine_herd/server/wellknown.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,29 +35,29 @@
         return {"error": "invalid request"}, 400
 
     return await webfinger_response(resource)
 
 
 async def webfinger_response(resource):
     domain = request.host
-    name = None
+    account = None
 
     if resource == f"acct:bovine@{domain}":
-        name = "bovine"
+        account = resource
         url = f"https://{domain}/activitypub/bovine"
     else:
         logger.debug("Got resource %s", resource)
         bovine_store = current_app.config["bovine_store"]
-        name, url = await bovine_store.get_name_url_for_did(resource)
+        account, url = await bovine_store.get_account_url_for_identity(resource)
 
-        if not name:
+        if not account:
             return {"status": "not found"}, 404
 
     return (
-        webfinger_response_json(name, url, domain),
+        webfinger_response_json(account, url),
         200,
         {"content-type": "application/jrd+json"},
     )
 
 
 @wellknown.get("/host-meta")
 async def wellknown_host_meta():
```

### Comparing `bovine_herd-0.2.5/bovine_herd/utils/__init__.py` & `bovine_herd-0.2.6/bovine_herd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.5/bovine_herd/utils/test/__init__.py` & `bovine_herd-0.2.6/bovine_herd/utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.5/pyproject.toml` & `bovine_herd-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine-herd"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bovine_herd"}]
 repository = "https://codeberg.org/bovine/bovine"
 
 [tool.poetry.dependencies]
```

### Comparing `bovine_herd-0.2.5/setup.py` & `bovine_herd-0.2.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,17 @@
  'bovine-store>=0.2.1,<0.3.0',
  'markdown>=3.4.1,<4.0.0',
  'python-markdown-math>=0.8,<0.9',
  'tortoise-orm[asyncpg]>=0.19.3,<0.20.0']
 
 setup_kwargs = {
     'name': 'bovine-herd',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': '',
-    'long_description': '# bovine_herd\n\n`bovine_herd` is a `bovine` powered ActivityPub server, which interoperates with the rest of the FediVerse.\n\nRunning:\n\n```bash\npip install bovine_herd\nhypercorn bovine_herd:app\n```\n\nThis will start `bovine_herd` using an sqlite3 database.\n\n## Interacting with the fediverse\n\nAssume that you alias `$DOMAIN` so that it redirects to the above server, e.g. via....\n\nThen by running\n\n```bash\npip install bovine_tool\npython -mbovine_tool.register --domain $DOMAIN moocow\n```\n\nyou create a new account for __moocow__. This command returns its bovine name, which will be of the form `moocow + uuid4()`, e.g. `moocow_09c80006-483c-4826-b48c-cf5134b4e898`. By running:\n\n```bash\npython -mbovine_tool.manage --new_did_key $BOVINE_NAME\n```\n\nyou will be given a secret (an Ed25519 private key, i.e. starts with `z3u2`). Once you have this secret, you can send a message via\n\n```bash\npython -mbovine.msg --secret $SECRET --host $DOMAIN moooo\n```\n\n## Configuration\n\nThe default database connection is "sqlite://bovine.sqlite3". This can be overwridden with the environment variable "BOVINE_DB_URL".\n\n- `BOVINE_REDIS` represents how to reach redis, e.g. `redis://localhost`. If not set, redis is not used. Redis is necessary when using more than one worker.\n- `BOVINE_LOGFILE` gives the path of the log file. When not present bovine.log is used.\n',
+    'long_description': '# bovine_herd\n\n`bovine_herd` is a `bovine` powered ActivityPub server, which interoperates with the rest of the FediVerse.\n\nRunning:\n\n```bash\npip install bovine_herd\nhypercorn bovine_herd:app\n```\n\nThis will start `bovine_herd` using an sqlite3 database.\n\n## Interacting with the fediverse\n\nAssume that you alias `$DOMAIN` so that it redirects to the above server. Then by running\n\n```bash\npip install bovine_tool\npython -mbovine_tool.register --domain $DOMAIN moocow\n```\n\nyou create a new account for __moocow__. This command returns its bovine name, which will be of the form `moocow + uuid4()`, e.g. `moocow_09c80006-483c-4826-b48c-cf5134b4e898`. By running:\n\n```bash\npython -mbovine_tool.manage --new_did_key $BOVINE_NAME\n```\n\nyou will be given a secret (an Ed25519 private key, i.e. starts with `z3u2`). Once you have this secret, you can send a message via\n\n```bash\npython -mbovine.msg --secret $SECRET --host $DOMAIN moooo\n```\n\n## Configuration\n\nThe default database connection is "sqlite://bovine.sqlite3". This can be overwridden with the environment variable "BOVINE_DB_URL".\n\n- `BOVINE_REDIS` represents how to reach redis, e.g. `redis://localhost`. If not set, redis is not used. Redis is necessary when using more than one worker.\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/bovine/bovine',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bovine_herd-0.2.5/PKG-INFO` & `bovine_herd-0.2.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine-herd
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Home-page: https://codeberg.org/bovine/bovine
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -32,17 +32,15 @@
 hypercorn bovine_herd:app
 ```
 
 This will start `bovine_herd` using an sqlite3 database.
 
 ## Interacting with the fediverse
 
-Assume that you alias `$DOMAIN` so that it redirects to the above server, e.g. via....
-
-Then by running
+Assume that you alias `$DOMAIN` so that it redirects to the above server. Then by running
 
 ```bash
 pip install bovine_tool
 python -mbovine_tool.register --domain $DOMAIN moocow
 ```
 
 you create a new account for __moocow__. This command returns its bovine name, which will be of the form `moocow + uuid4()`, e.g. `moocow_09c80006-483c-4826-b48c-cf5134b4e898`. By running:
@@ -58,9 +56,8 @@
 ```
 
 ## Configuration
 
 The default database connection is "sqlite://bovine.sqlite3". This can be overwridden with the environment variable "BOVINE_DB_URL".
 
 - `BOVINE_REDIS` represents how to reach redis, e.g. `redis://localhost`. If not set, redis is not used. Redis is necessary when using more than one worker.
-- `BOVINE_LOGFILE` gives the path of the log file. When not present bovine.log is used.
```

