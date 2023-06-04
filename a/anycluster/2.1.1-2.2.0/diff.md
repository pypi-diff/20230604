# Comparing `tmp/anycluster-2.1.1.tar.gz` & `tmp/anycluster-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycluster-2.1.1.tar", last modified: Mon May 22 06:46:05 2023, max compression
+gzip compressed data, was "anycluster-2.2.0.tar", last modified: Sun Jun  4 14:57:16 2023, max compression
```

## Comparing `anycluster-2.1.1.tar` & `anycluster-2.2.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.081524 anycluster-2.1.1/
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.1.1/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.1.1/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-05-22 06:46:05.081524 anycluster-2.1.1/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.1.1/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.073525 anycluster-2.1.1/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.1.1/anycluster/ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3656 2023-05-19 12:35:24.000000 anycluster-2.1.1/anycluster/FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    31624 2023-04-19 10:53:31.000000 anycluster-2.1.1/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.1.1/anycluster/MapTools.py
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.1.1/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.073525 anycluster-2.1.1/anycluster/api/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.077525 anycluster-2.1.1/anycluster/api/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.1.1/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.1.1/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2650 2023-05-19 13:08:28.000000 anycluster-2.1.1/anycluster/api/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)      947 2023-04-24 13:16:49.000000 anycluster-2.1.1/anycluster/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     6016 2023-04-24 12:45:45.000000 anycluster-2.1.1/anycluster/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.1.1/anycluster/api/json_schemas.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2739 2023-05-19 13:08:27.000000 anycluster-2.1.1/anycluster/api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.077525 anycluster-2.1.1/anycluster/api/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.077525 anycluster-2.1.1/anycluster/api/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.1.1/anycluster/api/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.1.1/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     6965 2023-04-19 19:03:37.000000 anycluster-2.1.1/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.1.1/anycluster/api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9420 2023-04-19 19:03:34.000000 anycluster-2.1.1/anycluster/api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      882 2023-04-24 12:47:36.000000 anycluster-2.1.1/anycluster/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7323 2023-04-24 12:21:50.000000 anycluster-2.1.1/anycluster/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.1.1/anycluster/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.1.1/anycluster/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/globalmaptiles.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.069524 anycluster-2.1.1/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.069524 anycluster-2.1.1/anycluster/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.077525 anycluster-2.1.1/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/10_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/5_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/pin_unknown.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.081524 anycluster-2.1.1/anycluster/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.081524 anycluster-2.1.1/anycluster/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.1.1/anycluster/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2533 2023-04-19 10:53:00.000000 anycluster-2.1.1/anycluster/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.1.1/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.1.1/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.1.1/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    10728 2023-04-19 10:54:13.000000 anycluster-2.1.1/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.1.1/anycluster/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2096 2023-04-19 10:47:07.000000 anycluster-2.1.1/anycluster/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.1.1/anycluster/tests/test_ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.1.1/anycluster/tests/test_FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16495 2023-04-19 10:54:09.000000 anycluster-2.1.1/anycluster/tests/test_MapClusterer.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.073525 anycluster-2.1.1/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-05-22 06:46:05.000000 anycluster-2.1.1/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2191 2023-05-22 06:46:05.000000 anycluster-2.1.1/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-05-22 06:46:05.000000 anycluster-2.1.1/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-05-22 06:46:05.000000 anycluster-2.1.1/anycluster.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-05-22 06:46:05.000000 anycluster-2.1.1/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-05-22 06:46:05.081524 anycluster-2.1.1/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-05-22 06:41:31.000000 anycluster-2.1.1/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.741238 anycluster-2.2.0/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.2.0/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.2.0/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-04 14:57:16.741238 anycluster-2.2.0/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.2.0/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.733238 anycluster-2.2.0/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.2.0/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3656 2023-05-26 12:34:24.000000 anycluster-2.2.0/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    36887 2023-05-30 10:03:21.000000 anycluster-2.2.0/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.2.0/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.2.0/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.733238 anycluster-2.2.0/anycluster/api/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.737238 anycluster-2.2.0/anycluster/api/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.2.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.2.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3290 2023-05-26 08:56:52.000000 anycluster-2.2.0/anycluster/api/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.2.0/anycluster/api/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     7337 2023-05-26 08:42:05.000000 anycluster-2.2.0/anycluster/api/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.2.0/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3301 2023-05-26 08:56:48.000000 anycluster-2.2.0/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.737238 anycluster-2.2.0/anycluster/api/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.737238 anycluster-2.2.0/anycluster/api/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.2.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.2.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     9287 2023-05-26 08:54:01.000000 anycluster-2.2.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.2.0/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    13727 2023-05-26 08:53:58.000000 anycluster-2.2.0/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.2.0/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9493 2023-05-26 08:40:46.000000 anycluster-2.2.0/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.2.0/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.2.0/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.733238 anycluster-2.2.0/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.733238 anycluster-2.2.0/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.737238 anycluster-2.2.0/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.2.0/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.741238 anycluster-2.2.0/anycluster/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.741238 anycluster-2.2.0/anycluster/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.2.0/anycluster/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.2.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.2.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.2.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.2.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    14813 2023-05-26 08:50:17.000000 anycluster-2.2.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.2.0/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.2.0/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.2.0/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.2.0/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    25353 2023-05-26 08:50:15.000000 anycluster-2.2.0/anycluster/tests/test_MapClusterer.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-04 14:57:16.733238 anycluster-2.2.0/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-04 14:57:16.000000 anycluster-2.2.0/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2191 2023-06-04 14:57:16.000000 anycluster-2.2.0/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-04 14:57:16.000000 anycluster-2.2.0/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-06-04 14:57:16.000000 anycluster-2.2.0/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-06-04 14:57:16.000000 anycluster-2.2.0/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-04 14:57:16.741238 anycluster-2.2.0/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-06-04 14:57:01.000000 anycluster-2.2.0/setup.py
```

### Comparing `anycluster-2.1.1/LICENSE` & `anycluster-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/PKG-INFO` & `anycluster-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.1.1
+Version: 2.2.0
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.1.1/README.md` & `anycluster-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/ClusterCache.py` & `anycluster-2.2.0/anycluster/ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/FilterComposer.py` & `anycluster-2.2.0/anycluster/FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/MapClusterer.py` & `anycluster-2.2.0/anycluster/MapClusterer.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 from .clusters import PointCluster
 from django.apps import apps
 from django.db.models import ForeignKey
 from django.conf import settings
 from django.db import connections
 from django.contrib.gis.db.models.fields import BaseSpatialField
 from django.contrib.gis.gdal import SpatialReference, CoordTransform
-from django.contrib.gis.geos import Point, GEOSGeometry
+from django.contrib.gis.geos import Point, GEOSGeometry, GeometryCollection, Polygon
 from anycluster import MapTools, ClusterCache, FilterComposer
 from anycluster.definitions import (CLUSTER_TYPE_KMEANS, CLUSTER_TYPE_GRID, GEOMETRY_TYPE_VIEWPORT, GEOMETRY_TYPE_AREA,
                                     MAX_BOUNDS)
 
 import json, math
 BASE_K = getattr(settings, 'ANYCLUSTER_BASE_K', 6)
 K_CAP = getattr(settings, 'ANYCLUSTER_K_CAP', 30)
@@ -769,14 +769,113 @@
         queryset = Gis.objects.raw(
             '''SELECT {fields} FROM {schema_name}.{geo_table} WHERE id={id};'''.format(
                 schema_name=self.schema_name, geo_table=geo_table, fields=gis_fields_str, id=str(id))
         )
 
         return queryset
 
+
+    def get_map_content_counts(self, geojson, geometry_type, filters, zoom, modulations):
+
+        result = {
+            'count': 0,
+            'modulations' : {},
+        }
+
+        # currently, the geometry type for counting is always set to GEOMETRY_TYPE_AREA,
+        # because otherwise pins which are outside the current viewport, but inside the cluster geometry would be counted
+        # the pins visible on the map would not always be the returned count if GEOMETRY_TYPE_VIEWPORT was supported
+        geometry_type = GEOMETRY_TYPE_AREA
+
+        geometries_for_counting = self.get_geometries_for_counting(geojson, geometry_type, zoom)
+
+        unmodulated_count = self.query_map_content_count(geometries_for_counting, filters)
+        result['count'] = unmodulated_count
+
+        for modulation_name, modulation_filters in modulations.items():
+
+            combined_filters = filters + modulation_filters['filters']
+            modulated_count = self.query_map_content_count(geometries_for_counting, combined_filters)
+            result['modulations'][modulation_name] = {
+                'count': modulated_count
+            }
+
+        return result
+
+
+    def query_map_content_count(self, geometries_for_counting, filters):
+
+        count = 0
+
+        filter_composer = FilterComposer(filters)
+        filterstring = filter_composer.as_sql()
+
+        geom_filterstring = self.get_geom_filter_string_from_geos(geometries_for_counting)
+
+        content_count_sql = '''
+            SELECT count(*) AS count
+            FROM {schema_name}.{geo_table}
+                WHERE {geo_column_str} IS NOT NULL
+                    AND {geom_filterstring} {filterstring};
+        '''.format(schema_name=self.schema_name, geo_table=geo_table, geo_column_str=geo_column_str,
+                    geom_filterstring=geom_filterstring, filterstring=filterstring)
+
+        cursor = connections['default'].cursor()
+        cursor.execute(content_count_sql)
+        query_result = cursor.fetchone()
+
+        count += query_result[0]
+
+        return count
+
+
+    def get_grouped_map_contents(self, geojson, geometry_type, zoom, filters, group_by):
+
+        # currently, the geometry type for counting is always set to GEOMETRY_TYPE_AREA,
+        # because otherwise pins which are outside the current viewport, but inside the cluster geometry would be counted
+        # the pins visible on the map would not always be the returned count if GEOMETRY_TYPE_VIEWPORT was supported
+        geometry_type = GEOMETRY_TYPE_AREA
+
+        geometries_for_counting = self.get_geometries_for_counting(geojson, geometry_type, zoom)
+
+        geom_filterstring = self.get_geom_filter_string_from_geos(geometries_for_counting)
+        
+        filter_composer = FilterComposer(filters)
+        filterstring = filter_composer.as_sql()
+
+        groups = {}
+
+        grouped_count_sql = '''
+            SELECT COUNT(id), {group_by}
+            FROM {schema_name}.{geo_table}
+                WHERE {geo_column_str} IS NOT NULL
+                    AND {geom_filterstring} {filterstring}
+                        GROUP BY {group_by} ORDER BY {group_by} ASC;
+        '''.format(schema_name=self.schema_name, geo_table=geo_table, geo_column_str=geo_column_str,
+                    geom_filterstring=geom_filterstring, filterstring=filterstring, group_by=group_by)
+
+        cursor = connections['default'].cursor()
+        cursor.execute(grouped_count_sql)
+        results = cursor.fetchall()
+        
+        for result in results:
+            count = result[0]
+            group_name = result[1]
+
+            if group_name not in groups:
+                groups[group_name] = {
+                    'count' : count,
+                }
+
+            else:
+                groups[group_name]['count'] += count
+        
+        return groups
+
+
     '''---------------------------------------------------------------------------------------------------------------------
         COSTRUCT A FILTERSTRING FOR GEOMETRIES
 
         multipolygon and collections are not supported by ST_Within so they need to be split into several geometries
         this function converts geometries into a string usable as a raw sql query
         if no request is given, it will take the geometry from the cache
 
@@ -784,28 +883,70 @@
         second, the list is converted to a string
     ---------------------------------------------------------------------------------------------------------------------'''
 
     def get_geom_filterstring(self, geojson):
 
         geos_geometries = self.convert_geojson_to_geos(geojson)
 
-        geomfilterstring = ''
+        return self.get_geom_filter_string_from_geos(geos_geometries)
+
 
-        geomfilterstring += '('
+    def get_geom_filter_string_from_geos(self, geos_geometries):
+
+        geomfilterstring = '('
 
         for counter, geos in enumerate(geos_geometries):
             if counter > 0:
                 geomfilterstring += ' OR '
+                
             geomfilterstring += " ST_Intersects({geo_column}, ST_GeometryFromText('{geometry}', {srid}) ) ".format(
                 geo_column=geo_column_str, geometry=geos.wkt, srid=self.db_srid)
 
         geomfilterstring += ')'
 
         return geomfilterstring
 
+
+    '''---------------------------------------------------------------------------------------------------------------------
+        get non-cell-based geometries, eg fr cointing and grouping
+    ---------------------------------------------------------------------------------------------------------------------'''
+    # return a list of geometries
+    def get_geometries_for_counting(self, geojson, geometry_type, zoom):
+
+        geos_geometries = self.convert_geojson_to_geos(geojson)
+
+        if geometry_type == GEOMETRY_TYPE_VIEWPORT:
+            snapped_viewport = self.snap_viewport_to_grid(geos_geometries, zoom)
+            geometries_for_counting = [snapped_viewport]
+        else:
+            geometries_for_counting = geos_geometries
+
+        return geometries_for_counting
+
+
+    def snap_viewport_to_grid(self, geos_geometries, zoom):
+
+        srid = geos_geometries[0].srid
+
+        viewport_geometry = GeometryCollection(*geos_geometries, srid=srid)
+
+        envelope = viewport_geometry.envelope
+        
+        cells = self.rectangle_to_clustercells(envelope, zoom)
+
+        first_cell = cells[0]
+        last_cell = cells[-1]
+
+        cells = GeometryCollection(first_cell, last_cell, srid=viewport_geometry.srid)
+
+        grid_rectangle = cells.envelope
+
+        return grid_rectangle
+
+
     '''---------------------------------------------------------------------------------------------------------------------
         K Calculation
 
         this is only used for strict geometries, such as drawn polygons or drawn circles
         based on the BASE_K in the settings (defaults to 6) it increases the k if one draws a big shape
     ---------------------------------------------------------------------------------------------------------------------'''
     # k calculation has to be done on square-pixel areas
```

### Comparing `anycluster-2.1.1/anycluster/MapTools.py` & `anycluster-2.2.0/anycluster/MapTools.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/api/__pycache__/json_schemas.cpython-38.pyc` & `anycluster-2.2.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc` & `anycluster-2.2.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/api/__pycache__/serializers.cpython-38.pyc` & `anycluster-2.2.0/anycluster/api/__pycache__/serializers.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri May 19 13:08:27 2023 UTC, .py size: 2739 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,166 +1,206 @@
-00000000: 550d 0d0a 0000 0000 cb74 6764 b30a 0000  U........tgd....
+00000000: 550d 0d0a 0000 0000 5074 7064 e50c 0000  U.......Ptpd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
+00000020: 0004 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6404  m.Z...d.d.l.Z.d.
 00000050: 6405 6c05 6d06 5a06 0100 6400 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6407 6408 8400  m.Z.m.Z...d.d...
 00000070: 5a0a 4700 6409 640a 8400 640a 6503 6a0b  Z.G.d.d...d.e.j.
-00000080: 8303 5a0c 4700 640b 640c 8400 640c 6503  ..Z.G.d.d...d.e.
-00000090: 6a0b 8303 5a0d 6403 5300 290d e900 0000  j...Z.d.S.).....
-000000a0: 0029 01da 0873 6574 7469 6e67 7329 01da  .)...settings)..
-000000b0: 0b73 6572 6961 6c69 7a65 7273 4ee9 0100  .serializersN...
-000000c0: 0000 2901 da23 4645 4154 5552 455f 4f52  ..)..#FEATURE_OR
-000000d0: 5f46 4541 5455 5245 434f 4c4c 4543 5449  _FEATURECOLLECTI
-000000e0: 4f4e 5f53 4348 454d 4129 02da 0e47 454f  ON_SCHEMA)...GEO
-000000f0: 4d45 5452 595f 5459 5045 53da 1647 454f  METRY_TYPES..GEO
-00000100: 4d45 5452 595f 5459 5045 5f56 4945 5750  METRY_TYPE_VIEWP
-00000110: 4f52 5463 0100 0000 0000 0000 0000 0000  ORTc............
-00000120: 0400 0000 0600 0000 4300 0000 7360 0000  ........C...s`..
-00000130: 007c 0044 005d 567d 0164 017c 016b 067d  .|.D.]V}.d.|.k.}
-00000140: 027c 0264 026b 0272 4e7c 01a0 0064 0364  .|.d.k.rN|...d.d
-00000150: 00a1 027d 037c 0373 3274 01a0 0264 04a1  ...}.|.s2t...d..
-00000160: 0182 017c 0374 036a 046b 0772 5a74 01a0  ...|.t.j.k.rZt..
-00000170: 0264 05a0 057c 03a1 01a1 0182 0171 0474  .d...|.......q.t
-00000180: 067c 0164 0119 0083 0101 0071 0464 0053  .|.d.......q.d.S
-00000190: 0029 064e da07 6669 6c74 6572 7346 da06  .).N..filtersF..
-000001a0: 636f 6c75 6d6e 7a17 4669 6c74 6572 2072  columnz.Filter r
-000001b0: 6571 7569 7265 2061 2063 6f6c 756d 6e7a  equire a columnz
-000001c0: 2649 7420 6973 206e 6f74 2061 6c6c 6f77  &It is not allow
-000001d0: 6564 2074 6f20 6669 6c74 6572 2043 6f6c  ed to filter Col
-000001e0: 756d 6e20 7b30 7d29 07da 0367 6574 7203  umn {0})...getr.
-000001f0: 0000 00da 0f56 616c 6964 6174 696f 6e45  .....ValidationE
-00000200: 7272 6f72 7202 0000 00da 1241 4e59 434c  rrorr......ANYCL
-00000210: 5553 5445 525f 4649 4c54 4552 53da 0666  USTER_FILTERS..f
-00000220: 6f72 6d61 74da 1366 696c 7465 7273 5f61  ormat..filters_a
-00000230: 7265 5f61 6c6c 6f77 6564 2904 7208 0000  re_allowed).r...
-00000240: 00da 0666 696c 7465 72da 0969 735f 6e65  ...filter..is_ne
-00000250: 7374 6564 7209 0000 00a9 0072 1100 0000  stedr......r....
-00000260: fa3e 2f68 6f6d 652f 746f 6d2f 616e 7963  .>/home/tom/anyc
-00000270: 6c75 7374 6572 2f64 656d 6f2f 646a 616e  luster/demo/djan
-00000280: 676f 2f61 6e79 636c 7573 7465 722f 6170  go/anycluster/ap
-00000290: 692f 7365 7269 616c 697a 6572 732e 7079  i/serializers.py
-000002a0: 720e 0000 000b 0000 0073 1200 0000 0002  r........s......
-000002b0: 0802 0802 0801 0c01 0401 0a02 0a01 1203  ................
-000002c0: 720e 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000002d0: 0000 0000 0000 0500 0000 4000 0000 736e  ..........@...sn
-000002e0: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
-000002f0: 0164 0264 0364 048d 035a 0565 036a 0665  .d.d.d...Z.e.j.e
-00000300: 0764 0364 058d 025a 0865 036a 0964 0364  .d.d...Z.e.j.d.d
-00000310: 068d 015a 0a65 036a 0b64 0267 0064 0364  ...Z.e.j.d.g.d.d
-00000320: 078d 035a 0c65 036a 0d64 0264 0264 0364  ...Z.e.j.d.d.d.d
-00000330: 048d 035a 0e64 0864 0984 005a 0f64 0a64  ...Z.d.d...Z.d.d
-00000340: 0b84 005a 1064 0c64 0d84 005a 1164 0e53  ...Z.d.d...Z.d.S
-00000350: 0029 0fda 1843 6c75 7374 6572 5265 7175  .)...ClusterRequ
-00000360: 6573 7453 6572 6961 6c69 7a65 72fa 0945  estSerializer..E
-00000370: 5053 473a 3433 3236 4654 a903 da07 6465  PSG:4326FT....de
-00000380: 6661 756c 74da 0872 6571 7569 7265 64da  fault..required.
-00000390: 0a77 7269 7465 5f6f 6e6c 79a9 02da 0763  .write_only....c
-000003a0: 686f 6963 6573 7218 0000 00a9 0172 1800  hoicesr......r..
-000003b0: 0000 a903 7217 0000 0072 1600 0000 7218  ....r....r....r.
-000003c0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000003d0: 0400 0000 0300 0000 4300 0000 733e 0000  ........C...s>..
-000003e0: 007c 0164 0119 0074 006b 0272 3a7c 0164  .|.d...t.k.r:|.d
-000003f0: 0219 007d 027c 0264 0319 0064 0419 0064  ...}.|.d...d...d
-00000400: 0519 007d 0374 017c 0383 0164 066b 0273  ...}.t.|...d.k.s
-00000410: 3a74 02a0 0364 07a1 0182 017c 0153 0029  :t...d.....|.S.)
-00000420: 084e da0d 6765 6f6d 6574 7279 5f74 7970  .N..geometry_typ
-00000430: 65da 0767 656f 6a73 6f6e da08 6765 6f6d  e..geojson..geom
-00000440: 6574 7279 da0b 636f 6f72 6469 6e61 7465  etry..coordinate
-00000450: 7372 0100 0000 e905 0000 007a 2156 6965  sr.........z!Vie
-00000460: 7770 6f72 7420 6d75 7374 2063 6f6e 7369  wport must consi
-00000470: 7374 206f 6620 3520 706f 696e 7473 2904  st of 5 points).
-00000480: 7207 0000 00da 036c 656e 7203 0000 0072  r......lenr....r
-00000490: 0b00 0000 2904 da04 7365 6c66 da04 6461  ....)...self..da
-000004a0: 7461 721e 0000 0072 2000 0000 7211 0000  tar....r ...r...
-000004b0: 0072 1100 0000 7212 0000 00da 0876 616c  .r....r......val
-000004c0: 6964 6174 6529 0000 0073 0c00 0000 0001  idate)...s......
-000004d0: 0c02 0801 1001 0c01 0a02 7a21 436c 7573  ..........z!Clus
-000004e0: 7465 7252 6571 7565 7374 5365 7269 616c  terRequestSerial
-000004f0: 697a 6572 2e76 616c 6964 6174 6563 0200  izer.validatec..
-00000500: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
-00000510: 0000 4300 0000 7348 0000 007a 1074 00a0  ..C...sH...z.t..
-00000520: 017c 0174 02a1 027d 0257 006e 3204 0074  .|.t...}.W.n2..t
-00000530: 006a 036a 046b 0a72 4201 007d 0301 007a  .j.j.k.rB..}...z
-00000540: 1074 05a0 047c 036a 06a1 0182 0157 0035  .t...|.j.....W.5
-00000550: 0064 007d 037e 0358 0059 006e 0258 007c  .d.}.~.X.Y.n.X.|
-00000560: 0153 00a9 014e 2907 da0a 6a73 6f6e 7363  .S...N)...jsonsc
-00000570: 6865 6d61 7225 0000 0072 0500 0000 da0a  hemar%...r......
-00000580: 6578 6365 7074 696f 6e73 720b 0000 0072  exceptionsr....r
-00000590: 0300 0000 da07 6d65 7373 6167 6529 0472  ......message).r
-000005a0: 2300 0000 da05 7661 6c75 65da 0869 735f  #.....value..is_
-000005b0: 7661 6c69 64da 0165 7211 0000 0072 1100  valid..er....r..
-000005c0: 0000 7212 0000 00da 1076 616c 6964 6174  ..r......validat
-000005d0: 655f 6765 6f6a 736f 6e34 0000 0073 0a00  e_geojson4...s..
-000005e0: 0000 0001 0201 1001 1401 1e01 7a29 436c  ............z)Cl
-000005f0: 7573 7465 7252 6571 7565 7374 5365 7269  usterRequestSeri
-00000600: 616c 697a 6572 2e76 616c 6964 6174 655f  alizer.validate_
-00000610: 6765 6f6a 736f 6e63 0200 0000 0000 0000  geojsonc........
-00000620: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00000630: 730c 0000 0074 007c 0183 0101 007c 0153  s....t.|.....|.S
-00000640: 0072 2600 0000 a901 720e 0000 00a9 0272  .r&.....r......r
-00000650: 2300 0000 722a 0000 0072 1100 0000 7211  #...r*...r....r.
-00000660: 0000 0072 1200 0000 da10 7661 6c69 6461  ...r......valida
-00000670: 7465 5f66 696c 7465 7273 3b00 0000 7304  te_filters;...s.
-00000680: 0000 0000 0108 017a 2943 6c75 7374 6572  .......z)Cluster
-00000690: 5265 7175 6573 7453 6572 6961 6c69 7a65  RequestSerialize
-000006a0: 722e 7661 6c69 6461 7465 5f66 696c 7465  r.validate_filte
-000006b0: 7273 4e29 12da 085f 5f6e 616d 655f 5fda  rsN)...__name__.
-000006c0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000006d0: 7561 6c6e 616d 655f 5f72 0300 0000 da09  ualname__r......
-000006e0: 4368 6172 4669 656c 64da 0b6f 7574 7075  CharField..outpu
-000006f0: 745f 7372 6964 da0b 4368 6f69 6365 4669  t_srid..ChoiceFi
-00000700: 656c 6472 0600 0000 721d 0000 00da 094a  eldr....r......J
-00000710: 534f 4e46 6965 6c64 721e 0000 00da 094c  SONFieldr......L
-00000720: 6973 7446 6965 6c64 7208 0000 00da 0c42  istFieldr......B
-00000730: 6f6f 6c65 616e 4669 656c 64da 0b63 6c65  ooleanField..cle
-00000740: 6172 5f63 6163 6865 7225 0000 0072 2d00  ar_cacher%...r-.
-00000750: 0000 7230 0000 0072 1100 0000 7211 0000  ..r0...r....r...
-00000760: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000770: 1d00 0000 7310 0000 0008 0210 020e 020c  ....s...........
-00000780: 0110 0210 0308 0b08 0772 1300 0000 6300  .........r....c.
-00000790: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-000007a0: 0000 0040 0000 0073 7c00 0000 6500 5a01  ...@...s|...e.Z.
-000007b0: 6400 5a02 6503 6a04 6401 6402 6403 6404  d.Z.e.j.d.d.d.d.
-000007c0: 8d03 5a05 6503 6a04 6401 6402 6403 6404  ..Z.e.j.d.d.d.d.
-000007d0: 8d03 5a06 6503 6a07 6508 6403 6405 8d02  ..Z.e.j.e.d.d...
-000007e0: 5a09 6503 6a0a 6503 a00b a100 6403 6406  Z.e.j.e.....d.d.
-000007f0: 8d02 5a0c 6503 6a0d 6403 6407 8d01 5a0e  ..Z.e.j.d.d...Z.
-00000800: 6503 6a0d 6403 6407 8d01 5a0f 6503 6a0a  e.j.d.d...Z.e.j.
-00000810: 6402 6700 6403 6408 8d03 5a10 6409 640a  d.g.d.d...Z.d.d.
-00000820: 8400 5a11 640b 5300 290c da1f 436c 7573  ..Z.d.S.)...Clus
-00000830: 7465 7243 6f6e 7465 6e74 5265 7175 6573  terContentReques
-00000840: 7453 6572 6961 6c69 7a65 7272 1400 0000  tSerializerr....
-00000850: 4654 7215 0000 0072 1900 0000 2902 da05  FTr....r....)...
-00000860: 6368 696c 6472 1800 0000 721b 0000 0072  childr....r....r
-00000870: 1c00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000880: 0002 0000 0002 0000 0043 0000 0073 0c00  .........C...s..
-00000890: 0000 7400 7c01 8301 0100 7c01 5300 7226  ..t.|.....|.S.r&
-000008a0: 0000 0072 2e00 0000 722f 0000 0072 1100  ...r....r/...r..
-000008b0: 0000 7211 0000 0072 1200 0000 7230 0000  ..r....r....r0..
-000008c0: 004c 0000 0073 0400 0000 0001 0801 7a30  .L...s........z0
-000008d0: 436c 7573 7465 7243 6f6e 7465 6e74 5265  ClusterContentRe
-000008e0: 7175 6573 7453 6572 6961 6c69 7a65 722e  questSerializer.
-000008f0: 7661 6c69 6461 7465 5f66 696c 7465 7273  validate_filters
-00000900: 4e29 1272 3100 0000 7232 0000 0072 3300  N).r1...r2...r3.
-00000910: 0000 7203 0000 0072 3400 0000 7235 0000  ..r....r4...r5..
-00000920: 00da 0a69 6e70 7574 5f73 7269 6472 3600  ...input_sridr6.
-00000930: 0000 7206 0000 0072 1d00 0000 7238 0000  ..r....r....r8..
-00000940: 00da 0c49 6e74 6567 6572 4669 656c 64da  ...IntegerField.
-00000950: 0369 6473 da0a 466c 6f61 7446 6965 6c64  .ids..FloatField
-00000960: da01 78da 0179 7208 0000 0072 3000 0000  ..x..yr....r0...
-00000970: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000980: 1200 0000 723b 0000 0040 0000 0073 1000  ....r;...@...s..
-00000990: 0000 0802 1001 1002 0e02 1201 0c01 0c01  ................
-000009a0: 1002 723b 0000 0029 0eda 0b64 6a61 6e67  ..r;...)...djang
-000009b0: 6f2e 636f 6e66 7202 0000 00da 0e72 6573  o.confr......res
-000009c0: 745f 6672 616d 6577 6f72 6b72 0300 0000  t_frameworkr....
-000009d0: 7227 0000 005a 0c6a 736f 6e5f 7363 6865  r'...Z.json_sche
-000009e0: 6d61 7372 0500 0000 da16 616e 7963 6c75  masr......anyclu
-000009f0: 7374 6572 2e64 6566 696e 6974 696f 6e73  ster.definitions
-00000a00: 7206 0000 0072 0700 0000 720e 0000 00da  r....r....r.....
-00000a10: 0a53 6572 6961 6c69 7a65 7272 1300 0000  .Serializerr....
-00000a20: 723b 0000 0072 1100 0000 7211 0000 0072  r;...r....r....r
-00000a30: 1100 0000 7212 0000 00da 083c 6d6f 6475  ....r......<modu
-00000a40: 6c65 3e01 0000 0073 0e00 0000 0c01 0c02  le>....s........
-00000a50: 0802 0c02 1003 0812 1223                 .........#
+00000080: 8303 5a0c 4700 640b 640c 8400 640c 650c  ..Z.G.d.d...d.e.
+00000090: 8303 5a0d 4700 640d 640e 8400 640e 650c  ..Z.G.d.d...d.e.
+000000a0: 8303 5a0e 4700 640f 6410 8400 6410 6503  ..Z.G.d.d...d.e.
+000000b0: 6a0b 8303 5a0f 6403 5300 2911 e900 0000  j...Z.d.S.).....
+000000c0: 0029 01da 0873 6574 7469 6e67 7329 01da  .)...settings)..
+000000d0: 0b73 6572 6961 6c69 7a65 7273 4ee9 0100  .serializersN...
+000000e0: 0000 2901 da23 4645 4154 5552 455f 4f52  ..)..#FEATURE_OR
+000000f0: 5f46 4541 5455 5245 434f 4c4c 4543 5449  _FEATURECOLLECTI
+00000100: 4f4e 5f53 4348 454d 4129 02da 0e47 454f  ON_SCHEMA)...GEO
+00000110: 4d45 5452 595f 5459 5045 53da 1647 454f  METRY_TYPES..GEO
+00000120: 4d45 5452 595f 5459 5045 5f56 4945 5750  METRY_TYPE_VIEWP
+00000130: 4f52 5463 0100 0000 0000 0000 0000 0000  ORTc............
+00000140: 0400 0000 0600 0000 4300 0000 7360 0000  ........C...s`..
+00000150: 007c 0044 005d 567d 0164 017c 016b 067d  .|.D.]V}.d.|.k.}
+00000160: 027c 0264 026b 0272 4e7c 01a0 0064 0364  .|.d.k.rN|...d.d
+00000170: 00a1 027d 037c 0373 3274 01a0 0264 04a1  ...}.|.s2t...d..
+00000180: 0182 017c 0374 036a 046b 0772 5a74 01a0  ...|.t.j.k.rZt..
+00000190: 0264 05a0 057c 03a1 01a1 0182 0171 0474  .d...|.......q.t
+000001a0: 067c 0164 0119 0083 0101 0071 0464 0053  .|.d.......q.d.S
+000001b0: 0029 064e da07 6669 6c74 6572 7346 da06  .).N..filtersF..
+000001c0: 636f 6c75 6d6e 7a17 4669 6c74 6572 2072  columnz.Filter r
+000001d0: 6571 7569 7265 2061 2063 6f6c 756d 6e7a  equire a columnz
+000001e0: 2649 7420 6973 206e 6f74 2061 6c6c 6f77  &It is not allow
+000001f0: 6564 2074 6f20 6669 6c74 6572 2043 6f6c  ed to filter Col
+00000200: 756d 6e20 7b30 7d29 07da 0367 6574 7203  umn {0})...getr.
+00000210: 0000 00da 0f56 616c 6964 6174 696f 6e45  .....ValidationE
+00000220: 7272 6f72 7202 0000 00da 1241 4e59 434c  rrorr......ANYCL
+00000230: 5553 5445 525f 4649 4c54 4552 53da 0666  USTER_FILTERS..f
+00000240: 6f72 6d61 74da 1366 696c 7465 7273 5f61  ormat..filters_a
+00000250: 7265 5f61 6c6c 6f77 6564 2904 7208 0000  re_allowed).r...
+00000260: 00da 0666 696c 7465 72da 0969 735f 6e65  ...filter..is_ne
+00000270: 7374 6564 7209 0000 00a9 0072 1100 0000  stedr......r....
+00000280: fa3e 2f68 6f6d 652f 746f 6d2f 616e 7963  .>/home/tom/anyc
+00000290: 6c75 7374 6572 2f64 656d 6f2f 646a 616e  luster/demo/djan
+000002a0: 676f 2f61 6e79 636c 7573 7465 722f 6170  go/anycluster/ap
+000002b0: 692f 7365 7269 616c 697a 6572 732e 7079  i/serializers.py
+000002c0: 720e 0000 000b 0000 0073 1200 0000 0002  r........s......
+000002d0: 0802 0802 0801 0c01 0401 0a02 0a01 1203  ................
+000002e0: 720e 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000002f0: 0000 0000 0000 0500 0000 4000 0000 736e  ..........@...sn
+00000300: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
+00000310: 0164 0264 0364 048d 035a 0565 036a 0665  .d.d.d...Z.e.j.e
+00000320: 0764 0364 058d 025a 0865 036a 0964 0364  .d.d...Z.e.j.d.d
+00000330: 068d 015a 0a65 036a 0b64 0267 0064 0364  ...Z.e.j.d.g.d.d
+00000340: 078d 035a 0c65 036a 0d64 0264 0264 0364  ...Z.e.j.d.d.d.d
+00000350: 048d 035a 0e64 0864 0984 005a 0f64 0a64  ...Z.d.d...Z.d.d
+00000360: 0b84 005a 1064 0c64 0d84 005a 1164 0e53  ...Z.d.d...Z.d.S
+00000370: 0029 0fda 1843 6c75 7374 6572 5265 7175  .)...ClusterRequ
+00000380: 6573 7453 6572 6961 6c69 7a65 72fa 0945  estSerializer..E
+00000390: 5053 473a 3433 3236 4654 a903 da07 6465  PSG:4326FT....de
+000003a0: 6661 756c 74da 0872 6571 7569 7265 64da  fault..required.
+000003b0: 0a77 7269 7465 5f6f 6e6c 79a9 02da 0763  .write_only....c
+000003c0: 686f 6963 6573 7218 0000 00a9 0172 1800  hoicesr......r..
+000003d0: 0000 a903 7217 0000 0072 1600 0000 7218  ....r....r....r.
+000003e0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000003f0: 0400 0000 0300 0000 4300 0000 733e 0000  ........C...s>..
+00000400: 007c 0164 0119 0074 006b 0272 3a7c 0164  .|.d...t.k.r:|.d
+00000410: 0219 007d 027c 0264 0319 0064 0419 0064  ...}.|.d...d...d
+00000420: 0519 007d 0374 017c 0383 0164 066b 0273  ...}.t.|...d.k.s
+00000430: 3a74 02a0 0364 07a1 0182 017c 0153 0029  :t...d.....|.S.)
+00000440: 084e da0d 6765 6f6d 6574 7279 5f74 7970  .N..geometry_typ
+00000450: 65da 0767 656f 6a73 6f6e da08 6765 6f6d  e..geojson..geom
+00000460: 6574 7279 da0b 636f 6f72 6469 6e61 7465  etry..coordinate
+00000470: 7372 0100 0000 e905 0000 007a 2156 6965  sr.........z!Vie
+00000480: 7770 6f72 7420 6d75 7374 2063 6f6e 7369  wport must consi
+00000490: 7374 206f 6620 3520 706f 696e 7473 2904  st of 5 points).
+000004a0: 7207 0000 00da 036c 656e 7203 0000 0072  r......lenr....r
+000004b0: 0b00 0000 2904 da04 7365 6c66 da04 6461  ....)...self..da
+000004c0: 7461 721e 0000 0072 2000 0000 7211 0000  tar....r ...r...
+000004d0: 0072 1100 0000 7212 0000 00da 0876 616c  .r....r......val
+000004e0: 6964 6174 6529 0000 0073 0c00 0000 0001  idate)...s......
+000004f0: 0c02 0801 1001 0c01 0a02 7a21 436c 7573  ..........z!Clus
+00000500: 7465 7252 6571 7565 7374 5365 7269 616c  terRequestSerial
+00000510: 697a 6572 2e76 616c 6964 6174 6563 0200  izer.validatec..
+00000520: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
+00000530: 0000 4300 0000 7348 0000 007a 1074 00a0  ..C...sH...z.t..
+00000540: 017c 0174 02a1 027d 0257 006e 3204 0074  .|.t...}.W.n2..t
+00000550: 006a 036a 046b 0a72 4201 007d 0301 007a  .j.j.k.rB..}...z
+00000560: 1074 05a0 047c 036a 06a1 0182 0157 0035  .t...|.j.....W.5
+00000570: 0064 007d 037e 0358 0059 006e 0258 007c  .d.}.~.X.Y.n.X.|
+00000580: 0153 00a9 014e 2907 da0a 6a73 6f6e 7363  .S...N)...jsonsc
+00000590: 6865 6d61 7225 0000 0072 0500 0000 da0a  hemar%...r......
+000005a0: 6578 6365 7074 696f 6e73 720b 0000 0072  exceptionsr....r
+000005b0: 0300 0000 da07 6d65 7373 6167 6529 0472  ......message).r
+000005c0: 2300 0000 da05 7661 6c75 65da 0869 735f  #.....value..is_
+000005d0: 7661 6c69 64da 0165 7211 0000 0072 1100  valid..er....r..
+000005e0: 0000 7212 0000 00da 1076 616c 6964 6174  ..r......validat
+000005f0: 655f 6765 6f6a 736f 6e34 0000 0073 0a00  e_geojson4...s..
+00000600: 0000 0001 0201 1001 1401 1e01 7a29 436c  ............z)Cl
+00000610: 7573 7465 7252 6571 7565 7374 5365 7269  usterRequestSeri
+00000620: 616c 697a 6572 2e76 616c 6964 6174 655f  alizer.validate_
+00000630: 6765 6f6a 736f 6e63 0200 0000 0000 0000  geojsonc........
+00000640: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00000650: 730c 0000 0074 007c 0183 0101 007c 0153  s....t.|.....|.S
+00000660: 0072 2600 0000 a901 720e 0000 00a9 0272  .r&.....r......r
+00000670: 2300 0000 722a 0000 0072 1100 0000 7211  #...r*...r....r.
+00000680: 0000 0072 1200 0000 da10 7661 6c69 6461  ...r......valida
+00000690: 7465 5f66 696c 7465 7273 3b00 0000 7304  te_filters;...s.
+000006a0: 0000 0000 0108 017a 2943 6c75 7374 6572  .......z)Cluster
+000006b0: 5265 7175 6573 7453 6572 6961 6c69 7a65  RequestSerialize
+000006c0: 722e 7661 6c69 6461 7465 5f66 696c 7465  r.validate_filte
+000006d0: 7273 4e29 12da 085f 5f6e 616d 655f 5fda  rsN)...__name__.
+000006e0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000006f0: 7561 6c6e 616d 655f 5f72 0300 0000 da09  ualname__r......
+00000700: 4368 6172 4669 656c 64da 0b6f 7574 7075  CharField..outpu
+00000710: 745f 7372 6964 da0b 4368 6f69 6365 4669  t_srid..ChoiceFi
+00000720: 656c 6472 0600 0000 721d 0000 00da 094a  eldr....r......J
+00000730: 534f 4e46 6965 6c64 721e 0000 00da 094c  SONFieldr......L
+00000740: 6973 7446 6965 6c64 7208 0000 00da 0c42  istFieldr......B
+00000750: 6f6f 6c65 616e 4669 656c 64da 0b63 6c65  ooleanField..cle
+00000760: 6172 5f63 6163 6865 7225 0000 0072 2d00  ar_cacher%...r-.
+00000770: 0000 7230 0000 0072 1100 0000 7211 0000  ..r0...r....r...
+00000780: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000790: 1d00 0000 7310 0000 0008 0210 020e 020c  ....s...........
+000007a0: 0110 0210 0308 0b08 0772 1300 0000 6300  .........r....c.
+000007b0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+000007c0: 0000 0040 0000 0073 2400 0000 6500 5a01  ...@...s$...e.Z.
+000007d0: 6400 5a02 6503 6a04 6401 6900 6402 6403  d.Z.e.j.d.i.d.d.
+000007e0: 8d03 5a05 6404 6405 8400 5a06 6406 5300  ..Z.d.d...Z.d.S.
+000007f0: 2907 da19 4d61 7043 6f6e 7465 6e74 436f  )...MapContentCo
+00000800: 756e 7453 6572 6961 6c69 7a65 7246 5472  untSerializerFTr
+00000810: 1c00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000820: 0004 0000 0004 0000 0043 0000 0073 2600  .........C...s&.
+00000830: 0000 7c01 7222 7c01 a000 a100 4400 5d14  ..|.r"|.....D.].
+00000840: 5c02 7d02 7d03 7401 7c03 6401 1900 8301  \.}.}.t.|.d.....
+00000850: 0100 710c 7c01 5300 2902 4e72 0800 0000  ..q.|.S.).Nr....
+00000860: 2902 da05 6974 656d 7372 0e00 0000 2904  )...itemsr....).
+00000870: 7223 0000 0072 2a00 0000 da0f 6d6f 6475  r#...r*.....modu
+00000880: 6c61 7469 6f6e 5f6e 616d 655a 0a6d 6f64  lation_nameZ.mod
+00000890: 756c 6174 696f 6e72 1100 0000 7211 0000  ulationr....r...
+000008a0: 0072 1200 0000 da14 7661 6c69 6461 7465  .r......validate
+000008b0: 5f6d 6f64 756c 6174 696f 6e73 4400 0000  _modulationsD...
+000008c0: 7308 0000 0000 0204 0210 010e 027a 2e4d  s............z.M
+000008d0: 6170 436f 6e74 656e 7443 6f75 6e74 5365  apContentCountSe
+000008e0: 7269 616c 697a 6572 2e76 616c 6964 6174  rializer.validat
+000008f0: 655f 6d6f 6475 6c61 7469 6f6e 734e 2907  e_modulationsN).
+00000900: 7231 0000 0072 3200 0000 7233 0000 0072  r1...r2...r3...r
+00000910: 0300 0000 7237 0000 00da 0b6d 6f64 756c  ....r7.....modul
+00000920: 6174 696f 6e73 723e 0000 0072 1100 0000  ationsr>...r....
+00000930: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00000940: 3b00 0000 4000 0000 7304 0000 0008 0210  ;...@...s.......
+00000950: 0272 3b00 0000 6300 0000 0000 0000 0000  .r;...c.........
+00000960: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00000970: 1800 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
+00000980: 6401 6402 8d01 5a05 6403 5300 2904 da1b  d.d...Z.d.S.)...
+00000990: 4772 6f75 7065 644d 6170 436f 6e74 656e  GroupedMapConten
+000009a0: 7453 6572 6961 6c69 7a65 7254 721b 0000  tSerializerTr...
+000009b0: 004e 2906 7231 0000 0072 3200 0000 7233  .N).r1...r2...r3
+000009c0: 0000 0072 0300 0000 7234 0000 00da 0867  ...r....r4.....g
+000009d0: 726f 7570 5f62 7972 1100 0000 7211 0000  roup_byr....r...
+000009e0: 0072 1100 0000 7212 0000 0072 4000 0000  .r....r....r@...
+000009f0: 4e00 0000 7302 0000 0008 0172 4000 0000  N...s......r@...
+00000a00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000a10: 0005 0000 0040 0000 0073 7c00 0000 6500  .....@...s|...e.
+00000a20: 5a01 6400 5a02 6503 6a04 6401 6402 6403  Z.d.Z.e.j.d.d.d.
+00000a30: 6404 8d03 5a05 6503 6a04 6401 6402 6403  d...Z.e.j.d.d.d.
+00000a40: 6404 8d03 5a06 6503 6a07 6508 6403 6405  d...Z.e.j.e.d.d.
+00000a50: 8d02 5a09 6503 6a0a 6503 a00b a100 6403  ..Z.e.j.e.....d.
+00000a60: 6406 8d02 5a0c 6503 6a0d 6403 6407 8d01  d...Z.e.j.d.d...
+00000a70: 5a0e 6503 6a0d 6403 6407 8d01 5a0f 6503  Z.e.j.d.d...Z.e.
+00000a80: 6a0a 6402 6700 6403 6408 8d03 5a10 6409  j.d.g.d.d...Z.d.
+00000a90: 640a 8400 5a11 640b 5300 290c da1f 436c  d...Z.d.S.)...Cl
+00000aa0: 7573 7465 7243 6f6e 7465 6e74 5265 7175  usterContentRequ
+00000ab0: 6573 7453 6572 6961 6c69 7a65 7272 1400  estSerializerr..
+00000ac0: 0000 4654 7215 0000 0072 1900 0000 2902  ..FTr....r....).
+00000ad0: da05 6368 696c 6472 1800 0000 721b 0000  ..childr....r...
+00000ae0: 0072 1c00 0000 6302 0000 0000 0000 0000  .r....c.........
+00000af0: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00000b00: 0c00 0000 7400 7c01 8301 0100 7c01 5300  ....t.|.....|.S.
+00000b10: 7226 0000 0072 2e00 0000 722f 0000 0072  r&...r....r/...r
+00000b20: 1100 0000 7211 0000 0072 1200 0000 7230  ....r....r....r0
+00000b30: 0000 005e 0000 0073 0400 0000 0001 0801  ...^...s........
+00000b40: 7a30 436c 7573 7465 7243 6f6e 7465 6e74  z0ClusterContent
+00000b50: 5265 7175 6573 7453 6572 6961 6c69 7a65  RequestSerialize
+00000b60: 722e 7661 6c69 6461 7465 5f66 696c 7465  r.validate_filte
+00000b70: 7273 4e29 1272 3100 0000 7232 0000 0072  rsN).r1...r2...r
+00000b80: 3300 0000 7203 0000 0072 3400 0000 7235  3...r....r4...r5
+00000b90: 0000 00da 0a69 6e70 7574 5f73 7269 6472  .....input_sridr
+00000ba0: 3600 0000 7206 0000 0072 1d00 0000 7238  6...r....r....r8
+00000bb0: 0000 00da 0c49 6e74 6567 6572 4669 656c  .....IntegerFiel
+00000bc0: 64da 0369 6473 da0a 466c 6f61 7446 6965  d..ids..FloatFie
+00000bd0: 6c64 da01 78da 0179 7208 0000 0072 3000  ld..x..yr....r0.
+00000be0: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
+00000bf0: 0072 1200 0000 7242 0000 0052 0000 0073  .r....rB...R...s
+00000c00: 1000 0000 0802 1001 1002 0e02 1201 0c01  ................
+00000c10: 0c01 1002 7242 0000 0029 10da 0b64 6a61  ....rB...)...dja
+00000c20: 6e67 6f2e 636f 6e66 7202 0000 00da 0e72  ngo.confr......r
+00000c30: 6573 745f 6672 616d 6577 6f72 6b72 0300  est_frameworkr..
+00000c40: 0000 7227 0000 005a 0c6a 736f 6e5f 7363  ..r'...Z.json_sc
+00000c50: 6865 6d61 7372 0500 0000 da16 616e 7963  hemasr......anyc
+00000c60: 6c75 7374 6572 2e64 6566 696e 6974 696f  luster.definitio
+00000c70: 6e73 7206 0000 0072 0700 0000 720e 0000  nsr....r....r...
+00000c80: 00da 0a53 6572 6961 6c69 7a65 7272 1300  ...Serializerr..
+00000c90: 0000 723b 0000 0072 4000 0000 7242 0000  ..r;...r@...rB..
+00000ca0: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
+00000cb0: 7212 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000cc0: 0000 0073 1200 0000 0c01 0c02 0802 0c02  ...s............
+00000cd0: 1003 0812 1223 100e 1004                 .....#....
```

### Comparing `anycluster-2.1.1/anycluster/api/__pycache__/urls.cpython-38.pyc` & `anycluster-2.2.0/anycluster/api/__pycache__/urls.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Apr 24 12:47:36 2023 UTC, .py size: 882 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,75 @@
-00000000: 550d 0d0a 0000 0000 687a 4664 7203 0000  U.......hzFdr...
+00000000: 550d 0d0a 0000 0000 bf6f 7064 8d04 0000  U........opd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000a 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
+00000020: 000c 0000 0040 0000 0073 ca00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6501 6405 6505 6a06 a007 a100 6406  ..e.d.e.j.....d.
 00000060: 6407 8d03 6501 6408 6505 6a08 a007 a100  d...e.d.e.j.....
 00000070: 6409 6407 8d03 6501 640a 6505 6a09 a007  d.d...e.d.e.j...
 00000080: a100 640b 6407 8d03 6501 640c 6505 6a0a  ..d.d...e.d.e.j.
 00000090: a007 a100 640d 6407 8d03 6501 640e 6505  ....d.d...e.d.e.
 000000a0: 6a0b a007 a100 640f 6407 8d03 6501 6410  j.....d.d...e.d.
-000000b0: 6505 6a0c a007 a100 6411 6407 8d03 6706  e.j.....d.d...g.
-000000c0: 5a0d 6503 650d 6412 6701 6413 8d02 5a0d  Z.e.e.d.g.d...Z.
-000000d0: 6414 5300 2915 e900 0000 0029 01da 0470  d.S.)......)...p
-000000e0: 6174 6829 01da 1666 6f72 6d61 745f 7375  ath)...format_su
-000000f0: 6666 6978 5f70 6174 7465 726e 73e9 0100  ffix_patterns...
-00000100: 0000 2901 da05 7669 6577 73da 005a 1361  ..)...views..Z.a
-00000110: 6e79 636c 7573 7465 725f 6170 695f 686f  nycluster_api_ho
-00000120: 6d65 2901 da04 6e61 6d65 7a20 6772 6964  me)...namez grid
-00000130: 2f3c 696e 743a 7a6f 6f6d 3e2f 3c69 6e74  /<int:zoom>/<int
-00000140: 3a67 7269 645f 7369 7a65 3e2f da0c 6772  :grid_size>/..gr
-00000150: 6964 5f63 6c75 7374 6572 7a22 6b6d 6561  id_clusterz"kmea
-00000160: 6e73 2f3c 696e 743a 7a6f 6f6d 3e2f 3c69  ns/<int:zoom>/<i
-00000170: 6e74 3a67 7269 645f 7369 7a65 3e2f da0e  nt:grid_size>/..
-00000180: 6b6d 6561 6e73 5f63 6c75 7374 6572 7a36  kmeans_clusterz6
-00000190: 6765 742d 6b6d 6561 6e73 2d63 6c75 7374  get-kmeans-clust
-000001a0: 6572 2d63 6f6e 7465 6e74 2f3c 696e 743a  er-content/<int:
-000001b0: 7a6f 6f6d 3e2f 3c69 6e74 3a67 7269 645f  zoom>/<int:grid_
-000001c0: 7369 7a65 3e2f da1a 6765 745f 6b6d 6561  size>/..get_kmea
-000001d0: 6e73 5f63 6c75 7374 6572 5f63 6f6e 7465  ns_cluster_conte
-000001e0: 6e74 7a2c 6765 742d 6172 6561 2d63 6f6e  ntz,get-area-con
-000001f0: 7465 6e74 2f3c 696e 743a 7a6f 6f6d 3e2f  tent/<int:zoom>/
-00000200: 3c69 6e74 3a67 7269 645f 7369 7a65 3e2f  <int:grid_size>/
-00000210: da10 6765 745f 6172 6561 5f63 6f6e 7465  ..get_area_conte
-00000220: 6e74 7a40 6765 742d 6461 7461 7365 742d  ntz@get-dataset-
-00000230: 636f 6e74 656e 742f 3c69 6e74 3a7a 6f6f  content/<int:zoo
-00000240: 6d3e 2f3c 696e 743a 6772 6964 5f73 697a  m>/<int:grid_siz
-00000250: 653e 2f3c 696e 743a 6461 7461 7365 745f  e>/<int:dataset_
-00000260: 6964 3e2f da13 6765 745f 6461 7461 7365  id>/..get_datase
-00000270: 745f 636f 6e74 656e 74da 046a 736f 6e29  t_content..json)
-00000280: 01da 0761 6c6c 6f77 6564 4e29 0eda 0b64  ...allowedN)...d
-00000290: 6a61 6e67 6f2e 7572 6c73 7202 0000 005a  jango.urlsr....Z
-000002a0: 1a72 6573 745f 6672 616d 6577 6f72 6b2e  .rest_framework.
-000002b0: 7572 6c70 6174 7465 726e 7372 0300 0000  urlpatternsr....
-000002c0: 7206 0000 0072 0500 0000 da07 4150 4948  r....r......APIH
-000002d0: 6f6d 65da 0761 735f 7669 6577 da0b 4772  ome..as_view..Gr
-000002e0: 6964 436c 7573 7465 72da 0d4b 6d65 616e  idCluster..Kmean
-000002f0: 7343 6c75 7374 6572 da11 4765 7443 6c75  sCluster..GetClu
-00000300: 7374 6572 436f 6e74 656e 74da 0e47 6574  sterContent..Get
-00000310: 4172 6561 436f 6e74 656e 74da 1147 6574  AreaContent..Get
-00000320: 4461 7461 7365 7443 6f6e 7465 6e74 da0b  DatasetContent..
-00000330: 7572 6c70 6174 7465 726e 73a9 0072 1800  urlpatterns..r..
-00000340: 0000 7218 0000 00fa 372f 686f 6d65 2f74  ..r.....7/home/t
-00000350: 6f6d 2f61 6e79 636c 7573 7465 722f 6465  om/anycluster/de
-00000360: 6d6f 2f64 6a61 6e67 6f2f 616e 7963 6c75  mo/django/anyclu
-00000370: 7374 6572 2f61 7069 2f75 726c 732e 7079  ster/api/urls.py
-00000380: da08 3c6d 6f64 756c 653e 0100 0000 7320  ..<module>....s 
-00000390: 0000 000c 010c 020c 0312 0112 0112 010c  ................
-000003a0: 0102 ff04 020c 0102 ff04 020c 0102 ff04  ................
-000003b0: f804 0c                                  ...
+000000b0: 6505 6a0c a007 a100 6411 6407 8d03 6501  e.j.....d.d...e.
+000000c0: 6412 6505 6a0d a007 a100 6413 6407 8d03  d.e.j.....d.d...
+000000d0: 6501 6414 6505 6a0e a007 a100 6415 6407  e.d.e.j.....d.d.
+000000e0: 8d03 6708 5a0f 6503 650f 6416 6701 6417  ..g.Z.e.e.d.g.d.
+000000f0: 8d02 5a0f 6418 5300 2919 e900 0000 0029  ..Z.d.S.)......)
+00000100: 01da 0470 6174 6829 01da 1666 6f72 6d61  ...path)...forma
+00000110: 745f 7375 6666 6978 5f70 6174 7465 726e  t_suffix_pattern
+00000120: 73e9 0100 0000 2901 da05 7669 6577 73da  s.....)...views.
+00000130: 005a 1361 6e79 636c 7573 7465 725f 6170  .Z.anycluster_ap
+00000140: 695f 686f 6d65 2901 da04 6e61 6d65 7a20  i_home)...namez 
+00000150: 6772 6964 2f3c 696e 743a 7a6f 6f6d 3e2f  grid/<int:zoom>/
+00000160: 3c69 6e74 3a67 7269 645f 7369 7a65 3e2f  <int:grid_size>/
+00000170: da0c 6772 6964 5f63 6c75 7374 6572 7a22  ..grid_clusterz"
+00000180: 6b6d 6561 6e73 2f3c 696e 743a 7a6f 6f6d  kmeans/<int:zoom
+00000190: 3e2f 3c69 6e74 3a67 7269 645f 7369 7a65  >/<int:grid_size
+000001a0: 3e2f da0e 6b6d 6561 6e73 5f63 6c75 7374  >/..kmeans_clust
+000001b0: 6572 7a36 6765 742d 6b6d 6561 6e73 2d63  erz6get-kmeans-c
+000001c0: 6c75 7374 6572 2d63 6f6e 7465 6e74 2f3c  luster-content/<
+000001d0: 696e 743a 7a6f 6f6d 3e2f 3c69 6e74 3a67  int:zoom>/<int:g
+000001e0: 7269 645f 7369 7a65 3e2f da1a 6765 745f  rid_size>/..get_
+000001f0: 6b6d 6561 6e73 5f63 6c75 7374 6572 5f63  kmeans_cluster_c
+00000200: 6f6e 7465 6e74 7a2c 6765 742d 6172 6561  ontentz,get-area
+00000210: 2d63 6f6e 7465 6e74 2f3c 696e 743a 7a6f  -content/<int:zo
+00000220: 6f6d 3e2f 3c69 6e74 3a67 7269 645f 7369  om>/<int:grid_si
+00000230: 7a65 3e2f da10 6765 745f 6172 6561 5f63  ze>/..get_area_c
+00000240: 6f6e 7465 6e74 7a40 6765 742d 6461 7461  ontentz@get-data
+00000250: 7365 742d 636f 6e74 656e 742f 3c69 6e74  set-content/<int
+00000260: 3a7a 6f6f 6d3e 2f3c 696e 743a 6772 6964  :zoom>/<int:grid
+00000270: 5f73 697a 653e 2f3c 696e 743a 6461 7461  _size>/<int:data
+00000280: 7365 745f 6964 3e2f da13 6765 745f 6461  set_id>/..get_da
+00000290: 7461 7365 745f 636f 6e74 656e 747a 3167  taset_contentz1g
+000002a0: 6574 2d6d 6170 2d63 6f6e 7465 6e74 2d63  et-map-content-c
+000002b0: 6f75 6e74 2f3c 696e 743a 7a6f 6f6d 3e2f  ount/<int:zoom>/
+000002c0: 3c69 6e74 3a67 7269 645f 7369 7a65 3e2f  <int:grid_size>/
+000002d0: da15 6765 745f 6d61 705f 636f 6e74 656e  ..get_map_conten
+000002e0: 745f 636f 756e 747a 3467 6574 2d67 726f  t_countz4get-gro
+000002f0: 7570 6564 2d6d 6170 2d63 6f6e 7465 6e74  uped-map-content
+00000300: 732f 3c69 6e74 3a7a 6f6f 6d3e 2f3c 696e  s/<int:zoom>/<in
+00000310: 743a 6772 6964 5f73 697a 653e 2fda 1867  t:grid_size>/..g
+00000320: 6574 5f67 726f 7570 6564 5f6d 6170 5f63  et_grouped_map_c
+00000330: 6f6e 7465 6e74 73da 046a 736f 6e29 01da  ontents..json)..
+00000340: 0761 6c6c 6f77 6564 4e29 10da 0b64 6a61  .allowedN)...dja
+00000350: 6e67 6f2e 7572 6c73 7202 0000 005a 1a72  ngo.urlsr....Z.r
+00000360: 6573 745f 6672 616d 6577 6f72 6b2e 7572  est_framework.ur
+00000370: 6c70 6174 7465 726e 7372 0300 0000 7206  lpatternsr....r.
+00000380: 0000 0072 0500 0000 da07 4150 4948 6f6d  ...r......APIHom
+00000390: 65da 0761 735f 7669 6577 da0b 4772 6964  e..as_view..Grid
+000003a0: 436c 7573 7465 72da 0d4b 6d65 616e 7343  Cluster..KmeansC
+000003b0: 6c75 7374 6572 da11 4765 7443 6c75 7374  luster..GetClust
+000003c0: 6572 436f 6e74 656e 74da 0e47 6574 4172  erContent..GetAr
+000003d0: 6561 436f 6e74 656e 74da 1147 6574 4461  eaContent..GetDa
+000003e0: 7461 7365 7443 6f6e 7465 6e74 da12 4765  tasetContent..Ge
+000003f0: 744d 6170 436f 6e74 656e 7443 6f75 6e74  tMapContentCount
+00000400: da15 4765 7447 726f 7570 6564 4d61 7043  ..GetGroupedMapC
+00000410: 6f6e 7465 6e74 73da 0b75 726c 7061 7474  ontents..urlpatt
+00000420: 6572 6e73 a900 721c 0000 0072 1c00 0000  erns..r....r....
+00000430: fa37 2f68 6f6d 652f 746f 6d2f 616e 7963  .7/home/tom/anyc
+00000440: 6c75 7374 6572 2f64 656d 6f2f 646a 616e  luster/demo/djan
+00000450: 676f 2f61 6e79 636c 7573 7465 722f 6170  go/anycluster/ap
+00000460: 692f 7572 6c73 2e70 79da 083c 6d6f 6475  i/urls.py..<modu
+00000470: 6c65 3e01 0000 0073 2c00 0000 0c01 0c02  le>....s,.......
+00000480: 0c03 1201 1201 1201 0c01 02ff 0402 0c01  ................
+00000490: 02ff 0402 0c01 02ff 0402 0c01 02ff 0402  ................
+000004a0: 0c01 02ff 04f4 0410                      ........
```

### Comparing `anycluster-2.1.1/anycluster/api/json_schemas.py` & `anycluster-2.2.0/anycluster/api/json_schemas.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/api/serializers.py` & `anycluster-2.2.0/anycluster/api/serializers.py`

 * *Files 24% similar despite different names*

```diff
@@ -57,14 +57,32 @@
         return value
 
     def validate_filters(self, value):
         filters_are_allowed(value)
         return value
 
 
+class MapContentCountSerializer(ClusterRequestSerializer):
+    # additional filters, which are applied on top of filters, only for the count query
+    modulations = serializers.JSONField(required=False, default={}, write_only=True)
+
+    def validate_modulations(self, value):
+
+        if value:
+
+            for modulation_name, modulation in value.items():
+                filters_are_allowed(modulation['filters'])
+
+        return value
+
+
+class GroupedMapContentSerializer(ClusterRequestSerializer):
+    group_by = serializers.CharField(write_only=True)
+    
+
 class ClusterContentRequestSerializer(serializers.Serializer):
 
     output_srid = serializers.CharField(default='EPSG:4326', required=False, write_only=True)
     input_srid = serializers.CharField(default='EPSG:4326', required=False, write_only=True)
 
     geometry_type = serializers.ChoiceField(choices=GEOMETRY_TYPES, write_only=True)
```

### Comparing `anycluster-2.1.1/anycluster/api/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.2.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc` & `anycluster-2.2.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc` & `anycluster-2.2.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Apr 19 19:03:34 2023 UTC, .py size: 9420 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,436 +1,581 @@
-00000000: 550d 0d0a 0000 0000 063b 4064 cc24 0000  U........;@d.$..
+00000000: 550d 0d0a 0000 0000 a673 7064 9f35 0000  U........spd.5..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 5a01 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  d.l.m.Z.m.Z.m.Z.
 00000080: 6d0f 5a0f 6d10 5a10 6d11 5a11 0100 6400  m.Z.m.Z.m.Z...d.
-00000090: 6407 6c12 6d13 5a13 6d14 5a14 0100 6400  d.l.m.Z.m.Z...d.
-000000a0: 6408 6c15 6d16 5a16 6d17 5a17 6d18 5a18  d.l.m.Z.m.Z.m.Z.
-000000b0: 6d19 5a19 0100 6400 6409 6c1a 6d1b 5a1b  m.Z...d.d.l.m.Z.
+00000090: 6407 6c12 6d13 5a13 6d14 5a14 6d15 5a15  d.l.m.Z.m.Z.m.Z.
+000000a0: 0100 6400 6408 6c16 6d17 5a17 6d18 5a18  ..d.d.l.m.Z.m.Z.
+000000b0: 6d19 5a19 6d1a 5a1a 0100 6400 6409 6c1b  m.Z.m.Z...d.d.l.
 000000c0: 6d1c 5a1c 6d1d 5a1d 6d1e 5a1e 6d1f 5a1f  m.Z.m.Z.m.Z.m.Z.
-000000d0: 0100 640a 5a20 640a 5a21 640b 5a22 4700  ..d.Z d.Z!d.Z"G.
-000000e0: 640c 640d 8400 640d 6514 6504 8304 5a23  d.d...d.e.e...Z#
-000000f0: 4700 640e 640f 8400 640f 6513 6514 6504  G.d.d...d.e.e.e.
-00000100: 8305 5a24 4700 6410 6411 8400 6411 6513  ..Z$G.d.d...d.e.
-00000110: 6514 6504 8305 5a25 4700 6412 6413 8400  e.e...Z%G.d.d...
-00000120: 6413 6513 6514 6504 8305 5a26 4700 6414  d.e.e.e...Z&G.d.
-00000130: 6415 8400 6415 6513 6514 6504 8305 5a27  d...d.e.e.e...Z'
-00000140: 6416 5300 2917 e900 0000 0029 01da 0772  d.S.)......)...r
-00000150: 6576 6572 7365 2902 da11 4150 4952 6571  everse)...APIReq
-00000160: 7565 7374 4661 6374 6f72 79da 0b41 5049  uestFactory..API
-00000170: 5465 7374 4361 7365 2901 da06 7374 6174  TestCase)...stat
-00000180: 7573 2901 da0c 436c 7573 7465 7243 6163  us)...ClusterCac
-00000190: 6865 2901 da0c 4d61 7043 6c75 7374 6572  he)...MapCluster
-000001a0: 6572 2906 da0d 434c 5553 5445 525f 5459  er)...CLUSTER_TY
-000001b0: 5045 53da 1647 454f 4d45 5452 595f 5459  PES..GEOMETRY_TY
-000001c0: 5045 5f56 4945 5750 4f52 54da 1247 454f  PE_VIEWPORT..GEO
-000001d0: 4d45 5452 595f 5459 5045 5f41 5245 41da  METRY_TYPE_AREA.
-000001e0: 0e47 454f 4d45 5452 595f 5459 5045 53da  .GEOMETRY_TYPES.
-000001f0: 1343 4c55 5354 4552 5f54 5950 455f 4b4d  .CLUSTER_TYPE_KM
-00000200: 4541 4e53 da11 434c 5553 5445 525f 5459  EANS..CLUSTER_TY
-00000210: 5045 5f47 5249 4429 02da 0757 6974 6847  PE_GRID)...WithG
-00000220: 4953 da0b 5769 7468 4669 6c74 6572 7329  IS..WithFilters)
-00000230: 04da 1147 454f 4a53 4f4e 5f52 4543 5441  ...GEOJSON_RECTA
-00000240: 4e47 4c45 da0f 4745 4f4a 534f 4e5f 504f  NGLE..GEOJSON_PO
-00000250: 4c59 474f 4eda 1447 454f 4a53 4f4e 5f4d  LYGON..GEOJSON_M
-00000260: 554c 5449 504f 4c59 474f 4eda 1947 454f  ULTIPOLYGON..GEO
-00000270: 4a53 4f4e 5f46 4541 5455 5245 434f 4c4c  JSON_FEATURECOLL
-00000280: 4543 5449 4f4e 2905 da12 4d61 7043 6c75  ECTION)...MapClu
-00000290: 7374 6572 5669 6577 4261 7365 da0d 4b6d  sterViewBase..Km
-000002a0: 6561 6e73 436c 7573 7465 72da 0b47 7269  eansCluster..Gri
-000002b0: 6443 6c75 7374 6572 da11 4765 7443 6c75  dCluster..GetClu
-000002c0: 7374 6572 436f 6e74 656e 74da 0e47 6574  sterContent..Get
-000002d0: 4172 6561 436f 6e74 656e 74e9 0001 0000  AreaContent.....
-000002e0: e90a 0000 0063 0000 0000 0000 0000 0000  .....c..........
-000002f0: 0000 0000 0000 0200 0000 4000 0000 7334  ..........@...s4
-00000300: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
-00000310: 005a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
-00000320: 005a 0564 0764 0884 005a 0664 0964 0a84  .Z.d.d...Z.d.d..
-00000330: 005a 0764 0b53 0029 0cda 1654 6573 744d  .Z.d.S.)...TestM
-00000340: 6170 436c 7573 7465 7256 6965 7742 6173  apClusterViewBas
-00000350: 6563 0100 0000 0000 0000 0000 0000 0200  ec..............
-00000360: 0000 0300 0000 4300 0000 730e 0000 0074  ......C...s....t
-00000370: 0074 0164 019c 027d 017c 0153 00a9 024e  .t.d...}.|.S...N
-00000380: a902 da04 7a6f 6f6d 5a09 6772 6964 5f73  ....zoomZ.grid_s
-00000390: 697a 65a9 02da 045a 4f4f 4dda 0947 5249  ize....ZOOM..GRI
-000003a0: 445f 5349 5a45 a902 da04 7365 6c66 da0a  D_SIZE....self..
-000003b0: 7572 6c5f 6b77 6172 6773 a900 7225 0000  url_kwargs..r%..
-000003c0: 00fa 432f 686f 6d65 2f74 6f6d 2f61 6e79  ..C/home/tom/any
-000003d0: 636c 7573 7465 722f 6465 6d6f 2f64 6a61  cluster/demo/dja
-000003e0: 6e67 6f2f 616e 7963 6c75 7374 6572 2f61  ngo/anycluster/a
-000003f0: 7069 2f74 6573 7473 2f74 6573 745f 7669  pi/tests/test_vi
-00000400: 6577 732e 7079 da0e 6765 745f 7572 6c5f  ews.py..get_url_
-00000410: 6b77 6172 6773 1600 0000 7308 0000 0000  kwargs....s.....
-00000420: 0302 0102 fe06 057a 2554 6573 744d 6170  .......z%TestMap
-00000430: 436c 7573 7465 7256 6965 7742 6173 652e  ClusterViewBase.
-00000440: 6765 745f 7572 6c5f 6b77 6172 6773 6301  get_url_kwargsc.
-00000450: 0000 0000 0000 0000 0000 0005 0000 0004  ................
-00000460: 0000 0043 0000 0073 3000 0000 7400 8300  ...C...s0...t...
-00000470: 7d01 7c00 a001 a100 7d02 7402 6401 7c02  }.|.....}.t.d.|.
-00000480: 6402 8d02 7d03 7c01 a003 7c03 6900 a102  d...}.|...|.i...
-00000490: 7d04 6900 7c04 5f04 7c04 5300 a903 4eda  }.i.|._.|.S...N.
-000004a0: 0e6b 6d65 616e 735f 636c 7573 7465 72a9  .kmeans_cluster.
-000004b0: 01da 066b 7761 7267 7329 0572 0300 0000  ...kwargs).r....
-000004c0: 7227 0000 0072 0200 0000 da04 706f 7374  r'...r......post
-000004d0: da07 7365 7373 696f 6e29 0572 2300 0000  ..session).r#...
-000004e0: da07 6661 6374 6f72 7972 2400 0000 da03  ..factoryr$.....
-000004f0: 7572 6cda 0772 6571 7565 7374 7225 0000  url..requestr%..
-00000500: 0072 2500 0000 7226 0000 00da 0b67 6574  .r%...r&.....get
-00000510: 5f72 6571 7565 7374 2000 0000 730c 0000  _request ...s...
-00000520: 0000 0206 0208 010c 010c 0206 027a 2254  .............z"T
-00000530: 6573 744d 6170 436c 7573 7465 7256 6965  estMapClusterVie
-00000540: 7742 6173 652e 6765 745f 7265 7175 6573  wBase.get_reques
-00000550: 7463 0100 0000 0000 0000 0000 0000 0b00  tc..............
-00000560: 0000 0a00 0000 4300 0000 7370 0000 007c  ......C...sp...|
-00000570: 00a0 00a1 007d 0174 0183 007d 027c 00a0  .....}.t...}.|..
-00000580: 02a1 007d 0364 017d 0464 027d 057c 00a0  ...}.d.}.d.}.|..
-00000590: 03a1 007d 0674 0444 005d 407d 0774 0544  ...}.t.D.]@}.t.D
-000005a0: 005d 367d 087c 0644 005d 2c7d 097c 026a  .]6}.|.D.],}.|.j
-000005b0: 067c 077c 087c 097c 047c 057c 0166 067c  .|.|.|.|.|.|.f.|
-000005c0: 038e 017d 0a7c 00a0 0774 087c 0a74 0983  ...}.|...t.|.t..
-000005d0: 02a1 0101 0071 3a71 3271 2a64 0053 0029  .....q:q2q*d.S.)
-000005e0: 034e 4669 e610 0000 290a 7231 0000 0072  .NFi....).r1...r
-000005f0: 1400 0000 7227 0000 00da 1067 6574 5f74  ....r'.....get_t
-00000600: 6573 745f 6669 6c74 6572 7372 0b00 0000  est_filtersr....
-00000610: 7208 0000 005a 1167 6574 5f6d 6170 5f63  r....Z.get_map_c
-00000620: 6c75 7374 6572 6572 da0a 6173 7365 7274  lusterer..assert
-00000630: 5472 7565 da0a 6973 696e 7374 616e 6365  True..isinstance
-00000640: 7207 0000 0029 0b72 2300 0000 7230 0000  r....).r#...r0..
-00000650: 00da 0462 6173 6572 2b00 0000 da0b 636c  ...baser+.....cl
-00000660: 6561 725f 6361 6368 655a 0b6f 7574 7075  ear_cacheZ.outpu
-00000670: 745f 7372 6964 da0c 6669 6c74 6572 5f6c  t_srid..filter_l
-00000680: 6973 7473 da0d 6765 6f6d 6574 7279 5f74  ists..geometry_t
-00000690: 7970 65da 0b63 6c75 7374 6572 7479 7065  ype..clustertype
-000006a0: da07 6669 6c74 6572 735a 0963 6c75 7374  ..filtersZ.clust
-000006b0: 6572 6572 7225 0000 0072 2500 0000 7226  ererr%...r%...r&
-000006c0: 0000 00da 1674 6573 745f 6765 745f 6d61  .....test_get_ma
-000006d0: 705f 636c 7573 7465 7265 722d 0000 0073  p_clusterer-...s
-000006e0: 1e00 0000 0002 0802 0601 0802 0402 0401  ................
-000006f0: 0802 0801 0802 0801 0e01 02ff 0201 02ff  ................
-00000700: 0402 7a2d 5465 7374 4d61 7043 6c75 7374  ..z-TestMapClust
-00000710: 6572 5669 6577 4261 7365 2e74 6573 745f  erViewBase.test_
-00000720: 6765 745f 6d61 705f 636c 7573 7465 7265  get_map_clustere
-00000730: 7263 0100 0000 0000 0000 0000 0000 0800  rc..............
-00000740: 0000 0a00 0000 4300 0000 735a 0000 007c  ......C...sZ...|
-00000750: 00a0 00a1 007d 0174 0183 007d 027c 00a0  .....}.t...}.|..
-00000760: 02a1 007d 0374 0344 005d 3a7d 0474 0444  ...}.t.D.]:}.t.D
-00000770: 005d 307d 057c 0344 005d 267d 067c 02a0  .]0}.|.D.]&}.|..
-00000780: 057c 0474 067c 057c 017c 06a1 057d 077c  .|.t.|.|.|...}.|
-00000790: 00a0 0774 087c 0774 0983 02a1 0101 0071  ...t.|.t.......q
-000007a0: 2a71 2271 1a64 0053 0029 014e 290a 7231  *q"q.d.S.).N).r1
-000007b0: 0000 0072 1400 0000 7232 0000 0072 0b00  ...r....r2...r..
-000007c0: 0000 7208 0000 00da 0967 6574 5f63 6163  ..r......get_cac
-000007d0: 6865 7220 0000 0072 3300 0000 7234 0000  her ...r3...r4..
-000007e0: 0072 0600 0000 2908 7223 0000 0072 3000  .r....).r#...r0.
-000007f0: 0000 7235 0000 0072 3700 0000 7238 0000  ..r5...r7...r8..
-00000800: 0072 3900 0000 723a 0000 00da 0563 6163  .r9...r:.....cac
-00000810: 6865 7225 0000 0072 2500 0000 7226 0000  her%...r%...r&..
-00000820: 00da 0e74 6573 745f 6765 745f 6361 6368  ...test_get_cach
-00000830: 6542 0000 0073 1000 0000 0002 0802 0602  eB...s..........
-00000840: 0802 0801 0802 0801 1202 7a25 5465 7374  ..........z%Test
-00000850: 4d61 7043 6c75 7374 6572 5669 6577 4261  MapClusterViewBa
-00000860: 7365 2e74 6573 745f 6765 745f 6361 6368  se.test_get_cach
-00000870: 6563 0100 0000 0000 0000 0000 0000 0900  ec..............
-00000880: 0000 0a00 0000 4300 0000 738e 0000 007c  ......C...s....|
-00000890: 00a0 00a1 007d 0174 0183 007d 027c 00a0  .....}.t...}.|..
-000008a0: 02a1 007d 0374 0344 005d 6e7d 0474 0444  ...}.t.D.]n}.t.D
-000008b0: 005d 647d 057c 0344 005d 5a7d 067c 02a0  .]d}.|.D.]Z}.|..
-000008c0: 057c 0474 067c 057c 017c 06a1 057d 077c  .|.t.|.|.|...}.|
-000008d0: 02a0 077c 017c 07a1 0201 007c 00a0 087c  ...|.|.....|...|
-000008e0: 026a 097c 016a 0aa1 0201 0064 0144 005d  .j.|.j.....d.D.]
-000008f0: 227d 087c 00a0 0b74 0c7c 077c 0883 027c  "}.|...t.|.|...|
-00000900: 016a 0a7c 026a 0919 007c 0819 00a1 0201  .j.|.j...|......
-00000910: 0071 6071 2a71 2271 1a64 0053 0029 024e  .q`q*q"q.d.S.).N
-00000920: 2904 7238 0000 0072 1e00 0000 7239 0000  ).r8...r....r9..
-00000930: 0072 3a00 0000 290d 7231 0000 0072 1400  .r:...).r1...r..
-00000940: 0000 7232 0000 0072 0b00 0000 7208 0000  ..r2...r....r...
-00000950: 0072 3c00 0000 7220 0000 005a 0973 6574  .r<...r ...Z.set
-00000960: 5f63 6163 6865 da08 6173 7365 7274 496e  _cache..assertIn
-00000970: da0a 6361 6368 655f 6e61 6d65 722d 0000  ..cache_namer-..
-00000980: 00da 0b61 7373 6572 7445 7175 616c da07  ...assertEqual..
-00000990: 6765 7461 7474 7229 0972 2300 0000 7230  getattr).r#...r0
-000009a0: 0000 0072 3500 0000 7237 0000 0072 3800  ...r5...r7...r8.
-000009b0: 0000 7239 0000 0072 3a00 0000 da0d 636c  ..r9...r:.....cl
-000009c0: 7573 7465 725f 6361 6368 65da 0461 7474  uster_cache..att
-000009d0: 7272 2500 0000 7225 0000 0072 2600 0000  rr%...r%...r&...
-000009e0: da0e 7465 7374 5f73 6574 5f63 6163 6865  ..test_set_cache
-000009f0: 5300 0000 7316 0000 0000 0208 0206 0208  S...s...........
-00000a00: 0208 0108 0208 0212 020c 0210 0208 027a  ...............z
-00000a10: 2554 6573 744d 6170 436c 7573 7465 7256  %TestMapClusterV
-00000a20: 6965 7742 6173 652e 7465 7374 5f73 6574  iewBase.test_set
-00000a30: 5f63 6163 6865 4e29 08da 085f 5f6e 616d  _cacheN)...__nam
-00000a40: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000a50: 0c5f 5f71 7561 6c6e 616d 655f 5f72 2700  .__qualname__r'.
-00000a60: 0000 7231 0000 0072 3b00 0000 723e 0000  ..r1...r;...r>..
-00000a70: 0072 4500 0000 7225 0000 0072 2500 0000  .rE...r%...r%...
-00000a80: 7225 0000 0072 2600 0000 721b 0000 0013  r%...r&...r.....
-00000a90: 0000 0073 0a00 0000 0803 080a 080d 0815  ...s............
-00000aa0: 0811 721b 0000 0063 0000 0000 0000 0000  ..r....c........
-00000ab0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000ac0: 7328 0000 0065 005a 0164 005a 0264 0164  s(...e.Z.d.Z.d.d
-00000ad0: 0284 005a 0367 0066 0164 0364 0484 015a  ...Z.g.f.d.d...Z
-00000ae0: 0464 0564 0684 005a 0564 0753 0029 08da  .d.d...Z.d.S.)..
-00000af0: 0f54 6573 7447 7269 6443 6c75 7374 6572  .TestGridCluster
-00000b00: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000b10: 0003 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
-00000b20: 7401 6401 9c02 7d01 7c01 5300 721c 0000  t.d...}.|.S.r...
-00000b30: 0072 1f00 0000 7222 0000 0072 2500 0000  .r....r"...r%...
-00000b40: 7225 0000 0072 2600 0000 7227 0000 006e  r%...r&...r'...n
-00000b50: 0000 0073 0800 0000 0003 0201 02fe 0605  ...s............
-00000b60: 7a1e 5465 7374 4772 6964 436c 7573 7465  z.TestGridCluste
-00000b70: 722e 6765 745f 7572 6c5f 6b77 6172 6773  r.get_url_kwargs
-00000b80: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00000b90: 0004 0000 0043 0000 0073 1000 0000 7400  .....C...s....t.
-00000ba0: 7c01 7401 6401 9c03 7d02 7c02 5300 a902  |.t.d...}.|.S...
-00000bb0: 4ea9 03da 0767 656f 6a73 6f6e 723a 0000  N....geojsonr:..
-00000bc0: 0072 3800 0000 2902 7210 0000 0072 0900  .r8...).r....r..
-00000bd0: 0000 2903 7223 0000 0072 3a00 0000 da09  ..).r#...r:.....
-00000be0: 706f 7374 5f64 6174 6172 2500 0000 7225  post_datar%...r%
-00000bf0: 0000 0072 2600 0000 da0d 6765 745f 706f  ...r&.....get_po
-00000c00: 7374 5f64 6174 6177 0000 0073 0a00 0000  st_dataw...s....
-00000c10: 0003 0201 0201 02fd 0606 7a1d 5465 7374  ..........z.Test
-00000c20: 4772 6964 436c 7573 7465 722e 6765 745f  GridCluster.get_
-00000c30: 706f 7374 5f64 6174 6163 0100 0000 0000  post_datac......
-00000c40: 0000 0000 0000 0700 0000 0600 0000 4300  ..............C.
-00000c50: 0000 7356 0000 007c 00a0 00a1 007d 017c  ..sV...|.....}.|
-00000c60: 00a0 01a1 007d 0274 0264 017c 0264 028d  .....}.t.d.|.d..
-00000c70: 027d 037c 0144 005d 307d 047c 00a0 037c  .}.|.D.]0}.|...|
-00000c80: 04a1 017d 057c 006a 046a 057c 037c 0564  ...}.|.j.j.|.|.d
-00000c90: 0364 048d 037d 067c 00a0 067c 066a 0774  .d...}.|...|.j.t
-00000ca0: 086a 09a1 0201 0071 2064 0053 0029 054e  .j.....q d.S.).N
-00000cb0: 5a0c 6772 6964 5f63 6c75 7374 6572 722a  Z.grid_clusterr*
-00000cc0: 0000 00da 046a 736f 6ea9 01da 0666 6f72  .....json....for
-00000cd0: 6d61 7429 0a72 3200 0000 7227 0000 0072  mat).r2...r'...r
-00000ce0: 0200 0000 724e 0000 00da 0663 6c69 656e  ....rN.....clien
-00000cf0: 7472 2c00 0000 7241 0000 00da 0b73 7461  tr,...rA.....sta
-00000d00: 7475 735f 636f 6465 7205 0000 00da 0b48  tus_coder......H
-00000d10: 5454 505f 3230 305f 4f4b 2907 7223 0000  TTP_200_OK).r#..
-00000d20: 0072 3700 0000 7224 0000 0072 2f00 0000  .r7...r$...r/...
-00000d30: 723a 0000 0072 4d00 0000 da08 7265 7370  r:...rM.....resp
-00000d40: 6f6e 7365 7225 0000 0072 2500 0000 7226  onser%...r%...r&
-00000d50: 0000 00da 0974 6573 745f 706f 7374 8200  .....test_post..
-00000d60: 0000 730e 0000 0000 0208 0208 010c 0208  ..s.............
-00000d70: 020a 0212 027a 1954 6573 7447 7269 6443  .....z.TestGridC
-00000d80: 6c75 7374 6572 2e74 6573 745f 706f 7374  luster.test_post
-00000d90: 4e29 0672 4600 0000 7247 0000 0072 4800  N).rF...rG...rH.
-00000da0: 0000 7227 0000 0072 4e00 0000 7256 0000  ..r'...rN...rV..
-00000db0: 0072 2500 0000 7225 0000 0072 2500 0000  .r%...r%...r%...
-00000dc0: 7226 0000 0072 4900 0000 6c00 0000 7306  r&...rI...l...s.
-00000dd0: 0000 0008 0208 090c 0b72 4900 0000 6300  .........rI...c.
-00000de0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000df0: 0000 0040 0000 0073 3000 0000 6500 5a01  ...@...s0...e.Z.
-00000e00: 6400 5a02 6401 6402 8400 5a03 6403 6404  d.Z.d.d...Z.d.d.
-00000e10: 8400 5a04 6700 6601 6405 6406 8401 5a05  ..Z.g.f.d.d...Z.
-00000e20: 6407 6408 8400 5a06 6409 5300 290a da11  d.d...Z.d.S.)...
-00000e30: 5465 7374 4b6d 6561 6e73 436c 7573 7465  TestKmeansCluste
-00000e40: 7263 0100 0000 0000 0000 0000 0000 0200  rc..............
-00000e50: 0000 0300 0000 4300 0000 730e 0000 0074  ......C...s....t
-00000e60: 0074 0164 019c 027d 017c 0153 0072 1c00  .t.d...}.|.S.r..
-00000e70: 0000 721f 0000 0072 2200 0000 7225 0000  ..r....r"...r%..
-00000e80: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-00000e90: 9500 0000 7308 0000 0000 0302 0102 fe06  ....s...........
-00000ea0: 057a 2054 6573 744b 6d65 616e 7343 6c75  .z TestKmeansClu
-00000eb0: 7374 6572 2e67 6574 5f75 726c 5f6b 7761  ster.get_url_kwa
-00000ec0: 7267 7363 0100 0000 0000 0000 0000 0000  rgsc............
-00000ed0: 0300 0000 0400 0000 4300 0000 7318 0000  ........C...s...
-00000ee0: 007c 00a0 00a1 007d 0174 0164 017c 0164  .|.....}.t.d.|.d
-00000ef0: 028d 027d 027c 0253 0072 2800 0000 2902  ...}.|.S.r(...).
-00000f00: 7227 0000 0072 0200 0000 2903 7223 0000  r'...r....).r#..
-00000f10: 0072 2400 0000 722f 0000 0072 2500 0000  .r$...r/...r%...
-00000f20: 7225 0000 0072 2600 0000 da07 6765 745f  r%...r&.....get_
-00000f30: 7572 6c9f 0000 0073 0600 0000 0002 0801  url....s........
-00000f40: 0c01 7a19 5465 7374 4b6d 6561 6e73 436c  ..z.TestKmeansCl
-00000f50: 7573 7465 722e 6765 745f 7572 6c63 0400  uster.get_urlc..
-00000f60: 0000 0000 0000 0000 0000 0500 0000 0400  ................
-00000f70: 0000 4300 0000 7310 0000 007c 027c 037c  ..C...s....|.|.|
-00000f80: 0164 019c 037d 047c 0453 0072 4a00 0000  .d...}.|.S.rJ...
-00000f90: 7225 0000 0029 0572 2300 0000 7238 0000  r%...).r#...r8..
-00000fa0: 0072 4c00 0000 723a 0000 0072 4d00 0000  .rL...r:...rM...
-00000fb0: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
-00000fc0: 4e00 0000 a600 0000 730a 0000 0000 0302  N.......s.......
-00000fd0: 0102 0102 fd06 067a 1f54 6573 744b 6d65  .......z.TestKme
-00000fe0: 616e 7343 6c75 7374 6572 2e67 6574 5f70  ansCluster.get_p
-00000ff0: 6f73 745f 6461 7461 6301 0000 0000 0000  ost_datac.......
-00001000: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
-00001010: 0073 c200 0000 7c00 a000 a100 7d01 7c00  .s....|.....}.|.
-00001020: a001 7402 7403 a102 7d02 7c00 6a04 6a05  ..t.t...}.|.j.j.
-00001030: 7c01 7c02 6401 6402 8d03 7d03 7c03 6a06  |.|.d.d...}.|.j.
-00001040: 7407 6a08 6b03 723c 7409 7c03 6a0a 8301  t.j.k.r<t.|.j...
-00001050: 0100 7c00 a00b 7c03 6a06 7407 6a08 a102  ..|...|.j.t.j...
-00001060: 0100 7c00 a00c a100 7d04 7403 740d 740e  ..|.....}.t.t.t.
-00001070: 740f 6604 4400 5d5c 7d05 7c04 4400 5d52  t.f.D.]\}.|.D.]R
-00001080: 7d06 7c00 a001 7410 7c05 7c06 a103 7d02  }.|...t.|.|...}.
-00001090: 7c00 6a04 6a05 7c01 7c02 6401 6402 8d03  |.j.j.|.|.d.d...
-000010a0: 7d03 7c03 6a06 7407 6a08 6b03 72aa 7409  }.|.j.t.j.k.r.t.
-000010b0: 7c05 8301 0100 7409 7c03 6a0a 8301 0100  |.....t.|.j.....
-000010c0: 7c00 a00b 7c03 6a06 7407 6a08 a102 0100  |...|.j.t.j.....
-000010d0: 7168 7160 6400 5300 2903 4e72 4f00 0000  qhq`d.S.).NrO...
-000010e0: 7250 0000 0029 1172 5800 0000 724e 0000  rP...).rX...rN..
-000010f0: 0072 0900 0000 7210 0000 0072 5200 0000  .r....r....rR...
-00001100: 722c 0000 0072 5300 0000 7205 0000 0072  r,...rS...r....r
-00001110: 5400 0000 da05 7072 696e 74da 0464 6174  T.....print..dat
-00001120: 6172 4100 0000 7232 0000 0072 1100 0000  arA...r2...r....
-00001130: 7212 0000 0072 1300 0000 720a 0000 0029  r....r....r....)
-00001140: 0772 2300 0000 722f 0000 0072 4d00 0000  .r#...r/...rM...
-00001150: 7255 0000 0072 3700 0000 724c 0000 0072  rU...r7...rL...r
-00001160: 3a00 0000 7225 0000 0072 2500 0000 7226  :...r%...r%...r&
-00001170: 0000 0072 5600 0000 b100 0000 731e 0000  ...rV.......s...
-00001180: 0000 0208 030c 0212 020c 010a 0110 0208  ................
-00001190: 0110 0208 020e 0212 020c 0108 010a 017a  ...............z
-000011a0: 1b54 6573 744b 6d65 616e 7343 6c75 7374  .TestKmeansClust
-000011b0: 6572 2e74 6573 745f 706f 7374 4e29 0772  er.test_postN).r
-000011c0: 4600 0000 7247 0000 0072 4800 0000 7227  F...rG...rH...r'
-000011d0: 0000 0072 5800 0000 724e 0000 0072 5600  ...rX...rN...rV.
-000011e0: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
-000011f0: 0072 2600 0000 7257 0000 0093 0000 0073  .r&...rW.......s
-00001200: 0800 0000 0802 080a 0807 0c0b 7257 0000  ............rW..
-00001210: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001220: 0000 0200 0000 4000 0000 7314 0000 0065  ......@...s....e
-00001230: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
-00001240: 0353 0029 04da 1b54 6573 7447 6574 4b6d  .S.)...TestGetKm
-00001250: 6561 6e73 436c 7573 7465 7243 6f6e 7465  eansClusterConte
-00001260: 6e74 6301 0000 0000 0000 0000 0000 0018  ntc.............
-00001270: 0000 000b 0000 0043 0000 0073 ee01 0000  .......C...s....
-00001280: 7c00 a000 a100 7d01 7401 4400 9001 5dda  |.....}.t.D...].
-00001290: 7d02 7c01 4400 9001 5dce 7d03 7402 7403  }.|.D...].}.t.t.
-000012a0: 6401 9c02 7d04 7404 6402 7c04 6403 8d02  d...}.t.d.|.d...
-000012b0: 7d05 7405 7c03 7c02 6404 9c03 7d06 7406  }.t.|.|.d...}.t.
-000012c0: 8300 7d07 7c07 6a07 7c05 7c06 6405 6406  ..}.|.j.|.|.d.d.
-000012d0: 8d03 7d08 6900 7c08 5f08 7409 a00a a100  ..}.i.|._.t.....
-000012e0: 7d09 7c09 7c08 6601 7c04 8e01 7d0a 7c02  }.|.|.f.|...}.|.
-000012f0: 740b 6b02 7290 7c00 a00c 740d 7c08 6a08  t.k.r.|...t.|.j.
-00001300: 6407 1900 6408 1900 8301 6409 a102 0100  d...d.....d.....
-00001310: 7c0a 6a0e 640a 1900 7d0b 740f 7c02 7402  |.j.d...}.t.|.t.
-00001320: 7410 7c03 8304 7d0c 7c0c a011 7c08 6a08  t.|...}.|...|.j.
-00001330: 6407 1900 a101 0100 7c00 a00c 7c0c 6a12  d.......|...|.j.
-00001340: 7c08 6a08 6407 1900 6408 1900 a102 0100  |.j.d...d.......
-00001350: 7c02 740b 6b02 9001 7206 7c00 a00c 740d  |.t.k...r.|...t.
-00001360: 7c0c 6a12 8301 6409 a102 0100 7c0c 6a12  |.j...d.....|.j.
-00001370: 640a 1900 7d0d 7c00 a00c 7413 7c0d 8301  d...}.|...t.|...
-00001380: 7414 a102 0100 7415 7c0c 8301 7d0e 7c0b  t.....t.|...}.|.
-00001390: 640b 1900 7d0f 7c0b 640c 1900 640d 1900  d...}.|.d...d...
-000013a0: 7d10 7c0b 640c 1900 640e 1900 7d11 7c00  }.|.d...d...}.|.
-000013b0: a00c 7c0e 6a16 6a12 7c08 6a08 6407 1900  ..|.j.j.|.j.d...
-000013c0: 6408 1900 a102 0100 7417 7c0e a018 7c02  d.......t.|...|.
-000013d0: 7c0f 7c10 7c11 7c03 7402 a106 8301 7d12  |.|.|.|.t.....}.
-000013e0: 7c00 a019 740d 7417 7c12 8301 8301 640a  |...t.t.|.....d.
-000013f0: 6b04 a101 0100 7c00 a00c 740d 7417 7c12  k.....|...t.t.|.
-00001400: 8301 8301 7c0b 640f 1900 a102 0100 7404  ....|.d.......t.
-00001410: 6410 7c04 6403 8d02 7d13 7c02 7c0f 7c10  d.|.d...}.|.|.|.
-00001420: 7c11 7c03 6411 9c05 7d14 7c07 6a07 7c13  |.|.d...}.|.j.|.
-00001430: 7c14 6405 6406 8d03 7d15 7c08 6a08 7c15  |.d.d...}.|.j.|.
-00001440: 5f08 741a a00a a100 7d16 7c16 7c15 6601  _.t.....}.|.|.f.
-00001450: 7c04 8e01 7d17 7c00 a00c 7c17 6a1b 741c  |...}.|...|.j.t.
-00001460: 6a1d a102 0100 7116 710c 6400 5300 2912  j.....q.q.d.S.).
-00001470: 4e72 1d00 0000 7229 0000 0072 2a00 0000  Nr....r)...r*...
-00001480: 724b 0000 0072 4f00 0000 7250 0000 005a  rK...rO...rP...Z
-00001490: 1061 6e79 636c 7573 7465 725f 6361 6368  .anycluster_cach
-000014a0: 65da 0a67 656f 6d65 7472 6965 73e9 0100  e..geometries...
-000014b0: 0000 7201 0000 00da 0369 6473 da06 6365  ..r......ids..ce
-000014c0: 6e74 6572 da01 78da 0179 da05 636f 756e  nter..x..y..coun
-000014d0: 74da 1a67 6574 5f6b 6d65 616e 735f 636c  t..get_kmeans_cl
-000014e0: 7573 7465 725f 636f 6e74 656e 7429 0572  uster_content).r
-000014f0: 3800 0000 725e 0000 0072 6000 0000 7261  8...r^...r`...ra
-00001500: 0000 0072 3a00 0000 291e 7232 0000 0072  ...r:...).r2...r
-00001510: 0b00 0000 7220 0000 0072 2100 0000 7202  ....r ...r!...r.
-00001520: 0000 0072 1000 0000 7203 0000 0072 2c00  ...r....r....r,.
-00001530: 0000 722d 0000 0072 1500 0000 da07 6173  ..r-...r......as
-00001540: 5f76 6965 7772 0a00 0000 7241 0000 00da  _viewr....rA....
-00001550: 036c 656e 725a 0000 0072 0600 0000 720c  .lenrZ...r....r.
-00001560: 0000 00da 0f6c 6f61 645f 6765 6f6d 6574  .....load_geomet
-00001570: 7269 6573 725c 0000 00da 0474 7970 65da  riesr\.....type.
-00001580: 0373 7472 7207 0000 0072 4300 0000 da04  .strr....rC.....
-00001590: 6c69 7374 7263 0000 0072 3300 0000 7217  listrc...r3...r.
-000015a0: 0000 0072 5300 0000 7205 0000 0072 5400  ...rS...r....rT.
-000015b0: 0000 2918 7223 0000 0072 3700 0000 7238  ..).r#...r7...r8
-000015c0: 0000 0072 3a00 0000 7224 0000 005a 0a6b  ...r:...r$...Z.k
-000015d0: 6d65 616e 735f 7572 6c5a 106b 6d65 616e  means_urlZ.kmean
-000015e0: 735f 706f 7374 5f64 6174 6172 2e00 0000  s_post_datar....
-000015f0: 5a0e 6b6d 6561 6e73 5f72 6571 7565 7374  Z.kmeans_request
-00001600: 5a0b 6b6d 6561 6e73 5f76 6965 775a 0f6b  Z.kmeans_viewZ.k
-00001610: 6d65 616e 735f 7265 7370 6f6e 7365 5a07  means_responseZ.
-00001620: 636c 7573 7465 7272 4300 0000 da04 6765  clusterrC.....ge
-00001630: 6f6d 5a0d 6d61 705f 636c 7573 7465 7265  omZ.map_clustere
-00001640: 7272 5e00 0000 7260 0000 0072 6100 0000  rr^...r`...ra...
-00001650: 5a0f 636c 7573 7465 725f 636f 6e74 656e  Z.cluster_conten
-00001660: 7472 2f00 0000 724d 0000 0072 3000 0000  tr/...rM...r0...
-00001670: da04 7669 6577 7255 0000 0072 2500 0000  ..viewrU...r%...
-00001680: 7225 0000 0072 2600 0000 7256 0000 00cf  r%...r&...rV....
-00001690: 0000 0073 5c00 0000 0002 0802 0a02 0a03  ...s\...........
-000016a0: 0201 02fe 0605 0c03 0201 0201 02fd 0606  ................
-000016b0: 0601 1001 0602 0802 0c02 0801 1a02 0a03  ................
-000016c0: 0e01 1002 1802 0a01 1202 0a02 1002 0802  ................
-000016d0: 0801 0c01 0c02 1a02 1802 1601 1804 0c03  ................
-000016e0: 0201 0201 0201 0201 02fb 0608 1001 0802  ................
-000016f0: 0801 0c02 7a25 5465 7374 4765 744b 6d65  ....z%TestGetKme
-00001700: 616e 7343 6c75 7374 6572 436f 6e74 656e  ansClusterConten
-00001710: 742e 7465 7374 5f70 6f73 744e a904 7246  t.test_postN..rF
-00001720: 0000 0072 4700 0000 7248 0000 0072 5600  ...rG...rH...rV.
-00001730: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
-00001740: 0072 2600 0000 725b 0000 00cd 0000 0073  .r&...r[.......s
-00001750: 0200 0000 0802 725b 0000 0063 0000 0000  ......r[...c....
-00001760: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00001770: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00001780: 0264 0164 0284 005a 0364 0353 0029 04da  .d.d...Z.d.S.)..
-00001790: 1254 6573 7447 6574 4172 6561 436f 6e74  .TestGetAreaCont
-000017a0: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
-000017b0: 0800 0000 0700 0000 4300 0000 738a 0000  ........C...s...
-000017c0: 0074 0074 0164 019c 027d 0174 0264 027c  .t.t.d...}.t.d.|
-000017d0: 0164 038d 027d 027c 00a0 03a1 007d 0374  .d...}.|.....}.t
-000017e0: 0474 0574 0674 0766 0444 005d 5a7d 047c  .t.t.t.f.D.]Z}.|
-000017f0: 0344 005d 507d 0574 087c 047c 0564 049c  .D.]P}.t.|.|.d..
-00001800: 037d 067c 006a 096a 0a7c 027c 0664 0564  .}.|.j.j.|.|.d.d
-00001810: 068d 037d 077c 076a 0b74 0c6a 0d6b 0372  ...}.|.j.t.j.k.r
-00001820: 7274 0e7c 0483 0101 0074 0e7c 076a 0f83  rt.|.....t.|.j..
-00001830: 0101 007c 00a0 107c 076a 0b74 0c6a 0da1  ...|...|.j.t.j..
-00001840: 0201 0071 3271 2a64 0053 0029 074e 721d  ...q2q*d.S.).Nr.
-00001850: 0000 005a 1067 6574 5f61 7265 615f 636f  ...Z.get_area_co
-00001860: 6e74 656e 7472 2a00 0000 2903 7238 0000  ntentr*...).r8..
-00001870: 0072 4c00 0000 723a 0000 0072 4f00 0000  .rL...r:...rO...
-00001880: 7250 0000 0029 1172 2000 0000 7221 0000  rP...).r ...r!..
-00001890: 0072 0200 0000 7232 0000 0072 1000 0000  .r....r2...r....
-000018a0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000018b0: 0a00 0000 7252 0000 0072 2c00 0000 7253  ....rR...r,...rS
-000018c0: 0000 0072 0500 0000 7254 0000 0072 5900  ...r....rT...rY.
-000018d0: 0000 725a 0000 0072 4100 0000 2908 7223  ..rZ...rA...).r#
-000018e0: 0000 0072 2400 0000 722f 0000 0072 3700  ...r$...r/...r7.
-000018f0: 0000 724c 0000 0072 3a00 0000 724d 0000  ..rL...r:...rM..
-00001900: 0072 5500 0000 7225 0000 0072 2500 0000  .rU...r%...r%...
-00001910: 7226 0000 0072 5600 0000 2201 0000 7320  r&...rV..."...s 
-00001920: 0000 0000 0302 0102 fe06 050c 0208 0210  ................
-00001930: 0208 0302 0102 0102 fd06 0612 020c 0108  ................
-00001940: 010a 027a 1c54 6573 7447 6574 4172 6561  ...z.TestGetArea
-00001950: 436f 6e74 656e 742e 7465 7374 5f70 6f73  Content.test_pos
-00001960: 744e 726c 0000 0072 2500 0000 7225 0000  tNrl...r%...r%..
-00001970: 0072 2500 0000 7226 0000 0072 6d00 0000  .r%...r&...rm...
-00001980: 2001 0000 7302 0000 0008 0272 6d00 0000   ...s......rm...
-00001990: 4e29 28da 0b64 6a61 6e67 6f2e 7572 6c73  N)(..django.urls
-000019a0: 7202 0000 005a 1372 6573 745f 6672 616d  r....Z.rest_fram
-000019b0: 6577 6f72 6b2e 7465 7374 7203 0000 0072  ework.testr....r
-000019c0: 0400 0000 da0e 7265 7374 5f66 7261 6d65  ......rest_frame
-000019d0: 776f 726b 7205 0000 00da 0a61 6e79 636c  workr......anycl
-000019e0: 7573 7465 7272 0600 0000 5a17 616e 7963  usterr....Z.anyc
-000019f0: 6c75 7374 6572 2e4d 6170 436c 7573 7465  luster.MapCluste
-00001a00: 7265 7272 0700 0000 da16 616e 7963 6c75  rerr......anyclu
-00001a10: 7374 6572 2e64 6566 696e 6974 696f 6e73  ster.definitions
-00001a20: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00001a30: 0b00 0000 720c 0000 0072 0d00 0000 5a17  ....r....r....Z.
-00001a40: 616e 7963 6c75 7374 6572 2e74 6573 7473  anycluster.tests
-00001a50: 2e6d 6978 696e 7372 0e00 0000 720f 0000  .mixinsr....r...
-00001a60: 005a 1761 6e79 636c 7573 7465 722e 7465  .Z.anycluster.te
-00001a70: 7374 732e 636f 6d6d 6f6e 7210 0000 0072  sts.commonr....r
-00001a80: 1100 0000 7212 0000 0072 1300 0000 5a14  ....r....r....Z.
-00001a90: 616e 7963 6c75 7374 6572 2e61 7069 2e76  anycluster.api.v
-00001aa0: 6965 7773 7214 0000 0072 1500 0000 7216  iewsr....r....r.
-00001ab0: 0000 0072 1700 0000 7218 0000 005a 0c4d  ...r....r....Z.M
-00001ac0: 4150 5f54 494c 4553 495a 4572 2100 0000  AP_TILESIZEr!...
-00001ad0: 7220 0000 0072 1b00 0000 7249 0000 0072  r ...r....rI...r
-00001ae0: 5700 0000 725b 0000 0072 6d00 0000 7225  W...r[...rm...r%
-00001af0: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00001b00: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001b10: 7320 0000 000c 0110 010c 020c 010c 0120  s ............. 
-00001b20: 0310 0118 021c 0204 0104 0104 0212 5914  ..............Y.
-00001b30: 2714 3a14 53                             '.:.S
+000000d0: 6d20 5a20 6d21 5a21 0100 6400 640a 6c22  m Z m!Z!..d.d.l"
+000000e0: 6d23 5a23 0100 6400 640b 6c24 5a24 640c  m#Z#..d.d.l$Z$d.
+000000f0: 5a25 640c 5a26 640d 5a27 4700 640e 640f  Z%d.Z&d.Z'G.d.d.
+00000100: 8400 640f 6514 6504 8304 5a28 4700 6410  ..d.e.e...Z(G.d.
+00000110: 6411 8400 6411 6513 6514 6504 8305 5a29  d...d.e.e.e...Z)
+00000120: 4700 6412 6413 8400 6413 6513 6514 6504  G.d.d...d.e.e.e.
+00000130: 8305 5a2a 4700 6414 6415 8400 6415 6513  ..Z*G.d.d...d.e.
+00000140: 6514 6504 8305 5a2b 4700 6416 6417 8400  e.e...Z+G.d.d...
+00000150: 6417 6513 6514 6504 8305 5a2c 4700 6418  d.e.e.e...Z,G.d.
+00000160: 6419 8400 6419 6515 6514 6504 8305 5a2d  d...d.e.e.e...Z-
+00000170: 4700 641a 641b 8400 641b 6515 6514 6504  G.d.d...d.e.e.e.
+00000180: 8305 5a2e 640b 5300 291c e900 0000 0029  ..Z.d.S.)......)
+00000190: 01da 0772 6576 6572 7365 2902 da11 4150  ...reverse)...AP
+000001a0: 4952 6571 7565 7374 4661 6374 6f72 79da  IRequestFactory.
+000001b0: 0b41 5049 5465 7374 4361 7365 2901 da06  .APITestCase)...
+000001c0: 7374 6174 7573 2901 da0c 436c 7573 7465  status)...Cluste
+000001d0: 7243 6163 6865 2901 da0c 4d61 7043 6c75  rCache)...MapClu
+000001e0: 7374 6572 6572 2906 da0d 434c 5553 5445  sterer)...CLUSTE
+000001f0: 525f 5459 5045 53da 1647 454f 4d45 5452  R_TYPES..GEOMETR
+00000200: 595f 5459 5045 5f56 4945 5750 4f52 54da  Y_TYPE_VIEWPORT.
+00000210: 1247 454f 4d45 5452 595f 5459 5045 5f41  .GEOMETRY_TYPE_A
+00000220: 5245 41da 0e47 454f 4d45 5452 595f 5459  REA..GEOMETRY_TY
+00000230: 5045 53da 1343 4c55 5354 4552 5f54 5950  PES..CLUSTER_TYP
+00000240: 455f 4b4d 4541 4e53 da11 434c 5553 5445  E_KMEANS..CLUSTE
+00000250: 525f 5459 5045 5f47 5249 4429 03da 0757  R_TYPE_GRID)...W
+00000260: 6974 6847 4953 da0b 5769 7468 4669 6c74  ithGIS..WithFilt
+00000270: 6572 73da 0b57 6974 6847 6172 6465 6e73  ers..WithGardens
+00000280: 2904 da11 4745 4f4a 534f 4e5f 5245 4354  )...GEOJSON_RECT
+00000290: 414e 474c 45da 0f47 454f 4a53 4f4e 5f50  ANGLE..GEOJSON_P
+000002a0: 4f4c 5947 4f4e da14 4745 4f4a 534f 4e5f  OLYGON..GEOJSON_
+000002b0: 4d55 4c54 4950 4f4c 5947 4f4e da19 4745  MULTIPOLYGON..GE
+000002c0: 4f4a 534f 4e5f 4645 4154 5552 4543 4f4c  OJSON_FEATURECOL
+000002d0: 4c45 4354 494f 4e29 06da 124d 6170 436c  LECTION)...MapCl
+000002e0: 7573 7465 7256 6965 7742 6173 65da 0d4b  usterViewBase..K
+000002f0: 6d65 616e 7343 6c75 7374 6572 da0b 4772  meansCluster..Gr
+00000300: 6964 436c 7573 7465 72da 1147 6574 436c  idCluster..GetCl
+00000310: 7573 7465 7243 6f6e 7465 6e74 da0e 4765  usterContent..Ge
+00000320: 7441 7265 6143 6f6e 7465 6e74 da12 4765  tAreaContent..Ge
+00000330: 744d 6170 436f 6e74 656e 7443 6f75 6e74  tMapContentCount
+00000340: 2901 da07 4761 7264 656e 734e e900 0100  )...GardensN....
+00000350: 00e9 0a00 0000 6300 0000 0000 0000 0000  ......c.........
+00000360: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+00000370: 3400 0000 6500 5a01 6400 5a02 6401 6402  4...e.Z.d.Z.d.d.
+00000380: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
+00000390: 8400 5a05 6407 6408 8400 5a06 6409 640a  ..Z.d.d...Z.d.d.
+000003a0: 8400 5a07 640b 5300 290c da16 5465 7374  ..Z.d.S.)...Test
+000003b0: 4d61 7043 6c75 7374 6572 5669 6577 4261  MapClusterViewBa
+000003c0: 7365 6301 0000 0000 0000 0000 0000 0002  sec.............
+000003d0: 0000 0003 0000 0043 0000 0073 0e00 0000  .......C...s....
+000003e0: 7400 7401 6401 9c02 7d01 7c01 5300 a902  t.t.d...}.|.S...
+000003f0: 4ea9 02da 047a 6f6f 6d5a 0967 7269 645f  N....zoomZ.grid_
+00000400: 7369 7a65 a902 da04 5a4f 4f4d da09 4752  size....ZOOM..GR
+00000410: 4944 5f53 495a 45a9 02da 0473 656c 66da  ID_SIZE....self.
+00000420: 0a75 726c 5f6b 7761 7267 73a9 0072 2800  .url_kwargs..r(.
+00000430: 0000 fa43 2f68 6f6d 652f 746f 6d2f 616e  ...C/home/tom/an
+00000440: 7963 6c75 7374 6572 2f64 656d 6f2f 646a  ycluster/demo/dj
+00000450: 616e 676f 2f61 6e79 636c 7573 7465 722f  ango/anycluster/
+00000460: 6170 692f 7465 7374 732f 7465 7374 5f76  api/tests/test_v
+00000470: 6965 7773 2e70 79da 0e67 6574 5f75 726c  iews.py..get_url
+00000480: 5f6b 7761 7267 731c 0000 0073 0800 0000  _kwargs....s....
+00000490: 0003 0201 02fe 0605 7a25 5465 7374 4d61  ........z%TestMa
+000004a0: 7043 6c75 7374 6572 5669 6577 4261 7365  pClusterViewBase
+000004b0: 2e67 6574 5f75 726c 5f6b 7761 7267 7363  .get_url_kwargsc
+000004c0: 0100 0000 0000 0000 0000 0000 0500 0000  ................
+000004d0: 0400 0000 4300 0000 7330 0000 0074 0083  ....C...s0...t..
+000004e0: 007d 017c 00a0 01a1 007d 0274 0264 017c  .}.|.....}.t.d.|
+000004f0: 0264 028d 027d 037c 01a0 037c 0369 00a1  .d...}.|...|.i..
+00000500: 027d 0469 007c 045f 047c 0453 00a9 034e  .}.i.|._.|.S...N
+00000510: da0e 6b6d 6561 6e73 5f63 6c75 7374 6572  ..kmeans_cluster
+00000520: a901 da06 6b77 6172 6773 2905 7203 0000  ....kwargs).r...
+00000530: 0072 2a00 0000 7202 0000 00da 0470 6f73  .r*...r......pos
+00000540: 74da 0773 6573 7369 6f6e 2905 7226 0000  t..session).r&..
+00000550: 00da 0766 6163 746f 7279 7227 0000 00da  ...factoryr'....
+00000560: 0375 726c da07 7265 7175 6573 7472 2800  .url..requestr(.
+00000570: 0000 7228 0000 0072 2900 0000 da0b 6765  ..r(...r).....ge
+00000580: 745f 7265 7175 6573 7426 0000 0073 0c00  t_request&...s..
+00000590: 0000 0002 0602 0801 0c01 0c02 0602 7a22  ..............z"
+000005a0: 5465 7374 4d61 7043 6c75 7374 6572 5669  TestMapClusterVi
+000005b0: 6577 4261 7365 2e67 6574 5f72 6571 7565  ewBase.get_reque
+000005c0: 7374 6301 0000 0000 0000 0000 0000 000b  stc.............
+000005d0: 0000 000a 0000 0043 0000 0073 7000 0000  .......C...sp...
+000005e0: 7c00 a000 a100 7d01 7401 8300 7d02 7c00  |.....}.t...}.|.
+000005f0: a002 a100 7d03 6401 7d04 6402 7d05 7c00  ....}.d.}.d.}.|.
+00000600: a003 a100 7d06 7404 4400 5d40 7d07 7405  ....}.t.D.]@}.t.
+00000610: 4400 5d36 7d08 7c06 4400 5d2c 7d09 7c02  D.]6}.|.D.],}.|.
+00000620: 6a06 7c07 7c08 7c09 7c04 7c05 7c01 6606  j.|.|.|.|.|.|.f.
+00000630: 7c03 8e01 7d0a 7c00 a007 7408 7c0a 7409  |...}.|...t.|.t.
+00000640: 8302 a101 0100 713a 7132 712a 6400 5300  ......q:q2q*d.S.
+00000650: 2903 4e46 69e6 1000 0029 0a72 3400 0000  ).NFi....).r4...
+00000660: 7215 0000 0072 2a00 0000 da10 6765 745f  r....r*.....get_
+00000670: 7465 7374 5f66 696c 7465 7273 720b 0000  test_filtersr...
+00000680: 0072 0800 0000 5a11 6765 745f 6d61 705f  .r....Z.get_map_
+00000690: 636c 7573 7465 7265 72da 0a61 7373 6572  clusterer..asser
+000006a0: 7454 7275 65da 0a69 7369 6e73 7461 6e63  tTrue..isinstanc
+000006b0: 6572 0700 0000 290b 7226 0000 0072 3300  er....).r&...r3.
+000006c0: 0000 da04 6261 7365 722e 0000 00da 0b63  ....baser......c
+000006d0: 6c65 6172 5f63 6163 6865 5a0b 6f75 7470  lear_cacheZ.outp
+000006e0: 7574 5f73 7269 64da 0c66 696c 7465 725f  ut_srid..filter_
+000006f0: 6c69 7374 73da 0d67 656f 6d65 7472 795f  lists..geometry_
+00000700: 7479 7065 da0b 636c 7573 7465 7274 7970  type..clustertyp
+00000710: 65da 0766 696c 7465 7273 5a09 636c 7573  e..filtersZ.clus
+00000720: 7465 7265 7272 2800 0000 7228 0000 0072  tererr(...r(...r
+00000730: 2900 0000 da16 7465 7374 5f67 6574 5f6d  ).....test_get_m
+00000740: 6170 5f63 6c75 7374 6572 6572 3300 0000  ap_clusterer3...
+00000750: 731e 0000 0000 0208 0206 0108 0204 0204  s...............
+00000760: 0108 0208 0108 0208 010e 0102 ff02 0102  ................
+00000770: ff04 027a 2d54 6573 744d 6170 436c 7573  ...z-TestMapClus
+00000780: 7465 7256 6965 7742 6173 652e 7465 7374  terViewBase.test
+00000790: 5f67 6574 5f6d 6170 5f63 6c75 7374 6572  _get_map_cluster
+000007a0: 6572 6301 0000 0000 0000 0000 0000 0008  erc.............
+000007b0: 0000 000a 0000 0043 0000 0073 5a00 0000  .......C...sZ...
+000007c0: 7c00 a000 a100 7d01 7401 8300 7d02 7c00  |.....}.t...}.|.
+000007d0: a002 a100 7d03 7403 4400 5d3a 7d04 7404  ....}.t.D.]:}.t.
+000007e0: 4400 5d30 7d05 7c03 4400 5d26 7d06 7c02  D.]0}.|.D.]&}.|.
+000007f0: a005 7c04 7406 7c05 7c01 7c06 a105 7d07  ..|.t.|.|.|...}.
+00000800: 7c00 a007 7408 7c07 7409 8302 a101 0100  |...t.|.t.......
+00000810: 712a 7122 711a 6400 5300 2901 4e29 0a72  q*q"q.d.S.).N).r
+00000820: 3400 0000 7215 0000 0072 3500 0000 720b  4...r....r5...r.
+00000830: 0000 0072 0800 0000 da09 6765 745f 6361  ...r......get_ca
+00000840: 6368 6572 2300 0000 7236 0000 0072 3700  cher#...r6...r7.
+00000850: 0000 7206 0000 0029 0872 2600 0000 7233  ..r....).r&...r3
+00000860: 0000 0072 3800 0000 723a 0000 0072 3b00  ...r8...r:...r;.
+00000870: 0000 723c 0000 0072 3d00 0000 da05 6361  ..r<...r=.....ca
+00000880: 6368 6572 2800 0000 7228 0000 0072 2900  cher(...r(...r).
+00000890: 0000 da0e 7465 7374 5f67 6574 5f63 6163  ....test_get_cac
+000008a0: 6865 4800 0000 7310 0000 0000 0208 0206  heH...s.........
+000008b0: 0208 0208 0108 0208 0112 027a 2554 6573  ...........z%Tes
+000008c0: 744d 6170 436c 7573 7465 7256 6965 7742  tMapClusterViewB
+000008d0: 6173 652e 7465 7374 5f67 6574 5f63 6163  ase.test_get_cac
+000008e0: 6865 6301 0000 0000 0000 0000 0000 0009  hec.............
+000008f0: 0000 000a 0000 0043 0000 0073 8e00 0000  .......C...s....
+00000900: 7c00 a000 a100 7d01 7401 8300 7d02 7c00  |.....}.t...}.|.
+00000910: a002 a100 7d03 7403 4400 5d6e 7d04 7404  ....}.t.D.]n}.t.
+00000920: 4400 5d64 7d05 7c03 4400 5d5a 7d06 7c02  D.]d}.|.D.]Z}.|.
+00000930: a005 7c04 7406 7c05 7c01 7c06 a105 7d07  ..|.t.|.|.|...}.
+00000940: 7c02 a007 7c01 7c07 a102 0100 7c00 a008  |...|.|.....|...
+00000950: 7c02 6a09 7c01 6a0a a102 0100 6401 4400  |.j.|.j.....d.D.
+00000960: 5d22 7d08 7c00 a00b 740c 7c07 7c08 8302  ]"}.|...t.|.|...
+00000970: 7c01 6a0a 7c02 6a09 1900 7c08 1900 a102  |.j.|.j...|.....
+00000980: 0100 7160 712a 7122 711a 6400 5300 2902  ..q`q*q"q.d.S.).
+00000990: 4e29 0472 3b00 0000 7221 0000 0072 3c00  N).r;...r!...r<.
+000009a0: 0000 723d 0000 0029 0d72 3400 0000 7215  ..r=...).r4...r.
+000009b0: 0000 0072 3500 0000 720b 0000 0072 0800  ...r5...r....r..
+000009c0: 0000 723f 0000 0072 2300 0000 5a09 7365  ..r?...r#...Z.se
+000009d0: 745f 6361 6368 65da 0861 7373 6572 7449  t_cache..assertI
+000009e0: 6eda 0a63 6163 6865 5f6e 616d 6572 3000  n..cache_namer0.
+000009f0: 0000 da0b 6173 7365 7274 4571 7561 6cda  ....assertEqual.
+00000a00: 0767 6574 6174 7472 2909 7226 0000 0072  .getattr).r&...r
+00000a10: 3300 0000 7238 0000 0072 3a00 0000 723b  3...r8...r:...r;
+00000a20: 0000 0072 3c00 0000 723d 0000 00da 0d63  ...r<...r=.....c
+00000a30: 6c75 7374 6572 5f63 6163 6865 da04 6174  luster_cache..at
+00000a40: 7472 7228 0000 0072 2800 0000 7229 0000  trr(...r(...r)..
+00000a50: 00da 0e74 6573 745f 7365 745f 6361 6368  ...test_set_cach
+00000a60: 6559 0000 0073 1600 0000 0002 0802 0602  eY...s..........
+00000a70: 0802 0801 0802 0802 1202 0c02 1002 0802  ................
+00000a80: 7a25 5465 7374 4d61 7043 6c75 7374 6572  z%TestMapCluster
+00000a90: 5669 6577 4261 7365 2e74 6573 745f 7365  ViewBase.test_se
+00000aa0: 745f 6361 6368 654e 2908 da08 5f5f 6e61  t_cacheN)...__na
+00000ab0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000ac0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 722a  ..__qualname__r*
+00000ad0: 0000 0072 3400 0000 723e 0000 0072 4100  ...r4...r>...rA.
+00000ae0: 0000 7248 0000 0072 2800 0000 7228 0000  ..rH...r(...r(..
+00000af0: 0072 2800 0000 7229 0000 0072 1e00 0000  .r(...r)...r....
+00000b00: 1900 0000 730a 0000 0008 0308 0a08 0d08  ....s...........
+00000b10: 1508 1172 1e00 0000 6300 0000 0000 0000  ...r....c.......
+00000b20: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000b30: 0073 2800 0000 6500 5a01 6400 5a02 6401  .s(...e.Z.d.Z.d.
+00000b40: 6402 8400 5a03 6700 6601 6403 6404 8401  d...Z.g.f.d.d...
+00000b50: 5a04 6405 6406 8400 5a05 6407 5300 2908  Z.d.d...Z.d.S.).
+00000b60: da0f 5465 7374 4772 6964 436c 7573 7465  ..TestGridCluste
+00000b70: 7263 0100 0000 0000 0000 0000 0000 0200  rc..............
+00000b80: 0000 0300 0000 4300 0000 730e 0000 0074  ......C...s....t
+00000b90: 0074 0164 019c 027d 017c 0153 0072 1f00  .t.d...}.|.S.r..
+00000ba0: 0000 7222 0000 0072 2500 0000 7228 0000  ..r"...r%...r(..
+00000bb0: 0072 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
+00000bc0: 7400 0000 7308 0000 0000 0302 0102 fe06  t...s...........
+00000bd0: 057a 1e54 6573 7447 7269 6443 6c75 7374  .z.TestGridClust
+00000be0: 6572 2e67 6574 5f75 726c 5f6b 7761 7267  er.get_url_kwarg
+00000bf0: 7363 0200 0000 0000 0000 0000 0000 0300  sc..............
+00000c00: 0000 0400 0000 4300 0000 7310 0000 0074  ......C...s....t
+00000c10: 007c 0174 0164 019c 037d 027c 0253 00a9  .|.t.d...}.|.S..
+00000c20: 024e a903 da07 6765 6f6a 736f 6e72 3d00  .N....geojsonr=.
+00000c30: 0000 723b 0000 0029 0272 1100 0000 7209  ..r;...).r....r.
+00000c40: 0000 0029 0372 2600 0000 723d 0000 00da  ...).r&...r=....
+00000c50: 0970 6f73 745f 6461 7461 7228 0000 0072  .post_datar(...r
+00000c60: 2800 0000 7229 0000 00da 0d67 6574 5f70  (...r).....get_p
+00000c70: 6f73 745f 6461 7461 7d00 0000 730a 0000  ost_data}...s...
+00000c80: 0000 0302 0102 0102 fd06 067a 1d54 6573  ...........z.Tes
+00000c90: 7447 7269 6443 6c75 7374 6572 2e67 6574  tGridCluster.get
+00000ca0: 5f70 6f73 745f 6461 7461 6301 0000 0000  _post_datac.....
+00000cb0: 0000 0000 0000 0007 0000 0006 0000 0043  ...............C
+00000cc0: 0000 0073 5600 0000 7c00 a000 a100 7d01  ...sV...|.....}.
+00000cd0: 7c00 a001 a100 7d02 7402 6401 7c02 6402  |.....}.t.d.|.d.
+00000ce0: 8d02 7d03 7c01 4400 5d30 7d04 7c00 a003  ..}.|.D.]0}.|...
+00000cf0: 7c04 a101 7d05 7c00 6a04 6a05 7c03 7c05  |...}.|.j.j.|.|.
+00000d00: 6403 6404 8d03 7d06 7c00 a006 7c06 6a07  d.d...}.|...|.j.
+00000d10: 7408 6a09 a102 0100 7120 6400 5300 2905  t.j.....q d.S.).
+00000d20: 4e5a 0c67 7269 645f 636c 7573 7465 7272  NZ.grid_clusterr
+00000d30: 2d00 0000 da04 6a73 6f6e a901 da06 666f  -.....json....fo
+00000d40: 726d 6174 290a 7235 0000 0072 2a00 0000  rmat).r5...r*...
+00000d50: 7202 0000 0072 5100 0000 da06 636c 6965  r....rQ.....clie
+00000d60: 6e74 722f 0000 0072 4400 0000 da0b 7374  ntr/...rD.....st
+00000d70: 6174 7573 5f63 6f64 6572 0500 0000 da0b  atus_coder......
+00000d80: 4854 5450 5f32 3030 5f4f 4b29 0772 2600  HTTP_200_OK).r&.
+00000d90: 0000 723a 0000 0072 2700 0000 7232 0000  ..r:...r'...r2..
+00000da0: 0072 3d00 0000 7250 0000 00da 0872 6573  .r=...rP.....res
+00000db0: 706f 6e73 6572 2800 0000 7228 0000 0072  ponser(...r(...r
+00000dc0: 2900 0000 da09 7465 7374 5f70 6f73 7488  ).....test_post.
+00000dd0: 0000 0073 0e00 0000 0002 0802 0801 0c02  ...s............
+00000de0: 0802 0a02 1202 7a19 5465 7374 4772 6964  ......z.TestGrid
+00000df0: 436c 7573 7465 722e 7465 7374 5f70 6f73  Cluster.test_pos
+00000e00: 744e 2906 7249 0000 0072 4a00 0000 724b  tN).rI...rJ...rK
+00000e10: 0000 0072 2a00 0000 7251 0000 0072 5900  ...r*...rQ...rY.
+00000e20: 0000 7228 0000 0072 2800 0000 7228 0000  ..r(...r(...r(..
+00000e30: 0072 2900 0000 724c 0000 0072 0000 0073  .r)...rL...r...s
+00000e40: 0600 0000 0802 0809 0c0b 724c 0000 0063  ..........rL...c
+00000e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000e60: 0300 0000 4000 0000 7330 0000 0065 005a  ....@...s0...e.Z
+00000e70: 0164 005a 0264 0164 0284 005a 0364 0364  .d.Z.d.d...Z.d.d
+00000e80: 0484 005a 0467 0066 0164 0564 0684 015a  ...Z.g.f.d.d...Z
+00000e90: 0564 0764 0884 005a 0664 0953 0029 0ada  .d.d...Z.d.S.)..
+00000ea0: 1154 6573 744b 6d65 616e 7343 6c75 7374  .TestKmeansClust
+00000eb0: 6572 6301 0000 0000 0000 0000 0000 0002  erc.............
+00000ec0: 0000 0003 0000 0043 0000 0073 0e00 0000  .......C...s....
+00000ed0: 7400 7401 6401 9c02 7d01 7c01 5300 721f  t.t.d...}.|.S.r.
+00000ee0: 0000 0072 2200 0000 7225 0000 0072 2800  ...r"...r%...r(.
+00000ef0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
+00000f00: 009b 0000 0073 0800 0000 0003 0201 02fe  .....s..........
+00000f10: 0605 7a20 5465 7374 4b6d 6561 6e73 436c  ..z TestKmeansCl
+00000f20: 7573 7465 722e 6765 745f 7572 6c5f 6b77  uster.get_url_kw
+00000f30: 6172 6773 6301 0000 0000 0000 0000 0000  argsc...........
+00000f40: 0003 0000 0004 0000 0043 0000 0073 1800  .........C...s..
+00000f50: 0000 7c00 a000 a100 7d01 7401 6401 7c01  ..|.....}.t.d.|.
+00000f60: 6402 8d02 7d02 7c02 5300 722b 0000 0029  d...}.|.S.r+...)
+00000f70: 0272 2a00 0000 7202 0000 0029 0372 2600  .r*...r....).r&.
+00000f80: 0000 7227 0000 0072 3200 0000 7228 0000  ..r'...r2...r(..
+00000f90: 0072 2800 0000 7229 0000 00da 0767 6574  .r(...r).....get
+00000fa0: 5f75 726c a500 0000 7306 0000 0000 0208  _url....s.......
+00000fb0: 010c 017a 1954 6573 744b 6d65 616e 7343  ...z.TestKmeansC
+00000fc0: 6c75 7374 6572 2e67 6574 5f75 726c 6304  luster.get_urlc.
+00000fd0: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00000fe0: 0000 0043 0000 0073 1000 0000 7c02 7c03  ...C...s....|.|.
+00000ff0: 7c01 6401 9c03 7d04 7c04 5300 724d 0000  |.d...}.|.S.rM..
+00001000: 0072 2800 0000 2905 7226 0000 0072 3b00  .r(...).r&...r;.
+00001010: 0000 724f 0000 0072 3d00 0000 7250 0000  ..rO...r=...rP..
+00001020: 0072 2800 0000 7228 0000 0072 2900 0000  .r(...r(...r)...
+00001030: 7251 0000 00ac 0000 0073 0a00 0000 0003  rQ.......s......
+00001040: 0201 0201 02fd 0606 7a1f 5465 7374 4b6d  ........z.TestKm
+00001050: 6561 6e73 436c 7573 7465 722e 6765 745f  eansCluster.get_
+00001060: 706f 7374 5f64 6174 6163 0100 0000 0000  post_datac......
+00001070: 0000 0000 0000 0700 0000 0700 0000 4300  ..............C.
+00001080: 0000 73c2 0000 007c 00a0 00a1 007d 017c  ..s....|.....}.|
+00001090: 00a0 0174 0274 03a1 027d 027c 006a 046a  ...t.t...}.|.j.j
+000010a0: 057c 017c 0264 0164 028d 037d 037c 036a  .|.|.d.d...}.|.j
+000010b0: 0674 076a 086b 0372 3c74 097c 036a 0a83  .t.j.k.r<t.|.j..
+000010c0: 0101 007c 00a0 0b7c 036a 0674 076a 08a1  ...|...|.j.t.j..
+000010d0: 0201 007c 00a0 0ca1 007d 0474 0374 0d74  ...|.....}.t.t.t
+000010e0: 0e74 0f66 0444 005d 5c7d 057c 0444 005d  .t.f.D.]\}.|.D.]
+000010f0: 527d 067c 00a0 0174 107c 057c 06a1 037d  R}.|...t.|.|...}
+00001100: 027c 006a 046a 057c 017c 0264 0164 028d  .|.j.j.|.|.d.d..
+00001110: 037d 037c 036a 0674 076a 086b 0372 aa74  .}.|.j.t.j.k.r.t
+00001120: 097c 0583 0101 0074 097c 036a 0a83 0101  .|.....t.|.j....
+00001130: 007c 00a0 0b7c 036a 0674 076a 08a1 0201  .|...|.j.t.j....
+00001140: 0071 6871 6064 0053 0029 034e 7252 0000  .qhq`d.S.).NrR..
+00001150: 0072 5300 0000 2911 725b 0000 0072 5100  .rS...).r[...rQ.
+00001160: 0000 7209 0000 0072 1100 0000 7255 0000  ..r....r....rU..
+00001170: 0072 2f00 0000 7256 0000 0072 0500 0000  .r/...rV...r....
+00001180: 7257 0000 00da 0570 7269 6e74 da04 6461  rW.....print..da
+00001190: 7461 7244 0000 0072 3500 0000 7212 0000  tarD...r5...r...
+000011a0: 0072 1300 0000 7214 0000 0072 0a00 0000  .r....r....r....
+000011b0: 2907 7226 0000 0072 3200 0000 7250 0000  ).r&...r2...rP..
+000011c0: 0072 5800 0000 723a 0000 0072 4f00 0000  .rX...r:...rO...
+000011d0: 723d 0000 0072 2800 0000 7228 0000 0072  r=...r(...r(...r
+000011e0: 2900 0000 7259 0000 00b7 0000 0073 1e00  )...rY.......s..
+000011f0: 0000 0002 0803 0c02 1202 0c01 0a01 1002  ................
+00001200: 0801 1002 0802 0e02 1202 0c01 0801 0a01  ................
+00001210: 7a1b 5465 7374 4b6d 6561 6e73 436c 7573  z.TestKmeansClus
+00001220: 7465 722e 7465 7374 5f70 6f73 744e 2907  ter.test_postN).
+00001230: 7249 0000 0072 4a00 0000 724b 0000 0072  rI...rJ...rK...r
+00001240: 2a00 0000 725b 0000 0072 5100 0000 7259  *...r[...rQ...rY
+00001250: 0000 0072 2800 0000 7228 0000 0072 2800  ...r(...r(...r(.
+00001260: 0000 7229 0000 0072 5a00 0000 9900 0000  ..r)...rZ.......
+00001270: 7308 0000 0008 0208 0a08 070c 0b72 5a00  s............rZ.
+00001280: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00001290: 0000 0002 0000 0040 0000 0073 1400 0000  .......@...s....
+000012a0: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
+000012b0: 6403 5300 2904 da1b 5465 7374 4765 744b  d.S.)...TestGetK
+000012c0: 6d65 616e 7343 6c75 7374 6572 436f 6e74  meansClusterCont
+000012d0: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
+000012e0: 1800 0000 0b00 0000 4300 0000 73ee 0100  ........C...s...
+000012f0: 007c 00a0 00a1 007d 0174 0144 0090 015d  .|.....}.t.D...]
+00001300: da7d 027c 0144 0090 015d ce7d 0374 0274  .}.|.D...].}.t.t
+00001310: 0364 019c 027d 0474 0464 027c 0464 038d  .d...}.t.d.|.d..
+00001320: 027d 0574 057c 037c 0264 049c 037d 0674  .}.t.|.|.d...}.t
+00001330: 0683 007d 077c 076a 077c 057c 0664 0564  ...}.|.j.|.|.d.d
+00001340: 068d 037d 0869 007c 085f 0874 09a0 0aa1  ...}.i.|._.t....
+00001350: 007d 097c 097c 0866 017c 048e 017d 0a7c  .}.|.|.f.|...}.|
+00001360: 0274 0b6b 0272 907c 00a0 0c74 0d7c 086a  .t.k.r.|...t.|.j
+00001370: 0864 0719 0064 0819 0083 0164 09a1 0201  .d...d.....d....
+00001380: 007c 0a6a 0e64 0a19 007d 0b74 0f7c 0274  .|.j.d...}.t.|.t
+00001390: 0274 107c 0383 047d 0c7c 0ca0 117c 086a  .t.|...}.|...|.j
+000013a0: 0864 0719 00a1 0101 007c 00a0 0c7c 0c6a  .d.......|...|.j
+000013b0: 127c 086a 0864 0719 0064 0819 00a1 0201  .|.j.d...d......
+000013c0: 007c 0274 0b6b 0290 0172 067c 00a0 0c74  .|.t.k...r.|...t
+000013d0: 0d7c 0c6a 1283 0164 09a1 0201 007c 0c6a  .|.j...d.....|.j
+000013e0: 1264 0a19 007d 0d7c 00a0 0c74 137c 0d83  .d...}.|...t.|..
+000013f0: 0174 14a1 0201 0074 157c 0c83 017d 0e7c  .t.....t.|...}.|
+00001400: 0b64 0b19 007d 0f7c 0b64 0c19 0064 0d19  .d...}.|.d...d..
+00001410: 007d 107c 0b64 0c19 0064 0e19 007d 117c  .}.|.d...d...}.|
+00001420: 00a0 0c7c 0e6a 166a 127c 086a 0864 0719  ...|.j.j.|.j.d..
+00001430: 0064 0819 00a1 0201 0074 177c 0ea0 187c  .d.......t.|...|
+00001440: 027c 0f7c 107c 117c 0374 02a1 0683 017d  .|.|.|.|.t.....}
+00001450: 127c 00a0 1974 0d74 177c 1283 0183 0164  .|...t.t.|.....d
+00001460: 0a6b 04a1 0101 007c 00a0 0c74 0d74 177c  .k.....|...t.t.|
+00001470: 1283 0183 017c 0b64 0f19 00a1 0201 0074  .....|.d.......t
+00001480: 0464 107c 0464 038d 027d 137c 027c 0f7c  .d.|.d...}.|.|.|
+00001490: 107c 117c 0364 119c 057d 147c 076a 077c  .|.|.d...}.|.j.|
+000014a0: 137c 1464 0564 068d 037d 157c 086a 087c  .|.d.d...}.|.j.|
+000014b0: 155f 0874 1aa0 0aa1 007d 167c 167c 1566  ._.t.....}.|.|.f
+000014c0: 017c 048e 017d 177c 00a0 0c7c 176a 1b74  .|...}.|...|.j.t
+000014d0: 1c6a 1da1 0201 0071 1671 0c64 0053 0029  .j.....q.q.d.S.)
+000014e0: 124e 7220 0000 0072 2c00 0000 722d 0000  .Nr ...r,...r-..
+000014f0: 0072 4e00 0000 7252 0000 0072 5300 0000  .rN...rR...rS...
+00001500: 5a10 616e 7963 6c75 7374 6572 5f63 6163  Z.anycluster_cac
+00001510: 6865 da0a 6765 6f6d 6574 7269 6573 e901  he..geometries..
+00001520: 0000 0072 0100 0000 da03 6964 73da 0663  ...r......ids..c
+00001530: 656e 7465 72da 0178 da01 79da 0563 6f75  enter..x..y..cou
+00001540: 6e74 da1a 6765 745f 6b6d 6561 6e73 5f63  nt..get_kmeans_c
+00001550: 6c75 7374 6572 5f63 6f6e 7465 6e74 2905  luster_content).
+00001560: 723b 0000 0072 6100 0000 7263 0000 0072  r;...ra...rc...r
+00001570: 6400 0000 723d 0000 0029 1e72 3500 0000  d...r=...).r5...
+00001580: 720b 0000 0072 2300 0000 7224 0000 0072  r....r#...r$...r
+00001590: 0200 0000 7211 0000 0072 0300 0000 722f  ....r....r....r/
+000015a0: 0000 0072 3000 0000 7216 0000 00da 0761  ...r0...r......a
+000015b0: 735f 7669 6577 720a 0000 0072 4400 0000  s_viewr....rD...
+000015c0: da03 6c65 6e72 5d00 0000 7206 0000 0072  ..lenr]...r....r
+000015d0: 0c00 0000 da0f 6c6f 6164 5f67 656f 6d65  ......load_geome
+000015e0: 7472 6965 7372 5f00 0000 da04 7479 7065  triesr_.....type
+000015f0: da03 7374 7272 0700 0000 7246 0000 00da  ..strr....rF....
+00001600: 046c 6973 7472 6600 0000 7236 0000 0072  .listrf...r6...r
+00001610: 1800 0000 7256 0000 0072 0500 0000 7257  ....rV...r....rW
+00001620: 0000 0029 1872 2600 0000 723a 0000 0072  ...).r&...r:...r
+00001630: 3b00 0000 723d 0000 0072 2700 0000 5a0a  ;...r=...r'...Z.
+00001640: 6b6d 6561 6e73 5f75 726c 5a10 6b6d 6561  kmeans_urlZ.kmea
+00001650: 6e73 5f70 6f73 745f 6461 7461 7231 0000  ns_post_datar1..
+00001660: 005a 0e6b 6d65 616e 735f 7265 7175 6573  .Z.kmeans_reques
+00001670: 745a 0b6b 6d65 616e 735f 7669 6577 5a0f  tZ.kmeans_viewZ.
+00001680: 6b6d 6561 6e73 5f72 6573 706f 6e73 655a  kmeans_responseZ
+00001690: 0763 6c75 7374 6572 7246 0000 00da 0467  .clusterrF.....g
+000016a0: 656f 6d5a 0d6d 6170 5f63 6c75 7374 6572  eomZ.map_cluster
+000016b0: 6572 7261 0000 0072 6300 0000 7264 0000  erra...rc...rd..
+000016c0: 005a 0f63 6c75 7374 6572 5f63 6f6e 7465  .Z.cluster_conte
+000016d0: 6e74 7232 0000 0072 5000 0000 7233 0000  ntr2...rP...r3..
+000016e0: 00da 0476 6965 7772 5800 0000 7228 0000  ...viewrX...r(..
+000016f0: 0072 2800 0000 7229 0000 0072 5900 0000  .r(...r)...rY...
+00001700: d500 0000 735c 0000 0000 0208 020a 020a  ....s\..........
+00001710: 0302 0102 fe06 050c 0302 0102 0102 fd06  ................
+00001720: 0606 0110 0106 0208 020c 0208 011a 020a  ................
+00001730: 030e 0110 0218 020a 0112 020a 0210 0208  ................
+00001740: 0208 010c 010c 021a 0218 0216 0118 040c  ................
+00001750: 0302 0102 0102 0102 0102 fb06 0810 0108  ................
+00001760: 0208 010c 027a 2554 6573 7447 6574 4b6d  .....z%TestGetKm
+00001770: 6561 6e73 436c 7573 7465 7243 6f6e 7465  eansClusterConte
+00001780: 6e74 2e74 6573 745f 706f 7374 4ea9 0472  nt.test_postN..r
+00001790: 4900 0000 724a 0000 0072 4b00 0000 7259  I...rJ...rK...rY
+000017a0: 0000 0072 2800 0000 7228 0000 0072 2800  ...r(...r(...r(.
+000017b0: 0000 7229 0000 0072 5e00 0000 d300 0000  ..r)...r^.......
+000017c0: 7302 0000 0008 0272 5e00 0000 6300 0000  s......r^...c...
+000017d0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+000017e0: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
+000017f0: 5a02 6401 6402 8400 5a03 6403 5300 2904  Z.d.d...Z.d.S.).
+00001800: da12 5465 7374 4765 7441 7265 6143 6f6e  ..TestGetAreaCon
+00001810: 7465 6e74 6301 0000 0000 0000 0000 0000  tentc...........
+00001820: 0008 0000 0007 0000 0043 0000 0073 8a00  .........C...s..
+00001830: 0000 7400 7401 6401 9c02 7d01 7402 6402  ..t.t.d...}.t.d.
+00001840: 7c01 6403 8d02 7d02 7c00 a003 a100 7d03  |.d...}.|.....}.
+00001850: 7404 7405 7406 7407 6604 4400 5d5a 7d04  t.t.t.t.f.D.]Z}.
+00001860: 7c03 4400 5d50 7d05 7408 7c04 7c05 6404  |.D.]P}.t.|.|.d.
+00001870: 9c03 7d06 7c00 6a09 6a0a 7c02 7c06 6405  ..}.|.j.j.|.|.d.
+00001880: 6406 8d03 7d07 7c07 6a0b 740c 6a0d 6b03  d...}.|.j.t.j.k.
+00001890: 7272 740e 7c04 8301 0100 740e 7c07 6a0f  rrt.|.....t.|.j.
+000018a0: 8301 0100 7c00 a010 7c07 6a0b 740c 6a0d  ....|...|.j.t.j.
+000018b0: a102 0100 7132 712a 6400 5300 2907 4e72  ....q2q*d.S.).Nr
+000018c0: 2000 0000 5a10 6765 745f 6172 6561 5f63   ...Z.get_area_c
+000018d0: 6f6e 7465 6e74 722d 0000 00a9 0372 3b00  ontentr-.....r;.
+000018e0: 0000 724f 0000 0072 3d00 0000 7252 0000  ..rO...r=...rR..
+000018f0: 0072 5300 0000 2911 7223 0000 0072 2400  .rS...).r#...r$.
+00001900: 0000 7202 0000 0072 3500 0000 7211 0000  ..r....r5...r...
+00001910: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00001920: 720a 0000 0072 5500 0000 722f 0000 0072  r....rU...r/...r
+00001930: 5600 0000 7205 0000 0072 5700 0000 725c  V...r....rW...r\
+00001940: 0000 0072 5d00 0000 7244 0000 00a9 0872  ...r]...rD.....r
+00001950: 2600 0000 7227 0000 0072 3200 0000 723a  &...r'...r2...r:
+00001960: 0000 0072 4f00 0000 723d 0000 0072 5000  ...rO...r=...rP.
+00001970: 0000 7258 0000 0072 2800 0000 7228 0000  ..rX...r(...r(..
+00001980: 0072 2900 0000 7259 0000 0028 0100 0073  .r)...rY...(...s
+00001990: 2000 0000 0003 0201 02fe 0605 0c02 0802   ...............
+000019a0: 1002 0803 0201 0201 02fd 0606 1202 0c01  ................
+000019b0: 0801 0a02 7a1c 5465 7374 4765 7441 7265  ....z.TestGetAre
+000019c0: 6143 6f6e 7465 6e74 2e74 6573 745f 706f  aContent.test_po
+000019d0: 7374 4e72 6f00 0000 7228 0000 0072 2800  stNro...r(...r(.
+000019e0: 0000 7228 0000 0072 2900 0000 7270 0000  ..r(...r)...rp..
+000019f0: 0026 0100 0073 0200 0000 0802 7270 0000  .&...s......rp..
+00001a00: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00001a10: 0000 0200 0000 4000 0000 731c 0000 0065  ......@...s....e
+00001a20: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
+00001a30: 0364 0484 005a 0464 0553 0029 06da 1654  .d...Z.d.S.)...T
+00001a40: 6573 7447 6574 4d61 7043 6f6e 7465 6e74  estGetMapContent
+00001a50: 436f 756e 7463 0100 0000 0000 0000 0000  Countc..........
+00001a60: 0000 0800 0000 0700 0000 4300 0000 7392  ..........C...s.
+00001a70: 0000 007c 00a0 00a1 0001 0074 0174 0264  ...|.......t.t.d
+00001a80: 019c 027d 0174 0364 027c 0164 038d 027d  ...}.t.d.|.d...}
+00001a90: 027c 00a0 04a1 007d 0374 0574 0674 0774  .|.....}.t.t.t.t
+00001aa0: 0866 0444 005d 5a7d 047c 0344 005d 507d  .f.D.]Z}.|.D.]P}
+00001ab0: 0574 097c 047c 0564 049c 037d 067c 006a  .t.|.|.d...}.|.j
+00001ac0: 0a6a 0b7c 027c 0664 0564 068d 037d 077c  .j.|.|.d.d...}.|
+00001ad0: 076a 0c74 0d6a 0e6b 0372 7a74 0f7c 0483  .j.t.j.k.rzt.|..
+00001ae0: 0101 0074 0f7c 076a 1083 0101 007c 00a0  ...t.|.j.....|..
+00001af0: 117c 076a 0c74 0d6a 0ea1 0201 0071 3a71  .|.j.t.j.....q:q
+00001b00: 3264 0053 0029 074e 7220 0000 00da 1567  2d.S.).Nr .....g
+00001b10: 6574 5f6d 6170 5f63 6f6e 7465 6e74 5f63  et_map_content_c
+00001b20: 6f75 6e74 722d 0000 0072 7100 0000 7252  ountr-...rq...rR
+00001b30: 0000 0072 5300 0000 2912 da0d 6372 6561  ...rS...)...crea
+00001b40: 7465 5f70 6f69 6e74 7372 2300 0000 7224  te_pointsr#...r$
+00001b50: 0000 0072 0200 0000 7235 0000 0072 1100  ...r....r5...r..
+00001b60: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00001b70: 0072 0a00 0000 7255 0000 0072 2f00 0000  .r....rU...r/...
+00001b80: 7256 0000 0072 0500 0000 7257 0000 0072  rV...r....rW...r
+00001b90: 5c00 0000 725d 0000 0072 4400 0000 7272  \...r]...rD...rr
+00001ba0: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
+00001bb0: 0000 7259 0000 0049 0100 0073 2200 0000  ..rY...I...s"...
+00001bc0: 0002 0803 0201 02fe 0605 0c02 0802 1002  ................
+00001bd0: 0803 0201 0201 02fd 0606 1202 0c01 0801  ................
+00001be0: 0a04 7a20 5465 7374 4765 744d 6170 436f  ..z TestGetMapCo
+00001bf0: 6e74 656e 7443 6f75 6e74 2e74 6573 745f  ntentCount.test_
+00001c00: 706f 7374 6301 0000 0000 0000 0000 0000  postc...........
+00001c10: 000a 0000 0007 0000 0043 0000 0073 f200  .........C...s..
+00001c20: 0000 6401 6402 6403 6404 6405 9c03 6701  ..d.d.d.d.d...g.
+00001c30: 6901 6401 6402 6406 6404 6405 9c03 6701  i.d.d.d.d.d...g.
+00001c40: 6901 6407 9c02 7d01 7c00 a000 a100 0100  i.d...}.|.......
+00001c50: 7401 7402 6408 9c02 7d02 7403 6409 7c02  t.t.d...}.t.d.|.
+00001c60: 640a 8d02 7d03 7404 7405 7406 7407 6604  d...}.t.t.t.t.f.
+00001c70: 4400 5d9c 7d04 7c00 a008 a100 7d05 7c05  D.].}.|.....}.|.
+00001c80: 4400 5d8a 7d06 7409 7c04 7c06 7c01 640b  D.].}.t.|.|.|.d.
+00001c90: 9c04 7d07 7c00 6a0a 6a0b 7c03 7c07 640c  ..}.|.j.j.|.|.d.
+00001ca0: 640d 8d03 7d08 7c08 6a0c 740d 6a0e 6b03  d...}.|.j.t.j.k.
+00001cb0: 72a2 740f 7c04 8301 0100 740f 7c08 6a10  r.t.|.....t.|.j.
+00001cc0: 8301 0100 7411 a012 7c08 6a13 a101 7d09  ....t...|.j...}.
+00001cd0: 7c00 a014 640e 7c09 a102 0100 7c00 a014  |...d.|.....|...
+00001ce0: 6403 7c09 640e 1900 a102 0100 7c00 a014  d.|.d.......|...
+00001cf0: 6406 7c09 640e 1900 a102 0100 7c00 a015  d.|.d.......|...
+00001d00: 7c08 6a0c 740d 6a0e a102 0100 7160 7150  |.j.t.j.....q`qP
+00001d10: 6400 5300 290f 4e72 3d00 0000 da05 7374  d.S.).Nr=.....st
+00001d20: 796c 65da 0573 746f 6e65 fa01 3d29 03da  yle..stone..=)..
+00001d30: 0663 6f6c 756d 6eda 0576 616c 7565 da08  .column..value..
+00001d40: 6f70 6572 6174 6f72 da06 666c 6f77 6572  operator..flower
+00001d50: 2902 7277 0000 0072 7c00 0000 7220 0000  ).rw...r|...r ..
+00001d60: 0072 7400 0000 722d 0000 0029 0472 3b00  .rt...r-...).r;.
+00001d70: 0000 724f 0000 0072 3d00 0000 da0b 6d6f  ..rO...r=.....mo
+00001d80: 6475 6c61 7469 6f6e 7372 5200 0000 7253  dulationsrR...rS
+00001d90: 0000 0072 7d00 0000 2916 7275 0000 0072  ...r}...).ru...r
+00001da0: 2300 0000 7224 0000 0072 0200 0000 7211  #...r$...r....r.
+00001db0: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
+00001dc0: 0000 7235 0000 0072 0a00 0000 7255 0000  ..r5...r....rU..
+00001dd0: 0072 2f00 0000 7256 0000 0072 0500 0000  .r/...rV...r....
+00001de0: 7257 0000 0072 5c00 0000 725d 0000 0072  rW...r\...r]...r
+00001df0: 5200 0000 da05 6c6f 6164 73da 0763 6f6e  R.....loads..con
+00001e00: 7465 6e74 7242 0000 0072 4400 0000 290a  tentrB...rD...).
+00001e10: 7226 0000 0072 7d00 0000 7227 0000 0072  r&...r}...r'...r
+00001e20: 3200 0000 724f 0000 0072 3a00 0000 723d  2...rO...r:...r=
+00001e30: 0000 0072 5000 0000 7258 0000 00da 0f70  ...rP...rX.....p
+00001e40: 6172 7365 645f 7265 7370 6f6e 7365 7228  arsed_responser(
+00001e50: 0000 0072 2800 0000 7229 0000 00da 1374  ...r(...r).....t
+00001e60: 6573 745f 706f 7374 5f6d 6f64 756c 6174  est_post_modulat
+00001e70: 6564 6b01 0000 734a 0000 0000 0402 0202  edk...sJ........
+00001e80: 0102 0102 fd04 ff02 ff02 0a02 0202 0102  ................
+00001e90: 0102 fd04 ff02 ff02 f606 1508 0302 0102  ................
+00001ea0: fe06 050c 0210 0208 0208 0302 0102 0102  ................
+00001eb0: 0102 fc06 0712 020c 0108 010a 020c 020c  ................
+00001ec0: 0110 0110 027a 2a54 6573 7447 6574 4d61  .....z*TestGetMa
+00001ed0: 7043 6f6e 7465 6e74 436f 756e 742e 7465  pContentCount.te
+00001ee0: 7374 5f70 6f73 745f 6d6f 6475 6c61 7465  st_post_modulate
+00001ef0: 644e 2905 7249 0000 0072 4a00 0000 724b  dN).rI...rJ...rK
+00001f00: 0000 0072 5900 0000 7281 0000 0072 2800  ...rY...r....r(.
+00001f10: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
+00001f20: 0072 7300 0000 4701 0000 7304 0000 0008  .rs...G...s.....
+00001f30: 0208 2272 7300 0000 6300 0000 0000 0000  .."rs...c.......
+00001f40: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
+00001f50: 0073 1400 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00001f60: 6402 8400 5a03 6403 5300 2904 da19 5465  d...Z.d.S.)...Te
+00001f70: 7374 4765 7447 726f 7570 6564 4d61 7043  stGetGroupedMapC
+00001f80: 6f6e 7465 6e74 7363 0100 0000 0000 0000  ontentsc........
+00001f90: 0000 0000 0b00 0000 0600 0000 4300 0000  ............C...
+00001fa0: 73dc 0000 007c 00a0 00a1 0001 0074 0174  s....|.......t.t
+00001fb0: 0264 019c 027d 0174 0364 027c 0164 038d  .d...}.t.d.|.d..
+00001fc0: 027d 0267 007d 0374 046a 056a 0664 0464  .}.g.}.t.j.j.d.d
+00001fd0: 058d 017d 047c 00a0 077c 04a0 08a1 0064  ...}.|...|.....d
+00001fe0: 066b 04a1 0101 0074 0974 0a74 0b74 0c66  .k.....t.t.t.t.f
+00001ff0: 0444 005d 887d 0574 0d7c 057c 0364 0764  .D.].}.t.|.|.d.d
+00002000: 089c 047d 067c 006a 0e6a 0f7c 027c 0664  ...}.|.j.j.|.|.d
+00002010: 0964 0a8d 037d 077c 076a 1074 116a 126b  .d...}.|.j.t.j.k
+00002020: 0372 9074 137c 0583 0101 0074 137c 076a  .r.t.|.....t.|.j
+00002030: 1483 0101 0074 15a0 167c 076a 17a1 017d  .....t...|.j...}
+00002040: 0874 046a 05a0 18a1 006a 1964 0764 0b64  .t.j.....j.d.d.d
+00002050: 0c8d 027d 097c 0944 005d 107d 0a7c 00a0  ...}.|.D.].}.|..
+00002060: 1a7c 0a7c 08a1 0201 0071 b47c 00a0 1b7c  .|.|.....q.|...|
+00002070: 076a 1074 116a 12a1 0201 0071 4e64 0053  .j.t.j.....qNd.S
+00002080: 0029 0d4e 7220 0000 005a 1867 6574 5f67  .).Nr ...Z.get_g
+00002090: 726f 7570 6564 5f6d 6170 5f63 6f6e 7465  rouped_map_conte
+000020a0: 6e74 7372 2d00 0000 7277 0000 0029 0172  ntsr-...rw...).r
+000020b0: 7600 0000 7201 0000 0072 7600 0000 2904  v...r....rv...).
+000020c0: 723b 0000 0072 4f00 0000 723d 0000 00da  r;...rO...r=....
+000020d0: 0867 726f 7570 5f62 7972 5200 0000 7253  .group_byrR...rS
+000020e0: 0000 0054 2901 da04 666c 6174 291c 7275  ...T)...flat).ru
+000020f0: 0000 0072 2300 0000 7224 0000 0072 0200  ...r#...r$...r..
+00002100: 0000 721b 0000 00da 076f 626a 6563 7473  ..r......objects
+00002110: da06 6669 6c74 6572 7236 0000 0072 6500  ..filterr6...re.
+00002120: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00002130: 0072 1400 0000 720a 0000 0072 5500 0000  .r....r....rU...
+00002140: 722f 0000 0072 5600 0000 7205 0000 0072  r/...rV...r....r
+00002150: 5700 0000 725c 0000 0072 5d00 0000 7252  W...r\...r]...rR
+00002160: 0000 0072 7e00 0000 727f 0000 00da 0361  ...r~...r......a
+00002170: 6c6c da0b 7661 6c75 6573 5f6c 6973 7472  ll..values_listr
+00002180: 4200 0000 7244 0000 0029 0b72 2600 0000  B...rD...).r&...
+00002190: 7227 0000 0072 3200 0000 723d 0000 005a  r'...r2...r=...Z
+000021a0: 0d73 746f 6e65 5f67 6172 6465 6e73 724f  .stone_gardensrO
+000021b0: 0000 0072 5000 0000 7258 0000 0072 8000  ...rP...rX...r..
+000021c0: 0000 da06 7374 796c 6573 7276 0000 0072  ....stylesrv...r
+000021d0: 2800 0000 7228 0000 0072 2900 0000 7259  (...r(...r)...rY
+000021e0: 0000 00a9 0100 0073 2e00 0000 0002 0803  .......s........
+000021f0: 0201 02fe 0605 0c02 0402 0e01 1202 1003  ................
+00002200: 0201 0201 0201 02fc 0607 1202 0c01 0801  ................
+00002210: 0a02 0c01 1402 0801 0e02 7a23 5465 7374  ..........z#Test
+00002220: 4765 7447 726f 7570 6564 4d61 7043 6f6e  GetGroupedMapCon
+00002230: 7465 6e74 732e 7465 7374 5f70 6f73 744e  tents.test_postN
+00002240: 726f 0000 0072 2800 0000 7228 0000 0072  ro...r(...r(...r
+00002250: 2800 0000 7229 0000 0072 8200 0000 a701  (...r)...r......
+00002260: 0000 7302 0000 0008 0272 8200 0000 292f  ..s......r....)/
+00002270: da0b 646a 616e 676f 2e75 726c 7372 0200  ..django.urlsr..
+00002280: 0000 5a13 7265 7374 5f66 7261 6d65 776f  ..Z.rest_framewo
+00002290: 726b 2e74 6573 7472 0300 0000 7204 0000  rk.testr....r...
+000022a0: 00da 0e72 6573 745f 6672 616d 6577 6f72  ...rest_framewor
+000022b0: 6b72 0500 0000 da0a 616e 7963 6c75 7374  kr......anyclust
+000022c0: 6572 7206 0000 005a 1761 6e79 636c 7573  err....Z.anyclus
+000022d0: 7465 722e 4d61 7043 6c75 7374 6572 6572  ter.MapClusterer
+000022e0: 7207 0000 00da 1661 6e79 636c 7573 7465  r......anycluste
+000022f0: 722e 6465 6669 6e69 7469 6f6e 7372 0800  r.definitionsr..
+00002300: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00002310: 0072 0c00 0000 720d 0000 005a 1761 6e79  .r....r....Z.any
+00002320: 636c 7573 7465 722e 7465 7374 732e 6d69  cluster.tests.mi
+00002330: 7869 6e73 720e 0000 0072 0f00 0000 7210  xinsr....r....r.
+00002340: 0000 005a 1761 6e79 636c 7573 7465 722e  ...Z.anycluster.
+00002350: 7465 7374 732e 636f 6d6d 6f6e 7211 0000  tests.commonr...
+00002360: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00002370: 5a14 616e 7963 6c75 7374 6572 2e61 7069  Z.anycluster.api
+00002380: 2e76 6965 7773 7215 0000 0072 1600 0000  .viewsr....r....
+00002390: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+000023a0: 1a00 0000 5a0d 616e 796d 6170 2e6d 6f64  ....Z.anymap.mod
+000023b0: 656c 7372 1b00 0000 7252 0000 005a 0c4d  elsr....rR...Z.M
+000023c0: 4150 5f54 494c 4553 495a 4572 2400 0000  AP_TILESIZEr$...
+000023d0: 7223 0000 0072 1e00 0000 724c 0000 0072  r#...r....rL...r
+000023e0: 5a00 0000 725e 0000 0072 7000 0000 7273  Z...r^...rp...rs
+000023f0: 0000 0072 8200 0000 7228 0000 0072 2800  ...r....r(...r(.
+00002400: 0000 7228 0000 0072 2900 0000 da08 3c6d  ..r(...r).....<m
+00002410: 6f64 756c 653e 0100 0000 7328 0000 000c  odule>....s(....
+00002420: 0110 010c 020c 010c 0120 0314 0118 0220  ......... ..... 
+00002430: 040c 0208 0204 0104 0104 0212 5914 2714  ............Y.'.
+00002440: 3a14 5314 2114 60                        :.S.!.`
```

### Comparing `anycluster-2.1.1/anycluster/api/tests/test_serializers.py` & `anycluster-2.2.0/anycluster/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/api/tests/test_views.py` & `anycluster-2.2.0/anycluster/api/tests/test_views.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,24 @@
 from rest_framework import status
 
 from anycluster import ClusterCache
 from anycluster.MapClusterer import MapClusterer
 from anycluster.definitions import (CLUSTER_TYPES, GEOMETRY_TYPE_VIEWPORT, GEOMETRY_TYPE_AREA, GEOMETRY_TYPES,
                                     CLUSTER_TYPE_KMEANS, CLUSTER_TYPE_GRID)
 
-from anycluster.tests.mixins import WithGIS, WithFilters
+from anycluster.tests.mixins import WithGIS, WithFilters, WithGardens
 from anycluster.tests.common import GEOJSON_RECTANGLE, GEOJSON_POLYGON, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION
 
-from anycluster.api.views import MapClusterViewBase, KmeansCluster, GridCluster, GetClusterContent, GetAreaContent 
+from anycluster.api.views import (MapClusterViewBase, KmeansCluster, GridCluster, GetClusterContent, GetAreaContent,
+                                    GetMapContentCount)
+
+
+from anymap.models import Gardens
+
+import json
 
 MAP_TILESIZE = 256
 GRID_SIZE = 256
 ZOOM = 10
 
 class TestMapClusterViewBase(WithFilters, APITestCase):
 
@@ -310,8 +316,147 @@
 
                 response = self.client.post(url, post_data, format='json')
 
                 if response.status_code != status.HTTP_200_OK:
                     print(geojson)
                     print(response.data)
                     
-                self.assertEqual(response.status_code, status.HTTP_200_OK)
+                self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
+
+class TestGetMapContentCount(WithGardens, WithFilters, APITestCase):
+
+    def test_post(self):
+
+        self.create_points()
+        
+        url_kwargs = {
+            'zoom': ZOOM,
+            'grid_size': GRID_SIZE,
+        }
+
+        url = reverse('get_map_content_count', kwargs=url_kwargs)
+
+        filter_lists = self.get_test_filters()
+        
+        for geojson in [GEOJSON_RECTANGLE, GEOJSON_POLYGON, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION]:
+
+            for filters in filter_lists:
+
+                post_data = {
+                    'geometry_type': GEOMETRY_TYPE_AREA,
+                    'geojson': geojson,
+                    'filters': filters,
+                }
+
+                response = self.client.post(url, post_data, format='json')
+
+                if response.status_code != status.HTTP_200_OK:
+                    print(geojson)
+                    print(response.data)
+
+                # print(json.loads(response.content))
+                    
+                self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
+    def test_post_modulated(self):
+        
+        modulations = {
+            'stone' : {
+                'filters' : [
+                    {
+                        'column': 'style',
+                        'value': 'stone',
+                        'operator': '=',
+                    }
+                ]
+            },
+            'flower' : {
+                'filters' : [
+                    {
+                        'column': 'style',
+                        'value': 'flower',
+                        'operator': '=',
+                    }
+                ]
+            }
+        }
+
+        self.create_points()
+        
+        url_kwargs = {
+            'zoom': ZOOM,
+            'grid_size': GRID_SIZE,
+        }
+
+        url = reverse('get_map_content_count', kwargs=url_kwargs)
+
+        for geojson in [GEOJSON_RECTANGLE, GEOJSON_POLYGON, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION]:
+
+            filter_lists = self.get_test_filters()
+
+            for filters in filter_lists:
+
+                post_data = {
+                    'geometry_type': GEOMETRY_TYPE_AREA,
+                    'geojson': geojson,
+                    'filters': filters,
+                    'modulations': modulations
+                }
+
+                response = self.client.post(url, post_data, format='json')
+
+                if response.status_code != status.HTTP_200_OK:
+                    print(geojson)
+                    print(response.data)
+
+                parsed_response = json.loads(response.content)
+                #print(parsed_response)
+                self.assertIn('modulations', parsed_response)
+                self.assertIn('stone', parsed_response['modulations'])
+                self.assertIn('flower', parsed_response['modulations'])
+                    
+                self.assertEqual(response.status_code, status.HTTP_200_OK)
+
+
+class TestGetGroupedMapContents(WithGardens, WithFilters, APITestCase):
+
+    def test_post(self):
+
+        self.create_points()
+        
+        url_kwargs = {
+            'zoom': ZOOM,
+            'grid_size': GRID_SIZE,
+        }
+
+        url = reverse('get_grouped_map_contents', kwargs=url_kwargs)
+
+        filters = []
+
+        stone_gardens = Gardens.objects.filter(style='stone')
+        self.assertTrue(stone_gardens.count() > 0)
+        
+        for geojson in [GEOJSON_RECTANGLE, GEOJSON_POLYGON, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION]:
+
+            post_data = {
+                'geometry_type': GEOMETRY_TYPE_AREA,
+                'geojson': geojson,
+                'filters': filters,
+                'group_by': 'style'
+            }
+
+            response = self.client.post(url, post_data, format='json')
+
+            if response.status_code != status.HTTP_200_OK:
+                print(geojson)
+                print(response.data)
+
+            parsed_response = json.loads(response.content)
+            styles = Gardens.objects.all().values_list('style', flat=True)
+
+            for style in styles:
+                self.assertIn(style, parsed_response)
+                
+            self.assertEqual(response.status_code, status.HTTP_200_OK)
```

### Comparing `anycluster-2.1.1/anycluster/api/urls.py` & `anycluster-2.2.0/anycluster/api/urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,10 +9,14 @@
     path('kmeans/<int:zoom>/<int:grid_size>/', views.KmeansCluster.as_view(), name='kmeans_cluster'),
     path('get-kmeans-cluster-content/<int:zoom>/<int:grid_size>/', views.GetClusterContent.as_view(),
         name='get_kmeans_cluster_content'),
     path('get-area-content/<int:zoom>/<int:grid_size>/', views.GetAreaContent.as_view(),
         name='get_area_content'),
     path('get-dataset-content/<int:zoom>/<int:grid_size>/<int:dataset_id>/', views.GetDatasetContent.as_view(),
         name='get_dataset_content'),
+    path('get-map-content-count/<int:zoom>/<int:grid_size>/', views.GetMapContentCount.as_view(),
+        name='get_map_content_count'),
+    path('get-grouped-map-contents/<int:zoom>/<int:grid_size>/', views.GetGroupedMapContents.as_view(),
+        name='get_grouped_map_contents'),
 ]
 
 urlpatterns = format_suffix_patterns(urlpatterns, allowed=['json'])
```

### Comparing `anycluster-2.1.1/anycluster/api/views.py` & `anycluster-2.2.0/anycluster/api/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from rest_framework.response import Response
 from rest_framework.renderers import JSONRenderer
 from rest_framework import status
 
 from anycluster.MapClusterer import MapClusterer
 from anycluster.definitions import GEOMETRY_TYPE_VIEWPORT, GEOMETRY_TYPE_AREA, CLUSTER_TYPE_GRID, CLUSTER_TYPE_KMEANS
 
-from .serializers import ClusterRequestSerializer, ClusterContentRequestSerializer
+from .serializers import (ClusterRequestSerializer, ClusterContentRequestSerializer, MapContentCountSerializer,
+                            GroupedMapContentSerializer)
 
 from anycluster import ClusterCache
 
 import json
 
 class APIHome(APIView):
 
@@ -35,26 +36,26 @@
 
     def get_map_clusterer(self, geometry_type, clustertype, filters, clear_cache, output_srid, request, **kwargs):
 
         grid_size = kwargs['grid_size']
         zoom = kwargs['zoom']
 
         if clear_cache == True:
-            cluster_cache = ClusterCache(geometry_type, zoom, clustertype, filters=filters)
+            cluster_cache = ClusterCache(geometry_type, zoom, clustertype, filters)
         else:
             cluster_cache = self.get_cache(geometry_type, zoom, clustertype, request, filters)
 
         schema_name = self.get_schema_name(request)
         clusterer = MapClusterer(cluster_cache, grid_size=grid_size, output_srid=output_srid, schema_name=schema_name)
         return clusterer
 
 
     def get_cache(self, geometry_type, zoom, clustertype, request, filters):
         cached = request.session.get(self.cache_name, {})
-        cluster_cache = ClusterCache(geometry_type, zoom, clustertype, filters=filters)
+        cluster_cache = ClusterCache(geometry_type, zoom, clustertype, filters)
         # ClusterCache decides if the cache is still valid for the given parameters and loads the cache if so
         cluster_cache.load_geometries(cached)
         return cluster_cache
 
 
     def set_cache(self, request, cluster_cache):
         cluster_cache_json = cluster_cache.serialize()
@@ -213,8 +214,63 @@
         dataset_id = kwargs['dataset_id']
 
         dataset = map_clusterer.get_dataset_content(dataset_id)
 
         serializer_fields = map_clusterer.get_gis_field_names()
         data = serializers.serialize('json', dataset, fields=serializer_fields)
 
-        return Response(json.loads(data))
+        return Response(json.loads(data))
+
+
+class GetMapContentCount(MapClusterViewBase, APIView):
+
+    def post(self, request, *args, **kwargs):
+
+        serializer = MapContentCountSerializer(data=request.data)
+
+        if serializer.is_valid():
+
+            clear_cache = True
+            filters = serializer.validated_data['filters']
+            geometry_type = serializer.validated_data['geometry_type']
+            output_srid = self.parse_srid(serializer.validated_data['output_srid'])
+
+            geojson = serializer.validated_data['geojson']
+            zoom = kwargs['zoom']
+            modulations = serializer.validated_data['modulations']
+
+            map_clusterer = self.get_map_clusterer(geometry_type, CLUSTER_TYPE_KMEANS, filters, clear_cache, output_srid,
+                request, **kwargs)
+
+            map_content_counts = map_clusterer.get_map_content_counts(geojson, geometry_type, filters, zoom, modulations)
+
+            return Response(map_content_counts, status=status.HTTP_200_OK)
+
+        return Response(serializer.errors, status=status.HTTP_400_BAD_REQUEST)
+
+
+class GetGroupedMapContents(MapClusterViewBase, APIView):
+    
+    def post(self, request, *args, **kwargs):
+        
+        serializer = GroupedMapContentSerializer(data=request.data)
+
+        if serializer.is_valid():
+
+            clear_cache = True
+            filters = serializer.validated_data['filters']
+            geometry_type = serializer.validated_data['geometry_type']
+            output_srid = self.parse_srid(serializer.validated_data['output_srid'])
+
+            geojson = serializer.validated_data['geojson']
+            zoom = kwargs['zoom']
+
+            group_by = serializer.validated_data['group_by']
+
+            map_clusterer = self.get_map_clusterer(geometry_type, CLUSTER_TYPE_KMEANS, filters, clear_cache, output_srid,
+                request, **kwargs)
+
+            groups = map_clusterer.get_grouped_map_contents(geojson, geometry_type, zoom, filters, group_by)
+
+            return Response(groups, status=status.HTTP_200_OK)
+            
+        return Response(serializer.errors, status=status.HTTP_400_BAD_REQUEST)
```

### Comparing `anycluster-2.1.1/anycluster/clusters.py` & `anycluster-2.2.0/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/definitions.py` & `anycluster-2.2.0/anycluster/definitions.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/globalmaptiles.py` & `anycluster-2.2.0/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/10.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/100.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/1000.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/10000.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/5.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/50.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.2.0/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.2.0/anycluster/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/tests/__pycache__/mixins.cpython-38.pyc` & `anycluster-2.2.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Apr 19 10:47:07 2023 UTC, .py size: 2096 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,180 @@
-00000000: 550d 0d0a 0000 0000 abc6 3f64 3008 0000  U.........?d0...
+00000000: 550d 0d0a 0000 0000 ce46 7064 b608 0000  U........Fpd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 9c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6400  d.l.m.Z.m.Z...d.
 00000080: 6407 6c0e 5a0e 6400 6407 6c0f 5a0f 6400  d.l.Z.d.d.l.Z.d.
 00000090: 6408 6c10 6d11 5a11 0100 4700 6409 640a  d.l.m.Z...G.d.d.
 000000a0: 8400 640a 8302 5a12 4700 640b 640c 8400  ..d...Z.G.d.d...
-000000b0: 640c 8302 5a13 6407 5300 290d e900 0000  d...Z.d.S.).....
-000000c0: 0029 01da 0873 6574 7469 6e67 7329 01da  .)...settings)..
-000000d0: 0550 6f69 6e74 2902 da10 5370 6174 6961  .Point)...Spatia
-000000e0: 6c52 6566 6572 656e 6365 da0e 436f 6f72  lReference..Coor
-000000f0: 6454 7261 6e73 666f 726d 2901 da08 7469  dTransform)...ti
-00000100: 6d65 7a6f 6e65 a901 da0c 436c 7573 7465  mezone....Cluste
-00000110: 7243 6163 6865 2902 da07 4761 7264 656e  rCache)...Garden
-00000120: 73da 0d47 4152 4445 4e5f 5354 594c 4553  s..GARDEN_STYLES
-00000130: 4ea9 01da 0d56 414c 4944 5f46 494c 5445  N....VALID_FILTE
-00000140: 5253 6300 0000 0000 0000 0000 0000 0000  RSc.............
-00000150: 0000 0004 0000 0000 0000 0073 3e00 0000  ...........s>...
-00000160: 6500 5a01 6400 5a02 8700 6601 6401 6402  e.Z.d.Z...f.d.d.
-00000170: 8408 5a03 640a 6404 6405 8401 5a04 6505  ..Z.d.d.d...Z.e.
-00000180: 8700 6601 6406 6407 8408 8301 5a06 6408  ..f.d.d.....Z.d.
-00000190: 6409 8400 5a07 8700 0400 5a08 5300 290b  d...Z.....Z.S.).
-000001a0: da07 5769 7468 4749 5363 0100 0000 0000  ..WithGISc......
-000001b0: 0000 0000 0000 0100 0000 0200 0000 0300  ................
-000001c0: 0000 7316 0000 0074 0083 00a0 01a1 0001  ..s....t........
-000001d0: 007c 00a0 02a1 0001 0064 0053 00a9 014e  .|.......d.S...N
-000001e0: 2903 da05 7375 7065 72da 0573 6574 5570  )...super..setUp
-000001f0: da0d 6372 6561 7465 5f70 6f69 6e74 7329  ..create_points)
-00000200: 01da 0473 656c 66a9 01da 095f 5f63 6c61  ...self....__cla
-00000210: 7373 5f5f a900 fa3b 2f68 6f6d 652f 746f  ss__...;/home/to
-00000220: 6d2f 616e 7963 6c75 7374 6572 2f64 656d  m/anycluster/dem
-00000230: 6f2f 646a 616e 676f 2f61 6e79 636c 7573  o/django/anyclus
-00000240: 7465 722f 7465 7374 732f 6d69 7869 6e73  ter/tests/mixins
-00000250: 2e70 7972 1000 0000 1100 0000 7304 0000  .pyr........s...
-00000260: 0000 010a 017a 0d57 6974 6847 4953 2e73  .....z.WithGIS.s
-00000270: 6574 5570 e964 0000 0063 0200 0000 0000  etUp.d...c......
-00000280: 0000 0000 0000 0a00 0000 0800 0000 4300  ..............C.
-00000290: 0000 73d8 0000 0074 0064 017c 0183 0244  ..s....t.d.|...D
-000002a0: 005d c87d 0274 0164 02a0 0274 03a0 0464  .].}.t.d...t...d
-000002b0: 0364 04a1 0274 0574 03a0 03a1 0083 01a0  .d...t.t........
-000002c0: 0664 05a1 0164 0619 00a1 0283 017d 0374  .d...d.......}.t
-000002d0: 0164 02a0 0274 03a0 0464 0764 08a1 0274  .d...t...d.d...t
-000002e0: 0574 03a0 03a1 0083 01a0 0664 05a1 0164  .t.........d...d
-000002f0: 0619 00a1 0283 017d 0474 077c 047c 0364  .......}.t.|.|.d
-00000300: 0964 0a8d 037d 0574 0874 097c 056a 0a83  .d...}.t.t.|.j..
-00000310: 0174 0964 0b83 0183 027d 067c 05a0 0b7c  .t.d.....}.|...|
-00000320: 06a1 0101 0074 03a0 0464 0164 0ca1 027d  .....t...d.d...}
-00000330: 0774 0c7c 0719 0064 0119 007d 0874 0d64  .t.|...d...}.t.d
-00000340: 0da0 027c 02a1 017c 0874 03a0 0464 0e64  ...|...|.t...d.d
-00000350: 0fa1 0274 0ea0 0fa1 007c 0564 108d 057d  ...t.....|.d...}
-00000360: 097c 09a0 10a1 0001 0071 0a64 0053 0029  .|.......q.d.S.)
-00000370: 114e 7201 0000 007a 077b 307d 2e7b 317d  .Nr....z.{0}.{1}
-00000380: e930 0000 00e9 3100 0000 da01 2ee9 ffff  .0....1.........
-00000390: ffff e909 0000 00e9 0d00 0000 69e6 1000  ............i...
-000003a0: 0029 01da 0473 7269 6469 110f 0000 e904  .)...sridi......
-000003b0: 0000 007a 0f74 6573 7420 6761 7264 656e  ...z.test garden
-000003c0: 207b 307d e901 0000 00e9 0500 0000 2905   {0}..........).
-000003d0: da04 6e61 6d65 da05 7374 796c 65da 0672  ..name..style..r
-000003e0: 6174 696e 67da 0c6c 6173 745f 7265 6e65  ating..last_rene
-000003f0: 7761 6cda 0b63 6f6f 7264 696e 6174 6573  wal..coordinates
-00000400: 2911 da05 7261 6e67 65da 0566 6c6f 6174  )...range..float
-00000410: da06 666f 726d 6174 da06 7261 6e64 6f6d  ..format..random
-00000420: da07 7261 6e64 696e 74da 0373 7472 da05  ..randint..str..
-00000430: 7370 6c69 7472 0300 0000 7205 0000 0072  splitr....r....r
-00000440: 0400 0000 721e 0000 00da 0974 7261 6e73  ....r......trans
-00000450: 666f 726d 720a 0000 0072 0900 0000 7206  formr....r....r.
-00000460: 0000 00da 036e 6f77 da04 7361 7665 290a  .....now..save).
-00000470: 7212 0000 00da 0661 6d6f 756e 74da 0163  r......amount..c
-00000480: 5a08 6c61 7469 7475 6465 5a09 6c6f 6e67  Z.latitudeZ.long
-00000490: 6974 7564 65da 0570 6f69 6e74 da02 6374  itude..point..ct
-000004a0: 5a0b 7374 796c 655f 696e 6465 7872 2300  Z.style_indexr#.
-000004b0: 0000 da06 6761 7264 656e 7215 0000 0072  ....gardenr....r
-000004c0: 1500 0000 7216 0000 0072 1100 0000 1600  ....r....r......
-000004d0: 0000 7320 0000 0000 020e 032a 012a 020e  ..s .......*.*..
-000004e0: 0214 010a 020c 010c 0202 0108 0102 010a  ................
-000004f0: 0106 0102 fb06 087a 1557 6974 6847 4953  .......z.WithGIS
-00000500: 2e63 7265 6174 655f 706f 696e 7473 6301  .create_pointsc.
-00000510: 0000 0000 0000 0000 0000 0002 0000 0007  ................
-00000520: 0000 0003 0000 0073 4200 0000 7400 8300  .......sB...t...
-00000530: a001 a100 0100 7402 6a03 6401 1900 6402  ......t.j.d...d.
-00000540: 1900 7d01 7c01 a004 6403 a101 732a 7405  ..}.|...d...s*t.
-00000550: 6404 8301 8201 7406 a007 6405 6406 6407  d.....t...d.d.d.
-00000560: 6408 7c01 6705 a101 0100 6400 5300 2909  d.|.g.....d.S.).
-00000570: 4eda 0764 6566 6175 6c74 da04 4e41 4d45  N..default..NAME
-00000580: da05 7465 7374 5f7a 1d4e 6f74 2061 2074  ..test_z.Not a t
-00000590: 6573 7420 6461 7461 6261 7365 2c20 6162  est database, ab
-000005a0: 6f72 7469 6e67 da04 7073 716c 7a02 2d66  orting..psqlz.-f
-000005b0: 7a2c 2f75 7372 2f73 6861 7265 2f70 6f73  z,/usr/share/pos
-000005c0: 7467 7265 7371 6c31 352f 6578 7465 6e73  tgresql15/extens
-000005d0: 696f 6e2f 6b6d 6561 6e73 2e73 716c 7a02  ion/kmeans.sqlz.
-000005e0: 2d64 2908 720f 0000 00da 0a73 6574 5570  -d).r......setUp
-000005f0: 436c 6173 7372 0200 0000 da09 4441 5441  Classr......DATA
-00000600: 4241 5345 53da 0a73 7461 7274 7377 6974  BASES..startswit
-00000610: 68da 0a56 616c 7565 4572 726f 72da 0a73  h..ValueError..s
-00000620: 7562 7072 6f63 6573 73da 0372 756e 2902  ubprocess..run).
-00000630: da03 636c 73da 1274 6573 745f 6461 7461  ..cls..test_data
-00000640: 6261 7365 5f6e 616d 6572 1300 0000 7215  base_namer....r.
-00000650: 0000 0072 1600 0000 723a 0000 0031 0000  ...r....r:...1..
-00000660: 0073 0a00 0000 0002 0a02 0e02 0a01 0802  .s..............
-00000670: 7a12 5769 7468 4749 532e 7365 7455 7043  z.WithGIS.setUpC
-00000680: 6c61 7373 6305 0000 0000 0000 0000 0000  lassc...........
-00000690: 0006 0000 0005 0000 0043 0000 0073 1200  .........C...s..
-000006a0: 0000 7400 7c01 7c02 7c03 7c04 8304 7d05  ..t.|.|.|.|...}.
-000006b0: 7c05 5300 720e 0000 0072 0700 0000 2906  |.S.r....r....).
-000006c0: 7212 0000 00da 0d67 656f 6d65 7472 795f  r......geometry_
-000006d0: 7479 7065 da04 7a6f 6f6d da0b 636c 7573  type..zoom..clus
-000006e0: 7465 7274 7970 65da 0766 696c 7465 7273  tertype..filters
-000006f0: da0d 636c 7573 7465 725f 6361 6368 6572  ..cluster_cacher
-00000700: 1500 0000 7215 0000 0072 1600 0000 da11  ....r....r......
-00000710: 6765 745f 636c 7573 7465 725f 6361 6368  get_cluster_cach
-00000720: 653d 0000 0073 0400 0000 0002 0e02 7a19  e=...s........z.
-00000730: 5769 7468 4749 532e 6765 745f 636c 7573  WithGIS.get_clus
-00000740: 7465 725f 6361 6368 6529 0172 1700 0000  ter_cache).r....
-00000750: 2909 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000760: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000770: 6e61 6d65 5f5f 7210 0000 0072 1100 0000  name__r....r....
-00000780: da0b 636c 6173 736d 6574 686f 6472 3a00  ..classmethodr:.
-00000790: 0000 7247 0000 00da 0d5f 5f63 6c61 7373  ..rG.....__class
-000007a0: 6365 6c6c 5f5f 7215 0000 0072 1500 0000  cell__r....r....
-000007b0: 7213 0000 0072 1600 0000 720d 0000 000f  r....r....r.....
-000007c0: 0000 0073 0a00 0000 0802 0c05 0a1b 0201  ...s............
-000007d0: 0e0b 720d 0000 0063 0000 0000 0000 0000  ..r....c........
-000007e0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
-000007f0: 7314 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
-00000800: 0284 005a 0364 0353 0029 04da 0b57 6974  ...Z.d.S.)...Wit
-00000810: 6846 696c 7465 7273 6301 0000 0000 0000  hFiltersc.......
-00000820: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-00000830: 0073 0c00 0000 6700 7400 6702 7d01 7c01  .s....g.t.g.}.|.
-00000840: 5300 720e 0000 0072 0b00 0000 2902 7212  S.r....r....).r.
-00000850: 0000 0072 4500 0000 7215 0000 0072 1500  ...rE...r....r..
-00000860: 0000 7216 0000 00da 1067 6574 5f74 6573  ..r......get_tes
-00000870: 745f 6669 6c74 6572 7346 0000 0073 0800  t_filtersF...s..
-00000880: 0000 0003 0201 02fe 0405 7a1c 5769 7468  ..........z.With
-00000890: 4669 6c74 6572 732e 6765 745f 7465 7374  Filters.get_test
-000008a0: 5f66 696c 7465 7273 4e29 0472 4800 0000  _filtersN).rH...
-000008b0: 7249 0000 0072 4a00 0000 724e 0000 0072  rI...rJ...rN...r
-000008c0: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-000008d0: 0000 0072 4d00 0000 4400 0000 7302 0000  ...rM...D...s...
-000008e0: 0008 0272 4d00 0000 2914 da0b 646a 616e  ...rM...)...djan
-000008f0: 676f 2e63 6f6e 6672 0200 0000 da17 646a  go.confr......dj
-00000900: 616e 676f 2e63 6f6e 7472 6962 2e67 6973  ango.contrib.gis
-00000910: 2e67 656f 7372 0300 0000 da17 646a 616e  .geosr......djan
-00000920: 676f 2e63 6f6e 7472 6962 2e67 6973 2e67  go.contrib.gis.g
-00000930: 6461 6c72 0400 0000 7205 0000 00da 0c64  dalr....r......d
-00000940: 6a61 6e67 6f2e 7574 696c 7372 0600 0000  jango.utilsr....
-00000950: da0a 616e 7963 6c75 7374 6572 7208 0000  ..anyclusterr...
-00000960: 00da 0d61 6e79 6d61 702e 6d6f 6465 6c73  ...anymap.models
-00000970: 7209 0000 0072 0a00 0000 723e 0000 0072  r....r....r>...r
-00000980: 2a00 0000 da17 616e 7963 6c75 7374 6572  *.....anycluster
-00000990: 2e74 6573 7473 2e63 6f6d 6d6f 6e72 0c00  .tests.commonr..
-000009a0: 0000 720d 0000 0072 4d00 0000 7215 0000  ..r....rM...r...
-000009b0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-000009c0: da08 3c6d 6f64 756c 653e 0100 0000 7312  ..<module>....s.
-000009d0: 0000 000c 010c 0110 010c 020c 0210 0210  ................
-000009e0: 020c 030e 35                             ....5
+000000b0: 640c 6512 8303 5a13 4700 640d 640e 8400  d.e...Z.G.d.d...
+000000c0: 640e 8302 5a14 6407 5300 290f e900 0000  d...Z.d.S.).....
+000000d0: 0029 01da 0873 6574 7469 6e67 7329 01da  .)...settings)..
+000000e0: 0550 6f69 6e74 2902 da10 5370 6174 6961  .Point)...Spatia
+000000f0: 6c52 6566 6572 656e 6365 da0e 436f 6f72  lReference..Coor
+00000100: 6454 7261 6e73 666f 726d 2901 da08 7469  dTransform)...ti
+00000110: 6d65 7a6f 6e65 a901 da0c 436c 7573 7465  mezone....Cluste
+00000120: 7243 6163 6865 2902 da07 4761 7264 656e  rCache)...Garden
+00000130: 73da 0d47 4152 4445 4e5f 5354 594c 4553  s..GARDEN_STYLES
+00000140: 4ea9 01da 0d56 414c 4944 5f46 494c 5445  N....VALID_FILTE
+00000150: 5253 6300 0000 0000 0000 0000 0000 0000  RSc.............
+00000160: 0000 0003 0000 0040 0000 0073 2600 0000  .......@...s&...
+00000170: 6500 5a01 6400 5a02 6409 6402 6403 8401  e.Z.d.Z.d.d.d...
+00000180: 5a03 6404 6405 8400 5a04 6406 6407 8400  Z.d.d...Z.d.d...
+00000190: 5a05 6408 5300 290a da0b 5769 7468 4761  Z.d.S.)...WithGa
+000001a0: 7264 656e 73e9 6400 0000 6302 0000 0000  rdens.d...c.....
+000001b0: 0000 0000 0000 0007 0000 0005 0000 0043  ...............C
+000001c0: 0000 0073 4200 0000 7400 6401 7c01 8302  ...sB...t.d.|...
+000001d0: 4400 5d32 7d02 7401 a002 6401 6402 a102  D.]2}.t...d.d...
+000001e0: 7d03 7403 7c03 1900 6401 1900 7d04 6403  }.t.|...d...}.d.
+000001f0: a004 7c02 a101 7d05 7c00 a005 7c05 7c04  ..|...}.|...|.|.
+00000200: a102 7d06 710a 6400 5300 2904 4e72 0100  ..}.q.d.S.).Nr..
+00000210: 0000 e904 0000 007a 0f74 6573 7420 6761  .......z.test ga
+00000220: 7264 656e 207b 307d 2906 da05 7261 6e67  rden {0})...rang
+00000230: 65da 0672 616e 646f 6dda 0772 616e 6469  e..random..randi
+00000240: 6e74 720a 0000 00da 0666 6f72 6d61 74da  ntr......format.
+00000250: 0c63 7265 6174 655f 706f 696e 7429 07da  .create_point)..
+00000260: 0473 656c 66da 0661 6d6f 756e 74da 0163  .self..amount..c
+00000270: 5a0b 7374 796c 655f 696e 6465 78da 0573  Z.style_index..s
+00000280: 7479 6c65 da04 6e61 6d65 da06 6761 7264  tyle..name..gard
+00000290: 656e a900 721b 0000 00fa 3b2f 686f 6d65  en..r.....;/home
+000002a0: 2f74 6f6d 2f61 6e79 636c 7573 7465 722f  /tom/anycluster/
+000002b0: 6465 6d6f 2f64 6a61 6e67 6f2f 616e 7963  demo/django/anyc
+000002c0: 6c75 7374 6572 2f74 6573 7473 2f6d 6978  luster/tests/mix
+000002d0: 696e 732e 7079 da0d 6372 6561 7465 5f70  ins.py..create_p
+000002e0: 6f69 6e74 7311 0000 0073 0a00 0000 0002  oints....s......
+000002f0: 0e02 0c01 0c02 0a02 7a19 5769 7468 4761  ........z.WithGa
+00000300: 7264 656e 732e 6372 6561 7465 5f70 6f69  rdens.create_poi
+00000310: 6e74 7363 0300 0000 0000 0000 0000 0000  ntsc............
+00000320: 0800 0000 0700 0000 4300 0000 73aa 0000  ........C...s...
+00000330: 0074 0064 01a0 0174 02a0 0364 0264 03a1  .t.d...t...d.d..
+00000340: 0274 0474 02a0 02a1 0083 01a0 0564 04a1  .t.t.........d..
+00000350: 0164 0519 00a1 0283 017d 0374 0064 01a0  .d.......}.t.d..
+00000360: 0174 02a0 0364 0664 07a1 0274 0474 02a0  .t...d.d...t.t..
+00000370: 02a1 0083 01a0 0564 04a1 0164 0519 00a1  .......d...d....
+00000380: 0283 017d 0474 067c 047c 0364 0864 098d  ...}.t.|.|.d.d..
+00000390: 037d 0574 0774 087c 056a 0983 0174 0864  .}.t.t.|.j...t.d
+000003a0: 0a83 0183 027d 067c 05a0 0a7c 06a1 0101  .....}.|...|....
+000003b0: 0074 0b7c 017c 0274 02a0 0364 0b64 0ca1  .t.|.|.t...d.d..
+000003c0: 0274 0ca0 0da1 007c 0564 0d8d 057d 077c  .t.....|.d...}.|
+000003d0: 07a0 0ea1 0001 007c 0753 0029 0e4e 7a07  .......|.S.).Nz.
+000003e0: 7b30 7d2e 7b31 7de9 3000 0000 e931 0000  {0}.{1}.0....1..
+000003f0: 00da 012e e9ff ffff ffe9 0900 0000 e90d  ................
+00000400: 0000 0069 e610 0000 2901 da04 7372 6964  ...i....)...srid
+00000410: 6911 0f00 00e9 0100 0000 e905 0000 0029  i..............)
+00000420: 0572 1900 0000 7218 0000 00da 0672 6174  .r....r......rat
+00000430: 696e 67da 0c6c 6173 745f 7265 6e65 7761  ing..last_renewa
+00000440: 6cda 0b63 6f6f 7264 696e 6174 6573 290f  l..coordinates).
+00000450: da05 666c 6f61 7472 1300 0000 7211 0000  ..floatr....r...
+00000460: 0072 1200 0000 da03 7374 72da 0573 706c  .r......str..spl
+00000470: 6974 7203 0000 0072 0500 0000 7204 0000  itr....r....r...
+00000480: 0072 2400 0000 da09 7472 616e 7366 6f72  .r$.....transfor
+00000490: 6d72 0900 0000 7206 0000 00da 036e 6f77  mr....r......now
+000004a0: da04 7361 7665 2908 7215 0000 0072 1900  ..save).r....r..
+000004b0: 0000 7218 0000 005a 086c 6174 6974 7564  ..r....Z.latitud
+000004c0: 655a 096c 6f6e 6769 7475 6465 da05 706f  eZ.longitude..po
+000004d0: 696e 74da 0263 7472 1a00 0000 721b 0000  int..ctr....r...
+000004e0: 0072 1b00 0000 721c 0000 0072 1400 0000  .r....r....r....
+000004f0: 1d00 0000 731c 0000 0000 022a 012a 020e  ....s......*.*..
+00000500: 0214 010a 0202 0102 0102 010a 0106 0102  ................
+00000510: fb06 0808 027a 1857 6974 6847 6172 6465  .....z.WithGarde
+00000520: 6e73 2e63 7265 6174 655f 706f 696e 7463  ns.create_pointc
+00000530: 0500 0000 0000 0000 0000 0000 0600 0000  ................
+00000540: 0500 0000 4300 0000 7312 0000 0074 007c  ....C...s....t.|
+00000550: 017c 027c 037c 0483 047d 057c 0553 00a9  .|.|.|...}.|.S..
+00000560: 014e 7207 0000 0029 0672 1500 0000 da0d  .Nr....).r......
+00000570: 6765 6f6d 6574 7279 5f74 7970 65da 047a  geometry_type..z
+00000580: 6f6f 6dda 0b63 6c75 7374 6572 7479 7065  oom..clustertype
+00000590: da07 6669 6c74 6572 73da 0d63 6c75 7374  ..filters..clust
+000005a0: 6572 5f63 6163 6865 721b 0000 0072 1b00  er_cacher....r..
+000005b0: 0000 721c 0000 00da 1167 6574 5f63 6c75  ..r......get_clu
+000005c0: 7374 6572 5f63 6163 6865 3300 0000 7304  ster_cache3...s.
+000005d0: 0000 0000 020e 027a 1d57 6974 6847 6172  .......z.WithGar
+000005e0: 6465 6e73 2e67 6574 5f63 6c75 7374 6572  dens.get_cluster
+000005f0: 5f63 6163 6865 4e29 0172 0e00 0000 2906  _cacheN).r....).
+00000600: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000610: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000620: 6d65 5f5f 721d 0000 0072 1400 0000 7238  me__r....r....r8
+00000630: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
+00000640: 0000 721c 0000 0072 0d00 0000 0f00 0000  ..r....r........
+00000650: 7306 0000 0008 020a 0c08 1672 0d00 0000  s..........r....
+00000660: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000670: 0004 0000 0000 0000 0073 2c00 0000 6500  .........s,...e.
+00000680: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
+00000690: 5a03 6504 8700 6601 6403 6404 8408 8301  Z.e...f.d.d.....
+000006a0: 5a05 8700 0400 5a06 5300 2905 da07 5769  Z.....Z.S.)...Wi
+000006b0: 7468 4749 5363 0100 0000 0000 0000 0000  thGISc..........
+000006c0: 0000 0100 0000 0200 0000 0300 0000 7316  ..............s.
+000006d0: 0000 0074 0083 00a0 01a1 0001 007c 00a0  ...t.........|..
+000006e0: 02a1 0001 0064 0053 0072 3200 0000 2903  .....d.S.r2...).
+000006f0: da05 7375 7065 72da 0573 6574 5570 721d  ..super..setUpr.
+00000700: 0000 0029 0172 1500 0000 a901 da09 5f5f  ...).r........__
+00000710: 636c 6173 735f 5f72 1b00 0000 721c 0000  class__r....r...
+00000720: 0072 3e00 0000 3b00 0000 7304 0000 0000  .r>...;...s.....
+00000730: 010a 017a 0d57 6974 6847 4953 2e73 6574  ...z.WithGIS.set
+00000740: 5570 6301 0000 0000 0000 0000 0000 0002  Upc.............
+00000750: 0000 0007 0000 0003 0000 0073 4200 0000  ...........sB...
+00000760: 7400 8300 a001 a100 0100 7402 6a03 6401  t.........t.j.d.
+00000770: 1900 6402 1900 7d01 7c01 a004 6403 a101  ..d...}.|...d...
+00000780: 732a 7405 6404 8301 8201 7406 a007 6405  s*t.d.....t...d.
+00000790: 6406 6407 6408 7c01 6705 a101 0100 6400  d.d.d.|.g.....d.
+000007a0: 5300 2909 4eda 0764 6566 6175 6c74 da04  S.).N..default..
+000007b0: 4e41 4d45 da05 7465 7374 5f7a 1d4e 6f74  NAME..test_z.Not
+000007c0: 2061 2074 6573 7420 6461 7461 6261 7365   a test database
+000007d0: 2c20 6162 6f72 7469 6e67 da04 7073 716c  , aborting..psql
+000007e0: 7a02 2d66 7a2c 2f75 7372 2f73 6861 7265  z.-fz,/usr/share
+000007f0: 2f70 6f73 7467 7265 7371 6c31 352f 6578  /postgresql15/ex
+00000800: 7465 6e73 696f 6e2f 6b6d 6561 6e73 2e73  tension/kmeans.s
+00000810: 716c 7a02 2d64 2908 723d 0000 00da 0a73  qlz.-d).r=.....s
+00000820: 6574 5570 436c 6173 7372 0200 0000 da09  etUpClassr......
+00000830: 4441 5441 4241 5345 53da 0a73 7461 7274  DATABASES..start
+00000840: 7377 6974 68da 0a56 616c 7565 4572 726f  swith..ValueErro
+00000850: 72da 0a73 7562 7072 6f63 6573 73da 0372  r..subprocess..r
+00000860: 756e 2902 da03 636c 73da 1274 6573 745f  un)...cls..test_
+00000870: 6461 7461 6261 7365 5f6e 616d 6572 3f00  database_namer?.
+00000880: 0000 721b 0000 0072 1c00 0000 7245 0000  ..r....r....rE..
+00000890: 003f 0000 0073 0a00 0000 0002 0a02 0e02  .?...s..........
+000008a0: 0a01 0802 7a12 5769 7468 4749 532e 7365  ....z.WithGIS.se
+000008b0: 7455 7043 6c61 7373 2907 7239 0000 0072  tUpClass).r9...r
+000008c0: 3a00 0000 723b 0000 0072 3e00 0000 da0b  :...r;...r>.....
+000008d0: 636c 6173 736d 6574 686f 6472 4500 0000  classmethodrE...
+000008e0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+000008f0: 1b00 0000 721b 0000 0072 3f00 0000 721c  ....r....r?...r.
+00000900: 0000 0072 3c00 0000 3900 0000 7306 0000  ...r<...9...s...
+00000910: 0008 020c 0402 0172 3c00 0000 6300 0000  .......r<...c...
+00000920: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00000930: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000940: 5a02 6401 6402 8400 5a03 6403 5300 2904  Z.d.d...Z.d.S.).
+00000950: da0b 5769 7468 4669 6c74 6572 7363 0100  ..WithFiltersc..
+00000960: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000970: 0000 4300 0000 730c 0000 0067 0074 0067  ..C...s....g.t.g
+00000980: 027d 017c 0153 0072 3200 0000 720b 0000  .}.|.S.r2...r...
+00000990: 0029 0272 1500 0000 7236 0000 0072 1b00  .).r....r6...r..
+000009a0: 0000 721b 0000 0072 1c00 0000 da10 6765  ..r....r......ge
+000009b0: 745f 7465 7374 5f66 696c 7465 7273 4e00  t_test_filtersN.
+000009c0: 0000 7308 0000 0000 0302 0102 fe04 057a  ..s............z
+000009d0: 1c57 6974 6846 696c 7465 7273 2e67 6574  .WithFilters.get
+000009e0: 5f74 6573 745f 6669 6c74 6572 734e 2904  _test_filtersN).
+000009f0: 7239 0000 0072 3a00 0000 723b 0000 0072  r9...r:...r;...r
+00000a00: 5000 0000 721b 0000 0072 1b00 0000 721b  P...r....r....r.
+00000a10: 0000 0072 1c00 0000 724f 0000 004c 0000  ...r....rO...L..
+00000a20: 0073 0200 0000 0802 724f 0000 0029 15da  .s......rO...)..
+00000a30: 0b64 6a61 6e67 6f2e 636f 6e66 7202 0000  .django.confr...
+00000a40: 00da 1764 6a61 6e67 6f2e 636f 6e74 7269  ...django.contri
+00000a50: 622e 6769 732e 6765 6f73 7203 0000 00da  b.gis.geosr.....
+00000a60: 1764 6a61 6e67 6f2e 636f 6e74 7269 622e  .django.contrib.
+00000a70: 6769 732e 6764 616c 7204 0000 0072 0500  gis.gdalr....r..
+00000a80: 0000 da0c 646a 616e 676f 2e75 7469 6c73  ....django.utils
+00000a90: 7206 0000 00da 0a61 6e79 636c 7573 7465  r......anycluste
+00000aa0: 7272 0800 0000 da0d 616e 796d 6170 2e6d  rr......anymap.m
+00000ab0: 6f64 656c 7372 0900 0000 720a 0000 0072  odelsr....r....r
+00000ac0: 4900 0000 7211 0000 00da 1761 6e79 636c  I...r......anycl
+00000ad0: 7573 7465 722e 7465 7374 732e 636f 6d6d  uster.tests.comm
+00000ae0: 6f6e 720c 0000 0072 0d00 0000 723c 0000  onr....r....r<..
+00000af0: 0072 4f00 0000 721b 0000 0072 1b00 0000  .rO...r....r....
+00000b00: 721b 0000 0072 1c00 0000 da08 3c6d 6f64  r....r......<mod
+00000b10: 756c 653e 0100 0000 7314 0000 000c 010c  ule>....s.......
+00000b20: 0110 010c 020c 0210 0210 020c 030e 2a10  ..............*.
+00000b30: 13                                       .
```

### Comparing `anycluster-2.1.1/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc` & `anycluster-2.2.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc` & `anycluster-2.2.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc` & `anycluster-2.2.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/tests/common.py` & `anycluster-2.2.0/anycluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/tests/mixins.py` & `anycluster-2.2.0/anycluster/tests/mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,66 +8,74 @@
 from anymap.models import Gardens, GARDEN_STYLES
 
 import subprocess, random
 
 from anycluster.tests.common import VALID_FILTERS
 
 
-class WithGIS:
-
-    def setUp(self):
-        super().setUp()
-        self.create_points()
-
+class WithGardens:
 
     def create_points(self, amount=100):
 
         for c in range(0,amount):
 
+            style_index = random.randint(0, 4)
+            style = GARDEN_STYLES[style_index][0]
+
+            name = 'test garden {0}'.format(c)
 
-            latitude = float('{0}.{1}'.format(random.randint(48,49), str(random.random()).split('.')[-1]))
-            longitude = float('{0}.{1}'.format(random.randint(9,13), str(random.random()).split('.')[-1]))
+            garden = self.create_point(name, style)
 
-            point = Point(longitude, latitude, srid=4326)
+            
+    def create_point(self, name, style):
 
-            ct = CoordTransform(SpatialReference(point.srid), SpatialReference(3857))
-            point.transform(ct)
+        latitude = float('{0}.{1}'.format(random.randint(48,49), str(random.random()).split('.')[-1]))
+        longitude = float('{0}.{1}'.format(random.randint(9,13), str(random.random()).split('.')[-1]))
 
-            style_index = random.randint(0, 4)
-            style = GARDEN_STYLES[style_index][0]
+        point = Point(longitude, latitude, srid=4326)
+
+        ct = CoordTransform(SpatialReference(point.srid), SpatialReference(3857))
+        point.transform(ct)
+
+        garden = Gardens(
+            name = name,
+            style = style,
+            rating = random.randint(1, 5),
+            last_renewal = timezone.now(),
+            coordinates = point
+        )
+
+        garden.save()
+
+        return garden
 
-            garden = Gardens(
-                name = 'test garden {0}'.format(c),
-                style = style,
-                rating = random.randint(1, 5),
-                last_renewal = timezone.now(),
-                coordinates = point
-            )
+    def get_cluster_cache(self, geometry_type, zoom, clustertype, filters):
+
+        cluster_cache = ClusterCache(geometry_type, zoom, clustertype, filters)
 
-            garden.save()
+        return cluster_cache
 
+class WithGIS(WithGardens):
+
+    def setUp(self):
+        super().setUp()
+        self.create_points()
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
 
         test_database_name = settings.DATABASES['default']['NAME']
 
         if not test_database_name.startswith('test_'):
             raise ValueError('Not a test database, aborting')
         #psql -f /usr/share/postgresql15/extension/kmeans.sql -d YOURGEODJANGODATABASE
         subprocess.run(['psql', '-f', '/usr/share/postgresql15/extension/kmeans.sql', '-d', test_database_name])
         
 
-    def get_cluster_cache(self, geometry_type, zoom, clustertype, filters):
-
-        cluster_cache = ClusterCache(geometry_type, zoom, clustertype, filters)
-
-        return cluster_cache
-
 
 class WithFilters:
 
     def get_test_filters(self):
 
         filters = [
             [],
```

### Comparing `anycluster-2.1.1/anycluster/tests/test_ClusterCache.py` & `anycluster-2.2.0/anycluster/tests/test_ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/tests/test_FilterComposer.py` & `anycluster-2.2.0/anycluster/tests/test_FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/anycluster/tests/test_MapClusterer.py` & `anycluster-2.2.0/anycluster/tests/test_MapClusterer.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 from django.contrib.gis.gdal import SpatialReference, CoordTransform
 from anycluster.MapClusterer import MapClusterer
 from anycluster import MapTools
 
 from anycluster.definitions import (CLUSTER_TYPES, GEOMETRY_TYPE_VIEWPORT, GEOMETRY_TYPE_AREA, GEOMETRY_TYPES,
                                     CLUSTER_TYPE_KMEANS, CLUSTER_TYPE_GRID)
 from anycluster.tests.common import GEOJSON_POLYGON, GEOJSON_RECTANGLE, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION
-from anycluster.tests.mixins import WithGIS, WithFilters
+from anycluster.tests.mixins import WithGIS, WithFilters, WithGardens
 
 from anymap.models import Gardens
 
 import json
 
 TEST_ZOOM_LEVEL = 7
+TEST_GRID_SIZE = 256
 
 class TestMapClusterer(WithFilters, WithGIS, TestCase):
 
 
     def test_init(self):
 
         for clustertype in CLUSTER_TYPES:
@@ -459,19 +460,280 @@
             for field_name in map_clusterer.get_gis_field_names():
 
                 if field_name == 'coordinates::bytea':
                     field_name = 'coordinates'
 
                 self.assertEqual(getattr(garden, field_name), getattr(garden_, field_name))
 
-
     def test_panned_request(self):
         pass
 
     def test_zoom_level_changed(self):
         pass
 
     def test_clustertype_changed(self):
         pass
 
     def test_clear_cache(self):
-        pass
+        pass
+
+
+
+class TestMapClustererContentCounts(WithFilters, WithGardens, TestCase):
+    def test_get_map_content_count(self):
+
+        zoom = 10
+
+        # test modulations
+        filters = [
+            {
+                'column': 'style',
+                'value': 'stone',
+                'operator': '=',
+            }
+        ]
+
+        modulations = {
+            'free' : {
+
+                'filters' : [
+                    {
+                        'column': 'free_entrance',
+                        'value': True,
+                        'operator': '=',
+                    }
+                ]
+            },
+            'paid' : {
+                'filters' : [
+                    {
+                        'column': 'free_entrance',
+                        'value': True,
+                        'operator': '!=',
+                    }
+                ]
+            }
+        }
+
+        
+        for clustertype in CLUSTER_TYPES:
+            for geometry_type in GEOMETRY_TYPES:
+
+                for geojson in [GEOJSON_POLYGON, GEOJSON_RECTANGLE, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION]:
+
+                    if clustertype == CLUSTER_TYPE_GRID and geometry_type != GEOMETRY_TYPE_VIEWPORT:
+                        continue
+
+                    if geometry_type == GEOMETRY_TYPE_VIEWPORT and geojson != GEOJSON_RECTANGLE:
+                        continue
+
+                    cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
+                    map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
+
+                    result = map_clusterer.get_map_content_counts(geojson, geometry_type, filters, zoom, modulations)
+
+                    expected_result = {
+                        'count': 0,
+                        'modulations':  {
+                            'free' : {
+                                'count': 0,
+                            },
+                            'paid' : {
+                                'count': 0,
+                            }
+                        },
+                    }
+                    self.assertEqual(result, expected_result)
+
+                    if geometry_type == GEOMETRY_TYPE_VIEWPORT:
+
+                        self.create_point('name 1', 'stone')
+                        self.create_point('name 2', 'flower')
+
+                        result = map_clusterer.get_map_content_counts(geojson, geometry_type, filters, zoom, modulations)
+
+                        expected_result = {
+                            'count': 1,
+                            'modulations': {
+                                'free': {
+                                    'count': 0
+                                    },
+                                'paid': {
+                                    'count': 1
+                                }
+                            }
+                        }
+
+                        # print(result)
+
+                        self.assertEqual(result, expected_result)
+                    
+                    gardens = Gardens.objects.all()
+                    for garden in gardens:
+                        garden.delete()
+
+
+                    gardens = Gardens.objects.all()
+
+                    self.assertEqual(gardens.count(), 0)
+
+
+    def test_query_map_content_count(self):
+
+        zoom = 10
+        geometry_type = GEOMETRY_TYPE_VIEWPORT
+        clustertype = CLUSTER_TYPE_KMEANS
+
+        
+        filters = []
+
+        cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
+        map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
+
+        geojson = GEOJSON_RECTANGLE
+
+        geometries_for_counting = map_clusterer.get_geometries_for_counting(geojson, geometry_type, zoom)
+
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters)
+        self.assertEqual(count, 0)
+
+        self.create_point('name 1', 'stone')
+        
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters)
+        self.assertEqual(count, 1)
+
+        self.create_point('name 2', 'flower')
+
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters)
+        self.assertEqual(count, 2)
+
+
+        filters = [
+            {
+                'column': 'style',
+                'value': 'stone',
+                'operator': '=',
+            }
+        ]
+
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters)
+        self.assertEqual(count, 1)
+
+        filters = [
+            {
+                'column': 'style',
+                'value': 'stone',
+                'operator': '=',
+            },
+            {
+                'column': 'style',
+                'value': 'flower',
+                'operator': '=',
+                'logicalOperator': 'OR',
+            }
+        ]
+
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters)
+        self.assertEqual(count, 2)
+
+        gardens = Gardens.objects.all()
+        for garden in gardens:
+            garden.delete()
+
+
+        gardens = Gardens.objects.all()
+
+        self.assertEqual(gardens.count(), 0)
+
+
+    def test_get_geometries_for_counting(self):
+        
+        zoom = 10
+        
+        for clustertype in CLUSTER_TYPES:
+            for geometry_type in GEOMETRY_TYPES:
+
+                for geojson in [GEOJSON_POLYGON, GEOJSON_RECTANGLE, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION]:
+
+                    if clustertype == CLUSTER_TYPE_GRID and geometry_type != GEOMETRY_TYPE_VIEWPORT:
+                        continue
+
+                    if geometry_type == GEOMETRY_TYPE_VIEWPORT and geojson != GEOJSON_RECTANGLE:
+                        continue
+
+                    filters = []
+
+                    cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
+                    map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
+
+                    geos_geometries = map_clusterer.get_geometries_for_counting(geojson, geometry_type, zoom)
+
+                    self.assertTrue(isinstance(geos_geometries, list))
+
+                    for geometry in geos_geometries:
+                        #print(geometry)
+                        self.assertTrue('POLYGON' in geometry.wkt)
+
+
+    def test_snap_viewport_to_grid(self):
+        
+        filters = []
+        zoom = 10
+
+        for clustertype in CLUSTER_TYPES:
+            for geometry_type in GEOMETRY_TYPES:
+        
+                cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
+
+                map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
+
+                # rectangle is 4326
+                geos_geometries = map_clusterer.convert_geojson_to_geos(GEOJSON_RECTANGLE)
+
+                grid_rectangle = map_clusterer.snap_viewport_to_grid(geos_geometries, zoom)
+
+                self.assertEqual(str(grid_rectangle), 'SRID=3857;POLYGON ((978393.96205 5948635.289016, 1565430.33928 5948635.289016, 1565430.33928 6574807.424728, 978393.96205 6574807.424728, 978393.96205 5948635.289016))')
+                self.assertEqual(grid_rectangle.srid, 3857)
+
+                grid_rectangle.transform(4326)
+
+                polygon_4326 = 'SRID=4326;POLYGON ((8.7890624999977 47.04018214327889, 14.06249999999632 47.04018214327889, 14.06249999999632 50.7364551355909, 8.7890624999977 50.7364551355909, 8.7890624999977 47.04018214327889))'
+
+                self.assertEqual(polygon_4326, str(grid_rectangle))
+
+
+    def test_get_grouped_map_contents(self):
+
+        zoom = 10
+        filters = []
+
+        self.create_point('name 1', 'stone')
+        self.create_point('name 2', 'flower')
+        
+        for clustertype in CLUSTER_TYPES:
+            for geometry_type in GEOMETRY_TYPES:
+
+                for geojson in [GEOJSON_POLYGON, GEOJSON_RECTANGLE, GEOJSON_MULTIPOLYGON, GEOJSON_FEATURECOLLECTION]:
+
+                    cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
+
+                    map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
+
+                    group_by = 'style'
+
+                    result = map_clusterer.get_grouped_map_contents(geojson, geometry_type, zoom, filters, group_by)
+
+                    if geometry_type == GEOMETRY_TYPE_VIEWPORT:
+
+                        expected_result = {
+                            'stone' : {
+                                'count': 1
+                            },
+                            'flower' : {
+                                'count': 1
+                            }
+                        }
+
+                        self.assertEqual(result, expected_result)
+
+                    gardens = Gardens.objects.all()
+                    self.assertEqual(gardens.count(), 2)
```

### Comparing `anycluster-2.1.1/anycluster.egg-info/PKG-INFO` & `anycluster-2.2.0/anycluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.1.1
+Version: 2.2.0
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.1.1/anycluster.egg-info/SOURCES.txt` & `anycluster-2.2.0/anycluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.1/setup.py` & `anycluster-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'psycopg2',
     'djangorestframework',
     'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='2.1.1',
+    version='2.2.0',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
```

