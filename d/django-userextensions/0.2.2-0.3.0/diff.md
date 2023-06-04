# Comparing `tmp/django-userextensions-0.2.2.tar.gz` & `tmp/django-userextensions-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-userextensions-0.2.2.tar", last modified: Mon Feb 20 00:07:14 2023, max compression
+gzip compressed data, was "django-userextensions-0.3.0.tar", last modified: Sun Jun  4 01:04:06 2023, max compression
```

## Comparing `django-userextensions-0.2.2.tar` & `django-userextensions-0.3.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.420251 django-userextensions-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-02-20 00:07:14.420251 django-userextensions-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/django_userextensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-02-20 00:07:14.000000 django-userextensions-0.2.2/django_userextensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-02-20 00:07:14.000000 django-userextensions-0.2.2/django_userextensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 00:07:14.000000 django-userextensions-0.2.2/django_userextensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-20 00:07:14.000000 django-userextensions-0.2.2/django_userextensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-20 00:07:14.000000 django-userextensions-0.2.2/django_userextensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 00:07:14.420251 django-userextensions-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/userextensions/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/userextensions/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/userextensions/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/management/commands/add_service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/userextensions/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/migrations/0002_userpreference_start_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/migrations/0003_auto_20200117_2153.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/migrations/0005_auto_20201114_0548.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/migrations/0006_auto_20210507_1831.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/migrations/0007_auto_20220807_2104.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.412251 django-userextensions-0.2.2/userextensions/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/userextensions/templates/userextensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/userextensions/templates/userextensions/ajax/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/ajax/get_token_history_for_srv_acct.htm
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/ajax/get_users_per_group.htm
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/ajax/show_srv_acct_token.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/userextensions/templates/userextensions/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/custom/create_custom_service_account.htm
--rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/custom/manage_service_accounts.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/userextensions/templates/userextensions/detail/
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/detail/detail_user.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/userextensions/templates/userextensions/form/
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/form/edit_favorite.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.416251 django-userextensions-0.2.2/userextensions/templates/userextensions/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/snippets/user_theme.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.420251 django-userextensions-0.2.2/userextensions/templates/userextensions/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/table/table_favorites.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/table/table_recents.htm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templates/userextensions/userextensions_base.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.420251 django-userextensions-0.2.2/userextensions/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/templatetags/userextension_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:07:14.420251 django-userextensions-0.2.2/userextensions/views/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/views/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/views/ajax.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-02-20 00:06:57.000000 django-userextensions-0.2.2/userextensions/views/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.418177 django-userextensions-0.3.0/django_userextensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-04 01:04:06.000000 django-userextensions-0.3.0/django_userextensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-04 01:04:06.000000 django-userextensions-0.3.0/django_userextensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 01:04:06.000000 django-userextensions-0.3.0/django_userextensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-04 01:04:06.000000 django-userextensions-0.3.0/django_userextensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 01:04:06.000000 django-userextensions-0.3.0/django_userextensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.418177 django-userextensions-0.3.0/userextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/management/commands/add_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0002_userpreference_start_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0003_auto_20200117_2153.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0005_auto_20201114_0548.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0006_auto_20210507_1831.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0007_auto_20220807_2104.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.414177 django-userextensions-0.3.0/userextensions/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/templates/userextensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/templates/userextensions/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/ajax/get_token_history_for_srv_acct.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/ajax/get_users_per_group.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/ajax/show_srv_acct_token.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/templates/userextensions/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/custom/create_custom_service_account.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/custom/manage_service_accounts.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/templates/userextensions/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/detail/detail_user.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/templates/userextensions/form/
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/form/edit_favorite.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/templates/userextensions/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/snippets/user_theme.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/templates/userextensions/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/table/table_favorites.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/table/table_recents.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/userextensions_base.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templatetags/userextension_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/views/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/views/ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/views/gui.py
```

### Comparing `django-userextensions-0.2.2/LICENSE` & `django-userextensions-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/PKG-INFO` & `django-userextensions-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-userextensions
-Version: 0.2.2
+Version: 0.3.0
 Summary: A user extension module for django
 Home-page: https://github.com/davidslusser/django-userextensions
-Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.2.2.tar.gz
+Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.3.0.tar.gz
 Author: David Slusser
 Author-email: dbslusser@gmail.com
 License: GPL-3.0
 Keywords: django,helpers,extension,user,profile
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `django-userextensions-0.2.2/README.md` & `django-userextensions-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/django_userextensions.egg-info/PKG-INFO` & `django-userextensions-0.3.0/django_userextensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-userextensions
-Version: 0.2.2
+Version: 0.3.0
 Summary: A user extension module for django
 Home-page: https://github.com/davidslusser/django-userextensions
-Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.2.2.tar.gz
+Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.3.0.tar.gz
 Author: David Slusser
 Author-email: dbslusser@gmail.com
 License: GPL-3.0
 Keywords: django,helpers,extension,user,profile
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `django-userextensions-0.2.2/django_userextensions.egg-info/SOURCES.txt` & `django-userextensions-0.3.0/django_userextensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/setup.py` & `django-userextensions-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/admin.py` & `django-userextensions-0.3.0/userextensions/admin.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/forms.py` & `django-userextensions-0.3.0/userextensions/forms.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/management/commands/add_service_account.py` & `django-userextensions-0.3.0/userextensions/management/commands/add_service_account.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/middleware.py` & `django-userextensions-0.3.0/userextensions/middleware.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/migrations/0001_initial.py` & `django-userextensions-0.3.0/userextensions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/migrations/0003_auto_20200117_2153.py` & `django-userextensions-0.3.0/userextensions/migrations/0003_auto_20200117_2153.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py` & `django-userextensions-0.3.0/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/migrations/0005_auto_20201114_0548.py` & `django-userextensions-0.3.0/userextensions/migrations/0005_auto_20201114_0548.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/migrations/0006_auto_20210507_1831.py` & `django-userextensions-0.3.0/userextensions/migrations/0006_auto_20210507_1831.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/migrations/0007_auto_20220807_2104.py` & `django-userextensions-0.3.0/userextensions/migrations/0007_auto_20220807_2104.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/mixins.py` & `django-userextensions-0.3.0/userextensions/mixins.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/models.py` & `django-userextensions-0.3.0/userextensions/models.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/signals.py` & `django-userextensions-0.3.0/userextensions/signals.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/templates/userextensions/custom/create_custom_service_account.htm` & `django-userextensions-0.3.0/userextensions/templates/userextensions/custom/create_custom_service_account.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/templates/userextensions/custom/manage_service_accounts.html` & `django-userextensions-0.3.0/userextensions/templates/userextensions/custom/manage_service_accounts.html`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% load static %}
 
 {% block local_head %}
 {% include 'handyhelpers/component/clipboard.htm' %}
 {% endblock local_head %}
 
 {% block content %}
-<div class="container-fluid mb-5 animated fadeIn">
+<div class="container-fluid my-5 animated fadeIn">
     <h1 class="text-primary"><b>Manage Service Accounts: </b></h1>
 </div>
 <div>&nbsp;</div>
 <div class="container-fluid pl-5 pr-5">
     <div class="row mb-5 animated fadeIn" style="animation-delay: .25s;">
         <div class="col-sm-12 col-md-3 col-lg-2 mb-3 pl-0">
             <i class="fas fa-users-cog fa-6x text-primary"></i><br/>
@@ -29,77 +29,77 @@
                             <th class="bg-transparent text-secondary">Admin Enabled</th>
                             <th class="bg-transparent text-secondary">Actions</th>
                         </tr>
                     </thead>
                     <tbody>
                     {% for row in service_accounts %}
                     <tr class="border-top border-secondary">
-                        <td><span class="ml-1">{{ row.user }}</span></td>
-                        <td><span class="ml-1">{{ row.group }}</span></td>
+                        <td><span class="mx-1">{{ row.user }}</span></td>
+                        <td><span class="mx-1">{{ row.group }}</span></td>
                         <td>
                             {% if row.enabled %}
-                            <span class="text-primary ml-1"><i class="fas fa-check"></i></span>
+                            <span class="text-primary mx-2"><i class="fas fa-check"></i></span>
                             {% else %}
-                            <span class="text-danger ml-1"><i class="fas fa-times"></i></span>
+                            <span class="text-danger mx-2"><i class="fas fa-times"></i></span>
                             {% endif %}
                         </td>
                         <td>
                             {% if row.admin_enabled %}
-                            <span class="text-primary ml-1"><i class="fas fa-check"></i></span>
+                            <span class="text-primary mx-2"><i class="fas fa-check"></i></span>
                             {% else %}
-                            <span class="text-danger ml-1"><i class="fas fa-times"></i></span>
+                            <span class="text-danger mx-2"><i class="fas fa-times"></i></span>
                             {% endif %}
                         </td>
                         <td>
                             <!-- view api token -->
                             <a href="#" title="view api token" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="showInfo('{% url "userextensions:show_srv_acct_token" %}', '{{ row.user.auth_token }}', 'API Token: <small><i>{{ row.user.username }}</i></small>', 'lg');">
-                                <i class="fas fa-key ml-1 mr-1"></i>
+                                <i class="fas fa-key mx-2"></i>
                             </a>
 
                             <!-- refresh api token -->
                             <a href="#" title="refresh api token" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="confirmAction('{% url "userextensions:refresh_srv_acct_token" %}?srv_acct_id={{ row.id }}', 'Update Token', 'This will delete the API token and create a new one. Do you wish to continue?', 'Continue', 'POST');">
-                                <i class="fas fa-sync-alt ml-1 mr-1"></i>
+                                <i class="fas fa-sync-alt mx-2"></i>
                             </a>
 
                             <!-- api token history -->
                             <a href="#" title="view api token history" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="showInfo('{% url "userextensions:get_srv_acct_token_history" %}', '{{ row.id }}', 'Token Refresh History: <small><i>{{ row.user.username }}</i></small>', 'lg');">
-                                <i class="fas fa-history ml-1 mr-1"></i>
+                                <i class="fas fa-history mx-2"></i>
                             </a>
 
                             <!-- enable/disable -->
                             {% if row.enabled %}
                             <a href="#" title="disable service account" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="confirmAction('{% url "userextensions:disable_srv_account" %}?srv_acct_id={{ row.id }}', 'Disable Service Account', 'This will set the <i>{{ row.user }}</i> service account to disabled. Do you wish to continue?', 'Continue', 'POST');">
-                                <i class="fas fa-toggle-off ml-1 mr-1"></i>
+                                <i class="fas fa-toggle-off mx-2"></i>
                             </a>
                             {% else %}
                             <a href="#" title="enable service account" role="button" data-toggle="tooltip" data-placement="left"
                                 onClick="confirmAction('{% url "userextensions:enable_srv_account" %}?srv_acct_id={{ row.id }}', 'Enable Service Account', 'This will set the <i>{{ row.user }}</i> service account to enabled. Do you wish to continue?', 'Continue', 'POST');">
-                                <i class="fas fa-toggle-on ml-1 mr-1"></i>
+                                <i class="fas fa-toggle-on mx-2"></i>
                             </a>
                             {% endif %}
 
                             <!-- view users in group -->
                             <a href="#" title="view users in {{ row.group }}" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="showInfo('{% url "userextensions:get_users_per_group" %}', '{{ row.group.id }}', 'Users: <small><i>{{ row.group.name }}</i></small>', 'lg');">
-                            <i class="fas fa-user-friends ml-1 mr-1"></i>
+                            <i class="fas fa-user-friends mx-2"></i>
                             </a>
 
                             <a href="#" title="create custom service account in {{ row.group }}" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="createCustomServiceAccount('{% url 'userextensions:create_custom_srv_account' %}?id={{ row.group.id }}', 'Create Custom Service Account', 'Create');">
-                                <i class="fas fa-user-plus"></i>
+                                <i class="fas fa-user-plus mx-2"></i>
                             </a>
 
                             <!-- delete -->
                             <a href="#" title="delete service account" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="confirmAction('{% url "userextensions:delete_srv_account" %}?srv_acct_id={{ row.id }}', 'Delete Service Account', 'This will permanently delete the <i>{{ row.user }}</i> service account. Do you wish to continue?', 'Continue', 'POST');">
-                               <i class="fas fa-trash ml-1 mr-1"></i>
+                               <i class="fas fa-trash mx-2"></i>
                             </a>
                         </td>
                     </tr>
                     {% endfor %}
                     </tbody>
                 </table>
             </div>
@@ -133,23 +133,23 @@
                         <td><span class="ml-1">
                             <a href="#" title="view users in {{ row }}" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="showInfo('{% url "userextensions:get_users_per_group" %}', '{{ row.id }}', 'Users: <small><i>{{ row.name }}</i></small>', 'lg');">{{ row.user_set.count }}</a>
                         </span></td>
                         <td>
                             <a href="#" title="view users in {{ row }}" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="showInfo('{% url "userextensions:get_users_per_group" %}', '{{ row.id }}', 'Users: <small><i>{{ row.name }}</i></small>', 'lg');">
-                                <i class="fas fa-user-friends ml-1 mr-1"></i>
+                                <i class="fas fa-user-friends mx-2"></i>
                             </a>
                             <a href="#" title="create service account" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="confirmAction('{% url 'userextensions:create_srv_account' %}?group_id={{ row.id }}', 'Create Service Account', 'This will create a new service account linked to <b><i>{{ row.name }}</i></b>. Do you wish to continue?', 'Continue', 'POST');">
-                                <i class="fas fa-plus ml-1 mr-1"></i>
+                                <i class="fas fa-plus mx-2"></i>
                             </a>
                             <a href="#" title="create custom service account" role="button" data-toggle="tooltip" data-placement="left"
                                onClick="createCustomServiceAccount('{% url 'userextensions:create_custom_srv_account' %}?id={{ row.id }}', 'Create Custom Service Account', 'Create');">
-                                <i class="fas fa-user-plus"></i>
+                                <i class="fas fa-user-plus mx-2"></i>
                             </a>
                         </td>
                     </tr>
                     {% endfor %}
                     </tbody>
                 </table>
             </div>
```

### Comparing `django-userextensions-0.2.2/userextensions/templates/userextensions/detail/detail_user.html` & `django-userextensions-0.3.0/userextensions/templates/userextensions/detail/detail_user.html`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/templates/userextensions/form/edit_favorite.htm` & `django-userextensions-0.3.0/userextensions/templates/userextensions/form/edit_favorite.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm` & `django-userextensions-0.3.0/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/templates/userextensions/table/table_favorites.htm` & `django-userextensions-0.3.0/userextensions/templates/userextensions/table/table_favorites.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/templates/userextensions/table/table_recents.htm` & `django-userextensions-0.3.0/userextensions/templates/userextensions/table/table_recents.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/templates/userextensions/userextensions_base.htm` & `django-userextensions-0.3.0/userextensions/templates/userextensions/userextensions_base.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/templatetags/userextension_tags.py` & `django-userextensions-0.3.0/userextensions/templatetags/userextension_tags.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/urls.py` & `django-userextensions-0.3.0/userextensions/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,12 +35,12 @@
     path('create_srv_account', action.CreateServiceAccount.as_view(), name='create_srv_account'),
     path('delete_srv_account', action.DeleteServiceAccount.as_view(), name='delete_srv_account'),
     path('enable_srv_account', action.EnableServiceAccount.as_view(), name='enable_srv_account'),
     path('disable_srv_account', action.DisableServiceAccount.as_view(), name='disable_srv_account'),
     path('edit_favorite', action.EditFavorite.as_view(), name='edit_favorite'),
 
     # ajax views
-    path('get_users_per_group', ajax.get_users_per_group, name='get_users_per_group'),
-    path('get_srv_acct_token_history', ajax.get_srv_acct_token_history, name='get_srv_acct_token_history'),
-    path('show_srv_acct_token', ajax.show_srv_acct_token, name='show_srv_acct_token'),
+    path('get_users_per_group', ajax.GetUsersPerGroup.as_view(), name='get_users_per_group'),
+    path('get_srv_acct_token_history', ajax.GetSerivceAccountTokenHistory.as_view(), name='get_srv_acct_token_history'),
+    path('show_srv_acct_token', ajax.GetSerivceAccountToken.as_view(), name='show_srv_acct_token'),
 
 ]
```

### Comparing `django-userextensions-0.2.2/userextensions/views/action.py` & `django-userextensions-0.3.0/userextensions/views/action.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.2.2/userextensions/views/gui.py` & `django-userextensions-0.3.0/userextensions/views/gui.py`

 * *Files identical despite different names*

