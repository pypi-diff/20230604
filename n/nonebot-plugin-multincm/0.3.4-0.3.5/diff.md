# Comparing `tmp/nonebot_plugin_multincm-0.3.4.tar.gz` & `tmp/nonebot_plugin_multincm-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.3.4.tar", last modified: Tue May 30 19:35:15 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.3.5.tar", last modified: Sun Jun  4 17:16:47 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.3.4.tar` & `nonebot_plugin_multincm-0.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/LICENSE
--rw-r--r--   0        0        0     8547 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/README.md
--rw-r--r--   0        0        0     1646 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0    12222 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      623 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0      134 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/const.py
--rw-r--r--   0        0        0     5556 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0    11669 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2928 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0     2279 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/msg_cache.py
--rw-r--r--   0        0        0   212591 2023-05-30 19:34:59.609112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     3007 2023-05-30 19:34:59.609112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      851 2023-05-30 19:34:59.609112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      867 2023-05-30 19:35:15.541289 nonebot_plugin_multincm-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     9497 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/LICENSE
+-rw-r--r--   0        0        0     8547 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/README.md
+-rw-r--r--   0        0        0     1816 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0    12222 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      623 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0      134 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/const.py
+-rw-r--r--   0        0        0     5556 2023-06-04 17:16:30.714776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0    11669 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2928 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0     2279 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/msg_cache.py
+-rw-r--r--   0        0        0   212591 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0     3007 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      851 2023-06-04 17:16:30.718776 nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      690 2023-06-04 17:16:47.143058 nonebot_plugin_multincm-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     9199 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.5/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.3.4/LICENSE` & `nonebot_plugin_multincm-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/README.md` & `nonebot_plugin_multincm-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/lrc_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/msg_cache.py` & `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/msg_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.3.5/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.4/pyproject.toml` & `nonebot_plugin_multincm-0.3.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.3.4"
+version = "0.3.5"
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
-    "nonebot2>=2.0.0-rc.1",
+    "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.2.0",
     "pydantic>=1.10.4",
     "pil-utils>=0.1.7",
     "pyncm>=1.6.8.9.1",
     "typing-extensions>=4.5.0",
     "anyio>=3.6.2",
     "nonebot-plugin-apscheduler>=0.2.0",
@@ -20,24 +20,14 @@
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-multincm"
 
-[project.optional-dependencies]
-dev = [
-    "pip>=23.0.1",
-    "setuptools>=67.6.1",
-    "nb-cli>=1.0.5",
-    "black>=23.3.0",
-    "ruff>=0.0.260",
-    "isort>=5.12.0",
-]
-
 [tool.pdm.build]
 includes = []
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `nonebot_plugin_multincm-0.3.4/PKG-INFO` & `nonebot_plugin_multincm-0.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.3.4
+Version: 0.3.5
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
-Requires-Dist: nonebot2>=2.0.0-rc.1
+Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.2.0
 Requires-Dist: pydantic>=1.10.4
 Requires-Dist: pil-utils>=0.1.7
 Requires-Dist: pyncm>=1.6.8.9.1
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: anyio>=3.6.2
 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0
-Requires-Dist: pip>=23.0.1; extra == "dev"
-Requires-Dist: setuptools>=67.6.1; extra == "dev"
-Requires-Dist: nb-cli>=1.0.5; extra == "dev"
-Requires-Dist: black>=23.3.0; extra == "dev"
-Requires-Dist: ruff>=0.0.260; extra == "dev"
-Requires-Dist: isort>=5.12.0; extra == "dev"
-Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
```

#### html2text {}

```diff
@@ -1,21 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.4 Summary: NCM
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.5 Summary: NCM
 Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
-nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
-Dist: pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
+nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-Dist:
+pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
-anyio>=3.6.2 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0 Requires-Dist:
-pip>=23.0.1; extra == "dev" Requires-Dist: setuptools>=67.6.1; extra == "dev"
-Requires-Dist: nb-cli>=1.0.5; extra == "dev" Requires-Dist: black>=23.3.0;
-extra == "dev" Requires-Dist: ruff>=0.0.260; extra == "dev" Requires-Dist:
-isort>=5.12.0; extra == "dev" Provides-Extra: dev Description-Content-Type:
-text/markdown
+anyio>=3.6.2 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0 Description-
+Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
    # NoneBot-Plugin-MultiNCM _â¨ ç½æäºå¤éç¹æ­ â¨_ [python] [pdm-
                              managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç»
 ä¸ä¸ªç½æäºå¤éç¹æ­æä»¶ï¼å¯ä»¥ç¿»é¡µï¼å¯ä»¥ç»å½ç½æäºè´¦å·ç¹
```

