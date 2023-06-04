# Comparing `tmp/nonebot-plugin-fuckyou-0.1.3.tar.gz` & `tmp/nonebot-plugin-fuckyou-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-fuckyou-0.1.3.tar", last modified: Sat Apr 29 16:04:32 2023, max compression
+gzip compressed data, was "nonebot-plugin-fuckyou-0.1.4.tar", last modified: Sun Jun  4 17:16:25 2023, max compression
```

## Comparing `nonebot-plugin-fuckyou-0.1.3.tar` & `nonebot-plugin-fuckyou-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-04-29 16:04:18.239304 nonebot-plugin-fuckyou-0.1.3/LICENSE
--rw-r--r--   0        0        0     4503 2023-04-29 16:04:18.239304 nonebot-plugin-fuckyou-0.1.3/README.md
--rw-r--r--   0        0        0      318 2023-04-29 16:04:18.239304 nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/__init__.py
--rw-r--r--   0        0        0     1851 2023-04-29 16:04:18.239304 nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/__main__.py
--rw-r--r--   0        0        0      439 2023-04-29 16:04:18.239304 nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/config.py
--rw-r--r--   0        0        0   221958 2023-04-29 16:04:18.243305 nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/const.py
--rw-r--r--   0        0        0     1121 2023-04-29 16:04:18.243305 nonebot-plugin-fuckyou-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 nonebot-plugin-fuckyou-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-04 17:16:07.308670 nonebot-plugin-fuckyou-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4641 2023-06-04 17:16:07.308670 nonebot-plugin-fuckyou-0.1.4/README.md
+-rw-r--r--   0        0        0      476 2023-06-04 17:16:07.308670 nonebot-plugin-fuckyou-0.1.4/nonebot_plugin_fuckyou/__init__.py
+-rw-r--r--   0        0        0     1851 2023-06-04 17:16:07.308670 nonebot-plugin-fuckyou-0.1.4/nonebot_plugin_fuckyou/__main__.py
+-rw-r--r--   0        0        0      439 2023-06-04 17:16:07.308670 nonebot-plugin-fuckyou-0.1.4/nonebot_plugin_fuckyou/config.py
+-rw-r--r--   0        0        0   221958 2023-06-04 17:16:07.308670 nonebot-plugin-fuckyou-0.1.4/nonebot_plugin_fuckyou/const.py
+-rw-r--r--   0        0        0      541 2023-06-04 17:16:07.308670 nonebot-plugin-fuckyou-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 nonebot-plugin-fuckyou-0.1.4/PKG-INFO
```

### Comparing `nonebot-plugin-fuckyou-0.1.3/LICENSE` & `nonebot-plugin-fuckyou-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fuckyou-0.1.3/README.md` & `nonebot-plugin-fuckyou-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-fuckyou
+Version: 0.1.4
+Summary: A NoneBot2 plugin designed for curse users
+License: MIT
+Author-email: student_2333 <lgc2333@126.com>
+Requires-Python: >=3.8,<4.0
+Project-URL: homepage, https://github.com/lgc2333/nonebot-plugin-fuckyou
+Description-Content-Type: text/markdown
+
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
   <img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/fuckyou/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
@@ -34,14 +44,16 @@
 
 _10 分钟紧急开发的插件（误_
 
 NoneBot2 骂人插件，攻击性极强
 
 插件词库来源：[xiaoye12123/js](https://gitee.com/xiaoye12123/js)
 
+有更多自定义配置项的 Fork: [Dogend233/nonebot-plugin-fuckyou-reset](https://github.com/Dogend233/nonebot-plugin-fuckyou-reset)
+
 ## 💿 安装
 
 以下提到的方法 任选**其一** 即可
 
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
@@ -155,7 +167,8 @@
 ### 0.1.2
 
 - 添加一个配置项
 
 ### 0.1.1
 
 - 添加几个配置项
+
```

#### html2text {}

```diff
@@ -1,15 +1,22 @@
+Metadata-Version: 2.1 Name: nonebot-plugin-fuckyou Version: 0.1.4 Summary: A
+NoneBot2 plugin designed for curse users License: MIT Author-email:
+student_2333
+126.com> Requires-Python: >=3.8,<4.0 Project-URL: homepage, https://github.com/
+lgc2333/nonebot-plugin-fuckyou Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # NoneBot-Plugin-FuckYou _ð ä½ æå ä¸ª ð´ï¼è¿ä¹çï¼ ð_ [license]
                   [pypi] [python] [pypi_download] [wakatime]
 ## ð ä»ç» _10 åéç´§æ¥å¼åçæä»¶ï¼è¯¯_ NoneBot2
 éªäººæä»¶ï¼æ»å»æ§æå¼º æä»¶è¯åºæ¥æºï¼[xiaoye12123/js](https://
-gitee.com/xiaoye12123/js) ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸**
-å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+gitee.com/xiaoye12123/js) ææ´å¤èªå®ä¹éç½®é¡¹ç Fork: [Dogend233/
+nonebot-plugin-fuckyou-reset](https://github.com/Dogend233/nonebot-plugin-
+fuckyou-reset) ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯
+[æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
 plugin install nonebot-plugin-fuckyou ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
 install nonebot-plugin-fuckyou ```   pdm ```bash pdm add nonebot-plugin-fuckyou
 ```   poetry ```bash poetry add nonebot-plugin-fuckyou ```   conda ```bash
 conda install nonebot-plugin-fuckyou ```  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
```

### Comparing `nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/__main__.py` & `nonebot-plugin-fuckyou-0.1.4/nonebot_plugin_fuckyou/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fuckyou-0.1.3/nonebot_plugin_fuckyou/const.py` & `nonebot-plugin-fuckyou-0.1.4/nonebot_plugin_fuckyou/const.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fuckyou-0.1.3/PKG-INFO` & `nonebot-plugin-fuckyou-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-fuckyou
-Version: 0.1.3
-Summary: A NoneBot2 plugin designed for curse users
-License: MIT
-Author-email: student_2333 <lgc2333@126.com>
-Requires-Python: >=3.8,<4.0
-Provides-Extra: dev
-Project-URL: homepage, https://github.com/lgc2333/nonebot-plugin-fuckyou
-Description-Content-Type: text/markdown
-
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
   <img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/fuckyou/logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
@@ -45,14 +34,16 @@
 
 _10 分钟紧急开发的插件（误_
 
 NoneBot2 骂人插件，攻击性极强
 
 插件词库来源：[xiaoye12123/js](https://gitee.com/xiaoye12123/js)
 
+有更多自定义配置项的 Fork: [Dogend233/nonebot-plugin-fuckyou-reset](https://github.com/Dogend233/nonebot-plugin-fuckyou-reset)
+
 ## 💿 安装
 
 以下提到的方法 任选**其一** 即可
 
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
@@ -166,8 +157,7 @@
 ### 0.1.2
 
 - 添加一个配置项
 
 ### 0.1.1
 
 - 添加几个配置项
-
```

#### html2text {}

```diff
@@ -1,21 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fuckyou Version: 0.1.3 Summary: A
-NoneBot2 plugin designed for curse users License: MIT Author-email:
-student_2333
-126.com> Requires-Python: >=3.8,<4.0 Provides-Extra: dev Project-URL: homepage,
-https://github.com/lgc2333/nonebot-plugin-fuckyou Description-Content-Type:
-text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # NoneBot-Plugin-FuckYou _ð ä½ æå ä¸ª ð´ï¼è¿ä¹çï¼ ð_ [license]
                   [pypi] [python] [pypi_download] [wakatime]
 ## ð ä»ç» _10 åéç´§æ¥å¼åçæä»¶ï¼è¯¯_ NoneBot2
 éªäººæä»¶ï¼æ»å»æ§æå¼º æä»¶è¯åºæ¥æºï¼[xiaoye12123/js](https://
-gitee.com/xiaoye12123/js) ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸**
-å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+gitee.com/xiaoye12123/js) ææ´å¤èªå®ä¹éç½®é¡¹ç Fork: [Dogend233/
+nonebot-plugin-fuckyou-reset](https://github.com/Dogend233/nonebot-plugin-
+fuckyou-reset) ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯
+[æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
 plugin install nonebot-plugin-fuckyou ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
 install nonebot-plugin-fuckyou ```   pdm ```bash pdm add nonebot-plugin-fuckyou
 ```   poetry ```bash poetry add nonebot-plugin-fuckyou ```   conda ```bash
 conda install nonebot-plugin-fuckyou ```  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
```

