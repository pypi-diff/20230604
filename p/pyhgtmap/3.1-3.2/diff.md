# Comparing `tmp/pyhgtmap-3.1.tar.gz` & `tmp/pyhgtmap-3.2.tar.gz`

## Comparing `pyhgtmap-3.1.tar` & `pyhgtmap-3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    31759 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/NASASRTMUtil.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/configUtil.py
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/contour.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/logger.py
--rw-r--r--   0        0        0    23414 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/main.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/varint.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/hgt/__init__.py
--rw-r--r--   0        0        0    27460 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/hgt/file.py
--rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/hgt/processor.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/hgt/tile.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/output/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/output/factory.py
--rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/output/o5mUtil.py
--rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/output/osmUtil.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyhgtmap/output/pbfUtil.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pyhgtmap-3.1/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyhgtmap-3.1/LICENSE.md
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 pyhgtmap-3.1/README.md
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pyhgtmap-3.1/pyproject.toml
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 pyhgtmap-3.1/PKG-INFO
+-rw-r--r--   0        0        0    31759 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/NASASRTMUtil.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/configUtil.py
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/contour.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/logger.py
+-rw-r--r--   0        0        0    23414 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/main.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/varint.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/hgt/__init__.py
+-rw-r--r--   0        0        0    27460 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/hgt/file.py
+-rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/hgt/processor.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/hgt/tile.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/output/__init__.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/output/factory.py
+-rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/output/o5mUtil.py
+-rw-r--r--   0        0        0     6409 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/output/osmUtil.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyhgtmap/output/pbfUtil.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyhgtmap-3.2/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyhgtmap-3.2/LICENSE.md
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 pyhgtmap-3.2/README.md
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyhgtmap-3.2/pyproject.toml
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 pyhgtmap-3.2/PKG-INFO
```

### Comparing `pyhgtmap-3.1/pyhgtmap/NASASRTMUtil.py` & `pyhgtmap-3.2/pyhgtmap/NASASRTMUtil.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/pyhgtmap/configUtil.py` & `pyhgtmap-3.2/pyhgtmap/configUtil.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/pyhgtmap/contour.py` & `pyhgtmap-3.2/pyhgtmap/contour.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/pyhgtmap/logger.py` & `pyhgtmap-3.2/pyhgtmap/logger.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/pyhgtmap/main.py` & `pyhgtmap-3.2/pyhgtmap/main.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/pyhgtmap/varint.py` & `pyhgtmap-3.2/pyhgtmap/varint.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/pyhgtmap/hgt/__init__.py` & `pyhgtmap-3.2/pyhgtmap/hgt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/pyhgtmap/hgt/file.py` & `pyhgtmap-3.2/pyhgtmap/hgt/file.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/pyhgtmap/hgt/processor.py` & `pyhgtmap-3.2/pyhgtmap/hgt/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         Args:
             nb_jobs (int): Max number of processes allowed (>1 to enable parallelization)
             node_start_id (int): ID of the first generated node
             way_start_id (int): ID of the first generated way
             options (optparse options): general options
         """
         self.next_node_id: Synchronized = cast(
-            Synchronized, multiprocessing.Value("i", node_start_id)
+            Synchronized, multiprocessing.Value("L", node_start_id)
         )
         self.next_way_id: Synchronized = cast(
-            Synchronized, multiprocessing.Value("i", way_start_id)
+            Synchronized, multiprocessing.Value("L", way_start_id)
         )
         self.available_children = multiprocessing.Semaphore(nb_jobs)
         self.parallel: bool = nb_jobs > 1
         # Not joined yet children
         self.active_children: List[ForkProcess] = []
         # Errors raised by previously joined children
         self.children_errors: List[Tuple[int, int]] = []
```

### Comparing `pyhgtmap-3.1/pyhgtmap/hgt/tile.py` & `pyhgtmap-3.2/pyhgtmap/hgt/tile.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/pyhgtmap/output/__init__.py` & `pyhgtmap-3.2/pyhgtmap/output/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
-from typing import Callable, List, NamedTuple, Tuple
+from typing import Any, Callable, List, NamedTuple, Tuple
 
 import numpy
+from nptyping import NDArray, Structure
 
 from pyhgtmap.hgt.tile import TileContours
 
 logger = logging.getLogger(__name__)
 
 # First node ID, number of nodes, closed loop, elevation
 WayType = NamedTuple(
@@ -14,14 +15,20 @@
         ("first_node_id", int),
         ("nb_nodes", int),
         ("closed_loop", bool),
         ("elevation", int),
     ],
 )
 
+# Efficient representation of many ways (array of 4-tuple, similar to a list of WayType)
+WaysType = NDArray[
+    Any,
+    Structure["first_node_id: Int, nb_nodes: Int, closed_loop: Bool, elevation: Int"],
+]
+
 NodeType = Tuple[int, int]
 
 
 def make_elev_classifier(majorDivisor: int, mediumDivisor: int) -> Callable[[int], str]:
     """returns a function taking an elevation and returning a
     category specifying whether it's a major, medium or minor contour.
     """
@@ -38,45 +45,49 @@
 
 
 class Output:
     """Base class for all output modules."""
 
     def __init__(self) -> None:
         self.timestampString: str
-        self.ways_pending_write: List[Tuple[List[WayType], int]] = []
+        self.ways_pending_write: List[Tuple[WaysType, int]] = []
 
     def write_nodes(
         self,
         tile_contours: TileContours,
         timestamp_string: str,
         start_node_id: int,
         osm_version: float,
-    ) -> Tuple[int, List[WayType]]:
+    ) -> Tuple[int, WaysType]:
         """
         Write nodes and prepare associated ways.
         Return (latest_node_id, [ways]) tuple.
         """
         raise NotImplementedError
 
-    def write_ways(self, ways: List[WayType], start_way_id: int) -> None:
+    def write_ways(self, ways: WaysType, start_way_id: int) -> None:
         """
         Add ways previously prepared by write_nodes to be written later
         (as ways should ideally be written after all nodes).
         """
         self.ways_pending_write.append((ways, start_way_id))
 
-    def _write_ways(self, ways: List[WayType], start_way_id: int) -> None:
+    def _write_ways(self, ways: WaysType, start_way_id: int) -> None:
         """Actually write ways, upon output finalization via done()."""
         raise NotImplementedError
 
     def done(self) -> None:
         """Finalize and close file."""
-        logger.debug("done() - Writing pending ways")
+        logger.debug(
+            "done() - Writing %s pending ways",
+            sum([len(x[0]) for x in self.ways_pending_write]),
+        )
         for ways, start_way_id in self.ways_pending_write:
             self._write_ways(ways, start_way_id)
+        logger.debug("done() - done!")
 
     def flush(self) -> None:
         """Flush file to disk."""
         raise NotImplementedError
 
 
 class Id(object):
@@ -117,7 +128,22 @@
         newNodes, nodeRefs = _makePoints(path, IDCounter, precision)
         nodes.extend(newNodes)
         if nodeRefs[0] == nodeRefs[-1]:
             ways.append(WayType(nodeRefs[0], len(nodeRefs) - 1, True, elevation))
         else:
             ways.append(WayType(nodeRefs[0], len(nodeRefs), False, elevation))
     return nodes, ways
+
+
+def build_efficient_ways(ways: List[WayType]) -> WaysType:
+    """Convert a list of ways (tuples) into a more efficient numpy array."""
+    return numpy.array(
+        ways,
+        dtype=numpy.dtype(
+            [
+                ("first_node_id", int),
+                ("nb_nodes", int),
+                ("closed_loop", bool),
+                ("elevation", int),
+            ]
+        ),
+    )  # type: ignore  # not supported by pylance
```

### Comparing `pyhgtmap-3.1/pyhgtmap/output/factory.py` & `pyhgtmap-3.2/pyhgtmap/output/factory.py`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/pyhgtmap/output/o5mUtil.py` & `pyhgtmap-3.2/pyhgtmap/output/o5mUtil.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- encoding: utf-8 -*-
 
 
 import time
-from typing import Callable, List, Tuple
+from typing import Callable, Tuple
 
 import pyhgtmap.output
 from pyhgtmap import output
 from pyhgtmap.hgt.tile import TileContours
 from pyhgtmap.varint import int2str, join, sint2str, writableInt, writableString
 
 HUNDREDNANO = 10000000
@@ -169,39 +169,39 @@
             deltaLon = sint2str(lon)
             deltaLat = sint2str(lat)
         data.append(deltaLon)
         data.append(deltaLat)
         # no tags, so data is complete now
         return join(data)
 
-    def _write_ways(self, ways, startWayId):
+    def _write_ways(self, ways: pyhgtmap.output.WaysType, startWayId):
         """writes ways to self.outf.  ways shall be a list of
         (<startNodeId>, <length>, <isCycle>, <elevation>) tuples.
         """
         if len(ways) == 0:
             return
         # write a reset byte
         self.writeReset()
         # write the first way
         self.writeWay(ways[0], idDelta=startWayId, first=True)
         # write all other ways
         for way in ways[1:]:
             self.writeWay(way, idDelta=1)
 
-    def writeWay(self, way, idDelta, first=False):
+    def writeWay(self, way: pyhgtmap.output.WayType, idDelta, first=False):
         wayDataset = []
         # 0x11 means way
         wayDataset.append(writableInt(0x11))
         wayData = self.makeWayData(way, idDelta, first)
         wayDataLen = len(wayData)
         wayDataset.append(int2str(wayDataLen))
         wayDataset.append(wayData)
         self.outf.write(join(wayDataset))
 
-    def makeWayData(self, way, idDelta, first):
+    def makeWayData(self, way: pyhgtmap.output.WayType, idDelta, first):
         startNodeId, length, isCycle, elevation = way
         data = []
         data.append(sint2str(idDelta))
         # version information
         if first:
             # first way
             data.append(self.makeVersionChunk(first=True))
@@ -259,24 +259,24 @@
 
     def write_nodes(
         self,
         tile_contours: TileContours,
         timestamp_string: str,
         start_node_id: int,
         osm_version: float,
-    ) -> Tuple[int, List[output.WayType]]:
+    ) -> Tuple[int, output.WaysType]:
         return writeNodes(self, tile_contours, timestamp_string, start_node_id)
 
 
 def writeNodes(
     output: Output,
     tile_contours: TileContours,
-    timestampString,
+    timestampString,  # dummy option
     start_node_id,
-):  # dummy option
+) -> Tuple[int, output.WaysType]:
     IDCounter = pyhgtmap.output.Id(start_node_id)
     ways = []
     nodes = []
     startId = start_node_id
     for elevation, contourList in tile_contours.contours.items():
         if not contourList:
             continue
@@ -290,8 +290,8 @@
             output.flush()
             startId = IDCounter.curId
             nodes = []
     newId = IDCounter.getId()
     if len(nodes) > 0:
         output.write(str((startId, nodes)) + "\n")
         output.flush()
-    return newId, ways
+    return newId, pyhgtmap.output.build_efficient_ways(ways)
```

### Comparing `pyhgtmap-3.1/pyhgtmap/output/osmUtil.py` & `pyhgtmap-3.2/pyhgtmap/output/osmUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import time
 from io import IOBase
-from typing import Callable, List, Tuple
+from typing import Callable, Tuple
 
 import numpy
 
 import pyhgtmap.output
 from pyhgtmap.hgt.tile import TileContours
 from pyhgtmap.varint import writableString
 
@@ -76,15 +76,15 @@
 
     def write(self, output):
         self.outF.write(writableString(output))
 
     def flush(self) -> None:
         self.outF.flush()
 
-    def _write_ways(self, ways, startWayId):
+    def _write_ways(self, ways: pyhgtmap.output.WaysType, startWayId):
         IDCounter = pyhgtmap.output.Id(startWayId)
         for startNodeId, length, isCycle, elevation in ways:
             IDCounter.curId += 1
             nodeIds = list(range(startNodeId, startNodeId + length))
             if isCycle:
                 nodeIds.append(nodeIds[0])
             nodeRefs = ('<nd ref="{:d}"/>\n' * len(nodeIds)).format(*nodeIds)
@@ -105,15 +105,15 @@
 
     def write_nodes(
         self,
         tile_contours: TileContours,
         timestamp_string: str,
         start_node_id: int,
         osm_version: float,
-    ) -> Tuple[int, List[pyhgtmap.output.WayType]]:
+    ) -> Tuple[int, pyhgtmap.output.WaysType]:
         return writeXML(
             self, tile_contours, timestamp_string, start_node_id, osm_version
         )
 
 
 def _makePoints(output, path, IDCounter, versionString, timestampString):
     """writes OSM representations of the points making up a path to
@@ -159,15 +159,15 @@
         else:
             ways.append((nodeRefs[0], len(nodeRefs), False, elevation))
     return ways
 
 
 def writeXML(
     output, tile_contours: TileContours, timestampString, start_node_id, osm_version
-):
+) -> Tuple[int, pyhgtmap.output.WaysType]:
     """emits node OSM XML to <output> and collects path information.
 
     <output> may be anything having a write method.  For now, its used with
     Output instance or an open pipe to the parent process, if running in parallel.
 
     <contourData> is a pyhgtmap.hgt.ContourObject instance, <elevations> a list
     of elevations to generate contour lines for.
@@ -191,8 +191,8 @@
                 IDCounter,
                 versionString,
                 timestampString,
             )
         )
         # output.flush()
     newId = IDCounter.getId()
-    return newId, ways
+    return newId, pyhgtmap.output.build_efficient_ways(ways)
```

### Comparing `pyhgtmap-3.1/pyhgtmap/output/pbfUtil.py` & `pyhgtmap-3.2/pyhgtmap/output/pbfUtil.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- encoding: utf-8 -*-
 
 import logging
 import os
 import time
 from typing import Callable, List, Tuple
 
-import numpy
-import numpy.typing
 import npyosmium
 import npyosmium.io
 import npyosmium.osm
 import npyosmium.osm.mutable
+import numpy
+import numpy.typing
 
 import pyhgtmap.output
 from pyhgtmap.hgt.tile import TileContours
 
 logger = logging.getLogger(__name__)
 
 BUFFER_SIZE: int = 4096 * 1024
@@ -65,30 +65,34 @@
         osm_header.set(
             key="generator",
             value="pyhgtmap {0:s}".format(pyhgtmap_version),
         )
 
         return osm_header
 
-    def _write_ways(self, ways: List[pyhgtmap.output.WayType], startWayId) -> None:
+    def _write_ways(self, ways: pyhgtmap.output.WaysType, startWayId) -> None:
         """writes ways to self.outf.  ways shall be a list of
         (<startNodeId>, <length>, <isCycle>, <elevation>) tuples.
 
         The waylist is split up to make sure the pbf blobs will not be too big.
         """
         for ind, way in enumerate(ways):
-            closed_loop_id: list[int] = [way.first_node_id] if way.closed_loop else []
+            closed_loop_id: list[int] = (
+                [way["first_node_id"]] if way["closed_loop"] else []
+            )
             osm_way = npyosmium.osm.mutable.Way(
                 id=startWayId + ind,
                 tags=(
-                    ("ele", str(way.elevation)),
+                    ("ele", str(way["elevation"])),
                     ("contour", "elevation"),
-                    ("contour_ext", self.elevClassifier(way.elevation)),
+                    ("contour_ext", self.elevClassifier(way["elevation"])),
                 ),
-                nodes=list(range(way.first_node_id, way.first_node_id + way.nb_nodes))
+                nodes=list(
+                    range(way["first_node_id"], way["first_node_id"] + way["nb_nodes"])
+                )
                 + closed_loop_id,
             )
             self.osm_writer.add_way(osm_way)
 
     def flush(self) -> None:
         pass
 
@@ -98,15 +102,15 @@
 
     def write_nodes(
         self,
         tile_contours: TileContours,
         timestamp_string: str,
         start_node_id: int,
         osm_version: float,
-    ) -> Tuple[int, List[pyhgtmap.output.WayType]]:
+    ) -> Tuple[int, pyhgtmap.output.WaysType]:
         logger.debug(f"writeNodes - startId: {start_node_id}")
 
         ways: List[pyhgtmap.output.WayType] = []
         next_node_id: int = start_node_id
 
         for elevation, contour_list in tile_contours.contours.items():
             # logger.debug(f"writeNodes - elevation: {elevation}")
@@ -126,8 +130,9 @@
                         next_node_id, len(contour), is_closed_way, elevation
                     )
                 )
                 # Bump ID for next iteration
                 next_node_id += len(contour)
 
         logger.debug(f"writeNodes - next_node_id: {next_node_id}")
-        return next_node_id, ways
+
+        return next_node_id, pyhgtmap.output.build_efficient_ways(ways)
```

### Comparing `pyhgtmap-3.1/LICENSE.md` & `pyhgtmap-3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhgtmap-3.1/README.md` & `pyhgtmap-3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/agrenott/pyhgtmap/pythonpackage.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 [![DeepSource](https://deepsource.io/gh/agrenott/pyhgtmap.svg/?label=active+issues&show_trend=true&token=2WJPDv60DJYqaFeVT85eTdGE)](https://deepsource.io/gh/agrenott/pyhgtmap/?ref=repository-badge)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/1251b91e12da4329bd09856d526c91b3)](https://app.codacy.com/gh/agrenott/pyhgtmap/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-[![Maintainability](https://api.codeclimate.com/v1/badges/0af92f6750f1bc0840a3/maintainability)](https://codeclimate.com/github/agrenott/pyhgtmap/maintainability)
+[![Maintainability](https://api.codeclimate.com/v1/badges/96551164b79ce7e76500/maintainability)](https://codeclimate.com/github/agrenott/pyhgtmap/maintainability)
 
 pyhgtmap is a fork of the original ![phyghtmap](http://katze.tfiu.de/projects/phyghtmap/) tool,
 which doesn't seem to be maintained anymore.
 
 This is a little program which lets you easily generate OSM contour lines from
 NASA SRTM data.  It was initially created as replacement for srtm2osm which
 stopped working when the NASA changed the server and started distributing the
```

### Comparing `pyhgtmap-3.1/pyproject.toml` & `pyhgtmap-3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 ]
 dependencies = [
   "bs4>=0.0.1",
   "colorlog>=6.7.0",
   "contourpy>=1.0.7",
   "matplotlib>=3.4.3",
   "numpy>=1.24.2",
+  "nptyping>=2.5.0",
   "npyosmium>=3.6.1",
   "pybind11-rdp>=0.1.3",
   "scipy>=1.8.0",
   "shapely>=2.0.1",
 ]
 description = "Creates OpenStreetMap suitable contour lines from NASA SRTM data"
 dynamic = ["version"]
```

### Comparing `pyhgtmap-3.1/PKG-INFO` & `pyhgtmap-3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhgtmap
-Version: 3.1
+Version: 3.2
 Summary: Creates OpenStreetMap suitable contour lines from NASA SRTM data
 Project-URL: repository, https://github.com/agrenott/pyhgtmap
 Author-email: Adrian Dempwolff <phyghtmap@aldw.de>, Aurélien Grenotton <agrenott@gmail.com>
 License-Expression: GPL-2.0-or-later
 License-File: LICENSE.md
 Keywords: OpenStreetMap,SRTM,countour,elevation,osm
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: bs4>=0.0.1
 Requires-Dist: colorlog>=6.7.0
 Requires-Dist: contourpy>=1.0.7
 Requires-Dist: matplotlib>=3.4.3
+Requires-Dist: nptyping>=2.5.0
 Requires-Dist: npyosmium>=3.6.1
 Requires-Dist: numpy>=1.24.2
 Requires-Dist: pybind11-rdp>=0.1.3
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: shapely>=2.0.1
 Provides-Extra: geotiff
 Requires-Dist: gdal; extra == 'geotiff'
@@ -33,15 +34,15 @@
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/agrenott/pyhgtmap/pythonpackage.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 [![DeepSource](https://deepsource.io/gh/agrenott/pyhgtmap.svg/?label=active+issues&show_trend=true&token=2WJPDv60DJYqaFeVT85eTdGE)](https://deepsource.io/gh/agrenott/pyhgtmap/?ref=repository-badge)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/1251b91e12da4329bd09856d526c91b3)](https://app.codacy.com/gh/agrenott/pyhgtmap/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-[![Maintainability](https://api.codeclimate.com/v1/badges/0af92f6750f1bc0840a3/maintainability)](https://codeclimate.com/github/agrenott/pyhgtmap/maintainability)
+[![Maintainability](https://api.codeclimate.com/v1/badges/96551164b79ce7e76500/maintainability)](https://codeclimate.com/github/agrenott/pyhgtmap/maintainability)
 
 pyhgtmap is a fork of the original ![phyghtmap](http://katze.tfiu.de/projects/phyghtmap/) tool,
 which doesn't seem to be maintained anymore.
 
 This is a little program which lets you easily generate OSM contour lines from
 NASA SRTM data.  It was initially created as replacement for srtm2osm which
 stopped working when the NASA changed the server and started distributing the
```

