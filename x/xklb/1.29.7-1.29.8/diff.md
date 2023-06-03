# Comparing `tmp/xklb-1.29.7.tar.gz` & `tmp/xklb-1.29.8.tar.gz`

## Comparing `xklb-1.29.7.tar` & `xklb-1.29.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.7/.gitattributes
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 xklb-1.29.7/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.7/Windows.md
--rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.7/pdm.lock
--rw-r--r--   0        0        0    19042 2020-02-02 00:00:00.000000 xklb-1.29.7/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.7/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.7/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.7/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/__init__.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/books.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/consts.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/dl_config.py
--rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/dl_extract.py
--rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/gui.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/hn_extract.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/lb.py
--rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/playback.py
--rw-r--r--   0        0        0    33325 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/player.py
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/praw_extract.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/search.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/subtitle.py
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/tabs_extract.py
--rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/tube_backend.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/tube_extract.py
--rw-r--r--   0        0        0    54188 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/usage.py
--rw-r--r--   0        0        0    33490 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/history.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     6032 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.7/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.7/LICENSE
--rw-r--r--   0        0        0    76377 2020-02-02 00:00:00.000000 xklb-1.29.7/README.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.29.7/pyproject.toml
--rw-r--r--   0        0        0    79973 2020-02-02 00:00:00.000000 xklb-1.29.7/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.8/.gitattributes
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 xklb-1.29.8/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.8/Windows.md
+-rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.8/pdm.lock
+-rw-r--r--   0        0        0    19065 2020-02-02 00:00:00.000000 xklb-1.29.8/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.8/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.8/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.8/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/__init__.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/books.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/consts.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/dl_config.py
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/gui.py
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/lb.py
+-rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/playback.py
+-rw-r--r--   0        0        0    33325 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/player.py
+-rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/search.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/subtitle.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/tube_extract.py
+-rw-r--r--   0        0        0    61617 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/usage.py
+-rw-r--r--   0        0        0    33490 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     6032 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.8/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.8/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.8/LICENSE
+-rw-r--r--   0        0        0    83918 2020-02-02 00:00:00.000000 xklb-1.29.8/README.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.29.8/pyproject.toml
+-rw-r--r--   0        0        0    87514 2020-02-02 00:00:00.000000 xklb-1.29.8/PKG-INFO
```

### Comparing `xklb-1.29.7/TODO` & `xklb-1.29.8/TODO`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/Windows.md` & `xklb-1.29.8/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/pdm.lock` & `xklb-1.29.8/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/readme.py` & `xklb-1.29.8/readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,18 @@
     ("Add local media", "fsadd"),
     ("Add online media", "tubeadd"),
     ("Add reddit media", "redditadd"),
     ("Create / Update a Hacker News database", "hnadd"),
     ("Add tabs", "tabsadd"),
     ("Watch / Listen", "watch"),
     ("Search captions / subtitles", "search"),
+    ("History", "history"),
     ("Open tabs", "tabs"),
     ("Download media", "download"),
-    ("Show Download Status", "download_status"),
+    ("Download Status", "download-status"),
     ("Update local media", "fsupdate"),
     ("Update online media", "tubeupdate"),
     ("Update reddit media", "redditupdate"),
     ("Convert pushshift data to reddit.db format", "pushshift"),
     ("List playlists", "playlists"),
     ("Blocklist a channel", "block"),
     ("Show large folders", "bigdirs"),
```

### Comparing `xklb-1.29.7/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.29.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.29.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/.github/workflows/push.yaml` & `xklb-1.29.8/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/sql/transfer.sql` & `xklb-1.29.8/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/av.py` & `xklb-1.29.8/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/books.py` & `xklb-1.29.8/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/consts.py` & `xklb-1.29.8/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/db.py` & `xklb-1.29.8/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/dl_config.py` & `xklb-1.29.8/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/dl_extract.py` & `xklb-1.29.8/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/fs_extract.py` & `xklb-1.29.8/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/gui.py` & `xklb-1.29.8/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/hn_extract.py` & `xklb-1.29.8/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/lb.py` & `xklb-1.29.8/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/play_actions.py` & `xklb-1.29.8/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/playback.py` & `xklb-1.29.8/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/player.py` & `xklb-1.29.8/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/praw_extract.py` & `xklb-1.29.8/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/search.py` & `xklb-1.29.8/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/subtitle.py` & `xklb-1.29.8/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/tabs_actions.py` & `xklb-1.29.8/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/tabs_extract.py` & `xklb-1.29.8/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/tube_backend.py` & `xklb-1.29.8/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/tube_extract.py` & `xklb-1.29.8/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/usage.py` & `xklb-1.29.8/xklb/usage.py`

 * *Files 16% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         library {action} --print --limit 10  # print the next 10 files
         library {action} -p -L 10  # print the next 10 files
         library {action} -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
 
         Printing modes
         library {action} -p    # print as a table
         library {action} -p a  # print an aggregate report
-        library {action} -p b  # print a bigdirs report (see lb bigdirs -h for more info)
+        library {action} -p b  # print a bigdirs report (see library bigdirs -h for more info)
         library {action} -p f  # print fields (defaults to path; use --cols to change)
                                # -- useful for piping paths to utilities like xargs or GNU Parallel
 
         library {action} -p d  # mark deleted
         library {action} -p w  # mark watched
 
         Some printing modes can be combined
@@ -419,17 +419,54 @@
            34:52 Who will give her a one liter stainless steel boiler for one Lari?
            34:54 Glass boilers cost two
 
     Search and open file
     $ library search fts.db dashi --open
 """
 
-history = """library history [database]
+history = """library history [--frequency daily|weekly|{monthly}|quarterly|yearly] [--limit LIMIT] DATABASE [{all}|watching|watched|deleted|created|modified]
 
+    Explore history through different facets
 
+    $ library history video.db watched
+    Finished watching:
+    ╒═══════════════╤═════════════════════════════════╤════════════════╤════════════╤════════════╕
+    │ time_period   │ duration_sum                    │ duration_avg   │ size_sum   │ size_avg   │
+    ╞═══════════════╪═════════════════════════════════╪════════════════╪════════════╪════════════╡
+    │ 2022-11       │ 4 days, 16 hours and 20 minutes │ 55.23 minutes  │ 26.3 GB    │ 215.9 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2022-12       │ 23 hours and 20.03 minutes      │ 35.88 minutes  │ 8.3 GB     │ 213.8 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-01       │ 17 hours and 3.32 minutes       │ 15.27 minutes  │ 14.3 GB    │ 214.1 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-02       │ 4 days, 5 hours and 60 minutes  │ 23.17 minutes  │ 148.3 GB   │ 561.6 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-03       │ 2 days, 18 hours and 18 minutes │ 11.20 minutes  │ 118.1 GB   │ 332.8 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-05       │ 5 days, 5 hours and 4 minutes   │ 45.75 minutes  │ 152.9 GB   │ 932.1 MB   │
+    ╘═══════════════╧═════════════════════════════════╧════════════════╧════════════╧════════════╛
+
+    $ library history video.db deleted
+    Deleted media:
+    ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
+    │ time_period   │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
+    ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
+    │ 2023-04       │ 1 year, 10 months, 3 days and 8 hours      │ 4.47 minutes   │ 1.6 TB     │ 7.4 MB     │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-05       │ 9 months, 26 days, 20 hours and 34 minutes │ 30.35 minutes  │ 1.1 TB     │ 73.7 MB    │
+    ╘═══════════════╧════════════════════════════════════════════╧════════════════╧════════════╧════════════╛
+    ╒════════════════════════════════════════════════════════════════════════════════════════════════════════════╤═══════════════╤══════════════════╤════════════════╕
+    │ title_path                                                                                                 │ duration      │   subtitle_count │ time_deleted   │
+    ╞════════════════════════════════════════════════════════════════════════════════════════════════════════════╪═══════════════╪══════════════════╪════════════════╡
+    │ Terminus (1987)                                                                                            │ 1 hour and    │                0 │ yesterday      │
+    │ /mnt/d/70_Now_Watching/Terminus_1987.mp4                                                                   │ 15.55 minutes │                  │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼──────────────────┼────────────────┤
+    │ Commodore 64 Longplay [062] The Transformers (EU) /mnt/d/71_Mealtime_Videos/Youtube/World_of_Longplays/Com │ 24.77 minutes │                2 │ yesterday      │
+    │ modore_64_Longplay_062_The_Transformers_EU_[1RRX7Kykb38].webm                                              │               │                  │                │
+    ...
 
 """
 
 playlists = """library playlists [database] [--aggregate] [--fields] [--json] [--delete ...]
 
     List of Playlists
 
@@ -514,15 +551,15 @@
 
     You can also invoke tabs manually:
 
         library tabs -L 1  # open one tab
 
     Print URLs
 
-        lb-dev tabs -w "frequency='yearly'" -p
+        library tabs -w "frequency='yearly'" -p
         ╒════════════════════════════════════════════════════════════════╤═════════════╤══════════════╕
         │ path                                                           │ frequency   │ time_valid   │
         ╞════════════════════════════════════════════════════════════════╪═════════════╪══════════════╡
         │ https://old.reddit.com/r/Autonomia/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
         ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
         ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
@@ -603,15 +640,15 @@
 
         library tubeadd reddit.db --playlist-db media
 
     You can also include a category for file organization
 
         library tubeadd -c Mealtime dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
 
-    Files will be saved to <lb download prefix>/<lb tubeadd category>/
+    Files will be saved to <download prefix>/<tubeadd category>/
 
         For example:
         library tubeadd -c Cool ...
         library download D:\'My Documents'\ ...
         Media will be downloaded to 'D:\My Documents\Cool\'
 
     Fetch extra metadata:
@@ -645,57 +682,57 @@
         library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
 """
 
 bigdirs = """library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by "deleted" | "played"] [--size=+5MB]
 
     See what folders take up space
 
-        lb bigdirs video.db
-        lb bigdirs audio.db
-        lb bigdirs fs.db
+        library bigdirs video.db
+        library bigdirs audio.db
+        library bigdirs fs.db
 """
 
 christen = """library christen DATABASE [--run]
 
     Rename files to be somewhat normalized
 
     Default mode is dry-run
 
-        lb christen fs.db
+        library christen fs.db
 
     To actually do stuff use the run flag
 
-        lb christen audio.db --run
+        library christen audio.db --run
 
     You can optionally replace all the spaces in your filenames with dots
 
-        lb christen --dot-space video.db
+        library christen --dot-space video.db
 """
 cluster_sort = """library cluster-sort [input_path | stdin] [output_path | stdout]
 
     Group lines of text into sorted output
 """
 
 copy_play_counts = """library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
 
     Copy play count information between databases
 
-        lb copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
+        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 """
 dedupe = """library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
 
     Dedupe your files
 """
 
 merge_dbs = """library merge-dbs DEST_DB SOURCE_DB ... [--upsert pk1[,pk2]]
 
     Merge database data and tables
 
-        lb merge-dbs --upsert --pk path video.db tv.db movies.db
-        lb merge-dbs --table media,playlists --pk path audio.db music.db podcasts.db
+        library merge-dbs --upsert --pk path video.db tv.db movies.db
+        library merge-dbs --table media,playlists --pk path audio.db music.db podcasts.db
 """
 
 merge_online_local = """library merge-online-local DATABASE
 
     If you have previously downloaded YouTube or other online media, you can dedupe
     your database and combine the online and local media records as long as your
     files have the youtube-dl / yt-dlp id in the filename.
@@ -748,19 +785,19 @@
 relmv = """library relmv [--dry-run] SOURCE ... DEST
 
     Move files/folders without losing hierarchy metadata
 
     Move fresh music to your phone every Sunday:
 
         # move last weeks' music back to their source folders
-        lb relmv /mnt/d/80_Now_Listening/ /mnt/d/
+        library relmv /mnt/d/80_Now_Listening/ /mnt/d/
 
         # move new music for this week
-        lb relmv (
-            lb listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
+        library relmv (
+            library listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
         ) /mnt/d/80_Now_Listening/
 """
 
 scatter = """library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS database relative_paths ...
 
     Balance size
```

### Comparing `xklb-1.29.7/xklb/utils.py` & `xklb-1.29.8/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/bigdirs.py` & `xklb-1.29.8/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/christen.py` & `xklb-1.29.8/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/cluster_sort.py` & `xklb-1.29.8/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/copy_play_counts.py` & `xklb-1.29.8/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/dedupe.py` & `xklb-1.29.8/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/download_status.py` & `xklb-1.29.8/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/history.py` & `xklb-1.29.8/xklb/scripts/history.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,17 @@
 
 def print_recent(tbl, time_column=None):
     utils.col_duration(tbl, "duration")
     if time_column:
         utils.col_naturaldate(tbl, time_column)
     tbl = [{"title_path": f"{d['title']}\n{d['path']}" if d["title"] is not None else d["path"], **d} for d in tbl]
     tbl = [{k: v for k, v in d.items() if k not in ("title", "path")} for d in tbl]
+
+    tbl = utils.col_resize(tbl, "title_path", 40)
+    tbl = utils.col_resize(tbl, "duration", 5)
     tbl = utils.list_dict_filter_bool(tbl)
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
 
 def recent_media(args, time_column):
     query = f"""
     SELECT
@@ -92,14 +95,16 @@
 
 
 def history() -> None:
     args = parse_args()
 
     if args.facet.startswith(("all", "watching")):
         print("Partially watched:")
+        tbl = player.historical_usage(args, args.frequency, f"time_played", "and coalesce(play_count, 0)=0")
+        print_history(tbl)
         query = f"""SELECT
                 path
                 , title
                 , duration
                 , subtitle_count
                 , time_played
                 , playhead
@@ -108,34 +113,32 @@
                 and coalesce(playhead, 0)>0
                 and coalesce(play_count, 0)=0
             ORDER BY time_played desc, playhead desc
             LIMIT {args.limit or 5}
         """
         tbl = list(args.db.query(query))
         print_recent(tbl, "time_played")
-        tbl = player.historical_usage(args, args.frequency, f"time_played", "and coalesce(play_count, 0)=0")
-        print_history(tbl)
 
     elif args.facet.startswith(("all", "watched")):
         print("Finished watching:")
+        tbl = player.historical_usage(args, args.frequency, f"time_played", "and coalesce(play_count, 0)>0")
+        print_history(tbl)
         query = f"""SELECT
                 path
                 , title
                 , duration
                 , subtitle_count
                 , time_played
             FROM media
             WHERE coalesce(play_count, 0)>0
             ORDER BY time_played desc, path
             LIMIT {args.limit or 5}
         """
         tbl = list(args.db.query(query))
         print_recent(tbl, "time_played")
-        tbl = player.historical_usage(args, args.frequency, f"time_played", "and coalesce(play_count, 0)>0")
-        print_history(tbl)
 
     else:
         print(f"{args.facet.title()} media:")
         tbl = player.historical_usage(args, args.frequency, f"time_{args.facet}")
         print_history(tbl)
         tbl = recent_media(args, f"time_{args.facet}")
         print_recent(tbl, f"time_{args.facet}")
```

### Comparing `xklb-1.29.7/xklb/scripts/merge_dbs.py` & `xklb-1.29.8/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/merge_online_local.py` & `xklb-1.29.8/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/move_list.py` & `xklb-1.29.8/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/optimize_db.py` & `xklb-1.29.8/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/playlists.py` & `xklb-1.29.8/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/redownload.py` & `xklb-1.29.8/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/relmv.py` & `xklb-1.29.8/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/scatter.py` & `xklb-1.29.8/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/streaming_tab_loader.py` & `xklb-1.29.8/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/mining/data.py` & `xklb-1.29.8/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/mining/extract_links.py` & `xklb-1.29.8/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/mining/nouns.py` & `xklb-1.29.8/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/mining/pushshift.py` & `xklb-1.29.8/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.29.8/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/xklb/assets/kotobago.png` & `xklb-1.29.8/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/.gitignore` & `xklb-1.29.8/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/LICENSE` & `xklb-1.29.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/README.md` & `xklb-1.29.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.29.007)
+    xk media library subcommands (v1.29.008)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -588,15 +588,15 @@
 
         library tubeadd reddit.db --playlist-db media
 
     You can also include a category for file organization
 
         library tubeadd -c Mealtime dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
 
-    Files will be saved to <lb download prefix>/<lb tubeadd category>/
+    Files will be saved to <download prefix>/<tubeadd category>/
 
         For example:
         library tubeadd -c Cool ...
         library download D:\'My Documents'\ ...
         Media will be downloaded to 'D:\My Documents\Cool\'
 
     Fetch extra metadata:
@@ -747,15 +747,15 @@
         library watch --print --limit 10  # print the next 10 files
         library watch -p -L 10  # print the next 10 files
         library watch -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
 
         Printing modes
         library watch -p    # print as a table
         library watch -p a  # print an aggregate report
-        library watch -p b  # print a bigdirs report (see lb bigdirs -h for more info)
+        library watch -p b  # print a bigdirs report (see library bigdirs -h for more info)
         library watch -p f  # print fields (defaults to path; use --cols to change)
                                # -- useful for piping paths to utilities like xargs or GNU Parallel
 
         library watch -p d  # mark deleted
         library watch -p w  # mark watched
 
         Some printing modes can be combined
@@ -957,14 +957,62 @@
 
     Search and open file
     $ library search fts.db dashi --open
 
 
 </details>
 
+<details><summary>History</summary>
+
+    $ library history -h
+    usage: library history [--frequency daily|weekly|{monthly}|quarterly|yearly] [--limit LIMIT] DATABASE [{all}|watching|watched|deleted|created|modified]
+
+    Explore history through different facets
+
+    $ library history video.db watched
+    Finished watching:
+    ╒═══════════════╤═════════════════════════════════╤════════════════╤════════════╤════════════╕
+    │ time_period   │ duration_sum                    │ duration_avg   │ size_sum   │ size_avg   │
+    ╞═══════════════╪═════════════════════════════════╪════════════════╪════════════╪════════════╡
+    │ 2022-11       │ 4 days, 16 hours and 20 minutes │ 55.23 minutes  │ 26.3 GB    │ 215.9 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2022-12       │ 23 hours and 20.03 minutes      │ 35.88 minutes  │ 8.3 GB     │ 213.8 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-01       │ 17 hours and 3.32 minutes       │ 15.27 minutes  │ 14.3 GB    │ 214.1 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-02       │ 4 days, 5 hours and 60 minutes  │ 23.17 minutes  │ 148.3 GB   │ 561.6 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-03       │ 2 days, 18 hours and 18 minutes │ 11.20 minutes  │ 118.1 GB   │ 332.8 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-05       │ 5 days, 5 hours and 4 minutes   │ 45.75 minutes  │ 152.9 GB   │ 932.1 MB   │
+    ╘═══════════════╧═════════════════════════════════╧════════════════╧════════════╧════════════╛
+
+    $ library history video.db deleted
+    Deleted media:
+    ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
+    │ time_period   │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
+    ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
+    │ 2023-04       │ 1 year, 10 months, 3 days and 8 hours      │ 4.47 minutes   │ 1.6 TB     │ 7.4 MB     │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-05       │ 9 months, 26 days, 20 hours and 34 minutes │ 30.35 minutes  │ 1.1 TB     │ 73.7 MB    │
+    ╘═══════════════╧════════════════════════════════════════════╧════════════════╧════════════╧════════════╛
+    ╒════════════════════════════════════════════════════════════════════════════════════════════════════════════╤═══════════════╤══════════════════╤════════════════╕
+    │ title_path                                                                                                 │ duration      │   subtitle_count │ time_deleted   │
+    ╞════════════════════════════════════════════════════════════════════════════════════════════════════════════╪═══════════════╪══════════════════╪════════════════╡
+    │ Terminus (1987)                                                                                            │ 1 hour and    │                0 │ yesterday      │
+    │ /mnt/d/70_Now_Watching/Terminus_1987.mp4                                                                   │ 15.55 minutes │                  │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼──────────────────┼────────────────┤
+    │ Commodore 64 Longplay [062] The Transformers (EU) /mnt/d/71_Mealtime_Videos/Youtube/World_of_Longplays/Com │ 24.77 minutes │                2 │ yesterday      │
+    │ modore_64_Longplay_062_The_Transformers_EU_[1RRX7Kykb38].webm                                              │               │                  │                │
+    ...
+
+
+
+</details>
+
 <details><summary>Open tabs</summary>
 
     $ library tabs -h
     usage: library tabs DATABASE
 
     Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
 
@@ -976,15 +1024,15 @@
 
     You can also invoke tabs manually:
 
         library tabs -L 1  # open one tab
 
     Print URLs
 
-        lb-dev tabs -w "frequency='yearly'" -p
+        library tabs -w "frequency='yearly'" -p
         ╒════════════════════════════════════════════════════════════════╤═════════════╤══════════════╕
         │ path                                                           │ frequency   │ time_valid   │
         ╞════════════════════════════════════════════════════════════════╪═════════════╪══════════════╡
         │ https://old.reddit.com/r/Autonomia/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
         ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
         ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
@@ -1074,17 +1122,17 @@
         ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
         │ Playlist-less media │ Youtube    │ 7.68 minutes     │                 99 │        1 │
         ╘═════════════════════╧════════════╧══════════════════╧════════════════════╧══════════╛
 
 
 </details>
 
-<details><summary>Show Download Status (download_status)</summary>
+<details><summary>Download Status (download-status)</summary>
 
-    $ library download_status -h
+    $ library download-status -h
     usage: library download-status [database]
 
     Print download queue groups
 
         library download-status video.db
         ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
         │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
@@ -1255,29 +1303,29 @@
 <details><summary>Show large folders (bigdirs)</summary>
 
     $ library bigdirs -h
     usage: library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by "deleted" | "played"] [--size=+5MB]
 
     See what folders take up space
 
-        lb bigdirs video.db
-        lb bigdirs audio.db
-        lb bigdirs fs.db
+        library bigdirs video.db
+        library bigdirs audio.db
+        library bigdirs fs.db
 
 
 </details>
 
 <details><summary>Copy play history (copy-play-counts)</summary>
 
     $ library copy-play-counts -h
     usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
 
     Copy play count information between databases
 
-        lb copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
+        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 
 
 </details>
 
 <details><summary>Dedupe music</summary>
 
     $ library dedupe -h
@@ -1367,16 +1415,16 @@
 <details><summary>Merge SQLITE databases (merge-dbs)</summary>
 
     $ library merge-dbs -h
     usage: library merge-dbs DEST_DB SOURCE_DB ... [--upsert pk1[,pk2]]
 
     Merge database data and tables
 
-        lb merge-dbs --upsert --pk path video.db tv.db movies.db
-        lb merge-dbs --table media,playlists --pk path audio.db music.db podcasts.db
+        library merge-dbs --upsert --pk path video.db tv.db movies.db
+        library merge-dbs --table media,playlists --pk path audio.db music.db podcasts.db
 
 
 </details>
 
 <details><summary>Sort lines by similarity (cluster-sort)</summary>
 
     $ library cluster-sort -h
@@ -1393,19 +1441,19 @@
     usage: library relmv [--dry-run] SOURCE ... DEST
 
     Move files/folders without losing hierarchy metadata
 
     Move fresh music to your phone every Sunday:
 
         # move last weeks' music back to their source folders
-        lb relmv /mnt/d/80_Now_Listening/ /mnt/d/
+        library relmv /mnt/d/80_Now_Listening/ /mnt/d/
 
         # move new music for this week
-        lb relmv (
-            lb listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
+        library relmv (
+            library listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
         ) /mnt/d/80_Now_Listening/
 
 
 </details>
 
 <details><summary>Automatic tab loader (surf)</summary>
 
@@ -1432,23 +1480,23 @@
     $ library christen -h
     usage: library christen DATABASE [--run]
 
     Rename files to be somewhat normalized
 
     Default mode is dry-run
 
-        lb christen fs.db
+        library christen fs.db
 
     To actually do stuff use the run flag
 
-        lb christen audio.db --run
+        library christen audio.db --run
 
     You can optionally replace all the spaces in your filenames with dots
 
-        lb christen --dot-space video.db
+        library christen --dot-space video.db
 
 
 </details>
 
 
 You can expand all by running this in your browser console:
```

### Comparing `xklb-1.29.7/pyproject.toml` & `xklb-1.29.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.29.7/PKG-INFO` & `xklb-1.29.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.29.7
+Version: 1.29.8
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -223,15 +223,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.29.007)
+    xk media library subcommands (v1.29.008)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -672,15 +672,15 @@
 
         library tubeadd reddit.db --playlist-db media
 
     You can also include a category for file organization
 
         library tubeadd -c Mealtime dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
 
-    Files will be saved to <lb download prefix>/<lb tubeadd category>/
+    Files will be saved to <download prefix>/<tubeadd category>/
 
         For example:
         library tubeadd -c Cool ...
         library download D:\'My Documents'\ ...
         Media will be downloaded to 'D:\My Documents\Cool\'
 
     Fetch extra metadata:
@@ -831,15 +831,15 @@
         library watch --print --limit 10  # print the next 10 files
         library watch -p -L 10  # print the next 10 files
         library watch -p  # this will print _all_ the media. be cautious about `-p` on an unfiltered set
 
         Printing modes
         library watch -p    # print as a table
         library watch -p a  # print an aggregate report
-        library watch -p b  # print a bigdirs report (see lb bigdirs -h for more info)
+        library watch -p b  # print a bigdirs report (see library bigdirs -h for more info)
         library watch -p f  # print fields (defaults to path; use --cols to change)
                                # -- useful for piping paths to utilities like xargs or GNU Parallel
 
         library watch -p d  # mark deleted
         library watch -p w  # mark watched
 
         Some printing modes can be combined
@@ -1041,14 +1041,62 @@
 
     Search and open file
     $ library search fts.db dashi --open
 
 
 </details>
 
+<details><summary>History</summary>
+
+    $ library history -h
+    usage: library history [--frequency daily|weekly|{monthly}|quarterly|yearly] [--limit LIMIT] DATABASE [{all}|watching|watched|deleted|created|modified]
+
+    Explore history through different facets
+
+    $ library history video.db watched
+    Finished watching:
+    ╒═══════════════╤═════════════════════════════════╤════════════════╤════════════╤════════════╕
+    │ time_period   │ duration_sum                    │ duration_avg   │ size_sum   │ size_avg   │
+    ╞═══════════════╪═════════════════════════════════╪════════════════╪════════════╪════════════╡
+    │ 2022-11       │ 4 days, 16 hours and 20 minutes │ 55.23 minutes  │ 26.3 GB    │ 215.9 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2022-12       │ 23 hours and 20.03 minutes      │ 35.88 minutes  │ 8.3 GB     │ 213.8 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-01       │ 17 hours and 3.32 minutes       │ 15.27 minutes  │ 14.3 GB    │ 214.1 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-02       │ 4 days, 5 hours and 60 minutes  │ 23.17 minutes  │ 148.3 GB   │ 561.6 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-03       │ 2 days, 18 hours and 18 minutes │ 11.20 minutes  │ 118.1 GB   │ 332.8 MB   │
+    ├───────────────┼─────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-05       │ 5 days, 5 hours and 4 minutes   │ 45.75 minutes  │ 152.9 GB   │ 932.1 MB   │
+    ╘═══════════════╧═════════════════════════════════╧════════════════╧════════════╧════════════╛
+
+    $ library history video.db deleted
+    Deleted media:
+    ╒═══════════════╤════════════════════════════════════════════╤════════════════╤════════════╤════════════╕
+    │ time_period   │ duration_sum                               │ duration_avg   │ size_sum   │ size_avg   │
+    ╞═══════════════╪════════════════════════════════════════════╪════════════════╪════════════╪════════════╡
+    │ 2023-04       │ 1 year, 10 months, 3 days and 8 hours      │ 4.47 minutes   │ 1.6 TB     │ 7.4 MB     │
+    ├───────────────┼────────────────────────────────────────────┼────────────────┼────────────┼────────────┤
+    │ 2023-05       │ 9 months, 26 days, 20 hours and 34 minutes │ 30.35 minutes  │ 1.1 TB     │ 73.7 MB    │
+    ╘═══════════════╧════════════════════════════════════════════╧════════════════╧════════════╧════════════╛
+    ╒════════════════════════════════════════════════════════════════════════════════════════════════════════════╤═══════════════╤══════════════════╤════════════════╕
+    │ title_path                                                                                                 │ duration      │   subtitle_count │ time_deleted   │
+    ╞════════════════════════════════════════════════════════════════════════════════════════════════════════════╪═══════════════╪══════════════════╪════════════════╡
+    │ Terminus (1987)                                                                                            │ 1 hour and    │                0 │ yesterday      │
+    │ /mnt/d/70_Now_Watching/Terminus_1987.mp4                                                                   │ 15.55 minutes │                  │                │
+    ├────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼──────────────────┼────────────────┤
+    │ Commodore 64 Longplay [062] The Transformers (EU) /mnt/d/71_Mealtime_Videos/Youtube/World_of_Longplays/Com │ 24.77 minutes │                2 │ yesterday      │
+    │ modore_64_Longplay_062_The_Transformers_EU_[1RRX7Kykb38].webm                                              │               │                  │                │
+    ...
+
+
+
+</details>
+
 <details><summary>Open tabs</summary>
 
     $ library tabs -h
     usage: library tabs DATABASE
 
     Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
 
@@ -1060,15 +1108,15 @@
 
     You can also invoke tabs manually:
 
         library tabs -L 1  # open one tab
 
     Print URLs
 
-        lb-dev tabs -w "frequency='yearly'" -p
+        library tabs -w "frequency='yearly'" -p
         ╒════════════════════════════════════════════════════════════════╤═════════════╤══════════════╕
         │ path                                                           │ frequency   │ time_valid   │
         ╞════════════════════════════════════════════════════════════════╪═════════════╪══════════════╡
         │ https://old.reddit.com/r/Autonomia/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
         ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
         ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
@@ -1158,17 +1206,17 @@
         ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
         │ Playlist-less media │ Youtube    │ 7.68 minutes     │                 99 │        1 │
         ╘═════════════════════╧════════════╧══════════════════╧════════════════════╧══════════╛
 
 
 </details>
 
-<details><summary>Show Download Status (download_status)</summary>
+<details><summary>Download Status (download-status)</summary>
 
-    $ library download_status -h
+    $ library download-status -h
     usage: library download-status [database]
 
     Print download queue groups
 
         library download-status video.db
         ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
         │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
@@ -1339,29 +1387,29 @@
 <details><summary>Show large folders (bigdirs)</summary>
 
     $ library bigdirs -h
     usage: library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by "deleted" | "played"] [--size=+5MB]
 
     See what folders take up space
 
-        lb bigdirs video.db
-        lb bigdirs audio.db
-        lb bigdirs fs.db
+        library bigdirs video.db
+        library bigdirs audio.db
+        library bigdirs fs.db
 
 
 </details>
 
 <details><summary>Copy play history (copy-play-counts)</summary>
 
     $ library copy-play-counts -h
     usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
 
     Copy play count information between databases
 
-        lb copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
+        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
 
 
 </details>
 
 <details><summary>Dedupe music</summary>
 
     $ library dedupe -h
@@ -1451,16 +1499,16 @@
 <details><summary>Merge SQLITE databases (merge-dbs)</summary>
 
     $ library merge-dbs -h
     usage: library merge-dbs DEST_DB SOURCE_DB ... [--upsert pk1[,pk2]]
 
     Merge database data and tables
 
-        lb merge-dbs --upsert --pk path video.db tv.db movies.db
-        lb merge-dbs --table media,playlists --pk path audio.db music.db podcasts.db
+        library merge-dbs --upsert --pk path video.db tv.db movies.db
+        library merge-dbs --table media,playlists --pk path audio.db music.db podcasts.db
 
 
 </details>
 
 <details><summary>Sort lines by similarity (cluster-sort)</summary>
 
     $ library cluster-sort -h
@@ -1477,19 +1525,19 @@
     usage: library relmv [--dry-run] SOURCE ... DEST
 
     Move files/folders without losing hierarchy metadata
 
     Move fresh music to your phone every Sunday:
 
         # move last weeks' music back to their source folders
-        lb relmv /mnt/d/80_Now_Listening/ /mnt/d/
+        library relmv /mnt/d/80_Now_Listening/ /mnt/d/
 
         # move new music for this week
-        lb relmv (
-            lb listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
+        library relmv (
+            library listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
         ) /mnt/d/80_Now_Listening/
 
 
 </details>
 
 <details><summary>Automatic tab loader (surf)</summary>
 
@@ -1516,23 +1564,23 @@
     $ library christen -h
     usage: library christen DATABASE [--run]
 
     Rename files to be somewhat normalized
 
     Default mode is dry-run
 
-        lb christen fs.db
+        library christen fs.db
 
     To actually do stuff use the run flag
 
-        lb christen audio.db --run
+        library christen audio.db --run
 
     You can optionally replace all the spaces in your filenames with dots
 
-        lb christen --dot-space video.db
+        library christen --dot-space video.db
 
 
 </details>
 
 
 You can expand all by running this in your browser console:
```

