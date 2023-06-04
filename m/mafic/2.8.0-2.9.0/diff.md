# Comparing `tmp/mafic-2.8.0.tar.gz` & `tmp/mafic-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafic-2.8.0.tar", max compression
+gzip compressed data, was "mafic-2.9.0.tar", max compression
```

## Comparing `mafic-2.8.0.tar` & `mafic-2.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1070 2023-06-02 13:31:53.013765 mafic-2.8.0/LICENSE
--rw-r--r--   0        0        0     3315 2023-06-02 13:31:53.013765 mafic-2.8.0/README.md
--rw-r--r--   0        0        0      886 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/__init__.py
--rw-r--r--   0        0        0     3554 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/__libraries.py
--rw-r--r--   0        0        0     1559 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/__main__.py
--rw-r--r--   0        0        0     4490 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/errors.py
--rw-r--r--   0        0        0     5617 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/events.py
--rw-r--r--   0        0        0    27782 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/filter.py
--rw-r--r--   0        0        0     7397 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/ip.py
--rw-r--r--   0        0        0    43682 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/node.py
--rw-r--r--   0        0        0    27349 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/player.py
--rw-r--r--   0        0        0     1232 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/playlist.py
--rw-r--r--   0        0        0      674 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/plugin.py
--rw-r--r--   0        0        0    12004 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/pool.py
--rw-r--r--   0        0        0        0 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/py.typed
--rw-r--r--   0        0        0     3648 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/region.py
--rw-r--r--   0        0        0     1031 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/search_type.py
--rw-r--r--   0        0        0     3437 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/stats.py
--rw-r--r--   0        0        0     5254 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/strategy.py
--rw-r--r--   0        0        0     4797 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/track.py
--rw-r--r--   0        0        0      747 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/type_variables.py
--rw-r--r--   0        0        0      199 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/__init__.py
--rw-r--r--   0        0        0     2996 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/common.py
--rw-r--r--   0        0        0     4712 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/http.py
--rw-r--r--   0        0        0     2385 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/incoming.py
--rw-r--r--   0        0        0      602 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/misc.py
--rw-r--r--   0        0        0     1189 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/typings/outgoing.py
--rw-r--r--   0        0        0      117 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/utils/__init__.py
--rw-r--r--   0        0        0     1203 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/utils/classproperty.py
--rw-r--r--   0        0        0      745 2023-06-02 13:31:53.013765 mafic-2.8.0/mafic/warnings.py
--rw-r--r--   0        0        0     3766 2023-06-02 13:31:53.013765 mafic-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-04 00:26:13.677316 mafic-2.9.0/LICENSE
+-rw-r--r--   0        0        0     3315 2023-06-04 00:26:13.677316 mafic-2.9.0/README.md
+-rw-r--r--   0        0        0      886 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/__init__.py
+-rw-r--r--   0        0        0     3554 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/__libraries.py
+-rw-r--r--   0        0        0     1559 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/__main__.py
+-rw-r--r--   0        0        0     4490 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/errors.py
+-rw-r--r--   0        0        0     5617 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/events.py
+-rw-r--r--   0        0        0    27782 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/filter.py
+-rw-r--r--   0        0        0     7397 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/ip.py
+-rw-r--r--   0        0        0    43682 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/node.py
+-rw-r--r--   0        0        0    27445 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/player.py
+-rw-r--r--   0        0        0     1232 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/playlist.py
+-rw-r--r--   0        0        0      674 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/plugin.py
+-rw-r--r--   0        0        0    12004 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/pool.py
+-rw-r--r--   0        0        0        0 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/py.typed
+-rw-r--r--   0        0        0     3648 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/region.py
+-rw-r--r--   0        0        0     1031 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/search_type.py
+-rw-r--r--   0        0        0     3437 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/stats.py
+-rw-r--r--   0        0        0     5254 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/strategy.py
+-rw-r--r--   0        0        0     4797 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/track.py
+-rw-r--r--   0        0        0      747 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/type_variables.py
+-rw-r--r--   0        0        0      199 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/typings/__init__.py
+-rw-r--r--   0        0        0     2996 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/typings/common.py
+-rw-r--r--   0        0        0     4712 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/typings/http.py
+-rw-r--r--   0        0        0     2385 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/typings/incoming.py
+-rw-r--r--   0        0        0      602 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/typings/misc.py
+-rw-r--r--   0        0        0     1189 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/typings/outgoing.py
+-rw-r--r--   0        0        0      117 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/utils/__init__.py
+-rw-r--r--   0        0        0     1203 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/utils/classproperty.py
+-rw-r--r--   0        0        0      745 2023-06-04 00:26:13.681316 mafic-2.9.0/mafic/warnings.py
+-rw-r--r--   0        0        0     3766 2023-06-04 00:26:13.681316 mafic-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.9.0/PKG-INFO
```

### Comparing `mafic-2.8.0/LICENSE` & `mafic-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/README.md` & `mafic-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/__init__.py` & `mafic-2.9.0/mafic/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .track import *
 from .warnings import *
 
 __title__ = "mafic"
 __author__ = "ooliver1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present ooliver1"
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 """The current version of mafic, using `PEP 440`_ format.
 
 .. _PEP 440: https://peps.python.org/pep-0440/
 """
 
 del __libraries
```

### Comparing `mafic-2.8.0/mafic/__libraries.py` & `mafic-2.9.0/mafic/__libraries.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/__main__.py` & `mafic-2.9.0/mafic/__main__.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/errors.py` & `mafic-2.9.0/mafic/errors.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/events.py` & `mafic-2.9.0/mafic/events.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/filter.py` & `mafic-2.9.0/mafic/filter.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/ip.py` & `mafic-2.9.0/mafic/ip.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/node.py` & `mafic-2.9.0/mafic/node.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/player.py` & `mafic-2.9.0/mafic/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """A Player is used to connect to a channel."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import asyncio
+import warnings
 from asyncio import Event
 from collections import OrderedDict
 from functools import reduce
 from logging import getLogger
 from operator import or_
 from time import time
 from typing import TYPE_CHECKING, Generic, cast
@@ -453,14 +454,22 @@
         if not self._connected and not force:
             return
 
         # Handled by Discord
         if self.client.is_closed():
             return
 
+        _log.debug(
+            "Disconnecting player and destroying client.",
+            extra={"guild": self._guild_id},
+        )
+        if self._node is not None:
+            self._node.remove_player(self.guild.id)
+            await self._node.destroy(guild_id=self.guild.id)
+
         try:
             _log.debug(
                 "Disconnecting from voice channel.",
                 extra={"guild": self._guild_id},
             )
             await self.guild.change_voice_state(channel=None)
         finally:
@@ -525,29 +534,22 @@
             volume=state["volume"],
             pause=self._paused,
             filter=reduce(or_, self._filters.values()) if self._filters else Filter(),
         )
 
         await old_node.destroy(guild_id=self.guild.id)
 
-    async def destroy(self) -> None:
-        """Destroy the player.
-
-        This will disconnect the player and remove it from the node.
-        """
-        _log.debug(
-            "Disconnecting player and destroying client.",
-            extra={"guild": self._guild_id},
+    async def destroy(self) -> None:  # noqa: D102
+        warnings.warn(
+            "Player.destroy is deprecated and will be removed in 3.0.0, "
+            "use .disconnect instead.",
+            DeprecationWarning,
         )
         await self.disconnect()
 
-        if self._node is not None:
-            self._node.remove_player(self.guild.id)
-            await self._node.destroy(guild_id=self.guild.id)
-
     async def fetch_tracks(
         self, query: str, search_type: SearchType | str = SearchType.YOUTUBE
     ) -> list[Track] | Playlist | None:
         r"""Fetch tracks from the node.
 
         Parameters
         ----------
```

### Comparing `mafic-2.8.0/mafic/playlist.py` & `mafic-2.9.0/mafic/playlist.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/plugin.py` & `mafic-2.9.0/mafic/plugin.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/pool.py` & `mafic-2.9.0/mafic/pool.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/region.py` & `mafic-2.9.0/mafic/region.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/search_type.py` & `mafic-2.9.0/mafic/search_type.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/stats.py` & `mafic-2.9.0/mafic/stats.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/strategy.py` & `mafic-2.9.0/mafic/strategy.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/track.py` & `mafic-2.9.0/mafic/track.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/type_variables.py` & `mafic-2.9.0/mafic/type_variables.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/typings/common.py` & `mafic-2.9.0/mafic/typings/common.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/typings/http.py` & `mafic-2.9.0/mafic/typings/http.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/typings/incoming.py` & `mafic-2.9.0/mafic/typings/incoming.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/typings/misc.py` & `mafic-2.9.0/mafic/typings/misc.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/typings/outgoing.py` & `mafic-2.9.0/mafic/typings/outgoing.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/utils/classproperty.py` & `mafic-2.9.0/mafic/utils/classproperty.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/mafic/warnings.py` & `mafic-2.9.0/mafic/warnings.py`

 * *Files identical despite different names*

### Comparing `mafic-2.8.0/pyproject.toml` & `mafic-2.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mafic"
-version = "2.8.0"
+version = "2.9.0"
 description = "A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord."
 authors = ["ooliver1 <oliverwilkes2006@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ooliver1/mafic"
 homepage = "https://github.com/ooliver1/mafic"
 keywords = [
```

### Comparing `mafic-2.8.0/PKG-INFO` & `mafic-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafic
-Version: 2.8.0
+Version: 2.9.0
 Summary: A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 Home-page: https://github.com/ooliver1/mafic
 License: MIT
 Keywords: nextcord,disnake,discord,disnake.py,lavalink,lavalink.py,pycord,py-cord
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
```

