# Comparing `tmp/algviz-0.2.2.tar.gz` & `tmp/algviz-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algviz-0.2.2.tar", last modified: Fri Dec 23 11:39:21 2022, max compression
+gzip compressed data, was "algviz-0.2.3.tar", last modified: Sun Jun  4 17:07:59 2023, max compression
```

## Comparing `algviz-0.2.2.tar` & `algviz-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-12-23 11:39:21.345683 algviz-0.2.2/
--rw-rw-rw-   0        0        0    35149 2022-05-22 10:50:14.000000 algviz-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     4097 2022-12-23 11:39:21.345683 algviz-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3184 2022-12-23 02:23:33.000000 algviz-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-23 11:39:21.317659 algviz-0.2.2/algviz/
--rw-rw-rw-   0        0        0     2838 2022-12-23 03:23:45.000000 algviz-0.2.2/algviz/__init__.py
--rw-rw-rw-   0        0        0    15093 2022-12-23 04:24:34.000000 algviz-0.2.2/algviz/cursor.py
--rw-rw-rw-   0        0        0     7626 2022-12-23 04:24:53.000000 algviz-0.2.2/algviz/graph.py
--rw-rw-rw-   0        0        0     3658 2022-12-23 04:29:05.000000 algviz-0.2.2/algviz/graph_node_base.py
--rw-rw-rw-   0        0        0     5211 2022-12-23 04:29:24.000000 algviz-0.2.2/algviz/linked_list.py
--rw-rw-rw-   0        0        0     3408 2022-12-23 04:29:32.000000 algviz-0.2.2/algviz/logger.py
--rw-rw-rw-   0        0        0     6088 2022-12-23 09:41:37.000000 algviz-0.2.2/algviz/map.py
--rw-rw-rw-   0        0        0    35861 2022-12-23 09:09:51.000000 algviz-0.2.2/algviz/svg_graph.py
--rw-rw-rw-   0        0        0    20308 2022-12-23 04:33:10.000000 algviz-0.2.2/algviz/svg_table.py
--rw-rw-rw-   0        0        0    19494 2022-12-23 04:33:23.000000 algviz-0.2.2/algviz/table.py
--rw-rw-rw-   0        0        0    12028 2022-12-23 04:34:15.000000 algviz-0.2.2/algviz/tree.py
--rw-rw-rw-   0        0        0    13280 2022-12-23 11:08:08.000000 algviz-0.2.2/algviz/utility.py
--rw-rw-rw-   0        0        0    21393 2022-12-23 04:35:13.000000 algviz-0.2.2/algviz/vector.py
--rw-rw-rw-   0        0        0     9785 2022-12-23 08:34:41.000000 algviz-0.2.2/algviz/visual.py
-drwxrwxrwx   0        0        0        0 2022-12-23 11:39:21.344683 algviz-0.2.2/algviz.egg-info/
--rw-rw-rw-   0        0        0     4097 2022-12-23 11:39:21.000000 algviz-0.2.2/algviz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2022-12-23 11:39:21.000000 algviz-0.2.2/algviz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-23 11:39:21.000000 algviz-0.2.2/algviz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-23 11:39:20.000000 algviz-0.2.2/algviz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2022-12-23 11:39:21.000000 algviz-0.2.2/algviz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-12-23 11:39:21.000000 algviz-0.2.2/algviz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-23 11:39:21.345683 algviz-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1446 2022-12-23 11:07:59.000000 algviz-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:07:59.656408 algviz-0.2.3/
+-rw-rw-rw-   0        0        0    35149 2022-05-22 10:50:14.000000 algviz-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     4360 2023-06-04 17:07:59.655912 algviz-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3446 2023-05-05 10:41:17.000000 algviz-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 17:07:59.642998 algviz-0.2.3/algviz/
+-rw-rw-rw-   0        0        0     2964 2023-06-04 13:51:17.000000 algviz-0.2.3/algviz/__init__.py
+-rw-rw-rw-   0        0        0    15093 2022-12-23 04:24:34.000000 algviz-0.2.3/algviz/cursor.py
+-rw-rw-rw-   0        0        0    11159 2023-06-04 16:53:31.000000 algviz-0.2.3/algviz/graph.py
+-rw-rw-rw-   0        0        0     3658 2022-12-23 04:29:05.000000 algviz-0.2.3/algviz/graph_node_base.py
+-rw-rw-rw-   0        0        0     5211 2022-12-23 04:29:24.000000 algviz-0.2.3/algviz/linked_list.py
+-rw-rw-rw-   0        0        0     3408 2022-12-23 04:29:32.000000 algviz-0.2.3/algviz/logger.py
+-rw-rw-rw-   0        0        0     6088 2022-12-23 09:41:37.000000 algviz-0.2.3/algviz/map.py
+-rw-rw-rw-   0        0        0    35861 2022-12-23 09:09:51.000000 algviz-0.2.3/algviz/svg_graph.py
+-rw-rw-rw-   0        0        0    20308 2022-12-23 04:33:10.000000 algviz-0.2.3/algviz/svg_table.py
+-rw-rw-rw-   0        0        0    19828 2023-05-24 12:25:12.000000 algviz-0.2.3/algviz/table.py
+-rw-rw-rw-   0        0        0    12028 2022-12-23 04:34:15.000000 algviz-0.2.3/algviz/tree.py
+-rw-rw-rw-   0        0        0    13626 2023-06-04 16:42:18.000000 algviz-0.2.3/algviz/utility.py
+-rw-rw-rw-   0        0        0    21393 2022-12-23 04:35:13.000000 algviz-0.2.3/algviz/vector.py
+-rw-rw-rw-   0        0        0     9785 2023-05-24 13:11:24.000000 algviz-0.2.3/algviz/visual.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:07:59.649952 algviz-0.2.3/algviz.egg-info/
+-rw-rw-rw-   0        0        0     4360 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       82 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:07:59.656408 algviz-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2023-06-04 16:41:58.000000 algviz-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:07:59.655415 algviz-0.2.3/tests/
+-rw-rw-rw-   0        0        0    11071 2023-06-04 14:03:48.000000 algviz-0.2.3/tests/test_graph.py
+-rw-rw-rw-   0        0        0    10959 2022-12-23 04:06:37.000000 algviz-0.2.3/tests/test_linked_list.py
+-rw-rw-rw-   0        0        0     1972 2022-12-23 04:03:34.000000 algviz-0.2.3/tests/test_logger.py
+-rw-rw-rw-   0        0        0     4097 2022-12-23 10:32:23.000000 algviz-0.2.3/tests/test_map.py
+-rw-rw-rw-   0        0        0      921 2023-05-24 12:50:29.000000 algviz-0.2.3/tests/test_regression.py
+-rw-rw-rw-   0        0        0    11905 2022-12-23 04:06:44.000000 algviz-0.2.3/tests/test_table.py
+-rw-rw-rw-   0        0        0    10612 2022-12-23 04:42:51.000000 algviz-0.2.3/tests/test_tree.py
+-rw-rw-rw-   0        0        0    10670 2022-12-23 04:07:06.000000 algviz-0.2.3/tests/test_vector.py
```

### Comparing `algviz-0.2.2/LICENSE` & `algviz-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/PKG-INFO` & `algviz-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algviz
-Version: 0.2.2
+Version: 0.2.3
 Summary: An algorithm visualization tool for jupyter notebook to show animation for vector, table, linked list, tree and graph data structures.
 Home-page: https://algviz.com/
 Author: zjl9959
 Author-email: zjl9959@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://algviz.readthedocs.io/en/latest/index.html
 Project-URL: Issue Tracker, https://github.com/zjl9959/algviz/issues
@@ -66,15 +66,15 @@
 
 ![bubble_sort_animation](https://cdn.jsdelivr.net/gh/zjl9959/algviz-launch@master/svgs/BubbleSort.svg)
 
 ## Examples
 
 Ready to see the magic? Click this button to try more algorithms on Gitpod!
 
-[![Open algviz examples in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/zjl9959/algviz-launch)
+[![Open algviz examples in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/zjl9959/algviz-launch) *Need to login with your github account.*
 
 ## Installation
 
 Please follow this [installation guide](https://algviz.com/en/installation.html) to setup algviz.
 
 ## Tutorial
 
@@ -86,13 +86,14 @@
 
 Algviz uses GNU general public [LICENSE](https://github.com/zjl9959/algviz/blob/main/LICENSE). You can use it freely for learning and communication.
 
 ## Contribution
 
 Any form of contribution is welcomed! Please feel free to report a [bug](https://github.com/zjl9959/algviz/issues) or create a [pull request](https://github.com/zjl9959/algviz/pulls).
 
+If you want to share your algorithm animation notebooks using algviz, you can create a [PR](https://github.com/zjl9959/algviz-launch/pulls) from this repo: 👉 [algviz-launch](https://github.com/zjl9959/algviz-launch).
 
 [bubble sort algorithm]: https://en.wikipedia.org/wiki/Bubble_sort
 [vector.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_vector.svg
 [table.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_table.svg
 [tree.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_tree.svg
 [graph.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_graph.svg
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `algviz-0.2.2/README.md` & `algviz-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 ![bubble_sort_animation](https://cdn.jsdelivr.net/gh/zjl9959/algviz-launch@master/svgs/BubbleSort.svg)
 
 ## Examples
 
 Ready to see the magic? Click this button to try more algorithms on Gitpod!
 
-[![Open algviz examples in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/zjl9959/algviz-launch)
+[![Open algviz examples in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/zjl9959/algviz-launch) *Need to login with your github account.*
 
 ## Installation
 
 Please follow this [installation guide](https://algviz.com/en/installation.html) to setup algviz.
 
 ## Tutorial
 
@@ -67,13 +67,14 @@
 
 Algviz uses GNU general public [LICENSE](https://github.com/zjl9959/algviz/blob/main/LICENSE). You can use it freely for learning and communication.
 
 ## Contribution
 
 Any form of contribution is welcomed! Please feel free to report a [bug](https://github.com/zjl9959/algviz/issues) or create a [pull request](https://github.com/zjl9959/algviz/pulls).
 
+If you want to share your algorithm animation notebooks using algviz, you can create a [PR](https://github.com/zjl9959/algviz-launch/pulls) from this repo: 👉 [algviz-launch](https://github.com/zjl9959/algviz-launch).
 
 [bubble sort algorithm]: https://en.wikipedia.org/wiki/Bubble_sort
 [vector.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_vector.svg
 [table.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_table.svg
 [tree.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_tree.svg
 [graph.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_graph.svg
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `algviz-0.2.2/algviz/__init__.py` & `algviz-0.2.3/algviz/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 Author: zjl9959@gmail.com
 
 License: GPLv3
 
 """
 
 from .visual import Visualizer
-from .graph import GraphNode, parseGraph, updateGraphEdge
+from .graph import GraphNode, parseGraph, updateGraphEdge, generateRandomGraph
 from .tree import BinaryTreeNode, TreeNode, RecursiveTree, parseBinaryTree, parseTree
 from .linked_list import ForwardLinkedListNode, DoublyLinkedListNode
 from .linked_list import parseForwardLinkedList, parseDoublyLinkedList
-from .utility import _version, AlgvizParamError, AlgvizRuntimeError, AlgvizFatalError, AlgvizTypeError
+from .utility import _version, set_up_random_seed
+from .utility import AlgvizParamError, AlgvizRuntimeError, AlgvizFatalError, AlgvizTypeError
 
 
 # Common colors name to RGB map (see: https://www.w3schools.com/tags/ref_colornames.asp)
 cAqua = (0, 255, 255)
 cBlack = (0, 0, 0)
 cBlue = (0, 0, 255)
 cBrown = (165, 42, 42)
@@ -77,20 +78,24 @@
 color_wheat = (245, 222, 179)
 color_white = (255, 255, 255)
 color_yellow = (255, 255, 0)
 
 
 __all__ = [
     'Visualizer',
-    'GraphNode', 'parseGraph', 'updateGraphEdge',
+    'GraphNode', 'parseGraph', 'updateGraphEdge', 'generateRandomGraph',
     'BinaryTreeNode', 'TreeNode', 'RecursiveTree', 'parseBinaryTree', 'parseTree',
     'ForwardLinkedListNode', 'DoublyLinkedListNode',
     'parseForwardLinkedList', 'parseDoublyLinkedList',
     'AlgvizParamError', 'AlgvizRuntimeError', 'AlgvizFatalError', 'AlgvizTypeError'
 ]
 
 
 __title__ = 'algviz'
 __version__ = _version
 __author__ = 'zjl9959@gmail.com'
 __license__ = 'GNU General Public License (GPLv3)'
 __help__ = "Visit https://algviz.com for more information."
+
+
+# Init the module.
+set_up_random_seed()
```

### Comparing `algviz-0.2.2/algviz/cursor.py` & `algviz-0.2.3/algviz/cursor.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/algviz/graph.py` & `algviz-0.2.3/algviz/graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -216,7 +216,91 @@
                 edge_val = edge[2]
             nodes_dict[node1].add(nodes_dict[node2], edge_val)
             if directed is False:
                 nodes_dict[node2].add(nodes_dict[node1], edge_val)
         else:
             raise AlgvizRuntimeError('(paraseGraph) can not find node object for edge {}.'.format(edge))
     return nodes_dict
+
+
+def generateRandomGraph(nb_nodes, nb_edges, max_degree=None, directed=False):
+    """Generate a random graph with the given constraint.
+
+    Args:
+        nb_nodes (int): the nodes number of this graph, the node id start from 0.
+        nb_edges (int): the edges number of this graph.
+        max_degree (max_degree): the maximum degree for graph nodes(minimum degree is 1).
+        directed (boolean): is this a directed graph or not.
+
+    Returns:
+        nodes (set(printable)), edges (list(tuple(node1, node2, edge))): all the nodes in this graph and all the edges in this graph.
+
+    Raises:
+        AlgvizParamError: generateRandomGraph: input nodes number should be greater than 0.
+        AlgvizParamError: generateRandomGraph: input edges number should be greater or equal than nodes number.
+        AlgvizParamError: generateRandomGraph: max_degree is not enough to generate such edges.
+        AlgvizRuntimeError: generateRandomGraph: can not pick a suitable node.
+    """
+    def random_pick_nodes(nodes_list, nodes_degree, exclude=list()):
+        pick_list = []
+        for n in nodes_list:
+            if nodes_degree[n] < max_degree and n not in exclude:
+                pick_list.append(n)
+        if len(pick_list) == 0:
+            return None
+        index = randint(0, len(pick_list) - 1)
+        return pick_list[index]
+
+    if max_degree is None:
+        max_degree = nb_nodes
+    if directed:
+        max_degree = min(max_degree, 2 * (nb_nodes - 1))
+    else:
+        max_degree = min(max_degree, nb_nodes - 1)
+
+    if nb_nodes < 0:
+        raise AlgvizParamError('generateRandomGraph: input nodes number should be greater than 0.')
+    if nb_edges < nb_nodes:
+        raise AlgvizParamError('generateRandomGraph: input edges number should be greater or equal than nodes number.')
+    if nb_nodes * max_degree < nb_edges * 2:
+        raise AlgvizParamError('generateRandomGraph: max_degree is not enough to generate such edges.')
+    from random import randint
+    # Create nodes for this graph.
+    nodes_not_in_graph = list()
+    nodes_degree = dict()
+    for i in range(nb_nodes):
+        nodes_not_in_graph.append(i)
+        nodes_degree[i] = 0
+    # Random pick nodes and generate edges.
+    edges = list()
+    # Make sure none node is isolate.
+    nodes_in_graph = list()
+    while len(nodes_not_in_graph) > 0:
+        index1 = randint(0, len(nodes_not_in_graph) - 1)
+        n1 = nodes_not_in_graph[index1]
+        if len(nodes_in_graph) > 0:
+            n2 = random_pick_nodes(nodes_in_graph, nodes_degree)
+            if n2 is None:
+                raise AlgvizRuntimeError('generateRandomGraph: can not pick a suitable node.')
+            edges.append((n1, n2))
+            nodes_degree[n2] += 1
+            nodes_degree[n1] += 1
+        nodes_in_graph.append(n1)
+        nodes_not_in_graph.pop(index1)
+    # Generate the rest edges randomly.
+    while len(edges) < nb_edges:
+        n1 = random_pick_nodes(nodes_in_graph, nodes_degree)
+        n2 = random_pick_nodes(nodes_in_graph, nodes_degree, [n1])
+        if n1 is None or n2 is None:
+            raise AlgvizRuntimeError('generateRandomGraph: can not pick a suitable node.')
+        if randint(0, 1) == 1:
+            n1, n2 = n2, n1
+        if directed:
+            if (n1, n2) in edges:
+                continue
+        else:
+            if (n1, n2) in edges or (n2, n1) in edges:
+                continue
+        edges.append((n1, n2))
+        nodes_degree[n1] += 1
+        nodes_degree[n2] += 1
+    return sorted(nodes_in_graph), edges
```

### Comparing `algviz-0.2.2/algviz/graph_node_base.py` & `algviz-0.2.3/algviz/graph_node_base.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/algviz/linked_list.py` & `algviz-0.2.3/algviz/linked_list.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/algviz/logger.py` & `algviz-0.2.3/algviz/logger.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/algviz/map.py` & `algviz-0.2.3/algviz/map.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/algviz/svg_graph.py` & `algviz-0.2.3/algviz/svg_graph.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/algviz/svg_table.py` & `algviz-0.2.3/algviz/svg_table.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/algviz/table.py` & `algviz-0.2.3/algviz/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -245,35 +245,39 @@
                 for c in range(col):
                     self._data[r].append(None)
                     self._new_rect_in_svg_(r, c)
         elif row < self._row:
             # Remove row in table.
             for r in range(row, self._row):
                 self._data.pop()
-                self._svg.delete_element(self._row_index2text[r])
-                self._row_index2text.pop(r)
                 for c in range(self._col):
                     self._svg.delete_element(self._index2rect[(r, c)])
                     self._index2rect.pop((r, c))
+            if self._show_index:
+                for r in range(row, self._row):
+                    self._svg.delete_element(self._row_index2text[r])
+                    self._row_index2text.pop(r)
         if col > self._col:
             # Add new columns into table.
             for r in range(min(self._row, row)):
                 for c in range(self._col, col):
                     self._data[r].append(None)
                     self._new_rect_in_svg_(r, c)
             for c in range(self._col, col):
                 self._new_col_index_text_in_svg_(c)
         elif col < self._col:
             for r in range(min(self._row, row)):
                 for c in range(col, self._col):
                     self._data[r].pop()
                     self._svg.delete_element(self._index2rect[(r, c)])
                     self._index2rect.pop((r, c))
-            for c in range(col, self._col):
-                self._svg.delete_element(self._col_index2text[c])
+            if self._show_index:
+                for c in range(col, self._col):
+                    self._svg.delete_element(self._col_index2text[c])
+                    self._col_index2text.pop(c)
         self._row = row
         self._col = col
         self._update_svg_size_()
         self._update_subscripts_position_()
 
     def _add_cursor_(self, cursor, is_row):
         """Add a cursor into the cursor manager to track it.
@@ -403,14 +407,16 @@
                 rect_pos_x = c * self._cell_width + self._cell_margin + self._row_cursor_mgr.get_cursors_occupy()
                 rect_pos_y = r * self._cell_height + self._cell_margin + self._col_cursor_mgr.get_cursors_occupy()
                 rect = (rect_pos_x, rect_pos_y, self._cell_width, self._cell_height)
                 gid = self._index2rect[(r, c)]
                 self._svg.update_rect_element(gid, rect)
 
     def _update_subscripts_position_(self):
+        if not self._show_index:
+            return
         for r in range(self._row):
             pos_x = self._col * self._cell_width + self._cell_margin * 2 + self._row_cursor_mgr.get_cursors_occupy()
             pos_y = (r + 0.5) * self._cell_height + self._label_font_size * 0.5 + self._cell_margin + self._col_cursor_mgr.get_cursors_occupy()
             self._svg.update_text_element(self._row_index2text[r], (pos_x, pos_y))
         for c in range(self._col):
             pos_x = (c + 0.5) * self._cell_width - self._label_font_size * len(str(c)) * 0.25 + self._cell_margin + self._row_cursor_mgr.get_cursors_occupy()
             pos_y = self._row * self._cell_height + 1 + self._label_font_size + self._cell_margin + self._col_cursor_mgr.get_cursors_occupy()
@@ -433,17 +439,21 @@
         rect_pos_y = r * self._cell_height + self._cell_margin + self._col_cursor_mgr.get_cursors_occupy()
         rect = (rect_pos_x, rect_pos_y, self._cell_width, self._cell_height)
         gid = self._svg.add_rect_element(rect, self._data[r][c], angle=False)
         self._index2rect[(r, c)] = gid
         self._cell_tcs[gid] = TraceColorStack()
 
     def _new_row_index_text_in_svg_(self, r):
+        if not self._show_index:
+            return
         pos_x = self._col * self._cell_width + self._cell_margin * 2 + self._row_cursor_mgr.get_cursors_occupy()
         pos_y = (r + 0.5) * self._cell_height + self._label_font_size * 0.5 + self._cell_margin + self._col_cursor_mgr.get_cursors_occupy()
         gid = self._svg.add_text_element((pos_x, pos_y), r, self._label_font_size)
         self._row_index2text[r] = gid
 
     def _new_col_index_text_in_svg_(self, c):
+        if not self._show_index:
+            return
         pos_x = (c + 0.5) * self._cell_width - self._label_font_size * len(str(c)) * 0.25 + self._cell_margin + self._row_cursor_mgr.get_cursors_occupy()
         pos_y = self._row * self._cell_height + 1 + self._label_font_size + self._cell_margin + self._col_cursor_mgr.get_cursors_occupy()
         gid = self._svg.add_text_element((pos_x, pos_y), c, self._label_font_size)
         self._col_index2text[c] = gid
```

### Comparing `algviz-0.2.2/algviz/tree.py` & `algviz-0.2.3/algviz/tree.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/algviz/utility.py` & `algviz-0.2.3/algviz/utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 
 Author: zjl9959@gmail.com
 
 License: GPLv3
 
 """
 
-_version = '0.2.2'                  # algviz version
+_version = '0.2.3'                  # algviz version
 _url = 'https://algviz.com'         # The homepage for algviz
+RANDOM_SEED = None
 KFATAL_HELP_INFO = """You can report this bug from link: https://github.com/zjl9959/algviz/issues"""
 
 
 # Define exceptions for algviz runtime.
 class AlgvizParamError(Exception):
     def __init__(self, message):
         super().__init__('[AlgvizParamError] {}'.format(message))
 
 
 class AlgvizRuntimeError(Exception):
     def __init__(self, message):
-        super().__init__('[AlgvizRuntimeError] {}\n{}'.format(message, KFATAL_HELP_INFO))
+        super().__init__('[AlgvizRuntimeError] {}\nrandom_seed={}\n{}'.format(message, RANDOM_SEED, KFATAL_HELP_INFO))
 
 
 class AlgvizFatalError(Exception):
     def __init__(self, message):
-        super().__init__('[AlgvizFatalError] {}\n{}'.format(message, KFATAL_HELP_INFO))
+        super().__init__('[AlgvizFatalError] {}\nrandom_seed={}\n{}'.format(message, RANDOM_SEED, KFATAL_HELP_INFO))
 
 
 class AlgvizTypeError(Exception):
     def __init__(self, obj):
         super().__init__('[AlgvizTypeError] Type {} not support!\n{}'.format(type(obj), KFATAL_HELP_INFO))
 
 
@@ -382,7 +383,19 @@
         return
     svg = svgs[0]
     style = dom.createElement('style')
     style_content = r".txt { alignment-baseline:middle; text-anchor:middle; font-family:Times,serif; }"
     text = dom.createTextNode(style_content)
     style.appendChild(text)
     svg.appendChild(style)
+
+
+def set_up_random_seed():
+    """Set up the random just once when program startup.
+    """
+    global RANDOM_SEED
+    if RANDOM_SEED is not None:
+        return
+    from random import seed
+    from time import time
+    RANDOM_SEED = int(time())
+    seed(RANDOM_SEED)
```

### Comparing `algviz-0.2.2/algviz/vector.py` & `algviz-0.2.3/algviz/vector.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/algviz/visual.py` & `algviz-0.2.3/algviz/visual.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.2/algviz.egg-info/PKG-INFO` & `algviz-0.2.3/algviz.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algviz
-Version: 0.2.2
+Version: 0.2.3
 Summary: An algorithm visualization tool for jupyter notebook to show animation for vector, table, linked list, tree and graph data structures.
 Home-page: https://algviz.com/
 Author: zjl9959
 Author-email: zjl9959@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://algviz.readthedocs.io/en/latest/index.html
 Project-URL: Issue Tracker, https://github.com/zjl9959/algviz/issues
@@ -66,15 +66,15 @@
 
 ![bubble_sort_animation](https://cdn.jsdelivr.net/gh/zjl9959/algviz-launch@master/svgs/BubbleSort.svg)
 
 ## Examples
 
 Ready to see the magic? Click this button to try more algorithms on Gitpod!
 
-[![Open algviz examples in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/zjl9959/algviz-launch)
+[![Open algviz examples in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/zjl9959/algviz-launch) *Need to login with your github account.*
 
 ## Installation
 
 Please follow this [installation guide](https://algviz.com/en/installation.html) to setup algviz.
 
 ## Tutorial
 
@@ -86,13 +86,14 @@
 
 Algviz uses GNU general public [LICENSE](https://github.com/zjl9959/algviz/blob/main/LICENSE). You can use it freely for learning and communication.
 
 ## Contribution
 
 Any form of contribution is welcomed! Please feel free to report a [bug](https://github.com/zjl9959/algviz/issues) or create a [pull request](https://github.com/zjl9959/algviz/pulls).
 
+If you want to share your algorithm animation notebooks using algviz, you can create a [PR](https://github.com/zjl9959/algviz-launch/pulls) from this repo: 👉 [algviz-launch](https://github.com/zjl9959/algviz-launch).
 
 [bubble sort algorithm]: https://en.wikipedia.org/wiki/Bubble_sort
 [vector.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_vector.svg
 [table.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_table.svg
 [tree.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_tree.svg
 [graph.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_graph.svg
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `algviz-0.2.2/setup.py` & `algviz-0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,31 +15,32 @@
 readme_filepath = path.join(script_path, 'README.md')
 long_description_data = ''
 with open(readme_filepath, encoding='utf-8') as f:
     long_description_data = f.read()
 
 setup(
     name="algviz",
-    version="0.2.2",
+    version="0.2.3",
     author="zjl9959",
     author_email="zjl9959@gmail.com",
     description=("An algorithm visualization tool for jupyter notebook to show animation for vector, table, linked list, tree and graph data structures."),
     long_description=long_description_data,
     long_description_content_type="text/markdown",
     license="GPLv3",
     keywords="Algorithm Visualizer Animation Jupyter-notebook Graph",
     url="https://algviz.com/",
     project_urls={
         "Documentation": "https://algviz.readthedocs.io/en/latest/index.html",
         "Issue Tracker": "https://github.com/zjl9959/algviz/issues",
     },
     packages=['algviz'],
     install_requires=[
-        'graphviz >= 0.8.4, != 0.18, <= 0.19.1',
-        'ipykernel >= 6.4.0, <= 6.7.0'
+        'graphviz >= 0.8.4, != 0.18, <= 0.20.1',
+        'ipykernel >= 6.4.0, <= 6.23.1',
+        'ipython >= 8.0.0, <= 8.12.0'
     ],
     python_requires='>=3.8',
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Topic :: Scientific/Engineering :: Visualization",
         'Programming Language :: Python :: 3'
```

