# Comparing `tmp/nonebot_plugin_bawiki-0.7.7.tar.gz` & `tmp/nonebot_plugin_bawiki-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.7.7.tar", last modified: Wed May 10 08:35:56 2023, max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.7.8.tar", last modified: Sun Jun  4 17:32:28 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.7.7.tar` & `nonebot_plugin_bawiki-0.7.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1068 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/LICENSE
--rw-r--r--   0        0        0     7722 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/README.md
--rw-r--r--   0        0        0    15528 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0    22664 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/__main__.py
--rw-r--r--   0        0        0     1881 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0     5812 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_bawiki.py
--rw-r--r--   0        0        0     8291 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_gamekee.py
--rw-r--r--   0        0        0    18827 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_schaledb.py
--rw-r--r--   0        0        0     7390 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/gacha.py
--rw-r--r--   0        0        0    21514 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-05-10 08:35:30.229850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gradient.png
--rw-r--r--   0        0        0      872 2023-05-10 08:35:30.229850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/resource.py
--rw-r--r--   0        0        0     3555 2023-05-10 08:35:30.229850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1381 2023-05-10 08:35:56.677607 nonebot_plugin_bawiki-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     9063 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/LICENSE
+-rw-r--r--   0        0        0     7722 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/README.md
+-rw-r--r--   0        0        0    14616 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0    22664 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/__main__.py
+-rw-r--r--   0        0        0     1881 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0     5812 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_bawiki.py
+-rw-r--r--   0        0        0     8291 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_gamekee.py
+-rw-r--r--   0        0        0    18827 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_schaledb.py
+-rw-r--r--   0        0        0     7390 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/gacha.py
+-rw-r--r--   0        0        0    21514 2023-06-04 17:15:18.634142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-06-04 17:15:18.638142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-06-04 17:15:18.642142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gradient.png
+-rw-r--r--   0        0        0      872 2023-06-04 17:15:18.642142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/resource.py
+-rw-r--r--   0        0        0     3555 2023-06-04 17:15:18.642142 nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1379 2023-06-04 17:32:28.667012 nonebot_plugin_bawiki-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     9061 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.8/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.7.7/LICENSE` & `nonebot_plugin_bawiki-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/README.md` & `nonebot_plugin_bawiki-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/__init__.py` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,305 +1,310 @@
-from nonebot import require
+from nonebot import get_available_plugin_names, require
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 
 from . import __main__ as __main__  # noqa: E402
+from .config import Cfg as Cfg  # noqa: E402
 
-__version__ = "0.7.7"
+__version__ = "0.7.8"
 __plugin_meta__ = PluginMetadata(
     name="BAWiki",
     description="碧蓝档案Wiki插件",
-    usage=(
-        "感谢各位sensei使用本插件！\n"
-        "插件有缓存机制，每3小时自动清空一次，如果插件遇到问题可以先手动清空缓存试一下捏\n"
-        "装载PicMenu插件即可查看插件详细菜单哦\n"
-        "祝玩得愉快～"
-    ),
-    extra={
-        "menu_template": "default",
-        "menu_data": [
-            {
-                "func": "日程表",
-                "trigger_method": "指令",
-                "trigger_condition": "ba日程表",
-                "brief_des": "查看活动日程表",
-                "detail_des": (
-                    "查看当前未结束的卡池、活动以及起止时间，"
-                    "默认为GameKee源，可以在指令后带参数使用SchaleDB数据源\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba日程表</ft> （GameKee源）\n"
-                    "- <ft color=(238,120,0)>ba日程表 schaledb</ft> （SchaleDB源，日服国际服一起发）\n"
-                    "- <ft color=(238,120,0)>ba日程表 schale 国际服</ft> （SchaleDB源，国际服）"
-                ),
-            },
-            {
-                "func": "学生图鉴",
-                "trigger_method": "指令",
-                "trigger_condition": "ba学生图鉴",
-                "brief_des": "查询学生详情（SchaleDB）",
-                "detail_des": (
-                    "访问对应学生SchaleDB页面并截图，支持部分学生别名\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba学生图鉴 白子</ft>\n"
-                    "- <ft color=(238,120,0)>ba学生图鉴 xcw</ft>"
-                ),
-            },
-            {
-                "func": "学生Wiki",
-                "trigger_method": "指令",
-                "trigger_condition": "ba学生wiki",
-                "brief_des": "查询学生详情（GameKee）",
-                "detail_des": (
-                    "访问对应学生GameKee Wiki页面并截图，支持部分学生别名\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba学生wiki 白子</ft>\n"
-                    "- <ft color=(238,120,0)>ba学生wiki xcw</ft>"
-                ),
-            },
-            {
-                "func": "羁绊查询",
-                "trigger_method": "指令",
-                "trigger_condition": "ba羁绊",
-                "brief_des": "查询学生解锁L2D需求的羁绊等级",
-                "detail_des": (
-                    "使用学生名称查询该学生解锁L2D看板需求的羁绊等级以及L2D预览，"
-                    "或者使用羁绊等级级数查询哪些学生达到该等级时解锁L2D看板\n"
-                    "使用学生名称查询时支持部分学生别名\n"
-                    " \n"
-                    "可以用这些指令触发：\n"
-                    "- <ft color=(238,120,0)>ba羁绊</ft>\n"
-                    "- <ft color=(238,120,0)>ba好感度</ft>\n"
-                    "- <ft color=(238,120,0)>bal2d</ft>\n"
-                    "- <ft color=(238,120,0)>balive2d</ft>\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba羁绊 xcw</ft>\n"
-                    "- <ft color=(238,120,0)>ba羁绊 9</ft>"
-                ),
-            },
-            {
-                "func": "角色评价",
-                "trigger_method": "指令",
-                "trigger_condition": "ba角评",
-                "brief_des": "查询学生角评一图流",
-                "detail_des": (
-                    "发送一张指定角色的评价图\n"
-                    "支持部分学生别名\n"
-                    "角评图作者 B站@夜猫咪喵喵猫\n"
-                    " \n"
-                    "可以使用 `all` / `总览` / `全部` 参数 查看全学生角评一图流\n"
-                    " \n"
-                    "可以用这些指令触发：\n"
-                    "- <ft color=(238,120,0)>ba学生评价</ft>\n"
-                    "- <ft color=(238,120,0)>ba角评</ft>\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba学生评价 白子</ft>\n"
-                    "- <ft color=(238,120,0)>ba角评 xcw</ft>"
-                    "- <ft color=(238,120,0)>ba角评 总览</ft>"
-                ),
-            },
-            {
-                "func": "总力战一图流",
-                "trigger_method": "指令",
-                "trigger_condition": "ba总力战",
-                "brief_des": "查询总力战推荐配队/Boss机制",
-                "detail_des": (
-                    "发送当前或指定总力战Boss的配队/机制一图流攻略图\n"
-                    "支持部分Boss别名\n"
-                    "图片作者 B站@夜猫咪喵喵猫\n"
-                    " \n"
-                    "使用 <ft color=(238,120,0)>ba总力战 -h</ft> 查询指令用法\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba总力战</ft>（日服&国际服当前总力战Boss配队攻略）\n"
-                    "- <ft color=(238,120,0)>ba总力战 -s j</ft>（日服当前总力战Boss配队攻略）\n"
-                    "- <ft color=(238,120,0)>ba总力战 -s j -w</ft>（日服当前总力战Boss机制图）\n"
-                    "- <ft color=(238,120,0)>ba总力战 寿司</ft>（Kaiten FX Mk.0 配队攻略）\n"
-                    "- <ft color=(238,120,0)>ba总力战 寿司 -t 屋外</ft>（Kaiten FX Mk.0 屋外战配队攻略）\n"
-                ),
-            },
-            {
-                "func": "活动一图流",
-                "trigger_method": "指令",
-                "trigger_condition": "ba活动",
-                "brief_des": "查询活动攻略图",
-                "detail_des": (
-                    "发送当前或指定活动一图流攻略图，可能会附带活动特殊机制等\n"
-                    "图片作者 B站@夜猫咪喵喵猫\n"
-                    " \n"
-                    "指令默认发送日服和国际服当前的活动攻略\n"
-                    "指令后面跟`日`或`j`开头的文本代表查询日服当前活动攻略，带以`国`或`g`开头的文本同理\n"
-                    "跟其他文本则代表指定活动名称\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba活动</ft>\n"
-                    "- <ft color=(238,120,0)>ba活动 日</ft>\n"
-                    "- <ft color=(238,120,0)>ba活动 温泉浴场</ft>"
-                ),
-            },
-            {
-                "func": "综合战术考试一图流",
-                "trigger_method": "指令",
-                "trigger_condition": "ba综合战术考试",
-                "brief_des": "查询综合战术考试攻略图",
-                "detail_des": (
-                    "发送当前或指定综合战术考试一图流攻略图\n"
-                    "图片作者 B站@夜猫咪喵喵猫\n"
-                    " \n"
-                    "指令默认发送日服和国际服当前的综合战术考试攻略\n"
-                    "指令后面跟`日`或`j`开头的文本代表查询日服当前综合战术考试攻略，带以`国`或`g`开头的文本同理\n"
-                    "跟整数则代表指定第几个综合战术考试\n"
-                    " \n"
-                    "p.s. 综合战术考试 和 合同火力演习 其实是一个东西，国际服叫前者，日服叫后者～\n"
-                    " \n"
-                    "可以用这些指令触发：\n"
-                    "- <ft color=(238,120,0)>ba综合战术考试</ft>\n"
-                    "- <ft color=(238,120,0)>ba合同火力演习</ft>\n"
-                    "- <ft color=(238,120,0)>ba战术考试</ft>\n"
-                    "- <ft color=(238,120,0)>ba火力演习</ft>\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba综合战术考试</ft>\n"
-                    "- <ft color=(238,120,0)>ba综合战术考试 日</ft>\n"
-                    "- <ft color=(238,120,0)>ba综合战术考试 8</ft>"
-                ),
-            },
-            {
-                "func": "制造一图流",
-                "trigger_method": "指令",
-                "trigger_condition": "ba制造",
-                "brief_des": "查询制造功能机制图",
-                "detail_des": (
-                    "发送游戏内制造功能的一图流介绍\n"
-                    "图片作者 B站@夜猫咪喵喵猫\n"
-                    " \n"
-                    "可以用这些指令触发：\n"
-                    "- <ft color=(238,120,0)>ba制造</ft>\n"
-                    "- <ft color=(238,120,0)>ba制作</ft>\n"
-                    "- <ft color=(238,120,0)>ba合成</ft>\n"
-                ),
-            },
-            {
-                "func": "国际服千里眼",
-                "trigger_method": "指令",
-                "trigger_condition": "ba千里眼",
-                "brief_des": "查询国际服未来的卡池与活动",
-                "detail_des": (
-                    "发送当前或指定日期的国际服未来卡池与活动列表\n"
-                    "图片作者 B站@夜猫咪喵喵猫\n"
-                    " \n"
-                    "参数可以指定起始日期以及列表个数，但同时指定时请将日期放在列表个数前面，以空格分隔\n"
-                    "参数中含有`全`或`a`时会发送整张前瞻图\n"
-                    " \n"
-                    "日期格式可以为（Y代表4位数年，m代表月，d代表日）：\n"
-                    "- <ft color=(238,120,0)>Y/m/d</ft>；<ft color=(238,120,0)>m/d</ft>\n"
-                    "- <ft color=(238,120,0)>Y-m-d</ft>；<ft color=(238,120,0)>m-d</ft>\n"
-                    "- <ft color=(238,120,0)>Y年m月d日</ft>；<ft color=(238,120,0)>m月d日</ft>\n"
-                    " \n"
-                    "可以用这些指令触发：\n"
-                    "- <ft color=(238,120,0)>ba国际服千里眼</ft>\n"
-                    "- <ft color=(238,120,0)>ba千里眼</ft>\n"
-                    "- <ft color=(238,120,0)>ba国际服前瞻</ft>\n"
-                    "- <ft color=(238,120,0)>ba前瞻</ft>\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba千里眼</ft>\n"
-                    "- <ft color=(238,120,0)>ba千里眼 all</ft>\n"
-                    "- <ft color=(238,120,0)>ba千里眼 3</ft>\n"
-                    "- <ft color=(238,120,0)>ba千里眼 11/15</ft>\n"
-                    "- <ft color=(238,120,0)>ba千里眼 11/15 3</ft>"
-                ),
-            },
-            {
-                "func": "学生语音",
-                "trigger_method": "指令",
-                "trigger_condition": "ba语音",
-                "brief_des": "发送学生语音",
-                "detail_des": (
-                    "从GameKee爬取学生语音并发送\n"
-                    "指定关键词时会从匹配结果中随机选择一个语音发送\n"
-                    " \n"
-                    "可以用这些指令触发：\n"
-                    "- <ft color=(238,120,0)>ba语音</ft>\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba语音 忧</ft>\n"
-                    "- <ft color=(238,120,0)>ba语音 美游 被cc</ft>"
-                ),
-            },
-            {
-                "func": "互动家具总览",
-                "trigger_method": "指令",
-                "trigger_condition": "ba互动家具",
-                "brief_des": "查询互动家具总览图",
-                "detail_des": "发送咖啡厅内所有互动家具以及对应学生的总览图\n图片作者 B站@夜猫咪喵喵猫",
-            },
-            {
-                "func": "模拟抽卡",
-                "trigger_method": "指令",
-                "trigger_condition": "ba抽卡",
-                "brief_des": "模拟抽卡",
-                "detail_des": (
-                    "模拟抽卡\n"
-                    "可以使用 <ft color=(238,120,0)>ba切换卡池</ft> 指令来切换卡池\n"
-                    "可以指定抽卡次数，需要在1~90之间，默认10\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba抽卡</ft>\n"
-                    "- <ft color=(238,120,0)>ba抽卡 20</ft>"
-                ),
-            },
-            {
-                "func": "切换卡池",
-                "trigger_method": "指令",
-                "trigger_condition": "ba切换卡池",
-                "brief_des": "设置模拟抽卡的UP池",
-                "detail_des": (
-                    "设置模拟抽卡功能的UP池角色\n"
-                    "默认从当前数据源UP池中轮流切换\n"
-                    "当参数为 <ft color=(238,120,0)>常驻</ft> 时，切换到常驻池（没有UP）\n"
-                    "可以自定义池子UP角色，支持2星与3星角色，参数中学生名称用空格分隔，支持部分学生别名\n"
-                    " \n"
-                    "指令示例：\n"
-                    "- <ft color=(238,120,0)>ba切换卡池</ft>\n"
-                    "- <ft color=(238,120,0)>ba切换卡池 常驻</ft>"
-                    "- <ft color=(238,120,0)>ba切换卡池 小桃 小绿</ft>"
-                ),
-            },
-            {
-                "func": "抽表情",
-                "trigger_method": "指令",
-                "trigger_condition": "ba表情",
-                "brief_des": "随机发送一个国际服社团聊天表情",
-                "detail_des": "随机发送一个国际服社团聊天表情\n来源：解包",
-            },
-            {
-                "func": "随机漫画",
-                "trigger_method": "指令",
-                "trigger_condition": "ba漫画",
-                "brief_des": "随机发送一话官推漫画",
-                "detail_des": "随机发送一话BA官推漫画\n来源：GameKee",
-            },
-            {
-                "func": "清空缓存",
-                "trigger_method": "超级用户 指令",
-                "trigger_condition": "ba清空缓存",
-                "brief_des": "清空插件请求缓存",
-                "detail_des": (
-                    "手动清空插件请求网络缓存下来的数据（正常3小时清空一次）\n"
-                    "如果插件出问题了，或者你想提前看到新内容，不妨试试清空一下插件缓存\n"
-                    "注：该指令只能由<ft color=(238,120,0)>超级用户</ft>触发\n"
-                    " \n"
-                    "可以用这些指令触发：\n"
-                    "- <ft color=(238,120,0)>ba清空缓存</ft>\n"
-                    "- <ft color=(238,120,0)>ba清除缓存</ft>"
-                ),
-            },
-        ],
-    },
+    usage="感谢各位 sensei 使用本插件！装载 PicMenu 插件即可查看插件详细菜单哦\n祝玩得愉快～",
+    homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-bawiki",
+    type="application",
+    config=Cfg,
+    supported_adapters=["~onebot.v11"],
+    extra={"License": "MIT", "Author": "student_2333"},
 )
+
+extra_pic_menu = {
+    "menu_template": "default",
+    "menu_data": [
+        {
+            "func": "日程表",
+            "trigger_method": "指令",
+            "trigger_condition": "ba日程表",
+            "brief_des": "查看活动日程表",
+            "detail_des": (
+                "查看当前未结束的卡池、活动以及起止时间，"
+                "默认为GameKee源，可以在指令后带参数使用SchaleDB数据源\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba日程表</ft> （GameKee源）\n"
+                "- <ft color=(238,120,0)>ba日程表 schaledb</ft> （SchaleDB源，日服国际服一起发）\n"
+                "- <ft color=(238,120,0)>ba日程表 schale 国际服</ft> （SchaleDB源，国际服）"
+            ),
+        },
+        {
+            "func": "学生图鉴",
+            "trigger_method": "指令",
+            "trigger_condition": "ba学生图鉴",
+            "brief_des": "查询学生详情（SchaleDB）",
+            "detail_des": (
+                "访问对应学生SchaleDB页面并截图，支持部分学生别名\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba学生图鉴 白子</ft>\n"
+                "- <ft color=(238,120,0)>ba学生图鉴 xcw</ft>"
+            ),
+        },
+        {
+            "func": "学生Wiki",
+            "trigger_method": "指令",
+            "trigger_condition": "ba学生wiki",
+            "brief_des": "查询学生详情（GameKee）",
+            "detail_des": (
+                "访问对应学生GameKee Wiki页面并截图，支持部分学生别名\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba学生wiki 白子</ft>\n"
+                "- <ft color=(238,120,0)>ba学生wiki xcw</ft>"
+            ),
+        },
+        {
+            "func": "羁绊查询",
+            "trigger_method": "指令",
+            "trigger_condition": "ba羁绊",
+            "brief_des": "查询学生解锁L2D需求的羁绊等级",
+            "detail_des": (
+                "使用学生名称查询该学生解锁L2D看板需求的羁绊等级以及L2D预览，"
+                "或者使用羁绊等级级数查询哪些学生达到该等级时解锁L2D看板\n"
+                "使用学生名称查询时支持部分学生别名\n"
+                " \n"
+                "可以用这些指令触发：\n"
+                "- <ft color=(238,120,0)>ba羁绊</ft>\n"
+                "- <ft color=(238,120,0)>ba好感度</ft>\n"
+                "- <ft color=(238,120,0)>bal2d</ft>\n"
+                "- <ft color=(238,120,0)>balive2d</ft>\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba羁绊 xcw</ft>\n"
+                "- <ft color=(238,120,0)>ba羁绊 9</ft>"
+            ),
+        },
+        {
+            "func": "角色评价",
+            "trigger_method": "指令",
+            "trigger_condition": "ba角评",
+            "brief_des": "查询学生角评一图流",
+            "detail_des": (
+                "发送一张指定角色的评价图\n"
+                "支持部分学生别名\n"
+                "角评图作者 B站@夜猫咪喵喵猫\n"
+                " \n"
+                "可以使用 `all` / `总览` / `全部` 参数 查看全学生角评一图流\n"
+                " \n"
+                "可以用这些指令触发：\n"
+                "- <ft color=(238,120,0)>ba学生评价</ft>\n"
+                "- <ft color=(238,120,0)>ba角评</ft>\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba学生评价 白子</ft>\n"
+                "- <ft color=(238,120,0)>ba角评 xcw</ft>"
+                "- <ft color=(238,120,0)>ba角评 总览</ft>"
+            ),
+        },
+        {
+            "func": "总力战一图流",
+            "trigger_method": "指令",
+            "trigger_condition": "ba总力战",
+            "brief_des": "查询总力战推荐配队/Boss机制",
+            "detail_des": (
+                "发送当前或指定总力战Boss的配队/机制一图流攻略图\n"
+                "支持部分Boss别名\n"
+                "图片作者 B站@夜猫咪喵喵猫\n"
+                " \n"
+                "使用 <ft color=(238,120,0)>ba总力战 -h</ft> 查询指令用法\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba总力战</ft>（日服&国际服当前总力战Boss配队攻略）\n"
+                "- <ft color=(238,120,0)>ba总力战 -s j</ft>（日服当前总力战Boss配队攻略）\n"
+                "- <ft color=(238,120,0)>ba总力战 -s j -w</ft>（日服当前总力战Boss机制图）\n"
+                "- <ft color=(238,120,0)>ba总力战 寿司</ft>（Kaiten FX Mk.0 配队攻略）\n"
+                "- <ft color=(238,120,0)>ba总力战 寿司 -t 屋外</ft>（Kaiten FX Mk.0 屋外战配队攻略）\n"
+            ),
+        },
+        {
+            "func": "活动一图流",
+            "trigger_method": "指令",
+            "trigger_condition": "ba活动",
+            "brief_des": "查询活动攻略图",
+            "detail_des": (
+                "发送当前或指定活动一图流攻略图，可能会附带活动特殊机制等\n"
+                "图片作者 B站@夜猫咪喵喵猫\n"
+                " \n"
+                "指令默认发送日服和国际服当前的活动攻略\n"
+                "指令后面跟`日`或`j`开头的文本代表查询日服当前活动攻略，带以`国`或`g`开头的文本同理\n"
+                "跟其他文本则代表指定活动名称\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba活动</ft>\n"
+                "- <ft color=(238,120,0)>ba活动 日</ft>\n"
+                "- <ft color=(238,120,0)>ba活动 温泉浴场</ft>"
+            ),
+        },
+        {
+            "func": "综合战术考试一图流",
+            "trigger_method": "指令",
+            "trigger_condition": "ba综合战术考试",
+            "brief_des": "查询综合战术考试攻略图",
+            "detail_des": (
+                "发送当前或指定综合战术考试一图流攻略图\n"
+                "图片作者 B站@夜猫咪喵喵猫\n"
+                " \n"
+                "指令默认发送日服和国际服当前的综合战术考试攻略\n"
+                "指令后面跟`日`或`j`开头的文本代表查询日服当前综合战术考试攻略，带以`国`或`g`开头的文本同理\n"
+                "跟整数则代表指定第几个综合战术考试\n"
+                " \n"
+                "p.s. 综合战术考试 和 合同火力演习 其实是一个东西，国际服叫前者，日服叫后者～\n"
+                " \n"
+                "可以用这些指令触发：\n"
+                "- <ft color=(238,120,0)>ba综合战术考试</ft>\n"
+                "- <ft color=(238,120,0)>ba合同火力演习</ft>\n"
+                "- <ft color=(238,120,0)>ba战术考试</ft>\n"
+                "- <ft color=(238,120,0)>ba火力演习</ft>\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba综合战术考试</ft>\n"
+                "- <ft color=(238,120,0)>ba综合战术考试 日</ft>\n"
+                "- <ft color=(238,120,0)>ba综合战术考试 8</ft>"
+            ),
+        },
+        {
+            "func": "制造一图流",
+            "trigger_method": "指令",
+            "trigger_condition": "ba制造",
+            "brief_des": "查询制造功能机制图",
+            "detail_des": (
+                "发送游戏内制造功能的一图流介绍\n"
+                "图片作者 B站@夜猫咪喵喵猫\n"
+                " \n"
+                "可以用这些指令触发：\n"
+                "- <ft color=(238,120,0)>ba制造</ft>\n"
+                "- <ft color=(238,120,0)>ba制作</ft>\n"
+                "- <ft color=(238,120,0)>ba合成</ft>\n"
+            ),
+        },
+        {
+            "func": "国际服千里眼",
+            "trigger_method": "指令",
+            "trigger_condition": "ba千里眼",
+            "brief_des": "查询国际服未来的卡池与活动",
+            "detail_des": (
+                "发送当前或指定日期的国际服未来卡池与活动列表\n"
+                "图片作者 B站@夜猫咪喵喵猫\n"
+                " \n"
+                "参数可以指定起始日期以及列表个数，但同时指定时请将日期放在列表个数前面，以空格分隔\n"
+                "参数中含有`全`或`a`时会发送整张前瞻图\n"
+                " \n"
+                "日期格式可以为（Y代表4位数年，m代表月，d代表日）：\n"
+                "- <ft color=(238,120,0)>Y/m/d</ft>；<ft color=(238,120,0)>m/d</ft>\n"
+                "- <ft color=(238,120,0)>Y-m-d</ft>；<ft color=(238,120,0)>m-d</ft>\n"
+                "- <ft color=(238,120,0)>Y年m月d日</ft>；<ft color=(238,120,0)>m月d日</ft>\n"
+                " \n"
+                "可以用这些指令触发：\n"
+                "- <ft color=(238,120,0)>ba国际服千里眼</ft>\n"
+                "- <ft color=(238,120,0)>ba千里眼</ft>\n"
+                "- <ft color=(238,120,0)>ba国际服前瞻</ft>\n"
+                "- <ft color=(238,120,0)>ba前瞻</ft>\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba千里眼</ft>\n"
+                "- <ft color=(238,120,0)>ba千里眼 all</ft>\n"
+                "- <ft color=(238,120,0)>ba千里眼 3</ft>\n"
+                "- <ft color=(238,120,0)>ba千里眼 11/15</ft>\n"
+                "- <ft color=(238,120,0)>ba千里眼 11/15 3</ft>"
+            ),
+        },
+        {
+            "func": "学生语音",
+            "trigger_method": "指令",
+            "trigger_condition": "ba语音",
+            "brief_des": "发送学生语音",
+            "detail_des": (
+                "从GameKee爬取学生语音并发送\n"
+                "指定关键词时会从匹配结果中随机选择一个语音发送\n"
+                " \n"
+                "可以用这些指令触发：\n"
+                "- <ft color=(238,120,0)>ba语音</ft>\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba语音 忧</ft>\n"
+                "- <ft color=(238,120,0)>ba语音 美游 被cc</ft>"
+            ),
+        },
+        {
+            "func": "互动家具总览",
+            "trigger_method": "指令",
+            "trigger_condition": "ba互动家具",
+            "brief_des": "查询互动家具总览图",
+            "detail_des": "发送咖啡厅内所有互动家具以及对应学生的总览图\n图片作者 B站@夜猫咪喵喵猫",
+        },
+        {
+            "func": "模拟抽卡",
+            "trigger_method": "指令",
+            "trigger_condition": "ba抽卡",
+            "brief_des": "模拟抽卡",
+            "detail_des": (
+                "模拟抽卡\n"
+                "可以使用 <ft color=(238,120,0)>ba切换卡池</ft> 指令来切换卡池\n"
+                "可以指定抽卡次数，需要在1~90之间，默认10\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba抽卡</ft>\n"
+                "- <ft color=(238,120,0)>ba抽卡 20</ft>"
+            ),
+        },
+        {
+            "func": "切换卡池",
+            "trigger_method": "指令",
+            "trigger_condition": "ba切换卡池",
+            "brief_des": "设置模拟抽卡的UP池",
+            "detail_des": (
+                "设置模拟抽卡功能的UP池角色\n"
+                "默认从当前数据源UP池中轮流切换\n"
+                "当参数为 <ft color=(238,120,0)>常驻</ft> 时，切换到常驻池（没有UP）\n"
+                "可以自定义池子UP角色，支持2星与3星角色，参数中学生名称用空格分隔，支持部分学生别名\n"
+                " \n"
+                "指令示例：\n"
+                "- <ft color=(238,120,0)>ba切换卡池</ft>\n"
+                "- <ft color=(238,120,0)>ba切换卡池 常驻</ft>"
+                "- <ft color=(238,120,0)>ba切换卡池 小桃 小绿</ft>"
+            ),
+        },
+        {
+            "func": "抽表情",
+            "trigger_method": "指令",
+            "trigger_condition": "ba表情",
+            "brief_des": "随机发送一个国际服社团聊天表情",
+            "detail_des": "随机发送一个国际服社团聊天表情\n来源：解包",
+        },
+        {
+            "func": "随机漫画",
+            "trigger_method": "指令",
+            "trigger_condition": "ba漫画",
+            "brief_des": "随机发送一话官推漫画",
+            "detail_des": "随机发送一话BA官推漫画\n来源：GameKee",
+        },
+        {
+            "func": "清空缓存",
+            "trigger_method": "超级用户 指令",
+            "trigger_condition": "ba清空缓存",
+            "brief_des": "清空插件请求缓存",
+            "detail_des": (
+                "手动清空插件请求网络缓存下来的数据（正常3小时清空一次）\n"
+                "如果插件出问题了，或者你想提前看到新内容，不妨试试清空一下插件缓存\n"
+                "注：该指令只能由<ft color=(238,120,0)>超级用户</ft>触发\n"
+                " \n"
+                "可以用这些指令触发：\n"
+                "- <ft color=(238,120,0)>ba清空缓存</ft>\n"
+                "- <ft color=(238,120,0)>ba清除缓存</ft>"
+            ),
+        },
+    ],
+}
+
+if "nonebot_plugin_PicMenu" in get_available_plugin_names():
+    __plugin_meta__.extra.update(extra_pic_menu)
```

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/__main__.py` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/config.py` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_bawiki.py` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_bawiki.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_gamekee.py` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_gamekee.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_schaledb.py` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/data_schaledb.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/gacha.py` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/calender_banner.png` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_new.png` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_star.png` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gradient.png` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/resource.py` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/resource.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.7.8/nonebot_plugin_bawiki/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.7/pyproject.toml` & `nonebot_plugin_bawiki-0.7.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "nonebot-plugin-bawiki"
-version = "0.7.7"
+version = "0.7.8"
 description = "A nonebot2 plugin for Blue Archive."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.3",
-    "nonebot2>=2.0.0b5",
+    "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.1",
     "nonebot-plugin-htmlrender>=0.2.0.1",
     "nonebot-plugin-apscheduler>=0.2.0",
     "beautifulsoup4>=4.11.1",
     "lxml>=4.9.1",
     "pil-utils>=0.1.4",
 ]
```

### Comparing `nonebot_plugin_bawiki-0.7.7/PKG-INFO` & `nonebot_plugin_bawiki-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.7.7
+Version: 0.7.8
 Summary: A nonebot2 plugin for Blue Archive.
 Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications
@@ -17,15 +17,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki
 Project-URL: Homepage, https://github.com/lgc2333/nonebot-plugin-bawiki/
 Requires-Python: <4.0,>=3.8
 Requires-Dist: aiohttp>=3.8.3
-Requires-Dist: nonebot2>=2.0.0b5
+Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-adapter-onebot>=2.1.1
 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.1
 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0
 Requires-Dist: beautifulsoup4>=4.11.1
 Requires-Dist: lxml>=4.9.1
 Requires-Dist: pil-utils>=0.1.4
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.7 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.8 Summary: A
 nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
 qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
 student_2333
 126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy Classifier:
 Topic :: Games/Entertainment :: Side-Scrolling/Arcade Games Classifier: Topic
 :: Internet Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
 Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Internet :: WWW/
 HTTP :: Dynamic Content :: Wiki Project-URL: Homepage, https://github.com/
 lgc2333/nonebot-plugin-bawiki/ Requires-Python: <4.0,>=3.8 Requires-Dist:
-aiohttp>=3.8.3 Requires-Dist: nonebot2>=2.0.0b5 Requires-Dist: nonebot-adapter-
+aiohttp>=3.8.3 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-
 onebot>=2.1.1 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.1 Requires-Dist:
 nonebot-plugin-apscheduler>=0.2.0 Requires-Dist: beautifulsoup4>=4.11.1
 Requires-Dist: lxml>=4.9.1 Requires-Dist: pil-utils>=0.1.4 Description-Content-
 Type: text/markdown
                                    [BAWiki]
 # NoneBot-Plugin-BAWiki _â¨ åºäº NoneBot2 çç¢§èæ¡£æ¡ Wiki æä»¶ â¨_
              [license] [pypi] [python] [pypi_download] [wakatime]
```

