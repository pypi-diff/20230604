# Comparing `tmp/nonebot-plugin-picmcstat-0.3.1.tar.gz` & `tmp/nonebot_plugin_picmcstat-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-picmcstat-0.3.1.tar", last modified: Sat May 13 15:29:43 2023, max compression
+gzip compressed data, was "nonebot_plugin_picmcstat-0.3.2.tar", last modified: Sun Jun  4 17:17:16 2023, max compression
```

## Comparing `nonebot-plugin-picmcstat-0.3.1.tar` & `nonebot_plugin_picmcstat-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/LICENSE
--rw-r--r--   0        0        0     5998 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/README.md
--rw-r--r--   0        0        0      295 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/__init__.py
--rw-r--r--   0        0        0     1572 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/__main__.py
--rw-r--r--   0        0        0      452 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/config.py
--rw-r--r--   0        0        0     1480 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/const.py
--rw-r--r--   0        0        0     7748 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/draw.py
--rw-r--r--   0        0        0    12656 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/res/default.png
--rw-r--r--   0        0        0      335 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/res/dirt.png
--rw-r--r--   0        0        0      556 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/res/grass_side_carried.png
--rw-r--r--   0        0        0      399 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/res.py
--rw-r--r--   0        0        0     4078 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/util.py
--rw-r--r--   0        0        0     1194 2023-05-13 15:29:31.177832 nonebot-plugin-picmcstat-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6288 1970-01-01 00:00:00.000000 nonebot-plugin-picmcstat-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5998 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/README.md
+-rw-r--r--   0        0        0      541 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/__init__.py
+-rw-r--r--   0        0        0     1572 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/__main__.py
+-rw-r--r--   0        0        0      452 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/config.py
+-rw-r--r--   0        0        0     1480 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/const.py
+-rw-r--r--   0        0        0     7748 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/draw.py
+-rw-r--r--   0        0        0      399 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res.py
+-rw-r--r--   0        0        0    12656 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res/default.png
+-rw-r--r--   0        0        0      335 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res/dirt.png
+-rw-r--r--   0        0        0      556 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res/grass_side_carried.png
+-rw-r--r--   0        0        0     4078 2023-06-04 17:17:04.182698 nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/util.py
+-rw-r--r--   0        0        0      675 2023-06-04 17:17:16.354115 nonebot_plugin_picmcstat-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6612 1970-01-01 00:00:00.000000 nonebot_plugin_picmcstat-0.3.2/PKG-INFO
```

### Comparing `nonebot-plugin-picmcstat-0.3.1/LICENSE` & `nonebot_plugin_picmcstat-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-picmcstat-0.3.1/README.md` & `nonebot_plugin_picmcstat-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/__main__.py` & `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/const.py` & `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/const.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/draw.py` & `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/res/default.png` & `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res/default.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/res/grass_side_carried.png` & `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/res/grass_side_carried.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-picmcstat-0.3.1/nonebot_plugin_picmcstat/util.py` & `nonebot_plugin_picmcstat-0.3.2/nonebot_plugin_picmcstat/util.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-picmcstat-0.3.1/PKG-INFO` & `nonebot_plugin_picmcstat-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-picmcstat
-Version: 0.3.1
+Version: 0.3.2
 Summary: A NoneBot2 plugin generates a pic from a Minecraft server's MOTD
+Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-picmcstat
+Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
-Author-email: student_2333 <lgc2333@126.com>
-Requires-Python: >=3.8,<4.0
-Provides-Extra: dev
+Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-picmcstat
+Requires-Python: <4.0,>=3.8
+Requires-Dist: mcstatus<11.0.0,>=10.0.1
+Requires-Dist: nonebot2<3.0.0,>=2.0.0
+Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.0
+Requires-Dist: pydantic<2.0.0,>=1.10.4
+Requires-Dist: pil-utils>=0.1.6
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/picmcstat/picmcstat.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
@@ -226,8 +232,7 @@
 - 加入快捷指令，详见配置项
 - 修复某些 JE 服无法正确显示 Motd 的问题
 -
 
 ### 0.1.1
 
 - 将查 JE 服时的 `游戏延迟` 字样 改为 `测试延迟`
-
```

#### html2text {}

```diff
@@ -1,12 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-picmcstat Version: 0.3.1 Summary: A
-NoneBot2 plugin generates a pic from a Minecraft server's MOTD License: MIT
-Author-email: student_2333
-126.com> Requires-Python: >=3.8,<4.0 Provides-Extra: dev Description-Content-
-Type: text/markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-picmcstat Version: 0.3.2 Summary: A
+NoneBot2 plugin generates a pic from a Minecraft server's MOTD Home-page:
+https://github.com/lgc-NB2Dev/nonebot-plugin-picmcstat Author-Email:
+student_2333
+126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
+nonebot-plugin-picmcstat Requires-Python: <4.0,>=3.8 Requires-Dist:
+mcstatus<11.0.0,>=10.0.1 Requires-Dist: nonebot2<3.0.0,>=2.0.0 Requires-Dist:
+nonebot-adapter-onebot<3.0.0,>=2.2.0 Requires-Dist: pydantic<2.0.0,>=1.10.4
+Requires-Dist: pil-utils>=0.1.6 Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # NoneBot-Plugin-PicMCStat _â¨ Minecraft æå¡å¨ MOTD æ¥è¯¢ å¾çç â¨_
              [license] [pypi] [python] [pypi_download] [wakatime]
 ## ð ä»ç» æä»¶å®éä¸æ¯å¯ä»¥å±ç¤º **ç©å®¶åè¡¨**ã**Mod
 ç«¯ä¿¡æ¯ ä»¥å Mod åè¡¨ï¼è¿æªæµè¯ï¼**
 çï¼è¿éæ²¡ææ¾å°åéçä¾å­æä»¥æ²¡å¨ææå¾éå±ç¤ºåºæ¥ï¼å¦æéå°é®é¢å¯ä»¥å
```

