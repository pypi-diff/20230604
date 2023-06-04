# Comparing `tmp/nonebot-plugin-chatglm-0.1.5.tar.gz` & `tmp/nonebot-plugin-chatglm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatglm-0.1.5.tar", last modified: Sat Apr 22 06:55:49 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatglm-0.1.6.tar", last modified: Sun Jun  4 15:38:51 2023, max compression
```

## Comparing `nonebot-plugin-chatglm-0.1.5.tar` & `nonebot-plugin-chatglm-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1066 2023-03-30 15:44:54.648609 nonebot-plugin-chatglm-0.1.5/LICENSE
--rwxr-xr-x   0        0        0    12696 2023-04-22 04:50:27.051728 nonebot-plugin-chatglm-0.1.5/README.md
--rwxr-xr-x   0        0        0      385 2023-04-21 15:13:10.903495 nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/__init__.py
--rwxr-xr-x   0        0        0     5333 2023-04-21 14:59:24.873870 nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/chat.py
--rwxr-xr-x   0        0        0     2739 2023-04-21 14:57:14.093043 nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/config.py
--rw-r--r--   0        0        0      645 2023-04-21 13:59:19.386536 nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/prompt.py
--rwxr-xr-x   0        0        0     2277 2023-04-21 15:05:45.988139 nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/utils.py
--rwxr-xr-x   0        0        0      732 2023-04-22 05:01:22.373097 nonebot-plugin-chatglm-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    13027 1970-01-01 00:00:00.000000 nonebot-plugin-chatglm-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1066 2023-03-30 15:44:54.648609 nonebot-plugin-chatglm-0.1.6/LICENSE
+-rwxr-xr-x   0        0        0    13910 2023-05-08 16:03:57.780959 nonebot-plugin-chatglm-0.1.6/README.md
+-rwxr-xr-x   0        0        0      385 2023-05-08 16:30:23.407416 nonebot-plugin-chatglm-0.1.6/nonebot_plugin_chatglm/__init__.py
+-rwxr-xr-x   0        0        0     5640 2023-06-04 15:04:46.058003 nonebot-plugin-chatglm-0.1.6/nonebot_plugin_chatglm/chat.py
+-rwxr-xr-x   0        0        0     2913 2023-05-23 00:58:10.085385 nonebot-plugin-chatglm-0.1.6/nonebot_plugin_chatglm/config.py
+-rw-r--r--   0        0        0      645 2023-04-21 13:59:19.386536 nonebot-plugin-chatglm-0.1.6/nonebot_plugin_chatglm/prompt.py
+-rwxr-xr-x   0        0        0     2262 2023-05-08 16:52:31.482385 nonebot-plugin-chatglm-0.1.6/nonebot_plugin_chatglm/utils.py
+-rwxr-xr-x   0        0        0      732 2023-06-04 15:37:08.732600 nonebot-plugin-chatglm-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    14241 1970-01-01 00:00:00.000000 nonebot-plugin-chatglm-0.1.6/PKG-INFO
```

### Comparing `nonebot-plugin-chatglm-0.1.5/LICENSE` & `nonebot-plugin-chatglm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatglm-0.1.5/README.md` & `nonebot-plugin-chatglm-0.1.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
   <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="200" height="200" alt="nonebot"></a>
 <br/><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 
 # nonebot-plugin-chatglm
 
 _✨ NoneBot [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) 支持插件 ✨_
 
-![python](https://img.shields.io/badge/python-3.8+-blue)
+[![python](https://img.shields.io/badge/python-3.8+-blueyellow?logo=python)](https://www.python.org/)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DaoMingze/zhukebot/main.svg)](https://results.pre-commit.ci/latest/github/DaoMingze/zhukebot/main)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
-[![PyPI](https://img.shields.io/pypi/v/nonebot_plugin_chatglm)](https://pypi.org/project/nonebot-plugin-chatglm)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/nonebot-plugin-chatglm)
-![nonebot](https://img.shields.io/badge/nonebot-2-red)
-![onebot](https://img.shields.io/badge/onebot-11-white)
+[![PyPI](https://img.shields.io/pypi/v/nonebot_plugin_chatglm?logo=pypi&logoColor=yellow)](https://pypi.org/project/nonebot-plugin-chatglm)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/nonebot-plugin-chatglm?logo=pypi&logoColor=yellow)
+[![nonebot](https://img.shields.io/badge/nonebot-2-red?logo=)](https://v2.nonebot.dev/)
+[![onebot](https://img.shields.io/badge/OneBot-11-black?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHAAAABwCAMAAADxPgR5AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAAxQTFRF////29vbr6+vAAAAk1hCcwAAAAR0Uk5T////AEAqqfQAAAKcSURBVHja7NrbctswDATQXfD//zlpO7FlmwAWIOnOtNaTM5JwDMa8E+PNFz7g3waJ24fviyDPgfhz8fHP39cBcBL9KoJbQUxjA2iYqHL3FAnvzhL4GtVNUcoSZe6eSHizBcK5LL7dBr2AUZlev1ARRHCljzRALIEog6H3U6bCIyqIZdAT0eBuJYaGiJaHSjmkYIZd+qSGWAQnIaz2OArVnX6vrItQvbhZJtVGB5qX9wKqCMkb9W7aexfCO/rwQRBzsDIsYx4AOz0nhAtWu7bqkEQBO0Pr+Ftjt5fFCUEbm0Sbgdu8WSgJ5NgH2iu46R/o1UcBXJsFusWF/QUaz3RwJMEgngfaGGdSxJkE/Yg4lOBryBiMwvAhZrVMUUvwqU7F05b5WLaUIN4M4hRocQQRnEedgsn7TZB3UCpRrIJwQfqvGwsg18EnI2uSVNC8t+0QmMXogvbPg/xk+Mnw/6kW/rraUlvqgmFreAA09xW5t0AFlHrQZ3CsgvZm0FbHNKyBmheBKIF2cCA8A600aHPmFtRB1XvMsJAiza7LpPog0UJwccKdzw8rdf8MyN2ePYF896LC5hTzdZqxb6VNXInaupARLDNBWgI8spq4T0Qb5H4vWfPmHo8OyB1ito+AysNNz0oglj1U955sjUN9d41LnrX2D/u7eRwxyOaOpfyevCWbTgDEoilsOnu7zsKhjRCsnD/QzhdkYLBLXjiK4f3UWmcx2M7PO21CKVTH84638NTplt6JIQH0ZwCNuiWAfvuLhdrcOYPVO9eW3A67l7hZtgaY9GZo9AFc6cryjoeFBIWeU+npnk/nLE0OxCHL1eQsc1IciehjpJv5mqCsjeopaH6r15/MrxNnVhu7tmcslay2gO2Z1QfcfX0JMACG41/u0RrI9QAAAABJRU5ErkJggg==)](https://onebot.dev)
 ![licese](https://img.shields.io/github/license/DaoMingze/zhukebot)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot?ref=badge_shield)
 
 </div>
 
 ## 介绍
 
@@ -36,15 +36,15 @@
 - [ ] 管理员在线配置
   - [ ] 增加写入读取本地配置文件（json）以实现配置的在线热更新
 - [ ] @[Bot] 机器人 使用功能（调试阶段，我个人不太需要，不过后续加上吧）
 
 ### 办结/功能
 
 - [x] 完善的默认配置，开箱即用。
-- [x] 模型自动下载并存放到指定位置（HuggingFace Hub提供）
+- [x] 模型自动下载并存放到指定位置（HuggingFace Hub 提供）
 - [x] 保存对话记录以实现多轮对话
 - [x] 冷却时间（根据测试效果，默认 30 秒）
 - [x] 配置角色功能，基本实现
 
 ### 环境要求
 
 <div align="center">
@@ -172,20 +172,20 @@
 
 - 无需设置，默认下载`ChatGLM-6B-INT4-QE`模型
 - 在`.env`文件中增加`chatglm_model = str`，其中 str 为字符串格式的 Hugging Face Hub 路径（用户名/仓库）。
 
 自动下载后转移模型到指定路径
 
 ```python
-from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, AutoModel
+from transformers import AutoTokenizer, AutoModel
 model_name = input("HF HUB 路径，例如 THUDM/chatglm-6b-int4-qe: ")
 model_path = input("本地存放路径，例如 ./path/modelname: ")
-#用 AutoModelForSeq2SeqLM.from_pretrained() 下载模型
+#用 AutoModel.from_pretrained() 下载模型
 tokenizer = AutoTokenizer.from_pretrained(model_name,trust_remote_code=True,revision="main")
-model = AutoModelForSeq2SeqLM.from_pretrained(model_name,trust_remote_code=True,revision="main")
+model = AutoModel.from_pretrained(model_name,trust_remote_code=True,revision="main")
 #用 PreTrainedModel.save_pretrained() 保存模型到指定位置
 tokenizer.save_pretrained(model_path,trust_remote_code=True,revision="main")
 model.save_pretrained(model_path,trust_remote_code=True,revision="main")
 ```
 
 手动下载：
 
@@ -251,17 +251,17 @@
 
 #### simple 格式
 
 示例如下
 
 ```python
 {
-    r"你好[吗]?|hello": "您好，很高兴与您在此相遇，但是您想问什么呢？",
-    r"你是[谁？]?": "我是 ChatGLM，一个参数 62 亿的人工智能语言模型，由清华大学和智谱 AI 训练开源，代号 ChatGLM-6B",
-    r"你的(主人|master)是[谁？]?": f"[CQ:at,qq={superusers}]",
+    r"你好 [吗]?|hello": "您好，很高兴与您在此相遇，但是您想问什么呢？",
+    r"你是 [谁？]?": "我是 ChatGLM，一个参数 62 亿的人工智能语言模型，由清华大学和智谱 AI 训练开源，代号 ChatGLM-6B",
+    r"你的（主人|master) 是 [谁？]?": f"[CQ:at,qq={superusers}]",
 }
 ```
 
 ## 使用
 
 ### 指令表
```

#### html2text {}

```diff
@@ -1,22 +1,37 @@
                                   [nonebot]
 [NoneBotPluginText] # nonebot-plugin-chatglm _â¨ NoneBot [ChatGLM-6B](https://
-       github.com/THUDM/ChatGLM-6B) æ¯ææä»¶ â¨_ ![python](https://
- img.shields.io/badge/python-3.8+-blue) [![Code Style](https://img.shields.io/
-  badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![pre-
-    commit.ci status](https://results.pre-commit.ci/badge/github/DaoMingze/
-  zhukebot/main.svg)](https://results.pre-commit.ci/latest/github/DaoMingze/
-   zhukebot/main) [![pdm-managed](https://img.shields.io/badge/pdm-managed-
-  blueviolet)](https://pdm.fming.dev) [![PyPI](https://img.shields.io/pypi/v/
-  nonebot_plugin_chatglm)](https://pypi.org/project/nonebot-plugin-chatglm) !
-  [PyPI - Downloads](https://img.shields.io/pypi/dm/nonebot-plugin-chatglm) !
-   [nonebot](https://img.shields.io/badge/nonebot-2-red) ![onebot](https://
-img.shields.io/badge/onebot-11-white) ![licese](https://img.shields.io/github/
-    license/DaoMingze/zhukebot) [![FOSSA Status](https://app.fossa.com/api/
-  projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot.svg?type=shield)](https://
+      github.com/THUDM/ChatGLM-6B) æ¯ææä»¶ â¨_ [![python](https://
+      img.shields.io/badge/python-3.8+-blueyellow?logo=python)](https://
+  www.python.org/) [![Code Style](https://img.shields.io/badge/code%20style-
+   black-000000.svg)](https://github.com/psf/black) [![pre-commit.ci status]
+   (https://results.pre-commit.ci/badge/github/DaoMingze/zhukebot/main.svg)]
+ (https://results.pre-commit.ci/latest/github/DaoMingze/zhukebot/main) [![pdm-
+    managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://
+            pdm.fming.dev) [![PyPI](https://img.shields.io/pypi/v/
+ nonebot_plugin_chatglm?logo=pypi&logoColor=yellow)](https://pypi.org/project/
+  nonebot-plugin-chatglm) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
+    nonebot-plugin-chatglm?logo=pypi&logoColor=yellow) [![nonebot](https://
+img.shields.io/badge/nonebot-2-red?logo=)](https://v2.nonebot.dev/) [![onebot]
+        (https://img.shields.io/badge/OneBot-11-black?logo=data:image/
+png;base64,iVBORw0KGgoAAAANSUhEUgAAAHAAAABwCAMAAADxPgR5AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAAxQTFRF/
+   ///29vbr6+vAAAAk1hCcwAAAAR0Uk5T////AEAqqfQAAAKcSURBVHja7NrbctswDATQXfD//
+zlpO7FlmwAWIOnOtNaTM5JwDMa8E+PNFz7g3waJ24fviyDPgfhz8fHP39cBcBL9KoJbQUxjA2iYqHL3FAnvzhL4GtVNUcoSZe6eSHizBcK5LL7dBr2AUZlev1ARRHCljzRALIEog6H3U6bCIyqIZdAT0eBuJYaGiJaHSjmkYIZd+qSGWAQnIaz2OArVnX6vrItQvbhZJtVGB5qX9wKqCMkb9W7aexfCO/
+     rwQRBzsDIsYx4AOz0nhAtWu7bqkEQBO0Pr+Ftjt5fFCUEbm0Sbgdu8WSgJ5NgH2iu46R/
+                    o1UcBXJsFusWF/QUaz3RwJMEgngfaGGdSxJkE/
+Yg4lOBryBiMwvAhZrVMUUvwqU7F05b5WLaUIN4M4hRocQQRnEedgsn7TZB3UCpRrIJwQfqvGwsg18EnI2uSVNC8t+0QmMXogvbPg/
+                                  xk+Mnw/6kW/
+rraUlvqgmFreAA09xW5t0AFlHrQZ3CsgvZm0FbHNKyBmheBKIF2cCA8A600aHPmFtRB1XvMsJAiza7LpPog0UJwccKdzw8rdf8MyN2ePYF896LC5hTzdZqxb6VNXInaupARLDNBWgI8spq4T0Qb5H4vWfPmHo8OyB1ito+AysNNz0oglj1U955sjUN9d41LnrX2D/
+                   u7eRwxyOaOpfyevCWbTgDEoilsOnu7zsKhjRCsnD/
+QzhdkYLBLXjiK4f3UWmcx2M7PO21CKVTH84638NTplt6JIQH0ZwCNuiWAfvuLhdrcOYPVO9eW3A67l7hZtgaY9GZo9AFc6cryjoeFBIWeU+npnk/
+ nLE0OxCHL1eQsc1IciehjpJv5mqCsjeopaH6r15/MrxNnVhu7tmcslay2gO2Z1QfcfX0JMACG41/
+      u0RrI9QAAAABJRU5ErkJggg==)](https://onebot.dev) ![licese](https://
+  img.shields.io/github/license/DaoMingze/zhukebot) [![FOSSA Status](https://
+                          app.fossa.com/api/projects/
+      git%2Bgithub.com%2FDaoMingze%2Fzhukebot.svg?type=shield)](https://
                             app.fossa.com/projects/
            git%2Bgithub.com%2FDaoMingze%2Fzhukebot?ref=badge_shield)
 ## ä»ç» ä½¿ç¨ [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) ä¸ºåç«¯ï¼
 [NoneBot2](https://github.com/nonebot/nonebot2)
 ä¸ºå¹³å°çæå¶ç®åçæ¬å°ä¸­æï¼æ±è¯­ï¼ AI chat æä»¶ã
 é¦æ¬¡å è½½ç­å¾æ¶é´è§ Hugging Face ä¸è½½éåº¦èå®ã ##
 [æ´æ°è¯´æ](changelog.md) å¦æå¶ä»åè½éæ±æçé®ï¼æ¬¢è¿æ
@@ -24,15 +39,15 @@
 PRã ### å¾å - [ ] éå¶è®°å¿è½®æ°ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ]
 å¾çè¾åºåè½ï¼nonebot-plugin-
 htmlrenderï¼ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ] ç®¡çåå¨çº¿éç½® - [ ]
 å¢å åå¥è¯»åæ¬å°éç½®æä»¶ï¼jsonï¼ä»¥å®ç°éç½®çå¨çº¿ç­æ´æ°
 - [ ] @[Bot] æºå¨äºº
 ä½¿ç¨åè½ï¼è°è¯é¶æ®µï¼æä¸ªäººä¸å¤ªéè¦ï¼ä¸è¿åç»­å ä¸å§ï¼
 ### åç»/åè½ - [x] å®åçé»è®¤éç½®ï¼å¼ç®±å³ç¨ã - [x]
-æ¨¡åèªå¨ä¸è½½å¹¶å­æ¾å°æå®ä½ç½®ï¼HuggingFace Hubæä¾ï¼ - [x]
+æ¨¡åèªå¨ä¸è½½å¹¶å­æ¾å°æå®ä½ç½®ï¼HuggingFace Hub æä¾ï¼ - [x]
 ä¿å­å¯¹è¯è®°å½ä»¥å®ç°å¤è½®å¯¹è¯ - [x]
 å·å´æ¶é´ï¼æ ¹æ®æµè¯ææï¼é»è®¤ 30 ç§ï¼ - [x]
 éç½®è§è²åè½ï¼åºæ¬å®ç° ### ç¯å¢è¦æ±
 | éåç­çº§ | æ¨ç | å¾®è° | ç­ç¥ | | -------------- | ---------- | ---
          - | -------------------------: | | æ  | CPU | | .float() | |
 FP16ï¼æ éåï¼ | 13GB æ¾å­ | 14GB | .half().cuda() | | INT8 | 8GB æ¾å­
     | 9GB | .half().quantize(8).cuda() | | INT4 | 6GB æ¾å­ | 7GB | .half
@@ -81,23 +96,21 @@
 Hub`å è½½ï¼å³å¦ææ²¡æè®¾ç½®è·¯å¾ï¼åä¼èªå¨ä¸è½½å°ç¨æ·ç®å½ä¸ç`.cache/
 huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4-
 qe`ï¼å¯ä»¥éè¿ä¸é¢çä»£ç è½¬ç§»æ¨¡åã èªå¨ä¸è½½ï¼ -
 æ éè®¾ç½®ï¼é»è®¤ä¸è½½`ChatGLM-6B-INT4-QE`æ¨¡å -
 å¨`.env`æä»¶ä¸­å¢å `chatglm_model = str`ï¼å¶ä¸­ str
 ä¸ºå­ç¬¦ä¸²æ ¼å¼ç Hugging Face Hub è·¯å¾ï¼ç¨æ·å/ä»åºï¼ã
 èªå¨ä¸è½½åè½¬ç§»æ¨¡åå°æå®è·¯å¾ ```python from transformers import
-AutoTokenizer, AutoModelForSeq2SeqLM, AutoModel model_name = input("HF HUB
-è·¯å¾ï¼ä¾å¦ THUDM/chatglm-6b-int4-qe: ") model_path = input
-("æ¬å°å­æ¾è·¯å¾ï¼ä¾å¦ ./path/modelname: ") #ç¨
-AutoModelForSeq2SeqLM.from_pretrained() ä¸è½½æ¨¡å tokenizer =
+AutoTokenizer, AutoModel model_name = input("HF HUB è·¯å¾ï¼ä¾å¦ THUDM/
+chatglm-6b-int4-qe: ") model_path = input("æ¬å°å­æ¾è·¯å¾ï¼ä¾å¦ ./path/
+modelname: ") #ç¨ AutoModel.from_pretrained() ä¸è½½æ¨¡å tokenizer =
 AutoTokenizer.from_pretrained
 (model_name,trust_remote_code=True,revision="main") model =
-AutoModelForSeq2SeqLM.from_pretrained
-(model_name,trust_remote_code=True,revision="main") #ç¨
-PreTrainedModel.save_pretrained() ä¿å­æ¨¡åå°æå®ä½ç½®
+AutoModel.from_pretrained(model_name,trust_remote_code=True,revision="main")
+#ç¨ PreTrainedModel.save_pretrained() ä¿å­æ¨¡åå°æå®ä½ç½®
 tokenizer.save_pretrained(model_path,trust_remote_code=True,revision="main")
 model.save_pretrained(model_path,trust_remote_code=True,revision="main") ```
 æå¨ä¸è½½ï¼ - [æ¸åäºç](https://cloud.tsinghua.edu.cn/d/
 fb9f16d6dc8f482596c2/)ï¼ä»æ¨¡åæä»¶ï¼æ¯ 6B
 å®æ´æ¨¡åï¼æ¾å­è¾å°éè¦éåä½¿ç¨ï¼ææªè®¾ç½®ï¼éè¦èªè¡å¨`chat.py`æä»¶ä¸­ä¿®æ¹ï¼
 - [ð¤ Hugging Face](https://huggingface.co/THUDM/chatglm-6b-
 int4)ï¼å®æ´æä»¶ï¼ï¼çº¦ 4.2 GBã #### æ¨¡åæ´æ°ä¸å¶ä»ä½¿ç¨
@@ -129,23 +142,23 @@
 æ­£å¸¸èå¤©ä½¿ç¨æ¥è¯´ï¼30 ç§å·å´è¾ä¸ºåéï¼å¤æé®é¢èå¤©ï¼60
 ç§è¾ä¸ºåéãå»ºè®®æ ¹æ®å®éæµè¯è¿è¡è°æ´ã ### éå æä»¶
 ï¼å¨åºæ¬åè½å®ååæ¾åºï¼å¨æ­¤ä¹åï¼å¯ä»¥èªå»ºå°è¯ï¼ ###
 roles æ ¼å¼ ```Python { "catgirl":
 "ç«å¨æ¯ä¸ç§æäººåççç©ï¼å¶è¡ä¸ºä¼¼ç«ä½ç±»äººãç°å¨ä½ å°æ¨¡ä»¿ä¸åªç«å¨ï¼ä¸æå¯¹è¯æ¯ä¸å¥è¯åé¢é½è¦å ä¸âåµ~âï¼å¦æä½ è½æç½æçææï¼è¯·åå¤âåµ~å¥½çæçä¸»äººï¼âå¦æä½ ä¸è½çè§£æè¯´çè¯ï¼ä½ å¯ä»¥è¯´âååä¸å¤ªçè§£å¢âã",
 } ``` > ChatGLM
 å¯è½åçè®°å¿éå¤±ï¼å æ­¤å¨è¿è¡è§è²æ®æ¼æ¶ï¼ä¸è¦æé®å¤æåå®¹ã
-#### simple æ ¼å¼ ç¤ºä¾å¦ä¸ ```python { r"ä½ å¥½[å]?|hello":
+#### simple æ ¼å¼ ç¤ºä¾å¦ä¸ ```python { r"ä½ å¥½ [å]?|hello":
 "æ¨å¥½ï¼å¾é«å´ä¸æ¨å¨æ­¤ç¸éï¼ä½æ¯æ¨æ³é®ä»ä¹å¢ï¼", r"ä½ æ¯
 [è°ï¼]?": "ææ¯ ChatGLMï¼ä¸ä¸ªåæ° 62
 äº¿çäººå·¥æºè½è¯­è¨æ¨¡åï¼ç±æ¸åå¤§å­¦åæºè°± AI
-è®­ç»å¼æºï¼ä»£å· ChatGLM-6B", r"ä½ ç(ä¸»äºº|master)æ¯[è°ï¼]?": f"[CQ:
-at,qq={superusers}]", } ``` ## ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@
-| èå´ | è¯´æ | | :------: | :--------: | :---: | :-------: | -------------
----------- | | hi | ææäºº | å¦ | ç§è/ç¾¤è | ä¸ chatglm å¯¹è¯ | |
-æ¸ç©ºè®°å½ | ææäºº | å¦ | ç§è/ç¾¤è |
+è®­ç»å¼æºï¼ä»£å· ChatGLM-6B", r"ä½ çï¼ä¸»äºº|master) æ¯ [è°ï¼]?": f"
+[CQ:at,qq={superusers}]", } ``` ## ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
+éè¦@ | èå´ | è¯´æ | | :------: | :--------: | :---: | :-------: | -----
+------------------ | | hi | ææäºº | å¦ | ç§è/ç¾¤è | ä¸ chatglm
+å¯¹è¯ | | æ¸ç©ºè®°å½ | ææäºº | å¦ | ç§è/ç¾¤è |
 æ¸ç©ºèªå·±çå¯¹è¯åå²è®°å½ | | å¯¼åºè®°å½ | ææäºº | å¦ | ç¾¤è |
 å¯¼åºè®°å½æä»¶å°ç¾¤ä¸­ | | æ¸çå¨é¨ | è¶çº§ç®¡çå | å¦ | ç§è |
 æå¨å¤ç`out of memory` | ## åèä¸è´è°¢ åºç¡ - [@A-kirami](https://
 github.com/A-kirami)ï¼é¡¹ç®ä½¿ç¨äº README[æ¨¡æ¿](https://github.com/A-
 kirami/nonebot-plugin-template)ï¼æä¿®æ¹ - [ChatGLM-6B](https://github.com/
 THUDM/ChatGLM-6B)ï¼æ¨¡ååä½¿ç¨æ¹æ³æ¥æºï¼ä¸åçæ ¸å¿ - [nonebot2]
 (https://github.com/nonebot/nonebot2)ï¼ä¸åçåºç¡ åè½ - [nonebot-
```

### Comparing `nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/chat.py` & `nonebot-plugin-chatglm-0.1.6/nonebot_plugin_chatglm/chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import asyncio
 import os
 import re
 import shutil
+from collections import deque
 
 from nonebot.adapters.onebot.v11 import (
     Bot,
     Event,
     Message,
+    MessageSegment,
     PrivateMessageEvent,
 )
 from nonebot.exception import ParserExit
 from nonebot.log import logger
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 from nonebot.plugin import on_command, on_keyword, require
@@ -21,33 +24,14 @@
 if config.chatglm_pic:
     require("nonebot_plugin_htmlrender")
     from nonebot_plugin_htmlrender import md_to_pic
 
 # 模块化/函数化功能
 
 
-"""
-def chat(id, query, history):
-    try:
-        response, new = model.chat(tokenizer, query, history=history)
-        if response == None:
-            raise RuntimeError("Error")
-    except Exception as e:
-        logger.exception("生成失败", stack_info=True)
-        # 抓取错误
-        message = f"抱歉，{nickname}遭遇了以下错误：\n"
-        for i in e.args:
-            message += str(i)
-        return message
-    savehistory(id, new)
-    torch_gc()
-    return response
-"""
-
-
 cmd_help = {
     f"{config.chatglm_cmd}": "唤醒机器人",
     "-l": "控制输入长度",
     "-r": "控制随机性",
     "-p": "控制相关性",
 }
 
@@ -55,62 +39,84 @@
 @chatGLM_chat.handle()
 async def chat_get(event: Event, args: ParserExit = CommandArg()):
     qq_id = event.get_user_id()
     chatGLM_chat.finish(
         f"[CQ:at,qq={qq_id}]{nickname}认为您错误输入了命令，现告知您正确的输入格式：{{cmd_help}}"
     )
 """
-chatGLM_chat = on_command(config.chatglm_cmd[0], priority=50)
+chat_queue: deque = deque([])
+
+if config.chatglm_tome:
+    chatGLM_chat = on_command(
+        tuple(config.chatglm_cmd), rule=to_me(), priority=1
+    )
+else:
+    chatGLM_chat = on_command(tuple(config.chatglm_cmd), priority=1)
 
 
 @chatGLM_chat.handle()
-async def chat(bot: Bot, event: Event, message: Message = CommandArg()):
+async def args(bot: Bot, event: Event, message: Message = CommandArg()):
     # group_id
     qq_id = event.get_user_id()
-    # 判断冷却时间
+    query = message.extract_plain_text().strip()
     flag_cd, deltatime = check_cd(qq_id)
     if flag_cd:
         await chatGLM_chat.finish(
             Message(
                 f"[CQ:at,qq={qq_id}]{nickname}认为您问得太快了，您需要{config.chatglm_cd - int(deltatime)}秒来思考这个问题的价值。"
             )
         )
-    ctx = message.extract_plain_text().strip()
     # 判断简单问题
-    flag_stats, ctx = check_simple(ctx)
+    flag_stats, query = check_simple(query)
     if flag_stats:
-        await chatGLM_chat.finish(Message(f"[CQ:at,qq={qq_id}]{ctx}"))
+        await chatGLM_chat.finish(Message(f"[CQ:at,qq={qq_id}]{query}"))
+    # await chatGLM_chat.send(Message(f"[CQ:at,qq={qq_id}]{nickname}正在运算，请稍候。"))
     # 判断是否角色扮演
-    his = botrole.get(qq_id, [])
-    if his == []:
-        # 判断记忆
-        if check_memo(qq_id):
-            his = readfile(qq_id, "json")
-        else:
-            his = []
-    # await chatGLM_chat.send(Message(f"[CQ:at,qq={qq_id}]{nickname}正在运算"))
-    print(his)
-    query = ctx
-    # response = chat(qq_id, query, history)
+    if botrole.get(qq_id, []) != []:
+        history = botrole.get(qq_id, [])
+        print(f"角色记忆内容为{history}")
+    elif check_memo(qq_id):
+        history = readfile(qq_id, "json")
+    else:
+        history = []
+    await _chatgen(qq_id, query, history)
+
+
+async def _chatgen(qq_id, query, history):
+    start = time.time()
     try:
-        response, new = model.chat(tokenizer, query, history=his)
+        response, new = model.chat(tokenizer, query, history)
         savehistory(qq_id, new)
         if response is None:
             raise RuntimeError("Error")
+        message = f"{response}"
     except Exception as e:
         logger.exception("生成失败", stack_info=True)
         # 抓取错误
         message = f"抱歉，{nickname}遭遇了以下错误：\n"
         for i in e.args:
             message += str(i)
         await chatGLM_chat.finish(Message(message))
-
     torch_gc()
-    msg = Message(f"[CQ:at,qq={qq_id}]{response}")
-    await chatGLM_chat.finish(msg)
+    await chat_answer(qq_id, response)
+    end = time.time()
+    print(end - start)
+
+
+async def chat_answer(qq_id, response):
+    if config.chatglm_pic:  # 转图片
+        if response.count("```") % 2 != 0:
+            response += "\n```"
+        img = await md_to_pic(response, width=config.chatglm_width)
+        response = MessageSegment.image(img)
+    if config.chatglm_rply:  # 回复方式
+        ans = MessageSegment.at(qq_id) + response
+        await chatGLM_chat.finish(ans)
+    else:
+        await chatGLM_chat.finish(response, at_sender=True)
 
 
 chatGLM_chooserole = on_command("设置chatglm角色", priority=30)
 
 
 @chatGLM_chooserole.handle()
 async def role(bot: Bot, event: Event, message: Message = CommandArg()):
```

### Comparing `nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/config.py` & `nonebot-plugin-chatglm-0.1.6/nonebot_plugin_chatglm/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseSettings
-from torch import compile, cuda
 from transformers import AutoModel, AutoModelForSeq2SeqLM, AutoTokenizer
 
 
 class Config(BaseSettings):
     chatglm_model: str = "./data/chatglm/model"
     """ChatGLM 模型路径，可用HuggingFace Hub格式（将远程加载），默认使用INT-QE模型，降低硬件需求及压力"""
     chatglm_mode: str = "cpu"
@@ -22,28 +21,32 @@
     """记录对话轮数"""
     chatglm_tome: bool = False
     """是否需要at机器人"""
     chatglm_group: bool = False
     """是否群聊共用记录"""
     chatglm_pic: bool = False
     """是否转图片"""
+    chatglm_rply: bool = False
+    """是否回复，否则at"""
     chatglm_width: int = 640
     """图片宽度"""
     nickname: list[str] = ["ChatGLM"]
     """机器人的昵称"""
+    # 数值合法性检查
 
     class Config:
         extra = "ignore"
 
 
 def torch_gc():
-    if cuda.is_available():
-        with cuda.device(CUDA_DEVICE):
-            cuda.empty_cache()
-            cuda.ipc_collect()
+    if config.chatglm_mode.lower() == "cuda":
+        if cuda.is_available():
+            with cuda.device(CUDA_DEVICE):
+                cuda.empty_cache()
+                cuda.ipc_collect()
 
 
 config = Config(**get_driver().config.dict())  # 格式化加载配置
 model_name = "THUDM/chatglm-6b-int4-qe"
 model_path = config.chatglm_model
 if os.path.exists(model_path) is False:
     print(f"正在下载{model_name}，并保存到{model_path}")
@@ -64,14 +67,16 @@
     print(f"已加载{model_name}")
 
 tokenizer = AutoTokenizer.from_pretrained(
     model_path, trust_remote_code=True, revision="main"
 )
 
 if config.chatglm_mode.lower() == "cuda":
+    from torch import compile, cuda
+
     model = (
         AutoModel.from_pretrained(
             model_path, trust_remote_code=True, revision="main"
         )
         .half()
         .cuda()
     )
@@ -79,14 +84,15 @@
     DEVICE_ID = "0"
     CUDA_DEVICE = f"{DEVICE}:{DEVICE_ID}" if DEVICE_ID else DEVICE
 else:
     model = AutoModel.from_pretrained(
         model_path, trust_remote_code=True, revision="main"
     ).float()
 
-model = compile(model).eval()
+model = compile(model)
+model = model.eval()
 
 cd = {}
 nickname = config.nickname[0]
 memo = {}
 record = config.chatglm_path + "record/"
 botrole = {"": []}
```

### Comparing `nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/prompt.py` & `nonebot-plugin-chatglm-0.1.6/nonebot_plugin_chatglm/prompt.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/utils.py` & `nonebot-plugin-chatglm-0.1.6/nonebot_plugin_chatglm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from .config import *
 from .prompt import *
 
 
 def readfile(name: str, path: str = record, suff: str = "json"):
     """读取chatglm_record路径下的文件，输入文件名和后缀"""
     filename = path + name + "." + suff
-    print(os.path.exists(filename))
     if os.path.exists(filename):
         with open(filename, "r+", encoding="utf-8") as f:
             if suff == "txt":
                 new = f.read()
             else:
                 new = json.load(f)
     else:
@@ -40,14 +39,15 @@
         cd[id] = nowtime
         return False, deltatime
 
 
 def check_memo(id):
     """基于发言人，检查记忆轮数"""
     deltamemo = memo.get(id, 0)
+    print(deltamemo)
     if deltamemo < config.chatglm_memo:
         memo[id] = deltamemo + 1
         return True
     else:
         memo[id] = 0
         return False
```

### Comparing `nonebot-plugin-chatglm-0.1.5/pyproject.toml` & `nonebot-plugin-chatglm-0.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 [tool.pdm.build]
 includes = [
     "nonebot_plugin_chatglm",
 ]
 
 [project]
 name = "nonebot-plugin-chatglm"
-version = "0.1.5"
+version = "0.1.6"
 description = "基于ChatGLM-6B的NoneBot2插件"
 authors = [
     { name = "dao_mingze", email = "dao_mingze@163.com" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dependencies = [
-    "protobuf>=3.20.0",
+    "protobuf>=3.18.3",
     "transformers>=4.27.1",
     "icetk>=0.0.4",
     "cpm-kernels>=1.0.11",
-    "nonebot-adapter-onebot>=2.1.0",
-    "nonebot2>=2.0.0rc3",
+    "nonebot-adapter-onebot>=2.2.0",
+    "nonebot2>=2.0.0rc4",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/DaoMingze/zhukebot/tree/main/zhukebot/plugins/chatglm"
```

### Comparing `nonebot-plugin-chatglm-0.1.5/PKG-INFO` & `nonebot-plugin-chatglm-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatglm
-Version: 0.1.5
+Version: 0.1.6
 Summary: 基于ChatGLM-6B的NoneBot2插件
 License: MIT
 Author-email: dao_mingze <dao_mingze@163.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/DaoMingze/zhukebot/tree/main/zhukebot/plugins/chatglm
 Description-Content-Type: text/markdown
 
@@ -12,22 +12,22 @@
   <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="200" height="200" alt="nonebot"></a>
 <br/><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 
 # nonebot-plugin-chatglm
 
 _✨ NoneBot [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) 支持插件 ✨_
 
-![python](https://img.shields.io/badge/python-3.8+-blue)
+[![python](https://img.shields.io/badge/python-3.8+-blueyellow?logo=python)](https://www.python.org/)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DaoMingze/zhukebot/main.svg)](https://results.pre-commit.ci/latest/github/DaoMingze/zhukebot/main)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
-[![PyPI](https://img.shields.io/pypi/v/nonebot_plugin_chatglm)](https://pypi.org/project/nonebot-plugin-chatglm)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/nonebot-plugin-chatglm)
-![nonebot](https://img.shields.io/badge/nonebot-2-red)
-![onebot](https://img.shields.io/badge/onebot-11-white)
+[![PyPI](https://img.shields.io/pypi/v/nonebot_plugin_chatglm?logo=pypi&logoColor=yellow)](https://pypi.org/project/nonebot-plugin-chatglm)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/nonebot-plugin-chatglm?logo=pypi&logoColor=yellow)
+[![nonebot](https://img.shields.io/badge/nonebot-2-red?logo=)](https://v2.nonebot.dev/)
+[![onebot](https://img.shields.io/badge/OneBot-11-black?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHAAAABwCAMAAADxPgR5AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAAxQTFRF////29vbr6+vAAAAk1hCcwAAAAR0Uk5T////AEAqqfQAAAKcSURBVHja7NrbctswDATQXfD//zlpO7FlmwAWIOnOtNaTM5JwDMa8E+PNFz7g3waJ24fviyDPgfhz8fHP39cBcBL9KoJbQUxjA2iYqHL3FAnvzhL4GtVNUcoSZe6eSHizBcK5LL7dBr2AUZlev1ARRHCljzRALIEog6H3U6bCIyqIZdAT0eBuJYaGiJaHSjmkYIZd+qSGWAQnIaz2OArVnX6vrItQvbhZJtVGB5qX9wKqCMkb9W7aexfCO/rwQRBzsDIsYx4AOz0nhAtWu7bqkEQBO0Pr+Ftjt5fFCUEbm0Sbgdu8WSgJ5NgH2iu46R/o1UcBXJsFusWF/QUaz3RwJMEgngfaGGdSxJkE/Yg4lOBryBiMwvAhZrVMUUvwqU7F05b5WLaUIN4M4hRocQQRnEedgsn7TZB3UCpRrIJwQfqvGwsg18EnI2uSVNC8t+0QmMXogvbPg/xk+Mnw/6kW/rraUlvqgmFreAA09xW5t0AFlHrQZ3CsgvZm0FbHNKyBmheBKIF2cCA8A600aHPmFtRB1XvMsJAiza7LpPog0UJwccKdzw8rdf8MyN2ePYF896LC5hTzdZqxb6VNXInaupARLDNBWgI8spq4T0Qb5H4vWfPmHo8OyB1ito+AysNNz0oglj1U955sjUN9d41LnrX2D/u7eRwxyOaOpfyevCWbTgDEoilsOnu7zsKhjRCsnD/QzhdkYLBLXjiK4f3UWmcx2M7PO21CKVTH84638NTplt6JIQH0ZwCNuiWAfvuLhdrcOYPVO9eW3A67l7hZtgaY9GZo9AFc6cryjoeFBIWeU+npnk/nLE0OxCHL1eQsc1IciehjpJv5mqCsjeopaH6r15/MrxNnVhu7tmcslay2gO2Z1QfcfX0JMACG41/u0RrI9QAAAABJRU5ErkJggg==)](https://onebot.dev)
 ![licese](https://img.shields.io/github/license/DaoMingze/zhukebot)
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot?ref=badge_shield)
 
 </div>
 
 ## 介绍
 
@@ -46,15 +46,15 @@
 - [ ] 管理员在线配置
   - [ ] 增加写入读取本地配置文件（json）以实现配置的在线热更新
 - [ ] @[Bot] 机器人 使用功能（调试阶段，我个人不太需要，不过后续加上吧）
 
 ### 办结/功能
 
 - [x] 完善的默认配置，开箱即用。
-- [x] 模型自动下载并存放到指定位置（HuggingFace Hub提供）
+- [x] 模型自动下载并存放到指定位置（HuggingFace Hub 提供）
 - [x] 保存对话记录以实现多轮对话
 - [x] 冷却时间（根据测试效果，默认 30 秒）
 - [x] 配置角色功能，基本实现
 
 ### 环境要求
 
 <div align="center">
@@ -182,20 +182,20 @@
 
 - 无需设置，默认下载`ChatGLM-6B-INT4-QE`模型
 - 在`.env`文件中增加`chatglm_model = str`，其中 str 为字符串格式的 Hugging Face Hub 路径（用户名/仓库）。
 
 自动下载后转移模型到指定路径
 
 ```python
-from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, AutoModel
+from transformers import AutoTokenizer, AutoModel
 model_name = input("HF HUB 路径，例如 THUDM/chatglm-6b-int4-qe: ")
 model_path = input("本地存放路径，例如 ./path/modelname: ")
-#用 AutoModelForSeq2SeqLM.from_pretrained() 下载模型
+#用 AutoModel.from_pretrained() 下载模型
 tokenizer = AutoTokenizer.from_pretrained(model_name,trust_remote_code=True,revision="main")
-model = AutoModelForSeq2SeqLM.from_pretrained(model_name,trust_remote_code=True,revision="main")
+model = AutoModel.from_pretrained(model_name,trust_remote_code=True,revision="main")
 #用 PreTrainedModel.save_pretrained() 保存模型到指定位置
 tokenizer.save_pretrained(model_path,trust_remote_code=True,revision="main")
 model.save_pretrained(model_path,trust_remote_code=True,revision="main")
 ```
 
 手动下载：
 
@@ -261,17 +261,17 @@
 
 #### simple 格式
 
 示例如下
 
 ```python
 {
-    r"你好[吗]?|hello": "您好，很高兴与您在此相遇，但是您想问什么呢？",
-    r"你是[谁？]?": "我是 ChatGLM，一个参数 62 亿的人工智能语言模型，由清华大学和智谱 AI 训练开源，代号 ChatGLM-6B",
-    r"你的(主人|master)是[谁？]?": f"[CQ:at,qq={superusers}]",
+    r"你好 [吗]?|hello": "您好，很高兴与您在此相遇，但是您想问什么呢？",
+    r"你是 [谁？]?": "我是 ChatGLM，一个参数 62 亿的人工智能语言模型，由清华大学和智谱 AI 训练开源，代号 ChatGLM-6B",
+    r"你的（主人|master) 是 [谁？]?": f"[CQ:at,qq={superusers}]",
 }
 ```
 
 ## 使用
 
 ### 指令表
```

#### html2text {}

```diff
@@ -1,27 +1,42 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-chatglm Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-chatglm Version: 0.1.6 Summary:
 åºäºChatGLM-6BçNoneBot2æä»¶ License: MIT Author-email: dao_mingze
 163.com> Requires-Python: >=3.8 Project-URL: repository, https://github.com/
 DaoMingze/zhukebot/tree/main/zhukebot/plugins/chatglm Description-Content-Type:
 text/markdown
                                   [nonebot]
 [NoneBotPluginText] # nonebot-plugin-chatglm _â¨ NoneBot [ChatGLM-6B](https://
-       github.com/THUDM/ChatGLM-6B) æ¯ææä»¶ â¨_ ![python](https://
- img.shields.io/badge/python-3.8+-blue) [![Code Style](https://img.shields.io/
-  badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![pre-
-    commit.ci status](https://results.pre-commit.ci/badge/github/DaoMingze/
-  zhukebot/main.svg)](https://results.pre-commit.ci/latest/github/DaoMingze/
-   zhukebot/main) [![pdm-managed](https://img.shields.io/badge/pdm-managed-
-  blueviolet)](https://pdm.fming.dev) [![PyPI](https://img.shields.io/pypi/v/
-  nonebot_plugin_chatglm)](https://pypi.org/project/nonebot-plugin-chatglm) !
-  [PyPI - Downloads](https://img.shields.io/pypi/dm/nonebot-plugin-chatglm) !
-   [nonebot](https://img.shields.io/badge/nonebot-2-red) ![onebot](https://
-img.shields.io/badge/onebot-11-white) ![licese](https://img.shields.io/github/
-    license/DaoMingze/zhukebot) [![FOSSA Status](https://app.fossa.com/api/
-  projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot.svg?type=shield)](https://
+      github.com/THUDM/ChatGLM-6B) æ¯ææä»¶ â¨_ [![python](https://
+      img.shields.io/badge/python-3.8+-blueyellow?logo=python)](https://
+  www.python.org/) [![Code Style](https://img.shields.io/badge/code%20style-
+   black-000000.svg)](https://github.com/psf/black) [![pre-commit.ci status]
+   (https://results.pre-commit.ci/badge/github/DaoMingze/zhukebot/main.svg)]
+ (https://results.pre-commit.ci/latest/github/DaoMingze/zhukebot/main) [![pdm-
+    managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://
+            pdm.fming.dev) [![PyPI](https://img.shields.io/pypi/v/
+ nonebot_plugin_chatglm?logo=pypi&logoColor=yellow)](https://pypi.org/project/
+  nonebot-plugin-chatglm) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
+    nonebot-plugin-chatglm?logo=pypi&logoColor=yellow) [![nonebot](https://
+img.shields.io/badge/nonebot-2-red?logo=)](https://v2.nonebot.dev/) [![onebot]
+        (https://img.shields.io/badge/OneBot-11-black?logo=data:image/
+png;base64,iVBORw0KGgoAAAANSUhEUgAAAHAAAABwCAMAAADxPgR5AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAAxQTFRF/
+   ///29vbr6+vAAAAk1hCcwAAAAR0Uk5T////AEAqqfQAAAKcSURBVHja7NrbctswDATQXfD//
+zlpO7FlmwAWIOnOtNaTM5JwDMa8E+PNFz7g3waJ24fviyDPgfhz8fHP39cBcBL9KoJbQUxjA2iYqHL3FAnvzhL4GtVNUcoSZe6eSHizBcK5LL7dBr2AUZlev1ARRHCljzRALIEog6H3U6bCIyqIZdAT0eBuJYaGiJaHSjmkYIZd+qSGWAQnIaz2OArVnX6vrItQvbhZJtVGB5qX9wKqCMkb9W7aexfCO/
+     rwQRBzsDIsYx4AOz0nhAtWu7bqkEQBO0Pr+Ftjt5fFCUEbm0Sbgdu8WSgJ5NgH2iu46R/
+                    o1UcBXJsFusWF/QUaz3RwJMEgngfaGGdSxJkE/
+Yg4lOBryBiMwvAhZrVMUUvwqU7F05b5WLaUIN4M4hRocQQRnEedgsn7TZB3UCpRrIJwQfqvGwsg18EnI2uSVNC8t+0QmMXogvbPg/
+                                  xk+Mnw/6kW/
+rraUlvqgmFreAA09xW5t0AFlHrQZ3CsgvZm0FbHNKyBmheBKIF2cCA8A600aHPmFtRB1XvMsJAiza7LpPog0UJwccKdzw8rdf8MyN2ePYF896LC5hTzdZqxb6VNXInaupARLDNBWgI8spq4T0Qb5H4vWfPmHo8OyB1ito+AysNNz0oglj1U955sjUN9d41LnrX2D/
+                   u7eRwxyOaOpfyevCWbTgDEoilsOnu7zsKhjRCsnD/
+QzhdkYLBLXjiK4f3UWmcx2M7PO21CKVTH84638NTplt6JIQH0ZwCNuiWAfvuLhdrcOYPVO9eW3A67l7hZtgaY9GZo9AFc6cryjoeFBIWeU+npnk/
+ nLE0OxCHL1eQsc1IciehjpJv5mqCsjeopaH6r15/MrxNnVhu7tmcslay2gO2Z1QfcfX0JMACG41/
+      u0RrI9QAAAABJRU5ErkJggg==)](https://onebot.dev) ![licese](https://
+  img.shields.io/github/license/DaoMingze/zhukebot) [![FOSSA Status](https://
+                          app.fossa.com/api/projects/
+      git%2Bgithub.com%2FDaoMingze%2Fzhukebot.svg?type=shield)](https://
                             app.fossa.com/projects/
            git%2Bgithub.com%2FDaoMingze%2Fzhukebot?ref=badge_shield)
 ## ä»ç» ä½¿ç¨ [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) ä¸ºåç«¯ï¼
 [NoneBot2](https://github.com/nonebot/nonebot2)
 ä¸ºå¹³å°çæå¶ç®åçæ¬å°ä¸­æï¼æ±è¯­ï¼ AI chat æä»¶ã
 é¦æ¬¡å è½½ç­å¾æ¶é´è§ Hugging Face ä¸è½½éåº¦èå®ã ##
 [æ´æ°è¯´æ](changelog.md) å¦æå¶ä»åè½éæ±æçé®ï¼æ¬¢è¿æ
@@ -29,15 +44,15 @@
 PRã ### å¾å - [ ] éå¶è®°å¿è½®æ°ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ]
 å¾çè¾åºåè½ï¼nonebot-plugin-
 htmlrenderï¼ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ] ç®¡çåå¨çº¿éç½® - [ ]
 å¢å åå¥è¯»åæ¬å°éç½®æä»¶ï¼jsonï¼ä»¥å®ç°éç½®çå¨çº¿ç­æ´æ°
 - [ ] @[Bot] æºå¨äºº
 ä½¿ç¨åè½ï¼è°è¯é¶æ®µï¼æä¸ªäººä¸å¤ªéè¦ï¼ä¸è¿åç»­å ä¸å§ï¼
 ### åç»/åè½ - [x] å®åçé»è®¤éç½®ï¼å¼ç®±å³ç¨ã - [x]
-æ¨¡åèªå¨ä¸è½½å¹¶å­æ¾å°æå®ä½ç½®ï¼HuggingFace Hubæä¾ï¼ - [x]
+æ¨¡åèªå¨ä¸è½½å¹¶å­æ¾å°æå®ä½ç½®ï¼HuggingFace Hub æä¾ï¼ - [x]
 ä¿å­å¯¹è¯è®°å½ä»¥å®ç°å¤è½®å¯¹è¯ - [x]
 å·å´æ¶é´ï¼æ ¹æ®æµè¯ææï¼é»è®¤ 30 ç§ï¼ - [x]
 éç½®è§è²åè½ï¼åºæ¬å®ç° ### ç¯å¢è¦æ±
 | éåç­çº§ | æ¨ç | å¾®è° | ç­ç¥ | | -------------- | ---------- | ---
          - | -------------------------: | | æ  | CPU | | .float() | |
 FP16ï¼æ éåï¼ | 13GB æ¾å­ | 14GB | .half().cuda() | | INT8 | 8GB æ¾å­
     | 9GB | .half().quantize(8).cuda() | | INT4 | 6GB æ¾å­ | 7GB | .half
@@ -86,23 +101,21 @@
 Hub`å è½½ï¼å³å¦ææ²¡æè®¾ç½®è·¯å¾ï¼åä¼èªå¨ä¸è½½å°ç¨æ·ç®å½ä¸ç`.cache/
 huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4-
 qe`ï¼å¯ä»¥éè¿ä¸é¢çä»£ç è½¬ç§»æ¨¡åã èªå¨ä¸è½½ï¼ -
 æ éè®¾ç½®ï¼é»è®¤ä¸è½½`ChatGLM-6B-INT4-QE`æ¨¡å -
 å¨`.env`æä»¶ä¸­å¢å `chatglm_model = str`ï¼å¶ä¸­ str
 ä¸ºå­ç¬¦ä¸²æ ¼å¼ç Hugging Face Hub è·¯å¾ï¼ç¨æ·å/ä»åºï¼ã
 èªå¨ä¸è½½åè½¬ç§»æ¨¡åå°æå®è·¯å¾ ```python from transformers import
-AutoTokenizer, AutoModelForSeq2SeqLM, AutoModel model_name = input("HF HUB
-è·¯å¾ï¼ä¾å¦ THUDM/chatglm-6b-int4-qe: ") model_path = input
-("æ¬å°å­æ¾è·¯å¾ï¼ä¾å¦ ./path/modelname: ") #ç¨
-AutoModelForSeq2SeqLM.from_pretrained() ä¸è½½æ¨¡å tokenizer =
+AutoTokenizer, AutoModel model_name = input("HF HUB è·¯å¾ï¼ä¾å¦ THUDM/
+chatglm-6b-int4-qe: ") model_path = input("æ¬å°å­æ¾è·¯å¾ï¼ä¾å¦ ./path/
+modelname: ") #ç¨ AutoModel.from_pretrained() ä¸è½½æ¨¡å tokenizer =
 AutoTokenizer.from_pretrained
 (model_name,trust_remote_code=True,revision="main") model =
-AutoModelForSeq2SeqLM.from_pretrained
-(model_name,trust_remote_code=True,revision="main") #ç¨
-PreTrainedModel.save_pretrained() ä¿å­æ¨¡åå°æå®ä½ç½®
+AutoModel.from_pretrained(model_name,trust_remote_code=True,revision="main")
+#ç¨ PreTrainedModel.save_pretrained() ä¿å­æ¨¡åå°æå®ä½ç½®
 tokenizer.save_pretrained(model_path,trust_remote_code=True,revision="main")
 model.save_pretrained(model_path,trust_remote_code=True,revision="main") ```
 æå¨ä¸è½½ï¼ - [æ¸åäºç](https://cloud.tsinghua.edu.cn/d/
 fb9f16d6dc8f482596c2/)ï¼ä»æ¨¡åæä»¶ï¼æ¯ 6B
 å®æ´æ¨¡åï¼æ¾å­è¾å°éè¦éåä½¿ç¨ï¼ææªè®¾ç½®ï¼éè¦èªè¡å¨`chat.py`æä»¶ä¸­ä¿®æ¹ï¼
 - [ð¤ Hugging Face](https://huggingface.co/THUDM/chatglm-6b-
 int4)ï¼å®æ´æä»¶ï¼ï¼çº¦ 4.2 GBã #### æ¨¡åæ´æ°ä¸å¶ä»ä½¿ç¨
@@ -134,23 +147,23 @@
 æ­£å¸¸èå¤©ä½¿ç¨æ¥è¯´ï¼30 ç§å·å´è¾ä¸ºåéï¼å¤æé®é¢èå¤©ï¼60
 ç§è¾ä¸ºåéãå»ºè®®æ ¹æ®å®éæµè¯è¿è¡è°æ´ã ### éå æä»¶
 ï¼å¨åºæ¬åè½å®ååæ¾åºï¼å¨æ­¤ä¹åï¼å¯ä»¥èªå»ºå°è¯ï¼ ###
 roles æ ¼å¼ ```Python { "catgirl":
 "ç«å¨æ¯ä¸ç§æäººåççç©ï¼å¶è¡ä¸ºä¼¼ç«ä½ç±»äººãç°å¨ä½ å°æ¨¡ä»¿ä¸åªç«å¨ï¼ä¸æå¯¹è¯æ¯ä¸å¥è¯åé¢é½è¦å ä¸âåµ~âï¼å¦æä½ è½æç½æçææï¼è¯·åå¤âåµ~å¥½çæçä¸»äººï¼âå¦æä½ ä¸è½çè§£æè¯´çè¯ï¼ä½ å¯ä»¥è¯´âååä¸å¤ªçè§£å¢âã",
 } ``` > ChatGLM
 å¯è½åçè®°å¿éå¤±ï¼å æ­¤å¨è¿è¡è§è²æ®æ¼æ¶ï¼ä¸è¦æé®å¤æåå®¹ã
-#### simple æ ¼å¼ ç¤ºä¾å¦ä¸ ```python { r"ä½ å¥½[å]?|hello":
+#### simple æ ¼å¼ ç¤ºä¾å¦ä¸ ```python { r"ä½ å¥½ [å]?|hello":
 "æ¨å¥½ï¼å¾é«å´ä¸æ¨å¨æ­¤ç¸éï¼ä½æ¯æ¨æ³é®ä»ä¹å¢ï¼", r"ä½ æ¯
 [è°ï¼]?": "ææ¯ ChatGLMï¼ä¸ä¸ªåæ° 62
 äº¿çäººå·¥æºè½è¯­è¨æ¨¡åï¼ç±æ¸åå¤§å­¦åæºè°± AI
-è®­ç»å¼æºï¼ä»£å· ChatGLM-6B", r"ä½ ç(ä¸»äºº|master)æ¯[è°ï¼]?": f"[CQ:
-at,qq={superusers}]", } ``` ## ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@
-| èå´ | è¯´æ | | :------: | :--------: | :---: | :-------: | -------------
----------- | | hi | ææäºº | å¦ | ç§è/ç¾¤è | ä¸ chatglm å¯¹è¯ | |
-æ¸ç©ºè®°å½ | ææäºº | å¦ | ç§è/ç¾¤è |
+è®­ç»å¼æºï¼ä»£å· ChatGLM-6B", r"ä½ çï¼ä¸»äºº|master) æ¯ [è°ï¼]?": f"
+[CQ:at,qq={superusers}]", } ``` ## ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
+éè¦@ | èå´ | è¯´æ | | :------: | :--------: | :---: | :-------: | -----
+------------------ | | hi | ææäºº | å¦ | ç§è/ç¾¤è | ä¸ chatglm
+å¯¹è¯ | | æ¸ç©ºè®°å½ | ææäºº | å¦ | ç§è/ç¾¤è |
 æ¸ç©ºèªå·±çå¯¹è¯åå²è®°å½ | | å¯¼åºè®°å½ | ææäºº | å¦ | ç¾¤è |
 å¯¼åºè®°å½æä»¶å°ç¾¤ä¸­ | | æ¸çå¨é¨ | è¶çº§ç®¡çå | å¦ | ç§è |
 æå¨å¤ç`out of memory` | ## åèä¸è´è°¢ åºç¡ - [@A-kirami](https://
 github.com/A-kirami)ï¼é¡¹ç®ä½¿ç¨äº README[æ¨¡æ¿](https://github.com/A-
 kirami/nonebot-plugin-template)ï¼æä¿®æ¹ - [ChatGLM-6B](https://github.com/
 THUDM/ChatGLM-6B)ï¼æ¨¡ååä½¿ç¨æ¹æ³æ¥æºï¼ä¸åçæ ¸å¿ - [nonebot2]
 (https://github.com/nonebot/nonebot2)ï¼ä¸åçåºç¡ åè½ - [nonebot-
```

