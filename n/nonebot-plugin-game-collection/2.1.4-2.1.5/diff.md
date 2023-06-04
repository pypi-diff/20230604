# Comparing `tmp/nonebot_plugin_game_collection-2.1.4.tar.gz` & `tmp/nonebot_plugin_game_collection-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.1.4.tar", last modified: Sun Jun  4 12:20:32 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.1.5.tar", last modified: Sun Jun  4 13:26:00 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.1.4.tar` & `nonebot_plugin_game_collection-2.1.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.855719 nonebot_plugin_game_collection-2.1.4/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.4/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-04 12:20:32.855219 nonebot_plugin_game_collection-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.795169 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    48705 2023-06-04 12:18:21.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.813685 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    11391 2023-06-04 09:46:42.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    20138 2023-06-04 11:54:55.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    16202 2023-06-04 11:51:18.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    30093 2023-06-04 08:55:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/config.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.818189 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/
--rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/api.py
--rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/data.py
--rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/run.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.824695 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.845210 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5375 2023-06-04 11:46:30.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.846711 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.853718 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:20:32.804677 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-04 12:20:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2038 2023-06-04 12:20:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 12:20:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-04 12:20:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-04 12:20:32.000000 nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 12:20:32.856220 nonebot_plugin_game_collection-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-06-04 12:20:29.000000 nonebot_plugin_game_collection-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.359868 nonebot_plugin_game_collection-2.1.5/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-04 13:26:00.359368 nonebot_plugin_game_collection-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.286893 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    48705 2023-06-04 12:18:21.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.305030 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    11410 2023-06-04 13:24:05.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    20170 2023-06-04 13:24:04.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    16202 2023-06-04 11:51:18.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    30093 2023-06-04 08:55:32.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/config.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.311539 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/
+-rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/api.py
+-rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/data.py
+-rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/run.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.316542 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.347382 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5375 2023-06-04 11:46:30.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.350029 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.356866 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.296352 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-04 13:26:00.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-06-04 13:26:00.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 13:26:00.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-04 13:26:00.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-04 13:26:00.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 13:26:00.359868 nonebot_plugin_game_collection-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-06-04 13:25:56.000000 nonebot_plugin_game_collection-2.1.5/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.1.4/LICENSE` & `nonebot_plugin_game_collection-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/README.md` & `nonebot_plugin_game_collection-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Account.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,26 +83,27 @@
         user.group_accounts[group_id] = GroupAccount(group_id = group_id, nickname = user.nickname)
         data.save()
 
     group_account = user.group_accounts[group_id]
 
     return user,group_account
 
-def update_company_index(company_index):
+def update_company_index():
     """
     从群数据生成公司名查找群号的字典
     """
     company_index = {}
     for group_id in group_data:
         if company_name := group_data[group_id].company.company_name:
             company_index[company_name] = group_id
             company_index[str(group_id)] = group_id
+    return company_index
 
 company_index:Dict[str,int] = {}
-update_company_index(company_index)
+company_index = update_company_index()
 
 def BG_path(event:MessageEvent):
     my_BG = BG_image / f"{str(event.user_id)}.png"
     if my_BG.exists():
         return my_BG
     else:
         return default_BG
@@ -264,15 +265,15 @@
 def Newday():
     """
     刷新每日
     """
     log = ""
     group_check = {k:set() for k in group_data}
     global company_index
-    update_company_index(company_index)
+    company_index = update_company_index()
     company_ids = company_index.values()
     stock_check = {k:0 for k in company_ids}
     # 检查user_data
     for user_id in user_data:
         user = user_data[user_id]
         user.transfer_limit = 0
         props = user.props
```

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Market.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def check_company_name(company_name:str):
     """
     检查公司名是否合法
     """
     if not company_name:
         return f"公司名称不能为空"
     global company_index
-    update_company_index(company_index)
+    company_index = update_company_index()
     if company_name in company_index:
         return f"{company_name} 已被注册"
     if " " in company_name or "\n" in company_name:
         return "公司名称不能含有空格或回车"
     count = 0
     for x in company_name:
         if ord(x) < 0x200:
@@ -100,15 +100,16 @@
     user = Manager.locate_user(event)[0]
     if user.props.get("33001",0) < 1:
         return f"你的【{props_library['33001']['name']}】已失效"
     if check := check_company_name(company_name):
         return check
     old_company_name = company.company_name
     company.company_name = company_name
-    update_company_index(company_index)
+    global company_index
+    company_index = update_company_index()
     return f'【{old_company_name}】已重命名为【{company_name}】'
 
 def value_update(group_account:GroupAccount):
     """
     刷新持股价值
     group_account:用户群账户
     """
```

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/api.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/data/data.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.4/setup.py` & `nonebot_plugin_game_collection-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.1.4',
+version='2.1.5',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

