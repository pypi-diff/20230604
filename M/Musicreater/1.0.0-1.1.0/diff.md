# Comparing `tmp/Musicreater-1.0.0.tar.gz` & `tmp/Musicreater-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Musicreater-1.0.0.tar", last modified: Sat May 27 11:56:56 2023, max compression
+gzip compressed data, was "Musicreater-1.1.0.tar", last modified: Sun Jun  4 13:34:27 2023, max compression
```

## Comparing `Musicreater-1.0.0.tar` & `Musicreater-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.378165 Musicreater-1.0.0/
--rw-rw-rw-   0        0        0    13072 2023-05-27 11:45:04.000000 Musicreater-1.0.0/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.234645 Musicreater-1.0.0/Musicreater/
--rw-rw-rw-   0        0        0      824 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/__init__.py
--rw-rw-rw-   0        0        0     6525 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/constants.py
--rw-rw-rw-   0        0        0     2903 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/exceptions.py
--rw-rw-rw-   0        0        0    12850 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/experiment.py
--rw-rw-rw-   0        0        0    10301 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/magicmain.py
--rw-rw-rw-   0        0        0    32861 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/main.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.316371 Musicreater-1.0.0/Musicreater/plugin/
--rw-rw-rw-   0        0        0      559 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/__init__.py
--rw-rw-rw-   0        0        0     2112 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/archive.py
--rw-rw-rw-   0        0        0     5999 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/bdx.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.328331 Musicreater-1.0.0/Musicreater/plugin/bdxfile/
--rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/bdxfile/__init__.py
--rw-rw-rw-   0        0        0     6194 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/bdxfile/main.py
--rw-rw-rw-   0        0        0      809 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/common.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.343282 Musicreater-1.0.0/Musicreater/plugin/funcpack/
--rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/funcpack/__init__.py
--rw-rw-rw-   0        0        0     3896 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/funcpack/main.py
--rw-rw-rw-   0        0        0     2492 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/main.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.355241 Musicreater-1.0.0/Musicreater/plugin/mcstructfile/
--rw-rw-rw-   0        0        0      521 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/mcstructfile/__init__.py
--rw-rw-rw-   0        0        0     1836 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/mcstructfile/main.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.368198 Musicreater-1.0.0/Musicreater/plugin/mcstructpack/
--rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/mcstructpack/__init__.py
--rw-rw-rw-   0        0        0     6242 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/mcstructpack/main.py
--rw-rw-rw-   0        0        0     7153 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/plugin/mcstructure.py
--rw-rw-rw-   0        0        0     4535 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/subclass.py
--rw-rw-rw-   0        0        0      848 2023-05-27 11:45:04.000000 Musicreater-1.0.0/Musicreater/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:56:56.273517 Musicreater-1.0.0/Musicreater.egg-info/
--rw-rw-rw-   0        0        0     7816 2023-05-27 11:56:54.000000 Musicreater-1.0.0/Musicreater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-05-27 11:56:55.000000 Musicreater-1.0.0/Musicreater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:56:55.000000 Musicreater-1.0.0/Musicreater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-27 11:56:55.000000 Musicreater-1.0.0/Musicreater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-27 11:56:55.000000 Musicreater-1.0.0/Musicreater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7816 2023-05-27 11:56:56.375178 Musicreater-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6747 2023-05-27 11:45:04.000000 Musicreater-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 11:56:56.379161 Musicreater-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1597 2023-05-27 11:45:04.000000 Musicreater-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.370883 Musicreater-1.1.0/
+-rw-rw-rw-   0        0        0    13072 2023-05-27 11:45:04.000000 Musicreater-1.1.0/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.295138 Musicreater-1.1.0/Musicreater/
+-rw-rw-rw-   0        0        0      825 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/__init__.py
+-rw-rw-rw-   0        0        0     6525 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/constants.py
+-rw-rw-rw-   0        0        0     2903 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/exceptions.py
+-rw-rw-rw-   0        0        0     6961 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/experiment.py
+-rw-rw-rw-   0        0        0    10301 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/magicmain.py
+-rw-rw-rw-   0        0        0    31166 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/main.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.334006 Musicreater-1.1.0/Musicreater/plugin/
+-rw-rw-rw-   0        0        0      559 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/__init__.py
+-rw-rw-rw-   0        0        0     2112 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/archive.py
+-rw-rw-rw-   0        0        0     5999 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/bdx.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.338991 Musicreater-1.1.0/Musicreater/plugin/bdxfile/
+-rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/bdxfile/__init__.py
+-rw-rw-rw-   0        0        0     6194 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/bdxfile/main.py
+-rw-rw-rw-   0        0        0      809 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/common.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.344969 Musicreater-1.1.0/Musicreater/plugin/funcpack/
+-rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/funcpack/__init__.py
+-rw-rw-rw-   0        0        0     3896 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/funcpack/main.py
+-rw-rw-rw-   0        0        0     2492 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/main.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.350951 Musicreater-1.1.0/Musicreater/plugin/mcstructfile/
+-rw-rw-rw-   0        0        0      521 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/mcstructfile/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/plugin/mcstructfile/main.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.356930 Musicreater-1.1.0/Musicreater/plugin/mcstructpack/
+-rw-rw-rw-   0        0        0      513 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/mcstructpack/__init__.py
+-rw-rw-rw-   0        0        0     6242 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/mcstructpack/main.py
+-rw-rw-rw-   0        0        0     7153 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/plugin/mcstructure.py
+-rw-rw-rw-   0        0        0     3797 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/plugin/noteblock.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.364904 Musicreater-1.1.0/Musicreater/plugin/websocket/
+-rw-rw-rw-   0        0        0      522 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/plugin/websocket/__init__.py
+-rw-rw-rw-   0        0        0      771 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/plugin/websocket/main.py
+-rw-rw-rw-   0        0        0     1168 2023-06-04 13:30:48.000000 Musicreater-1.1.0/Musicreater/plugin/websocket.py
+-rw-rw-rw-   0        0        0     4535 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/subclass.py
+-rw-rw-rw-   0        0        0      848 2023-05-27 11:45:04.000000 Musicreater-1.1.0/Musicreater/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:34:27.310087 Musicreater-1.1.0/Musicreater.egg-info/
+-rw-rw-rw-   0        0        0     7816 2023-06-04 13:34:26.000000 Musicreater-1.1.0/Musicreater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2023-06-04 13:34:27.000000 Musicreater-1.1.0/Musicreater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 13:34:26.000000 Musicreater-1.1.0/Musicreater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-06-04 13:34:26.000000 Musicreater-1.1.0/Musicreater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-04 13:34:26.000000 Musicreater-1.1.0/Musicreater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7816 2023-06-04 13:34:27.369886 Musicreater-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6747 2023-05-27 11:45:04.000000 Musicreater-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 13:34:27.370883 Musicreater-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1597 2023-05-27 11:45:04.000000 Musicreater-1.1.0/setup.py
```

### Comparing `Musicreater-1.0.0/LICENSE.md` & `Musicreater-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/__init__.py` & `Musicreater-1.1.0/Musicreater/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 Terms & Conditions: License.md in the root directory
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
-from .main import *
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 __all__ = []
 __author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"), ("鸣凤鸽子", "MingFengPigeon"))
+
+from .main import *
```

### Comparing `Musicreater-1.0.0/Musicreater/constants.py` & `Musicreater-1.1.0/Musicreater/constants.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/exceptions.py` & `Musicreater-1.1.0/Musicreater/exceptions.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/magicmain.py` & `Musicreater-1.1.0/Musicreater/magicmain.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/main.py` & `Musicreater-1.1.0/Musicreater/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # 音·创 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库根目录下的 License.md
 
 
 import os
 import math
-from typing import Tuple, List
+from typing import Tuple, List, Union
 
 import mido
 
 from .exceptions import *
 from .constants import *
 from .utils import *
 from .subclass import *
@@ -83,14 +83,17 @@
 
     enable_old_exe_format: bool
     """是否启用旧版execute指令格式"""
 
     execute_cmd_head: str
     """execute指令头部"""
 
+    channels: Dict[int, Dict[int, List[Tuple[str, int, int, Union[None, int]]]]]
+    """频道信息字典"""
+
     music_command_list: List[SingleCommand]
     """音乐指令列表"""
 
     music_tick_num: int
     """音乐总延迟"""
 
     progress_bar_command: List[SingleCommand]
@@ -124,14 +127,15 @@
         self.execute_cmd_head = (
             "execute {} ~ ~ ~ "
             if enable_old_exe_format
             else "execute as {} at @s positioned ~ ~ ~ run "
         )
 
         self.progress_bar_command = self.music_command_list = []
+        self.channels = {}
         self.music_tick_num = 0
 
     @classmethod
     def from_midi_file(
         cls,
         midi_file_path: str,
         old_exe_format: bool = False,
@@ -143,15 +147,15 @@
         ----------
         midi_file: str
             midi文件地址
         enable_old_exe_format: bool
             是否启用旧版(≤1.19)指令格式，默认为否
         """
 
-        midi_music_name = os.path.splitext(os.path.basename(midi_file_path))[0]
+        midi_music_name = os.path.splitext(os.path.basename(midi_file_path))[0].replace(' ','_')
         """文件名，不含路径且不含后缀"""
 
         try:
             return cls(mido.MidiFile(midi_file_path), midi_music_name, old_exe_format)
         except (ValueError, TypeError) as E:
             raise MidiDestroyedError(f"文件{midi_file_path}损坏：{E}")
         except FileNotFoundError as E:
@@ -481,43 +485,27 @@
                     annotation="移除临时计算计分板（秒）",
                 )
             )
 
         self.progress_bar_command = result
         return result
 
-    def to_command_list_in_score(
+    def to_music_channels(
         self,
-        scoreboard_name: str = "mscplay",
-        max_volume: float = 1.0,
-        speed: float = 1.0,
-    ) -> Tuple[List[List[SingleCommand]], int, int]:
+    ) -> Dict[int, Dict[int, List[Tuple[str, int, int, Union[None, int]]]]]:
         """
-        使用金羿的转换思路，将midi转换为我的世界命令列表
-
-        Parameters
-        ----------
-        scoreboard_name: str
-            我的世界的计分板名称
-        max_volume: float
-            最大播放音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放
-        speed: float
-            速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
+        使用金羿的转换思路，将midi解析并转换为频道信息
 
         Returns
         -------
-        tuple( list[list[SingleCommand指令,... ],... ], int指令数量, int音乐时长游戏刻 )
+        Dict[int, Dict[int, List[Tuple[str,int,int,Union[None,int]]]]]
         """
 
-        if speed == 0:
-            raise ZeroSpeedError("播放速度仅可为正实数")
-        max_volume = 1 if max_volume > 1 else (0.001 if max_volume <= 0 else max_volume)
-
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
-        channels = empty_midi_channels()
+        midi_channels = empty_midi_channels()
 
         # 我们来用通道统计音乐信息
         # 但是是用分轨的思路的
         for track_no, track in enumerate(self.midi.tracks):
             microseconds = 0
 
             for msg in track:
@@ -542,30 +530,30 @@
                     # 曾用于调试模式
                     #     try:
                     #         if msg.channel > 15:
                     #             raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
                     #     except AttributeError:
                     #         pass
 
-                    if not track_no in channels[msg.channel].keys():
-                        channels[msg.channel][track_no] = []
+                    if not track_no in midi_channels[msg.channel].keys():
+                        midi_channels[msg.channel][track_no] = []
                     if msg.type == "program_change":
-                        channels[msg.channel][track_no].append(
+                        midi_channels[msg.channel][track_no].append(
                             ("PgmC", msg.program, microseconds)
                         )
 
                     elif msg.type == "note_on" and msg.velocity != 0:
-                        channels[msg.channel][track_no].append(
+                        midi_channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
                         msg.type == "note_off"
                     ):
-                        channels[msg.channel][track_no].append(
+                        midi_channels[msg.channel][track_no].append(
                             ("NoteE", msg.note, microseconds)
                         )
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
@@ -573,30 +561,62 @@
 
         2 音符开始消息
         ("NoteS", 开始的音符ID, 力度（响度）, 距离演奏开始的毫秒)
 
         3 音符结束消息
         ("NoteS", 结束的音符ID, 距离演奏开始的毫秒)"""
 
+        self.channels = midi_channels
+        return self.channels
+
+    def to_command_list_in_score(
+        self,
+        scoreboard_name: str = "mscplay",
+        max_volume: float = 1.0,
+        speed: float = 1.0,
+    ) -> Tuple[List[List[SingleCommand]], int, int]:
+        """
+        使用金羿的转换思路，将midi转换为我的世界命令列表
+
+        Parameters
+        ----------
+        scoreboard_name: str
+            我的世界的计分板名称
+        max_volume: float
+            最大播放音量，注意：这里的音量范围为(0,1]，如果超出将被处理为正确值，其原理为在距离玩家 (1 / volume -1) 的地方播放
+        speed: float
+            速度，注意：这里的速度指的是播放倍率，其原理为在播放音频的时候，每个音符的播放时间除以 speed
+
+        Returns
+        -------
+        tuple( list[list[SingleCommand指令,... ],... ], int指令数量, int音乐时长游戏刻 )
+        """
+
+        if speed == 0:
+            raise ZeroSpeedError("播放速度仅可为正实数")
+        max_volume = 1 if max_volume > 1 else (0.001 if max_volume <= 0 else max_volume)
+
         tracks = []
         cmdAmount = 0
         maxScore = 0
 
+        self.to_music_channels()
+
         # 此处 我们把通道视为音轨
-        for i in channels.keys():
+        for i in self.channels.keys():
             # 如果当前通道为空 则跳过
-            if not channels[i]:
+            if not self.channels[i]:
                 continue
 
             # 第十通道是打击乐通道
             SpecialBits = True if i == 9 else False
 
             # nowChannel = []
 
-            for track_no, track in channels[i].items():
+            for track_no, track in self.channels[i].items():
                 nowTrack = []
 
                 for msg in track:
                     if msg[0] == "PgmC":
                         InstID = msg[1]
 
                     elif msg[0] == "NoteS":
@@ -665,101 +685,38 @@
         tuple( list[SingleCommand,...], int音乐时长游戏刻 )
         """
 
         if speed == 0:
             raise ZeroSpeedError("播放速度仅可为正实数")
         max_volume = 1 if max_volume > 1 else (0.001 if max_volume <= 0 else max_volume)
 
-        # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
-        channels = empty_midi_channels()
-
-        # 我们来用通道统计音乐信息
-        # 但是是用分轨的思路的
-        for track_no, track in enumerate(self.midi.tracks):
-            microseconds = 0
-
-            for msg in track:
-                if msg.time != 0:
-                    try:
-                        microseconds += (
-                            msg.time * tempo / self.midi.ticks_per_beat / 1000
-                        )
-                        # print(microseconds)
-                    except NameError:
-                        # raise NotDefineTempoError("计算当前分数时出错 未定义参量 Tempo")
-                        microseconds += (
-                            msg.time
-                            * mido.midifiles.midifiles.DEFAULT_TEMPO
-                            / self.midi.ticks_per_beat
-                        ) / 1000
-
-                if msg.is_meta:
-                    if msg.type == "set_tempo":
-                        tempo = msg.tempo
-                else:
-                    try:
-                        # 曾用于调试模式
-                        # if msg.channel > 15:
-                            # raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
-                        if not track_no in channels[msg.channel].keys():
-                            channels[msg.channel][track_no] = []
-                    except AttributeError:
-                        pass
-
-                    if msg.type == "program_change":
-                        channels[msg.channel][track_no].append(
-                            ("PgmC", msg.program, microseconds)
-                        )
-
-                    elif msg.type == "note_on" and msg.velocity != 0:
-                        channels[msg.channel][track_no].append(
-                            ("NoteS", msg.note, msg.velocity, microseconds)
-                        )
-
-                    elif (msg.type == "note_on" and msg.velocity == 0) or (
-                        msg.type == "note_off"
-                    ):
-                        channels[msg.channel][track_no].append(
-                            ("NoteE", msg.note, microseconds)
-                        )
-
-        """整合后的音乐通道格式
-        每个通道包括若干消息元素其中逃不过这三种：
-
-        1 切换乐器消息
-        ("PgmC", 切换后的乐器ID: int, 距离演奏开始的毫秒)
-
-        2 音符开始消息
-        ("NoteS", 开始的音符ID, 力度（响度）, 距离演奏开始的毫秒)
-
-        3 音符结束消息
-        ("NoteS", 结束的音符ID, 距离演奏开始的毫秒)"""
+        self.to_music_channels()
 
         tracks = {}
 
         # 此处 我们把通道视为音轨
-        for i in channels.keys():
+        for i in self.channels.keys():
             # 如果当前通道为空 则跳过
-            if not channels[i]:
+            if not self.channels[i]:
                 continue
 
             # 第十通道是打击乐通道
             SpecialBits = True if i == 9 else False
 
             # nowChannel = []
 
-            for track_no, track in channels[i].items():
+            for track_no, track in self.channels[i].items():
                 for msg in track:
                     if msg[0] == "PgmC":
                         InstID = msg[1]
 
                     elif msg[0] == "NoteS":
                         try:
                             soundID, _X = (
-                                self.perc_inst_to_soundID_withX(InstID)
+                                self.perc_inst_to_soundID_withX(msg[1])
                                 if SpecialBits
                                 else self.inst_to_souldID_withX(InstID)
                             )
                         except UnboundLocalError as E:
                             # raise NotDefineProgramError(f"未定义乐器便提前演奏。\n{E}")
                             soundID, _X = (
                                 self.perc_inst_to_soundID_withX(-1)
@@ -768,22 +725,30 @@
                             )
                         score_now = round(msg[-1] / float(speed) / 50)
                         # print(score_now)
 
                         try:
                             tracks[score_now].append(
                                 self.execute_cmd_head.format(player_selector)
-                                + f"playsound {soundID} @s ^ ^ ^{1 / max_volume - 1} {msg[2] / 128} "
-                                f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                                + f"playsound {soundID} @s ^ ^ ^{128 / max_volume / msg[2] - 1} {msg[2] / 128} "
+                                + (
+                                    ""
+                                    if SpecialBits
+                                    else f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                                )
                             )
                         except KeyError:
                             tracks[score_now] = [
                                 self.execute_cmd_head.format(player_selector)
-                                + f"playsound {soundID} @s ^ ^ ^{1 / max_volume - 1} {msg[2] / 128} "
-                                f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                                + f"playsound {soundID} @s ^ ^ ^{128 / max_volume / msg[2] - 1} {msg[2] / 128} "
+                                + (
+                                    ""
+                                    if SpecialBits
+                                    else f"{2 ** ((msg[1] - 60 - _X) / 12)}"
+                                )
                             ]
 
         all_ticks = list(tracks.keys())
         all_ticks.sort()
         results = []
 
         for i in range(len(all_ticks)):
@@ -815,15 +780,14 @@
         self,
     ) -> dict:
         """
         使用金羿的转换思路，将midi转换为字典
         :return: dict()
         """
 
-        
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
         channels = empty_midi_channels()
 
         # 我们来用通道统计音乐信息
         # 但是是用分轨的思路的
         for track_no, track in enumerate(self.midi.tracks):
             microseconds = 0
@@ -846,15 +810,15 @@
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
                 else:
                     try:
                         # 曾用于调试模式
                         # if msg.channel > 15:
-                            # raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
+                        # raise ChannelOverFlowError(f"当前消息 {msg} 的通道超限(≤15)")
                         if not track_no in channels[msg.channel].keys():
                             channels[msg.channel][track_no] = []
                     except AttributeError:
                         pass
 
                     if msg.type == "program_change":
                         channels[msg.channel][track_no].append(
@@ -883,19 +847,17 @@
         ("NoteS", 开始的音符ID, 力度（响度）, 距离演奏开始的毫秒)
 
         3 音符结束消息
         ("NoteS", 结束的音符ID, 距离演奏开始的毫秒)"""
 
         return channels
 
-
     def copy_important(self):
         dst = MidiConvert(
             midi_obj=None,
             midi_name=self.midi_music_name,
             enable_old_exe_format=self.enable_old_exe_format,
         )
         dst.music_command_list = [i.copy() for i in self.music_command_list]
         dst.progress_bar_command = [i.copy() for i in self.progress_bar_command]
         dst.music_tick_num = self.music_tick_num
         return dst
-
```

### Comparing `Musicreater-1.0.0/Musicreater/plugin/__init__.py` & `Musicreater-1.1.0/Musicreater/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/archive.py` & `Musicreater-1.1.0/Musicreater/plugin/archive.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/bdx.py` & `Musicreater-1.1.0/Musicreater/plugin/bdx.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/bdxfile/__init__.py` & `Musicreater-1.1.0/Musicreater/plugin/bdxfile/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/bdxfile/main.py` & `Musicreater-1.1.0/Musicreater/plugin/bdxfile/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/common.py` & `Musicreater-1.1.0/Musicreater/plugin/common.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/funcpack/__init__.py` & `Musicreater-1.1.0/Musicreater/plugin/funcpack/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/funcpack/main.py` & `Musicreater-1.1.0/Musicreater/plugin/funcpack/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/main.py` & `Musicreater-1.1.0/Musicreater/plugin/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/mcstructfile/__init__.py` & `Musicreater-1.1.0/Musicreater/plugin/mcstructfile/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/mcstructfile/main.py` & `Musicreater-1.1.0/Musicreater/plugin/mcstructfile/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,7 +63,13 @@
             os.path.join(data_cfg.dist_path, f"{midi_cvt.midi_music_name}.mcstructure")
         ),
         "wb+",
     ) as f:
         struct.dump(f)
 
     return size, max_delay
+
+
+def to_mcstructure_file_in_redstone(
+    midi_cvt: MidiConvert,
+    data_cfg: ConvertConfig,):
+    pass
```

### Comparing `Musicreater-1.0.0/Musicreater/plugin/mcstructpack/__init__.py` & `Musicreater-1.1.0/Musicreater/plugin/mcstructpack/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/mcstructpack/main.py` & `Musicreater-1.1.0/Musicreater/plugin/mcstructpack/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/plugin/mcstructure.py` & `Musicreater-1.1.0/Musicreater/plugin/mcstructure.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/subclass.py` & `Musicreater-1.1.0/Musicreater/subclass.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater/utils.py` & `Musicreater-1.1.0/Musicreater/utils.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/Musicreater.egg-info/PKG-INFO` & `Musicreater-1.1.0/Musicreater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 1.0.0
+Version: 1.1.0
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: Musicreater Version: 1.1.0 Summary:
 ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
 https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `Musicreater-1.0.0/Musicreater.egg-info/SOURCES.txt` & `Musicreater-1.1.0/Musicreater.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 Musicreater.egg-info/top_level.txt
 Musicreater/plugin/__init__.py
 Musicreater/plugin/archive.py
 Musicreater/plugin/bdx.py
 Musicreater/plugin/common.py
 Musicreater/plugin/main.py
 Musicreater/plugin/mcstructure.py
+Musicreater/plugin/noteblock.py
+Musicreater/plugin/websocket.py
 Musicreater/plugin/bdxfile/__init__.py
 Musicreater/plugin/bdxfile/main.py
 Musicreater/plugin/funcpack/__init__.py
 Musicreater/plugin/funcpack/main.py
 Musicreater/plugin/mcstructfile/__init__.py
 Musicreater/plugin/mcstructfile/main.py
 Musicreater/plugin/mcstructpack/__init__.py
-Musicreater/plugin/mcstructpack/main.py
+Musicreater/plugin/mcstructpack/main.py
+Musicreater/plugin/websocket/__init__.py
+Musicreater/plugin/websocket/main.py
```

### Comparing `Musicreater-1.0.0/PKG-INFO` & `Musicreater-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 1.0.0
+Version: 1.1.0
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Musicreater Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: Musicreater Version: 1.1.0 Summary:
 ä¸æ¬¾åè´¹å¼æºç ãæçä¸çã midé³ä¹è½¬æ¢åºã Home-page:
 https://github.com/TriM-Organization/Musicreater Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: Chinese (Simplified) Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `Musicreater-1.0.0/README.md` & `Musicreater-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `Musicreater-1.0.0/setup.py` & `Musicreater-1.1.0/setup.py`

 * *Files identical despite different names*

