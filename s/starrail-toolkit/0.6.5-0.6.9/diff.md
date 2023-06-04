# Comparing `tmp/starrail-toolkit-0.6.5.tar.gz` & `tmp/starrail-toolkit-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.6.5.tar", last modified: Fri May 26 18:16:20 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.6.9.tar", last modified: Sun Jun  4 17:42:25 2023, max compression
```

## Comparing `starrail-toolkit-0.6.5.tar` & `starrail-toolkit-0.6.9.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.762319 starrail-toolkit-0.6.5/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.5/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     6145 2023-05-26 18:16:20.762148 starrail-toolkit-0.6.5/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     5638 2023-05-26 18:14:07.000000 starrail-toolkit-0.6.5/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-26 18:16:20.762368 starrail-toolkit-0.6.5/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-15 03:28:48.000000 starrail-toolkit-0.6.5/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.754496 starrail-toolkit-0.6.5/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.755015 starrail-toolkit-0.6.5/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3650 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.756449 starrail-toolkit-0.6.5/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-26 04:24:47.000000 starrail-toolkit-0.6.5/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3549 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6284 2023-05-26 04:23:47.000000 starrail-toolkit-0.6.5/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1318 2023-05-26 04:23:17.000000 starrail-toolkit-0.6.5/starrail/gacha/factory.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1134 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6566 2023-05-26 04:12:49.000000 starrail-toolkit-0.6.5/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1080 2023-05-26 04:23:17.000000 starrail-toolkit-0.6.5/starrail/gacha/migrate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     7702 2023-05-26 09:09:00.000000 starrail-toolkit-0.6.5/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4854 2023-05-26 18:02:21.000000 starrail-toolkit-0.6.5/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.756699 starrail-toolkit-0.6.5/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6509 2023-05-26 09:49:54.000000 starrail-toolkit-0.6.5/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.757333 starrail-toolkit-0.6.5/starrail/gui/common/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/common/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1916 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/common/config.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      282 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/common/icon.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      645 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/common/stylesheet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/common/utils.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.758335 starrail-toolkit-0.6.5/starrail/gui/interfaces/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/base.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    21352 2023-05-26 18:02:38.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/gacha_sync.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/home.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5635 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/setting.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/unlock_fps.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      372 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/interfaces/users.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.758983 starrail-toolkit-0.6.5/starrail/gui/widgets/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/widgets/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/widgets/dialog.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/widgets/link_card.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2830 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/widgets/pie_chart.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/gui/widgets/title_bar.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.759364 starrail-toolkit-0.6.5/starrail/unlock/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/unlock/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/unlock/fps.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/unlock/service.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.760113 starrail-toolkit-0.6.5/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1804 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/accounts.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.760988 starrail-toolkit-0.6.5/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)     4783 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/constants.py
--rw-r--r--   0 littlenyima   (501) staff       (20)    10001 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      597 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      765 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-05-26 03:35:53.000000 starrail-toolkit-0.6.5/starrail/utils/misc.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-05-26 18:04:11.000000 starrail-toolkit-0.6.5/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-26 18:16:20.761878 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     6145 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     1755 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-26 18:16:20.000000 starrail-toolkit-0.6.5/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.614493 starrail-toolkit-0.6.9/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6000 2023-06-04 17:42:25.614354 starrail-toolkit-0.6.9/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5493 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-06-04 17:42:25.614531 starrail-toolkit-0.6.9/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.607913 starrail-toolkit-0.6.9/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      760 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1838 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.608364 starrail-toolkit-0.6.9/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3827 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1056 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1494 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.609546 starrail-toolkit-0.6.9/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3549 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6284 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1318 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/factory.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1134 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6566 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1080 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/migrate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     7702 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6287 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3489 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.609750 starrail-toolkit-0.6.9/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6752 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.610352 starrail-toolkit-0.6.9/starrail/gui/common/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/common/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1916 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/common/config.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      304 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gui/common/icon.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      645 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/common/stylesheet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      576 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gui/common/thread.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1516 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/common/utils.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.611080 starrail-toolkit-0.6.9/starrail/gui/interfaces/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3713 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/base.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    26369 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/gacha_sync.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2536 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/home.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5635 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/setting.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4476 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/unlock_fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3046 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/gui/interfaces/users.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.611580 starrail-toolkit-0.6.9/starrail/gui/widgets/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/widgets/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5438 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/widgets/dialog.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2509 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/widgets/link_card.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2830 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/widgets/pie_chart.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1841 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/gui/widgets/title_bar.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.611872 starrail-toolkit-0.6.9/starrail/unlock/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/unlock/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2327 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/unlock/fps.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      182 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/unlock/service.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.612574 starrail-toolkit-0.6.9/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     2459 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/utils/accounts.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      948 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.613387 starrail-toolkit-0.6.9/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5198 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      230 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/constants.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)    10670 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      597 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      765 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      144 2023-06-02 03:58:21.000000 starrail-toolkit-0.6.9/starrail/utils/misc.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      106 2023-06-04 14:27:29.000000 starrail-toolkit-0.6.9/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-06-04 17:42:25.614170 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6000 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1785 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       87 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-06-04 17:42:25.000000 starrail-toolkit-0.6.9/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.6.5/LICENSE` & `starrail-toolkit-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/PKG-INFO` & `starrail-toolkit-0.6.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,41 @@
-Metadata-Version: 2.1
-Name: starrail-toolkit
-Version: 0.6.5
-Summary: Honkai Star Rail Toolkit
-Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
-Author: LittleNyima
-Author-email: littlenyima@163.com
-License: GPLv3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
-<b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
-
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.5    |    0.6.5     |   0.6.5   |   0.6.5    |
+|   0.6.9    |    0.6.9     |   0.6.9   |   0.6.9    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 支持更多的可设置选项
-- [ ] 支持国际服
 - [x] 支持解锁120帧
 - [x] 支持以 SRGF 标准导出
-- [ ] 支持以 SRGF 标准导入
-- [ ] 支持手动设置 API URL
+- [x] 支持以 SRGF 标准导入
+- [x] 支持手动设置 API URL
 - [x] 支持夜间模式
-- [ ] 支持多用户切换
-- [ ] 美化程序界面
+- [x] 支持多用户切换
+- [x] 美化程序界面
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouk.com/ig3lR0xdvwwh)，两种途径的内容相同，可以自行选择下载方式。
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouk.com/iN7870y9o7gb)，两种途径的内容相同，可以自行选择下载方式。
 
-***BREAKING：目前用户界面正在优化中，预览如下图所示。***（注意：该版本尚未发布，所以 release 中仍然是旧版界面，且该界面正在调试过程中，可能会有一些问题，如果出现问题，请先下载旧版 release 使用。）
-
-![gui preview gacha](https://s1.ax1x.com/2023/05/25/p9HOzLQ.png)
+![gui preview gacha](https://s1.ax1x.com/2023/06/01/p9xxdXj.png)
 
 ![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
@@ -69,14 +49,20 @@
 
 ```shell
 git clone git@github.com:LittleNyima/honkai-starrail-toolkit.git
 cd honkai-starrail-toolkit
 python3 setup.py install
 ```
 
+注：如果出现关于 `qfluentwidgets` 相关的报错，可能是因为默认 pypi 源的版本较低，可以使用以下命令安装最新版本的依赖：
+
+```
+pip install -U PySide6-Fluent-Widgets -i https://pypi.org/simple/
+```
+
 ##  命令行使用指南
 
 ### 获取抽卡查询 API URL
 
 请参考[这个教程](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
```

### Comparing `starrail-toolkit-0.6.5/setup.py` & `starrail-toolkit-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/__init__.py` & `starrail-toolkit-0.6.9/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/config.py` & `starrail-toolkit-0.6.9/starrail/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/entry/cli.py` & `starrail-toolkit-0.6.9/starrail/entry/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import traceback
 
 from starrail import __version__, digital_version
 from starrail.config import configuration as cfg
 from starrail.entry.setup import setup
-from starrail.gacha.service import export_gacha_from_api
+from starrail.gacha.service import export_gacha_from_api, import_srgf_data
 from starrail.unlock.service import unlock_fps
 from starrail.utils import babelfish, loggings
 from starrail.utils.auto_update import check_update
 
 logger = loggings.get_logger(__file__)
 
 
@@ -40,14 +40,18 @@
     )
     gacha.add_argument(
         '--export', nargs='+', type=str, default=['all'],
         choices=['all', 'csv', 'html', 'json', 'md', 'srgf', 'xlsx'],
         help='Types of expected export formats.',
     )
     gacha.add_argument(
+        '--load', type=str,
+        help='Import source json under SRGF standard.',
+    )
+    gacha.add_argument(
         '--request-interval', type=float, default=0.1,
         help='Minimum interval (seconds) between two requests.',
     )
 
     unlock = subparsers.add_parser('unlock')
     unlock.add_argument(
         '--fps', type=int,
@@ -91,14 +95,15 @@
     args = parser.parse_args()
     setup(log_level=args.log_level, locale=args.locale)
     logger.info(args)
     logger.info(cfg)
     cli_check_update()
 
     if args.command == 'gacha':
+        import_srgf_data(filename=args.load)
         export_gacha_from_api(
             api_url=args.api,
             export=args.export,
             request_interval=args.request_interval,
         )
     elif args.command == 'unlock':
         unlock_fps(fps=args.fps, reset=args.reset)
```

### Comparing `starrail-toolkit-0.6.5/starrail/entry/gui.py` & `starrail-toolkit-0.6.9/starrail/entry/gui.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/entry/setup.py` & `starrail-toolkit-0.6.9/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gacha/autodet.py` & `starrail-toolkit-0.6.9/starrail/gacha/autodet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gacha/database.py` & `starrail-toolkit-0.6.9/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gacha/factory.py` & `starrail-toolkit-0.6.9/starrail/gacha/factory.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gacha/fetch.py` & `starrail-toolkit-0.6.9/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gacha/fileio.py` & `starrail-toolkit-0.6.9/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gacha/migrate.py` & `starrail-toolkit-0.6.9/starrail/gacha/migrate.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gacha/parse.py` & `starrail-toolkit-0.6.9/starrail/gacha/parse.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gacha/service.py` & `starrail-toolkit-0.6.9/starrail/gacha/service.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
 import os
 import time
+import traceback
+from collections import defaultdict
 
 import starrail.gacha.fileio as fileio
 from starrail.gacha.autodet import detect_api_url
 from starrail.gacha.fetch import fetch_json
 from starrail.gacha.parse import GachaDataManager
 from starrail.gacha.type import GachaType
 from starrail.gacha.url import get_api_url, get_url_template
-from starrail.utils import loggings
+from starrail.utils import babelfish, loggings
 from starrail.utils.accounts import account_record
 
 logger = loggings.get_logger(__file__)
 
 
 def integers():
     r = 1
@@ -138,7 +140,48 @@
         output_dir = os.getcwd()
         filename = f'HKSR-export-{uid}-{timestamp}.{format}'
         if format == 'srgf':
             filename += '.json'
         path = os.path.join(output_dir, filename)
         export_hooks[format](manager, path)
         logger.info(f'Gacha data in {format} format is saved to {path}')
+
+
+def import_srgf_data(filename):
+    if not filename:
+        logger.info('Skipping import srgf data')
+        return
+    try:
+        with open(filename, encoding='utf-8') as f:
+            data = json.load(f)
+        info = data['info']
+        uid = info['uid']
+        update_info = dict(
+            uid=info['uid'],
+            lang=info['lang'],
+            region='',  # unused
+            region_time_zone=str(info['region_time_zone']),
+        )
+        record_cache = defaultdict(list)
+        for item in data['list']:
+            item.update(update_info)
+            record_cache[int(item['gacha_type'])].append(item)
+
+        manager = GachaDataManager(uid=uid)
+        logger.info(f'Successfully connected to cache of uid {uid}')
+        manager.log_stats()
+
+        for k, v in record_cache.items():
+            manager.add_records(k, v)
+            manager.gacha[k].sort()
+
+        fileio.export_as_sql(manager, manager.cache_path)
+
+        timestamp = info['export_timestamp']
+        timestruct = time.localtime(timestamp)
+        timestr = time.strftime(babelfish.constants.TIME_FMT, timestruct)
+        account_record.update_timestamp(uid, timestr)
+
+        logger.info(f'Successfully load gacha data from {filename}')
+    except Exception:
+        logger.error('Import gacha data failed. Traceback:')
+        logger.error(traceback.format_exc())
```

### Comparing `starrail-toolkit-0.6.5/starrail/gacha/url.py` & `starrail-toolkit-0.6.9/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/application.py` & `starrail-toolkit-0.6.9/starrail/gui/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from starrail.gui.interfaces.gacha_sync import GachaSyncInterface
 from starrail.gui.interfaces.home import HomeInterface
 from starrail.gui.interfaces.setting import SettingInterface
 from starrail.gui.interfaces.unlock_fps import UnlockFpsInterface
 from starrail.gui.interfaces.users import UsersInterface
 from starrail.gui.widgets.title_bar import CustomTitleBar
 from starrail.utils import babelfish
+from starrail.utils.accounts import account_record as ar
 
 
 class StackedWidget(QFrame):
 
     currentWidgetChanged = Signal(QWidget)
 
     def __init__(self, parent=None):
@@ -79,14 +80,15 @@
             self,
         )
         self.settingInterface = SettingInterface(self)
 
         self.initLayout()
         self.initNavigation()
         self.initWindow()
+        self.initHooks()
 
     def initLayout(self):
         self.hBoxLayout.setSpacing(0)
         self.hBoxLayout.setContentsMargins(0, 0, 0, 0)
         self.hBoxLayout.addWidget(self.navigationInterface)
         self.hBoxLayout.addLayout(self.widgetLayout)
         self.hBoxLayout.setStretchFactor(self.widgetLayout, 1)
@@ -185,14 +187,18 @@
 
         desktop = QApplication.screens()[0].availableGeometry()
         w, h = desktop.width(), desktop.height()
         self.move(w // 2 - self.width() // 2, h // 2 - self.height() // 2)
 
         StyleSheet.STAR_RAIL_TOOLKIT.apply(self)
 
+    def initHooks(self):
+        ar.latest_uid_changed = self.gachaSyncInterface.updateUidHook
+        ar.accounts_changed = self.usersInterface.updateUserList
+
     def resizeEvent(self, _):
         self.titleBar.move(46, 0)
         self.titleBar.resize(self.width() - 46, self.titleBar.height())
 
     def afterShow(self):
         if qcfg.get(qcfg.check_update):
             checkUpdate(self)
```

### Comparing `starrail-toolkit-0.6.5/starrail/gui/common/config.py` & `starrail-toolkit-0.6.9/starrail/gui/common/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/common/stylesheet.py` & `starrail-toolkit-0.6.9/starrail/gui/common/stylesheet.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/common/utils.py` & `starrail-toolkit-0.6.9/starrail/gui/common/utils.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/interfaces/base.py` & `starrail-toolkit-0.6.9/starrail/gui/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/interfaces/gacha_sync.py` & `starrail-toolkit-0.6.9/starrail/gui/interfaces/gacha_sync.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,41 @@
+import json
 import os
 import time
-import traceback
+from collections import defaultdict
 
 import qfluentwidgets as qfw
 from PySide6 import QtCharts, QtWidgets
-from PySide6.QtCore import Qt, QThread, Signal
+from PySide6.QtCore import Qt, Signal
 from PySide6.QtGui import QPainter
 from PySide6.QtWidgets import QLabel, QVBoxLayout
 
 import starrail.gacha.service as service
 from starrail.gacha.type import GachaType
+from starrail.gui.common.icon import Icon
 from starrail.gui.common.stylesheet import StyleSheet
+from starrail.gui.common.thread import StatefulThread
 from starrail.gui.interfaces.base import BaseInterface, CardWidget
 from starrail.gui.widgets.pie_chart import SmartPieChart
 from starrail.utils import babelfish, loggings
 from starrail.utils.accounts import account_record, get_latest_uid
 
 AF = Qt.AlignmentFlag
 logger = loggings.get_logger(__file__)
 
 
 # = FUNCTIONS =
 
-class GachaSyncThread(QThread):
+class GachaSyncThread(StatefulThread):
 
     syncStateSignal = Signal(str)
-    syncSuccessSignal = Signal(str)
-    syncFailSignal = Signal(str)
 
-    def __init__(self, parent=None):
+    def __init__(self, api_url='', parent=None):
         super().__init__(parent=parent)
-
-    def run(self):
-        try:
-            uid = self.syncGachaData()
-            self.syncSuccessSignal.emit(uid)
-        except Exception:
-            self.syncFailSignal.emit(
-                f'{babelfish.ui_traceback()}:\n{traceback.format_exc()}',
-            )
+        self.api_url = api_url
 
     def logAndUpdateState(self, message, level=loggings.logging.INFO):
         logger.log(level=level, msg=f'[GUI] {message}')
         self.syncStateSignal.emit(message)
 
     def exportGachaType(self, api_template, gacha_type, request_interval):
         r = []
@@ -71,22 +64,22 @@
             metainfo = dict(region=region, region_time_zone=timezone)
             for data_item in data_list:
                 data_item.update(metainfo)
             r.extend(data_list)
             end_id = data_list[-1]['id']
         return r
 
-    def syncGachaData(self):
+    def work(self):
         self.logAndUpdateState(babelfish.ui_extracting_api_url())
-        api_url = service.detect_api_url()
+        api_url = self.api_url or service.detect_api_url()
         response, code = service.fetch_json(api_url)
         valid, _, msg = service.check_response(response, code)
         logger.info(f'check_response (api): {msg}')
         if not valid:
-            self.syncFailSignal.emit(babelfish.ui_extract_api_fail())
+            self.failureSignal.emit(babelfish.ui_extract_api_fail())
             raise ValueError(babelfish.ui_extract_api_fail_with_msg(msg))
 
         api_template = service.get_url_template(api_url)
         record_cache = dict()
 
         for gacha_type in service.GachaType:
             records = self.exportGachaType(
@@ -116,24 +109,68 @@
 
         service.fileio.export_as_sql(manager, manager.cache_path)
         manager.log_stats()
 
         return uid
 
 
-class RecordExportThread(QThread):
+class RecordImportThread(StatefulThread):
+
+    def __init__(self, path, parent=None):
+        super().__init__(parent=parent)
+        self.path = path
 
-    saveSuccessSignal = Signal(str)
+    def work(self):
+        with open(self.path, encoding='utf-8') as f:
+            data = json.load(f)
+        info = data['info']
+        uid = info['uid']
+        update_info = dict(
+            uid=info['uid'],
+            lang=info['lang'],
+            region='',  # unused
+            region_time_zone=str(info['region_time_zone']),
+        )
+        record_cache = defaultdict(list)
+        for item in data['list']:
+            item.update(update_info)
+            record_cache[int(item['gacha_type'])].append(item)
+
+        manager = service.GachaDataManager(uid=uid)
+        logger.info(f'Successfully connected to cache of uid {uid}')
+        manager.log_stats()
+
+        total = 0
+
+        for k, v in record_cache.items():
+            manager.add_records(k, v)
+            manager.gacha[k].sort()
+            total += len(v)
+
+        service.fileio.export_as_sql(manager, manager.cache_path)
+
+        timestamp = info['export_timestamp']
+        timestruct = time.localtime(timestamp)
+        timestr = time.strftime(babelfish.constants.TIME_FMT, timestruct)
+        account_record.update_timestamp(uid, timestr)
+
+        logger.info(f'Successfully load gacha data from {self.path}')
+        msg = babelfish.ui_load_success_msg(uid=uid, cnt=total)
+        # return msg: {uid: uid, msg: msg}
+        return json.dumps(dict(uid=uid, msg=msg), ensure_ascii=False)
+
+
+class RecordExportThread(StatefulThread):
 
     def __init__(self, uid, path, parent=None):
         super().__init__(parent=parent)
         self.uid = uid
         self.path = path
 
-    def run(self):
+    def work(self):
         manager = service.GachaDataManager(self.uid)
         export_hooks = dict(
             csv=service.fileio.export_as_csv,
             html=service.fileio.export_as_html,
             json=service.fileio.export_as_json,
             md=service.fileio.export_as_md,
             srgf=service.fileio.export_as_srgf,
@@ -142,15 +179,16 @@
         timestamp = time.strftime('%Y%m%d%H%M%S')
         for format, hook in export_hooks.items():
             if format == 'srgf':
                 format = 'srgf.json'
             filename = f'HKSR-export-{self.uid}-{timestamp}.{format}'
             export_path = os.path.join(self.path, filename)
             hook(manager, export_path)
-        self.saveSuccessSignal.emit(self.path)
+
+        return self.path
 
 # = UI =
 
 
 pie_chart_mapping = {
     GachaType.CHARACTER: [
         (babelfish.ui_5star_character(),  'redLegend',    '#e52f2f'),
@@ -391,36 +429,60 @@
         self.saveButton = qfw.PrimaryPushButton(
             text=babelfish.ui_save_data(),
             parent=self,
             icon=qfw.FluentIcon.SAVE_AS,
         )
         self.saveButton.clicked.connect(self.onSaveButtonClicked)
         self.saveButton.setDisabled(True)
+        self.loadButton = qfw.PrimaryPushButton(
+            text=babelfish.ui_load_gacha(),
+            parent=self,
+            icon=Icon.FILE_IMPORT,
+        )
+        self.loadButton.clicked.connect(self.onLoadButtonClicked)
+        self.urlCard = self.addCard(babelfish.ui_customize_url())
+        self.urlCheckbox = qfw.CheckBox(
+            text=babelfish.ui_use_customize_url(),
+            parent=self,
+        )
+        self.urlCheckbox.stateChanged.connect(self.onCheckboxChanged)
+        self.urlLineEdit = qfw.LineEdit(parent=self)
+        default_url = 'https://api-takumi.mihoyo.com/common/gacha_record/...'
+        self.urlLineEdit.setText(default_url)
+        self.urlLineEdit.setDisabled(True)
+        self.urlLineEdit.setClearButtonEnabled(False)
 
         self.__initRecordCards()
 
         # Gacha Sync Temp Objects
         self.syncThread = None
         self.syncToolTip = None
         self.saveThread = None
+        self.loadThread = None
 
         self.uid = get_latest_uid()
         logger.info(f'Detected current uid: {self.uid}')
         if self.uid:
             self.saveButton.setEnabled(True)
             self.updateRecordDisplay()
 
         self.__initWidget()
 
     def __initWidget(self):
         self.buttonsCard.addWidget(self.syncButton)
         self.buttonsCard.addSpacing(10)
         self.buttonsCard.addWidget(self.saveButton)
+        self.buttonsCard.addSpacing(10)
+        self.buttonsCard.addWidget(self.loadButton)
         self.buttonsCard.addStretch(1)
 
+        self.urlCard.addWidget(self.urlCheckbox)
+        self.urlCard.addSpacing(20)  # 10 (from line edit) + 10 (spacing)
+        self.urlCard.addWidget(self.urlLineEdit)
+
     def __initRecordCards(self):
         self.characterCard = self.addResultCard(
             GachaType.CHARACTER,
             babelfish.translate('CHARACTER'),
         )
         self.lightConeCard = self.addResultCard(
             GachaType.LIGHT_CONE,
@@ -466,76 +528,118 @@
             )
 
     def resizeEvent(self, e):
         if self.syncToolTip:
             self.syncToolTip.move(self.syncToolTip.getSuitablePos())
         return super().resizeEvent(e)
 
+    def disableButtons(self):
+        self.syncButton.setDisabled(True)
+        self.saveButton.setDisabled(True)
+        self.loadButton.setDisabled(True)
+
+    def enableButtons(self):
+        self.syncButton.setEnabled(True)
+        self.saveButton.setEnabled(True)
+        self.loadButton.setEnabled(True)
+
+    # == HOOKS ==
+
+    def updateUidHook(self, uid):
+        self.uid = uid
+        self.updateRecordDisplay()
+
     # == SLOTS ==
 
     def onSyncButtonClicked(self):
         logger.info('[GUI] Start gacha data synchronization')
 
-        self.syncButton.setDisabled(True)
-        self.saveButton.setDisabled(True)
+        self.disableButtons()
 
         self.syncToolTip = qfw.StateToolTip(
             babelfish.ui_synchronizing_gacha(),
             babelfish.ui_sync_gacha_initial(),
             self.window(),
         )
         self.syncToolTip.move(self.syncToolTip.getSuitablePos())
         self.syncToolTip.show()
 
-        self.syncThread = GachaSyncThread(self)
+        api_url = ''
+        if self.urlCheckbox.checkState() == Qt.CheckState.Checked:
+            api_url = self.urlLineEdit.text().strip()
+        self.syncThread = GachaSyncThread(api_url=api_url, parent=self)
         self.syncThread.syncStateSignal.connect(
             lambda s: self.setToolTipContentSlot(self.syncToolTip, s),
         )
-        self.syncThread.syncSuccessSignal.connect(self.syncSuccessSlot)
-        self.syncThread.syncFailSignal.connect(self.syncFailSlot)
+        self.syncThread.successSignal.connect(self.syncSuccessSlot)
+        self.syncThread.failureSignal.connect(self.syncFailureSlot)
         self.syncThread.start()
 
     def onSaveButtonClicked(self):
         logger.info('[GUI] Start gacha data exporting')
 
-        self.syncButton.setDisabled(True)
-        self.saveButton.setDisabled(True)
+        self.disableButtons()
 
         path = QtWidgets.QFileDialog.getExistingDirectory(
             self, 'Select Export Folder', os.path.expanduser('~'),
         )
         if path:
             self.saveThread = RecordExportThread(self.uid, path, self)
-            self.saveThread.saveSuccessSignal.connect(self.saveSuccessSlot)
+            self.saveThread.successSignal.connect(self.saveSuccessSlot)
+            self.saveThread.failureSignal.connect(self.saveFailureSlot)
             self.saveThread.start()
         else:
-            self.syncButton.setEnabled(True)
-            self.saveButton.setEnabled(True)
+            self.enableButtons()
+
+    def onLoadButtonClicked(self):
+        logger.info('[GUI] Trying to load gacha data')
+
+        self.disableButtons()
+
+        path, _ = QtWidgets.QFileDialog.getOpenFileName(
+            parent=self,
+            caption='Select Import File',
+            dir=os.path.expanduser('~'),
+            filter='JSON Files (*.json);;All Files (*)',
+        )
+        if path:
+            self.loadThread = RecordImportThread(path=path, parent=self)
+            self.loadThread.successSignal.connect(self.loadSuccessSlot)
+            self.loadThread.failureSignal.connect(self.loadFailureSlot)
+            self.loadThread.start()
+        else:
+            self.enableButtons()
+
+    def onCheckboxChanged(self, status):
+        if status == Qt.CheckState.Checked.value:  # enabled
+            self.urlLineEdit.setEnabled(True)
+            self.urlLineEdit.setClearButtonEnabled(True)
+        elif status == Qt.CheckState.Unchecked.value:  # disabled
+            self.urlLineEdit.setDisabled(True)
+            self.urlLineEdit.setClearButtonEnabled(False)
 
     def setToolTipContentSlot(self, tooltip: qfw.StateToolTip, content: str):
         tooltip.setContent(content)
 
-    def syncSuccessSlot(self, uid: int):
+    def syncSuccessSlot(self, uid: str):
         logger.info('[GUI] Gacha data synchronization success')
 
         self.uid = uid
         account_record.update_timestamp(uid)
 
         self.syncToolTip.setTitle(babelfish.ui_sync_gacha_success())
         self.syncToolTip.setContent('')
         self.syncToolTip.setState(True)
         self.syncToolTip = None
         self.syncThread = None
 
-        self.syncButton.setEnabled(True)
-        self.saveButton.setEnabled(True)
-
+        self.enableButtons()
         self.updateRecordDisplay()
 
-    def syncFailSlot(self, message: str):
+    def syncFailureSlot(self, message: str):
         logger.info(f'[GUI] Gacha data sync fail with message {message}')
 
         if self.syncToolTip is not None:
             self.syncToolTip.setTitle(babelfish.ui_sync_gacha_fail())
             self.syncToolTip.setContent('')
             self.syncToolTip.setState(True)
             self.syncToolTip = None
@@ -547,25 +651,71 @@
             orient=Qt.Orientation.Horizontal,
             isClosable=True,
             duration=-1,
             position=qfw.InfoBarPosition.TOP_RIGHT,
             parent=self,
         )
 
-        self.syncButton.setEnabled(True)
-        self.saveButton.setEnabled(True)
+        self.enableButtons()
 
     def saveSuccessSlot(self, path):
         self.saveThread = None
 
         qfw.InfoBar.success(
             title=babelfish.ui_save_success(),
             content=babelfish.ui_save_success_msg(path),
             orient=Qt.Orientation.Horizontal,
             isClosable=True,
             duration=-1,
             position=qfw.InfoBarPosition.TOP_RIGHT,
             parent=self,
         )
 
-        self.syncButton.setEnabled(True)
-        self.saveButton.setEnabled(True)
+        self.enableButtons()
+
+    def saveFailureSlot(self, msg):
+        self.saveThread = None
+
+        qfw.InfoBar.error(
+            title=babelfish.ui_save_failure(),
+            content=msg,
+            orient=Qt.Orientation.Horizontal,
+            isClosable=True,
+            duration=-1,
+            position=qfw.InfoBarPosition.TOP_RIGHT,
+            parent=self,
+        )
+
+        self.enableButtons()
+
+    def loadSuccessSlot(self, msg):
+        self.loadThread = None
+        msg = json.loads(msg)
+        self.uid = msg['uid']
+
+        qfw.InfoBar.success(
+            title=babelfish.ui_load_success(),
+            content=msg['msg'],
+            orient=Qt.Orientation.Horizontal,
+            isClosable=True,
+            duration=-1,
+            position=qfw.InfoBarPosition.TOP_RIGHT,
+            parent=self,
+        )
+
+        self.enableButtons()
+        self.updateRecordDisplay()
+
+    def loadFailureSlot(self, msg):
+        self.loadThread = None
+
+        qfw.InfoBar.error(
+            title=babelfish.ui_load_failure(),
+            content=msg,
+            orient=Qt.Orientation.Horizontal,
+            isClosable=True,
+            duration=-1,
+            position=qfw.InfoBarPosition.TOP_RIGHT,
+            parent=self,
+        )
+
+        self.enableButtons()
```

### Comparing `starrail-toolkit-0.6.5/starrail/gui/interfaces/home.py` & `starrail-toolkit-0.6.9/starrail/gui/interfaces/home.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/interfaces/setting.py` & `starrail-toolkit-0.6.9/starrail/gui/interfaces/setting.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/interfaces/unlock_fps.py` & `starrail-toolkit-0.6.9/starrail/gui/interfaces/unlock_fps.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/widgets/dialog.py` & `starrail-toolkit-0.6.9/starrail/gui/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/widgets/link_card.py` & `starrail-toolkit-0.6.9/starrail/gui/widgets/link_card.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/widgets/pie_chart.py` & `starrail-toolkit-0.6.9/starrail/gui/widgets/pie_chart.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/gui/widgets/title_bar.py` & `starrail-toolkit-0.6.9/starrail/gui/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/unlock/fps.py` & `starrail-toolkit-0.6.9/starrail/unlock/fps.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/utils/accounts.py` & `starrail-toolkit-0.6.9/starrail/utils/accounts.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 
 def todict(d, keys):
     return {k: d[k] for k in d if k in keys}
 
 
 class AccountRecord:
 
+    latest_uid_changed = None
+    accounts_changed = None
+
     def __init__(self, path):
         self._path = path
         cache = self.safe_load()
         self.meta = cache['meta']
         self.accounts = cache['accounts']
 
     def safe_load(self):
         try:
-            with open(self.path, encoding='utf-8') as f:
+            with open(self._path, encoding='utf-8') as f:
                 cache = json.load(f)
             return cache
         except Exception:
             return dict(
                 meta=dict(latest=''),
                 accounts=dict(),
             )
@@ -34,33 +37,53 @@
         os.makedirs(dirname, exist_ok=True)
         with open(self._path, 'w', encoding='utf-8') as f:
             json.dump(
                 dict(meta=self.meta, accounts=self.accounts), f,
                 ensure_ascii=False, indent=2,
             )
 
-    def update_timestamp(self, uid):
-        timestamp = time.strftime(babelfish.constants.TIME_FMT)
-        if uid in self.accounts:
-            self.accounts[uid]['last_update'] = timestamp
-        else:
-            self.accounts[uid] = dict(last_update=timestamp)
-        self.meta['latest'] = uid
+    def add_account(self, uid: str):
+        uid = str(uid)
+        if uid not in self.accounts:
+            self.accounts[uid] = dict(
+                last_update='',
+                pid='',
+                cookie='',
+            )
+            if self.accounts_changed is not None:
+                self.accounts_changed()
+
+    def update_timestamp(self, uid, timestamp=None):
+        uid = str(uid)
+        self.latest_uid = uid
+        if not timestamp:
+            timestamp = time.strftime(babelfish.constants.TIME_FMT)
+        if uid not in self.accounts:
+            self.add_account(uid)
+        self.accounts[uid]['last_update'] = timestamp
         self.flush()
 
+    @property
     def latest_uid(self):
         return self.meta['latest']
 
+    @latest_uid.setter
+    def latest_uid(self, value):
+        if self.meta['latest'] != value:
+            self.meta['latest'] = value
+            if self.latest_uid_changed is not None:
+                self.latest_uid_changed(value)
+
 
 account_record = AccountRecord(cfg.account_record_path)
 
 
 def get_latest_uid():
-    if account_record.latest_uid():
-        return account_record.latest_uid()
+    if account_record.latest_uid:
+        return account_record.latest_uid
     if os.path.isdir(cfg.db_dir):
         caches = os.listdir(cfg.db_dir)
         caches = [
             cache.split('.')[0]
             for cache in caches if cache.endswith('.sqlite3')
         ]
         if caches:
```

### Comparing `starrail-toolkit-0.6.5/starrail/utils/auto_update.py` & `starrail-toolkit-0.6.9/starrail/utils/auto_update.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/utils/babelfish/__init__.py` & `starrail-toolkit-0.6.9/starrail/utils/babelfish/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 ui_check_update = dictionary.ui_check_update
 ui_check_update_at_start = dictionary.ui_check_update_at_start
 ui_check_update_at_start_desc = dictionary.ui_check_update_at_start_desc
 ui_check_update_fail = dictionary.ui_check_update_fail
 ui_check_update_success = dictionary.ui_check_update_success
 ui_copyright = dictionary.ui_copyright
 ui_curr_fps = dictionary.ui_curr_fps
+ui_current_account = dictionary.ui_current_account
 ui_current_version = dictionary.ui_current_version
+ui_customize_url = dictionary.ui_customize_url
 ui_deduce_uid_fail = dictionary.ui_deduce_uid_fail
 ui_downloading_gacha = dictionary.ui_downloading_gacha
 ui_en = dictionary.ui_en
 ui_extract_api_fail = dictionary.ui_extract_api_fail
 ui_extract_api_fail_with_msg = dictionary.ui_extract_api_fail_with_msg
 ui_extracting_api_url = dictionary.ui_extracting_api_url
 ui_fine = dictionary.ui_fine
@@ -47,41 +49,47 @@
 ui_gacha_true_prob = dictionary.ui_gacha_true_prob
 ui_gacha_type = dictionary.ui_gacha_type
 ui_get_started = dictionary.ui_get_started
 ui_get_started_desc = dictionary.ui_get_started_desc
 ui_github_repo = dictionary.ui_github_repo
 ui_github_repo_desc = dictionary.ui_github_repo_desc
 ui_is_latest_version = dictionary.ui_is_latest_version
+ui_load_failure = dictionary.ui_load_failure
+ui_load_gacha = dictionary.ui_load_gacha
+ui_load_success = dictionary.ui_load_success
+ui_load_success_msg = dictionary.ui_load_success_msg
 ui_locale = dictionary.ui_locale
 ui_locale_setting_desc = dictionary.ui_locale_setting_desc
 ui_no_data = dictionary.ui_no_data
 ui_not_good = dictionary.ui_not_good
 ui_ooops = dictionary.ui_ooops
 ui_open_docs = dictionary.ui_open_docs
 ui_open_issues = dictionary.ui_open_issues
 ui_open_repo = dictionary.ui_open_repo
 ui_open_troubleshooting = dictionary.ui_open_troubleshooting
 ui_operation_zone = dictionary.ui_operation_zone
 ui_personalization = dictionary.ui_personalization
 ui_reset_fps = dictionary.ui_reset_fps
 ui_reset_panel = dictionary.ui_reset_panel
 ui_save_data = dictionary.ui_save_data
+ui_save_failure = dictionary.ui_save_failure
 ui_save_success = dictionary.ui_save_success
 ui_save_success_msg = dictionary.ui_save_success_msg
 ui_send_feedback = dictionary.ui_send_feedback
 ui_send_feedback_desc = dictionary.ui_send_feedback_desc
 ui_set_fps_fail_with_msg = dictionary.ui_set_fps_fail_with_msg
 ui_setting_failure = dictionary.ui_setting_failure
 ui_setting_panel = dictionary.ui_setting_panel
 ui_setting_restart_content = dictionary.ui_setting_restart_content
 ui_setting_restart_title = dictionary.ui_setting_restart_title
 ui_setting_success = dictionary.ui_setting_success
 ui_settings = dictionary.ui_settings
 ui_since_last_guarantee = dictionary.ui_since_last_guarantee
 ui_status_panel = dictionary.ui_status_panel
+ui_switch = dictionary.ui_switch
 ui_sync = dictionary.ui_sync
 ui_sync_gacha_fail = dictionary.ui_sync_gacha_fail
 ui_sync_gacha_initial = dictionary.ui_sync_gacha_initial
 ui_sync_gacha_success = dictionary.ui_sync_gacha_success
 ui_synchronizing_gacha = dictionary.ui_synchronizing_gacha
 ui_theme_mode = dictionary.ui_theme_mode
 ui_theme_mode_dark = dictionary.ui_theme_mode_dark
@@ -92,13 +100,14 @@
 ui_traceback = dictionary.ui_traceback
 ui_troubleshooting = dictionary.ui_troubleshooting
 ui_troubleshooting_desc = dictionary.ui_troubleshooting_desc
 ui_unlock_fps = dictionary.ui_unlock_fps
 ui_unlock_fps_desc = dictionary.ui_unlock_fps_desc
 ui_update_available = dictionary.ui_update_available
 ui_update_desc = dictionary.ui_update_desc
+ui_use_customize_url = dictionary.ui_use_customize_url
 ui_users = dictionary.ui_users
 ui_users_desc = dictionary.ui_users_desc
 ui_welcome = dictionary.ui_welcome
 ui_zhs = dictionary.ui_zhs
 
 __all__ = ['constants', 'translate']
```

### Comparing `starrail-toolkit-0.6.5/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.6.9/starrail/utils/babelfish/dictionary.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,18 +86,23 @@
     en='Copyright © {} LittleNyima.',
     zhs='版权所有 © {} LittleNyima。',
 )
 ui_curr_fps = _MS(
     en='Current FPS in Game Settings: {}.',
     zhs='当前游戏设定帧率：{}。',
 )
+ui_current_account = _MS(en='Current', zhs='当前账号')
 ui_current_version = _MS(
     en='Current version: {}.',
     zhs='当前版本：{}。',
 )
+ui_customize_url = _MS(
+    en='Customize API URL',
+    zhs='自定义 API URL',
+)
 ui_deduce_uid_fail = _MS(
     en='Fail to deduce uid. There may be no record. Please check.',
     zhs='检测 UID 失败，账号可能没有抽卡记录，请重试。',
 )
 ui_downloading_gacha = _MS(
     en='Downloading page {page} of type {name}',
     zhs='正在导出{name}的第{page}页',
@@ -152,14 +157,21 @@
     en='This project is open-resource, licenced under GPLv3. View code here.',
     zhs='本项目代码开源，以 GPLv3 分发。点此查看源代码。',
 )
 ui_is_latest_version = _MS(
     en='Your application is the latest version.',
     zhs='已经是最新版本啦',
 )
+ui_load_failure = _MS(en='Record Load Failed', zhs='加载失败')
+ui_load_gacha = _MS(en='Import from JSON', zhs='导入数据')
+ui_load_success = _MS(en='Record Load Success', zhs='加载成功')
+ui_load_success_msg = _MS(
+    en='Successfully loaded {cnt} items for uid {uid}.',
+    zhs='成功导入了用户{uid}的{cnt}条记录。',
+)
 ui_locale = _MS(en='Display Language', zhs='显示语言')
 ui_locale_setting_desc = _MS(en='Changing the display language', zhs='改变显示语言')
 ui_no_data = _MS(en='No Data', zhs='暂无数据')
 ui_not_good = _MS(en='No', zhs='不好')
 ui_ooops = _MS(en='OOOPS!', zhs='出错了！')
 ui_open_docs = _MS(en='Open Documentations', zhs='打开帮助页面')
 ui_open_issues = _MS(en='Open Issue Page', zhs='打开反馈页面')
@@ -169,14 +181,15 @@
 ui_personalization = _MS(en='Personalization', zhs='个性化')
 ui_reset_fps = _MS(
     en='Reset FPS',
     zhs='重置帧率',
 )
 ui_reset_panel = _MS(en='Reset Panel', zhs='重置面板')
 ui_save_data = _MS(en='Save As', zhs='保存数据')
+ui_save_failure = _MS(en='Data Save Failed', zhs='保存失败')
 ui_save_success = _MS(en='Data Save Success', zhs='保存成功')
 ui_save_success_msg = _MS(en='Data is saved to {}', zhs='数据已保存到{}')
 ui_send_feedback = _MS(en='Send Feedback', zhs='提交反馈')
 ui_send_feedback_desc = _MS(
     en='Feedback is welcome if you encounter problems or have suggestions.',
     zhs='如果你遇到问题，或对本项目有更多建议，欢迎提交反馈。',
 )
@@ -197,14 +210,15 @@
 ui_setting_success = _MS(en='Success', zhs='设置成功')
 ui_settings = _MS(en='Settings', zhs='设置')
 ui_since_last_guarantee = _MS(
     en='Since Last Guarantee',
     zhs='保底已垫',
 )
 ui_status_panel = _MS(en='Status Panel', zhs='状态面板')
+ui_switch = _MS(en='Switch', zhs='切换')
 ui_sync = _MS(en='Sync Data', zhs='同步数据')
 ui_sync_gacha_fail = _MS(
     en='Synchronization Failed',
     zhs='同步失败',
 )
 ui_sync_gacha_initial = _MS(
     en='Initializing...',
@@ -256,14 +270,15 @@
         'it is recommended to download from the network disk distribution.'
     ),
     zhs=(
         '崩坏：星穹铁道工具箱有新的可用版本，更新日志：{}\n 请更新到最新版本以使用全新'
         '功能。如果你对GitHub的连接不稳定，请从网盘下载最新版本。'
     ),
 )
+ui_use_customize_url = _MS(en='Use Customize URL', zhs='使用自定义URL')
 ui_users = _MS(en='Users', zhs='用户管理')
 ui_users_desc = _MS(en='Multi-user management', zhs='如果有多个账号可以用这个切换')
 ui_welcome = _MS(
     en='Welcome to HKSR Toolkit!',
     zhs='欢迎登车！',
 )
 ui_zhs = _MS(
```

### Comparing `starrail-toolkit-0.6.5/starrail/utils/babelfish/locale.py` & `starrail-toolkit-0.6.9/starrail/utils/babelfish/locale.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.6.9/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail/utils/loggings.py` & `starrail-toolkit-0.6.9/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.6.5/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.6.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.6.5
+Version: 0.6.9
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,47 +15,42 @@
 
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/05/06/p9atspD.png" alt="logo" />
 </div>
 
-<b><i>有一说一，现在的界面有点太丑了，在改了在改了</i></b>
-
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 | 发行版版本 |
 | :--------: | :----------: | :-------: | :--------: |
-|   0.6.5    |    0.6.5     |   0.6.5   |   0.6.5    |
+|   0.6.9    |    0.6.9     |   0.6.9   |   0.6.9    |
 
 目前第一阶段开发已完成，历史开发计划见[该页面](docs/history-dev-plan.md)。
 
 - [x] 支持更多的可设置选项
-- [ ] 支持国际服
 - [x] 支持解锁120帧
 - [x] 支持以 SRGF 标准导出
-- [ ] 支持以 SRGF 标准导入
-- [ ] 支持手动设置 API URL
+- [x] 支持以 SRGF 标准导入
+- [x] 支持手动设置 API URL
 - [x] 支持夜间模式
-- [ ] 支持多用户切换
-- [ ] 美化程序界面
+- [x] 支持多用户切换
+- [x] 美化程序界面
 
 ## 常见问题解答
 
 关于程序使用过程中存在的问题，可以参考[本链接](docs/troubleshooting.md)获得解答。若问题无法解决，欢迎[提出反馈](https://github.com/LittleNyima/honkai-starrail-toolkit/issues)。
 
 ## 安装方式
 
 ### 下载可执行程序
 
-目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouk.com/ig3lR0xdvwwh)，两种途径的内容相同，可以自行选择下载方式。
-
-***BREAKING：目前用户界面正在优化中，预览如下图所示。***（注意：该版本尚未发布，所以 release 中仍然是旧版界面，且该界面正在调试过程中，可能会有一些问题，如果出现问题，请先下载旧版 release 使用。）
+目前提供两种分发途径：[GitHub Release](https://github.com/LittleNyima/honkai-starrail-toolkit/releases) 和 [蓝奏云](https://wwmg.lanzouk.com/iN7870y9o7gb)，两种途径的内容相同，可以自行选择下载方式。
 
-![gui preview gacha](https://s1.ax1x.com/2023/05/25/p9HOzLQ.png)
+![gui preview gacha](https://s1.ax1x.com/2023/06/01/p9xxdXj.png)
 
 ![gui preview unlock](https://s1.ax1x.com/2023/05/23/p9o76gA.png)
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
@@ -69,14 +64,20 @@
 
 ```shell
 git clone git@github.com:LittleNyima/honkai-starrail-toolkit.git
 cd honkai-starrail-toolkit
 python3 setup.py install
 ```
 
+注：如果出现关于 `qfluentwidgets` 相关的报错，可能是因为默认 pypi 源的版本较低，可以使用以下命令安装最新版本的依赖：
+
+```
+pip install -U PySide6-Fluent-Widgets -i https://pypi.org/simple/
+```
+
 ##  命令行使用指南
 
 ### 获取抽卡查询 API URL
 
 请参考[这个教程](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
```

### Comparing `starrail-toolkit-0.6.5/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.6.9/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 starrail/gacha/url.py
 starrail/gui/__init__.py
 starrail/gui/application.py
 starrail/gui/common/__init__.py
 starrail/gui/common/config.py
 starrail/gui/common/icon.py
 starrail/gui/common/stylesheet.py
+starrail/gui/common/thread.py
 starrail/gui/common/utils.py
 starrail/gui/interfaces/__init__.py
 starrail/gui/interfaces/base.py
 starrail/gui/interfaces/gacha_sync.py
 starrail/gui/interfaces/home.py
 starrail/gui/interfaces/setting.py
 starrail/gui/interfaces/unlock_fps.py
```

