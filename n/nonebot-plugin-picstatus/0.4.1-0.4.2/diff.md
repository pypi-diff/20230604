# Comparing `tmp/nonebot_plugin_picstatus-0.4.1.tar.gz` & `tmp/nonebot_plugin_picstatus-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_picstatus-0.4.1.tar", last modified: Thu Jun  1 06:04:20 2023, max compression
+gzip compressed data, was "nonebot_plugin_picstatus-0.4.2.tar", last modified: Sun Jun  4 16:33:22 2023, max compression
```

## Comparing `nonebot_plugin_picstatus-0.4.1.tar` & `nonebot_plugin_picstatus-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-06-01 06:04:09.033235 nonebot_plugin_picstatus-0.4.1/LICENSE
--rw-r--r--   0        0        0     6736 2023-06-01 06:04:09.033235 nonebot_plugin_picstatus-0.4.1/README.md
--rw-r--r--   0        0        0      697 2023-06-01 06:04:09.033235 nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/__init__.py
--rw-r--r--   0        0        0     3502 2023-06-01 06:04:09.033235 nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/__main__.py
--rw-r--r--   0        0        0     1212 2023-06-01 06:04:09.033235 nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/config.py
--rw-r--r--   0        0        0      251 2023-06-01 06:04:09.033235 nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/const.py
--rw-r--r--   0        0        0    18979 2023-06-01 06:04:09.033235 nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/draw.py
--rw-r--r--   0        0        0   378600 2023-06-01 06:04:09.033235 nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/res/default_avatar.png
--rw-r--r--   0        0        0  1527158 2023-06-01 06:04:09.045235 nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/res/default_bg.png
--rw-r--r--   0        0        0     1385 2023-06-01 06:04:09.045235 nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/statistics.py
--rw-r--r--   0        0        0     4665 2023-06-01 06:04:09.045235 nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/util.py
--rw-r--r--   0        0        0       22 2023-06-01 06:04:09.045235 nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/version.py
--rw-r--r--   0        0        0      765 2023-06-01 06:04:20.605406 nonebot_plugin_picstatus-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7418 1970-01-01 00:00:00.000000 nonebot_plugin_picstatus-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/LICENSE
+-rw-r--r--   0        0        0     6857 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/README.md
+-rw-r--r--   0        0        0      932 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/__init__.py
+-rw-r--r--   0        0        0     3502 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/__main__.py
+-rw-r--r--   0        0        0     1251 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/config.py
+-rw-r--r--   0        0        0      251 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/const.py
+-rw-r--r--   0        0        0    18979 2023-06-04 16:33:05.983925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/draw.py
+-rw-r--r--   0        0        0   378600 2023-06-04 16:33:05.987925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/res/default_avatar.png
+-rw-r--r--   0        0        0  1527158 2023-06-04 16:33:05.999925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/res/default_bg.png
+-rw-r--r--   0        0        0     1385 2023-06-04 16:33:05.999925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/statistics.py
+-rw-r--r--   0        0        0     4727 2023-06-04 16:33:05.999925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/util.py
+-rw-r--r--   0        0        0       22 2023-06-04 16:33:05.999925 nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/version.py
+-rw-r--r--   0        0        0      763 2023-06-04 16:33:22.424657 nonebot_plugin_picstatus-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7537 1970-01-01 00:00:00.000000 nonebot_plugin_picstatus-0.4.2/PKG-INFO
```

### Comparing `nonebot_plugin_picstatus-0.4.1/LICENSE` & `nonebot_plugin_picstatus-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.4.1/README.md` & `nonebot_plugin_picstatus-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -139,14 +139,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.4.2
+
+- 添加配置项 `PS_REQ_TIMEOUT` ([#25](https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus/issues/25))
+
 ### 0.4.1
 
 - 现在默认使用 `pil_utils` 自动选择系统内支持中文的字体，删除插件内置字体
 - 使用 `pil_utils` 写 Bot 昵称，可以显示 Emoji 等特殊字符
 - 测试网站出错时不会往日志里甩错误堆栈了
 
 ### 0.4.0
```

#### html2text {}

```diff
@@ -26,16 +26,17 @@
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [ææ¢¦ API](https://api.gumengya.com) -
 éæºèæ¯å¾æ¥æº ### [LoliApi](https://docs.loliapi.com/) -
 éæºèæ¯å¾æ¥æºï¼ææ¶å¼ç¨ï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.4.1 - ç°å¨é»è®¤ä½¿ç¨
-`pil_utils`
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.4.2 - æ·»å éç½®é¡¹
+`PS_REQ_TIMEOUT` ([#25](https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus/
+issues/25)) ### 0.4.1 - ç°å¨é»è®¤ä½¿ç¨ `pil_utils`
 èªå¨éæ©ç³»ç»åæ¯æä¸­æçå­ä½ï¼å é¤æä»¶åç½®å­ä½ - ä½¿ç¨
 `pil_utils` å Bot æµç§°ï¼å¯ä»¥æ¾ç¤º Emoji ç­ç¹æ®å­ç¬¦ -
 æµè¯ç½ç«åºéæ¶ä¸ä¼å¾æ¥å¿éç©éè¯¯å æ äº ### 0.4.0 - ä½¿ç¨
 [nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-
 plugin-send-anything-anywhere) å¼å®¹å¤å¹³å°åéï¼å¹¶å¯¹ OneBot V11 å
 Telegram åäºç¹æ®å¼å®¹ - å°ç¶æå¾çä¿å­ä¸º `jpg`
 æ ¼å¼ï¼ç¼©åä½ç§¯ - æµè¯ç½ç«ç°å¨æç§éç½®æä»¶ä¸­çé¡ºåºæåº
```

### Comparing `nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/__init__.py` & `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,9 +14,18 @@
 if config.ps_only_su:
     usage += "\n注意：仅SuperUser可以使用此指令"
 
 __plugin_meta__ = PluginMetadata(
     name="PicStatus",
     description="以图片形式显示当前设备的运行状态",
     usage=usage,
+    type="application",
+    homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus",
     config=Cfg,
+    supported_adapters=[
+        "~onebot.v11",
+        "~onebot.v12",
+        "~telegram",
+        "~kaiheila",
+        "~qqguild",
+    ],
 )
```

### Comparing `nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/__main__.py` & `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/config.py` & `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,10 +33,11 @@
     ps_footer_size: int = 22
     ps_test_sites: List[TestSiteCfg] = [
         TestSiteCfg(name="百度", url="https://baidu.com"),
         TestSiteCfg(name="Google", url="https://google.com", use_proxy=True),
     ]
     ps_test_timeout: int = 5
     ps_max_text_len: int = 18
+    ps_req_timeout: Optional[int] = 10
 
 
 config: Cfg = Cfg.parse_obj(get_driver().config.dict())
```

### Comparing `nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/draw.py` & `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/res/default_avatar.png` & `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/res/default_avatar.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/res/default_bg.png` & `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/res/default_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/statistics.py` & `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/statistics.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_picstatus-0.4.1/nonebot_plugin_picstatus/util.py` & `nonebot_plugin_picstatus-0.4.2/nonebot_plugin_picstatus/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,19 @@
     proxy: Optional[str] = None,
     **kwargs,
 ) -> str:
     ...
 
 
 async def async_request(url: str, *args, is_text=False, proxy=None, **kwargs):
-    async with AsyncClient(proxies=proxy, follow_redirects=True) as cli:
+    async with AsyncClient(
+        proxies=proxy,
+        follow_redirects=True,
+        timeout=config.ps_req_timeout,
+    ) as cli:
         res = await cli.get(url, *args, **kwargs)
         return res.text if is_text else res.content
 
 
 async def get_anime_pic():
     data = json.loads(
         await async_request("https://api.gumengya.com/Api/DmImg", is_text=True),
```

### Comparing `nonebot_plugin_picstatus-0.4.1/pyproject.toml` & `nonebot_plugin_picstatus-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "nonebot-plugin-picstatus"
-version = "0.4.1"
+version = "0.4.2"
 description = "A NoneBot2 plugin generates a picture which shows the status of current device"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "Pillow<10.0.0,>=9.2.0",
     "psutil<6.0.0,>=5.9.2",
-    "nonebot2>=2.0.0b4",
+    "nonebot2>=2.0.0",
     "nonebot-plugin-send-anything-anywhere>=0.2.4",
     "anyio>=3.7.0",
     "httpx>=0.24.1",
     "pil-utils>=0.1.7",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
```

### Comparing `nonebot_plugin_picstatus-0.4.1/PKG-INFO` & `nonebot_plugin_picstatus-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-picstatus
-Version: 0.4.1
+Version: 0.4.2
 Summary: A NoneBot2 plugin generates a picture which shows the status of current device
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus
 Requires-Python: <4.0,>=3.8
 Requires-Dist: Pillow<10.0.0,>=9.2.0
 Requires-Dist: psutil<6.0.0,>=5.9.2
-Requires-Dist: nonebot2>=2.0.0b4
+Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
 Requires-Dist: anyio>=3.7.0
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: pil-utils>=0.1.7
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
@@ -157,14 +157,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.4.2
+
+- 添加配置项 `PS_REQ_TIMEOUT` ([#25](https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus/issues/25))
+
 ### 0.4.1
 
 - 现在默认使用 `pil_utils` 自动选择系统内支持中文的字体，删除插件内置字体
 - 使用 `pil_utils` 写 Bot 昵称，可以显示 Emoji 等特殊字符
 - 测试网站出错时不会往日志里甩错误堆栈了
 
 ### 0.4.0
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-picstatus Version: 0.4.1 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-picstatus Version: 0.4.2 Summary: A
 NoneBot2 plugin generates a picture which shows the status of current device
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus Author-Email:
 student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-picstatus Requires-Python: <4.0,>=3.8 Requires-Dist:
 Pillow<10.0.0,>=9.2.0 Requires-Dist: psutil<6.0.0,>=5.9.2 Requires-Dist:
-nonebot2>=2.0.0b4 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
+nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
 Requires-Dist: anyio>=3.7.0 Requires-Dist: httpx>=0.24.1 Requires-Dist: pil-
 utils>=0.1.7 Description-Content-Type: text/markdown
                                     [logo]
                                     [logo]
    # NoneBot-Plugin-PicStatus _â¨ è¿è¡ç¶æå¾çç for NoneBot2 â¨_
              [license] [pypi] [python] [pypi_download] [wakatime]
 ## ð ä»ç» ä¸å¤è¯´ï¼ç´æ¥çå¾ï¼ ### ææå¾  ç¹å»å±å¼ !
@@ -36,16 +36,17 @@
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [ææ¢¦ API](https://api.gumengya.com) -
 éæºèæ¯å¾æ¥æº ### [LoliApi](https://docs.loliapi.com/) -
 éæºèæ¯å¾æ¥æºï¼ææ¶å¼ç¨ï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.4.1 - ç°å¨é»è®¤ä½¿ç¨
-`pil_utils`
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.4.2 - æ·»å éç½®é¡¹
+`PS_REQ_TIMEOUT` ([#25](https://github.com/lgc-NB2Dev/nonebot-plugin-picstatus/
+issues/25)) ### 0.4.1 - ç°å¨é»è®¤ä½¿ç¨ `pil_utils`
 èªå¨éæ©ç³»ç»åæ¯æä¸­æçå­ä½ï¼å é¤æä»¶åç½®å­ä½ - ä½¿ç¨
 `pil_utils` å Bot æµç§°ï¼å¯ä»¥æ¾ç¤º Emoji ç­ç¹æ®å­ç¬¦ -
 æµè¯ç½ç«åºéæ¶ä¸ä¼å¾æ¥å¿éç©éè¯¯å æ äº ### 0.4.0 - ä½¿ç¨
 [nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-
 plugin-send-anything-anywhere) å¼å®¹å¤å¹³å°åéï¼å¹¶å¯¹ OneBot V11 å
 Telegram åäºç¹æ®å¼å®¹ - å°ç¶æå¾çä¿å­ä¸º `jpg`
 æ ¼å¼ï¼ç¼©åä½ç§¯ - æµè¯ç½ç«ç°å¨æç§éç½®æä»¶ä¸­çé¡ºåºæåº
```

