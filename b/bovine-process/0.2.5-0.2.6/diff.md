# Comparing `tmp/bovine_process-0.2.5.tar.gz` & `tmp/bovine_process-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_process-0.2.5.tar", max compression
+gzip compressed data, was "bovine_process-0.2.6.tar", max compression
```

## Comparing `bovine_process-0.2.5.tar` & `bovine_process-0.2.6.tar`

### file list

```diff
@@ -1,32 +1,52 @@
--rw-r--r--   0        0        0     1681 2023-05-28 14:23:45.592439 bovine_process-0.2.5/README.md
--rw-r--r--   0        0        0     1664 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/__init__.py
--rw-r--r--   0        0        0      770 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/add_to_queue.py
--rw-r--r--   0        0        0      809 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/incoming/__init__.py
--rw-r--r--   0        0        0      863 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/incoming/follow_accept.py
--rw-r--r--   0        0        0      709 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/incoming/handle_update.py
--rw-r--r--   0        0        0      847 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/incoming/incoming_delete.py
--rw-r--r--   0        0        0      877 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/incoming/store_incoming.py
--rw-r--r--   0        0        0     1414 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/incoming/test_handle_update.py
--rw-r--r--   0        0        0      983 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/incoming/test_store_incoming.py
--rw-r--r--   0        0        0     1604 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/incoming/test_undo.py
--rw-r--r--   0        0        0      721 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/incoming/undo.py
--rw-r--r--   0        0        0      693 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/outgoing/__init__.py
--rw-r--r--   0        0        0      642 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/outgoing/accept_follow.py
--rw-r--r--   0        0        0      878 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/outgoing/outgoing_delete.py
--rw-r--r--   0        0        0      943 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/outgoing/outgoing_update.py
--rw-r--r--   0        0        0      972 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/outgoing/store_outgoing.py
--rw-r--r--   0        0        0     1626 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/outgoing/test_outgoing_update.py
--rw-r--r--   0        0        0      386 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/outgoing/update_id.py
--rw-r--r--   0        0        0     1598 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/send_item.py
--rw-r--r--   0        0        0      364 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/test_types.py
--rw-r--r--   0        0        0      723 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/types.py
--rw-r--r--   0        0        0        0 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/utils/__init__.py
--rw-r--r--   0        0        0      741 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/utils/by_activity_type.py
--rw-r--r--   0        0        0      844 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/utils/processor_list.py
--rw-r--r--   0        0        0     1084 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/utils/test_by_activity_type.py
--rw-r--r--   0        0        0      429 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/utils/test_processor_list.py
--rw-r--r--   0        0        0      759 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/utils/test_update_id.py
--rw-r--r--   0        0        0      481 2023-05-28 14:23:45.592439 bovine_process-0.2.5/bovine_process/utils/update_id.py
--rw-r--r--   0        0        0      939 2023-05-28 14:23:50.788485 bovine_process-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 bovine_process-0.2.5/setup.py
--rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 bovine_process-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1619 2023-06-04 18:31:36.366115 bovine_process-0.2.6/README.md
+-rw-r--r--   0        0        0     1664 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/__init__.py
+-rw-r--r--   0        0        0      770 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/add_to_queue.py
+-rw-r--r--   0        0        0     1176 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/__init__.py
+-rw-r--r--   0        0        0     1152 2023-06-04 18:34:44.991995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      978 2023-06-04 18:34:44.995995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/follow_accept.cpython-310.pyc
+-rw-r--r--   0        0        0      813 2023-06-04 18:34:44.995995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/handle_update.cpython-310.pyc
+-rw-r--r--   0        0        0      948 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/incoming_delete.cpython-310.pyc
+-rw-r--r--   0        0        0     2131 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/interactions.cpython-310.pyc
+-rw-r--r--   0        0        0     1066 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/store_incoming.cpython-310.pyc
+-rw-r--r--   0        0        0     1637 2023-06-04 18:34:45.067995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/test_handle_update.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1880 2023-06-04 18:34:45.103996 bovine_process-0.2.6/bovine_process/incoming/__pycache__/test_store_incoming.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      863 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/follow_accept.py
+-rw-r--r--   0        0        0      709 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/handle_update.py
+-rw-r--r--   0        0        0      847 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/incoming_delete.py
+-rw-r--r--   0        0        0     2501 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/interactions.py
+-rw-r--r--   0        0        0      877 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/store_incoming.py
+-rw-r--r--   0        0        0     1414 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/test_handle_update.py
+-rw-r--r--   0        0        0      983 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/test_store_incoming.py
+-rw-r--r--   0        0        0      693 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/__init__.py
+-rw-r--r--   0        0        0      733 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      820 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/accept_follow.cpython-310.pyc
+-rw-r--r--   0        0        0      960 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/outgoing_delete.cpython-310.pyc
+-rw-r--r--   0        0        0      887 2023-06-04 18:34:45.003995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/outgoing_update.cpython-310.pyc
+-rw-r--r--   0        0        0     1132 2023-06-04 18:34:45.003995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/store_outgoing.cpython-310.pyc
+-rw-r--r--   0        0        0     1613 2023-06-04 18:34:45.107996 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/test_outgoing_update.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      604 2023-06-04 18:34:45.003995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/update_id.cpython-310.pyc
+-rw-r--r--   0        0        0      642 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/accept_follow.py
+-rw-r--r--   0        0        0      878 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/outgoing_delete.py
+-rw-r--r--   0        0        0      943 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/outgoing_update.py
+-rw-r--r--   0        0        0      972 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/store_outgoing.py
+-rw-r--r--   0        0        0     1626 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/test_outgoing_update.py
+-rw-r--r--   0        0        0      386 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/update_id.py
+-rw-r--r--   0        0        0     1598 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/send_item.py
+-rw-r--r--   0        0        0      364 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/test_types.py
+-rw-r--r--   0        0        0      723 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/types.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:31:36.498116 bovine_process-0.2.6/bovine_process/utils/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-04 18:34:44.995995 bovine_process-0.2.6/bovine_process/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1156 2023-06-04 18:34:44.995995 bovine_process-0.2.6/bovine_process/utils/__pycache__/by_activity_type.cpython-310.pyc
+-rw-r--r--   0        0        0     1324 2023-06-04 18:34:44.995995 bovine_process-0.2.6/bovine_process/utils/__pycache__/processor_list.cpython-310.pyc
+-rw-r--r--   0        0        0     2420 2023-06-04 18:34:45.111996 bovine_process-0.2.6/bovine_process/utils/__pycache__/test_by_activity_type.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1077 2023-06-04 18:34:45.115996 bovine_process-0.2.6/bovine_process/utils/__pycache__/test_processor_list.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1591 2023-06-04 18:34:45.119996 bovine_process-0.2.6/bovine_process/utils/__pycache__/test_update_id.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      515 2023-06-04 18:34:45.003995 bovine_process-0.2.6/bovine_process/utils/__pycache__/update_id.cpython-310.pyc
+-rw-r--r--   0        0        0      741 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/by_activity_type.py
+-rw-r--r--   0        0        0      844 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/processor_list.py
+-rw-r--r--   0        0        0     1084 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/test_by_activity_type.py
+-rw-r--r--   0        0        0      429 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/test_processor_list.py
+-rw-r--r--   0        0        0      759 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/test_update_id.py
+-rw-r--r--   0        0        0      481 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/update_id.py
+-rw-r--r--   0        0        0      939 2023-06-04 18:31:36.370115 bovine_process-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 bovine_process-0.2.6/PKG-INFO
```

### Comparing `bovine_process-0.2.5/README.md` & `bovine_process-0.2.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 - Send objects to follower's inbox
 - Enque object for bovine_pubsub
 
 The behavior defined in this package corresponds to [6. Client to Server Interactions](https://www.w3.org/TR/activitypub/#client-to-server-interactions) and [7. Server to Server Interactions](https://www.w3.org/TR/activitypub/#server-to-server-interactions) of the ActivityPub specification. However, only a small subset of side effects is implemented.
 
 ## Implemented Side Effects
 
-- Create, Update, Delete. Deletes are handled by replacing the object with a Tombstone. Various checks are performed to ensure only appropriate Updates happen.
-- [ ] Specify Update checks
+- Create, Update, Delete on objects, i.e. basic crud
+- Like, Dislike, EmojiReact -> add to likes collection; Undo removes
+- Announce -> add to share collection; Undo removes
+- The same person can Like, Announce, etc.. multiple times
+- Create with inReplyTo -> add to replies collection; Delete removes
+
 - Follow and Accept
   - Outgoing Accept of Follow adds to followers
   - Incoming Accept of Follows adds to following
-- [ ] Implement other side effects, in particular Like, Announce, and inReplyTo
-- [ ] Authority checks.
 
-That's it. Currently, no collections for replies and likes are kept in bovine_store, so implementing these side effects cannot happen yet:
-
-- [ ] Announce -> add to share collection
-- [ ] Like -> add to likes collection
-- [ ] Create with inReplyTo -> add to replies collection
+- [ ] Specify Update checks
+- [ ] Authority checks.
+- [ ] Refactor for easier customization / extension. Adding a new side effect currently requires publishing a new package. This should not be the case.
 
 ## Tests
 
 The folder `tests/data` contains test cases what side effects happen in the database for certain cases.
```

### Comparing `bovine_process-0.2.5/bovine_process/__init__.py` & `bovine_process-0.2.6/bovine_process/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/add_to_queue.py` & `bovine_process-0.2.6/bovine_process/add_to_queue.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/incoming/follow_accept.py` & `bovine_process-0.2.6/bovine_process/incoming/follow_accept.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/incoming/handle_update.py` & `bovine_process-0.2.6/bovine_process/incoming/handle_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/incoming/incoming_delete.py` & `bovine_process-0.2.6/bovine_process/incoming/incoming_delete.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/incoming/store_incoming.py` & `bovine_process-0.2.6/bovine_process/incoming/store_incoming.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/incoming/test_handle_update.py` & `bovine_process-0.2.6/bovine_process/incoming/test_handle_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/incoming/test_store_incoming.py` & `bovine_process-0.2.6/bovine_process/incoming/test_store_incoming.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/incoming/test_undo.py` & `bovine_process-0.2.6/bovine_process/outgoing/test_outgoing_update.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,50 @@
-from unittest.mock import MagicMock
-
-import pytest
-from bovine_store.utils.test import store  # noqa F401
+from bovine_store.utils.test import bovine_store_actor, store  # noqa F401
 
 from bovine_process.types import ProcessingItem
 
-from .store_incoming import store_incoming
-from .undo import undo
+from .outgoing_update import outgoing_update
+from .store_outgoing import store_outgoing
 
 
-async def test_undo_bad_format(store):  # noqa F801
+async def test_basic_update(store, bovine_store_actor):  # noqa F801
     first_id = "https://my_domain/first"
-    item = {
+    second_id = "https://my_domain/second"
+    third_id = "https://my_domain/third"
+    create = {
         "@context": "https://www.w3.org/ns/activitystreams",
         "id": first_id,
-        "type": "Undo",
+        "type": "Create",
+        "actor": bovine_store_actor.actor_id,
+        "object": {
+            "type": "Note",
+            "id": second_id,
+            "content": "new",
+            "attributedTo": bovine_store_actor.actor_id,
+        },
     }
 
-    processing_item = ProcessingItem("tag:actor", item)
-
-    result = await undo(processing_item, {})
-
-    assert result is None
-
-
-@pytest.mark.skip("FIXME: Not sure what to implement")
-async def test_undo(store):  # noqa F801a
-    actor = "https://remote_actor"
-    first_id = "https://my_domain/first"
-    second_id = "https://my_domain/second"
-
-    item = {
+    update = {
         "@context": "https://www.w3.org/ns/activitystreams",
-        "type": "Like",
-        "actor": actor,
-        "id": second_id,
+        "id": third_id,
+        "type": "Create",
+        "actor": bovine_store_actor.actor_id,
+        "object": {
+            "type": "Note",
+            "id": second_id,
+            "content": "updated",
+            "attributedTo": bovine_store_actor.actor_id,
+        },
     }
 
-    processing_item = ProcessingItem(actor, item)
-
-    result = await store_incoming(
-        processing_item, store, MagicMock(actor_id="local_user_id")
-    )
-
-    undo_item = {
-        "@context": "https://www.w3.org/ns/activitystreams",
-        "id": first_id,
-        "actor": actor,
-        "type": "Undo",
-        "object": item,
-    }
+    processing_item = ProcessingItem(bovine_store_actor.actor_id, create)
 
-    processing_item = ProcessingItem(actor, undo_item)
-    result = await undo(processing_item, store, {})
+    await store_outgoing(processing_item, bovine_store_actor)
 
-    assert result is None
+    stored = await store.retrieve(bovine_store_actor.actor_id, second_id)
+    assert stored["content"] == "new"
 
-    first = await store.retrieve("local_actor_url", first_id)
-    second = await store.retrieve("local_actor_url", second_id)
+    processing_item = ProcessingItem(bovine_store_actor.actor_id, update)
+    await outgoing_update(processing_item, bovine_store_actor)
 
-    assert first is None
-    assert second is None
+    stored = await store.retrieve(bovine_store_actor.actor_id, second_id)
+    assert stored["content"] == "updated"
```

### Comparing `bovine_process-0.2.5/bovine_process/outgoing/__init__.py` & `bovine_process-0.2.6/bovine_process/outgoing/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/outgoing/accept_follow.py` & `bovine_process-0.2.6/bovine_process/outgoing/accept_follow.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/outgoing/outgoing_delete.py` & `bovine_process-0.2.6/bovine_process/outgoing/outgoing_delete.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/outgoing/outgoing_update.py` & `bovine_process-0.2.6/bovine_process/outgoing/outgoing_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/outgoing/store_outgoing.py` & `bovine_process-0.2.6/bovine_process/outgoing/store_outgoing.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/send_item.py` & `bovine_process-0.2.6/bovine_process/send_item.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/types.py` & `bovine_process-0.2.6/bovine_process/types.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/utils/by_activity_type.py` & `bovine_process-0.2.6/bovine_process/utils/by_activity_type.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/utils/processor_list.py` & `bovine_process-0.2.6/bovine_process/utils/processor_list.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/utils/test_by_activity_type.py` & `bovine_process-0.2.6/bovine_process/utils/test_by_activity_type.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/bovine_process/utils/test_update_id.py` & `bovine_process-0.2.6/bovine_process/utils/test_update_id.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.5/pyproject.toml` & `bovine_process-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine-process"
-version = "0.2.5"
+version = "0.2.6"
 description = "Processing of Side Effects of ActivityPub Activities for an ActivityPub Server"
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bovine_process"}]
 license = "MIT"
 repository = "https://codeberg.org/bovine/bovine"
```

### Comparing `bovine_process-0.2.5/PKG-INFO` & `bovine_process-0.2.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine-process
-Version: 0.2.5
+Version: 0.2.6
 Summary: Processing of Side Effects of ActivityPub Activities for an ActivityPub Server
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -33,25 +33,25 @@
 - Send objects to follower's inbox
 - Enque object for bovine_pubsub
 
 The behavior defined in this package corresponds to [6. Client to Server Interactions](https://www.w3.org/TR/activitypub/#client-to-server-interactions) and [7. Server to Server Interactions](https://www.w3.org/TR/activitypub/#server-to-server-interactions) of the ActivityPub specification. However, only a small subset of side effects is implemented.
 
 ## Implemented Side Effects
 
-- Create, Update, Delete. Deletes are handled by replacing the object with a Tombstone. Various checks are performed to ensure only appropriate Updates happen.
-- [ ] Specify Update checks
+- Create, Update, Delete on objects, i.e. basic crud
+- Like, Dislike, EmojiReact -> add to likes collection; Undo removes
+- Announce -> add to share collection; Undo removes
+- The same person can Like, Announce, etc.. multiple times
+- Create with inReplyTo -> add to replies collection; Delete removes
+
 - Follow and Accept
   - Outgoing Accept of Follow adds to followers
   - Incoming Accept of Follows adds to following
-- [ ] Implement other side effects, in particular Like, Announce, and inReplyTo
-- [ ] Authority checks.
 
-That's it. Currently, no collections for replies and likes are kept in bovine_store, so implementing these side effects cannot happen yet:
-
-- [ ] Announce -> add to share collection
-- [ ] Like -> add to likes collection
-- [ ] Create with inReplyTo -> add to replies collection
+- [ ] Specify Update checks
+- [ ] Authority checks.
+- [ ] Refactor for easier customization / extension. Adding a new side effect currently requires publishing a new package. This should not be the case.
 
 ## Tests
 
 The folder `tests/data` contains test cases what side effects happen in the database for certain cases.
```

