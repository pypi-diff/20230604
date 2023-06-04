# Comparing `tmp/nonebot_plugin_callapi-0.1.1.tar.gz` & `tmp/nonebot_plugin_callapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_callapi-0.1.1.tar", last modified: Mon May 15 19:23:00 2023, max compression
+gzip compressed data, was "nonebot_plugin_callapi-0.1.2.tar", last modified: Sun Jun  4 17:15:57 2023, max compression
```

## Comparing `nonebot_plugin_callapi-0.1.1.tar` & `nonebot_plugin_callapi-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-05-15 19:22:49.226889 nonebot_plugin_callapi-0.1.1/LICENSE
--rw-r--r--   0        0        0     4572 2023-05-15 19:22:49.226889 nonebot_plugin_callapi-0.1.1/README.md
--rw-r--r--   0        0        0      304 2023-05-15 19:22:49.226889 nonebot_plugin_callapi-0.1.1/nonebot_plugin_callapi/__init__.py
--rw-r--r--   0        0        0     8442 2023-05-15 19:22:49.226889 nonebot_plugin_callapi-0.1.1/nonebot_plugin_callapi/__main__.py
--rw-r--r--   0        0        0      197 2023-05-15 19:22:49.226889 nonebot_plugin_callapi-0.1.1/nonebot_plugin_callapi/config.py
--rw-r--r--   0        0        0      838 2023-05-15 19:23:00.803087 nonebot_plugin_callapi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 nonebot_plugin_callapi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-04 17:15:45.382951 nonebot_plugin_callapi-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4572 2023-06-04 17:15:45.382951 nonebot_plugin_callapi-0.1.2/README.md
+-rw-r--r--   0        0        0      462 2023-06-04 17:15:45.382951 nonebot_plugin_callapi-0.1.2/nonebot_plugin_callapi/__init__.py
+-rw-r--r--   0        0        0     8442 2023-06-04 17:15:45.382951 nonebot_plugin_callapi-0.1.2/nonebot_plugin_callapi/__main__.py
+-rw-r--r--   0        0        0      197 2023-06-04 17:15:45.382951 nonebot_plugin_callapi-0.1.2/nonebot_plugin_callapi/config.py
+-rw-r--r--   0        0        0      661 2023-06-04 17:15:57.382979 nonebot_plugin_callapi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5178 1970-01-01 00:00:00.000000 nonebot_plugin_callapi-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_callapi-0.1.1/LICENSE` & `nonebot_plugin_callapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_callapi-0.1.1/README.md` & `nonebot_plugin_callapi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_callapi-0.1.1/nonebot_plugin_callapi/__main__.py` & `nonebot_plugin_callapi-0.1.2/nonebot_plugin_callapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_callapi-0.1.1/pyproject.toml` & `nonebot_plugin_callapi-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "nonebot-plugin-callapi"
-version = "0.1.1"
+version = "0.1.2"
 description = "Use bot command to call its API"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
-    "nonebot2>=2.0.0-rc.1",
+    "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.2.0",
     "pydantic>=1.10.4",
     "Pygments>=2.15.1",
     "pil-utils>=0.1.7",
     "nonebot-plugin-send-anything-anywhere>=0.2.4",
 ]
 requires-python = ">=3.8,<4.0"
@@ -18,24 +18,14 @@
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-callapi"
 
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

### Comparing `nonebot_plugin_callapi-0.1.1/PKG-INFO` & `nonebot_plugin_callapi-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-callapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Use bot command to call its API
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-callapi
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-callapi
 Requires-Python: <4.0,>=3.8
-Requires-Dist: nonebot2>=2.0.0-rc.1
+Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.2.0
 Requires-Dist: pydantic>=1.10.4
 Requires-Dist: Pygments>=2.15.1
 Requires-Dist: pil-utils>=0.1.7
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
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
@@ -1,20 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-callapi Version: 0.1.1 Summary: Use
+Metadata-Version: 2.1 Name: nonebot-plugin-callapi Version: 0.1.2 Summary: Use
 bot command to call its API Home-page: https://github.com/lgc-NB2Dev/nonebot-
 plugin-callapi Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-callapi Requires-Python: <4.0,>=3.8 Requires-Dist:
-nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
-Dist: pydantic>=1.10.4 Requires-Dist: Pygments>=2.15.1 Requires-Dist: pil-
+nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-Dist:
+pydantic>=1.10.4 Requires-Dist: Pygments>=2.15.1 Requires-Dist: pil-
 utils>=0.1.7 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
-Requires-Dist: pip>=23.0.1; extra == "dev" Requires-Dist: setuptools>=67.6.1;
-extra == "dev" Requires-Dist: nb-cli>=1.0.5; extra == "dev" Requires-Dist:
-black>=23.3.0; extra == "dev" Requires-Dist: ruff>=0.0.260; extra == "dev"
-Requires-Dist: isort>=5.12.0; extra == "dev" Provides-Extra: dev Description-
-Content-Type: text/markdown
+Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # NoneBot-Plugin-CallAPI _â¨ ä½¿ç¨æä»¤æ¥è°ç¨ Bot ç API â¨_ [python]
                            [pdm-managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç» ä½¿ç¨ Bot æä»¤æ¥ç´æ¥è°ç¨ Bot ç API å§ï¼
 æ¬æä»¶çè®ºä¸å¼å®¹ä»»ä½ééå¨~ ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³
```

