# Comparing `tmp/django-oasis4-certs-1.0.1b1.tar.gz` & `tmp/django-oasis4-certs-1.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oasis4-certs-1.0.1b1.tar", last modified: Thu Mar 16 22:48:08 2023, max compression
+gzip compressed data, was "django-oasis4-certs-1.0.2b0.tar", last modified: Sat Jun  3 22:26:25 2023, max compression
```

## Comparing `django-oasis4-certs-1.0.1b1.tar` & `django-oasis4-certs-1.0.2b0.tar`

### file list

```diff
@@ -1,85 +1,13 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.373313 django-oasis4-certs-1.0.1b1/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-certs-1.0.1b1/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      144 2023-02-10 23:54:38.000000 django-oasis4-certs-1.0.1b1/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13728 2023-03-16 22:48:08.373313 django-oasis4-certs-1.0.1b1/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      844 2023-02-16 15:46:38.000000 django-oasis4-certs-1.0.1b1/README.md
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.360314 django-oasis4-certs-1.0.1b1/django_oasis4_certs.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13728 2023-03-16 22:48:08.000000 django-oasis4-certs-1.0.1b1/django_oasis4_certs.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     2767 2023-03-16 22:48:08.000000 django-oasis4-certs-1.0.1b1/django_oasis4_certs.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-03-16 22:48:08.000000 django-oasis4-certs-1.0.1b1/django_oasis4_certs.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       89 2023-03-16 22:48:08.000000 django-oasis4-certs-1.0.1b1/django_oasis4_certs.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       12 2023-03-16 22:48:08.000000 django-oasis4-certs-1.0.1b1/django_oasis4_certs.egg-info/top_level.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.361313 django-oasis4-certs-1.0.1b1/oasis_certs/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2023-01-24 22:31:04.000000 django-oasis4-certs-1.0.1b1/oasis_certs/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      681 2023-02-02 02:09:16.000000 django-oasis4-certs-1.0.1b1/oasis_certs/admin.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1067 2023-02-08 13:56:31.000000 django-oasis4-certs-1.0.1b1/oasis_certs/admin_views.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.362314 django-oasis4-certs-1.0.1b1/oasis_certs/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2023-01-27 02:43:18.000000 django-oasis4-certs-1.0.1b1/oasis_certs/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.362314 django-oasis4-certs-1.0.1b1/oasis_certs/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      554 2023-02-07 19:33:56.000000 django-oasis4-certs-1.0.1b1/oasis_certs/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      753 2023-02-07 19:55:47.000000 django-oasis4-certs-1.0.1b1/oasis_certs/api/serializers/certificate.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.363314 django-oasis4-certs-1.0.1b1/oasis_certs/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      592 2023-02-07 09:02:13.000000 django-oasis4-certs-1.0.1b1/oasis_certs/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11664 2023-03-16 22:27:48.000000 django-oasis4-certs-1.0.1b1/oasis_certs/api/services/oasis_certs.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2410 2023-02-07 10:42:04.000000 django-oasis4-certs-1.0.1b1/oasis_certs/api/services/oasis_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1048 2023-02-13 14:05:54.000000 django-oasis4-certs-1.0.1b1/oasis_certs/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.363314 django-oasis4-certs-1.0.1b1/oasis_certs/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      504 2023-02-02 11:23:06.000000 django-oasis4-certs-1.0.1b1/oasis_certs/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.363314 django-oasis4-certs-1.0.1b1/oasis_certs/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      616 2023-02-07 19:00:11.000000 django-oasis4-certs-1.0.1b1/oasis_certs/lib/choices/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      812 2023-02-07 20:39:46.000000 django-oasis4-certs-1.0.1b1/oasis_certs/lib/choices/category.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      829 2023-02-07 23:22:02.000000 django-oasis4-certs-1.0.1b1/oasis_certs/lib/choices/cycle_type.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.363314 django-oasis4-certs-1.0.1b1/oasis_certs/lib/cursors/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      562 2023-02-07 10:59:32.000000 django-oasis4-certs-1.0.1b1/oasis_certs/lib/cursors/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1995 2023-02-07 10:59:45.000000 django-oasis4-certs-1.0.1b1/oasis_certs/lib/cursors/cursor.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.364313 django-oasis4-certs-1.0.1b1/oasis_certs/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      575 2023-02-02 11:24:04.000000 django-oasis4-certs-1.0.1b1/oasis_certs/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      735 2023-02-07 23:42:22.000000 django-oasis4-certs-1.0.1b1/oasis_certs/lib/managers/certificate.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.358314 django-oasis4-certs-1.0.1b1/oasis_certs/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.358314 django-oasis4-certs-1.0.1b1/oasis_certs/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.364313 django-oasis4-certs-1.0.1b1/oasis_certs/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     7606 2023-02-16 15:33:25.000000 django-oasis4-certs-1.0.1b1/oasis_certs/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    15466 2023-02-16 15:33:20.000000 django-oasis4-certs-1.0.1b1/oasis_certs/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.367313 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1572 2023-02-02 02:00:20.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      334 2023-02-02 02:04:48.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0002_rename_certificates_certificate.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1906 2023-02-03 02:19:04.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0003_alter_certificate_options_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      500 2023-02-07 00:50:29.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0004_certificate_period_type.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      936 2023-02-07 01:10:28.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0005_remove_certificate_period_type_certificate_closed_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      415 2023-02-07 01:20:24.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0006_rename_legend_certificate_body_text.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      786 2023-02-07 19:19:14.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0007_remove_certificate_unq_certificates_key_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      899 2023-02-07 23:13:15.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0008_certificate_customer_type_alter_certificate_category.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      874 2023-02-08 13:59:03.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0009_certificate_signed_alter_certificate_cycle_type.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      521 2023-02-08 14:47:02.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0010_alter_certificate_footer_text.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1409 2023-03-16 22:19:18.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0011_certificatefile.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      554 2023-03-16 22:44:49.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/0012_alter_certificatefile_period_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2023-02-02 02:00:20.000000 django-oasis4-certs-1.0.1b1/oasis_certs/migrations/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4041 2023-03-16 22:44:32.000000 django-oasis4-certs-1.0.1b1/oasis_certs/models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.358314 django-oasis4-certs-1.0.1b1/oasis_certs/static/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.358314 django-oasis4-certs-1.0.1b1/oasis_certs/static/oasis_certs/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.367313 django-oasis4-certs-1.0.1b1/oasis_certs/static/oasis_certs/css/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      899 2023-02-26 20:01:22.000000 django-oasis4-certs-1.0.1b1/oasis_certs/static/oasis_certs/css/certs_base_style.css
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      511 2023-02-08 19:42:40.000000 django-oasis4-certs-1.0.1b1/oasis_certs/static/oasis_certs/css/certs_cells.css
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.368313 django-oasis4-certs-1.0.1b1/oasis_certs/static/oasis_certs/img/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)   552396 2022-05-23 14:06:34.000000 django-oasis4-certs-1.0.1b1/oasis_certs/static/oasis_certs/img/logo.png
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.359314 django-oasis4-certs-1.0.1b1/oasis_certs/templates/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.369313 django-oasis4-certs-1.0.1b1/oasis_certs/templates/mail/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      495 2023-03-01 21:00:33.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/mail/send_certificate.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.371313 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4221 2023-02-08 14:59:33.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/certs_base_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2618 2023-02-08 16:28:31.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/coffee_sales_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      528 2023-02-09 13:59:02.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/contribution_balance_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5330 2023-02-09 20:28:31.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/credits_statement_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2708 2023-02-08 15:31:15.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/farms_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5958 2023-02-09 16:54:11.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/future_contracts_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3352 2023-02-08 01:20:28.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/hability_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      517 2023-02-08 19:40:55.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/purchase_inputs_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3543 2023-02-16 15:38:51.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/wh_icr_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2965 2023-02-08 13:30:31.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/wh_ivr_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2805 2023-02-07 10:55:36.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templates/oasis_certs/wh_source_template.html
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-16 22:48:08.372313 django-oasis4-certs-1.0.1b1/oasis_certs/templatetags/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-08 00:10:11.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templatetags/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      744 2023-02-08 00:28:53.000000 django-oasis4-certs-1.0.1b1/oasis_certs/templatetags/define_able.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1113 2023-02-13 14:05:54.000000 django-oasis4-certs-1.0.1b1/oasis_certs/urls.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      910 2023-03-16 22:46:54.000000 django-oasis4-certs-1.0.1b1/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-03-16 22:48:08.373313 django-oasis4-certs-1.0.1b1/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:26:25.745976 django-oasis4-certs-1.0.2b0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-certs-1.0.2b0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      144 2023-02-10 23:54:38.000000 django-oasis4-certs-1.0.2b0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    13741 2023-06-03 22:26:25.745976 django-oasis4-certs-1.0.2b0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      844 2023-02-16 15:46:38.000000 django-oasis4-certs-1.0.2b0/README.md
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:26:25.745976 django-oasis4-certs-1.0.2b0/django_oasis4_certs.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    13741 2023-06-03 22:26:25.000000 django-oasis4-certs-1.0.2b0/django_oasis4_certs.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)      258 2023-06-03 22:26:25.000000 django-oasis4-certs-1.0.2b0/django_oasis4_certs.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-03 22:26:25.000000 django-oasis4-certs-1.0.2b0/django_oasis4_certs.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       89 2023-06-03 22:26:25.000000 django-oasis4-certs-1.0.2b0/django_oasis4_certs.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-03 22:26:25.000000 django-oasis4-certs-1.0.2b0/django_oasis4_certs.egg-info/top_level.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      923 2023-06-03 22:15:47.000000 django-oasis4-certs-1.0.2b0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-03 22:26:25.745976 django-oasis4-certs-1.0.2b0/setup.cfg
```

### Comparing `django-oasis4-certs-1.0.1b1/LICENSE` & `django-oasis4-certs-1.0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oasis4-certs-1.0.1b1/PKG-INFO` & `django-oasis4-certs-1.0.2b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4-certs
-Version: 1.0.1b1
+Version: 1.0.2b0
 Summary: Certificate generator for Django from OASIS4©
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
         
@@ -110,15 +110,15 @@
         IDIOMA; TRADUCCIONES. En el caso de que la versión en español de este Contrato esté acompañada por cualquier otra
         versión traducida a otro idioma, dicha versión traducida sólo se ofrece a título informativo y prevalecerá la versión
         en español.
         
 Keywords: django,zibanu,library
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `django-oasis4-certs-1.0.1b1/README.md` & `django-oasis4-certs-1.0.2b0/README.md`

 * *Files identical despite different names*

### Comparing `django-oasis4-certs-1.0.1b1/django_oasis4_certs.egg-info/PKG-INFO` & `django-oasis4-certs-1.0.2b0/django_oasis4_certs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4-certs
-Version: 1.0.1b1
+Version: 1.0.2b0
 Summary: Certificate generator for Django from OASIS4©
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
         
@@ -110,15 +110,15 @@
         IDIOMA; TRADUCCIONES. En el caso de que la versión en español de este Contrato esté acompañada por cualquier otra
         versión traducida a otro idioma, dicha versión traducida sólo se ofrece a título informativo y prevalecerá la versión
         en español.
         
 Keywords: django,zibanu,library
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `django-oasis4-certs-1.0.1b1/pyproject.toml` & `django-oasis4-certs-1.0.2b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,26 +3,26 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "django-oasis4-certs"
-version = "1.0.1-beta.1"
+version = "1.0.2-beta.0"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "Certificate generator for Django from OASIS4©"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     "License :: Other/Proprietary License",
     "Programming Language :: Python :: 3.9",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Framework :: Django",
     "Framework :: Django :: 4.1",
     "Environment :: Web Environment",
     "Operating System :: OS Independent",
     "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
```

