# Comparing `tmp/pyaddepar-0.6.2.tar.gz` & `tmp/pyaddepar-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyaddepar-0.6.2.tar", last modified: Thu May 28 21:24:11 2020, max compression
+gzip compressed data, was "pyaddepar-0.7.0.tar", max compression
```

## Comparing `pyaddepar-0.6.2.tar` & `pyaddepar-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,6 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-28 21:24:11.000000 pyaddepar-0.6.2/
--rw-r--r--   0 root         (0) root         (0)       62 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2728 2020-05-28 21:24:11.000000 pyaddepar-0.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1873 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-28 21:24:11.000000 pyaddepar-0.6.2/license/
--rw-r--r--   0 root         (0) root         (0)     1542 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/license/NUMPY_LICENSE
--rw-r--r--   0 root         (0) root         (0)     3768 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/license/PANDAS_LICENSE
--rw-r--r--   0 root         (0) root         (0)    14230 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/license/PSF_LICENSE
--rw-r--r--   0 root         (0) root         (0)      549 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/license/REQUESTS_LICENCE
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-28 21:24:11.000000 pyaddepar-0.6.2/pyaddepar/
--rw-r--r--   0 root         (0) root         (0)      158 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/pyaddepar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5338 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/pyaddepar/addeparrequest.py
--rw-r--r--   0 root         (0) root         (0)     2049 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/pyaddepar/flask_addepar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-28 21:24:11.000000 pyaddepar-0.6.2/pyaddepar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2728 2020-05-28 21:24:10.000000 pyaddepar-0.6.2/pyaddepar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      409 2020-05-28 21:24:10.000000 pyaddepar-0.6.2/pyaddepar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-05-28 21:24:10.000000 pyaddepar-0.6.2/pyaddepar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2020-05-28 21:24:10.000000 pyaddepar-0.6.2/pyaddepar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2020-05-28 21:24:10.000000 pyaddepar-0.6.2/pyaddepar.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2020-05-28 21:24:11.000000 pyaddepar-0.6.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      665 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-05-28 21:24:11.000000 pyaddepar-0.6.2/test/
--rw-r--r--   0 root         (0) root         (0)     1159 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/test/test_app.py
--rw-r--r--   0 root         (0) root         (0)     4289 2020-05-28 21:18:47.000000 pyaddepar-0.6.2/test/test_request.py
+-rw-r--r--   0        0        0     1772 2023-06-04 04:13:32.729812 pyaddepar-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-04 04:13:32.729812 pyaddepar-0.7.0/pyaddepar/__init__.py
+-rw-r--r--   0        0        0     6014 2023-06-04 04:13:32.733812 pyaddepar-0.7.0/pyaddepar/addeparrequest.py
+-rw-r--r--   0        0        0     2127 2023-06-04 04:13:32.733812 pyaddepar-0.7.0/pyaddepar/flask_addepar.py
+-rw-r--r--   0        0        0      491 2023-06-04 04:13:58.550195 pyaddepar-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 pyaddepar-0.7.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyaddepar-0.6.2/README.md` & `pyaddepar-0.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# pyaddepar
-[![Action Status](https://github.com/lobnek/pyaddepar/workflows/CI/badge.svg)](https://github.com/lobnek/pyaddepar/actions/)
-
+# [pyaddepar](http://lobnek.github.io/pyaddepar/)
 
 Some utility code for interacting with addepar. For more information on addepar please check out
 https://addepar.com/.
 
 ## Installing pyaddepar
 Install with pip
 ```
 pip install pyaddepar
 ```
 
-    
+
 ## AddeparRequest
 AddeparRequest is a class hiding the management of your key(s), the pagination of requests and conversion of your results to standard pandas containers.
 
 ```
 import pandas as pd
 from pyaddepar.addeparrequest import AddeparRequest
 
@@ -30,15 +28,15 @@
             print(entity)
             print(entity["option_type"])
             print(entity["node_strike_price"])
 
             print((expiry-today).days/365.0)
 
 ```
-    
+
 ## Settings.cfg
 We recommend to define a configuration file `(*.cfg)` containing
 
 ADDEPAR = {"key":"A",
            "secret":"B",
            "id":"maffay",
            "company":"maffay"
@@ -54,15 +52,14 @@
 
 from pyaddepar.flask_addepar import addepar
 
 if __name__ == '__main__':
     app = Flask(__name__)
     app.config.from_pyfile('config/settings.cfg')
     addepar.init_app(app)
-    
+
     with app.app_context():
         for key, entity in addepar.request.entities():
             print(key)
             print(entity)
 
 ```
-
```

### Comparing `pyaddepar-0.6.2/pyaddepar/addeparrequest.py` & `pyaddepar-0.7.0/pyaddepar/addeparrequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import io
 import json
 import logging
 import os
 from enum import Enum
 
 import pandas as pd
 import requests
-import io
 
 
 class OutputType(Enum):
     CSV = "csv"
     JSON = "json"
     TSV = "tsv"
     XLSX = "xlsx"
@@ -37,68 +40,120 @@
 
     @property
     def auth(self):
         return self.key, self.secret
 
     @property
     def headers(self):
-        return {"Accept": "*/*", "Addepar-Firm": self.id, "content-type": "application/vnd.api+json"}
+        return {
+            "Accept": "*/*",
+            "Addepar-Firm": self.id,
+            "content-type": "application/vnd.api+json",
+        }
 
     @staticmethod
     def dicturl(d):
-        return '&'.join(["{key}={value}".format(key=key, value=value) for key, value in d.items()])
+        return "&".join(
+            ["{key}={value}".format(key=key, value=value) for key, value in d.items()]
+        )
 
     def get(self, request):
-        request = "https://{company}.addepar.com/api{request}".format(request=request, company=self.company)
-        self.logger.debug("Request: {request}, Headers: {headers}".format(request=request, headers=self.headers))
+        request = "https://{company}.addepar.com/api{request}".format(
+            request=request, company=self.company
+        )
+        self.logger.debug(
+            "Request: {request}, Headers: {headers}".format(
+                request=request, headers=self.headers
+            )
+        )
 
         r = requests.get(request, auth=(self.key, self.secret), headers=self.headers)
-        assert r.ok, "Invalid response. Statuscode {code}. Query: {x}".format(code=r.status_code, x=request)
+        assert r.ok, "Invalid response. Statuscode {code}. Query: {x}".format(
+            code=r.status_code, x=request
+        )
         return r
 
     def post(self, data, request="entities"):
-        r = "https://{company}.addepar.com/api/v1/{request}".format(request=request, company=self.company)
-        self.logger.debug("Request: {request}, Headers: {headers}".format(request=r, headers=self.headers))
-        r = requests.post(r, auth=(self.key, self.secret), headers=self.headers, data=json.dumps(data))
+        r = "https://{company}.addepar.com/api/v1/{request}".format(
+            request=request, company=self.company
+        )
+        self.logger.debug(
+            "Request: {request}, Headers: {headers}".format(
+                request=r, headers=self.headers
+            )
+        )
+        r = requests.post(
+            r, auth=(self.key, self.secret), headers=self.headers, data=json.dumps(data)
+        )
         assert r.ok, "Invalid response. Statuscode {}".format(r.status_code)
         return r
 
     def delete(self, entity):
         assert entity
-        r = "https://{company}.addepar.com/api/v1/entities/{entity}".format(company=self.company, entity=entity)
+        r = "https://{company}.addepar.com/api/v1/entities/{entity}".format(
+            company=self.company, entity=entity
+        )
         return requests.delete(r, auth=(self.key, self.secret), headers=self.headers)
 
     @property
     def version(self):
         return self.get("/v1/api_version").json()
 
-    def view_csv(self, view_id, portfolio_id, portfolio_type, start_date=pd.Timestamp("today"),
-                 end_date=pd.Timestamp("today")):
-
+    def view_csv(
+        self,
+        view_id,
+        portfolio_id,
+        portfolio_type,
+        start_date=pd.Timestamp("today"),
+        end_date=pd.Timestamp("today"),
+    ):
         assert isinstance(portfolio_type, PortfolioType)
 
-        param = AddeparRequest.dicturl({"portfolio_id": portfolio_id, "portfolio_type": portfolio_type.value,
-                                 "output_type": OutputType.CSV.value, "start_date": start_date.strftime("%Y-%m-%d"),
-                                 "end_date": end_date.strftime("%Y-%m-%d"), "addepar_firm": self.id})
-
-        request = "/v1/portfolio/views/{view}/results?{param}".format(view=view_id, param=param)
+        param = AddeparRequest.dicturl(
+            {
+                "portfolio_id": portfolio_id,
+                "portfolio_type": portfolio_type.value,
+                "output_type": OutputType.CSV.value,
+                "start_date": start_date.strftime("%Y-%m-%d"),
+                "end_date": end_date.strftime("%Y-%m-%d"),
+                "addepar_firm": self.id,
+            }
+        )
+
+        request = "/v1/portfolio/views/{view}/results?{param}".format(
+            view=view_id, param=param
+        )
 
         self.logger.debug("Request: {request}".format(request=request))
         return pd.read_csv(io.BytesIO(self.get(request=request).content))
 
-    def transaction_csv(self, view_id, portfolio_id, portfolio_type, start_date=pd.Timestamp("today"),
-                        end_date=pd.Timestamp("today")):
-
+    def transaction_csv(
+        self,
+        view_id,
+        portfolio_id,
+        portfolio_type,
+        start_date=pd.Timestamp("today"),
+        end_date=pd.Timestamp("today"),
+    ):
         assert isinstance(portfolio_type, PortfolioType)
 
-        param = AddeparRequest.dicturl({"portfolio_id": portfolio_id, "portfolio_type": portfolio_type.value,
-                                 "output_type": OutputType.CSV.value, "start_date": start_date.strftime("%Y-%m-%d"),
-                                 "end_date": end_date.strftime("%Y-%m-%d"), "addepar_firm": self.id})
-
-        request = "/v1/transactions/views/{view}/results?{param}".format(view=view_id, param=param)
+        param = AddeparRequest.dicturl(
+            {
+                "portfolio_id": portfolio_id,
+                "portfolio_type": portfolio_type.value,
+                "output_type": OutputType.CSV.value,
+                "start_date": start_date.strftime("%Y-%m-%d"),
+                "end_date": end_date.strftime("%Y-%m-%d"),
+                "addepar_firm": self.id,
+            }
+        )
+
+        request = "/v1/transactions/views/{view}/results?{param}".format(
+            view=view_id, param=param
+        )
 
         self.logger.debug("Request: {request}".format(request=request))
         return pd.read_csv(io.BytesIO(self.get(request=request).content))
 
     def entities(self, link="/v1/entities", modeltype=None):
         while link:
             a = self.get(link).json()
@@ -115,24 +170,32 @@
         return self.entities(link="/v1/users")
 
     @property
     def groups(self):
         return self.entities(link="/v1/groups")
 
     def group(self, id):
-        return AttrDict(self.get("/v1/groups/{id}".format(id=id)).json()["data"]["attributes"])
+        return AttrDict(
+            self.get("/v1/groups/{id}".format(id=id)).json()["data"]["attributes"]
+        )
 
     def user(self, id):
-        return AttrDict(self.get("/v1/users/{id}".format(id=id)).json()["data"]["attributes"])
+        return AttrDict(
+            self.get("/v1/users/{id}".format(id=id)).json()["data"]["attributes"]
+        )
 
     def entity(self, id):
-        return AttrDict(self.get("/v1/entities/{id}".format(id=id)).json()["data"]["attributes"])
+        return AttrDict(
+            self.get("/v1/entities/{id}".format(id=id)).json()["data"]["attributes"]
+        )
 
     def members(self, id):
-        for row in self.get("/v1/groups/{id}/relationships/members".format(id=id)).json()["data"]:
+        for row in self.get(
+            "/v1/groups/{id}/relationships/members".format(id=id)
+        ).json()["data"]:
             yield row["id"]
 
     @property
     def persons(self):
         return self.entities(link="/v1/entities", modeltype="PERSON_NODE")
 
     @property
```

### Comparing `pyaddepar-0.6.2/pyaddepar/flask_addepar.py` & `pyaddepar-0.7.0/pyaddepar/flask_addepar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from flask import Flask, current_app
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+from flask import current_app
+from flask import Flask
+
 from pyaddepar.addeparrequest import AddeparRequest
 
 
 class InvalidSettingsError(Exception):
     pass
 
 
@@ -12,56 +17,56 @@
     def __init__(self, app=None, config=None):
         self.app = None
         if app is not None:
             self.init_app(app, config)
 
     def init_app(self, app, config=None):
         if not app or not isinstance(app, Flask):
-            raise Exception('Invalid Flask application instance')
+            raise Exception("Invalid Flask application instance")
 
         self.app = app
 
-        app.extensions = getattr(app, 'extensions', {})
+        app.extensions = getattr(app, "extensions", {})
 
-        if 'addepar' not in app.extensions:
-            app.extensions['addepar'] = {}
+        if "addepar" not in app.extensions:
+            app.extensions["addepar"] = {}
 
-        if self in app.extensions['addepar']:
+        if self in app.extensions["addepar"]:
             # Raise an exception if extension already initialized as
             # potentially new configuration would not be loaded.
-            raise Exception('Extension already initialized')
+            raise Exception("Extension already initialized")
 
         if not config:
             # If not passed a config then we read the connection settings
             # from the app config.
             config = app.config
 
         # Obtain db connection(s)
         requests = create_requests(config)
 
         # Store objects in application instance so that multiple apps do not
         # end up accessing the same objects.
-        s = {'app': app, 'request': requests}
-        app.extensions['addepar'][self] = s
+        s = {"app": app, "request": requests}
+        app.extensions["addepar"][self] = s
 
     @property
     def request(self):
         """
         Return Addepar request associated with this Addepar instance.
         """
-        return current_app.extensions['addepar'][self]['request']
+        return current_app.extensions["addepar"][self]["request"]
 
 
 def create_requests(config):
     """
     Given Flask application's config dict, extract relevant config vars
     out of it and establish MongoEngine connection(s) based on them.
     """
     # Validate that the config is a dict
     if config is None or not isinstance(config, dict):
-        raise InvalidSettingsError('Invalid application configuration')
+        raise InvalidSettingsError("Invalid application configuration")
 
     # Return a single connection
     return AddeparRequest(**config["ADDEPAR"])
 
 
 addepar = Addepar()
```

