# Comparing `tmp/wikicat-0.0.1.dev7.tar.gz` & `tmp/wikicat-0.0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikicat-0.0.1.dev7.tar", last modified: Sun Jun  4 04:50:34 2023, max compression
+gzip compressed data, was "wikicat-0.0.1.dev8.tar", last modified: Sun Jun  4 19:26:27 2023, max compression
```

## Comparing `wikicat-0.0.1.dev7.tar` & `wikicat-0.0.1.dev8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:50:34.453968 wikicat-0.0.1.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-06-04 04:50:34.453968 wikicat-0.0.1.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:50:34.449967 wikicat-0.0.1.dev7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:50:34.449967 wikicat-0.0.1.dev7/docs/wikicat/
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/docs/wikicat/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/docs/wikicat/viewer.md
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/docs/wikicat.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 04:50:34.453968 wikicat-0.0.1.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:50:34.453968 wikicat-0.0.1.dev7/wikicat/
--rw-r--r--   0 runner    (1001) docker     (123)    29094 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:50:34.453968 wikicat-0.0.1.dev7/wikicat/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/processing/download_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/processing/generate_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/processing/merge_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/processing/process_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 04:50:23.000000 wikicat-0.0.1.dev7/wikicat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:50:34.453968 wikicat-0.0.1.dev7/wikicat/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/viewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/viewer/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-04 04:50:22.000000 wikicat-0.0.1.dev7/wikicat/viewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:50:34.453968 wikicat-0.0.1.dev7/wikicat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-06-04 04:50:34.000000 wikicat-0.0.1.dev7/wikicat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-04 04:50:34.000000 wikicat-0.0.1.dev7/wikicat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 04:50:34.000000 wikicat-0.0.1.dev7/wikicat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-04 04:50:34.000000 wikicat-0.0.1.dev7/wikicat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 04:50:34.000000 wikicat-0.0.1.dev7/wikicat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:26:27.565622 wikicat-0.0.1.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-04 19:26:27.565622 wikicat-0.0.1.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:26:27.561622 wikicat-0.0.1.dev8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:26:27.561622 wikicat-0.0.1.dev8/docs/wikicat/
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/docs/wikicat/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/docs/wikicat/viewer.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/docs/wikicat.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 19:26:27.565622 wikicat-0.0.1.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:26:27.561622 wikicat-0.0.1.dev8/wikicat/
+-rw-r--r--   0 runner    (1001) docker     (123)    29094 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:26:27.565622 wikicat-0.0.1.dev8/wikicat/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/processing/download_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/processing/generate_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/processing/merge_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/processing/process_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:26:27.565622 wikicat-0.0.1.dev8/wikicat/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/viewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/viewer/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-04 19:26:15.000000 wikicat-0.0.1.dev8/wikicat/viewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:26:27.565622 wikicat-0.0.1.dev8/wikicat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-04 19:26:27.000000 wikicat-0.0.1.dev8/wikicat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-04 19:26:27.000000 wikicat-0.0.1.dev8/wikicat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 19:26:27.000000 wikicat-0.0.1.dev8/wikicat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-04 19:26:27.000000 wikicat-0.0.1.dev8/wikicat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 19:26:27.000000 wikicat-0.0.1.dev8/wikicat.egg-info/top_level.txt
```

### Comparing `wikicat-0.0.1.dev7/LICENSE` & `wikicat-0.0.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/PKG-INFO` & `wikicat-0.0.1.dev8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikicat
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: Toolkit for managing and navigating graphs of Wikipedia categories
 Home-page: https://xhluca.github.io/wikicat
 Author: Xing Han Lu, Aristides Milios
 Author-email: wikicat@xinghanlu.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -176,7 +176,13 @@
 ```
 
 See the `wikicat.viewer.build_app()` function for more details.
 
 ## Warning
 
 Because of the size of the graph, some parts of the API (such as the viewer and the processing CLI) require a lot of memory. We recommend using a machine with at least 32 GB of RAM. We are working on a more memory-efficient version of the API.
+
+## Alternatives
+
+`wikicat` was designed for offline and high-throughput workflows, with support for different versions of Wikipedia (as categories change over time). As a result, there's a high overhead (long build time and high RAM usage). If this is not what you are looking for, you can check out alternatives to this library:
+* [MediaWiki](https://www.mediawiki.org/wiki/MediaWiki): This is Wikipedia's web API, and contains documentations for accessing categories (see [API:Categories](https://www.mediawiki.org/wiki/API:Categories) and [API:Categorymembers](https://www.mediawiki.org/wiki/API:Categorymembers))
+* [Wikipedia Histories](https://github.com/ndrezn/wikipedia-histories): This library contains a [domain-level analysis](https://github.com/ndrezn/wikipedia-histories/#domain-level-analysis) module that allows you to query articles associated with a certain category. Since it utilizes the Wikipedia Web API, it does not have the same overhead.
```

### Comparing `wikicat-0.0.1.dev7/README.md` & `wikicat-0.0.1.dev8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -161,7 +161,13 @@
 ```
 
 See the `wikicat.viewer.build_app()` function for more details.
 
 ## Warning
 
 Because of the size of the graph, some parts of the API (such as the viewer and the processing CLI) require a lot of memory. We recommend using a machine with at least 32 GB of RAM. We are working on a more memory-efficient version of the API.
+
+## Alternatives
+
+`wikicat` was designed for offline and high-throughput workflows, with support for different versions of Wikipedia (as categories change over time). As a result, there's a high overhead (long build time and high RAM usage). If this is not what you are looking for, you can check out alternatives to this library:
+* [MediaWiki](https://www.mediawiki.org/wiki/MediaWiki): This is Wikipedia's web API, and contains documentations for accessing categories (see [API:Categories](https://www.mediawiki.org/wiki/API:Categories) and [API:Categorymembers](https://www.mediawiki.org/wiki/API:Categorymembers))
+* [Wikipedia Histories](https://github.com/ndrezn/wikipedia-histories): This library contains a [domain-level analysis](https://github.com/ndrezn/wikipedia-histories/#domain-level-analysis) module that allows you to query articles associated with a certain category. Since it utilizes the Wikipedia Web API, it does not have the same overhead.
```

### Comparing `wikicat-0.0.1.dev7/docs/wikicat/processing.md` & `wikicat-0.0.1.dev8/docs/wikicat/processing.md`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/docs/wikicat/viewer.md` & `wikicat-0.0.1.dev8/docs/wikicat/viewer.md`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/docs/wikicat.md` & `wikicat-0.0.1.dev8/docs/wikicat.md`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/setup.py` & `wikicat-0.0.1.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat/__init__.py` & `wikicat-0.0.1.dev8/wikicat/__init__.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat/constants.py` & `wikicat-0.0.1.dev8/wikicat/constants.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat/processing/download_dump.py` & `wikicat-0.0.1.dev8/wikicat/processing/download_dump.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat/processing/generate_graph.py` & `wikicat-0.0.1.dev8/wikicat/processing/generate_graph.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat/processing/merge_tables.py` & `wikicat-0.0.1.dev8/wikicat/processing/merge_tables.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat/processing/process_dump.py` & `wikicat-0.0.1.dev8/wikicat/processing/process_dump.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat/viewer/__init__.py` & `wikicat-0.0.1.dev8/wikicat/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat/viewer/__main__.py` & `wikicat-0.0.1.dev8/wikicat/viewer/__main__.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat/viewer/components.py` & `wikicat-0.0.1.dev8/wikicat/viewer/components.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat/viewer/utils.py` & `wikicat-0.0.1.dev8/wikicat/viewer/utils.py`

 * *Files identical despite different names*

### Comparing `wikicat-0.0.1.dev7/wikicat.egg-info/PKG-INFO` & `wikicat-0.0.1.dev8/wikicat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikicat
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: Toolkit for managing and navigating graphs of Wikipedia categories
 Home-page: https://xhluca.github.io/wikicat
 Author: Xing Han Lu, Aristides Milios
 Author-email: wikicat@xinghanlu.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -176,7 +176,13 @@
 ```
 
 See the `wikicat.viewer.build_app()` function for more details.
 
 ## Warning
 
 Because of the size of the graph, some parts of the API (such as the viewer and the processing CLI) require a lot of memory. We recommend using a machine with at least 32 GB of RAM. We are working on a more memory-efficient version of the API.
+
+## Alternatives
+
+`wikicat` was designed for offline and high-throughput workflows, with support for different versions of Wikipedia (as categories change over time). As a result, there's a high overhead (long build time and high RAM usage). If this is not what you are looking for, you can check out alternatives to this library:
+* [MediaWiki](https://www.mediawiki.org/wiki/MediaWiki): This is Wikipedia's web API, and contains documentations for accessing categories (see [API:Categories](https://www.mediawiki.org/wiki/API:Categories) and [API:Categorymembers](https://www.mediawiki.org/wiki/API:Categorymembers))
+* [Wikipedia Histories](https://github.com/ndrezn/wikipedia-histories): This library contains a [domain-level analysis](https://github.com/ndrezn/wikipedia-histories/#domain-level-analysis) module that allows you to query articles associated with a certain category. Since it utilizes the Wikipedia Web API, it does not have the same overhead.
```

### Comparing `wikicat-0.0.1.dev7/wikicat.egg-info/SOURCES.txt` & `wikicat-0.0.1.dev8/wikicat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

