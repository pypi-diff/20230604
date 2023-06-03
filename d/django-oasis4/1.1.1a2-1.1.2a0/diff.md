# Comparing `tmp/django-oasis4-1.1.1a2.tar.gz` & `tmp/django-oasis4-1.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oasis4-1.1.1a2.tar", last modified: Wed May 24 04:03:34 2023, max compression
+gzip compressed data, was "django-oasis4-1.1.2a0.tar", last modified: Sat Jun  3 22:24:24 2023, max compression
```

## Comparing `django-oasis4-1.1.1a2.tar` & `django-oasis4-1.1.2a0.tar`

### file list

```diff
@@ -1,149 +1,152 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.722520 django-oasis4-1.1.1a2/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-1.1.1a2/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      144 2023-03-02 20:32:01.000000 django-oasis4-1.1.1a2/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13080 2023-05-24 04:03:34.722520 django-oasis4-1.1.1a2/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      217 2023-02-13 15:48:51.000000 django-oasis4-1.1.1a2/README.md
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.704521 django-oasis4-1.1.1a2/django_oasis4.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13080 2023-05-24 04:03:34.000000 django-oasis4-1.1.1a2/django_oasis4.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     4419 2023-05-24 04:03:34.000000 django-oasis4-1.1.1a2/django_oasis4.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-05-24 04:03:34.000000 django-oasis4-1.1.1a2/django_oasis4.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       78 2023-05-24 04:03:34.000000 django-oasis4-1.1.1a2/django_oasis4.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        6 2023-05-24 04:03:34.000000 django-oasis4-1.1.1a2/django_oasis4.egg-info/top_level.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.704521 django-oasis4-1.1.1a2/oasis/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-10 23:55:40.000000 django-oasis4-1.1.1a2/oasis/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1394 2023-03-18 18:38:34.000000 django-oasis4-1.1.1a2/oasis/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.705520 django-oasis4-1.1.1a2/oasis/coffee_offers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-22 14:19:30.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      686 2023-03-06 19:37:38.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/admin.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1253 2023-03-07 16:31:05.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/admin_views.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.705520 django-oasis4-1.1.1a2/oasis/coffee_offers/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-23 15:03:46.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.706520 django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      683 2023-03-06 19:10:13.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      772 2023-02-23 15:21:03.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1199 2023-03-06 20:11:27.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/offer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.706520 django-oasis4-1.1.1a2/oasis/coffee_offers/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-03-01 20:03:07.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11193 2023-04-03 19:11:07.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/services/coffee_offers.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4101 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.706520 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-26 20:27:18.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.707520 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      656 2023-02-26 20:35:07.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1137 2023-03-07 09:29:38.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/coffee_offers_states.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      739 2023-02-26 20:34:29.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/oasis_states.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.707520 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      417 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/events/on_post_save_offer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.708521 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 21:38:01.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3414 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/utils/offer_state_machine.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.708521 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      757 2023-02-26 21:14:28.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1336 2023-02-26 21:13:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/date_validators.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      823 2023-02-26 20:45:48.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/oasis_statuses.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.700521 django-oasis4-1.1.1a2/oasis/coffee_offers/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.700521 django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.708521 django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4521 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     6279 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.709520 django-oasis4-1.1.1a2/oasis/coffee_offers/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 23:14:13.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1365 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/tasks/sync_coffe_offers.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.710520 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1072 2023-03-08 13:40:32.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/change_status.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2023-03-08 13:40:32.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/change_status.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.710520 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/coffee_offers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/coffee_offers/contract_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/coffee_offers/promisory_note.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/coffee_offers/terms_conditions.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1054 2023-03-02 20:24:29.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/save_offer.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      785 2023-03-02 20:03:04.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/save_offer.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      981 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.710520 django-oasis4-1.1.1a2/oasis/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-11-16 14:55:35.000000 django-oasis4-1.1.1a2/oasis/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.711520 django-oasis4-1.1.1a2/oasis/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      582 2023-01-17 21:45:20.000000 django-oasis4-1.1.1a2/oasis/lib/choices/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      783 2023-03-18 17:17:41.000000 django-oasis4-1.1.1a2/oasis/lib/choices/customer_type.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.714520 django-oasis4-1.1.1a2/oasis/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1525 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      780 2023-02-23 14:39:16.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      682 2023-01-28 14:38:17.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1355 2023-01-18 02:07:35.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_document_type.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1578 2023-03-08 14:17:45.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_offer.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1212 2022-12-14 20:34:45.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_product.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2159 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_state_machine.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1201 2023-03-02 21:35:32.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_associate_balance.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2701 2023-03-01 16:42:42.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_client.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1050 2023-01-27 03:47:52.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1390 2023-02-07 10:48:09.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4007 2023-01-24 23:42:01.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_discount.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-01-24 23:42:01.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_geographic_location.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      799 2023-02-23 14:57:09.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_location.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     7130 2023-03-08 14:56:20.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_operation.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-02-06 19:28:19.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_periods.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      906 2022-12-19 16:49:04.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_product.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      730 2023-01-25 00:42:41.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_type_client.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.714520 django-oasis4-1.1.1a2/oasis/lib/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      658 2023-02-07 09:06:27.000000 django-oasis4-1.1.1a2/oasis/lib/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      789 2023-02-07 09:25:36.000000 django-oasis4-1.1.1a2/oasis/lib/serializers/oasis_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2022-12-14 20:01:00.000000 django-oasis4-1.1.1a2/oasis/lib/serializers/product.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.714520 django-oasis4-1.1.1a2/oasis/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      579 2023-03-03 19:38:17.000000 django-oasis4-1.1.1a2/oasis/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3274 2023-04-03 19:11:07.000000 django-oasis4-1.1.1a2/oasis/lib/utils/oasis_actions.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.701521 django-oasis4-1.1.1a2/oasis/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.701521 django-oasis4-1.1.1a2/oasis/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.715520 django-oasis4-1.1.1a2/oasis/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2138 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5606 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.718520 django-oasis4-1.1.1a2/oasis/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    29691 2022-12-13 18:21:01.000000 django-oasis4-1.1.1a2/oasis/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    31003 2023-01-17 22:22:35.000000 django-oasis4-1.1.1a2/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    17130 2023-01-26 02:36:44.000000 django-oasis4-1.1.1a2/oasis/migrations/0003_oasiscompany_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5814 2023-01-27 03:47:55.000000 django-oasis4-1.1.1a2/oasis/migrations/0004_account_vaccountingbalanceclient.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      515 2023-02-02 01:56:29.000000 django-oasis4-1.1.1a2/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1582 2023-02-05 00:32:58.000000 django-oasis4-1.1.1a2/oasis/migrations/0006_periods.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      949 2023-02-07 02:05:07.000000 django-oasis4-1.1.1a2/oasis/migrations/0007_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     9373 2023-02-23 14:51:01.000000 django-oasis4-1.1.1a2/oasis/migrations/0008_location_coffeewarehouse_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3584 2023-03-01 16:44:41.000000 django-oasis4-1.1.1a2/oasis/migrations/0009_associatebalance.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    47342 2023-03-03 23:16:58.000000 django-oasis4-1.1.1a2/oasis/migrations/0010_operation.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3905 2023-03-04 03:34:51.000000 django-oasis4-1.1.1a2/oasis/migrations/0011_offer_statemachine_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      442 2023-03-04 03:50:49.000000 django-oasis4-1.1.1a2/oasis/migrations/0012_offer_price.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1782 2023-03-06 20:01:57.000000 django-oasis4-1.1.1a2/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      832 2023-03-07 08:33:48.000000 django-oasis4-1.1.1a2/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      465 2023-03-07 08:43:20.000000 django-oasis4-1.1.1a2/oasis/migrations/0015_statemachine_update_oasis.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      571 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/migrations/0017_statemachine_state_at_timeout.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1553 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a2/oasis/migrations/0018_offermov.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1009 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/migrations/0019_stat.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2022-12-10 21:43:40.000000 django-oasis4-1.1.1a2/oasis/migrations/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.719520 django-oasis4-1.1.1a2/oasis/models/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1647 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/models/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     9352 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/models/local_models.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)   117483 2023-03-04 02:04:38.000000 django-oasis4-1.1.1a2/oasis/models/oasis_models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.720520 django-oasis4-1.1.1a2/oasis/stats/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      419 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/admin.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.720520 django-oasis4-1.1.1a2/oasis/stats/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.720520 django-oasis4-1.1.1a2/oasis/stats/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      329 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/api/serializers/stats.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.720520 django-oasis4-1.1.1a2/oasis/stats/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      327 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3684 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/stats/api/services/stats.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      455 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.721520 django-oasis4-1.1.1a2/oasis/stats/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      477 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/stats/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.721520 django-oasis4-1.1.1a2/oasis/stats/lib/cursors/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      504 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/stats/lib/cursors/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1917 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/stats/lib/cursors/cursor.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      586 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/stats/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.722520 django-oasis4-1.1.1a2/oasis/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      812 2023-02-23 14:54:47.000000 django-oasis4-1.1.1a2/oasis/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1206 2023-02-23 14:46:31.000000 django-oasis4-1.1.1a2/oasis/tasks/sync_coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1474 2023-01-26 02:47:20.000000 django-oasis4-1.1.1a2/oasis/tasks/sync_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-01-18 02:09:04.000000 django-oasis4-1.1.1a2/oasis/tasks/sync_document_types.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1856 2023-03-01 20:00:10.000000 django-oasis4-1.1.1a2/oasis/tasks/sync_products.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      866 2023-05-24 03:51:17.000000 django-oasis4-1.1.1a2/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-05-24 04:03:34.722520 django-oasis4-1.1.1a2/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.354398 django-oasis4-1.1.2a0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-1.1.2a0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      144 2023-03-02 20:32:01.000000 django-oasis4-1.1.2a0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    13080 2023-06-03 22:24:24.354398 django-oasis4-1.1.2a0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      217 2023-02-13 15:48:51.000000 django-oasis4-1.1.2a0/README.md
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.321399 django-oasis4-1.1.2a0/django_oasis4.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    13080 2023-06-03 22:24:24.000000 django-oasis4-1.1.2a0/django_oasis4.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     4618 2023-06-03 22:24:24.000000 django-oasis4-1.1.2a0/django_oasis4.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-03 22:24:24.000000 django-oasis4-1.1.2a0/django_oasis4.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       79 2023-06-03 22:24:24.000000 django-oasis4-1.1.2a0/django_oasis4.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        6 2023-06-03 22:24:24.000000 django-oasis4-1.1.2a0/django_oasis4.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.322399 django-oasis4-1.1.2a0/oasis/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-10 23:55:40.000000 django-oasis4-1.1.2a0/oasis/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1394 2023-03-18 18:38:34.000000 django-oasis4-1.1.2a0/oasis/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.323399 django-oasis4-1.1.2a0/oasis/coffee_offers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-22 14:19:30.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      686 2023-03-06 19:37:38.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/admin.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1253 2023-03-07 16:31:05.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/admin_views.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.323399 django-oasis4-1.1.2a0/oasis/coffee_offers/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-23 15:03:46.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.324399 django-oasis4-1.1.2a0/oasis/coffee_offers/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      683 2023-03-06 19:10:13.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      772 2023-02-23 15:21:03.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/api/serializers/coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1199 2023-03-06 20:11:27.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/api/serializers/offer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.325399 django-oasis4-1.1.2a0/oasis/coffee_offers/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-03-01 20:03:07.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11193 2023-04-03 19:11:07.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/api/services/coffee_offers.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5245 2023-06-03 21:53:44.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.325399 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-26 20:27:18.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.326399 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      656 2023-02-26 20:35:07.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/choices/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1137 2023-06-02 10:37:36.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/choices/coffee_offers_states.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      739 2023-02-26 20:34:29.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/choices/oasis_states.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.326399 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/events/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      417 2023-03-16 21:48:47.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/events/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-03-16 21:48:47.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/events/on_post_save_offer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.327399 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 21:38:01.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     6431 2023-06-03 21:46:20.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/utils/offer_state_machine.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.328399 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/validators/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      757 2023-02-26 21:14:28.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/validators/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1336 2023-02-26 21:13:57.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/validators/date_validators.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      823 2023-02-26 20:45:48.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/lib/validators/oasis_statuses.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.314399 django-oasis4-1.1.2a0/oasis/coffee_offers/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.315399 django-oasis4-1.1.2a0/oasis/coffee_offers/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.328399 django-oasis4-1.1.2a0/oasis/coffee_offers/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4521 2023-03-16 14:42:57.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     6279 2023-03-16 14:42:57.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.329399 django-oasis4-1.1.2a0/oasis/coffee_offers/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 23:14:13.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1564 2023-06-03 21:35:38.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/tasks/sync_coffe_offers.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.330399 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1072 2023-03-08 13:40:32.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/change_status.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2023-03-08 13:40:32.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/change_status.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.332399 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/coffee_offers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-06-02 13:51:20.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/coffee_offers/coffee_notification.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/coffee_offers/coffee_offer.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/coffee_offers/contract_template.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-05-31 21:36:30.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/coffee_offers/intention_letter.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/coffee_offers/promissory_note.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-06-01 00:16:12.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/coffee_offers/remittance_letter.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1054 2023-03-02 20:24:29.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/save_offer.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      785 2023-03-02 20:03:04.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/templates/save_offer.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      981 2023-03-16 14:42:57.000000 django-oasis4-1.1.2a0/oasis/coffee_offers/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.332399 django-oasis4-1.1.2a0/oasis/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-11-16 14:55:35.000000 django-oasis4-1.1.2a0/oasis/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.333399 django-oasis4-1.1.2a0/oasis/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      582 2023-01-17 21:45:20.000000 django-oasis4-1.1.2a0/oasis/lib/choices/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      783 2023-03-18 17:17:41.000000 django-oasis4-1.1.2a0/oasis/lib/choices/customer_type.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.338399 django-oasis4-1.1.2a0/oasis/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1525 2023-03-16 14:42:57.000000 django-oasis4-1.1.2a0/oasis/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      780 2023-02-23 14:39:16.000000 django-oasis4-1.1.2a0/oasis/lib/managers/local_coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      682 2023-01-28 14:38:17.000000 django-oasis4-1.1.2a0/oasis/lib/managers/local_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1355 2023-01-18 02:07:35.000000 django-oasis4-1.1.2a0/oasis/lib/managers/local_document_type.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1578 2023-03-08 14:17:45.000000 django-oasis4-1.1.2a0/oasis/lib/managers/local_offer.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1212 2022-12-14 20:34:45.000000 django-oasis4-1.1.2a0/oasis/lib/managers/local_product.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2159 2023-03-16 14:42:57.000000 django-oasis4-1.1.2a0/oasis/lib/managers/local_state_machine.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1201 2023-03-02 21:35:32.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_associate_balance.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2701 2023-03-01 16:42:42.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_client.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1050 2023-01-27 03:47:52.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1390 2023-02-07 10:48:09.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4007 2023-01-24 23:42:01.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_discount.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-01-24 23:42:01.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_geographic_location.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      799 2023-02-23 14:57:09.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_location.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     7130 2023-03-08 14:56:20.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_operation.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-02-06 19:28:19.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_periods.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      906 2022-12-19 16:49:04.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_product.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      730 2023-01-25 00:42:41.000000 django-oasis4-1.1.2a0/oasis/lib/managers/oasis_type_client.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.339398 django-oasis4-1.1.2a0/oasis/lib/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      658 2023-02-07 09:06:27.000000 django-oasis4-1.1.2a0/oasis/lib/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      789 2023-02-07 09:25:36.000000 django-oasis4-1.1.2a0/oasis/lib/serializers/oasis_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2022-12-14 20:01:00.000000 django-oasis4-1.1.2a0/oasis/lib/serializers/product.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.340399 django-oasis4-1.1.2a0/oasis/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      579 2023-03-03 19:38:17.000000 django-oasis4-1.1.2a0/oasis/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3275 2023-06-01 01:52:21.000000 django-oasis4-1.1.2a0/oasis/lib/utils/oasis_actions.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.317399 django-oasis4-1.1.2a0/oasis/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.317399 django-oasis4-1.1.2a0/oasis/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.340399 django-oasis4-1.1.2a0/oasis/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2138 2023-05-24 03:50:25.000000 django-oasis4-1.1.2a0/oasis/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5606 2023-05-24 03:50:25.000000 django-oasis4-1.1.2a0/oasis/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.346398 django-oasis4-1.1.2a0/oasis/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    29691 2022-12-13 18:21:01.000000 django-oasis4-1.1.2a0/oasis/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    31003 2023-01-17 22:22:35.000000 django-oasis4-1.1.2a0/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    17130 2023-01-26 02:36:44.000000 django-oasis4-1.1.2a0/oasis/migrations/0003_oasiscompany_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5814 2023-01-27 03:47:55.000000 django-oasis4-1.1.2a0/oasis/migrations/0004_account_vaccountingbalanceclient.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      515 2023-02-02 01:56:29.000000 django-oasis4-1.1.2a0/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1582 2023-02-05 00:32:58.000000 django-oasis4-1.1.2a0/oasis/migrations/0006_periods.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      949 2023-02-07 02:05:07.000000 django-oasis4-1.1.2a0/oasis/migrations/0007_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9373 2023-02-23 14:51:01.000000 django-oasis4-1.1.2a0/oasis/migrations/0008_location_coffeewarehouse_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3584 2023-03-01 16:44:41.000000 django-oasis4-1.1.2a0/oasis/migrations/0009_associatebalance.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    47342 2023-03-03 23:16:58.000000 django-oasis4-1.1.2a0/oasis/migrations/0010_operation.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3905 2023-03-04 03:34:51.000000 django-oasis4-1.1.2a0/oasis/migrations/0011_offer_statemachine_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      442 2023-03-04 03:50:49.000000 django-oasis4-1.1.2a0/oasis/migrations/0012_offer_price.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1782 2023-03-06 20:01:57.000000 django-oasis4-1.1.2a0/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      832 2023-03-07 08:33:48.000000 django-oasis4-1.1.2a0/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      465 2023-03-07 08:43:20.000000 django-oasis4-1.1.2a0/oasis/migrations/0015_statemachine_update_oasis.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-03-16 14:42:57.000000 django-oasis4-1.1.2a0/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      571 2023-03-16 14:42:57.000000 django-oasis4-1.1.2a0/oasis/migrations/0017_statemachine_state_at_timeout.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1553 2023-03-16 21:48:47.000000 django-oasis4-1.1.2a0/oasis/migrations/0018_offermov.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1009 2023-05-19 21:49:17.000000 django-oasis4-1.1.2a0/oasis/migrations/0019_stat.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2022-12-10 21:43:40.000000 django-oasis4-1.1.2a0/oasis/migrations/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.347398 django-oasis4-1.1.2a0/oasis/models/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1647 2023-05-19 21:49:17.000000 django-oasis4-1.1.2a0/oasis/models/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9352 2023-05-19 21:49:17.000000 django-oasis4-1.1.2a0/oasis/models/local_models.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)   117483 2023-03-04 02:04:38.000000 django-oasis4-1.1.2a0/oasis/models/oasis_models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.349398 django-oasis4-1.1.2a0/oasis/stats/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.2a0/oasis/stats/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      419 2023-05-19 21:49:17.000000 django-oasis4-1.1.2a0/oasis/stats/admin.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.350398 django-oasis4-1.1.2a0/oasis/stats/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.2a0/oasis/stats/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.350398 django-oasis4-1.1.2a0/oasis/stats/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      329 2023-05-19 21:49:17.000000 django-oasis4-1.1.2a0/oasis/stats/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-05-19 21:49:17.000000 django-oasis4-1.1.2a0/oasis/stats/api/serializers/stats.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.351398 django-oasis4-1.1.2a0/oasis/stats/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      327 2023-05-19 21:49:17.000000 django-oasis4-1.1.2a0/oasis/stats/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3684 2023-05-24 03:50:25.000000 django-oasis4-1.1.2a0/oasis/stats/api/services/stats.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      455 2023-05-19 21:49:17.000000 django-oasis4-1.1.2a0/oasis/stats/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.351398 django-oasis4-1.1.2a0/oasis/stats/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      477 2023-05-24 03:50:25.000000 django-oasis4-1.1.2a0/oasis/stats/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.352398 django-oasis4-1.1.2a0/oasis/stats/lib/cursors/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      504 2023-05-24 03:50:25.000000 django-oasis4-1.1.2a0/oasis/stats/lib/cursors/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1917 2023-05-24 03:50:25.000000 django-oasis4-1.1.2a0/oasis/stats/lib/cursors/cursor.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      586 2023-05-24 03:50:25.000000 django-oasis4-1.1.2a0/oasis/stats/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-03 22:24:24.353398 django-oasis4-1.1.2a0/oasis/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      812 2023-02-23 14:54:47.000000 django-oasis4-1.1.2a0/oasis/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1206 2023-02-23 14:46:31.000000 django-oasis4-1.1.2a0/oasis/tasks/sync_coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1474 2023-01-26 02:47:20.000000 django-oasis4-1.1.2a0/oasis/tasks/sync_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-01-18 02:09:04.000000 django-oasis4-1.1.2a0/oasis/tasks/sync_document_types.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1856 2023-03-01 20:00:10.000000 django-oasis4-1.1.2a0/oasis/tasks/sync_products.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      867 2023-06-03 22:14:13.000000 django-oasis4-1.1.2a0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-03 22:24:24.354398 django-oasis4-1.1.2a0/setup.cfg
```

### Comparing `django-oasis4-1.1.1a2/LICENSE` & `django-oasis4-1.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/PKG-INFO` & `django-oasis4-1.1.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4
-Version: 1.1.1a2
+Version: 1.1.2a0
 Summary: OASIS4 Data Interfaces
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
```

### Comparing `django-oasis4-1.1.1a2/django_oasis4.egg-info/PKG-INFO` & `django-oasis4-1.1.2a0/django_oasis4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4
-Version: 1.1.1a2
+Version: 1.1.2a0
 Summary: OASIS4 Data Interfaces
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
```

### Comparing `django-oasis4-1.1.1a2/django_oasis4.egg-info/SOURCES.txt` & `django-oasis4-1.1.2a0/django_oasis4.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,20 @@
 oasis/coffee_offers/locale/es/LC_MESSAGES/django.po
 oasis/coffee_offers/tasks/__init__.py
 oasis/coffee_offers/tasks/sync_coffe_offers.py
 oasis/coffee_offers/templates/change_status.html
 oasis/coffee_offers/templates/change_status.txt
 oasis/coffee_offers/templates/save_offer.html
 oasis/coffee_offers/templates/save_offer.txt
+oasis/coffee_offers/templates/coffee_offers/coffee_notification.html
+oasis/coffee_offers/templates/coffee_offers/coffee_offer.html
 oasis/coffee_offers/templates/coffee_offers/contract_template.html
-oasis/coffee_offers/templates/coffee_offers/promisory_note.html
-oasis/coffee_offers/templates/coffee_offers/terms_conditions.html
+oasis/coffee_offers/templates/coffee_offers/intention_letter.html
+oasis/coffee_offers/templates/coffee_offers/promissory_note.html
+oasis/coffee_offers/templates/coffee_offers/remittance_letter.html
 oasis/lib/__init__.py
 oasis/lib/choices/__init__.py
 oasis/lib/choices/customer_type.py
 oasis/lib/managers/__init__.py
 oasis/lib/managers/local_coffee_ware_house.py
 oasis/lib/managers/local_company.py
 oasis/lib/managers/local_document_type.py
```

### Comparing `django-oasis4-1.1.1a2/oasis/apps.py` & `django-oasis4-1.1.2a0/oasis/apps.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/admin.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/admin.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/admin_views.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/admin_views.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/__init__.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/coffee_ware_house.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/api/serializers/coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/offer.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/api/serializers/offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/api/services/__init__.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/api/services/coffee_offers.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/api/services/coffee_offers.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/apps.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/apps.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,17 +59,32 @@
         settings.COFFEE_OFFERS_LOAD_ALL = getattr(settings, "COFFEE_OFFERS_LOAD_ALL", False)
         # Round factor
         settings.COFFEE_OFFERS_ROUND_FACTOR = getattr(settings, "COFFEE_OFFERS_ROUND_FACTOR", 10)
         # Contract Template
         settings.COFFEE_OFFERS_CONTRACT_TEMPLATE = getattr(settings, "COFFEE_OFFERS_CONTRACT_TEMPLATE",
                                                            "contract_template.html")
         # Terms and conditions template
-        settings.COFFEE_OFFERS_TERMS_TEMPLATE = getattr(settings, "COFFEE_OFFERS_TERMS_TEMPLATE",
-                                                        "terms_conditions.html")
+        settings.COFFEE_OFFERS_OFFER_TEMPLATE = getattr(settings, "COFFEE_OFFERS_OFFER_TEMPLATE",
+                                                        "coffee_offer.html")
         # Promissory note
         settings.COFFEE_OFFERS_PROMISE_TEMPLATE = getattr(settings, "COFFEE_OFFERS_PROMISE_TEMPLATE",
-                                                          "promisory_note.html")
+                                                          "promissory_note.html")
+        # Intention Letter
+        settings.COFFEE_OFFERS_INTENTION_LETTER_TEMPLATE = getattr(settings, "COFFEE_OFFERS_INTENTION_LETTER_TEMPLATE",
+                                                                   "intention_letter.html")
+        # Remittance Letter
+        settings.COFFEE_OFFERS_REMITTANCE_EMAIL_TEMPLATE = getattr(settings,
+                                                                   "COFFEE_OFFERS_REMITTANCE_EMAIL_TEMPLATE",
+                                                                   "coffee_offers/remittance_letter.html")
+        # Notification template
+        settings.COFFEE_OFFERS_NOTIFICATION_EMAIL_TEMPLATE = getattr(settings,
+                                                                     "COFFEE_OFFERS_NOTIFICATION_EMAIL_TEMPLATE",
+                                                                     "coffee_offers/coffee_notification.html")
+        # Notifications EMails
+        settings.COFFEE_OFFERS_LEGAL_AREA_EMAIL = getattr(settings, "COFFEE_OFFERS_LEGAL_AREA_EMAIL", None)
+        settings.COFFEE_OFFERS_COFFEE_AREA_EMAIL = getattr(settings, "COFFEE_OFFERS_COFFEE_AREA_EMAIL", None)
+
         # Coffee factor for offers
         settings.COFFEE_OFFERS_FACTOR = getattr(settings, "COFFEE_OFFERS_FACTOR", 94)
         # Coffee Offers product list
         settings.COFFEE_OFFERS_PRODUCT_LIST = getattr(settings, "COFFEE_OFFERS_PRODUCT_LIST",
                                                       "2101,2102,2104,2106,2107,2109,2112,2113,2114,2126,2120,2134")
```

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/__init__.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/lib/choices/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/coffee_offers_states.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/lib/choices/coffee_offers_states.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/oasis_states.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/lib/choices/oasis_states.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/events/on_post_save_offer.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/lib/events/on_post_save_offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/utils/__init__.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/__init__.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/lib/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/date_validators.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/lib/validators/date_validators.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/oasis_statuses.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/lib/validators/oasis_statuses.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo` & `django-oasis4-1.1.2a0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po` & `django-oasis4-1.1.2a0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/tasks/__init__.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/tasks/sync_coffe_offers.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/tasks/sync_coffe_offers.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # IDE:          PyCharm
 # Developed by: macercha
 # Date:         6/03/23 16:34
 # Project:      CFHL Transactional Backend
 # Module Name:  sync_coffe_offers
 # Description:
 # ****************************************************************
+import logging
 from core import celery_app
 from django.conf import settings
 from oasis.coffee_offers.lib.utils import OfferStateMachine
 from oasis.models import Offer
 from oasis.models import Operation
 from typing import Any
 
@@ -25,10 +26,15 @@
 
     offer_qs = Offer.objects.get_all_active_offers()
     for offer in offer_qs:
         operation = Operation.objects.get_by_operation_pk(document_id=document_id,
                                                           location_id=offer.warehouse.location_id,
                                                           number_id=offer.contract).first()
         if operation is not None:
-            state_machine = OfferStateMachine(offer, operation)
-            state_machine.run()
-            state_machine.validate_timeout()
+            try:
+                state_machine = OfferStateMachine(offer, operation)
+                state_machine.run()
+                state_machine.validate_timeout()
+            except ValueError as exc:
+                logging.debug(str(exc))
+            except Exception as exc:
+                logging.debug(str(exc))
```

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/templates/change_status.html` & `django-oasis4-1.1.2a0/oasis/coffee_offers/templates/change_status.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/templates/change_status.txt` & `django-oasis4-1.1.2a0/oasis/coffee_offers/templates/change_status.txt`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/templates/save_offer.html` & `django-oasis4-1.1.2a0/oasis/coffee_offers/templates/save_offer.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/templates/save_offer.txt` & `django-oasis4-1.1.2a0/oasis/coffee_offers/templates/save_offer.txt`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/urls.py` & `django-oasis4-1.1.2a0/oasis/coffee_offers/urls.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/choices/__init__.py` & `django-oasis4-1.1.2a0/oasis/lib/choices/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/choices/customer_type.py` & `django-oasis4-1.1.2a0/oasis/lib/choices/customer_type.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/__init__.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_coffee_ware_house.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/local_coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_company.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/local_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_document_type.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/local_document_type.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_offer.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/local_offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_product.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/local_product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_state_machine.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/local_state_machine.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_associate_balance.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_associate_balance.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_client.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_client.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_company.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_cycle.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_discount.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_discount.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_geographic_location.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_geographic_location.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_location.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_location.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_operation.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_operation.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_periods.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_periods.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_product.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_type_client.py` & `django-oasis4-1.1.2a0/oasis/lib/managers/oasis_type_client.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/serializers/__init__.py` & `django-oasis4-1.1.2a0/oasis/lib/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/serializers/oasis_cycle.py` & `django-oasis4-1.1.2a0/oasis/lib/serializers/oasis_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/serializers/product.py` & `django-oasis4-1.1.2a0/oasis/lib/serializers/product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/utils/__init__.py` & `django-oasis4-1.1.2a0/oasis/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/utils/oasis_actions.py` & `django-oasis4-1.1.2a0/oasis/lib/utils/oasis_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
                 offer = Offer.objects.get_by_pk(pk=offer_id).get()
                 operation = Operation.objects.get_by_operation_pk(document_id=document_id,
                                                                   location_id=offer.warehouse.location_id,
                                                                   number_id=offer.contract).first()
                 if operation is not None:
                     state_machine = OfferStateMachine(offer=offer, operation=operation)
                     state_machine.set(new_state=new_state)
+
                 else:
                     raise Operation.DoesNotExist(_("Operation record does not exist!"))
             else:
                 raise ValidationError(_("Error changing state. Required data not found."))
         except Exception as exc:
             raise
         else:
```

### Comparing `django-oasis4-1.1.1a2/oasis/locale/es/LC_MESSAGES/django.mo` & `django-oasis4-1.1.2a0/oasis/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/locale/es/LC_MESSAGES/django.po` & `django-oasis4-1.1.2a0/oasis/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0001_initial.py` & `django-oasis4-1.1.2a0/oasis/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py` & `django-oasis4-1.1.2a0/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0003_oasiscompany_company.py` & `django-oasis4-1.1.2a0/oasis/migrations/0003_oasiscompany_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0004_account_vaccountingbalanceclient.py` & `django-oasis4-1.1.2a0/oasis/migrations/0004_account_vaccountingbalanceclient.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py` & `django-oasis4-1.1.2a0/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0006_periods.py` & `django-oasis4-1.1.2a0/oasis/migrations/0006_periods.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0007_cycle.py` & `django-oasis4-1.1.2a0/oasis/migrations/0007_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0008_location_coffeewarehouse_and_more.py` & `django-oasis4-1.1.2a0/oasis/migrations/0008_location_coffeewarehouse_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0009_associatebalance.py` & `django-oasis4-1.1.2a0/oasis/migrations/0009_associatebalance.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0010_operation.py` & `django-oasis4-1.1.2a0/oasis/migrations/0010_operation.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0011_offer_statemachine_and_more.py` & `django-oasis4-1.1.2a0/oasis/migrations/0011_offer_statemachine_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py` & `django-oasis4-1.1.2a0/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py` & `django-oasis4-1.1.2a0/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py` & `django-oasis4-1.1.2a0/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0017_statemachine_state_at_timeout.py` & `django-oasis4-1.1.2a0/oasis/migrations/0017_statemachine_state_at_timeout.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0018_offermov.py` & `django-oasis4-1.1.2a0/oasis/migrations/0018_offermov.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0019_stat.py` & `django-oasis4-1.1.2a0/oasis/migrations/0019_stat.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/models/__init__.py` & `django-oasis4-1.1.2a0/oasis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/models/local_models.py` & `django-oasis4-1.1.2a0/oasis/models/local_models.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/models/oasis_models.py` & `django-oasis4-1.1.2a0/oasis/models/oasis_models.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/stats/api/services/stats.py` & `django-oasis4-1.1.2a0/oasis/stats/api/services/stats.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/stats/lib/cursors/cursor.py` & `django-oasis4-1.1.2a0/oasis/stats/lib/cursors/cursor.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/stats/urls.py` & `django-oasis4-1.1.2a0/oasis/stats/urls.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/tasks/__init__.py` & `django-oasis4-1.1.2a0/oasis/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/tasks/sync_coffee_ware_house.py` & `django-oasis4-1.1.2a0/oasis/tasks/sync_coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/tasks/sync_company.py` & `django-oasis4-1.1.2a0/oasis/tasks/sync_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/tasks/sync_document_types.py` & `django-oasis4-1.1.2a0/oasis/tasks/sync_document_types.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/tasks/sync_products.py` & `django-oasis4-1.1.2a0/oasis/tasks/sync_products.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/pyproject.toml` & `django-oasis4-1.1.2a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "django-oasis4"
-version = "1.1.1-alpha.2"
+version = "1.1.2-alpha.0"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "OASIS4 Data Interfaces"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
@@ -26,13 +26,13 @@
     "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
     "Django>=4.1",
     "cx-Oracle",
     "celery>=5.2.7",
     "django-celery-beat",
-    "zibanu-django>=1.0.0a8"
+    "zibanu-django>=1.2.0a11"
 ]
 keywords = [
     "django",
     "cadefihuila"
 ]
```

