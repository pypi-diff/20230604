# Comparing `tmp/django_shopify_app-1.1.4.tar.gz` & `tmp/django_shopify_app-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_shopify_app-1.1.4.tar", last modified: Wed May 10 03:54:45 2023, max compression
+gzip compressed data, was "django_shopify_app-1.1.5.tar", last modified: Sun Jun  4 05:27:25 2023, max compression
```

## Comparing `django_shopify_app-1.1.4.tar` & `django_shopify_app-1.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.178917 django_shopify_app-1.1.4/django_shopify_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-10 03:54:45.000000 django_shopify_app-1.1.4/django_shopify_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-10 03:54:45.000000 django_shopify_app-1.1.4/django_shopify_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:54:45.000000 django_shopify_app-1.1.4/django_shopify_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 03:54:45.000000 django_shopify_app-1.1.4/django_shopify_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 03:54:45.000000 django_shopify_app-1.1.4/django_shopify_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/management/commands/run_shopify_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/management/commands/update_shop_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/services/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/templates/shopify_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/templates/shopify_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/templates/shopify_app/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.688447 django_shopify_app-1.1.5/django_shopify_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-04 05:27:25.000000 django_shopify_app-1.1.5/django_shopify_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-04 05:27:25.000000 django_shopify_app-1.1.5/django_shopify_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 05:27:25.000000 django_shopify_app-1.1.5/django_shopify_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-04 05:27:25.000000 django_shopify_app-1.1.5/django_shopify_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 05:27:25.000000 django_shopify_app-1.1.5/django_shopify_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.688447 django_shopify_app-1.1.5/shopify_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.688447 django_shopify_app-1.1.5/shopify_app/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.688447 django_shopify_app-1.1.5/shopify_app/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/management/commands/run_shopify_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/management/commands/update_shop_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.688447 django_shopify_app-1.1.5/shopify_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/shopify_app/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/services/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/shopify_app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/shopify_app/templates/shopify_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/templates/shopify_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/templates/shopify_app/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/shopify_app/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:27:25.692447 django_shopify_app-1.1.5/shopify_app/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-04 05:27:16.000000 django_shopify_app-1.1.5/shopify_app/views.py
```

### Comparing `django_shopify_app-1.1.4/PKG-INFO` & `django_shopify_app-1.1.5/django_shopify_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_shopify_app
-Version: 1.1.4
+Name: django-shopify-app
+Version: 1.1.5
 Summary: A django app with all the tools required to make a Shopify app
 Home-page: http://pypi.python.org/pypi/django_shopify_app/
 Author: Moship
 Author-email: hello@moship.io
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `django_shopify_app-1.1.4/README.md` & `django_shopify_app-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.4/django_shopify_app.egg-info/PKG-INFO` & `django_shopify_app-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-shopify-app
-Version: 1.1.4
+Name: django_shopify_app
+Version: 1.1.5
 Summary: A django app with all the tools required to make a Shopify app
 Home-page: http://pypi.python.org/pypi/django_shopify_app/
 Author: Moship
 Author-email: hello@moship.io
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `django_shopify_app-1.1.4/django_shopify_app.egg-info/SOURCES.txt` & `django_shopify_app-1.1.5/django_shopify_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.4/setup.py` & `django_shopify_app-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='django_shopify_app',
-    version='1.1.4',
+    version='1.1.5',
     author='Moship',
     author_email='hello@moship.io',
     packages=find_packages(),
     scripts=[],
     url='http://pypi.python.org/pypi/django_shopify_app/',
     license="MIT",
     description='A django app with all the tools required to make a Shopify app',
```

### Comparing `django_shopify_app-1.1.4/shopify_app/apps.py` & `django_shopify_app-1.1.5/shopify_app/apps.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.4/shopify_app/decorators.py` & `django_shopify_app-1.1.5/shopify_app/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,16 @@
 
 def latest_access_scopes_required(func):
     def wrapper(*args, **kwargs):
         shop = kwargs.get("shop")
 
         try:
             configured_access_scopes = apps.get_app_config(
-                "shopify_app").SHOPIFY_API_SCOPES
+                "shopify_app"
+            ).SHOPIFY_API_SCOPES
             current_access_scopes = shop.access_scopes
 
             assert ApiAccess(configured_access_scopes) == ApiAccess(
                 current_access_scopes)
         except:
             kwargs["scope_changes_required"] = True
```

### Comparing `django_shopify_app-1.1.4/shopify_app/management/commands/run_shopify_pubsub.py` & `django_shopify_app-1.1.5/shopify_app/management/commands/run_shopify_pubsub.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.4/shopify_app/management/commands/update_shop_webhooks.py` & `django_shopify_app-1.1.5/shopify_app/management/commands/update_shop_webhooks.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.4/shopify_app/models.py` & `django_shopify_app-1.1.5/shopify_app/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,9 +53,12 @@
         return result
 
     @cached_property
     def host(self):
         admin_url = f'{self.shopify_domain}/admin'
         return base64.b64encode(admin_url.encode()).decode()
 
+    def on_user_login(self, user_data):
+        print(user_data)
+
     class Meta:
         abstract = True
```

### Comparing `django_shopify_app-1.1.4/shopify_app/services/webhooks.py` & `django_shopify_app-1.1.5/shopify_app/services/webhooks.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.4/shopify_app/templates/shopify_app/index.html` & `django_shopify_app-1.1.5/shopify_app/templates/shopify_app/index.html`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.4/shopify_app/urls.py` & `django_shopify_app-1.1.5/shopify_app/urls.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.4/shopify_app/utils/__init__.py` & `django_shopify_app-1.1.5/shopify_app/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.4/shopify_app/views.py` & `django_shopify_app-1.1.5/shopify_app/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+
 import json
+import requests
+
 from django.views import View
 from django.urls import reverse
 from django.conf import settings
-from django.shortcuts import redirect, render
+from django.shortcuts import redirect, render, HttpResponse
 from django.views.decorators.clickjacking import xframe_options_exempt
 from django.utils.decorators import method_decorator
 
 from rest_framework.views import APIView
 from rest_framework.response import Response
 from rest_framework.exceptions import APIException
 
@@ -18,85 +21,126 @@
 )
 from .decorators import shopify_embed
 
 
 class ShopAPIView(APIView):
     pass
 
+def create_permission_url(shop_url, redirect_path='', redirect_path_name=''):
+
+    shopify.Session.setup(
+        api_key=settings.SHOPIFY_API_KEY,
+        secret=settings.SHOPIFY_API_SECRET
+    )
+
+    api_version = '2022-07'
+    state = ''
+
+    if redirect_path_name:
+        path = reverse(redirect_path_name)
+    elif redirect_path:
+        path = redirect_path
+
+    redirect_uri = f"{settings.SHOPIFY_APP_HOST}{path}"
+    scopes = settings.SHOPIFY_APP_SCOPES
+
+    newSession = shopify.Session(shop_url, api_version)
+    auth_url = newSession.create_permission_url(
+        scopes, redirect_uri, state
+    )
+    return auth_url
 
 class InitTokenRequestView(View):
 
     redirect_path_name = ''
 
     @method_decorator(xframe_options_exempt)
     @method_decorator(shopify_embed)
     def get(self, request, *args, **kwargs):
 
-        shopify.Session.setup(
-            api_key=settings.SHOPIFY_API_KEY,
-            secret=settings.SHOPIFY_API_SECRET
-        )
-
         shop_url = request.GET.get('shop')
-        api_version = '2022-07'
-        state = ''
-        path = reverse(self.redirect_path_name)
-        redirect_uri = f"{settings.SHOPIFY_APP_HOST}{path}"
-        scopes = settings.SHOPIFY_APP_SCOPES
-
-        newSession = shopify.Session(shop_url, api_version)
-        auth_url = newSession.create_permission_url(
-            scopes, redirect_uri, state
+        auth_url = create_permission_url(
+            shop_url, redirect_path_name=self.redirect_path_name
         )
 
         if request.GET.get('embedded'):
             context = {
                 'api_key': settings.SHOPIFY_API_KEY,
                 'host': request.GET.get('host'),
                 'redirect': auth_url
             }
             return render(request, 'shopify_app/index.html', context=context)
         else:
             return redirect(auth_url)
 
 
+def request_personal_access_token(
+        shop, client_id, client_secret, authorization_code
+):
+
+    response = requests.post(
+        (
+        f'https://{shop}/admin/oauth/access_token'
+        f'?client_id={client_id}&client_secret={client_secret}&'
+        f'code={authorization_code}'
+        )
+    )
+    if response.status_code != 200:
+        raise Exception('Could not request access token')
+
+    return response.json()
+
+
 class EndTokenRequestView(View):
     redirect_path_name = ''
 
     def get(self, request, *args, **kwargs):
 
         shop_url = request.GET.get('shop')
 
         shopify.Session.setup(
             api_key=settings.SHOPIFY_API_KEY,
             secret=settings.SHOPIFY_API_SECRET
         )
 
-        session = shopify.Session(shop_url, '2022-07')
+        if not shopify.Session.validate_params(request.GET.dict()):
+            raise Exception('Invalid HMAC: Possibly malicious login')
 
-        access_token = session.request_token(request.GET.dict())
+        data = request_personal_access_token(
+            shop_url, settings.SHOPIFY_API_KEY, settings.SHOPIFY_API_SECRET,
+            request.GET.get('code')
+        )
 
         Shop = get_shop_model()
-        shop_record = Shop.objects.get_or_create(shopify_domain=session.url)[0]
+        shop_record = Shop.objects.get_or_create(shopify_domain=shop_url)[0]
+
+        if data.get('associated_user'):
+
+            shop_record.on_user_login(data['associated_user'])
+
+            host = settings.SHOPIFY_APP_HOST
+            path = reverse(self.redirect_path_name)
+            query = request.META['QUERY_STRING']
+
+            return redirect(f"{host}{path}?{query}")
+        else:
+            access_token = data.pop('access_token')
 
         installed = bool(not shop_record.shopify_token and access_token)
 
         shop_record.shopify_token = access_token
-        shop_record.access_scopes = session.access_scopes
+        shop_record.access_scopes = data['scope']
 
         shop_record.save()
 
         if installed:
             shop_record.installed()
 
-        host = settings.SHOPIFY_APP_HOST
-        path = reverse(self.redirect_path_name)
-        query = request.META['QUERY_STRING']
-
-        return redirect(f"{host}{path}?{query}")
+        auth_url = create_permission_url(shop_url, redirect_path=request.path)
+        return redirect(f"{auth_url}&grant_options[]=per-user")
 
 
 class WebhookAuthenticationFailed(APIException):
     status_code = 401
     default_detail = 'authentication failed'
```

