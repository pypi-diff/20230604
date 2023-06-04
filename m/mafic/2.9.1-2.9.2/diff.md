# Comparing `tmp/mafic-2.9.1.tar.gz` & `tmp/mafic-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafic-2.9.1.tar", max compression
+gzip compressed data, was "mafic-2.9.2.tar", max compression
```

## Comparing `mafic-2.9.1.tar` & `mafic-2.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1070 2023-06-04 13:13:28.026235 mafic-2.9.1/LICENSE
--rw-r--r--   0        0        0     3315 2023-06-04 13:13:28.026235 mafic-2.9.1/README.md
--rw-r--r--   0        0        0      886 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/__init__.py
--rw-r--r--   0        0        0     3554 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/__libraries.py
--rw-r--r--   0        0        0     1559 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/__main__.py
--rw-r--r--   0        0        0     4490 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/errors.py
--rw-r--r--   0        0        0     5617 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/events.py
--rw-r--r--   0        0        0    27782 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/filter.py
--rw-r--r--   0        0        0     7397 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/ip.py
--rw-r--r--   0        0        0    43682 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/node.py
--rw-r--r--   0        0        0    27445 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/player.py
--rw-r--r--   0        0        0     1232 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/playlist.py
--rw-r--r--   0        0        0      674 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/plugin.py
--rw-r--r--   0        0        0    12004 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/pool.py
--rw-r--r--   0        0        0        0 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/py.typed
--rw-r--r--   0        0        0     3679 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/region.py
--rw-r--r--   0        0        0     1031 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/search_type.py
--rw-r--r--   0        0        0     3437 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/stats.py
--rw-r--r--   0        0        0     5254 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/strategy.py
--rw-r--r--   0        0        0     4797 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/track.py
--rw-r--r--   0        0        0      747 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/type_variables.py
--rw-r--r--   0        0        0      199 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/typings/__init__.py
--rw-r--r--   0        0        0     2996 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/typings/common.py
--rw-r--r--   0        0        0     4712 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/typings/http.py
--rw-r--r--   0        0        0     2385 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/typings/incoming.py
--rw-r--r--   0        0        0      602 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/typings/misc.py
--rw-r--r--   0        0        0     1189 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/typings/outgoing.py
--rw-r--r--   0        0        0      117 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/utils/__init__.py
--rw-r--r--   0        0        0     1203 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/utils/classproperty.py
--rw-r--r--   0        0        0      745 2023-06-04 13:13:28.030235 mafic-2.9.1/mafic/warnings.py
--rw-r--r--   0        0        0     3766 2023-06-04 13:13:28.030235 mafic-2.9.1/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-04 13:33:32.628357 mafic-2.9.2/LICENSE
+-rw-r--r--   0        0        0     3315 2023-06-04 13:33:32.628357 mafic-2.9.2/README.md
+-rw-r--r--   0        0        0      886 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/__init__.py
+-rw-r--r--   0        0        0     3554 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/__libraries.py
+-rw-r--r--   0        0        0     1559 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/__main__.py
+-rw-r--r--   0        0        0     4490 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/errors.py
+-rw-r--r--   0        0        0     5617 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/events.py
+-rw-r--r--   0        0        0    27782 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/filter.py
+-rw-r--r--   0        0        0     7397 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/ip.py
+-rw-r--r--   0        0        0    43682 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/node.py
+-rw-r--r--   0        0        0    27445 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/player.py
+-rw-r--r--   0        0        0     1232 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/playlist.py
+-rw-r--r--   0        0        0      674 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/plugin.py
+-rw-r--r--   0        0        0    11111 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/pool.py
+-rw-r--r--   0        0        0        0 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/py.typed
+-rw-r--r--   0        0        0     3679 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/region.py
+-rw-r--r--   0        0        0     1031 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/search_type.py
+-rw-r--r--   0        0        0     3437 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/stats.py
+-rw-r--r--   0        0        0     5575 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/strategy.py
+-rw-r--r--   0        0        0     4797 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/track.py
+-rw-r--r--   0        0        0      747 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/type_variables.py
+-rw-r--r--   0        0        0      199 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/typings/__init__.py
+-rw-r--r--   0        0        0     2996 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/typings/common.py
+-rw-r--r--   0        0        0     4712 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/typings/http.py
+-rw-r--r--   0        0        0     2385 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/typings/incoming.py
+-rw-r--r--   0        0        0      602 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/typings/misc.py
+-rw-r--r--   0        0        0     1189 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/typings/outgoing.py
+-rw-r--r--   0        0        0      117 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/utils/__init__.py
+-rw-r--r--   0        0        0     1203 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/utils/classproperty.py
+-rw-r--r--   0        0        0      745 2023-06-04 13:33:32.632357 mafic-2.9.2/mafic/warnings.py
+-rw-r--r--   0        0        0     3766 2023-06-04 13:33:32.632357 mafic-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.9.2/PKG-INFO
```

### Comparing `mafic-2.9.1/LICENSE` & `mafic-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/README.md` & `mafic-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/__init__.py` & `mafic-2.9.2/mafic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .track import *
 from .warnings import *
 
 __title__ = "mafic"
 __author__ = "ooliver1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present ooliver1"
-__version__ = "2.9.1"
+__version__ = "2.9.2"
 """The current version of mafic, using `PEP 440`_ format.
 
 .. _PEP 440: https://peps.python.org/pep-0440/
 """
 
 del __libraries
```

### Comparing `mafic-2.9.1/mafic/__libraries.py` & `mafic-2.9.2/mafic/__libraries.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/__main__.py` & `mafic-2.9.2/mafic/__main__.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/errors.py` & `mafic-2.9.2/mafic/errors.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/events.py` & `mafic-2.9.2/mafic/events.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/filter.py` & `mafic-2.9.2/mafic/filter.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/ip.py` & `mafic-2.9.2/mafic/ip.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/node.py` & `mafic-2.9.2/mafic/node.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/player.py` & `mafic-2.9.2/mafic/player.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/playlist.py` & `mafic-2.9.2/mafic/playlist.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/plugin.py` & `mafic-2.9.2/mafic/plugin.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/pool.py` & `mafic-2.9.2/mafic/pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,16 +61,14 @@
     """
 
     __slots__ = ()
 
     # Generics as expected, do not work in class variables.
     # Don't fear, the public methods using this are typed well.
     _nodes: ClassVar[dict[str, Node[Any]]] = {}
-    _node_regions: ClassVar[dict[VoiceRegion, set[Node[Any]]]] = {}
-    _node_shards: ClassVar[dict[int, set[Node[Any]]]] = {}
     _client: ClientT | None = None
 
     def __init__(
         self,
         client: ClientT,
         default_strategies: StrategyList[ClientT] | None = None,
     ) -> None:
@@ -214,29 +212,14 @@
         node:
             The node to add.
         player:
             The player class to use for this node when resuming.
 
             .. versionadded:: 2.8
         """
-        # Add to dictionaries, creating a set or extending it if needed.
-        if node.regions:
-            for region in node.regions:
-                self._node_regions[region] = {
-                    node,
-                    *self._node_regions.get(region, set()),
-                }
-
-        if node.shard_ids:
-            for shard_id in node.shard_ids:
-                self._node_shards[shard_id] = {
-                    node,
-                    *self._node_shards.get(shard_id, set()),
-                }
-
         _log.info("Created node, connecting it...", extra={"label": node.label})
         await node.connect(player_cls=player_cls)
 
         self._nodes[node.label] = node
 
     async def remove_node(
         self, node: Node[ClientT] | str, *, transfer_players: bool = True
@@ -251,22 +234,14 @@
             The node to remove.
         transfer_players:
             Whether to transfer players to other nodes or destroy them.
         """
         if isinstance(node, str):
             node = self._nodes[node]
 
-        if node.regions:
-            for region in node.regions:
-                self._node_regions[region].remove(node)
-
-        if node.shard_ids:
-            for shard_id in node.shard_ids:
-                self._node_shards[shard_id].remove(node)
-
         # Remove prematurely so it is not chosen.
         del self._nodes[node.label]
 
         if transfer_players:
 
             async def transfer_player(player: Player[ClientT]) -> None:
                 try:
```

### Comparing `mafic-2.9.1/mafic/region.py` & `mafic-2.9.2/mafic/region.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/search_type.py` & `mafic-2.9.2/mafic/search_type.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/stats.py` & `mafic-2.9.2/mafic/stats.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/strategy.py` & `mafic-2.9.2/mafic/strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from collections.abc import Callable
 from enum import Enum, auto
 from logging import getLogger
 from random import choice
 from typing import List, Optional
 
 from .node import Node
+from .region import VoiceRegion
 from .type_variables import ClientT
 
 StrategyCallable = Callable[
     [List[Node[ClientT]], int, Optional[int], Optional[str]], List[Node[ClientT]]
 ]
 """Represents a strategy callable.
 
@@ -103,14 +104,25 @@
             "Failed to match endpoint %s (match: %s) to a region, "
             "defaulting to all nodes.",
             endpoint,
             match.group("region"),
         )
         return nodes
 
+    try:
+        voice_region = VoiceRegion(voice_region)
+    except ValueError:
+        _log.error(
+            "Failed to match endpoint %s (match: %s) to a region, "
+            "defaulting to all nodes.",
+            endpoint,
+            voice_region,
+        )
+        return nodes
+
     regional_nodes = list(
         filter(
             lambda node: node.regions is not None and voice_region in node.regions,
             nodes,
         )
     )
```

### Comparing `mafic-2.9.1/mafic/track.py` & `mafic-2.9.2/mafic/track.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/type_variables.py` & `mafic-2.9.2/mafic/type_variables.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/typings/common.py` & `mafic-2.9.2/mafic/typings/common.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/typings/http.py` & `mafic-2.9.2/mafic/typings/http.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/typings/incoming.py` & `mafic-2.9.2/mafic/typings/incoming.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/typings/misc.py` & `mafic-2.9.2/mafic/typings/misc.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/typings/outgoing.py` & `mafic-2.9.2/mafic/typings/outgoing.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/utils/classproperty.py` & `mafic-2.9.2/mafic/utils/classproperty.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/mafic/warnings.py` & `mafic-2.9.2/mafic/warnings.py`

 * *Files identical despite different names*

### Comparing `mafic-2.9.1/pyproject.toml` & `mafic-2.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mafic"
-version = "2.9.1"
+version = "2.9.2"
 description = "A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ooliver1/mafic"
 homepage = "https://github.com/ooliver1/mafic"
 keywords = [
```

### Comparing `mafic-2.9.1/PKG-INFO` & `mafic-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafic
-Version: 2.9.1
+Version: 2.9.2
 Summary: A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 Home-page: https://github.com/ooliver1/mafic
 License: MIT
 Keywords: nextcord,disnake,discord,disnake.py,lavalink,lavalink.py,pycord,py-cord
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
```

