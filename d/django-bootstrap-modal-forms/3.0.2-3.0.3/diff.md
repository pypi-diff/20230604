# Comparing `tmp/django-bootstrap-modal-forms-3.0.2.tar.gz` & `tmp/django-bootstrap-modal-forms-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bootstrap-modal-forms-3.0.2.tar", last modified: Tue May  2 17:50:42 2023, max compression
+gzip compressed data, was "django-bootstrap-modal-forms-3.0.3.tar", last modified: Sun Jun  4 16:54:03 2023, max compression
```

## Comparing `django-bootstrap-modal-forms-3.0.2.tar` & `django-bootstrap-modal-forms-3.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:42.802849 django-bootstrap-modal-forms-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    37063 2023-05-02 17:50:42.802849 django-bootstrap-modal-forms-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36236 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:42.798849 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:42.798849 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:42.798849 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:42.798849 django-bootstrap-modal-forms-3.0.2/django_bootstrap_modal_forms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37063 2023-05-02 17:50:42.000000 django-bootstrap-modal-forms-3.0.2/django_bootstrap_modal_forms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-02 17:50:42.000000 django-bootstrap-modal-forms-3.0.2/django_bootstrap_modal_forms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:50:42.000000 django-bootstrap-modal-forms-3.0.2/django_bootstrap_modal_forms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 17:50:42.000000 django-bootstrap-modal-forms-3.0.2/django_bootstrap_modal_forms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 17:50:42.000000 django-bootstrap-modal-forms-3.0.2/django_bootstrap_modal_forms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:42.802849 django-bootstrap-modal-forms-3.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/examples/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/examples/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:42.802849 django-bootstrap-modal-forms-3.0.2/examples/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/examples/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/examples/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/examples/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/examples/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/examples/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:42.802849 django-bootstrap-modal-forms-3.0.2/setup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/setup/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/setup/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/setup/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:50:42.802849 django-bootstrap-modal-forms-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:42.802849 django-bootstrap-modal-forms-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/tests/tests_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-02 17:50:33.000000 django-bootstrap-modal-forms-3.0.2/tests/tests_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.455512 django-bootstrap-modal-forms-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    37063 2023-06-04 16:54:03.455512 django-bootstrap-modal-forms-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36236 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.447512 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.439513 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.447512 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.447512 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37063 2023-06-04 16:54:03.000000 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 16:54:03.000000 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:54:03.000000 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 16:54:03.000000 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 16:54:03.000000 django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.451512 django-bootstrap-modal-forms-3.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.451512 django-bootstrap-modal-forms-3.0.3/examples/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/examples/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.451512 django-bootstrap-modal-forms-3.0.3/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/setup/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/setup/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/setup/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 16:54:03.455512 django-bootstrap-modal-forms-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:54:03.451512 django-bootstrap-modal-forms-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/tests/tests_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-04 16:53:54.000000 django-bootstrap-modal-forms-3.0.3/tests/tests_unit.py
```

### Comparing `django-bootstrap-modal-forms-3.0.2/CHANGELOG.rst` & `django-bootstrap-modal-forms-3.0.3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/LICENSE.txt` & `django-bootstrap-modal-forms-3.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/PKG-INFO` & `django-bootstrap-modal-forms-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap-modal-forms
-Version: 3.0.2
+Version: 3.0.3
 Summary: A Django plugin for creating AJAX driven forms in Bootstrap modal.
 Home-page: https://github.com/trco/django-bootstrap-modal-forms
 Author: Uros Trstenjak
 Author-email: uros.trstenjak@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-bootstrap-modal-forms-3.0.2/README.rst` & `django-bootstrap-modal-forms-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/generic.py` & `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/generic.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/mixins.py` & `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/mixins.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,14 +74,18 @@
 
 
 class FormValidationMixin:
     """
     Generic View Mixin which saves object and redirects to success_url if request is not ajax request. Otherwise response 204 No content is returned.
     """
 
+    def get_success_message(self):
+        if hasattr(self, 'success_message'):
+            return self.success_message
+
     def get_success_url(self):
         if self.success_url:
             return self.success_url
         return super().get_success_url()
 
     def form_valid(self, form):
         isAjaxRequest = is_ajax(self.request.META)
@@ -89,13 +93,13 @@
 
         if isAjaxRequest:
             if asyncUpdate:
                 form.save()
             return HttpResponse(status=204)
 
         form.save()
-        messages.success(self.request, self.success_message)
+        messages.success(self.request, self.get_success_message())
         return HttpResponseRedirect(self.get_success_url())
 
 
 def is_ajax(meta):
     return 'HTTP_X_REQUESTED_WITH' in meta and meta['HTTP_X_REQUESTED_WITH'] == 'XMLHttpRequest'
```

### Comparing `django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js` & `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 django-bootstrap-modal-forms
-version : 3.0.2
+version : 3.0.3
 Copyright (c) 2023 Marcel Rupp
 */
 
 // Open modal & load the form at formURL to the modalContent element
 const modalFormCallback = function(settings) {
     let modal = document.querySelector(settings.modalID);
     let content = modal.querySelector(settings.modalContent);
```

### Comparing `django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js` & `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/bootstrap5.modal.forms.min.js`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js` & `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 django-bootstrap-modal-forms
-version : 3.0.2
+version : 3.0.3
 Copyright (c) 2023 Uroš Trstenjak
 https://github.com/trco/django-bootstrap-modal-forms
 */
 
 (function($) {
 
     // Open modal & load the form at formURL to the modalContent element
```

### Comparing `django-bootstrap-modal-forms-3.0.2/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js` & `django-bootstrap-modal-forms-3.0.3/bootstrap_modal_forms/static/js/jquery.bootstrap.modal.forms.min.js`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/django_bootstrap_modal_forms.egg-info/PKG-INFO` & `django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap-modal-forms
-Version: 3.0.2
+Version: 3.0.3
 Summary: A Django plugin for creating AJAX driven forms in Bootstrap modal.
 Home-page: https://github.com/trco/django-bootstrap-modal-forms
 Author: Uros Trstenjak
 Author-email: uros.trstenjak@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-bootstrap-modal-forms-3.0.2/django_bootstrap_modal_forms.egg-info/SOURCES.txt` & `django-bootstrap-modal-forms-3.0.3/django_bootstrap_modal_forms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/examples/forms.py` & `django-bootstrap-modal-forms-3.0.3/examples/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/examples/migrations/0001_initial.py` & `django-bootstrap-modal-forms-3.0.3/examples/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/examples/models.py` & `django-bootstrap-modal-forms-3.0.3/examples/models.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/examples/urls.py` & `django-bootstrap-modal-forms-3.0.3/examples/urls.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/examples/views.py` & `django-bootstrap-modal-forms-3.0.3/examples/views.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/setup/settings.py` & `django-bootstrap-modal-forms-3.0.3/setup/settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/setup.py` & `django-bootstrap-modal-forms-3.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     README = readme_file.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-bootstrap-modal-forms',
-    version='3.0.2',
+    version='3.0.3',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A Django plugin for creating AJAX driven forms in Bootstrap modal.',
     long_description=README,
     url='https://github.com/trco/django-bootstrap-modal-forms',
     author='Uros Trstenjak',
```

### Comparing `django-bootstrap-modal-forms-3.0.2/tests/base.py` & `django-bootstrap-modal-forms-3.0.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/tests/tests_functional.py` & `django-bootstrap-modal-forms-3.0.3/tests/tests_functional.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap-modal-forms-3.0.2/tests/tests_unit.py` & `django-bootstrap-modal-forms-3.0.3/tests/tests_unit.py`

 * *Files identical despite different names*

