# Comparing `tmp/cashews-6.1.0.tar.gz` & `tmp/cashews-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cashews-6.1.0.tar", last modified: Mon May  8 17:09:35 2023, max compression
+gzip compressed data, was "cashews-6.2.0.tar", last modified: Sun Jun  4 19:45:10 2023, max compression
```

## Comparing `cashews-6.1.0.tar` & `cashews-6.2.0.tar`

### file list

```diff
@@ -1,73 +1,96 @@
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.236388 cashews-6.1.0/
--rw-r--r--   0 pandadoc   (501) staff       (20)     1081 2022-03-15 17:20:31.000000 cashews-6.1.0/LICENSE
--rw-r--r--   0 pandadoc   (501) staff       (20)    28062 2023-05-08 17:09:35.236574 cashews-6.1.0/PKG-INFO
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.217746 cashews-6.1.0/cashews/
--rw-r--r--   0 pandadoc   (501) staff       (20)     1281 2023-04-01 17:20:20.000000 cashews-6.1.0/cashews/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1464 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/_typing.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.220555 cashews-6.1.0/cashews/backends/
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-03-15 17:20:31.000000 cashews-6.1.0/cashews/backends/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     9148 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/backends/diskcache.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     6438 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/backends/interface.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     8648 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/backends/memory.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.221954 cashews-6.1.0/cashews/backends/redis/
--rw-r--r--   0 pandadoc   (501) staff       (20)      213 2023-04-01 17:21:03.000000 cashews-6.1.0/cashews/backends/redis/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)    10542 2023-03-31 23:54:32.000000 cashews-6.1.0/cashews/backends/redis/backend.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1881 2023-04-01 10:22:37.000000 cashews-6.1.0/cashews/backends/redis/client.py
--rw-r--r--   0 pandadoc   (501) staff       (20)    12475 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/backends/redis/client_side.py
--rw-r--r--   0 pandadoc   (501) staff       (20)    11670 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/backends/transaction.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      639 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/cache_condition.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      882 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/commands.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.222636 cashews-6.1.0/cashews/contrib/
--rw-r--r--   0 pandadoc   (501) staff       (20)       63 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/contrib/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1701 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/contrib/_starlette.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.224148 cashews-6.1.0/cashews/decorators/
--rw-r--r--   0 pandadoc   (501) staff       (20)      616 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     7303 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/bloom.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.226227 cashews-6.1.0/cashews/decorators/cache/
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-03-15 17:20:31.000000 cashews-6.1.0/cashews/decorators/cache/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2000 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/cache/defaults.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4006 2023-05-08 07:21:58.000000 cashews-6.1.0/cashews/decorators/cache/early.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2732 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/decorators/cache/fail.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     3247 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/cache/hit.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2408 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/cache/iterator.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2324 2023-04-02 09:24:36.000000 cashews-6.1.0/cashews/decorators/cache/simple.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     3531 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/cache/soft.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     3004 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/decorators/circuit_breaker.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     3505 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/locked.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2253 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/decorators/rate.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2234 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/decorators/rate_slide.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      961 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/exceptions.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     7214 2023-05-08 17:06:55.000000 cashews-6.1.0/cashews/formatter.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2372 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/helpers.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     5924 2023-05-04 21:58:39.000000 cashews-6.1.0/cashews/key.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1900 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/picklers.py
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/py.typed
--rw-r--r--   0 pandadoc   (501) staff       (20)     8004 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/serialize.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1124 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/ttl.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.233228 cashews-6.1.0/cashews/utils/
--rw-r--r--   0 pandadoc   (501) staff       (20)      175 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/utils/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1415 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/utils/_bitarray.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1713 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/utils/_bitarray_lib.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      848 2022-11-14 08:28:19.000000 cashews-6.1.0/cashews/utils/object_size.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      862 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/utils/split_hash.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2795 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/validation.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.236138 cashews-6.1.0/cashews/wrapper/
--rw-r--r--   0 pandadoc   (501) staff       (20)      558 2023-04-01 17:20:44.000000 cashews-6.1.0/cashews/wrapper/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      623 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/wrapper/auto_init.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2749 2023-04-05 06:41:56.000000 cashews-6.1.0/cashews/wrapper/backend_settings.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     6862 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/wrapper/commands.py
--rw-r--r--   0 pandadoc   (501) staff       (20)    11806 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/wrapper/decorators.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1558 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/wrapper/disable_control.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4437 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/wrapper/tags.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      820 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/wrapper/time_condition.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4163 2023-04-04 22:17:36.000000 cashews-6.1.0/cashews/wrapper/transaction.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     3026 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/wrapper/wrapper.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.219116 cashews-6.1.0/cashews.egg-info/
--rw-r--r--   0 pandadoc   (501) staff       (20)    28062 2023-05-08 17:09:34.000000 cashews-6.1.0/cashews.egg-info/PKG-INFO
--rw-r--r--   0 pandadoc   (501) staff       (20)     1721 2023-05-08 17:09:35.000000 cashews-6.1.0/cashews.egg-info/SOURCES.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-05-08 17:09:34.000000 cashews-6.1.0/cashews.egg-info/dependency_links.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-05-08 17:09:34.000000 cashews-6.1.0/cashews.egg-info/not-zip-safe
--rw-r--r--   0 pandadoc   (501) staff       (20)      200 2023-05-08 17:09:35.000000 cashews-6.1.0/cashews.egg-info/requires.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)        8 2023-05-08 17:09:35.000000 cashews-6.1.0/cashews.egg-info/top_level.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)     1452 2023-05-08 17:09:35.237156 cashews-6.1.0/setup.cfg
--rw-r--r--   0 pandadoc   (501) staff       (20)       52 2022-03-15 17:20:32.000000 cashews-6.1.0/setup.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.308101 cashews-6.2.0/
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1081 2022-03-15 17:20:31.000000 cashews-6.2.0/LICENSE
+-rw-r--r--   0 pandadoc   (501) staff       (20)    28586 2023-06-04 19:45:10.308304 cashews-6.2.0/PKG-INFO
+-rw-r--r--   0 pandadoc   (501) staff       (20)    27494 2023-06-04 19:30:11.000000 cashews-6.2.0/README.md
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.284917 cashews-6.2.0/cashews/
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1315 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1496 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/_typing.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.287528 cashews-6.2.0/cashews/backends/
+-rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-03-15 17:20:31.000000 cashews-6.2.0/cashews/backends/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     9261 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/backends/diskcache.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     6573 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/backends/interface.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     8723 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/backends/memory.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.288660 cashews-6.2.0/cashews/backends/redis/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      213 2023-04-01 17:21:03.000000 cashews-6.2.0/cashews/backends/redis/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)    10629 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/backends/redis/backend.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1881 2023-04-01 10:22:37.000000 cashews-6.2.0/cashews/backends/redis/client.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)    12475 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/backends/redis/client_side.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)    11808 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/backends/transaction.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1055 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/cache_condition.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      920 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/commands.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.289127 cashews-6.2.0/cashews/contrib/
+-rw-r--r--   0 pandadoc   (501) staff       (20)       63 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/contrib/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1754 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/contrib/_starlette.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.290764 cashews-6.2.0/cashews/decorators/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      616 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/decorators/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     7303 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/decorators/bloom.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.292829 cashews-6.2.0/cashews/decorators/cache/
+-rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-03-15 17:20:31.000000 cashews-6.2.0/cashews/decorators/cache/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      202 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/decorators/cache/_exception.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2000 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/decorators/cache/defaults.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4544 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/decorators/cache/early.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2732 2023-05-08 17:06:36.000000 cashews-6.2.0/cashews/decorators/cache/fail.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     3726 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/decorators/cache/hit.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2408 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/decorators/cache/iterator.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2842 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/decorators/cache/simple.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     3531 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/decorators/cache/soft.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     3004 2023-05-08 17:06:36.000000 cashews-6.2.0/cashews/decorators/circuit_breaker.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     3288 2023-06-02 21:51:11.000000 cashews-6.2.0/cashews/decorators/locked.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2253 2023-05-08 17:06:36.000000 cashews-6.2.0/cashews/decorators/rate.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2234 2023-05-08 17:06:36.000000 cashews-6.2.0/cashews/decorators/rate_slide.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      961 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/exceptions.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     7348 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/formatter.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2372 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/helpers.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5924 2023-05-04 21:58:39.000000 cashews-6.2.0/cashews/key.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1900 2023-06-03 19:34:24.000000 cashews-6.2.0/cashews/picklers.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)        0 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/py.typed
+-rw-r--r--   0 pandadoc   (501) staff       (20)     8004 2023-06-03 19:35:08.000000 cashews-6.2.0/cashews/serialize.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1124 2023-05-08 17:06:36.000000 cashews-6.2.0/cashews/ttl.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.294316 cashews-6.2.0/cashews/utils/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      175 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/utils/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1415 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/utils/_bitarray.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1713 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/utils/_bitarray_lib.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      848 2022-11-14 08:28:19.000000 cashews-6.2.0/cashews/utils/object_size.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      862 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/utils/split_hash.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2795 2023-05-08 17:06:36.000000 cashews-6.2.0/cashews/validation.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.297538 cashews-6.2.0/cashews/wrapper/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      558 2023-04-01 17:20:44.000000 cashews-6.2.0/cashews/wrapper/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      623 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/wrapper/auto_init.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2749 2023-04-05 06:41:56.000000 cashews-6.2.0/cashews/wrapper/backend_settings.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     7179 2023-06-04 19:30:11.000000 cashews-6.2.0/cashews/wrapper/commands.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)    11806 2023-05-08 17:06:36.000000 cashews-6.2.0/cashews/wrapper/decorators.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1558 2023-05-08 17:06:36.000000 cashews-6.2.0/cashews/wrapper/disable_control.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4437 2023-05-08 17:06:36.000000 cashews-6.2.0/cashews/wrapper/tags.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      820 2023-03-27 18:56:42.000000 cashews-6.2.0/cashews/wrapper/time_condition.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4163 2023-04-04 22:17:36.000000 cashews-6.2.0/cashews/wrapper/transaction.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     3026 2023-05-08 17:06:36.000000 cashews-6.2.0/cashews/wrapper/wrapper.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.286416 cashews-6.2.0/cashews.egg-info/
+-rw-r--r--   0 pandadoc   (501) staff       (20)    28586 2023-06-04 19:45:10.000000 cashews-6.2.0/cashews.egg-info/PKG-INFO
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2295 2023-06-04 19:45:10.000000 cashews-6.2.0/cashews.egg-info/SOURCES.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-06-04 19:45:10.000000 cashews-6.2.0/cashews.egg-info/dependency_links.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-06-04 19:45:10.000000 cashews-6.2.0/cashews.egg-info/not-zip-safe
+-rw-r--r--   0 pandadoc   (501) staff       (20)      200 2023-06-04 19:45:10.000000 cashews-6.2.0/cashews.egg-info/requires.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)        8 2023-06-04 19:45:10.000000 cashews-6.2.0/cashews.egg-info/top_level.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1452 2023-06-04 19:45:10.309123 cashews-6.2.0/setup.cfg
+-rw-r--r--   0 pandadoc   (501) staff       (20)       52 2022-03-15 17:20:32.000000 cashews-6.2.0/setup.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-04 19:45:10.307719 cashews-6.2.0/tests/
+-rw-r--r--   0 pandadoc   (501) staff       (20)     8429 2023-06-04 19:30:11.000000 cashews-6.2.0/tests/test_backend_commands.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1484 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_blooms.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     9373 2023-06-04 19:30:11.000000 cashews-6.2.0/tests/test_cache.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2235 2023-06-04 19:30:11.000000 cashews-6.2.0/tests/test_cache_exception.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1561 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_circuit_breaker.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5906 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_client_side_cache.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5561 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_disable_control.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5013 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_invalidate.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      663 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_iterators_cache.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     7199 2023-05-08 17:06:55.000000 cashews-6.2.0/tests/test_key.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1899 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_lock_decorator.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2360 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_middleware.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     8144 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_pickle_serializer.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2287 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_rate_limit.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2546 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_redis_down.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2830 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_settings_url.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     6407 2023-04-04 22:17:36.000000 cashews-6.2.0/tests/test_tags_feature.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     9958 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_transaction.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2963 2023-03-27 18:56:42.000000 cashews-6.2.0/tests/test_utils.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     8263 2023-04-04 22:17:36.000000 cashews-6.2.0/tests/test_wrapper.py
```

### Comparing `cashews-6.1.0/LICENSE` & `cashews-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/PKG-INFO` & `cashews-6.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cashews
-Version: 6.1.0
+Version: 6.2.0
 Summary: cache tools with async power
 Home-page: https://github.com/Krukov/cashews/
 Author: Dmitry Kryukov
 Author-email: glebov.ru@gmail.com
 License: MIT
 Keywords: cache aio async multicache aiocache
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -250,14 +249,15 @@
 
 await cache.is_locked("key", wait=60)  # -> bool
 async with cache.lock("key", expire=10):
     ...
 await cache.set_lock("key", value="value", expire=60)  # -> bool
 await cache.unlock("key", "value")  # -> bool
 
+await cache.get_keys_count()  # -> int - total number of keys in cache
 await cache.close()
 ```
 
 ### Disable Cache
 
 Cache can be disabled not only at setup, but also in runtime. Cashews allow you to disable/enable any call of cache or specific commands:
 
@@ -480,39 +480,57 @@
     await email_exists.set(email)
 
 await email_exists("example@example.com")
 ```
 
 ### Cache condition
 
-By default, any result of function call is stored, even it is a `None`.
-Caching decorators have parameter `condition`, that can be:
+By default, any successful result of function call is stored, even it is a `None`.
+Caching decorators have the parameter - `condition`, that can be:
 
-- a callable object that receive result of function call, args, kwargs and a cache key
+- a callable object that receive a result of function call or an exception, args, kwargs and a cache key
 - a string: "not_none" or "skip_none" to do not cache `None` values in
 
 ```python
 from cashews import cache, NOT_NONE
 
 cache.setup("mem://")
 
 @cache(ttl="1h", condition=NOT_NONE)
 async def get():
     ...
 
 
 def skit_test_result(result, args, kwargs, key=None) -> bool:
-    return result != "test"
+    return result and result != "test"
 
 @cache(ttl="1h", condition=skit_test_result)
 async def get():
     ...
 
 ```
 
+It is also possible to cache an exception that function can raise, to do so use special conditions (only for simple, hit and early)
+
+```python
+from cashews import cache, with_exceptions, only_exceptions
+
+cache.setup("mem://")
+
+@cache(ttl="1h", condition=with_exceptions(MyException, TimeoutError))
+async def get():
+    ...
+
+
+@cache(ttl="1h", condition=only_exceptions(MyException, TimeoutError))
+async def get():
+    ...
+
+```
+
 Also caching decorators have parameter `time_condition` - min latency in seconds (can be set like `ttl`)
 of getting a result of function call to be cached.
 
 ```python
 from cashews import cache
 
 cache.setup("mem://")
@@ -1004,9 +1022,7 @@
 
 ```shell
 pip install .[tests,redis,diskcache,speedup] fastapi aiohttp requests
 
 pytest // run all tests with all backends
 pytest -m "not redis" // all tests without tests for redis backend
 ```
-
-
```

### Comparing `cashews-6.1.0/cashews/__init__.py` & `cashews-6.2.0/cashews/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .cache_condition import NOT_NONE  # noqa
+from .cache_condition import NOT_NONE, only_exceptions, with_exceptions  # noqa
 from .commands import Command  # noqa
 from .contrib import *  # noqa
 from .decorators import context_cache_detect, fast_condition, thunder_protection  # noqa
 from .exceptions import CacheBackendInteractionError, CircuitBreakerOpen, LockedError, RateLimitError  # noqa
 from .formatter import default_formatter, get_template_and_func_for, get_template_for_key  # noqa
 from .helpers import add_prefix, all_keys_lower, memory_limit  # noqa
 from .key import get_cache_key_template, noself  # noqa
```

### Comparing `cashews-6.1.0/cashews/_typing.py` & `cashews-6.2.0/cashews/_typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,17 @@
     from typing_extensions import Protocol
 
 _TTLTypes = Union[int, float, str, timedelta, None]
 TTL = Union[_TTLTypes, Callable[[Any], _TTLTypes]]
 
 
 class CallableCacheCondition(Protocol):
-    def __call__(self, result: Any, args: Tuple, kwargs: Dict[str, Any], key: str = "") -> bool:  # pragma: no cover
+    def __call__(
+        self, result: Any, args: Tuple, kwargs: Dict[str, Any], key: str = ""
+    ) -> Union[bool, Exception]:  # pragma: no cover
         ...
 
 
 Key = str
 KeyTemplate = str
 KeyOrTemplate = Union[KeyTemplate, Key]
 Value = Any
```

### Comparing `cashews-6.1.0/cashews/backends/diskcache.py` & `cashews-6.2.0/cashews/backends/diskcache.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,10 +253,13 @@
             if not values:
                 break
             _values.append(values.pop())
 
         await self.set(key, values)
         return _values
 
+    async def get_keys_count(self) -> int:
+        return await self._run_in_executor(lambda: len(self._cache))
+
 
 class DiskCache(SerializerMixin, _DiskCache):
     pass
```

### Comparing `cashews-6.1.0/cashews/backends/interface.py` & `cashews-6.2.0/cashews/backends/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,21 @@
     async def get_size(self, key: Key) -> int:
         """
         Return size in bites that allocated by a value for given key
         """
         ...
 
     @abstractmethod
+    async def get_keys_count(self) -> int:
+        """
+        Return count keys in cache
+        """
+        ...
+
+    @abstractmethod
     async def ping(self, message: Optional[bytes] = None) -> bytes:
         ...
 
     @abstractmethod
     async def clear(self):
         ...
```

### Comparing `cashews-6.1.0/cashews/backends/memory.py` & `cashews-6.2.0/cashews/backends/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,17 @@
             if not values:
                 break
             _values.append(values.pop())
 
         self._set(key, values)
         return _values
 
+    async def get_keys_count(self) -> int:
+        return len(self.store)
+
     async def close(self):
         self.__remove_expired_stop.set()
         if self.__remove_expired_task:
             await self.__remove_expired_task
             self.__remove_expired_task = None
         self.__is_init = False
```

### Comparing `cashews-6.1.0/cashews/backends/redis/backend.py` & `cashews-6.2.0/cashews/backends/redis/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,10 +278,13 @@
 
     async def set_remove(self, key: Key, *values: str):
         await self._client.srem(key, *values)
 
     async def set_pop(self, key: Key, count: int = 100) -> Iterable[str]:
         return [value.decode() for value in await self._client.spop(key, count)]
 
+    async def get_keys_count(self) -> int:
+        return await self._client.dbsize()
+
     async def close(self):
         await self._client.close()
         self.__is_init = False
```

### Comparing `cashews-6.1.0/cashews/backends/redis/client.py` & `cashews-6.2.0/cashews/backends/redis/client.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/backends/redis/client_side.py` & `cashews-6.2.0/cashews/backends/redis/client_side.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/backends/transaction.py` & `cashews-6.2.0/cashews/backends/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,16 @@
         if await self._local_cache.exists(key):
             return True
         if self._key_is_delete(key):
             return False
         return await self._backend.exists(key)
 
     # non transaction - proxy methods
+    async def get_keys_count(self) -> int:
+        return await self._backend.get_keys_count() + await self._local_cache.get_keys_count()
 
     @property
     def is_init(self) -> bool:
         return self._backend.is_init
 
     async def init(self):
         return await self._backend.init()
```

### Comparing `cashews-6.1.0/cashews/commands.py` & `cashews-6.2.0/cashews/commands.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,12 +30,13 @@
 
     SET_ADD = "set_add"
     SET_REMOVE = "set_remove"
     SET_POP = "set_pop"
 
     PING = "ping"
     GET_SIZE = "get_size"
+    GET_KEYS_COUNT = "get_keys_count"
 
 
 ALL = set(Command)
 PATTERN_CMDS = {Command.GET_MATCH, Command.DELETE_MATCH, Command.SCAN}
 RETRIEVE_CMDS = {Command.GET, Command.INCR, Command.GET_MANY, Command.GET_MATCH}
```

### Comparing `cashews-6.1.0/cashews/contrib/_starlette.py` & `cashews-6.2.0/cashews/contrib/_starlette.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from starlette.responses import StreamingResponse
 
 from cashews.backends.interface import Backend
 from cashews.serialize import register_type
 
 
-async def encode_streaming_response(value: StreamingResponse, backend: Backend, key: str, ttl) -> bytes:
-    value.body_iterator = set_iterator(backend, key, value.body_iterator, ttl)
+async def encode_streaming_response(
+    value: StreamingResponse, backend: Backend, key: str, expire: int, **kwargs
+) -> bytes:
+    value.body_iterator = set_iterator(backend, key, value.body_iterator, expire)
     serialized_value = b""
     serialized_value += bytes(str(value.status_code), "utf-8") + b":"
     for header, header_value in value.raw_headers:
         serialized_value += header + b"=" + header_value + b";"
     return serialized_value
 
 
-async def decode_streaming_response(value: bytes, backend: Backend, key) -> StreamingResponse:
+async def decode_streaming_response(value: bytes, backend: Backend, key: str, **kwargs) -> StreamingResponse:
     status_code, headers = value.split(b":")
     status_code = int(status_code)
     raw_headers = []
     for header in headers.split(b";"):
         if not header:
             continue
         header_name, header_value = header.split(b"=")
@@ -25,18 +27,18 @@
 
     content = get_iterator(backend, key)
     resp = StreamingResponse(content=content, status_code=status_code)
     resp.raw_headers = raw_headers
     return resp
 
 
-async def set_iterator(backend: Backend, key: str, iterator, ttl):
+async def set_iterator(backend: Backend, key: str, iterator, expire: int):
     chunk_number = 0
     async for chunk in iterator:
-        await backend.set(f"{key}:chunk:{chunk_number}", chunk, expire=ttl)
+        await backend.set(f"{key}:chunk:{chunk_number}", chunk, expire=expire)
         yield chunk
         chunk_number += 1
 
 
 async def get_iterator(backend: Backend, key: str):
     chunk_number = 0
     while True:
```

### Comparing `cashews-6.1.0/cashews/decorators/__init__.py` & `cashews-6.2.0/cashews/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/decorators/bloom.py` & `cashews-6.2.0/cashews/decorators/bloom.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/decorators/cache/defaults.py` & `cashews-6.2.0/cashews/decorators/cache/defaults.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/decorators/cache/early.py` & `cashews-6.2.0/cashews/decorators/cache/early.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import TYPE_CHECKING, Optional
 
 from cashews._typing import TTL, AsyncCallable_T, CallableCacheCondition, Decorator, KeyOrTemplate, Tags
 from cashews.formatter import register_template
 from cashews.key import get_cache_key, get_cache_key_template
 from cashews.ttl import ttl_to_seconds
 
+from ._exception import RaiseException, return_or_raise
 from .defaults import _empty, context_cache_detect
 
 if TYPE_CHECKING:  # pragma: no cover
     from cashews.backends import Cache
 
 __all__ = ("early",)
 
@@ -73,36 +74,46 @@
                 ttl=_ttl,
                 early_ttl=_early_ttl,
                 name="early",
                 template=_key_template,
             )
             early_expire_at, result = cached
             if early_expire_at >= datetime.utcnow():
-                return result
+                return return_or_raise(result)
             lock_key = _cache_key + _LOCK_SUFFIX
             if not await backend.set(lock_key, "1", expire=_early_ttl, exist=False):
-                return result
+                return return_or_raise(result)
             logger.info(
                 "Recalculate cache for %s (exp_at %s)",
                 _cache_key,
                 early_expire_at,
             )
             asyncio.create_task(_get_result_for_early(*args_to_call, unlock=True))
-            return result
+            return return_or_raise(result)
 
         return _wrap
 
     return _decor
 
 
 async def _get_result_for_early(
     backend: "Cache", func, args, kwargs, key, ttl: int, early_ttl: int, condition, tags, unlock=False
 ):
     try:
-        result = await func(*args, **kwargs)
-        if condition(result, args, kwargs, key):
-            early_expire_at = datetime.utcnow() + timedelta(seconds=early_ttl)
+        _exc = None
+        try:
+            result = await func(*args, **kwargs)
+        except Exception as exc:
+            _exc = exc
+            result = exc
+        cond_result = condition(result, args, kwargs, key=key)
+        early_expire_at = datetime.utcnow() + timedelta(seconds=early_ttl)
+        if isinstance(cond_result, bool) and cond_result and not isinstance(result, Exception):
             await backend.set(key, [early_expire_at, result], expire=ttl, tags=tags)
-        return result
+        elif isinstance(cond_result, Exception):
+            await backend.set(key, [early_expire_at, RaiseException(result)], expire=ttl, tags=tags)
+        if _exc:
+            raise _exc
+        return return_or_raise(result)
     finally:
         if unlock:
             asyncio.create_task(backend.delete(key + _LOCK_SUFFIX))
```

### Comparing `cashews-6.1.0/cashews/decorators/cache/fail.py` & `cashews-6.2.0/cashews/decorators/cache/fail.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/decorators/cache/hit.py` & `cashews-6.2.0/cashews/decorators/cache/hit.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, Optional
 
 from cashews._typing import TTL, AsyncCallable_T, CallableCacheCondition, Decorator, Key, KeyOrTemplate, Tags
 from cashews.formatter import register_template
 from cashews.key import get_cache_key, get_cache_key_template
 from cashews.ttl import ttl_to_seconds
 
+from ._exception import RaiseException, return_or_raise
 from .defaults import _empty, context_cache_detect
 
 if TYPE_CHECKING:  # pragma: no cover
     from cashews import Cache
 
 __all__ = ("hit",)
 
@@ -49,38 +50,52 @@
         async def _wrap(*args, **kwargs):
             _ttl = ttl_to_seconds(ttl, *args, **kwargs, with_callable=True)
             _cache_key = get_cache_key(func, _key_template, args, kwargs)
             _tags = [get_cache_key(func, tag, args, kwargs) for tag in tags]
 
             call_args = (func, args, kwargs, backend, _cache_key, _ttl, condition, _tags)
 
-            result, hits = await asyncio.gather(
+            cached, hits = await asyncio.gather(
                 backend.get(_cache_key, default=_empty),
                 backend.incr(_cache_key + ":counter", expire=_ttl, tags=_tags),
             )
-            if result is not _empty and hits and hits <= cache_hits:
+            if cached is not _empty and hits and hits <= cache_hits:
                 context_cache_detect._set(
                     _cache_key,
                     ttl=_ttl,
                     cache_hits=cache_hits,
                     name="hit",
                     template=_key_template,
                 )
                 if update_after and hits == update_after:
                     asyncio.create_task(_get_and_save(*call_args))
-                return result
+                return return_or_raise(cached)
             return await _get_and_save(*call_args)
 
         return _wrap
 
     return _decor
 
 
 async def _get_and_save(func, args, kwargs, backend: "Cache", key: Key, ttl, store, tags):
-    result = await func(*args, **kwargs)
-    if store(result, args, kwargs, key=key):
+    _exc = None
+    try:
+        result = await func(*args, **kwargs)
+    except Exception as exc:
+        _exc = exc
+        result = exc
+
+    cond_result = store(result, args, kwargs, key=key)
+    to_cache = None
+    if isinstance(cond_result, bool) and cond_result and not isinstance(result, Exception):
+        to_cache = (result,)
+    elif isinstance(cond_result, Exception):
+        to_cache = (RaiseException(result),)
+
+    if to_cache is not None:
         await asyncio.gather(
             backend.delete(key + ":counter"),
-            backend.set(key, result, expire=ttl, tags=tags),
+            backend.set(key, to_cache[0], expire=ttl, tags=tags),
         )
-
+    if _exc:
+        raise _exc
     return result
```

### Comparing `cashews-6.1.0/cashews/decorators/cache/iterator.py` & `cashews-6.2.0/cashews/decorators/cache/iterator.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/decorators/cache/simple.py` & `cashews-6.2.0/cashews/decorators/cache/simple.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import TYPE_CHECKING, Optional
 
 from cashews._typing import TTL, AsyncCallable_T, CallableCacheCondition, Decorator, KeyOrTemplate, Tags
 from cashews.formatter import register_template
 from cashews.key import get_cache_key, get_cache_key_template
 from cashews.ttl import ttl_to_seconds
 
+from ._exception import RaiseException, return_or_raise
 from .defaults import _empty, context_cache_detect
 
 if TYPE_CHECKING:  # pragma: no cover
     from cashews import Cache
 
 __all__ = ("cache",)
 
@@ -46,16 +47,27 @@
             _ttl = ttl_to_seconds(ttl, *args, **kwargs, with_callable=True)
             _tags = [get_cache_key(func, tag, args, kwargs) for tag in tags]
             _cache_key = get_cache_key(func, _key_template, args, kwargs)
 
             cached = await backend.get(_cache_key, default=_empty)
             if cached is not _empty:
                 context_cache_detect._set(_cache_key, ttl=_ttl, name="simple", template=_key_template)
-                return cached
-            result = await func(*args, **kwargs)
-            if condition(result, args, kwargs, key=_cache_key):
+                return return_or_raise(cached)
+            _exc = None
+            try:
+                result = await func(*args, **kwargs)
+            except Exception as exc:
+                _exc = exc
+                result = exc
+
+            cond_result = condition(result, args, kwargs, key=_cache_key)
+            if isinstance(cond_result, bool) and cond_result and not isinstance(result, Exception):
                 await backend.set(_cache_key, result, expire=_ttl, tags=_tags)
+            elif isinstance(cond_result, Exception):
+                await backend.set(_cache_key, RaiseException(result), expire=_ttl, tags=_tags)
+            if _exc:
+                raise _exc
             return result
 
         return _wrap
 
     return _decor
```

### Comparing `cashews-6.1.0/cashews/decorators/cache/soft.py` & `cashews-6.2.0/cashews/decorators/cache/soft.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/decorators/circuit_breaker.py` & `cashews-6.2.0/cashews/decorators/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/decorators/locked.py` & `cashews-6.2.0/cashews/decorators/locked.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,33 +73,28 @@
                 yield chunk
             return
 
     return _wrap
 
 
 def thunder_protection(key: Optional[KeyOrTemplate] = None) -> Decorator:
-    futures: Dict[str, asyncio.Future] = {}
+    tasks: Dict[str, asyncio.Task] = {}
 
     def _decor(func: AsyncCallable_T) -> AsyncCallable_T:
         _key_template = get_cache_key_template(func, key=key)
 
-        def done_callback(_key: Key, task: asyncio.Task):
-            future = futures[_key]
-            if task.exception():
-                future.set_exception(task.exception())
-            else:
-                future.set_result(task.result())
-            del futures[_key]
+        def done_callback(_key: Key, _: asyncio.Task):
+            del tasks[_key]
 
         @wraps(func)
         async def _wrapper(*args, **kwargs):
             _key = get_cache_key(func, _key_template, args, kwargs)
-            if _key in futures:
-                return await futures[_key]
+            if _key in tasks:
+                return await tasks[_key]
             task = asyncio.create_task(func(*args, **kwargs))
-            futures[_key] = asyncio.Future()
+            tasks[_key] = task
             task.add_done_callback(partial(done_callback, _key))
             return await task
 
         return _wrapper
 
     return _decor
```

### Comparing `cashews-6.1.0/cashews/decorators/rate.py` & `cashews-6.2.0/cashews/decorators/rate.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/decorators/rate_slide.py` & `cashews-6.2.0/cashews/decorators/rate_slide.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/exceptions.py` & `cashews-6.2.0/cashews/exceptions.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/formatter.py` & `cashews-6.2.0/cashews/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 def _decode_bytes(value: bytes):
     try:
         return value.decode()
     except UnicodeDecodeError:
         return value.hex()
 
 
+def _decode_exception(value: Exception):
+    return f"{value.__class__.__name__}:{value}"
+
+
 def _get_decode_array(format_value):
     def _decode_array(values: Iterable[str]) -> TemplateValue:
         return ":".join([format_value(value) for value in values])
 
     return _decode_array
 
 
@@ -45,14 +49,15 @@
     def __init__(self, default=lambda field: "*"):
         self.__default = default
         _decode_array = _get_decode_array(self._format_field)
         self.__type_format = {
             str: _decode_direct,
             bool: _decoded_bool,
             bytes: _decode_bytes,
+            Exception: _decode_exception,
             tuple: _decode_array,
             list: _decode_array,
             set: _decode_array,
             dict: _get_decoded_dict(self._format_field),
         }
         super().__init__()
```

### Comparing `cashews-6.1.0/cashews/helpers.py` & `cashews-6.2.0/cashews/helpers.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/key.py` & `cashews-6.2.0/cashews/key.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/picklers.py` & `cashews-6.2.0/cashews/picklers.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/serialize.py` & `cashews-6.2.0/cashews/serialize.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/ttl.py` & `cashews-6.2.0/cashews/ttl.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/utils/_bitarray.py` & `cashews-6.2.0/cashews/utils/_bitarray.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/utils/_bitarray_lib.py` & `cashews-6.2.0/cashews/utils/_bitarray_lib.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/utils/object_size.py` & `cashews-6.2.0/cashews/utils/object_size.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/utils/split_hash.py` & `cashews-6.2.0/cashews/utils/split_hash.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/validation.py` & `cashews-6.2.0/cashews/validation.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/wrapper/__init__.py` & `cashews-6.2.0/cashews/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/wrapper/auto_init.py` & `cashews-6.2.0/cashews/wrapper/auto_init.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/wrapper/backend_settings.py` & `cashews-6.2.0/cashews/wrapper/backend_settings.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/wrapper/commands.py` & `cashews-6.2.0/cashews/wrapper/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,14 +130,23 @@
     async def get_size(self, key: Key) -> int:
         return await self._with_middlewares(Command.GET_SIZE, key)(key=key)
 
     async def ping(self, message: Optional[bytes] = None) -> bytes:
         message = b"PING" if message is None else message
         return await self._with_middlewares(Command.PING, message.decode())(message=message)
 
+    async def get_keys_count(self) -> int:
+        result = 0
+        for backend, _ in self._backends.values():
+            count = await self._with_middlewares_for_backend(
+                Command.GET_KEYS_COUNT, backend, self._default_middlewares
+            )()
+            result += count
+        return result
+
     async def clear(self):
         for backend, _ in self._backends.values():
             await self._with_middlewares_for_backend(Command.CLEAR, backend, self._default_middlewares)()
 
     async def is_locked(
         self,
         key: Key,
```

### Comparing `cashews-6.1.0/cashews/wrapper/decorators.py` & `cashews-6.2.0/cashews/wrapper/decorators.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/wrapper/disable_control.py` & `cashews-6.2.0/cashews/wrapper/disable_control.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/wrapper/tags.py` & `cashews-6.2.0/cashews/wrapper/tags.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/wrapper/time_condition.py` & `cashews-6.2.0/cashews/wrapper/time_condition.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/wrapper/transaction.py` & `cashews-6.2.0/cashews/wrapper/transaction.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews/wrapper/wrapper.py` & `cashews-6.2.0/cashews/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `cashews-6.1.0/cashews.egg-info/PKG-INFO` & `cashews-6.2.0/cashews.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cashews
-Version: 6.1.0
+Version: 6.2.0
 Summary: cache tools with async power
 Home-page: https://github.com/Krukov/cashews/
 Author: Dmitry Kryukov
 Author-email: glebov.ru@gmail.com
 License: MIT
 Keywords: cache aio async multicache aiocache
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -250,14 +249,15 @@
 
 await cache.is_locked("key", wait=60)  # -> bool
 async with cache.lock("key", expire=10):
     ...
 await cache.set_lock("key", value="value", expire=60)  # -> bool
 await cache.unlock("key", "value")  # -> bool
 
+await cache.get_keys_count()  # -> int - total number of keys in cache
 await cache.close()
 ```
 
 ### Disable Cache
 
 Cache can be disabled not only at setup, but also in runtime. Cashews allow you to disable/enable any call of cache or specific commands:
 
@@ -480,39 +480,57 @@
     await email_exists.set(email)
 
 await email_exists("example@example.com")
 ```
 
 ### Cache condition
 
-By default, any result of function call is stored, even it is a `None`.
-Caching decorators have parameter `condition`, that can be:
+By default, any successful result of function call is stored, even it is a `None`.
+Caching decorators have the parameter - `condition`, that can be:
 
-- a callable object that receive result of function call, args, kwargs and a cache key
+- a callable object that receive a result of function call or an exception, args, kwargs and a cache key
 - a string: "not_none" or "skip_none" to do not cache `None` values in
 
 ```python
 from cashews import cache, NOT_NONE
 
 cache.setup("mem://")
 
 @cache(ttl="1h", condition=NOT_NONE)
 async def get():
     ...
 
 
 def skit_test_result(result, args, kwargs, key=None) -> bool:
-    return result != "test"
+    return result and result != "test"
 
 @cache(ttl="1h", condition=skit_test_result)
 async def get():
     ...
 
 ```
 
+It is also possible to cache an exception that function can raise, to do so use special conditions (only for simple, hit and early)
+
+```python
+from cashews import cache, with_exceptions, only_exceptions
+
+cache.setup("mem://")
+
+@cache(ttl="1h", condition=with_exceptions(MyException, TimeoutError))
+async def get():
+    ...
+
+
+@cache(ttl="1h", condition=only_exceptions(MyException, TimeoutError))
+async def get():
+    ...
+
+```
+
 Also caching decorators have parameter `time_condition` - min latency in seconds (can be set like `ttl`)
 of getting a result of function call to be cached.
 
 ```python
 from cashews import cache
 
 cache.setup("mem://")
@@ -1004,9 +1022,7 @@
 
 ```shell
 pip install .[tests,redis,diskcache,speedup] fastapi aiohttp requests
 
 pytest // run all tests with all backends
 pytest -m "not redis" // all tests without tests for redis backend
 ```
-
-
```

### Comparing `cashews-6.1.0/cashews.egg-info/SOURCES.txt` & `cashews-6.2.0/cashews.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+README.md
 setup.cfg
 setup.py
 cashews/__init__.py
 cashews/_typing.py
 cashews/cache_condition.py
 cashews/commands.py
 cashews/exceptions.py
@@ -34,14 +35,15 @@
 cashews/decorators/__init__.py
 cashews/decorators/bloom.py
 cashews/decorators/circuit_breaker.py
 cashews/decorators/locked.py
 cashews/decorators/rate.py
 cashews/decorators/rate_slide.py
 cashews/decorators/cache/__init__.py
+cashews/decorators/cache/_exception.py
 cashews/decorators/cache/defaults.py
 cashews/decorators/cache/early.py
 cashews/decorators/cache/fail.py
 cashews/decorators/cache/hit.py
 cashews/decorators/cache/iterator.py
 cashews/decorators/cache/simple.py
 cashews/decorators/cache/soft.py
@@ -55,8 +57,28 @@
 cashews/wrapper/backend_settings.py
 cashews/wrapper/commands.py
 cashews/wrapper/decorators.py
 cashews/wrapper/disable_control.py
 cashews/wrapper/tags.py
 cashews/wrapper/time_condition.py
 cashews/wrapper/transaction.py
-cashews/wrapper/wrapper.py
+cashews/wrapper/wrapper.py
+tests/test_backend_commands.py
+tests/test_blooms.py
+tests/test_cache.py
+tests/test_cache_exception.py
+tests/test_circuit_breaker.py
+tests/test_client_side_cache.py
+tests/test_disable_control.py
+tests/test_invalidate.py
+tests/test_iterators_cache.py
+tests/test_key.py
+tests/test_lock_decorator.py
+tests/test_middleware.py
+tests/test_pickle_serializer.py
+tests/test_rate_limit.py
+tests/test_redis_down.py
+tests/test_settings_url.py
+tests/test_tags_feature.py
+tests/test_transaction.py
+tests/test_utils.py
+tests/test_wrapper.py
```

### Comparing `cashews-6.1.0/setup.cfg` & `cashews-6.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cashews
-version = 6.1.0
+version = 6.2.0
 url = https://github.com/Krukov/cashews/
 author = Dmitry Kryukov
 author_email = glebov.ru@gmail.com
 description = cache tools with async power
 keywords = cache aio async multicache aiocache
 long_description = file: README.md
 long_description_content_type = text/markdown
```

