# Comparing `tmp/nonebot_plugin_game_collection-2.1.3.tar.gz` & `tmp/nonebot_plugin_game_collection-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.1.3.tar", last modified: Sat Apr 29 02:55:17 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.1.4.tar", last modified: Sun Jun  4 12:20:32 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.1.3.tar` & `nonebot_plugin_game_collection-2.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.878164 nonebot_plugin_game_collection-2.1.3/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.3/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-04-29 02:55:17.877663 nonebot_plugin_game_collection-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.822116 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    41103 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.838130 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    11367 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    20097 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    13471 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    28768 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/config.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.843634 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/
--rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/api.py
--rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/data.py
--rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/run.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.848639 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.868156 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12610 2023-04-29 02:52:46.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     4949 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.871157 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.876163 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 02:55:17.831624 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-04-29 02:55:17.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2038 2023-04-29 02:55:17.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 02:55:17.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-29 02:55:17.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-04-29 02:55:17.000000 nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 02:55:17.878164 nonebot_plugin_game_collection-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-04-29 02:55:13.000000 nonebot_plugin_game_collection-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.855719 nonebot_plugin_game_collection-2.1.4/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.4/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-04 12:20:32.855219 nonebot_plugin_game_collection-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.795169 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    48705 2023-06-04 12:18:21.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.813685 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    11391 2023-06-04 09:46:42.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    20138 2023-06-04 11:54:55.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    16202 2023-06-04 11:51:18.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    30093 2023-06-04 08:55:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/config.py
+drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.818189 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/
+-rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/api.py
+-rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/data.py
+-rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/run.py
+drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.824695 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.845210 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5375 2023-06-04 11:46:30.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.846711 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.853718 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.804677 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-04 12:20:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-06-04 12:20:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 12:20:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-04 12:20:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-04 12:20:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 12:20:32.856220 nonebot_plugin_game_collection-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-06-04 12:20:29.000000 nonebot_plugin_game_collection-2.1.4/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.1.3/LICENSE` & `nonebot_plugin_game_collection-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/README.md` & `nonebot_plugin_game_collection-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Account.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Game.py`

 * *Files 10% similar despite different names*

```diff
@@ -331,15 +331,15 @@
             return "这场对决邀请已经过时了，请重新发起决斗..."
         user_id = event.user_id
         if self.player1_id and self.player1_id != user_id and not self.next:
             if not self.at or self.at == user_id: 
                 self.time = time.time()
                 self.player2_id = user_id
             else:
-                return f'现在是 {user_data[self.player2_id].group_accounts[event.group_id].nickname} 发起的对决，请等待比赛结束后再开始下一轮...'
+                return f'现在是 {user_data[self.player1_id].group_accounts[event.group_id].nickname} 发起的对决，请等待比赛结束后再开始下一轮...'
         else:
             return " "
     def nextround(self):
         """
         把session状态切换到下一回合
         """
         self.time = time.time()
@@ -410,32 +410,48 @@
     elif game == "dice":
         gold = session.info["max_gold"]
         tip1 = "本场对决为【掷色子】\n"
         tip2 = "开数！"
     elif game == "poker":
         gold = session.gold
         tip1 = "本场对决为【扑克对战】\n"
-        tip2 = "出牌！\n"
+        tip2 = "加注！\n"
         tip2 += MessageSegment.image(text_to_png(
             "P1初始状态\n"
             f'HP {session.info["P1"]["HP"]} SP {session.info["P1"]["SP"]} DEF {session.info["P1"]["DEF"]}\n'
             "——————————————\n"
             "P2初始状态\n"
             f'HP {session.info["P2"]["HP"]} SP {session.info["P2"]["SP"]} DEF {session.info["P2"]["DEF"]}\n'
             "——————————————\n"
             "P1初始手牌\n" + 
             "".join([f'【{pokerACT.suit[suit]}{pokerACT.point[point]}】' for suit, point in session.info["P1"]["hand"]])
             ),30)
     elif game == "lucky_number":
         gold = session.gold
         tip1 = "本场对决为【猜数字】\n"
         tip2 = "发送数字"
+    elif game == "cantrell":
+        gold = session.gold
+        tip1 = "本场对决为【港式五张】\n"
+        tip2 = "开牌！\n"
+        tip2 += MessageSegment.image(text_to_png(
+                "P1初始手牌：\n"
+                "|"
+                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"][0:3]]) +
+                "   |   |"
+                "\n——————————————\n"
+                'P2初始手牌\n'
+                "|"
+                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand2"][0:3]]) +
+                "   |   |"
+                ),30)
     else:
         gold = session.gold
         tip1 = ""
+        tip2 = ""
     return Message(
         f"{MessageSegment.at(session.player2_id)}接受了对决！\n" +
         tip1 +
         f"赌注为 {gold} 金币\n" +
         f"请{MessageSegment.at(session.player1_id)}{tip2}"
         )
 
@@ -968,19 +984,19 @@
     """
     flag, msg = start(event, gold)
     if flag == False:
         return msg
     session = current_games[event.group_id]
     session.gold = gold
     session.info = lucky_number_info(gold)
-    return (f"随机 1-100 数字已生成。"
+    return (f"随机牌堆已生成。"
             f"挑战金额：{gold}/次\n"
             f"{msg}")
 
-async def guess_number(bot:Bot, event:GroupMessageEvent, N:int):
+async def check_card(bot:Bot, event:GroupMessageEvent, N:int):
     """
     猜数字
     """
     group_id = event.group_id
     global current_games
     session = current_games[group_id]
     if msg := session.shot_check(event):
@@ -994,14 +1010,188 @@
     if N > TrueN:
         return f"{N}比这个数字大\n金额：{session.gold}"
     if N < TrueN:
         return f"{N}比这个数字小\n金额：{session.gold}"
     session.win = event.user_id
     await end(bot, event)
 
+"""+++++++++++++++++
+——————————
+       梭哈
+——————————
++++++++++++++++++"""
+
+def cantrell_info(gold):
+    """
+    生成港式五张游戏内容
+    """
+    deck = random_poker()
+    return {
+        "game":"cantrell",
+        "round_gold":gold,
+        "hand1":deck[0:5],
+        "pt1":cantrell_pt(deck[0:5]),
+        "hand2":deck[5:10],
+        "pt2":cantrell_pt(deck[5:10])
+        }
+
+def cantrell(event:GroupMessageEvent, gold:int):
+    """
+    发起游戏：港式五张
+    """
+    flag, msg = start(event, gold, max_bet_gold * 10)
+    if flag == False:
+        return msg
+    session = current_games[event.group_id]
+    session.gold = gold
+    session.info = cantrell_info(gold)
+    return (f"随机牌堆已生成\n"
+            f"开局金额：{gold}\n"
+            f"{msg}")
+
+cantrell_suit = {1:"♠",2:"♥",3:"♣",4:"♦"}
+cantrell_point = {1:"2",2:"3",3:"4",4:"5",5:"6",6:"7",7:"8",8:"9",9:"10",10:"J",11:"Q",12:"K",13:"A"}
+
+async def cantrell_check(bot:Bot, event:GroupMessageEvent):
+    """
+    看牌
+    """
+    group_id = event.group_id
+    global current_games
+    session = current_games[group_id]
+    if msg := session.shot_check(event):
+        return None if msg == " " else msg
+    expose = int(round((session.round  + 0.5)/ 2)) + 3
+    expose = expose if expose < 5 else 5
+    if event.user_id == session.player1_id:
+        hand = "hand1"
+    else:
+        hand = "hand2"
+    msg = (
+        "你的手牌：\n"
+        + ("|" + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info[hand][0:expose]]) + (5 - expose)*"   |")
+        )
+    await bot.send_private_msg(user_id = event.user_id, message = MessageSegment.image(text_to_png(msg,30)))
+    return
+
+def is_straight(points):
+    """
+    判断是否为顺子
+    """
+    points = sorted(points)
+    for i in range(1, len(points)):
+        if points[i] - points[i-1] != 1:
+            return False
+    return True
+
+def cantrell_pt(hand:list) -> Tuple[int,str]:
+    """
+    牌型点数
+    """
+    pt = 0
+    name = ""
+
+    suits = [x[0] for x in hand]
+    points = [x[1] for x in hand]
+
+    setpoints = set(points)
+
+    # 判断同花
+    if len(set(suits)) == 1:
+        pt += suits[0]
+        if is_straight(points):
+            point = max(points)
+            pt += point * (100**9)
+            name += f"同花顺{cantrell_suit[suits[0]]}{cantrell_point[point]} "
+        else:
+            point = sum(points)
+            pt += point * (100**6)
+            name += f"同花{cantrell_suit[suits[0]]}{cantrell_point[point]} "
+    else:
+        pt += sum(suits)
+        # 判断顺子
+        if is_straight(points):
+            point = max(points)
+            pt += point * (100**5)
+            name += f"顺子{cantrell_point[point]} "
+        else:
+            # 判断四条或葫芦
+            if len(setpoints) == 2:
+                for point in setpoints:
+                    if points.count(point) == 4:
+                        pt += point * (100**8)
+                        name += f"四条{cantrell_point[point]} "
+                    if points.count(point) == 3:
+                        pt += point * (100**7)
+                        name += f"葫芦{cantrell_point[point]} "
+            else:
+                # 判断三条，两对，一对
+                exp = 1
+                tmp = 0
+                for point in setpoints:
+                    if points.count(point) == 3:
+                        pt += point * (100**4)
+                        name += f"三条{cantrell_point[point]} "
+                        break
+                    if points.count(point) == 2:
+                        exp += 1
+                        tmp += point
+                        name += f"对{cantrell_point[point]} "
+                else:
+                    pt += tmp * (100**exp)
+
+            for point in setpoints:
+                if points.count(point) == 1:
+                    pt += point * (100)
+                    name += f"散{cantrell_point[point]} "
+
+    return pt,name[:-1]
+
+async def cantrell_play(bot:Bot, event:GroupMessageEvent, gold:int, max_bet_gold:int = max_bet_gold * 10):
+    """
+    加注
+    """
+    group_id = event.group_id
+    global current_games
+    session = current_games[group_id]
+    if msg := session.shot_check(event):
+        return None if msg == " " else msg
+    expose = session.round / 2
+    if expose == int(expose):
+        session.nextround()
+        expose = int(expose) + 3
+        session.gold += session.info["round_gold"]
+        msg = (
+            f'玩家：{user_data[session.player1_id].group_accounts[group_id].nickname}\n'
+            "手牌：\n"
+            "|"
+            + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"][0:expose]]) + (5 - expose)*"   |"
+            "\n——————————————\n"
+            f'玩家：{user_data[session.player2_id].group_accounts[group_id].nickname}\n'
+            "手牌：\n"
+            "|"
+            + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand2"][0:expose]]) + (5 - expose)*"   |"
+            )
+        if expose == 5:
+            if session.info["pt1"][0] > session.info["pt2"][0]:
+                session.win = session.player1_id
+            else:
+                session.win = session.player2_id
+            await end(bot, event)
+        else:
+            return MessageSegment.image(text_to_png(f"您已跟注{session.info['round_gold']}金币\n" + msg,30))
+    else:
+        if gold > max_bet_gold:
+            return MessageSegment.at(event.user_id) + f"加注金额不能超过{max_bet_gold}"
+        group_account = Manager.locate_user(event)[1]
+        if gold + session.gold > group_account.gold:
+            return Message(MessageSegment.at(event.user_id) + f"你没有足够的金币。\n——你还有{group_account.gold - session.gold}枚金币。")
+        session.nextround()
+        session.info["round_gold"] = gold
+        return MessageSegment.at(event.user_id) + f"您已加注{gold}金币"
 
 """+++++++++++++++++
 ——————————
       随机对战
 ——————————
 +++++++++++++++++"""
 
@@ -1134,14 +1324,24 @@
     if game == "russian":
         return " ".join(("—" if x == 0 else "|") for x in session.info["bullet"])
     if game == "dice":
         return (f'玩家 1\n'
                 f'组合：{" ".join(str(x) for x in session.info["dice_array1"])}\n'
                 f'玩家 2\n'
                 f'组合：{" ".join(str(x) for x in session.info["dice_array2"])}')
+    if game == "cantrell":
+        return MessageSegment.image(text_to_png(("P1手牌：\n"
+                "|"
+                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand1"]]) +
+                f"\n牌型：\n{session.info['pt1'][1]}"
+                "\n——————————————\n"
+                "P2手牌：\n"
+                "|"
+                + "".join([f'{cantrell_suit[suit]}{cantrell_point[point]}|' for suit, point in session.info["hand2"]]) +
+                f"\n牌型：\n{session.info['pt2'][1]}"),30))
     else:
         return ""
 
 async def end(bot:Bot, event:GroupMessageEvent):
     """
     输出结算界面
     """
```

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
     return user,group_account
 
 def update_company_index(company_index):
     """
     从群数据生成公司名查找群号的字典
     """
+    company_index = {}
     for group_id in group_data:
         if company_name := group_data[group_id].company.company_name:
             company_index[company_name] = group_id
             company_index[str(group_id)] = group_id
 
 company_index:Dict[str,int] = {}
 update_company_index(company_index)
```

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Market.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     user = Manager.locate_user(event)[0]
     if user.props.get("33001",0) < 1:
         return f"你的【{props_library['33001']['name']}】已失效"
     if check := check_company_name(company_name):
         return check
     old_company_name = company.company_name
     company.company_name = company_name
+    update_company_index(company_index)
     return f'【{old_company_name}】已重命名为【{company_name}】'
 
 def value_update(group_account:GroupAccount):
     """
     刷新持股价值
     group_account:用户群账户
     """
```

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Prop.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     MessageSegment
     )
 import random
 
 from .utils.utils import get_message_at
 from .utils.chart import bbcode_to_png
 from .data.data import props_library, props_index, element_library
-from .config import bot_name, sign_gold, revolt_gold,max_bet_gold, gacha_gold
+from .config import bot_name, sign_gold, revolt_gold, max_bet_gold, gacha_gold
 
 from .Manager import data
 from . import Manager
 
 user_data = data.user
 group_data = data.group
 
@@ -41,14 +41,16 @@
         props = random.choice(["31001","32001","32002","33001","33101"])
     elif 30 < code <= 40:
         props = random.choice(["41001","42001","42101"])
     elif 40 < code <= 50:
         props = random.choice(["51001","51002","52001","52002","52101","52102"])
     elif code == 51:
         props = random.choice(["61001","62101"])
+    elif code == 52:
+        props = random.choice(["63101","63102"])
     else:
         props = "11001"
     return props
 
 def gacha(event:MessageEvent, N:int):
     """
     抽卡
@@ -111,14 +113,18 @@
             return self.use_42101(event)
         elif self == "52101":
             return self.use_52101(event)
         elif self == "52102":
             return self.use_52102(event,count)
         elif self == "53101":
             return self.use_53101(event,count)
+        elif self == "63101":
+            return self.use_63101(event)
+        elif self == "63102":
+            return self.use_63102(event)
         else:
             return f"【{props_library[self]['name']}】不是可用道具。"
 
     @classmethod
     def use_03100(cls, event:MessageEvent) -> str:
         """
         使用道具：测试金库
@@ -221,29 +227,30 @@
             user.gold -= gold
             group_account.gold -= gold
             target_user.gold += gold
             target_group_account.gold += gold
             info = f"调查没有发现问题。你赔偿了对方{gold}枚金币"
         else:
             gold = int(target_group_account.gold * N / 1000)
+            gold = group_account.gold if gold > group_account.gold else gold
             user.gold += gold
             group_account.gold += gold
             target_user.gold -= gold
             target_group_account.gold -= gold
-            info = f"你获得了{gold}枚金币\n"
-            stocks = group_account.stocks
-            target_stocks = target_group_account.stocks
-            for company_id, count in target_stocks.items():
-                if stock := int(count * N / 100):
-                    stocks.setdefault(company_id,0)
-                    stocks[company_id] += stock
-                    target_stocks[company_id] -= stock
-                    if at in (company := group_data[company_id].company):
-                        del company.exchange[at]
-                    info += f"{company.company_name}：{stock}\n"
+            info = f"你获得了{gold}枚金币"
+            #stocks = group_account.stocks
+            #target_stocks = target_group_account.stocks
+            #for company_id, count in target_stocks.items():
+            #    if stock := int(count * N / 100):
+            #        stocks.setdefault(company_id,0)
+            #        stocks[company_id] += stock
+            #        target_stocks[company_id] -= stock
+            #        if at in (company := group_data[company_id].company):
+            #            del company.exchange[at]
+            #        info += f"{company.company_name}：{stock}\n"
             info += f"（{N/10}%）" 
         return info
 
     @classmethod
     def use_52101(cls, event:MessageEvent,) -> str:
         """
         使用道具：神秘天平
@@ -257,46 +264,56 @@
 
         props["52101"] -= 1
         if props["52101"] < 1:
             del props["52101"]
 
         group_id = group_account.group_id
         ranklist = Manager.group_ranklist(group_id,"金币")
-        target_id = random.choice(ranklist[:20])[0]
+        target_id = random.choice([x[0] for x in ranklist if x[1] > revolt_gold[0]])
         if target_id == event.user_id:
             return f"道具使用失败，你损失了一个『{props_library['52101']['name']}』"
         target_user = user_data[target_id]
         target_group_account = target_user.group_accounts[group_id]
 
-        gold = int((group_account.gold + target_group_account.gold) / 2)
-        fee = int(gold / 20)
+        change = int((group_account.gold - target_group_account.gold) / 2)
+        limit = min((group_account.gold,target_group_account.gold))
+        if change > limit:
+            change = limit
+        if change < -limit:
+            change = -limit
+
+        abschange = abs(change)
+        fee = int(abschange / 20)
 
         flag = group_account.props.get("42001",0)
+        tag = "失去" if change > 0 else "获得"
         if flag > 0:
-            change = gold - group_account.gold
-            user.gold += change
-            group_account.gold += change
-            msg1 = f"\n你获得了{gold}金币『{props_library['42001']['name']}』。"
+            user.gold -= change
+            group_account.gold -= change
+            msg1 = f"\n你{tag}了{abschange}金币『{props_library['42001']['name']}』。"
         else:
-            change = gold - group_account.gold - fee
-            user.gold += change
-            group_account.gold += change
-            msg1 = f"\n你获得了{gold - fee}金币(扣除5%手续费：{fee})。"
+            user.gold -= change
+            user.gold -= fee
+            group_account.gold -= change
+            group_account.gold -= fee
+            msg1 = f"\n你{tag}了{abs(change + fee)}金币(扣除5%手续费：{fee})。"
 
         flag = target_group_account.props.get("42001",0)
+        tag = "失去" if change < 0 else "获得"
+
         if flag > 0:
-            change = gold - target_group_account.gold
             target_user.gold += change
             target_group_account.gold += change
-            msg2 = f"\n对方获得了{gold}金币『{props_library['42001']['name']}』。"
+            msg2 = f"\n对方{tag}了{abschange}金币『{props_library['42001']['name']}』。"
         else:
-            change = gold - target_group_account.gold - fee
             target_user.gold += change
+            target_user.gold -= fee
             target_group_account.gold += change
-            msg2 = f"\n对方获得了{gold - fee}金币(扣除5%手续费：{fee})。"
+            target_group_account.gold -= fee
+            msg2 = f"\n对方{tag}了{abs(change - fee)}金币(扣除5%手续费：{fee})。"
 
         return f"你与{target_group_account.nickname}平分了金币。" + msg1 + msg2
 
     @classmethod
     def use_52102(cls, event:MessageEvent, count:int,) -> str:
         """
         使用道具：幸运硬币
@@ -304,44 +321,48 @@
         user,group_account = Manager.locate_user(event)
         if not group_account:
             return "私聊未关联账户，请发送【关联账户】关联群内账户。"
         props = group_account.props
         if props.get("52102",0) < 1:
             return "数量不足"
 
-        gold = group_account.gold
-        if count == 1 or count == 2:
-            gold = int(gold/2)
-        if count == 2 or count == 4:
-            if props.get("62101",0) > 1:
+        if count == 1:
+            gold = int(group_account.gold/2)
+            X = 1
+        else:
+            if props.get("62101",0) > 0:
                 props["62101"] -= 1
                 if props["62101"] < 1:
                     del props["62101"]
             else:
                 return "钻石数量不足"
-        else:
-            gold = gold if gold < (limit := 50 * max_bet_gold) else limit
+            if count == 2:
+                gold = int(group_account.gold/2)
+                X = 2
+            else:
+                gold = group_account.gold
+                X = 1
+
+        gold = gold if gold < (limit := 50 * max_bet_gold) else limit
 
         props["52102"] -= 1
         if props["52102"] < 1:
             del props["52102"]
 
-        if random.randint(0,1) == 1:
+        if random.randint(0,X) > 0:
             user.gold += gold
             group_account.gold += gold
             return f"你获得了{gold}金币"
         else:
+            gold = int(group_account.gold/2)
             user.gold -= gold
             group_account.gold -= gold
-            if gold > group_account.gold:
-                user.props.setdefault("53101",0)
-                user.props["53101"] += 1
-                return f"你失去了{gold}金币。\n{bot_name}送你1个『{props_library['53101']['name']}』，祝你好运~"
-            else:
-                return f"你失去了{gold}金币。"
+            user.props.setdefault("53101",0)
+            user.props["53101"] += 1
+            return f"你失去了{gold}金币。\n{bot_name}送你1个『{props_library['53101']['name']}』，祝你好运~"
 
     @classmethod
     def use_53101(cls, event:MessageEvent, count:int) -> str:
         """
         使用道具：随机红包
         """
         user,group_account = Manager.locate_user(event)
@@ -357,12 +378,70 @@
 
         gold = random.randint(sign_gold[0] * count, revolt_gold[1] * count)
 
         user.gold += gold
         group_account.gold += gold
         return f"你获得了{gold}金币。祝你好运~"
 
+    @classmethod
+    def use_63101(cls, event:MessageEvent) -> str:
+        """
+        使用道具：超级幸运硬币
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = user.props
+        if props.get("63101",0) < 1:
+            return "数量不足"
+
+        props["63101"] -= 1
+        if props["63101"] < 1:
+            del props["63101"]
+
+        gold = group_account.gold
+
+        if random.randint(0,2) > 0:
+            user.gold += gold
+            group_account.gold += gold
+            return f"你获得了{gold}金币"
+        else:
+            user.gold -= gold
+            group_account.gold -= gold
+            user.props.setdefault("53101",0)
+            user.props["53101"] += 1
+            return f"你失去了{gold}金币。\n{bot_name}送你1个『{props_library['53101']['name']}』，祝你好运~"
+
+    @classmethod
+    def use_63102(cls, event:MessageEvent) -> str:
+        """
+        使用道具：重开券
+        """
+        user,group_account = Manager.locate_user(event)
+        if not group_account:
+            return "私聊未关联账户，请发送【关联账户】关联群内账户。"
+        props = user.props
+        if props.get("63102",0) < 1:
+            return "数量不足"
+
+        props["63102"] -= 1
+        if props["63102"] < 1:
+            del props["63102"]
+
+        group_id = group_account.group_id
+        user_id = user.user_id
+        for company_id in group_account.stocks:
+            company = group_data[company_id].company
+            company.stock += group_account.stocks[company_id]
+            exchange = company.exchange
+            if user_id in exchange:
+                del exchange[user_id]
+        user.gold -= group_account.gold
+        group_data[group_id].namelist.remove(user_id)
+        del group_account
+        return "本群账户已重置，祝你好运~"
+
 def use_prop(event:MessageEvent, prop_name:str, count:int):
     if prop_code := props_index.get(prop_name):
         return Prop(prop_code).use(event,count)
     else:
         return f"没有【{prop_name}】这种道具。"
```

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,18 +363,60 @@
     r"^\d{1,3}$",
     rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "lucky_number",
     permission = GROUP,
     priority = 20,
     block = True
     )
 
-@guess_number.handle()
+# 港式五张
+cantrell = on_command("同花顺",aliases = {"五张牌","港式五张","梭哈"}, permission = GROUP, priority = 20, block = True)
+
+@cantrell.handle()
+async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
+    gold = arg.extract_plain_text().strip()
+    if gold.isdigit():
+        gold = int(gold)
+    else:
+        gold = int(bet_gold)
+    msg = Game.cantrell(event, gold)
+    await cantrell.finish(msg)
+
+# 看牌
+cantrell_check = on_command(
+    "看牌",
+    rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "cantrell",
+    permission = GROUP,
+    priority = 20,
+    block = True
+    )
+
+@cantrell_check.handle()
 async def _(bot:Bot, event:GroupMessageEvent):
-    msg = await Game.guess_number(bot, event, int(event.get_plaintext()))
-    await guess_number.finish(msg)
+    msg = await Game.cantrell_check(bot, event)
+    await cantrell_check.finish(msg)
+
+# 加注
+cantrell_play = on_command(
+    "加注",
+    aliases = {"跟注","开牌"},
+    rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "cantrell",
+    permission = GROUP,
+    priority = 20,
+    block = True
+    )
+
+@cantrell_play.handle()
+async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
+    gold = arg.extract_plain_text().strip()
+    if gold.isdigit():
+        gold = int(gold)
+    else:
+        gold =  current_games[event.group_id].info["round_gold"]
+    msg = await Game.cantrell_play(bot, event, gold)
+    await cantrell_play.finish(msg)
 
 # 随机对战
 random_game = on_command("随机对战", permission = GROUP, priority = 5, block = True)
 
 @random_game.handle()
 async def _(bot:Bot, event:GroupMessageEvent, arg:Message = CommandArg()):
     gold = arg.extract_plain_text().strip()
```

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/api.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/data/data.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9657142857142856%*

 * *Differences: {'16': "{'trigger_condition': '赌注上限为十倍赌注上限'}",*

 * * '18': "{'trigger_condition': '赌注上限为每轮十倍赌注上限'}",*

 * * 'insert': "[(19, OrderedDict([('func', '同花顺'), ('trigger_method', '同花顺 【金额】 【at】'), "*

 * *           "('trigger_condition', '赌注上限为每轮五倍赌注上限'), ('brief_des', '发起同花顺'), ('detail_des', '通过 同花顺 "*

 * *           "来对其他人对战，先手看牌加注，后手看牌跟注，直到一方认输或点数大的获胜。')]))]"}*

```diff
@@ -111,32 +111,39 @@
         "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u4e00\u500d\u8d4c\u6ce8\u4e0a\u9650",
         "trigger_method": "\u88c5\u5f39 \u3010\u5b50\u5f39\u6570\u3011 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
         "brief_des": "\u53d1\u8d77\u63b7\u9ab0\u5b50",
         "detail_des": "\u901a\u8fc7 \u63b7\u9ab0\u5b50 \u6765\u5bf9\u5176\u4ed6\u4eba\u53d1\u8d77\u51b3\u6597\n\u8f6e\u6d41\u5f00\u6570\u6bd4\u5927\u5c0f\n\u4e2d\u9014\u53ef\u7ed3\u675f\n\u8f6e\u6d41\u5f00\u6570\uff0c\u5148\u6bd4\u7ec4\u5408\uff0c\u518d\u6bd4\u70b9\u6570\u3002\n\u7ec4\u5408\uff1a\n\u5f79\u6ee1 > \u4e32 > \u6761 > \u4e24\u5bf9 > \u5bf9 > \u6563\n\n\u3010\u5f00\u59cb\u6e38\u620f\u3011\n\u6447\u9ab0\u5b50/\u63b7\u8272\u5b50 \u3010\u91d1\u989d\u3011 \u3010at\u3011\uff08\u4e3a\u7a7a\u5219\u6240\u6709\u7fa4\u53cb\u90fd\u53ef\u63a5\u53d7\uff09\n\u3010\u56de\u5e94\u3011\n\u63a5\u53d7\u6311\u6218/\u62d2\u7edd\u6311\u6218\n\u3010\u56de\u5408\u4e2d\u3011\n\u5f00\u6570/\u5f00\u70b9/\u53d6\u51fa\uff08\u8f6e\u6d41\u5f00\u6570\uff09\n\u3010\u7ed3\u675f\u3011\n\u7ed3\u675f\uff08\u53ea\u6709\u6682\u8d25\u65b9\u53ef\u53d1\u8d77\uff09\n\u3010\u7ed3\u7b97\u3011\n\u7ed3\u7b97\uff08\u5f53\u67d0\u4e00\u65b960\u79d2\u6ca1\u6709\u56de\u5e94\uff0c\u4ee5\u76ee\u524d\u6bd4\u5206\u7ed3\u7b97\uff09",
         "func": "\u63b7\u9ab0\u5b50",
-        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u4e94\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u5341\u500d\u8d4c\u6ce8\u4e0a\u9650",
         "trigger_method": "\u6447\u9ab0\u5b50/\u63b7\u8272\u5b50 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
         "brief_des": "\u53d1\u8d77\u6251\u514b\u5bf9\u6218",
         "detail_des": "\u901a\u8fc7 \u6251\u514b\u5bf9\u6218 \u6765\u5bf9\u5176\u4ed6\u4eba\u5bf9\u6218\n\u6253\u51fa\u81ea\u5df1\u7684\u624b\u724c\n\u5f53\u5bf9\u65b9\u7684\u8840\u91cf\u5c0f\u4e8e1\u6216\u8005\u5728\u81ea\u5df1\u56de\u5408\u51fa\u724c\u524d\u8840\u91cf>40\u5373\u53ef\u83b7\u80dc\n\u724c\u5e93\u4e00\u517152\u5f20\u724c\uff0c\u5f53\u724c\u5e93\u6ca1\u6709\u724c\u4e86\u5c31\u4ee5\u76ee\u524d\u8840\u91cf\u7ed3\u7b97\uff0c\u7ed3\u675f\u6e38\u620f\u3002\n\n\u5148\u624b\u521d\u59cb\u70b9\u6570\uff1aHP 20 SP 0 DEF 0\n\u540e\u624b\u521d\u59cb\u70b9\u6570\uff1aHP 25 SP 2 DEF 0\n\u6bcf\u56de\u5408\u62bd\u4e09\u5f20\u724c\uff0c\u6253\u51fa\u5176\u4e2d\u7684\u4e00\u5f20\u4f5c\u4e3a\u884c\u52a8\u724c\uff0c\u5f03\u6389\u5269\u4f59\u624b\u724c\u3002\n\uff08\u7279\u522b\u6ce8\u610f\uff1a\u9632\u5fa1\u724c\u4f5c\u4e3a\u884c\u52a8\u724c\u662f\u653b\u51fb\uff09\n\u4e4b\u540e\u5bf9\u65b9\u6447\u4e00\u4e2a20\u9762\u9ab0\u5b50\uff0c\n\u5982\u679c\u70b9\u6570\u5c0f\u4e8e\u5bf9\u65b9SP\u5219\u4ece\u724c\u5e93\u7ffb\u51fa\u4e00\u5f20\u724c\u4f5c\u4e3a\u6280\u80fd\u724c\u6253\u51fa\u3002\n\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u5bf9\u65b9SP\u70b9\u3002\n\n<ft size=30 color=black>\u9ed1\u6843</ft>\n\u63cf\u8ff0\uff1a\u9632\u5fa1\n\u884c\u52a8\u724c\u6548\u679c\uff1a\u6253\u51fa\u653b\u51fb\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u589e\u52a0DEF\n<ft size=30 color=red>\u7ea2\u6843</ft>\n\u63cf\u8ff0\uff1a\u751f\u547d\n\u884c\u52a8\u724c\u6548\u679c\uff1a\u6062\u590dHP\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u6062\u590dHP\n<ft size=30 color=black>\u6885\u82b1</ft>\n\u63cf\u8ff0\uff1a\u6280\u80fd\n\u884c\u52a8\u724c\u6548\u679c\uff1a\u4e3b\u52a8\u6280\u80fd\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u589e\u52a0SP\n<ft size=30 color=red>\u65b9\u7247</ft>\n\u63cf\u8ff0\uff1a\u653b\u51fb\u884c\u52a8\u724c\u6548\u679c\uff1a\u6253\u51fa\u653b\u51fb\n\u6280\u80fd\u724c\u6548\u679c\uff1a\u6253\u51fa\u53cd\u51fb\n\n\u4e3b\u52a8\u6280\u80fd\uff1a\n\u6447\u4e00\u4e2a20\u9762\u9ab0\u5b50\n\u5982\u679c\u70b9\u6570\u5c0f\u4e8e\u81ea\u8eabSP\u5219\u628a\u5269\u4f59\u4e24\u5f20\u624b\u724c\u4f5c\u4e3a\u6280\u80fd\u724c\u5168\u90e8\u6253\u51fa\n\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u81ea\u8eabSP\u70b9ACE\u6280\u80fd\uff1a\n\u6447\u4e00\u4e2a6\u9762\u9ab0\u5b50\n\u628a\u6253\u51fa\u7684ACE\u724c\u70b9\u66ff\u6362\u6210\u6447\u51fa\u7684\u70b9\u6570\n\u518d\u628a\u4e09\u5f20\u624b\u724c\u5168\u90e8\u4f5c\u4e3a\u6280\u80fd\u724c\u6253\u51fa\n\u6309\u7167\u6280\u80fd\u724c\u70b9\u6570\u6263\u9664\u81ea\u8eabSP\u70b9\n\n\u3010\u5f00\u59cb\u6e38\u620f\u3011\n\u6251\u514b\u5bf9\u6218 \u3010\u91d1\u989d\u3011 \u3010at\u3011\uff08\u4e3a\u7a7a\u5219\u6240\u6709\u7fa4\u53cb\u90fd\u53ef\u63a5\u53d7\uff09\n\u3010\u56de\u5e94\u3011\n\u63a5\u53d7\u6311\u6218/\u62d2\u7edd\u6311\u6218\n\u3010\u56de\u5408\u4e2d\u3011\n\u51fa\u724c 1/2/3\uff08\u8f6e\u6d41\u51fa\u724c\uff09\n\u3010\u7ed3\u7b97\u3011\n\u7ed3\u7b97\uff08\u5f53\u67d0\u4e00\u65b960\u79d2\u6ca1\u6709\u56de\u5e94\uff0c\u4ee5\u76ee\u524d\u8840\u91cf\u7ed3\u7b97\uff09",
         "func": "\u6251\u514b\u5bf9\u6218",
         "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u4e00\u500d\u8d4c\u6ce8\u4e0a\u9650",
         "trigger_method": "\u6251\u514b\u5bf9\u6218 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
         "brief_des": "\u53d1\u8d77\u731c\u6570\u5b57",
         "detail_des": "\u901a\u8fc7 \u731c\u6570\u5b57 \u6765\u5bf9\u5176\u4ed6\u4eba\u5bf9\u6218\uff0c\u8f6e\u6d41\u731c\u6570\u5b57\uff0c\u731c\u4e2d\u6570\u5b57\u5373\u53ef\u83b7\u80dc\u3002\u6bcf\u8f6e\u8d4c\u6ce8\u90fd\u4f1a\u589e\u957f\u4e00\u500d",
         "func": "\u731c\u6570\u5b57",
-        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u6bcf\u8f6e\u4e00\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u6bcf\u8f6e\u5341\u500d\u8d4c\u6ce8\u4e0a\u9650",
         "trigger_method": "\u731c\u6570\u5b57 \u3010\u91d1\u989d\u3011 \u3010at\u3011"
     },
     {
+        "brief_des": "\u53d1\u8d77\u540c\u82b1\u987a",
+        "detail_des": "\u901a\u8fc7 \u540c\u82b1\u987a \u6765\u5bf9\u5176\u4ed6\u4eba\u5bf9\u6218\uff0c\u5148\u624b\u770b\u724c\u52a0\u6ce8\uff0c\u540e\u624b\u770b\u724c\u8ddf\u6ce8\uff0c\u76f4\u5230\u4e00\u65b9\u8ba4\u8f93\u6216\u70b9\u6570\u5927\u7684\u83b7\u80dc\u3002",
+        "func": "\u540c\u82b1\u987a",
+        "trigger_condition": "\u8d4c\u6ce8\u4e0a\u9650\u4e3a\u6bcf\u8f6e\u4e94\u500d\u8d4c\u6ce8\u4e0a\u9650",
+        "trigger_method": "\u540c\u82b1\u987a \u3010\u91d1\u989d\u3011 \u3010at\u3011"
+    },
+    {
         "brief_des": "\u521b\u5efa\u8d5b\u9a6c\u5c0f\u6e38\u620f",
         "detail_des": "\u6d41\u7a0b\uff1a\n\u8d5b\u9a6c\u521b\u5efa\uff1a\u7b2c\u4e00\u4f4d\u73a9\u5bb6\u53d1\u8d77\u6d3b\u52a8 \u2192\n\u8d5b\u9a6c\u52a0\u5165 \u3010\u4f60\u7684\u9a6c\u513f\u540d\u79f0\u3011\uff1a\u73a9\u5bb6\u53c2\u8d5b \u2192\n\u8d5b\u9a6c\u5f00\u59cb\uff1a\u6e38\u620f\u8fdb\u884c \u2192\n\u8fdb\u884c\u4e2d \u2192\n\u7ed3\u7b97\n\n\u5f53\u9047\u5230\u9519\u8bef\u6216\u5176\u4ed6\u60c5\u51b5\u53ef\u4f7f\u7528\u8d5b\u9a6c\u91cd\u7f6e\u6765\u91cd\u7f6e\u9a6c\u573a\u3002",
         "func": "\u8d5b\u9a6c\u5c0f\u6e38\u620f",
         "trigger_condition": "\u65e0",
         "trigger_method": "\u8d5b\u9a6c\u521b\u5efa"
     },
     {
```

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9104166666666665%*

 * *Differences: {"'52102'": "{'des': '2-成功率翻倍，3-奖励翻倍。'}",*

 * * "'53101'": "{'color': '#FF6666'}",*

 * * "'62101'": "{'color': '#0099FF'}",*

 * * "'63101'": "OrderedDict([('name', '超级幸运硬币'), ('color', '#FF3300'), ('rare', 6), ('intro', "*

 * *            "'有66.6%的概率获得金币，33.3%的概率失去金币。没有上限'), ('des', '成功率翻倍，奖励翻倍，惩罚翻倍。')])",*

 * * "'63102'": "OrderedDict([('name', '重开券'), ('color', '#006633'), ('rare', 6), ('intro', "*

 * *            "'清空自己的金币，股票'), ('des', '事了拂衣去，深藏身与名。')])"}*

```diff
@@ -123,34 +123,48 @@
         "des": "\u4f7f\u7528\u795e\u79d8\u5929\u5e73\u9700\u8981\u4e00\u70b9\u70b9\u624b\u7eed\u8d39\u3002",
         "intro": "\u4e0e\u968f\u673a\u4e00\u4e2a\u4eba\u5e73\u5206\u91d1\u5e01\u3002",
         "name": "\u795e\u79d8\u5929\u5e73",
         "rare": 5
     },
     "52102": {
         "color": "#FF6600",
-        "des": "\u5e26\u53c2\u65702\u62164\u4f7f\u7528\u4e00\u9897\u94bb\u77f3\u53d6\u6d88\u4e0a\u7ebf\u3002",
+        "des": "2-\u6210\u529f\u7387\u7ffb\u500d\uff0c3-\u5956\u52b1\u7ffb\u500d\u3002",
         "intro": "\u670950%\u7684\u6982\u7387\u83b7\u5f97\u91d1\u5e01\uff0c50%\u7684\u6982\u7387\u5931\u53bb\u91d1\u5e01\u3002\n\u4e0a\u9650 Lv.50 \u91d1\u5e93\u3002",
         "name": "\u5e78\u8fd0\u786c\u5e01",
         "rare": 5
     },
     "53101": {
-        "color": "#FF3300",
+        "color": "#FF6666",
         "des": "\u611f\u8c22\u5404\u4f4d\u73a9\u5bb6\u7684\u652f\u6301\uff01",
         "intro": "\u6253\u5f00\u540e\u53ef\u4ee5\u83b7\u5f97\u3010\u91d1\u5e01\u7b7e\u5230-\u91cd\u7f6e\u7b7e\u5230\u3011\u8303\u56f4\u7684\u968f\u673a\u91d1\u5e01\u3002",
         "name": "\u968f\u673a\u7ea2\u5305",
         "rare": 5
     },
     "61001": {
         "color": "#66CCFF",
         "des": "",
         "intro": "",
         "name": "\u7eaf\u51c0\u7a7a\u6c14",
         "rare": 6
     },
     "62101": {
-        "color": "#87CEFA",
+        "color": "#0099FF",
         "des": "\u201c\u94bb\u77f3\u6709\u4ec0\u4e48\u7528\uff1f\u201d\n\u201c\u6ca1\u7528\u3002\u201d",
         "intro": "\u65e0\u6bd4\u73cd\u8d35\u7684\u94bb\u77f3\uff0c\u53ea\u6709\u5343\u5206\u4e4b\u4e94\u7684\u6982\u7387\u83b7\u5f97\uff0c\u4ee5\u540e\u53ef\u80fd\u6709\u7528\u3002",
         "name": "\u94bb\u77f3",
         "rare": 6
+    },
+    "63101": {
+        "color": "#FF3300",
+        "des": "\u6210\u529f\u7387\u7ffb\u500d\uff0c\u5956\u52b1\u7ffb\u500d\uff0c\u60e9\u7f5a\u7ffb\u500d\u3002",
+        "intro": "\u670966.6%\u7684\u6982\u7387\u83b7\u5f97\u91d1\u5e01\uff0c33.3%\u7684\u6982\u7387\u5931\u53bb\u91d1\u5e01\u3002\u6ca1\u6709\u4e0a\u9650",
+        "name": "\u8d85\u7ea7\u5e78\u8fd0\u786c\u5e01",
+        "rare": 6
+    },
+    "63102": {
+        "color": "#006633",
+        "des": "\u4e8b\u4e86\u62c2\u8863\u53bb\uff0c\u6df1\u85cf\u8eab\u4e0e\u540d\u3002",
+        "intro": "\u6e05\u7a7a\u81ea\u5df1\u7684\u91d1\u5e01\uff0c\u80a1\u7968",
+        "name": "\u91cd\u5f00\u5238",
+        "rare": 6
     }
 }
```

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.3/setup.py` & `nonebot_plugin_game_collection-2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.1.3',
+version='2.1.4',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

