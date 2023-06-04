# Comparing `tmp/nonebot_plugin_rimofun-0.1.0.tar.gz` & `tmp/nonebot_plugin_rimofun-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rimofun-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_rimofun-0.1.1.tar", last modified: Sun Jun  4 17:17:47 2023, max compression
```

## Comparing `nonebot_plugin_rimofun-0.1.0.tar` & `nonebot_plugin_rimofun-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1069 2023-03-10 20:27:35.092003 nonebot_plugin_rimofun-0.1.0/LICENSE
--rw-r--r--   0        0        0     3631 2023-03-10 20:27:35.092003 nonebot_plugin_rimofun-0.1.0/README.md
--rw-r--r--   0        0        0     1166 2023-03-10 20:27:35.092003 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/__init__.py
--rw-r--r--   0        0        0     5444 2023-03-10 20:27:35.092003 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/__main__.py
--rw-r--r--   0        0        0       57 2023-03-10 20:27:35.476026 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/.git
--rw-r--r--   0        0        0      147 2023-03-10 20:27:35.860049 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/LICENSE
--rw-r--r--   0        0        0     2590 2023-03-10 20:27:35.860049 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/__init__.py
--rw-r--r--   0        0        0     6002 2023-03-10 20:27:35.860049 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/常用汉字.json
--rw-r--r--   0        0        0   608988 2023-03-10 20:27:35.864050 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/现代汉语常用词表.json
--rw-r--r--   0        0        0     4455 2023-03-10 20:27:35.864050 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库.json
--rw-r--r--   0        0        0     7480 2023-03-10 20:27:35.864050 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库_数据增强.json
--rw-r--r--   0        0        0       69 2023-03-10 20:27:35.864050 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/莉沫词库.json
--rw-r--r--   0        0        0     5934 2023-03-10 20:27:35.864050 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/img/s.jpg
--rw-r--r--   0        0        0     1233 2023-03-10 20:27:35.864050 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/readme.md
--rw-r--r--   0        0        0      642 2023-03-10 20:27:35.864050 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/setup.py
--rw-r--r--   0        0        0     1635 2023-03-10 20:27:35.092003 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/config.py
--rw-r--r--   0        0        0     1997 2023-03-10 20:27:35.092003 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/data_source.py
--rw-r--r--   0        0        0       65 2023-03-10 20:27:35.852049 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/.git
--rw-r--r--   0        0        0     2332 2023-03-10 20:27:35.872050 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/not_translator/__init__.py
--rw-r--r--   0        0        0  3180205 2023-03-10 20:27:35.892051 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/en_US.txt
--rw-r--r--   0        0        0  1369263 2023-03-10 20:27:35.900052 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/zh_hans.txt
--rw-r--r--   0        0        0     6002 2023-03-10 20:27:35.900052 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/not_translator/常用汉字.json
--rw-r--r--   0        0        0    31239 2023-03-10 20:27:35.900052 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/not_translator/摸型.json
--rw-r--r--   0        0        0     4498 2023-03-10 20:27:35.904052 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/readme.md
--rw-r--r--   0        0        0    29473 2023-03-10 20:27:35.904052 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/训练代码/data/名字.json
--rw-r--r--   0        0        0     1191 2023-03-10 20:27:35.904052 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/训练代码/数据.py
--rw-r--r--   0        0        0     1740 2023-03-10 20:27:35.904052 nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/训练代码/超.py
--rw-r--r--   0        0        0     1243 2023-03-10 20:27:35.092003 nonebot_plugin_rimofun-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 nonebot_plugin_rimofun-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      575 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3619 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/README.md
+-rw-r--r--   0        0        0     1326 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/__init__.py
+-rw-r--r--   0        0        0     5444 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/__main__.py
+-rw-r--r--   0        0        0       57 2023-06-04 17:17:25.575806 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/.git
+-rw-r--r--   0        0        0      147 2023-06-04 17:17:26.247807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/LICENSE
+-rw-r--r--   0        0        0     2590 2023-06-04 17:17:26.247807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/__init__.py
+-rw-r--r--   0        0        0     6002 2023-06-04 17:17:26.247807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/常用汉字.json
+-rw-r--r--   0        0        0   608988 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/现代汉语常用词表.json
+-rw-r--r--   0        0        0     4455 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库.json
+-rw-r--r--   0        0        0     7480 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库_数据增强.json
+-rw-r--r--   0        0        0       69 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/莉沫词库.json
+-rw-r--r--   0        0        0     5934 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/img/s.jpg
+-rw-r--r--   0        0        0     1233 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/readme.md
+-rw-r--r--   0        0        0      642 2023-06-04 17:17:26.251807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/setup.py
+-rw-r--r--   0        0        0     1635 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/config.py
+-rw-r--r--   0        0        0     1997 2023-06-04 17:17:24.867806 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/data_source.py
+-rw-r--r--   0        0        0       65 2023-06-04 17:17:26.239807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/.git
+-rw-r--r--   0        0        0     2332 2023-06-04 17:17:26.259807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/__init__.py
+-rw-r--r--   0        0        0  3180205 2023-06-04 17:17:26.279807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/en_US.txt
+-rw-r--r--   0        0        0  1369263 2023-06-04 17:17:26.287807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/zh_hans.txt
+-rw-r--r--   0        0        0     6002 2023-06-04 17:17:26.287807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/常用汉字.json
+-rw-r--r--   0        0        0    31239 2023-06-04 17:17:26.291807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/摸型.json
+-rw-r--r--   0        0        0     4498 2023-06-04 17:17:26.291807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/readme.md
+-rw-r--r--   0        0        0    29473 2023-06-04 17:17:26.291807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/data/名字.json
+-rw-r--r--   0        0        0     1191 2023-06-04 17:17:26.291807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/数据.py
+-rw-r--r--   0        0        0     1740 2023-06-04 17:17:26.291807 nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/超.py
+-rw-r--r--   0        0        0      660 2023-06-04 17:17:47.614089 nonebot_plugin_rimofun-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 nonebot_plugin_rimofun-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_rimofun-0.1.0/README.md` & `nonebot_plugin_rimofun-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc2333/nonebot-plugin-rimofun/master/readme/rimofun.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/rimofun/rimofun.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # NoneBot-Plugin-RimoFun
 
 _✨ 基于 [RimoChan](https://github.com/RimoChan) 开发的工具的有趣插件~ ✨_
 
 <a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-rimofun.svg" alt="license">
+    <img src="https://img.shields.io/github/license/lgc2333/nonebot-plugin-rimofun.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-rimofun">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-rimofun.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 <a href="https://pypi.python.org/pypi/nonebot-plugin-rimofun">
   <img src="https://img.shields.io/pypi/dm/nonebot-plugin-rimofun" alt="pypi download">
```

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/__main__.py` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/__init__.py` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/常用汉字.json` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/常用汉字.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/现代汉语常用词表.json` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/现代汉语常用词表.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库.json` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库_数据增强.json` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/bnhhsh/data/色情词库_数据增强.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/img/s.jpg` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/img/s.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/readme.md` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/readme.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/bnhhsh/setup.py` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/bnhhsh/setup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/config.py` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/data_source.py` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/not_translator/__init__.py` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/en_US.txt` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/en_US.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/zh_hans.txt` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/ipa_data/zh_hans.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/not_translator/常用汉字.json` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/常用汉字.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/not_translator/摸型.json` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/not_translator/摸型.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/readme.md` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/readme.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/训练代码/data/名字.json` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/data/名字.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/训练代码/数据.py` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/数据.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/nonebot_plugin_rimofun/not_translator/训练代码/超.py` & `nonebot_plugin_rimofun-0.1.1/nonebot_plugin_rimofun/not_translator/训练代码/超.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rimofun-0.1.0/PKG-INFO` & `nonebot_plugin_rimofun-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rimofun
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use RimoChan's stuff to do some interesting things
+Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-rimofun
+Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
-Author: student_2333
-Author-email: lgc2333@126.com
-Requires-Python: >=3.8.1,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0-rc.1)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0)
-Requires-Dist: pypinyin (>=0.48.0,<0.49.0)
-Requires-Dist: unvcode (>=1.0.0,<2.0.0)
-Requires-Dist: yinglish (>=1.0.1,<2.0.0)
+Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-rimofun
+Requires-Python: <4.0,>=3.8
+Requires-Dist: nonebot2>=2.0.0
+Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
+Requires-Dist: pydantic<2.0.0,>=1.10.6
+Requires-Dist: pypinyin<1.0.0,>=0.48.0
+Requires-Dist: yinglish<2.0.0,>=1.0.1
+Requires-Dist: unvcode<2.0.0,>=1.0.0
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc2333/nonebot-plugin-rimofun/master/readme/rimofun.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <a href="https://v2.nonebot.dev/store"><img src="https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/rimofun/rimofun.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # NoneBot-Plugin-RimoFun
 
 _✨ 基于 [RimoChan](https://github.com/RimoChan) 开发的工具的有趣插件~ ✨_
 
 <a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-rimofun.svg" alt="license">
+    <img src="https://img.shields.io/github/license/lgc2333/nonebot-plugin-rimofun.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-rimofun">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-rimofun.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 <a href="https://pypi.python.org/pypi/nonebot-plugin-rimofun">
   <img src="https://img.shields.io/pypi/dm/nonebot-plugin-rimofun" alt="pypi download">
@@ -151,8 +147,7 @@
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
 芝士刚刚发布的插件，还没有更新日志的说 qwq~
-
```

#### html2text {}

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rimofun Version: 0.1.0 Summary: Use
-RimoChan's stuff to do some interesting things License: MIT Author:
-student_2333 Author-email: lgc2333@126.com Requires-Python: >=3.8.1,<4.0
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: nonebot-adapter-onebot
-(>=2.2.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0-rc.1) Requires-Dist: pydantic
-(>=1.10.6,<2.0.0) Requires-Dist: pypinyin (>=0.48.0,<0.49.0) Requires-Dist:
-unvcode (>=1.0.0,<2.0.0) Requires-Dist: yinglish (>=1.0.1,<2.0.0) Description-
+Metadata-Version: 2.1 Name: nonebot-plugin-rimofun Version: 0.1.1 Summary: Use
+RimoChan's stuff to do some interesting things Home-page: https://github.com/
+lgc-NB2Dev/nonebot-plugin-rimofun Author-Email: student_2333
+126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
+nonebot-plugin-rimofun Requires-Python: <4.0,>=3.8 Requires-Dist:
+nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1 Requires-
+Dist: pydantic<2.0.0,>=1.10.6 Requires-Dist: pypinyin<1.0.0,>=0.48.0 Requires-
+Dist: yinglish<2.0.0,>=1.0.1 Requires-Dist: unvcode<2.0.0,>=1.0.0 Description-
 Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-RimoFun _â¨ åºäº [RimoChan](https://github.com/RimoChan)
 å¼åçå·¥å·çæè¶£æä»¶~ â¨_ [license] [pypi] [python] [pypi_download]
                                   [wakatime]
 ## ð ä»ç» æä¸äº [RimoChan](https://github.com/RimoChan)
```

