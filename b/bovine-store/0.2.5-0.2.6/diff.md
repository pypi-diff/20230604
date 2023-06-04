# Comparing `tmp/bovine_store-0.2.5.tar.gz` & `tmp/bovine_store-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_store-0.2.5.tar", max compression
+gzip compressed data, was "bovine_store-0.2.6.tar", max compression
```

## Comparing `bovine_store-0.2.5.tar` & `bovine_store-0.2.6.tar`

### file list

```diff
@@ -1,44 +1,75 @@
--rw-r--r--   0        0        0     2754 2023-05-28 14:23:45.592439 bovine_store-0.2.5/README.md
--rw-r--r--   0        0        0     6489 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/__init__.py
--rw-r--r--   0        0        0     1115 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/actor/__init__.py
--rw-r--r--   0        0        0     7070 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/actor/bovine_store_actor.py
--rw-r--r--   0        0        0     1844 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/actor/register.py
--rw-r--r--   0        0        0      731 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/actor/test_bovine_application_actor.py
--rw-r--r--   0        0        0     5217 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/actor/test_bovine_store_actor.py
--rw-r--r--   0        0        0     1684 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/actor/test_register.py
--rw-r--r--   0        0        0     1955 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/blueprint.py
--rw-r--r--   0        0        0      892 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/config.py
--rw-r--r--   0        0        0        0 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/fedi/__init__.py
--rw-r--r--   0        0        0      999 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/fedi/authorize.py
--rw-r--r--   0        0        0     1597 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/fedi/retrieve_public_key.py
--rw-r--r--   0        0        0     2398 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/fedi/test_authorize.py
--rw-r--r--   0        0        0     3986 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/fedi/test_retrieve_public_key.py
--rw-r--r--   0        0        0     2285 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/models.py
--rw-r--r--   0        0        0     1356 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/__init__.py
--rw-r--r--   0        0        0     3432 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/collection.py
--rw-r--r--   0        0        0     1101 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/remote.py
--rw-r--r--   0        0        0     1343 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/retrieve_object.py
--rw-r--r--   0        0        0     2544 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/store.py
--rw-r--r--   0        0        0      533 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/test_application_actor_data.py
--rw-r--r--   0        0        0     4100 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/test_collection.py
--rw-r--r--   0        0        0     1657 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/test_retrieve_object.py
--rw-r--r--   0        0        0     3591 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/test_store.py
--rw-r--r--   0        0        0     1904 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/test_store_remote.py
--rw-r--r--   0        0        0      184 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/test_utils.py
--rw-r--r--   0        0        0      582 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/store/utils.py
--rw-r--r--   0        0        0     3541 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/templates/fallback.html
--rw-r--r--   0        0        0      314 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/test_bovine_admin_store.py
--rw-r--r--   0        0        0      475 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/test_store.py
--rw-r--r--   0        0        0      455 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/types.py
--rw-r--r--   0        0        0      787 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/utils/__init__.py
--rw-r--r--   0        0        0      834 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/utils/collection.py
--rw-r--r--   0        0        0     1288 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/utils/ordered_collection.py
--rw-r--r--   0        0        0      680 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/utils/permissions.py
--rw-r--r--   0        0        0     2231 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/utils/test.py
--rw-r--r--   0        0        0      619 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/utils/test_path.py
--rw-r--r--   0        0        0      726 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/utils/test_permissions.py
--rw-r--r--   0        0        0      294 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/utils/test_summary.py
--rw-r--r--   0        0        0      375 2023-05-28 14:23:45.592439 bovine_store-0.2.5/bovine_store/utils/test_test.py
--rw-r--r--   0        0        0      917 2023-05-28 14:23:50.788485 bovine_store-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 bovine_store-0.2.5/setup.py
--rw-r--r--   0        0        0     3450 1970-01-01 00:00:00.000000 bovine_store-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     2857 2023-06-04 18:31:36.370115 bovine_store-0.2.6/README.md
+-rw-r--r--   0        0        0     6755 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/__init__.py
+-rw-r--r--   0        0        0     1115 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/__init__.py
+-rw-r--r--   0        0        0     1587 2023-06-04 18:33:42.427369 bovine_store-0.2.6/bovine_store/actor/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     8275 2023-06-04 18:33:43.307378 bovine_store-0.2.6/bovine_store/actor/__pycache__/bovine_store_actor.cpython-310.pyc
+-rw-r--r--   0        0        0     1831 2023-06-04 18:33:43.311378 bovine_store-0.2.6/bovine_store/actor/__pycache__/register.cpython-310.pyc
+-rw-r--r--   0        0        0     1525 2023-06-04 18:33:44.071386 bovine_store-0.2.6/bovine_store/actor/__pycache__/test_bovine_application_actor.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     5966 2023-06-04 18:33:44.075386 bovine_store-0.2.6/bovine_store/actor/__pycache__/test_bovine_store_actor.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     4341 2023-06-04 18:33:44.087386 bovine_store-0.2.6/bovine_store/actor/__pycache__/test_register.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     8175 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/bovine_store_actor.py
+-rw-r--r--   0        0        0     1844 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/register.py
+-rw-r--r--   0        0        0      731 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/test_bovine_application_actor.py
+-rw-r--r--   0        0        0     5217 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/test_bovine_store_actor.py
+-rw-r--r--   0        0        0     1684 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/test_register.py
+-rw-r--r--   0        0        0     2694 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/blueprint.py
+-rw-r--r--   0        0        0      892 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/config.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:31:36.514116 bovine_store-0.2.6/bovine_store/fedi/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-04 18:33:44.063386 bovine_store-0.2.6/bovine_store/fedi/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1149 2023-06-04 18:33:44.063386 bovine_store-0.2.6/bovine_store/fedi/__pycache__/authorize.cpython-310.pyc
+-rw-r--r--   0        0        0     1533 2023-06-04 18:33:44.095386 bovine_store-0.2.6/bovine_store/fedi/__pycache__/retrieve_public_key.cpython-310.pyc
+-rw-r--r--   0        0        0     2854 2023-06-04 18:33:44.091386 bovine_store-0.2.6/bovine_store/fedi/__pycache__/test_authorize.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3976 2023-06-04 18:33:44.095386 bovine_store-0.2.6/bovine_store/fedi/__pycache__/test_retrieve_public_key.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1021 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/fedi/authorize.py
+-rw-r--r--   0        0        0     1597 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/fedi/retrieve_public_key.py
+-rw-r--r--   0        0        0     2469 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/fedi/test_authorize.py
+-rw-r--r--   0        0        0     3986 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/fedi/test_retrieve_public_key.py
+-rw-r--r--   0        0        0     2285 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/models.py
+-rw-r--r--   0        0        0     1356 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/__init__.py
+-rw-r--r--   0        0        0     1126 2023-06-04 18:33:42.703372 bovine_store-0.2.6/bovine_store/store/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2995 2023-06-04 18:33:43.311378 bovine_store-0.2.6/bovine_store/store/__pycache__/collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1394 2023-06-04 18:33:43.311378 bovine_store-0.2.6/bovine_store/store/__pycache__/remote.cpython-310.pyc
+-rw-r--r--   0        0        0     1636 2023-06-04 18:33:43.307378 bovine_store-0.2.6/bovine_store/store/__pycache__/retrieve_object.cpython-310.pyc
+-rw-r--r--   0        0        0     2619 2023-06-04 18:33:42.931374 bovine_store-0.2.6/bovine_store/store/__pycache__/store.cpython-310.pyc
+-rw-r--r--   0        0        0     1471 2023-06-04 18:33:44.103386 bovine_store-0.2.6/bovine_store/store/__pycache__/test_application_actor_data.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     7060 2023-06-04 18:33:44.115386 bovine_store-0.2.6/bovine_store/store/__pycache__/test_collection.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2714 2023-06-04 18:33:44.119386 bovine_store-0.2.6/bovine_store/store/__pycache__/test_retrieve_object.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     4796 2023-06-04 18:33:44.127386 bovine_store-0.2.6/bovine_store/store/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2943 2023-06-04 18:33:44.135386 bovine_store-0.2.6/bovine_store/store/__pycache__/test_store_remote.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1111 2023-06-04 18:33:44.139387 bovine_store-0.2.6/bovine_store/store/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      809 2023-06-04 18:33:43.303378 bovine_store-0.2.6/bovine_store/store/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     4394 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/collection.py
+-rw-r--r--   0        0        0     1101 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/remote.py
+-rw-r--r--   0        0        0     1343 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/retrieve_object.py
+-rw-r--r--   0        0        0     2544 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/store.py
+-rw-r--r--   0        0        0      533 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/test_application_actor_data.py
+-rw-r--r--   0        0        0     4100 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/test_collection.py
+-rw-r--r--   0        0        0     1657 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/test_retrieve_object.py
+-rw-r--r--   0        0        0     3591 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/test_store.py
+-rw-r--r--   0        0        0     1904 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/test_store_remote.py
+-rw-r--r--   0        0        0      184 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/test_utils.py
+-rw-r--r--   0        0        0      582 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/utils.py
+-rw-r--r--   0        0        0     3541 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/templates/fallback.html
+-rw-r--r--   0        0        0      314 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/test_bovine_admin_store.py
+-rw-r--r--   0        0        0      475 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/test_store.py
+-rw-r--r--   0        0        0      479 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/types.py
+-rw-r--r--   0        0        0      951 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/__init__.py
+-rw-r--r--   0        0        0     1359 2023-06-04 18:33:43.307378 bovine_store-0.2.6/bovine_store/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1611 2023-06-04 18:33:43.311378 bovine_store-0.2.6/bovine_store/utils/__pycache__/collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1397 2023-06-04 18:33:44.039385 bovine_store-0.2.6/bovine_store/utils/__pycache__/ordered_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1009 2023-06-04 18:33:43.307378 bovine_store-0.2.6/bovine_store/utils/__pycache__/permissions.cpython-310.pyc
+-rw-r--r--   0        0        0     2660 2023-06-04 18:33:44.043386 bovine_store-0.2.6/bovine_store/utils/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0        0        0     1682 2023-06-04 18:33:44.143386 bovine_store-0.2.6/bovine_store/utils/__pycache__/test_path.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1381 2023-06-04 18:33:44.143386 bovine_store-0.2.6/bovine_store/utils/__pycache__/test_permissions.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1481 2023-06-04 18:33:44.147387 bovine_store-0.2.6/bovine_store/utils/__pycache__/test_summary.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1245 2023-06-04 18:33:44.151387 bovine_store-0.2.6/bovine_store/utils/__pycache__/test_test.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1124 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/collection.py
+-rw-r--r--   0        0        0     1288 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/ordered_collection.py
+-rw-r--r--   0        0        0      680 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/permissions.py
+-rw-r--r--   0        0        0     2231 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/test.py
+-rw-r--r--   0        0        0      619 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/test_path.py
+-rw-r--r--   0        0        0      726 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/test_permissions.py
+-rw-r--r--   0        0        0      294 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/test_summary.py
+-rw-r--r--   0        0        0      375 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/test_test.py
+-rw-r--r--   0        0        0      917 2023-06-04 18:31:36.374115 bovine_store-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3553 1970-01-01 00:00:00.000000 bovine_store-0.2.6/PKG-INFO
```

### Comparing `bovine_store-0.2.5/README.md` & `bovine_store-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ## Usage
 
 bovine_store assumes that a database connection is initialized using [tortoise-orm](https://tortoise.github.io/). See `examples/basic_app.py` for how to do this in the context of a quart app.
 
 ## TODO
 
 - [ ] When properties of actor are updated, send an update Activity
+  - Doesn't fit into the current bovine framework ... bovine_store doesn't know how to send activities
 - [ ] Generally rework the actor properties mechanism. It is currently not possible to emulate say Mastodon featured collection with it.
 - [ ] bovine_store.models.BovineActorKeyPair needs renamings; and work, e.g. a future identity column should have a uniqueness constraint.
 - [ ] Generally the code quality is not as high as it should be.
 
 ## Design discussion
 
 Some goals and design decisions:
```

### Comparing `bovine_store-0.2.5/bovine_store/__init__.py` & `bovine_store-0.2.6/bovine_store/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import bovine_store
 
 from .types import EndpointType
 from .actor.bovine_store_actor import BovineStoreActor
 from .actor.register import register
 from .models import BovineActor, BovineActorEndpoint, BovineActorKeyPair
 
-from .utils import user_to_handle_name_actor_url
+from .utils import user_to_account_and_actor_url
 from bovine_store.utils.collection import collection_response
 
 from .store import load_application_actor_data
 from .store.retrieve_object import retrieve_remote_object
 from .store.utils import domain_from_host
 
 
@@ -67,24 +67,24 @@
 
     async def user_count(self) -> int:
         """Returns the total number of bovine actors used in nodeinfo,
         this count probably lies with bovine being a multi hostname server
         and supporting bot accounts."""
         return await BovineActor.filter().count()
 
-    async def get_name_url_for_did(self, did):
-        """FIXME: Should probably return acct: identity + actor_url for
-        its use in webfinger"""
-        key = await BovineActorKeyPair.get_or_none(public_key=did).prefetch_related(
-            "bovine_actor"
-        )
+    async def get_account_url_for_identity(self, identity: str):
+        """Returns the account, i.e. the identity starting with acct:,
+        and the actoru_url for a given identity"""
+        key = await BovineActorKeyPair.get_or_none(
+            public_key=identity
+        ).prefetch_related("bovine_actor")
         if not key:
             return None, None
-        await key.bovine_actor.fetch_related("endpoints")
-        return user_to_handle_name_actor_url(key.bovine_actor)
+        await key.bovine_actor.fetch_related("endpoints", "keypairs")
+        return user_to_account_and_actor_url(key.bovine_actor)
 
     async def application_actor_for_url(self, url: str):
         """Returns the application actor fot the given url"""
         account_url = urljoin(url, "/activitypub/bovine")
         application_data = await load_application_actor_data(self.application_data)
 
         app_actor = bovine_store.actor.BovineApplicationActor(
@@ -100,15 +100,21 @@
 
 class BovineAdminStore:
     """Store for managing actors. This store should be used to create
     actor management interfaces.
 
     These can be kept separate from the actual fediverse server implementation.
 
-    For usage see `bovine_tool` and `bovine_management`."""
+    For usage see `bovine_tool` and `bovine_management`.
+
+    The parameters endpoint_path, endpoint_path_function can probably be removed
+    at one point. The parameter domain can actually be of the form
+    "http://domain_name" or "https://domain_name". This is useful for end
+    to end tests.
+    """
 
     def __init__(
         self,
         endpoint_path: str | None = None,
         endpoint_path_function: Callable = None,
         domain: str = None,
     ):
@@ -126,32 +132,31 @@
                 The bovine name given by handle_name + uuid4"""
 
         if self.endpoint_path is None and self.endpoint_path_function is None:
             if self.domain is None:
                 raise Exception("Need to specify an endpoint")
             if "://" not in self.domain:
                 domain = "https://" + self.domain
+            else:
+                domain = self.domain
 
             self.endpoint_path = urljoin(domain, "endpoints/template")
 
         result = await register(
             handle_name,
             endpoint_path=self.endpoint_path,
             endpoint_path_function=self.endpoint_path_function,
         )
         return result.bovine_name
 
-    async def add_did_key_to_actor(
+    async def add_identity_string_to_actor(
         self, bovine_name: str, name: str, identity: str
     ) -> None:
         """Modifies an Actor by adding a new identity to it. name is used
-        to identity the identity and serves little functional purpose.
-
-        FIXME: Should probably be renamed to add_identity_string_to_actor,
-        or similar."""
+        to identity the identity and serves little functional purpose."""
         actor = await BovineActor.get_or_none(bovine_name=bovine_name)
         await BovineActorKeyPair.create(
             bovine_actor=actor, name=name, public_key=identity, private_key=""
         )
 
     async def set_properties_for_actor(
         self, bovine_name: str, properties: dict
```

### Comparing `bovine_store-0.2.5/bovine_store/actor/__init__.py` & `bovine_store-0.2.6/bovine_store/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/actor/bovine_store_actor.py` & `bovine_store-0.2.6/bovine_store/actor/bovine_store_actor.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,23 @@
         self.actor_object: Actor = actor_object
 
         self.domain = domain_from_host(actor_object.id)
         self.endpoints = endpoints
 
         super().__init__(config)
 
+    async def retrieve_own_object(self, object_id: str) -> dict | None:
+        """Retrieves an object owner by the actor"""
+        result = await StoredJsonObject.get_or_none(id=object_id)
+        if not result:
+            return None
+        if result.owner != self.actor_object.id:
+            return None
+        return result.content
+
     async def retrieve(self, object_id: str, include=[], skip_fetch: bool = False):
         data = await self._retrieve_object_from_database(
             object_id, skip_fetch=skip_fetch
         )
 
         if data is None:
             return data
@@ -130,14 +139,37 @@
         )
 
     async def add_to_following(self, object_id):
         return await CollectionItem.create(
             part_of=self.actor_object.following, object_id=object_id
         )
 
+    async def add_to_interaction(
+        self, interaction: str, object_id: str, remote_id: str
+    ):
+        return await CollectionItem.create(
+            part_of=f"{object_id}/{interaction}", object_id=remote_id
+        )
+
+    async def remove_from_interaction(
+        self, interaction: str, object_id: str, remote_id: str
+    ):
+        obj = await CollectionItem.get_or_none(
+            part_of=f"{object_id}/{interaction}", object_id=remote_id
+        )
+        if obj:
+            await obj.delete()
+
+    async def remove_references(self, remote_id: str):
+        references = await CollectionItem.filter(
+            part_of__endswith="replies", object_id=remote_id
+        ).all()
+        for reply in references:
+            await reply.delete()
+
     async def resolve_endpoints(self, endpoints):
         tasks = [collection_all(self.actor_id, endpoint) for endpoint in endpoints]
         result = await asyncio.gather(*tasks)
         result = set(sum(result, []))
 
         logger.info("Resolved %s to %s", ", ".join(endpoints), ", ".join(result))
         return result
```

### Comparing `bovine_store-0.2.5/bovine_store/actor/register.py` & `bovine_store-0.2.6/bovine_store/actor/register.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/actor/test_bovine_application_actor.py` & `bovine_store-0.2.6/bovine_store/actor/test_bovine_application_actor.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/actor/test_bovine_store_actor.py` & `bovine_store-0.2.6/bovine_store/actor/test_bovine_store_actor.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/actor/test_register.py` & `bovine_store-0.2.6/bovine_store/actor/test_register.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/blueprint.py` & `bovine_store-0.2.6/bovine_store/blueprint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 from quart import Blueprint, g, request, current_app, render_template, redirect
 
 from .utils import determine_summary, path_from_request
+from .utils.collection import add_sub_collections
 from .fedi.authorize import add_authorization
 
 logger = logging.getLogger(__name__)
 
 bovine_store_blueprint = Blueprint(
     "bovine_store", __name__, template_folder="templates"
 )
@@ -26,18 +27,18 @@
     ):
         if "text" not in request.headers.get("accept", ""):
             return {"status": "unauthorized"}, 401
 
         return await fallback_handler(object_path)
 
     store = current_app.config["bovine_store"]
-
     obj = await store.retrieve_for_get(g.retriever, object_path)
 
     if obj:
+        obj = add_sub_collections(obj)
         return obj, 200, {"content-type": "application/activity+json"}
 
     return (
         {
             "@context": "https://www.w3.org/ns/activitystreams",
             "type": "Tombstone",
             "id": object_path,
@@ -65,7 +66,27 @@
             "fallback.html",
             object_path=object_path,
             object_type=object_type,
             object_summary=object_summary,
         ),
         415,
     )
+
+
+@bovine_store_blueprint.get("/<uuid>/<collection>")
+async def retrieve_collection_from_store(uuid, collection):
+    endpoint_path = path_from_request(request)
+    object_path = endpoint_path.removesuffix(f"/{collection}")
+    if (
+        g.retriever is None
+        or g.retriever == "NONE"
+        or "json" not in request.headers.get("accept", "").lower()
+    ):
+        return {"status": "unauthorized"}, 401
+
+    store = current_app.config["bovine_store"]
+    obj = await store.retrieve_for_get(g.retriever, object_path)
+
+    if not obj:
+        return {"status": "unauthorized"}, 401
+
+    return await store.collection_response(endpoint_path)
```

### Comparing `bovine_store-0.2.5/bovine_store/config.py` & `bovine_store-0.2.6/bovine_store/config.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/fedi/retrieve_public_key.py` & `bovine_store-0.2.6/bovine_store/fedi/retrieve_public_key.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/fedi/test_authorize.py` & `bovine_store-0.2.6/bovine_store/fedi/test_authorize.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     test_app.config["validate_http_signature"].assert_awaited_once()
 
 
 @patch("bovine.utils.date.check_max_offset_now")
 async def test_add_authorization_moo_auth_1(mock, test_app):  # noqa F401
     test_app.config["validate_http_signature"] = AsyncMock()
     test_app.config["bovine_store"] = AsyncMock(BovineStore)
-    test_app.config["bovine_store"].get_name_url_for_did.return_value = "name", "mock"
+    test_app.config["bovine_store"].get_account_url_for_identity.return_value = (
+        "acct:name",
+        "mock",
+    )
 
     headers = {
         "Date": "Wed, 15 Mar 2023 17:28:15 GMT",
         "Host": "myhost.tld",
         "Authorization": "Moo-Auth-1 did:key:z6MkekwC6R9bj9ErToB7AiZJfyCSDhaZe1UxhDbCqJrhqpS5",
         "X-Moo-Signature": "z5ahdHCbP9aJEsDtvG1MEZpxPzuvGKYcdXdKvMq5YL21Z2umxjs1SopCY2Ap8vZxVjTEf6dYbGuB7mtgcgUyNdBLe",
     }
@@ -39,15 +42,18 @@
     test_app.config["validate_http_signature"].assert_not_awaited()
 
 
 @patch("bovine.utils.date.check_max_offset_now")
 async def test_add_authorization_moo_auth_1_post(mock, test_app):  # noqa F401
     test_app.config["validate_http_signature"] = AsyncMock()
     test_app.config["bovine_store"] = AsyncMock(BovineStore)
-    test_app.config["bovine_store"].get_name_url_for_did.return_value = "name", "mock"
+    test_app.config["bovine_store"].get_account_url_for_identity.return_value = (
+        "name",
+        "mock",
+    )
 
     headers = {
         "Date": "Wed, 15 Mar 2023 17:28:15 GMT",
         "Host": "myhost.tld",
         "Digest": "sha-256=MILb5lUDD6Z0pDSxhgxj+hMBEw0uTzP3g2qUJGHMp9k=",
         "Authorization": "Moo-Auth-1 did:key:z6MkekwC6R9bj9ErToB7AiZJfyCSDhaZe1UxhDbCqJrhqpS5",
         "X-Moo-Signature": "z4vPkJaoaSVQp5DrMb8EvCajJcerW36rsyWDELTWQ3cYmaonnGfb8WHiwH54BShidCcmpoyHjanVRYNrXXXka4jAn",
```

### Comparing `bovine_store-0.2.5/bovine_store/fedi/test_retrieve_public_key.py` & `bovine_store-0.2.6/bovine_store/fedi/test_retrieve_public_key.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/models.py` & `bovine_store-0.2.6/bovine_store/models.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/store/__init__.py` & `bovine_store-0.2.6/bovine_store/store/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/store/collection.py` & `bovine_store-0.2.6/bovine_store/store/collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -57,51 +57,82 @@
     #     return result[0]["count"]
     # return result[0]["COUNT (DISTINCT ci.object_id)"]
 
 
 async def collection_items(retriever, collection_id, **kwargs) -> dict | None:
     limit = int(kwargs.get("limit", 10))
 
-    sql_query = f"""SELECT DISTINCT ci.id, ci.object_id
-        {sql_joined_tables}
-        {sql_where}
-    """
-
-    query_args = [collection_id, retriever, retriever, retriever]
+    query = CollectionItem.filter(part_of=collection_id)
 
     if kwargs.get("last"):
-        sql_query = f"{sql_query} ORDER BY ci.id ASC"
+        query = query.order_by("id")
     elif kwargs.get("first"):
-        sql_query = f"{sql_query} ORDER BY ci.id DESC"
+        query = query.order_by("-id")
     elif kwargs.get("min_id"):
         min_id = int(kwargs.get("min_id"))
-        sql_query = f"{sql_query} AND ci.id < $5"
-        query_args.append(min_id)
-        sql_query = f"{sql_query} ORDER BY ci.id DESC"
+        query = query.filter(id__lt=min_id).order_by("-id")
     elif kwargs.get("max_id"):
         max_id = int(kwargs.get("max_id"))
-        sql_query = f"{sql_query} AND ci.id > $5"
-        query_args.append(max_id)
-        sql_query = f"{sql_query} ORDER BY ci.id ASC"
+        query = query.filter(id__gt=max_id).order_by("id")
+
+    result = await query.limit(limit).all()
 
-    sql_query = f"{sql_query} LIMIT {limit}"
-    client = connections.get("default")
+    print(result)
 
-    result = await client.execute_query_dict(sql_query, query_args)
     next_prev = {}
     if len(result) > 0:
-        min_id = max(x["id"] for x in result)
-        max_id = min(x["id"] for x in result)
+        min_id = max(x.id for x in result)
+        max_id = min(x.id for x in result)
         next_prev = {
             "prev": f"max_id={min_id}",
             "next": f"min_id={max_id}",
         }
-    result = sorted(result, key=lambda x: -x["id"])
+    result = sorted(result, key=lambda x: -x.id)
+
+    return {"items": [x.object_id for x in result], **next_prev}
+
+    return result
+
+    # sql_query = f"""SELECT DISTINCT ci.id, ci.object_id
+    #     {sql_joined_tables}
+    #     {sql_where}
+    # """
+
+    # query_args = [collection_id, retriever, retriever, retriever]
+
+    # if kwargs.get("last"):
+    #     sql_query = f"{sql_query} ORDER BY ci.id ASC"
+    # elif kwargs.get("first"):
+    #     sql_query = f"{sql_query} ORDER BY ci.id DESC"
+    # elif kwargs.get("min_id"):
+    #     min_id = int(kwargs.get("min_id"))
+    #     sql_query = f"{sql_query} AND ci.id < $5"
+    #     query_args.append(min_id)
+    #     sql_query = f"{sql_query} ORDER BY ci.id DESC"
+    # elif kwargs.get("max_id"):
+    #     max_id = int(kwargs.get("max_id"))
+    #     sql_query = f"{sql_query} AND ci.id > $5"
+    #     query_args.append(max_id)
+    #     sql_query = f"{sql_query} ORDER BY ci.id ASC"
+
+    # sql_query = f"{sql_query} LIMIT {limit}"
+    # client = connections.get("default")
+
+    # result = await client.execute_query_dict(sql_query, query_args)
+    # next_prev = {}
+    # if len(result) > 0:
+    #     min_id = max(x["id"] for x in result)
+    #     max_id = min(x["id"] for x in result)
+    #     next_prev = {
+    #         "prev": f"max_id={min_id}",
+    #         "next": f"min_id={max_id}",
+    #     }
+    # result = sorted(result, key=lambda x: -x["id"])
 
-    return {"items": [x["object_id"] for x in result], **next_prev}
+    # return {"items": [x["object_id"] for x in result], **next_prev}
 
 
 async def collection_all(retriever, collection_id) -> list:
     items = await CollectionItem.filter(part_of=collection_id).all()
     return [item.object_id for item in items]
 
     sql_query = f"""SELECT ci.id, ci.object_id
```

### Comparing `bovine_store-0.2.5/bovine_store/store/remote.py` & `bovine_store-0.2.6/bovine_store/store/remote.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/store/retrieve_object.py` & `bovine_store-0.2.6/bovine_store/store/retrieve_object.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/store/store.py` & `bovine_store-0.2.6/bovine_store/store/store.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/store/test_application_actor_data.py` & `bovine_store-0.2.6/bovine_store/store/test_application_actor_data.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/store/test_collection.py` & `bovine_store-0.2.6/bovine_store/store/test_collection.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/store/test_retrieve_object.py` & `bovine_store-0.2.6/bovine_store/store/test_retrieve_object.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/store/test_store.py` & `bovine_store-0.2.6/bovine_store/store/test_store.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/store/test_store_remote.py` & `bovine_store-0.2.6/bovine_store/store/test_store_remote.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/store/utils.py` & `bovine_store-0.2.6/bovine_store/store/utils.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/templates/fallback.html` & `bovine_store-0.2.6/bovine_store/templates/fallback.html`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/utils/__init__.py` & `bovine_store-0.2.6/bovine_store/utils/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,21 +12,28 @@
 
 def get_actor_endpoint(endpoints):
     for endpoint in endpoints:
         if endpoint.endpoint_type == EndpointType.ACTOR:
             return endpoint
 
 
-def user_to_handle_name_actor_url(user):
+def get_account(keypairs):
+    for kp in keypairs:
+        if kp.public_key.startswith("acct:"):
+            return kp
+
+
+def user_to_account_and_actor_url(user):
     if not user:
         return None, None
 
     endpoint = get_actor_endpoint(user.endpoints)
+    keypair = get_account(user.keypairs)
 
-    return (user.handle_name, endpoint.name)
+    return (keypair.public_key, endpoint.name)
 
 
 def path_from_request(request) -> str:
     url = request.url
     if request.headers.get("X-Forwarded-Proto") == "https":
         url = url.replace("http://", "https://")
```

### Comparing `bovine_store-0.2.5/bovine_store/utils/ordered_collection.py` & `bovine_store-0.2.6/bovine_store/utils/ordered_collection.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/utils/permissions.py` & `bovine_store-0.2.6/bovine_store/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/utils/test.py` & `bovine_store-0.2.6/bovine_store/utils/test.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/utils/test_path.py` & `bovine_store-0.2.6/bovine_store/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/bovine_store/utils/test_permissions.py` & `bovine_store-0.2.6/bovine_store/utils/test_permissions.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.5/pyproject.toml` & `bovine_store-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine-store"
-version = "0.2.5"
+version = "0.2.6"
 description = "Store for ActivityPub activities, actors and objects"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine_store"}]
 repository = "https://codeberg.org/bovine/bovine"
```

### Comparing `bovine_store-0.2.5/setup.py` & `bovine_store-0.2.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,69 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bovine-store
+Version: 0.2.6
+Summary: Store for ActivityPub activities, actors and objects
+Home-page: https://codeberg.org/bovine/bovine
+License: MIT
+Author: Helge
+Author-email: helge.krueger@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bovine (>=0.2.1,<0.3.0)
+Requires-Dist: quart (>=0.18.3,<0.19.0)
+Requires-Dist: tortoise-orm[asyncpg] (>=0.19.3,<0.20.0)
+Project-URL: Repository, https://codeberg.org/bovine/bovine
+Description-Content-Type: text/markdown
+
+# bovine_store
+
+`bovine_store` is meant to be the module handling storing of
+local ActivityPub objects and caching of remote ActivityPub
+objects.
+
+## Usage
+
+bovine_store assumes that a database connection is initialized using [tortoise-orm](https://tortoise.github.io/). See `examples/basic_app.py` for how to do this in the context of a quart app.
+
+## TODO
+
+- [ ] When properties of actor are updated, send an update Activity
+  - Doesn't fit into the current bovine framework ... bovine_store doesn't know how to send activities
+- [ ] Generally rework the actor properties mechanism. It is currently not possible to emulate say Mastodon featured collection with it.
+- [ ] bovine_store.models.BovineActorKeyPair needs renamings; and work, e.g. a future identity column should have a uniqueness constraint.
+- [ ] Generally the code quality is not as high as it should be.
+
+## Design discussion
+
+Some goals and design decisions:
+
+- Objects with an id are stored separately and can be looked up via this id. This is done by json-ld magic.
+- Collections are not stored. Instead for local items, the information that the item belongs to a collection is stored. `bovine_store.store.collection` contains the coroutines necessary to build the collection from this information. All collections are assumed to ActivityStreams 2 `OrderedCollection` and ordered by the database id.
+- Every object is currently assigned an `owner`. The idea was that an activity is owner by its actor. This can then be propagated to the subobjects, e.g. the object, attachments, and so on. Unfortunately, this is too naive:
+  - Some implementations include remote objects, e.g. the object being liked in a Like Activity.
+  - Mastodon includes its custom emojis. These have an id and should probably belong to the server.
+- There are three kinds of visibility.
+  - An object is always visible to its owner
+  - Public Objects are assigned `VisibilityType.PUBLIC`. These can viewed by all users providing valid authentication.
+  - Furthemore, by adding actors to the `VisibileTo` list of an object. This can be made visible to the corresponding actors.
+- An item is visible to be inside a collection if and only if said item is visible. This should probably be augmented by visible to the owner of the collection.
+- `bovine_store.blueprint` contains a quart blueprint with the basic retrievel mechanism for the stored objects.
+- `bovine_store.collection` contains the helper routine for collection responses.
+
+## Examples
+
+A demonstration webserver can be seen using
+
+```bash
+poetry run python examples/basic_app.py
+```
+
+Note this is a very basic example. Instructions what the example does are
+printed to the command line after start.
+
+Note: This example creates two files `db.sqlite3`, which contains the
+database and `context_cache.sqlite`, which contains the cache of json-ld
+contexts.
 
-packages = \
-['bovine_store',
- 'bovine_store.actor',
- 'bovine_store.fedi',
- 'bovine_store.store',
- 'bovine_store.utils']
-
-package_data = \
-{'': ['*'], 'bovine_store': ['templates/*']}
-
-install_requires = \
-['bovine>=0.2.1,<0.3.0',
- 'quart>=0.18.3,<0.19.0',
- 'tortoise-orm[asyncpg]>=0.19.3,<0.20.0']
-
-setup_kwargs = {
-    'name': 'bovine-store',
-    'version': '0.2.5',
-    'description': 'Store for ActivityPub activities, actors and objects',
-    'long_description': '# bovine_store\n\n`bovine_store` is meant to be the module handling storing of\nlocal ActivityPub objects and caching of remote ActivityPub\nobjects.\n\n## Usage\n\nbovine_store assumes that a database connection is initialized using [tortoise-orm](https://tortoise.github.io/). See `examples/basic_app.py` for how to do this in the context of a quart app.\n\n## TODO\n\n- [ ] When properties of actor are updated, send an update Activity\n- [ ] Generally rework the actor properties mechanism. It is currently not possible to emulate say Mastodon featured collection with it.\n- [ ] bovine_store.models.BovineActorKeyPair needs renamings; and work, e.g. a future identity column should have a uniqueness constraint.\n- [ ] Generally the code quality is not as high as it should be.\n\n## Design discussion\n\nSome goals and design decisions:\n\n- Objects with an id are stored separately and can be looked up via this id. This is done by json-ld magic.\n- Collections are not stored. Instead for local items, the information that the item belongs to a collection is stored. `bovine_store.store.collection` contains the coroutines necessary to build the collection from this information. All collections are assumed to ActivityStreams 2 `OrderedCollection` and ordered by the database id.\n- Every object is currently assigned an `owner`. The idea was that an activity is owner by its actor. This can then be propagated to the subobjects, e.g. the object, attachments, and so on. Unfortunately, this is too naive:\n  - Some implementations include remote objects, e.g. the object being liked in a Like Activity.\n  - Mastodon includes its custom emojis. These have an id and should probably belong to the server.\n- There are three kinds of visibility.\n  - An object is always visible to its owner\n  - Public Objects are assigned `VisibilityType.PUBLIC`. These can viewed by all users providing valid authentication.\n  - Furthemore, by adding actors to the `VisibileTo` list of an object. This can be made visible to the corresponding actors.\n- An item is visible to be inside a collection if and only if said item is visible. This should probably be augmented by visible to the owner of the collection.\n- `bovine_store.blueprint` contains a quart blueprint with the basic retrievel mechanism for the stored objects.\n- `bovine_store.collection` contains the helper routine for collection responses.\n\n## Examples\n\nA demonstration webserver can be seen using\n\n```bash\npoetry run python examples/basic_app.py\n```\n\nNote this is a very basic example. Instructions what the example does are\nprinted to the command line after start.\n\nNote: This example creates two files `db.sqlite3`, which contains the\ndatabase and `context_cache.sqlite`, which contains the cache of json-ld\ncontexts.\n',
-    'author': 'Helge',
-    'author_email': 'helge.krueger@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://codeberg.org/bovine/bovine',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

