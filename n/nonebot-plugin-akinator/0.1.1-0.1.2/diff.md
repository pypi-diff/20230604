# Comparing `tmp/nonebot-plugin-akinator-0.1.1.tar.gz` & `tmp/nonebot-plugin-akinator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-akinator-0.1.1.tar", last modified: Sat Apr 15 06:42:37 2023, max compression
+gzip compressed data, was "nonebot-plugin-akinator-0.1.2.tar", last modified: Sun Jun  4 17:12:12 2023, max compression
```

## Comparing `nonebot-plugin-akinator-0.1.1.tar` & `nonebot-plugin-akinator-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1069 2023-04-15 06:42:27.267887 nonebot-plugin-akinator-0.1.1/LICENSE
--rw-r--r--   0        0        0     4133 2023-04-15 06:42:27.267887 nonebot-plugin-akinator-0.1.1/README.md
--rw-r--r--   0        0        0      331 2023-04-15 06:42:27.267887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/__init__.py
--rw-r--r--   0        0        0     4396 2023-04-15 06:42:27.267887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/__main__.py
--rw-r--r--   0        0        0       39 2023-04-15 06:42:27.643886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.git
--rw-r--r--   0        0        0     1873 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      200 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1103 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      749 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1128 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1799 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.gitignore
--rw-r--r--   0        0        0      173 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.readthedocs.yml
--rw-r--r--   0        0        0     5328 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1082 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/LICENSE
--rw-r--r--   0        0        0       34 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/MANIFEST.in
--rw-r--r--   0        0        0     1994 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/README.rst
--rw-r--r--   0        0        0      380 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/akinator/__init__.py
--rw-r--r--   0        0        0    12713 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/akinator/akinator.py
--rw-r--r--   0        0        0      356 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/akinator/async_aki/__init__.py
--rw-r--r--   0        0        0    14044 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py
--rw-r--r--   0        0        0     2510 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/akinator/exceptions.py
--rw-r--r--   0        0        0     5559 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/akinator/utils.py
--rw-r--r--   0        0        0      319 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/docs/conf.py
--rw-r--r--   0        0        0    11653 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/docs/index.rst
--rw-r--r--   0        0        0        6 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/docs/requirements.txt
--rw-r--r--   0        0        0      612 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/examples/aki.py
--rw-r--r--   0        0        0      887 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/examples/async_aki.py
--rw-r--r--   0        0        0      681 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/pyproject.toml
--rw-r--r--   0        0        0       18 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/requirements.txt
--rw-r--r--   0        0        0     1496 2023-04-15 06:42:27.651886 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/setup.py
--rw-r--r--   0        0        0      302 2023-04-15 06:42:27.267887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/config.py
--rw-r--r--   0        0        0    10648 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/game.py
--rw-r--r--   0        0        0    11528 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/bg.jpg
--rw-r--r--   0        0        0    43524 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/concentration_intense.webp
--rw-r--r--   0        0        0    46462 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/confiant.webp
--rw-r--r--   0        0        0    45550 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/etonnement.webp
--rw-r--r--   0        0        0    49318 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/inspiration_forte.webp
--rw-r--r--   0        0        0    45300 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/inspiration_legere.webp
--rw-r--r--   0        0        0    50740 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/leger_decouragement.webp
--rw-r--r--   0        0        0    40432 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/mobile.webp
--rw-r--r--   0        0        0    36506 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/serein.webp
--rw-r--r--   0        0        0    45464 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/surprise.webp
--rw-r--r--   0        0        0    42668 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/tension.webp
--rw-r--r--   0        0        0    54230 2023-04-15 06:42:27.271887 nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/vrai_decouragement.webp
--rw-r--r--   0        0        0     1404 2023-04-15 06:42:27.275887 nonebot-plugin-akinator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4477 1970-01-01 00:00:00.000000 nonebot-plugin-akinator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4251 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/README.md
+-rw-r--r--   0        0        0      501 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/__init__.py
+-rw-r--r--   0        0        0     4396 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/__main__.py
+-rw-r--r--   0        0        0       39 2023-06-04 17:11:53.716845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.git
+-rw-r--r--   0        0        0     1873 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      200 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1103 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      749 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1128 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1799 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.gitignore
+-rw-r--r--   0        0        0      173 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.readthedocs.yml
+-rw-r--r--   0        0        0     5328 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1082 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/LICENSE
+-rw-r--r--   0        0        0       34 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/MANIFEST.in
+-rw-r--r--   0        0        0     1994 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/README.rst
+-rw-r--r--   0        0        0      380 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/akinator/__init__.py
+-rw-r--r--   0        0        0    12713 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/akinator/akinator.py
+-rw-r--r--   0        0        0      356 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/akinator/async_aki/__init__.py
+-rw-r--r--   0        0        0    14044 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py
+-rw-r--r--   0        0        0     2510 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/akinator/exceptions.py
+-rw-r--r--   0        0        0     5559 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/akinator/utils.py
+-rw-r--r--   0        0        0      319 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/docs/conf.py
+-rw-r--r--   0        0        0    11653 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/docs/index.rst
+-rw-r--r--   0        0        0        6 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/docs/requirements.txt
+-rw-r--r--   0        0        0      612 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/examples/aki.py
+-rw-r--r--   0        0        0      887 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/examples/async_aki.py
+-rw-r--r--   0        0        0      681 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/requirements.txt
+-rw-r--r--   0        0        0     1496 2023-06-04 17:11:53.724845 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/setup.py
+-rw-r--r--   0        0        0      302 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/config.py
+-rw-r--r--   0        0        0    10648 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/game.py
+-rw-r--r--   0        0        0    11528 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/bg.jpg
+-rw-r--r--   0        0        0    43524 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/concentration_intense.webp
+-rw-r--r--   0        0        0    46462 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/confiant.webp
+-rw-r--r--   0        0        0    45550 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/etonnement.webp
+-rw-r--r--   0        0        0    49318 2023-06-04 17:11:53.368839 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/inspiration_forte.webp
+-rw-r--r--   0        0        0    45300 2023-06-04 17:11:53.372840 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/inspiration_legere.webp
+-rw-r--r--   0        0        0    50740 2023-06-04 17:11:53.372840 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/leger_decouragement.webp
+-rw-r--r--   0        0        0    40432 2023-06-04 17:11:53.372840 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/mobile.webp
+-rw-r--r--   0        0        0    36506 2023-06-04 17:11:53.372840 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/serein.webp
+-rw-r--r--   0        0        0    45464 2023-06-04 17:11:53.372840 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/surprise.webp
+-rw-r--r--   0        0        0    42668 2023-06-04 17:11:53.372840 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/tension.webp
+-rw-r--r--   0        0        0    54230 2023-06-04 17:11:53.372840 nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/vrai_decouragement.webp
+-rw-r--r--   0        0        0      696 2023-06-04 17:11:53.372840 nonebot-plugin-akinator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4575 1970-01-01 00:00:00.000000 nonebot-plugin-akinator-0.1.2/PKG-INFO
```

### Comparing `nonebot-plugin-akinator-0.1.1/LICENSE` & `nonebot-plugin-akinator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/README.md` & `nonebot-plugin-akinator-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -114,16 +114,16 @@
 开始游戏后，直接发送你的答案即可（序号和文字均可）
 
 ### 效果图
 
 <details>
   <summary>点击展开</summary>
 
-![Alt text](readme/QQ%E5%9B%BE%E7%89%8720230415063509.png)  
-![Alt text](readme/QQ%E5%9B%BE%E7%89%8720230415063607.png)
+![Alt text](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/akinator/QQ%E5%9B%BE%E7%89%8720230415063509.png)  
+![Alt text](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/akinator/QQ%E5%9B%BE%E7%89%8720230415063607.png)
 
 </details>
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)
```

#### html2text {}

```diff
@@ -18,16 +18,17 @@
 é»è®¤å¼ | è¯´æ | | :-------------------: | :--: | :-----: | :--------------
 --------------------------------------: | | `PROXY` | å¦ | æ  | è®¿é®
 Akinator ä½¿ç¨çä»£ç | | `AKINATOR_CHILD_MODE` | å¦ | `False` |
 æ¯å¦å¯ç¨ Akinator çå¿ç«¥æ¨¡å¼ï¼ç»æä¸ä¼åºç° NSFW äººç©ï¼ | |
 `AKINATOR_LANGUAGE` | å¦ | `cn` | Akinator çè¯­è¨ | ## ð ä½¿ç¨
 åéæä»¤ `akinator` / `aki` å³å¯å¼å§æ¸¸æ
 å¼å§æ¸¸æåï¼ç´æ¥åéä½ çç­æ¡å³å¯ï¼åºå·åæå­åå¯ï¼ ###
-ææå¾  ç¹å»å±å¼ ![Alt text](readme/
-QQ%E5%9B%BE%E7%89%8720230415063509.png) ![Alt text](readme/
+ææå¾  ç¹å»å±å¼ ![Alt text](https://raw.githubusercontent.com/lgc-
+NB2Dev/readme/main/akinator/QQ%E5%9B%BE%E7%89%8720230415063509.png) ![Alt text]
+(https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/akinator/
 QQ%E5%9B%BE%E7%89%8720230415063607.png)  ## ð èç³» QQï¼3076823485
 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [Infiniticity/akinator.py](https://github.com/
 Infiniticity/akinator.py) - Akinator API çå°è£ ### [MeetWq/pil-utils]
 (https://github.com/MeetWq/pil-utils/) - Pillow å·¥å·åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
```

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/__main__.py` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/.gitignore` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/LICENSE` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/README.rst` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/README.rst`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/akinator/akinator.py` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/akinator/akinator.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/akinator/exceptions.py` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/akinator/exceptions.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/akinator/utils.py` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/akinator/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/docs/index.rst` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/examples/aki.py` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/examples/aki.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/examples/async_aki.py` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/examples/async_aki.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/pyproject.toml` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/akinator/setup.py` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/akinator/setup.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/game.py` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/game.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/bg.jpg` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/concentration_intense.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/concentration_intense.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/confiant.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/confiant.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/etonnement.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/etonnement.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/inspiration_forte.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/inspiration_forte.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/inspiration_legere.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/inspiration_legere.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/leger_decouragement.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/leger_decouragement.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/mobile.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/mobile.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/serein.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/serein.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/surprise.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/surprise.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/tension.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/tension.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/nonebot_plugin_akinator/res/vrai_decouragement.webp` & `nonebot-plugin-akinator-0.1.2/nonebot_plugin_akinator/res/vrai_decouragement.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.1/PKG-INFO` & `nonebot-plugin-akinator-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-akinator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Template plugin project
 License: MIT
 Author-email: student_2333 <lgc2333@126.com>
 Requires-Python: >=3.8,<4.0
-Provides-Extra: dev
 Provides-Extra: extra
 Project-URL: homepage, https://github.com/lgc2333/nonebot-plugin-akinator
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
@@ -126,16 +125,16 @@
 开始游戏后，直接发送你的答案即可（序号和文字均可）
 
 ### 效果图
 
 <details>
   <summary>点击展开</summary>
 
-![Alt text](readme/QQ%E5%9B%BE%E7%89%8720230415063509.png)  
-![Alt text](readme/QQ%E5%9B%BE%E7%89%8720230415063607.png)
+![Alt text](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/akinator/QQ%E5%9B%BE%E7%89%8720230415063509.png)  
+![Alt text](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/akinator/QQ%E5%9B%BE%E7%89%8720230415063607.png)
 
 </details>
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-akinator Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-akinator Version: 0.1.2 Summary:
 Template plugin project License: MIT Author-email: student_2333
-126.com> Requires-Python: >=3.8,<4.0 Provides-Extra: dev Provides-Extra: extra
-Project-URL: homepage, https://github.com/lgc2333/nonebot-plugin-akinator
-Description-Content-Type: text/markdown
+126.com> Requires-Python: >=3.8,<4.0 Provides-Extra: extra Project-URL:
+homepage, https://github.com/lgc2333/nonebot-plugin-akinator Description-
+Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # NoneBot-Plugin-Akinator _â¨ ç½ç»å¤©æ â¨_ [license] [pypi] [python]
                           [pypi_download] [wakatime]
 ## ð ä»ç» æç½ç»å¤©æ Akinator æ¬è¿ä½ ç Bot ! ## ð¿ å®è£
 ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
 å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
@@ -23,16 +23,17 @@
 é»è®¤å¼ | è¯´æ | | :-------------------: | :--: | :-----: | :--------------
 --------------------------------------: | | `PROXY` | å¦ | æ  | è®¿é®
 Akinator ä½¿ç¨çä»£ç | | `AKINATOR_CHILD_MODE` | å¦ | `False` |
 æ¯å¦å¯ç¨ Akinator çå¿ç«¥æ¨¡å¼ï¼ç»æä¸ä¼åºç° NSFW äººç©ï¼ | |
 `AKINATOR_LANGUAGE` | å¦ | `cn` | Akinator çè¯­è¨ | ## ð ä½¿ç¨
 åéæä»¤ `akinator` / `aki` å³å¯å¼å§æ¸¸æ
 å¼å§æ¸¸æåï¼ç´æ¥åéä½ çç­æ¡å³å¯ï¼åºå·åæå­åå¯ï¼ ###
-ææå¾  ç¹å»å±å¼ ![Alt text](readme/
-QQ%E5%9B%BE%E7%89%8720230415063509.png) ![Alt text](readme/
+ææå¾  ç¹å»å±å¼ ![Alt text](https://raw.githubusercontent.com/lgc-
+NB2Dev/readme/main/akinator/QQ%E5%9B%BE%E7%89%8720230415063509.png) ![Alt text]
+(https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/akinator/
 QQ%E5%9B%BE%E7%89%8720230415063607.png)  ## ð èç³» QQï¼3076823485
 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [Infiniticity/akinator.py](https://github.com/
 Infiniticity/akinator.py) - Akinator API çå°è£ ### [MeetWq/pil-utils]
 (https://github.com/MeetWq/pil-utils/) - Pillow å·¥å·åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
```

