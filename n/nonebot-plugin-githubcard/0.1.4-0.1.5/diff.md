# Comparing `tmp/nonebot_plugin_githubcard-0.1.4.tar.gz` & `tmp/nonebot_plugin_githubcard-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_githubcard-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_githubcard-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_githubcard-0.1.4.tar` & `nonebot_plugin_githubcard-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-03-16 13:13:09.152445 nonebot_plugin_githubcard-0.1.4/LICENSE
--rw-r--r--   0        0        0      717 2023-05-22 04:13:54.015382 nonebot_plugin_githubcard-0.1.4/nonebot_plugin_githubcard/__init__.py
--rw-r--r--   0        0        0      272 2023-05-22 10:35:39.369190 nonebot_plugin_githubcard-0.1.4/nonebot_plugin_githubcard/config.py
--rw-r--r--   0        0        0     1335 2023-05-22 11:01:06.788568 nonebot_plugin_githubcard-0.1.4/nonebot_plugin_githubcard/data_source.py
--rw-r--r--   0        0        0      693 2023-05-22 10:35:34.586215 nonebot_plugin_githubcard-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1712 2023-05-22 10:36:44.967843 nonebot_plugin_githubcard-0.1.4/README.md
--rw-r--r--   0        0        0     2638 1970-01-01 00:00:00.000000 nonebot_plugin_githubcard-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-16 13:13:09.152445 nonebot_plugin_githubcard-0.1.5/LICENSE
+-rw-r--r--   0        0        0      997 2023-06-04 08:51:57.520655 nonebot_plugin_githubcard-0.1.5/nonebot_plugin_githubcard/__init__.py
+-rw-r--r--   0        0        0      272 2023-05-22 10:35:39.369190 nonebot_plugin_githubcard-0.1.5/nonebot_plugin_githubcard/config.py
+-rw-r--r--   0        0        0     1335 2023-05-22 11:01:06.788568 nonebot_plugin_githubcard-0.1.5/nonebot_plugin_githubcard/data_source.py
+-rw-r--r--   0        0        0      693 2023-06-04 08:52:31.906193 nonebot_plugin_githubcard-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1712 2023-05-22 10:36:44.967843 nonebot_plugin_githubcard-0.1.5/README.md
+-rw-r--r--   0        0        0     2638 1970-01-01 00:00:00.000000 nonebot_plugin_githubcard-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_githubcard-0.1.4/LICENSE` & `nonebot_plugin_githubcard-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.4/nonebot_plugin_githubcard/__init__.py` & `nonebot_plugin_githubcard-0.1.5/nonebot_plugin_githubcard/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 from nonebot.rule import T_State
 from nonebot import get_driver
+from nonebot.log import logger
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageSegment
 from .config import Config
 from .data_source import get_github_reposity_information
 from nonebot.plugin import on_regex
 
+import re
+
 global_config = get_driver().config
 config = Config(**global_config.dict())
-github = on_regex(r"github.com\/(.+)?\/([^\/\s]+)", priority=10, block=False)
+github = on_regex(r"https?://github\.com/([^/]+/[^/]+)", priority=10, block=False)
 
+def match_link_parts(link):
+    pattern = r'https?://github\.com/([^/]+/[^/]+)'
+    match = re.search(pattern, link)
+    if match:
+        return match.group(0)
+    else:
+        return None
+    
 @github.handle()
 async def github_handle(bot: Bot, event: GroupMessageEvent, state: T_State):
-    url = event.get_plaintext()
+    url = match_link_parts(event.get_plaintext())
     imageUrl = await get_github_reposity_information(url)
     assert(imageUrl != "获取信息失败")
-    await github.send(MessageSegment.image(imageUrl))
+    await github.send(MessageSegment.image(imageUrl))
+
```

### Comparing `nonebot_plugin_githubcard-0.1.4/nonebot_plugin_githubcard/data_source.py` & `nonebot_plugin_githubcard-0.1.5/nonebot_plugin_githubcard/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.4/pyproject.toml` & `nonebot_plugin_githubcard-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-githubcard"
-version = "0.1.4"
+version = "0.1.5"
 description = "检测GitHub仓库链接并自动发送卡片信息（适用于Onebot V11）"
 authors = ["ElainaFanBoy <demo0929@vip.qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ElainaFanBoy/nonebot_plugin_githubcard"
 repository = "https://github.com/ElainaFanBoy/nonebot_plugin_githubcard"
```

### Comparing `nonebot_plugin_githubcard-0.1.4/README.md` & `nonebot_plugin_githubcard-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.4/PKG-INFO` & `nonebot_plugin_githubcard-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-githubcard
-Version: 0.1.4
+Version: 0.1.5
 Summary: 检测GitHub仓库链接并自动发送卡片信息（适用于Onebot V11）
 Home-page: https://github.com/ElainaFanBoy/nonebot_plugin_githubcard
 License: MIT
 Author: ElainaFanBoy
 Author-email: demo0929@vip.qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-githubcard Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-githubcard Version: 0.1.5 Summary:
 æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºOnebot V11ï¼
 Home-page: https://github.com/ElainaFanBoy/nonebot_plugin_githubcard License:
 MIT Author: ElainaFanBoy Author-email: demo0929@vip.qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

