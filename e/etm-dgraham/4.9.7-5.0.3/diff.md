# Comparing `tmp/etm-dgraham-4.9.7.tar.gz` & `tmp/etm-dgraham-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-4.9.7.tar", last modified: Tue Nov 15 18:42:54 2022, max compression
+gzip compressed data, was "etm-dgraham-5.0.3.tar", last modified: Sun Jun  4 20:49:09 2023, max compression
```

## Comparing `etm-dgraham-4.9.7.tar` & `etm-dgraham-5.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2022-11-15 18:42:54.831356 etm-dgraham-4.9.7/
--rw-r--r--   0 dag        (501) staff       (20)     3417 2022-11-15 18:34:18.000000 etm-dgraham-4.9.7/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-4.9.7/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   117499 2022-11-15 18:42:54.831200 etm-dgraham-4.9.7/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   116587 2022-11-15 01:37:02.000000 etm-dgraham-4.9.7/README.md
--rw-rw-rw-   0 dag        (501) staff       (20)       25 2020-06-03 13:02:08.000000 etm-dgraham-4.9.7/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 18:30:57.000000 etm-dgraham-4.9.7/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2022-11-15 18:42:54.823535 etm-dgraham-4.9.7/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-4.9.7/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-4.9.7/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-4.9.7/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2022-11-15 18:42:54.827174 etm-dgraham-4.9.7/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-4.9.7/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)     9461 2022-11-11 17:43:50.000000 etm-dgraham-4.9.7/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2022-11-15 18:34:18.000000 etm-dgraham-4.9.7/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    10739 2021-12-29 14:26:10.000000 etm-dgraham-4.9.7/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-4.9.7/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)   252804 2022-11-15 18:34:18.000000 etm-dgraham-4.9.7/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    32495 2022-11-13 19:09:25.000000 etm-dgraham-4.9.7/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-11-15 13:40:42.000000 etm-dgraham-4.9.7/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)    86196 2022-11-15 18:34:18.000000 etm-dgraham-4.9.7/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2022-11-15 18:42:54.829309 etm-dgraham-4.9.7/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   117499 2022-11-15 18:42:54.000000 etm-dgraham-4.9.7/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-4.9.7/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-4.9.7/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      886 2022-11-15 18:42:54.000000 etm-dgraham-4.9.7/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2022-11-15 18:42:54.000000 etm-dgraham-4.9.7/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2022-11-15 18:42:54.000000 etm-dgraham-4.9.7/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-4.9.7/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      333 2022-11-15 18:42:54.000000 etm-dgraham-4.9.7/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-4.9.7/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2022-11-15 18:42:54.000000 etm-dgraham-4.9.7/etm_dgraham.egg-info/top_level.txt
--rw-rw-rw-   0 dag        (501) staff       (20)    28934 2020-06-03 13:02:08.000000 etm-dgraham-4.9.7/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-4.9.7/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-4.9.7/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-4.9.7/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-4.9.7/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-4.9.7/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2022-11-15 18:42:54.831391 etm-dgraham-4.9.7/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     5110 2022-10-24 21:26:00.000000 etm-dgraham-4.9.7/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2022-11-15 18:42:54.829431 etm-dgraham-4.9.7/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-4.9.7/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2022-11-15 18:42:54.830787 etm-dgraham-4.9.7/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-4.9.7/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-4.9.7/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-4.9.7/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)     4123 2020-07-29 20:29:15.000000 etm-dgraham-4.9.7/utilities/make_examples.py
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-4.9.7/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.990183 etm-dgraham-5.0.3/
+-rw-r--r--   0 dag        (501) staff       (20)     2383 2023-06-04 20:44:52.000000 etm-dgraham-5.0.3/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.3/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   129426 2023-06-04 20:49:09.990045 etm-dgraham-5.0.3/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   128514 2023-06-04 16:47:17.000000 etm-dgraham-5.0.3/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.3/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.3/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.982389 etm-dgraham-5.0.3/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.3/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.3/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.3/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.986434 etm-dgraham-5.0.3/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.3/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-03 11:21:41.000000 etm-dgraham-5.0.3/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-04 20:44:52.000000 etm-dgraham-5.0.3/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.3/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.3/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.3/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   277773 2023-06-04 20:44:52.000000 etm-dgraham-5.0.3/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37255 2023-05-23 18:01:39.000000 etm-dgraham-5.0.3/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.3/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    97060 2023-06-04 20:44:52.000000 etm-dgraham-5.0.3/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.988593 etm-dgraham-5.0.3/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   129426 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-04 20:49:09.000000 etm-dgraham-5.0.3/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.3/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.3/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.3/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.3/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.3/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.3/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-04 20:49:09.990218 etm-dgraham-5.0.3/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.3/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.988688 etm-dgraham-5.0.3/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.3/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-04 20:49:09.989522 etm-dgraham-5.0.3/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.3/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.3/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.3/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.3/utilities/open_in_mutt
```

### Comparing `etm-dgraham-4.9.7/CHANGES.txt` & `etm-dgraham-5.0.3/CHANGES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,82 @@
-Recent tagged changes as of 2022-11-15T13:34:13.719827-05:00:
-- 0 seconds ago (HEAD -> working, tag: 4.9.7) Daniel Graham
-    b4f22a66 2022-11-15 13:34:13 -0500
-    Tagged version 4.9.7.
-
-- 14 minutes ago (tag: 4.9.8) Daniel Graham
-    3e3e5c77 2022-11-15 13:20:24 -0500
-    Tagged version 4.9.8.
-
-- 5 hours ago (tag: 4.9.6) Daniel Graham
-    6015ec88 2022-11-15 08:40:16 -0500
-    Tagged version 4.9.6.
-
-- 17 hours ago (tag: 4.9.5) Daniel Graham
-    250004cc 2022-11-14 20:36:44 -0500
-    Tagged version 4.9.5. Added support for argument replacements in
-    saved queries.
-
-- 3 days ago (tag: 4.9.4) Daniel Graham
-    c71d75c2 2022-11-12 12:10:39 -0500
-    Tagged version 4.9.4. Restore cursor position after auto refresh
-    and item edit.
-
-- 3 days ago (tag: 4.9.3) Daniel Graham
-    98de70b1 2022-11-12 09:40:52 -0500
-    Tagged version 4.9.3. Avoid scrolling display with auto refresh.
-
-- 4 days ago (tag: 4.9.2) Daniel Graham
-    ee9c2a6a 2022-11-11 12:42:45 -0500
-    Tagged version 4.9.2. Added @w (wrap) as an event option to
-    specify two durations to wrap the event with busy periods before
-    and/or after for, say, travel time to and from the location of the
-    event.
-
-- 6 days ago (tag: 4.9.1) Daniel Graham
-    25f5f057 2022-11-09 15:33:49 -0500
-    Tagged version 4.9.1.
-
-- 7 days ago (tag: 4.9.0) Daniel Graham
-    2c7f3656 2022-11-08 11:07:56 -0500
-    Tagged version 4.9.0. Backwards incompatible changes have been
-    made to cfg.yaml which will automatically be implemented the first
-    time etm is run after this update. The setting for style (dark or
-    light) now sets the background defaults for new  type_colors and
-    window_colors settings. The cfg.yaml settings for these variables
-    are empty by default and are only used to override one or more of
-    the background defaults. The previously used settings for colors
-    and style_modifications have thus been replaced. Additionally,
-    changes that require updating cfg.yaml, e.g., when a setting has
-    been removed and must be replaced with the default value, a new
-    process is used to better preserve the embedded comments.
-
-- 3 weeks ago (tag: 4.8.8) Daniel Graham
-    f26fee1d 2022-10-28 14:40:36 -0400
-    Tagged version 4.8.8.
-
-- 3 weeks ago (tag: 4.8.7) Daniel Graham
-    65af25ae 2022-10-28 14:28:41 -0400
-    Tagged version 4.8.7.
-
-- 3 weeks ago (tag: 4.8.6) Daniel Graham
-    71f82dcd 2022-10-26 15:25:24 -0400
-    Tagged version 4.8.6.
-
-- 3 weeks ago (tag: 4.8.5) Daniel Graham
-    322ebcf6 2022-10-25 13:25:14 -0400
-    Tagged version 4.8.5.
-
-- 3 weeks ago (tag: 4.8.4) Daniel Graham
-    70d0f98e 2022-10-24 17:25:49 -0400
-    Tagged version 4.8.4. Building both sdist and bdist_wheel for
-    upload
-
-- 3 weeks ago (tag: 4.8.3) Daniel Graham
-    7e304d59 2022-10-24 16:52:54 -0400
-    Tagged version 4.8.3.
-
-- 4 weeks ago (tag: 4.8.2) Daniel Graham
-    416bd7cd 2022-10-21 21:54:58 -0400
-    Tagged version 4.8.2.
-
-- 4 weeks ago (tag: 4.8.1) Daniel Graham
-    e3e182ae 2022-10-20 16:53:19 -0400
-    Tagged version 4.8.1.
-
-- 4 weeks ago (tag: 4.8.0) Daniel Graham
-    7420832f 2022-10-19 13:46:52 -0400
-    Tagged version 4.8.0. Added preserve as an overdue option for
-    repeating tasks.
-
-- 4 weeks ago (tag: 4.7.17) Daniel Graham
-    475d89a9 2022-10-17 08:03:21 -0400
-    Tagged version 4.7.17.
-
-- 5 weeks ago (tag: 4.7.16) Daniel Graham
-    90083942 2022-10-14 11:14:51 -0400
-    Tagged version 4.7.16.
+Recent tagged changes as of 2023-06-04T16:44:49.898199-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.0.3) Daniel Graham
+    e0a0d9e 2023-06-04 16:44:49 -0400
+    Tagged version 5.0.3.
+
+- 3 hours ago (tag: 5.0.2) Daniel Graham
+    4c5d4bb 2023-06-04 13:26:17 -0400
+    Tagged version 5.0.2.
+
+- 4 hours ago (tag: 5.0.1) Daniel Graham
+    b30f0ed 2023-06-04 12:47:15 -0400
+    Tagged version 5.0.1.
+
+- 33 hours ago (tag: 5.0.0) Daniel Graham
+    7bc8090 2023-06-03 07:21:38 -0400
+    Tagged version 5.0.0. Use pendulum periods for f and elements of h
+    instead of datetimes.
+
+- 8 days ago (tag: 4.12.9) Daniel Graham
+    b8fbc47 2023-05-27 13:45:19 -0400
+    Tagged version 4.12.9.
+
+- 9 days ago (tag: 4.12.8) Daniel Graham
+    b0316d5 2023-05-26 13:50:15 -0400
+    Tagged version 4.12.8.
+
+- 10 days ago (tag: 4.12.7) Daniel Graham
+    442ff98 2023-05-25 13:53:52 -0400
+    Tagged version 4.12.7.
+
+- 12 days ago (tag: 4.12.6) Daniel Graham
+    3da7332 2023-05-23 14:01:37 -0400
+    Tagged version 4.12.6.
+
+- 2 weeks ago (tag: 4.12.5) Daniel Graham
+    f0c24d8 2023-05-21 15:08:06 -0400
+    Tagged version 4.12.5.
+
+- 2 weeks ago (tag: 4.12.4) Daniel Graham
+    15b3333 2023-05-20 14:33:40 -0400
+    Tagged version 4.12.4.
+
+- 3 weeks ago (tag: 4.12.3) Daniel Graham
+    dd49fda 2023-05-17 12:24:12 -0400
+    Tagged version 4.12.3.
+
+- 3 weeks ago (tag: 4.12.2) Daniel Graham
+    2a304a3 2023-05-17 09:34:05 -0400
+    Tagged version 4.12.2.
+
+- 3 weeks ago (tag: 4.12.1) Daniel Graham
+    68005b7 2023-05-15 14:20:25 -0400
+    Tagged version 4.12.1. Added display for all-day events to busy
+    view
+
+- 3 weeks ago (tag: 4.12.0) Daniel Graham
+    ce2ab09 2023-05-13 12:46:39 -0400
+    Tagged version 4.12.0. Added engaged view
+
+- 3 weeks ago (tag: 4.11.18) Daniel Graham
+    cd5482a 2023-05-11 12:20:48 -0400
+    Tagged version 4.11.18.
+
+- 4 weeks ago (tag: 4.11.17) Daniel Graham
+    8a02515 2023-05-09 10:14:28 -0400
+    Tagged version 4.11.17.
+
+- 5 weeks ago (tag: 4.11.16) Daniel Graham
+    b2310ce 2023-05-01 14:43:18 -0400
+    Tagged version 4.11.16.
+
+- 5 weeks ago (tag: 4.11.15) Daniel Graham
+    96aff42 2023-05-01 14:12:10 -0400
+    Tagged version 4.11.15.
+
+- 5 weeks ago (tag: 4.11.14) Daniel Graham
+    b437f7b 2023-04-28 08:24:55 -0400
+    Tagged version 4.11.14.
+
+- 5 weeks ago (tag: 4.11.13) Daniel Graham
+    4c47483 2023-04-28 08:14:27 -0400
+    Tagged version 4.11.13.
```

### Comparing `etm-dgraham-4.9.7/PKG-INFO` & `etm-dgraham-5.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 4.9.7
+Version: 5.0.3
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -20,15 +20,15 @@
 Classifier: Topic :: Office/Business :: Scheduling
 Requires-Python: >=3.7.3
 Description-Content-Type: text/markdown
 
 
 <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/etmlogo.png" alt="etm" title="event and task manager" width="200px" />
 
-This is the etm user manual. It is best viewed at [GitHub.io](https://dagraham.github.io/etm-dgraham/) where all the internal, contents links work correctly. etm itself is available from [PyPi](https://pypi.org/project/etm-dgraham/) and [GitHub](https://github.com/dagraham/etm-dgraham) and further information from the etm discussion group at [groups.io](https://groups.io/g/etm) - note especially the [files](https://groups.io/g/etm/files/) folder. Brief how-to videos are available at [youtube](https://www.youtube.com/playlist?list=PLN2WQIqrwSxxh2eNY_YczO6YC-icpKWeG).
+This is the etm user manual. It is best viewed at [GitHub.io](https://dagraham.github.io/etm-dgraham/) where all the internal, contents links work correctly. etm itself is available from [PyPi](https://pypi.org/project/etm-dgraham/) and [GitHub](https://github.com/dagraham/etm-dgraham) and further information from the etm discussion group at [groups.io](https://groups.io/g/etm-dgraham). Brief how-to videos are available at [youtube](https://www.youtube.com/@etm-dgraham).
 
 
 # Contents {#contents}
 -   [Overview](#overview)
     -   [Reminders](#reminders)
         -   [examples](#examples)
         -   [text entry versus forms](#text-entry-versus-forms)
@@ -49,26 +49,29 @@
             -   [Simple query examples](#simple-query-examples)
             -   [Archive queries](#archive-queries)
             -   [Update queries](#update-queries)
             -   [Complex queries](#complex-queries)
             -   [Command History](#command-history)
             -   [Saved Queries](#saved-queries)
         -   [Common Features](#common-features)
+    -   [Mobile Access to your reminders](#mobile)
     -   [Menus](#menus)
         -   [etm menu notes](#etm-menu-notes)
         -   [view menu notes](#view-menu-notes)
         -   [editor menu notes](#editor-menu-notes)
         -   [selected menu notes](#selected-menu-notes)
     -   [Installation](#installation)
         -   [For personal use](#for-personal-use)
-        -   [for use in a virtual environment](#for-use-in-a-virtual-environment)
+        -   [for use in an isolated environment](#for-use-in-an-isolated-environment)
         -   [for use system wide](#for-use-system-wide)
     -   [Usage](#usage)
         -   [Terminal size and color](#terminal-size-and-color)
         -   [Home directory](#home-directory)
+        -   [Timers](#timers)
+        -   [lorem examples](#loremexamples)
         -   [Using etm+](#etmplus)
     -   [Deinstallation](#deinstallation)
         -   [From a virtual environment](#from-a-virtual-environment)
         -   [From a system wide installation](#from-a-system-wide-installation)
 -   [Details](#details)
     -   [Item Types](#item-types)
         -   [event](#event)
@@ -90,19 +93,21 @@
 			- [anniversary substitutions](#anniversary-substitutions)
         -   [archived reminders](#archived-reminders)
         -   [configuration](#configuration)
         -   [data storage](#data-storage)
 
 # Overview {#overview}
 
+*etm* began life in 2013 as *etm-qt* sporting a gui based on *Qt*. The intent was to provide an app supporting GTD (David Allen's Getting Things Done) and exploiting the power of python-dateutil. The name changed to *etmtk* in 2014 when *Tk* replaced *Qt*. Development of *etmtk* continued until 2019 when name changed to *etm-dgraham*, to honor the PyPi naming convention, and the interface changed to a terminal based one based on *promt_toolkit*. Features have changed over the years but the text based interface and basic format of the reminders has changed very little. The goal has always been to be the Swiss Army Knife of tools for managing reminders.
+
 ## Reminders {#reminders}
 
 *etm* offers a simple way to manage your events, tasks and other reminders.
 
-Rather than filling out fields in a form to create or edit reminders, a simple text-based format is used. Each reminder in *etm* begins with a *type character* followed by a brief *summary* of the item and then, perhaps, by one or more *@key value* pairs to specify other attributes of the reminder. Mnemonics are used to make the keys easy to remember, e.g, @s for starting datetime, @l for location, @d for description and so forth.
+Rather than filling out fields in a form to create or edit reminders, a simple text-based format is used. Each reminder in *etm* begins with a *type character* followed by a brief *summary* of the item and then, perhaps, by one or more *@key value* pairs to specify other attributes of the reminder. Mnemonics are used to make the keys easy to remember, e.g, @s for scheduled datetime, @l for location, @d for description and so forth.
 
 The 4 types of reminders in etm with their associated type characters:
 
 * task: **-**
 * event: **\***
 * journal: **%**
 * inbox: **!**
@@ -123,38 +128,38 @@
 
 * A journal entry (**%**): a favorite Churchill quotation that you heard at 2pm today with the quote itself as the [d]escription.
 
         % Give me a pig - Churchill @s 2p @d Dogs look up at
           you. Cats look down at you. Give me a pig - they
           look you in the eye and treat you as an equal.
 
+	The *summary*, "Give me a pig - Churchill" in this example, follows the type character and is meant to be brief - analagous to the subject of an email. The optional *description* follows the "@d" and is meant to be more expansive - analagous to the body of an email.
+
 * A task (**-**): build a dog house, with component [j]obs.
 
         - Build dog house @j pick up materials @j cut pieces
           @j assemble @j sand @j paint
 
-* Inbox (**!**): meet Alex for coffee Friday. This can be
-  changed to an event when the time is confirmed by
-  replacing the **!** with an **\*** and adding the time to `@s`.
+* Inbox (**!**): meet Alex for coffee Friday.
 
         ! Coffee with Alex @s fri @e 1h
 
-    This inbox entry will appear on the current day in *agenda view* until you make the changes.
+	This can be changed to an event when the details are confirmed by replacing the **!** with an **\*** and adding the time to `@s`.  This inbox entry will appear on the current day in *agenda view* until you make the changes.
 
 * An appointment (event) for a dental exam and cleaning at 2pm on Feb 5 and then again [@+] at 9am on Sep 3.
 
         * dental exam and cleaning @s 2p feb 5 2019 @e 45m
           @+ 9am Sep 3 2019
 
 [↺ contents](#contents)
 
 ### text entry versus forms {#text-entry-versus-forms}
 
 * Text entry removes the need to hunt for and click in the relevant entry box and allows you to keep your fingers on the keyboard.
-* Text entry supports the full flexibility of the superb Python *dateutil* package. Consider, for example, creating a reminder for Presidential election day which repeats every 4 years on the first Tuesday after a Monday in November (a monthday falling between 2 and 8). In *etm*, this event would be
+* Text entry supports the full flexibility of the superb Python *dateutil* package. Consider, for example, creating a reminder to vote for President election day which repeats every 4 years on the first Tuesday after a Monday in November (a Tuesday whose monthday falls between 2 and 8). In *etm*, this event would be
 
         * Presidential election day @s nov 1 2020 @r y &i 4 &M 11
           &m 2, 3, 4, 5, 6, 7, 8 &w tu
 
     Try this with a form based calendar application.
 
 [↺ contents](#contents)
@@ -162,14 +167,15 @@
 ### unobtrusive and timely entry assistance {#unobtrusive-and-timely-entry-assistance}
 
 When you want to create a new reminder or edit an exiting one, *etm* opens an area at the bottom of the screen that is divided into two parts by a horizontal line. The lower part is the entry area where what you type appears. The upper part is the prompt/feedback area where *etm* responds to your typing. This response might take the form of providing a suggestion about alternatives, information about the type of input required or feedback about how your current entry is being interpreted. It is important to realize that none of this interferes with your typing - you can blaze away as quickly as you like or even paste complete entries and never glance at the prompt if you like. This is the **unobtrusive** part of the prompt/feedback process.
 
 <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/new.png" alt="new" title="new entry" width="600px" hspace="20px"/>
 
 
+
 [↺ contents](#contents)
 
 #### just in time entry prompts and feedback {#just-in-time-entry-prompts-and-feedback}
 
 Let's create the election day reminder to illustrate the **timely** part of the process. Begin by pressing `N` to create a new reminder and notice that *etm* automatically prompts you for the item type character and suggests the alternatives.
 
         item type
@@ -186,35 +192,35 @@
 
         ────────────────────────────────────────────────────────────
         *_
 
 Enter the summary followed by an `@` and *etm* will automatically display the required and available `@-keys`.
 
         @-key
-        required: @s (start)
+        required: @s (scheduled)
         available: @+ (include), @- (exclude), @a (alerts),
         @b (beginby), @c (calendar), @d (description),
         @e (extent), @g (goto), @i (index), @l (location),
         @m (mask), @n (attendee), @o (overdue),
-        @r (repetition frequency), @s (start), @t (tag),
+        @r (repetition frequency), @s (scheduled), @t (tag),
         @u (used time), @x (expansion), @z (timezone)
         ────────────────────────────────────────────────────────────
         * Presidential election day @_
 
-You see that `@s` is required, so add the `s` and *etm* will prompt you for the value for the start option and describe the type of input required.
+You see that `@s` is required, so add the `s` and *etm* will prompt you for the value for the scheduled option and describe the type of input required.
 
-        start
-        starting date or datetime
+        scheduled
+        scheduled date or datetime
 
         ────────────────────────────────────────────────────────────
         * Presidential election day @s_
 
 As you enter the datetime, *etm* will display its interpretation of your entry.
 
-        start
+        scheduled
         Sun Nov 1 2020
 
         ────────────────────────────────────────────────────────────
         * Presidential election day @s nov 1 20_
 
 Now append an `@` to see the prompt for options and notice that `@s`, having been provided, is no longer listed.
 
@@ -303,15 +309,15 @@
             │   Tue Nov 2 2032                 │
             │   Tue Nov 4 2036                 │
             │                                  │
             │           <    OK    >           │
             │                                  │
             └──────────────────────────────────┘
 
-These are the first 5 repetitions on or after Nov 1 2020. Notice that the start value of Nov 1 2020 is not one of the repetitions since it doesn't satisfy the requirements. These appear correct, so press ^S to save the reminder.
+These are the first 5 repetitions on or after Nov 1 2020. Notice that the scheduled value of Nov 1 2020 is not one of the repetitions since it doesn't satisfy the requirements. These appear correct, so press ^S to save the reminder.
 
 
 General observations:
 
 * The general structure of this reminder is
 
 			* Presidential election day
@@ -328,67 +334,67 @@
 * The prompts provide "just in time" information relevant to the entry you are typing and need only be consulted if you are uncertain about your entry. With a little
 	experience, most reminders can be completed without a glance at the prompt.
 
 [↺ contents](#contents)
 
 #### fuzzy parsing of datetimes {#fuzzy-parsing-of-datetimes}
 
-Whenever *etm* expects a datetime entry as, for example, when you are entering an `@s` starting datetime, it applies fuzzy parsing to your entry.  Suppose it is Dec 17 2019, your computer is in the Eastern timezone and you have just entered `@s` for your lunch event
+Whenever *etm* expects a datetime entry as, for example, when you are entering an `@s` scheduled datetime, it applies fuzzy parsing to your entry.  Suppose it is Dec 17 2019, your computer is in the Eastern timezone and you have just entered `@s` for your lunch event
 
-        start
-        starting date or datetime
+        scheduled
+        scheduled date or datetime
 
         ────────────────────────────────────────────────────────────
         * lunch @s_
 
 If you enter `1`, *etm* will interpret it as 1am on the current date in the local timezone.
 
-        start
+        scheduled
         Tue Dec 17 2019 1:00am EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1_
 
 Adding `p` changes the interpretation to 1pm.
 
-        start
+        scheduled
         Tue Dec 17 2019 1:00pm EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p_
 
 Now start adding 'fri' by appending an 'f'.
 
-        start
+        scheduled
         '1p f' is incomplete or invalid
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p f_
 
 and *etm* will complain that the entry is now either incomplete or invalid. Add the remaining 'ri'.
 
-        start
+        scheduled
         Fri Dec 20 2019 1:00pm EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p fri_
 
 and *etm* understands that you want the coming Friday, Dec 20. Now suppose that you will be in California on Friday and you want Pacific, not Eastern time. Then add an entry for `@z`.
 
-        start
+        scheduled
         local datetime: Fri Dec 20 2019 4:00pm EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p fri_ @z US/Pacific
 
 Note that `local datetime` is now prepended to the result which is still displayed in the local timezone, since that is the location of your computer, but the time has changed to `4:00pm EST` which, of course, is the same time as `1:00pm PST`. *etm* **always** displays times in the current local time zone. When you save this item, the time will be converted to universal time and the `@z US/Pacific` will be deleted - once the time has been converted, the original timezone is no longer relevant.
 
 What if you had entered the 'fri' first?
 
-        start
+        scheduled
         Fri Dec 20 2019
 
         ────────────────────────────────────────────────────────────
         * lunch @s fri
 
 Here *etm* supposes again that you want the coming Friday, Dec 20 but without a time being specified, it is interpreted as a date rather than a datetime and thus without a timezone. Add the `1p` and timezone the result will be the same as before.
 
@@ -399,15 +405,15 @@
         or 'float' to specify a naive/floating datetime
 
         ────────────────────────────────────────────────────────────
         * lunch @s fri 1p @z
 
 and note that supplying 'float' as the timezone does the trick.
 
-        start
+        scheduled
         Fri Dec 20 2019 1:00pm
 
         ────────────────────────────────────────────────────────────
         * lunch @s fri 1p_ @z float
 
 The datetime now appears without either the 'local datetime' prefix or the 'EST' suffix which reveals that it is a naive/floating datetime.
 
@@ -490,54 +496,74 @@
 
 The display for each reminder shows the itemtype and summary column on the left followed by a *flags* column which displays a combination of letters from 'g' (goto), 'k' (connection), 'p' (pinned) and 't' (timer) reflecting the presence of these attributes in the reminder. This column is sometimes followed on the extreme right by another column whose contents depends on the view. E.g. in index and journal views the 'id' of the reminder is displayed while in history view, the last modification timestamp of the reminder is displayed.
 
   * a: Agenda: dated unfinished tasks and other reminders by year-week and week day
   * b: Busy: a graphical illustration of busy and conflicted times by year-week
   * c: Completed: finished tasks and jobs and used time entries by year-week and week day
   * d: Do Next: undated tasks grouped by location/context and ordered by priority (highest first) and extent (least first)
+  * e: Engaged: instances of reminders with used time entries with daily totals displayed graphically
   * f: Forthcoming: unfinished dated tasks and other dated reminders by next occurrence
   * h: History: all items by the latter of the modified or created datetimes in descending order, i.e., most recent first. Datetimes are displayed using a 5 character format where, e.g., 1:15pm today would be displayed as 13:15, November 7 of the current year as 11/17 and January 15 of 2012 as 12.01.
   * i: Index: all items grouped hierarchically by index entry
   * j: Journal: journal entries grouped hierarchically by index entry
   * k: Konnection: items with @k konnection links either to or from the selected item.
   * l: Location: items grouped hierarchically by location entry
   * m: Timers: items with timers.
   * p: Pinned: items whose pin status is on.
   * q: Query: items matching a user specified query. Enter ? for query usage.
   * r: Review: undated tasks sorted by the time since the task was last modified with the most recently modified last.
   * t: Tags: all items with @t tag entries grouped by tag
   * u: Used Time: all items with @u used time entries grouped by month and hierarchically by index
   * U: Used Summary: used time aggregates grouped by month and hierarchically by index
-  * y: Yearly Planning Calendar: compact monthly calendar by half year.
+  * y: Yearly Planning Calendar: compact monthly calendar.
 
 
 [↺ contents](#contents)
 
 ### Weekly Views {#weekly-views}
 
-The _weekly_ agenda, busy and completed views display one week at a time and are *synchronized* so that all three views always display the same week. Left or right cursor keys go backward or forward a week at a time and the pressing the space bar jumps to the week containing the current day. You can also press "J" and enter a date to jump to the week containing the date.
+The _agenda_, _busy_, _completed_ and _engaged_ views display one week at a time and are *synchronized* so that all four views always display the same week. Press the ▶ (right) or ◀ (left) cursor keys go forward or backward a week at a time or press the space bar to jump to the week containing the current day. You can also press "J" and enter a date to jump to the week containing the date.
+
+In _agenda_ view, only days with scheduled reminders are listed. If nothing is scheduled for the entire week, then "Nothing scheduled" is displayed.
+
 
-In both agenda and completed views, only days with scheduled reminders are listed. If nothing is scheduled for the entire week, then "Nothing scheduled" is displayed.
+In _busy_ view, only days that have events with busy times (@e and/or @w entries) are displayed. Press the number of the weekday, [1→Mon, ..., 7→Sun], to show the details of the busy periods from that day or press the ▼ (down) or ▲ (up) cursor keys to show the details of the next or previous day with busy periods.
+
+_Completed_ view shows instances of completed tasks.
+
+_Engaged_ view shows instances of reminders with used time entries with daily totals displayed graphically.
 
 The normal agenda listing for a week day:
 
 * all day events (events with dates as `@s` entries)
 * datetime items (reminders with datetimes as `@s` entries) by time
 * all day tasks (tasks with dates as `@s` entries)
 * all day journal enties (journal entries with dates as `@s` entries)
 
 And, on the current day only:
 
 * inbox items
 * *<* past due warnings in descending order of the number of days past due
 * *>* beginby warnings in ascending order of the number of days remaining
 
+Busy view requires a little explanation. Here is screen shot of agenda view for an illustrative week
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/agenda.png" alt="new" title="agenda view" width="600px" hspace="20px"/>
+
+along with one of busy view for the same week
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/busy.png" alt="new" title="busy view" width="600px" hspace="20px"/>
+
+The first thing to notice in busy view is that busy times are displayed each week day for the period between 7am and 9pm. This period is determined by the *beginbusy* setting in `cfg.yaml` which sets the number of hours after midnight that the display is to begin each day. The period ends 14 hours after *beginbusy*. In this case, it runs from 7 hours after midnight (*beginbusy*) to 7+14=21 hours after midnight or from 7am until 9pm. The resolution is 15 minute periods for each character *slot* so that, for example, the row for *Fr 2* shows a busy period with using 4 green (busy) characters for 10-10:15am, 10:15-10:30am, 10:30-10:45am and 10:45-11am. Now you might notice that this implies that the 4 character slots that begin at 8pm end just before the 9pm slot and that the 9pm slot actually corresponds to the interval 9-9:15pm. Since the actual display includes this last slot, it actually extends for 14 hours plus 15 minutes and thus actually ends at 9:15pm.
+
+The second thing to notice is the red, conflict bar in the display for *Mo 28*. Since the details for this day are displayed in the "busy times" panel at the bottom as well as in the agenda view, you will notice that the conflict corresponds to the overlap between the 6-8am event and the 7-9:30am event. This conflict from 7-8am is illustrated by the 4 red (conflict) characters. Notice also that the period for the first event extends from 6-7am before the period displayed begins at 7am. The single green character to the left of 7am indicates that there were busy times before the displayed period begins. Similarly, the green character to the right of 9-9:15pm on *We 30* indicates that there were busy times after 9:15pm on that day. This corresponds to the 8-10:30pm event shown in agenda view for Wednesday that extends from 9:15-10:30pm after the displayed period.
+
+As you might expect, if a conflict occurred either before or after the displayed period then the corresponding *before* or *after* character would be red instead of green.
+
 [↺ contents](#contents)
 
-### Timer view {#timer-view}
+### Timer View {#timer-view}
 
 This view lists all reminders with associated timers sorted by the elapsed time since the timer's *state* was last changed. The display for each reminder shows the itemtype and summary, any applicable *flags* and, in the right hand column, the elapsed time and *state* of the associated timer.
 
 The sort order assures that the reminder with the active timer will always be at the top of the list and followed by the reminders with the most recently modified timers. This makes it easy to switch back and forth between recent timers.
 
 [↺ contents](#contents)
 
@@ -574,26 +600,28 @@
 reminders with links from the selection
 : the list of items whose ids are included in the @k entries of the selected item
 
 [↺ contents](#contents)
 
 ### Used Time Views {#used-time-views}
 
-The *used time* and *used time summary* views are bound to `u` and `U` respectively. They report `@u` (used time) entries in your reminders grouped by year-month and then heirarchially by `@i` entries. I have a file of reminders with `@i` and `@u` entries such as
+The *used time* and *used time summary* views are bound to `u` and `U` respectively. They report `@u` (used time) entries in your reminders, rounded up according to the `usedtime_minutes` setting in your `cfg.yaml` file and grouped by year-month and then heirarchially by `@i` entries.
+
+I have a file of reminders with `@i` and `@u` entries such as
 
 		* Modi ut sit sed amet sit @s 2019-11-11 10:00am @e
 		   1h30m
 		@u 58m: 2019-11-11 10:58am @u 34m: 2019-11-11 10:34am
 		@i client A/project a1/correspondence
 		@d Aliquam non sed aliquam eius tempora quisquam dolorem.
 		Neque quiquia labore tempora magnam. Quiquia tempora
 		porro est ut. Ut tempora sed non ut eius neque porro.
 		Sed quaerat consectetur dolor sit.
 
-and the *used time view* for November begins with
+With `usedtime_minutes: 6`, the *used time view* for November begins with
 
 		November 2019
 		  client A
 			project a1
 			  correspondence
 				* Modi ut sit sed amet sit: 1.6h Nov 11
 				% Amet modi neque eius adipisci: 2.7h Nov 27
@@ -995,14 +1023,15 @@
 * monthend: 12am on the 1st of the following month
 
 and can be combined with period strings using M (month),
 w (week), d (day), h (hour) and m (minute). E.g.:
 * `weekbeg - 1w`  (the beginning of the previous week)
 * `monthend + 1M` (the end of the following month)
 
+
 [↺ contents](#contents)
 
 #### Command History {#command-history}
 
 Any query entered at the 'query:' prompt and submitted by pressing 'Enter' is added to the command history. These queries are kept as long as 'etm' is running and can be accessed using the up and down cursor keys in the query field. This means you can enter a query, check the result, press 'q' to reopen the query prompt, press the up cursor and you will have your previous query ready to modify and submit again. It is also possible to keep a permanent list of queries accessible by shortcuts. See 'Saved Queries' below.
 
 [↺ contents](#contents)
@@ -1106,14 +1135,31 @@
 	* While entering the search expression, push the `up` or `down` cursor keys to change the direction of search.
     * After entering the search expression, press “n” to search (cyclically) for other matches in the direction specified.
 	* Once a search is initiated, it remains active in all views with matches highlighted. To remove the highlighting, search for something unlikely to be matched, e.g., 3 consecutive commas.
 
 
 [↺ contents](#contents)
 
+## Mobile access to your reminders {#mobile}
+
+The files `current.txt` and `next.txt` in your etm home directory are created by *etm* but not displayed within *etm* itself. Whether or not these files are created depends on two settings in your `cfg.yaml`:
+
+* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary.
+
+* `keep_next`: true or false. If `true`, the contents of *do next* view will be written to `next.txt` in your etm home directory and updated whenever necessary.
+
+By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule and tasks on your mobile device.
+
+Here is a screen shot from an iPhone of an illustrative `current.txt`:
+
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/current_on_iphone.png" alt="new" title="current view" width="300px" hspace="20px"/>
+
+
+[↺ contents](#contents)
+
 ## Menus {#menus}
 
 Pressing F1 toggles the *etm* menu display - opening it if it is closed and closing it if it is open. There are four menu tabs labeled *etm*, *view*, *editor* and *selected* with the options listed below:
 
     etm
 		F1) activate/close menu
         F2) about etm
@@ -1126,35 +1172,38 @@
         ---
         ^q) quit
     view
         a) agenda
         b) busy
         c) completed
         d) do next
+        e) engaged
         f) forthcoming
         h) history
         i) index
         j) journal
         l) location
         p) pinned
         q) query
 		r) review
         t) tags
         u) used time
         U) used time summary
+        v) refresh views to fit resized terminal
         ---
         s) scheduled alerts for today
-        y) half yearly calendar
+        y) yearly calendar
         ---
         /) search forward
         ?) search backward
         n) next incrementally in search
         ^l) prompt for and jump to line number
         ^p) jump to next pinned item
-        ^c) copy active view to clipboars
+        ^c) copy active view to clipboard
+        ^t) start quick timer
         ---
         J) jump to date in a), b) and c)
         right) next in a), b), c), u), U) and y)
         left) previous in a), b), c), u), U) and y)
         space) current in a), b), c), u), U) and y)
     editor
         N) create new item
@@ -1175,16 +1224,17 @@
         g) open goto link
         k) show konnections
         ^r) show repetitions
 		^u) update last modified
         ^x) toggle archived status
         ---
         T) change timer to next state
-        TR) record usedtime and delete timer
+        TR) record usedtime and end timer or add usedtime
         TD) delete timer
+        ---
         TT) toggle paused/running for active timer
 
 
 [↺ contents](#contents)
 
 ### etm menu notes {#etm-menu-notes}
 
@@ -1210,14 +1260,15 @@
 
 [↺ contents](#contents)
 
 ### view menu notes {#view-menu-notes}
 
 The *view* menu provides access to all the *etm* views with the shortcut keys for these views. E.g., press `a` to open *agenda view*.
 
+The *start quick timer* option creates a new, inbox reminder with the current datetime as the subject, associates a timer with reminder and starts the timer. If another timer is active, it will be paused if necessary and made inactive. Subsequent invocations repeat this process.
 
 The entries here are pretty obvious and the views themselves are descibed elsewhere.
 
 [↺ contents](#contents)
 
 ### editor menu notes {#editor-menu-notes}
 
@@ -1238,102 +1289,86 @@
 * *reschedule* will prompt for a datetime. If the reminder is repeating, the provided datetime will replace the datetime of the selected instance. Otherwise it will be used either to replace the current value of `@s` or, if there is no `@s` entry, to create one.
 * *schedule new* will prompt for a datetime and add that instance to any other instances of the reminder.
 * *open goto* will use the system default application to open the file path or url specified in the selected reminders `@g` entry. Items with goto links are displayed with a 'g' in the *flags* column of normal views.
 * *toggle pin* toggles the pin status of an item between off and on. Items for which the pin status are displayed with a 'p', in the *flags* column of normal views and are also displayed in *pinned view*.
 * *show repetitions* pops up a display showing illustrative repetitions if the item is repeating.
 * *toggle archived status* moves the selected reminder from the items table if it is active to the archive table and vice versa if the archive table is active.
 * *change timer to next state*.
-    * these are the states for the timer associated with a reminder and the relevant status of any other timers:
+    * These are the states for the timer associated with a reminder and the relevant status of any other timers:
         * *n* (no timer is associated with this reminder)
             * *n-*: no other timer is active
             * *n+*: another timer is active
         * *i* (a timer is associated with this reminder and it is inactive)
             * *i-*: no other timer is active
             * *i+*: another timer is active
         * *r-*: running (a timer is associated with this reminder and it is running - there cannot be another active timer)
         * *p-*: paused (a timer is associated with this reminder and it is paused - there cannot be another active timer)
 
-       These are the "next" state transitions associated with this action:
+    * These are the "next" state transitions associated with this action:
         * *n+* ⇒ *i+*
-        * *n-* ⇒ *r-*
+        * *n-* ⇒ *p-*
         * *i-* ⇒ *r-*
         * *i+* ⇒ *r-*
         * *r-* ⇒ *p-*
         * *p-* ⇒ *r-*
 
     * Here are the details:
-        * If no timer is currently associated with the reminder, one will be created. If another timer is *active*, the new timer will be *inactive*, otherwise it will be *running*.
+        * If no timer is currently associated with the reminder, one will be created. If another timer is *active*, the new timer will be *inactive*, otherwise it will be *active* and *paused*.
         * If an *inactive* timer is already associated with the reminder. Its state will be changed to *running*. If another timer is *active*, that timer will be changed to *inactive* and, if *running*, its elapsed time will be incremented by the period it has been *running*.
         * If an *active* timer is already associated with the reminder, its state will be toggled between *paused* and *running*. With a transition from *running* to *paused*, the elapsed time for the timer in increased by the period since the timer's state changed to *running*.
 
       Additionally, if there is an *active* timer, its state, either *r* (running) or *p* (paused), is displayed in the *etm* status bar together with the relevant time period, either the total elapsed time or how long the timer has been paused. If there are *inactive* timers with non-zero elapsed times, the total of such elapsed times will also be reported in the status bar. E.g., this display in the status bar
 
             r:4m + i:13m
 
       would mean that the *active* timer is *running* with 4 minutes of unrecorded elapsed time and that there is an additional 13 minutes of unrecorded elapsed time in *inactive* timers.
+
 * *record used time* with a reminder selected, will:
     * If a timer is not currently associated with the reminder, prompt for a timeperiod and ending time to use in adding a usedtime entry to the reminder.
     * If a timer is currently associated with the reminder, use its elapsed time and the last moment it was running as the defaults in the prompt for a usedtime timeperiod and ending time. If the entry is saved, the elapsed time for the timer will be reset to zero and, additionally, if the timer is currently *running*, its status will be changed to *paused*.
 
-    **Important**: timer data is stored in memory and will be lost if *etm* is stopped. Be sure to record usedtime entries for timers with elapsed times before quitting etm. The status bar will always indicate if there is unrecorded elapsed time.
-
 
 [↺ contents](#contents)
 
 ## Installation {#installation}
 
 
 ### For personal use {#for-personal-use}
 
 The easiest way to install *etm* for personal use is to use *pip*:
 
 	$ python3 -m pip install -U etm-dgraham
 
-This will install *etm* with all the needed python supporting modules. You can then start *etm* with
+(This same command can be used to update *etm* when a new version is released.) This will install *etm* with all the needed python supporting modules. You can then start *etm* with
 
 	$ etm <path to home>
 
+
 See [Home directory](#home-directory) for details about `<path to home>`.
 
-<!--  [![etm: installing etm in a virtual environment](http://img.youtube.com/vi/fEPPG82AH7M/0.jpg)](http://www.youtube.com/watch?v=fEPPG82AH7M "installing etm in a virtual environment") -->
 
 [↺ contents](#contents)
 
-### For use in a virtual environment {#For-use-in-a-virtual-environment}
-
-Setting up a virtual environment for etm is only slightly more complicated. The steps for OS/X or linux are illustrated below. For details see [python-virtual-environments-a-primer](https://www.google.com/url?q=https%3A%2F%2Frealpython.com%2Fpython-virtual-environments-a-primer%2F&sa=D&sntz=1&usg=AFQjCNFh7QpJQ4rPCDjZ1eLrV1BRCCpSmw).
-
-Open a terminal and begin by creating a new directory/folder for the virtual environment, say `etm-pypi`, in your home directory:
-
-        $ mkdir ~/etm-pypi
-        $ cd ~/etm-pypi
-
-Now continue by creating the virtual environment (python >= 3.7.4 is required for etm):
-
-        $ python3 -m venv env
+### For use in an isolated environment {#For-use-in-an-isolated-environment}
 
-After a few seconds you will have an `./env` directory. Now activate the virtual environment:
+Installing etm in an isolated or virtual environment (sandbox) is only slightly more complicated. Begin by using *pip* to install *pipx*:
 
-        $ source env/bin/activate
+    $ python3 -m pip install -U pipx
 
-The prompt will now change to something containing `(env)` to indicate that the virtual environment is active. Updating pip is now recommended:
+Now run:
 
-        (env) $ pip install -U pip
+    $ pipx ensurepath
 
-Note that this invokes `./env/bin/pip`. Once this is finished, use pip to install etm:
+to ensure that directories necessary for *pipx* operation are in your PATH environment variable and finally to install *etm* itself:
 
-        (env) $ pip install -U etm-dgraham
+    $ pipx install etm-dgraham
 
-This will install etm and all its requirements in
+(To upgrade *etm* when a new version becomes available, simply replace "install" in this command with "upgrade".) You can then start *etm* as before with
 
-		./env/lib/python3.x/sitepackages
-
-and will also install an executable called `etm` in `./env/bin`.You can then start etm using
-
-        (env) $ etm <path to home>
+    $ etm <path to home>
 
 Details about `<path to home>` are in [Home directory](#home-directory).
 
 [↺ contents](#contents)
 
 ### For use system wide {#for-use-system-wide}
 
@@ -1365,28 +1400,30 @@
 
 [↺ contents](#contents)
 
 ## Usage {#usage}
 
 ### Terminal size and color scheme {#terminal-size-and-color-scheme}
 
-The suggested terminal size for etm is 60 (columns) by 32 or more (rows). The default color scheme is best with a dark terminal background. A scheme better suited to light backgrounds can be set using `style: light` in `cfg.yaml` in your home directory. Some of the *etm* display may not be visible unless `style` is set correctly for your display.
+The suggested terminal size for etm is 70 (columns) by 32 or more (rows). The default color scheme is best with a dark terminal background. A scheme better suited to light backgrounds can be set using `style: light` in `cfg.yaml` in your home directory. Some of the *etm* display may not be visible unless `style` is set correctly for your display.
 
 The size of the terminal is used when *etm* starts to set various display options so changing the terminal size, especially reducing the width, is best avoided once *etm* is running.
 
 [↺ contents](#contents)
 
 ### Home directory {#home-directory}
 
 Before you start etm, think about where you would like to keep your personal data and configuration files. This will be your etm *home* directory. The default is to use whatever directory you're in when you start _etm_ as your _etm_ home directory. If you start _etm_ in your virtual environment directory then the default will be to use that as your home directory as well. If this is not what you want, you can just give the path for whatever directory you would like to use when you start _etm_.
 
 	$ etm <path to home>
+
 Finally, if there is an environmental variable, `ETMHOME`, set to this path then you can just enter
 
 	$ etm
+
 and etm will use `ETMHOME` as its home directory.
 
 Home directory considerations:
 
 * If more than one person will be using etm on the same computer, you might want to have different *home* directories for each user.
 * If you want to use etm on more than one computer and use Dropbox, you might want to use `~/Dropbox/etm` to have access on each of your computers.
 * If you want to separate personal and professional reminders, you could use different _home_ directories for each. You can run two instances of _etm_ simultaneously, one for each directory, and have access to both at the same time.
@@ -1403,24 +1440,80 @@
 Here `cfg.yaml` is your user configuration file and `db.json` contains all your etm reminders. The folders `backups/` contains the 7 most recent daily backups of your `db.json` and `cfg.yaml` files. The folder `logs` contains the current `etm.log` file and the 7 most recent daily backups. Note that backup files are only created when the relevant file has been modified since the last backup.
 
 The file `cfg.yaml` can be edited and the options are documented in the file.
 See [configuration](#configuration) for details.
 
 [↺ contents](#contents)
 
+### Timers {#timers}
+
+For tracking time spent, *etm* supports the use of one or more timers. Each timer is associated with a particular reminder and, if a timer is recorded, a used time entry will be added to the associated reminder using this format:
+
+        @u <time spent>: <datetime recorded>
+
+The timer itself records seconds, but the used time entry for `<time spent>` depends upon the `usedtime_minutes` setting in `cfg.yaml` as follows:
+
+- 0: time is recorded in seconds after rounding to the nearest second
+- 1: time is recorded in minutes after rounding off to the nearest minute, e.g., 1m29s => 1m; 1m30s => 2m
+- 6: time is rounded up to the next one-tenth of an hour for reporting but recorded in minutes
+- 12: time is rounded up to the next two-tenths of an hour for reporting but recorded in minutes
+- 30: time is rounded up to the next half hour for reporting but recorded in minutes
+- 60: time is rounded up to the next hour for reporting but recorded in minutes
+
+The [Used Time Views](#used-time-views) show aggregations of these reported times by month and index entry. Any rounding up is done before aggregating.
+
+Used time entries can be recorded directly by editing the relevant reminder and adding one or more `@u` entries. It is also possible to use *etm* to create timers *attached* to particular reminders and control them with hotkeys.
+
+- T: with a reminder selected
+    - If a timer is not already associated with this reminder, then create a new timer and associate it with this reminder
+        - if another timer is active, make this timer inactive
+        - otherwise make this timer active and paused
+    - If a timer is already associated with this reminder
+        - if the timer is inactive, make it active and running
+        - otherwise toggle the state of the timer between paused and running
+- TR: if a reminder is selected with an associated timer
+    - open a dialog to record a used time entry with the current value of the timer and the current datetime
+    - if, after possible editing, recording is confirmed then add the used time entry and delete the timer
+- TD: if a reminder is selected with an associated timer
+    - open a dialog to confirm deleting the timer without recording the used time
+    - if deletion is confirmed then delete the timer
+- TT: if there is an active timer
+    - toggle the paused/running state for the active timer. Note that the reminder associated with the active timer *need not be selected*.
+    - Note that if there are one or more timers, *exactly one of them will be the active timer*, i.e., either running or paused. The others, if any, will be inactive.
+
+[Timer View](#timer-view), bound to `m`, provides a convenient way of manipulating multiple timers. It lists each existing timer with the active timer first and followed by the other timers in the order of most recently active. Pausing/running the active timer can be done from any view by pressing `TT`. To switch to another timer, change to timer view, press `TT` if necessary to pause the active timer, select the timer you want to start and press 'T' to change its state from 'inactive' to 'running'. It will move to the top of the list and the other timers will move down by one row.
+
+When there are one or more timers, their status is always displayed in the status bar. E.g., `r:6.3m + i:1h3.2` would mean that the active timer is running with 6.3m of elapsed time and there are other, inactive timers with a total of 1h3.2m of elapsed time.
+
+[↺ contents](#contents)
+
+### *lorem* examples {#loremexamples}
+
+If you are new to *etm*, you might find it very useful to install the *lorem* examples. If you press `F5`, enter 'lorem' at the prompt and press `return`, *etm* will generate a series of reminders all of which are tagged 'lorem'. These fall within a three month period including the month in which they were created as well as the previous and subsequent months. The examples are designed to illustrate nearly all of the etm views and features. You can play around with the examples as long as you wish and then remove them all at once by pressing `q` to open query view, entering the query 'any t lorem \| remove' and pressing `return`.
+
+These examples are named for and depend upon the python package *lorem* that can generate random words, phrases, sentences and paragraphs in 'lorem ipsum' text. E.g., "Lorem ipsum dolor sit amet, consectetur adipiscing elit ...". This is "a placeholder text commonly used to demonstrate the visual form of a document or a typeface without relying on meaningful content."
+
+[↺ contents](#contents)
+
 ### Using etm+ {#etmplus}
 
 An added bonus of setting `ETMHOME` to the path of your *home* directory is the possibility of using the `etm+` shortcut for creating reminders. E.g., entering
 
 	$ etm+ '* lunch with Peter @s fri 12p'
 would append the line `* lunch with Peter @s fri 12p` to the file `inbasket.text`in `ETMHOME`, creating the file if necessary. `etm+` also accepts input piped to it so that
 
 	$ echo '* lunch with Peter @s fri 12p' | etm+
 would produce exactly the same result.
 
+Finally, if `{T}` is included, it will be replaced with a time stamp corresponding to the moment the script was invoked. E.g.,
+
+	$ echo '% got the test result at {T}' | etm+
+
+would append something like `% got the test result at 2022-12-07 9:13:55 EST`.
+
 Important
 : The single quotes are necessary to keep the shell from expanding the "*" into the names of all the files in the current working directory and other such mischief.
 
 *etm* checks once every minute for the presence of a file named `inbasket.text`in `ETMHOME` and, if found, will display an inbasket character, ⓘ , at the right end of its status bar reminding you that inbasket items are available for importing. Just press F5 in etm to import the reminders from this file and, on successful completion, automatically remove the file.
 
 Note finally that `etm+` will accept quick notes which are not themselves valid etm reminders such as
 
@@ -1471,49 +1564,48 @@
 
 ### event {#event}
 
 Type character: **\***
 
 An event is something that happens at a particular date or datetime without any action from the user. Christmas, for example, is an event that happens whether or not the user does anything about it.
 
-- The `@s` entry is required and can be specified either as a date or as a datetime. It is interpreted as the starting date or datetime of the event.
+- The `@s` entry is required and can be specified either as a date or as a datetime. It is interpreted as the scheduled date or datetime at which the event begins.
 - If `@s` is a date, the event is regarded as an *occasion* or *all-day* event. Such occasions are displayed first on the relevant date.
 - If `@s` is a datetime, an `@e` entry is allowed and is interpreted as the extent or duration of the event - the end of the event is then given implicitly by starting datetime plus the extent and this period is treated as busy time.
 
 Corresponds to VEVENT in the vcalendar specification.
 
 [↺ contents](#contents)
 
 ### task {#task}
 
 Type character: **-**
 
 A task is something that requires action from the user and lasts, so to speak, until the task is completed and marked finished. Filing a tax return, for example, is a task.
 
-- The `@s` entry is optional and, if given, is interpreted as the date or datetime at which the task is due.
-    - Tasks with an `@s` datetime entry are regarded as past due after the datetime and are displayed in *Agenda View* on the relevant date according to the starting time.
+- The `@s` entry is optional and, if given, is interpreted as the date or datetime at which the task is scheduled to be completed.
+    - Tasks with an `@s` datetime entry are regarded as past due after the datetime and are displayed in *Agenda View* on the relevant date according to the scheduled time.
     - Tasks with `@s` date entry are regarded as past due after the due date and are displayed in *Agenda View* on the due date after all items with datetimes.
     - Tasks that are past due are also displayed in *Agenda View* on the current date using the type character `<` with an indication of the number of days that the task is past due.
 - Tasks without an `@s` entry are to be completed when possible and are sometimes called *todos*. They are regarded as *next* items in the *Getting Things Done* terminology and are displayed in *Do Next* view grouped by @l (location/context).
-- Tasks with an `@r` (repeat) entry can have an `@o` (overdue) setting.
-	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. mortage payments to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. Whenever a payment is sent, it applies to the oldest, past due one. This is the default when no `@o` entry is given.
-    - `@o p`: preserve. When an instance becomes past due, a new, non-repeating copy is created with the past due datetime as the `@s` entry and with an `@k` containing the document_id of the original item. Suppose, for example, that minutes are kept for a weekly meeting to be sent to the attendees after each meeting. Creating a task that repeats weekly with `@o p` recognizes the distinction between sending the minutes for `22/10/8` and `22/10/15` and, should both become past due, permits finishing the tasks in any convenient order.
-	- `@o r`: reset. Whenever completed, the next instance is due at the first datetime from the recurrance rule that falls after the current datetime. E.g., getting a haircut every 14 days is due 14 days after the last haircut. With this option, at most one instance can be past due.
-	- `@o s`: skip. Like 'keep' and 'reset' combined with the addition that past due instances are ignored. E.g., taking out the trash every Monday morning for pickup is due every Monday morning but, if a Monday passes without taking out the trash, the instance is better regarded as irrelevant than past due. With this option, an instance can never be past due.
+- Tasks with an `@r` (repeat) or an `@+` entry can have an `@o` (overdue) setting.
+	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. minutes from a monthly meeting to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. By default, a completion applies to the oldest, past due one, though other instances can be selected. This is the default when no `@o` entry is given.
+	- `@o r`: reset. Whenever completed, the next instance is due at the first datetime that falls after the current datetime. E.g., getting a haircut every 14 days is due 14 days after the last haircut. With this option, at most one instance can be past due.
+	- `@o s`: skip. Like 'keep' with the addition that past due instances are ignored. E.g., taking out the trash every Monday morning for pickup is due every Monday morning but, if a Monday passes without taking out the trash, the instance is better regarded as irrelevant than past due. With this option, an instance can never be past due.
 
 	    Furthermore, if the options setting `limit_skip_display` were true, then only the first instance of such a task would be displayed in agenda view. E.g., with the `limit_skip_display` setting true, then for the task
 
 			- meds @s +0d @r d &h 8,14,20 @o s
 
 		agenda view at 10am today would only display the first, 2pm (14h) instance of this task. If, on the other hand, this setting were false, then agenda view would display not only the 2pm instance but also the 8pm (20h) instances and all three instances on every future date.
 
 - Jobs
     - Tasks, both with and without @s entries can have component jobs using @j entries.
-    - For tasks with an @s entry, jobs can have an &s entry to set the due date/datetime for the job. It is entered as a timeperiod relative to  the starting datetime (+ before or - after) for the task. Zero minutes is the default when &s is not entered.
-    - For tasks with an @s entry, jobs can also have &a, alert, and &b, beginning soon, notices. The entry for &a is given as a time period relative to &s (+ before or - after) and the entry for &b is a positive integer number of days before the starting date/time to begin displaying "beginning soon" notices. The entry for @s in the task becomes the default for &s in each job.  E.g., with
+    - For tasks with an @s entry, jobs can have an &s entry to set the due date/datetime for the job. It is entered as a timeperiod relative to  the scheduled datetime (+ before or - after) for the task. Zero minutes is the default when &s is not entered.
+    - For tasks with an @s entry, jobs can also have &a, alert, and &b, beginning soon, notices. The entry for &a is given as a time period relative to &s (+ before or - after) and the entry for &b is a positive integer number of days before the scheduled date/time to begin displaying "beginning soon" notices. The entry for @s in the task becomes the default for &s in each job.  E.g., with
 
             - beginning soon example @s 1/30/2018
                 @j job A &s 5d &b 10
                 @j job B &b 5
 
         Beginning soon notices would begin on Jan 15 for job A (due Jan 25) and on January 25 for job B (due Jan 30).
     - Prerequisites
@@ -1581,15 +1673,15 @@
 
 [↺ contents](#contents)
 
 ### inbox {#inbox}
 
 Type character: **!**
 
-An inbox item can be regarded as a task that is always due on the current date. E.g., you have created an event to remind you of a lunch meeting but need to confirm the time. Just record it using **!** instead of **\*** and the entry  will appear highlighted in the agenda view on the current date until you confirm the starting time.
+An inbox item can be regarded as a task that is always due on the current date. E.g., you have created an event to remind you of a lunch meeting but need to confirm the time. Just record it using **!** instead of **\*** and the entry  will appear highlighted in the agenda view on the current date until you confirm the scheduled time.
 
 Corresponds to VTODO in the vcalendar specification.
 
 [↺ contents](#contents)
 
 ### status {#status}
 
@@ -1597,15 +1689,15 @@
 
 [↺ contents](#contents)
 
 #### beginning soon {#beginning-soon}
 
 Type character: **>**
 
-For unfinished tasks and other items with `@b` entries, when the starting date given by `@s` is within `@b` days of the current date, a warning that the item is beginning soon appears on the current date together with the item summary and the number of days remaining until the current date.
+For unfinished tasks and other items with `@b` entries, when the scheduled date given by `@s` is within `@b` days of the current date, a warning that the item is beginning soon appears on the current date together with the item summary and the number of days remaining until the current date.
 
 [↺ contents](#contents)
 
 #### past due {#past-due}
 
 Type character: **<**
 
@@ -1649,15 +1741,15 @@
 @ keys
 </h3>
 
 `@` followed by a character from the list below and a value appropriate to the key is used to apply attributes to an item. E.g.,
 
             @s mon 9a
 
-would specify the the starting datetime for the item is 9am on the Monday following the current date.
+would specify the the scheduled datetime for the item is 9am on the Monday following the current date.
 
 *  @+: include. list of datetimes to include
 *  @-: exclude. list of datetimes to exclude
 *  @a*: alert. list of + (before) or - (after) periods: list of commands
 *  @b: beginby. integer (number of days before)
 *  @c: calendar. string
 *  @d: description. string
@@ -1671,30 +1763,30 @@
 *  @l: location (aka context). forward slash delimited string. E.g., home/maintenance
 *  @m: mask. string stored in obfuscated form
 *  @n*: attendee. string using "[name:] address" format. If "address" begins with exactly 10 digits followed by an "@" it is treated as a mobile phone number. Otherwise it is treated as an email address. The optional "name:" can be used to facilitate autocompletion.
 *  @o: overdue. character from (r) restart, (s) skip, (k) keep, (p) preserve
 *  @p: priority. integer from 0 (none), 1 (low), 2 (normal), 3 (high), 4 (urgent)
 *  @r*: repetition frequency, a character from (y)early, (m)onthly, (w)eekly,
   (d)aily, (h)ourly or mi(n)utely, optionally followed by repetition &key entries
-*  @s: start. date or datetime
+*  @s: scheduled date or datetime
 *  @t*: tag. string
 *  @u*: usedtime. string using "timeperiod spent: ending datetime" format
 *  @w: wrap. A pair of before and after timeperiods to extend the busy period for an event, e.g., for travel time to and/or from the location of the event. Use `0m` as one of the timeperiods to avoid a wrap in that direction.
 *  @x*: expansion. string
 *  @z: timezone. string. A timezone specification, such as 'US/Eastern' or 'Europe/Paris' for aware datetimes or 'float', to indicate a naive or floating datetime. Datetime entries in the item are interpreted as belonging to the specified timezone when the entry is saved. The current timezone is the default when @z is not specified. Aware datetimes are converted to UTC (coordinated universal time) when stored and the @z entry, now irrelevant, is discarded.
 
 <h3 id="ampkeys">
 & keys
 </h3>
 
 & followed by a character from one of the lists below. These keys are only used with @j (job) and @r (repetition) entries.
 
 For use with @j:
 
-*  &s: start/due: period relative to @s entry (default 0m)
+*  &s: scheduled: period relative to @s entry (default 0m) at which job is scheduled to be completed
 *  &a: alert: list of + (before) or - (after) periods relative to &s: list of cmd names from the users configuration file
 *  &b: beginby. integer number of days before &s
 *  &d: description. string
 *  &e: extent. period
 *  &f: finished. datetime
 *  &l: location/context. string
 *  &m: masked. string stored in obfuscated form
@@ -1722,16 +1814,16 @@
 ## Notes {#notes}
 
 ### notices {#notices}
 
 * A link character, 'g', is appended to the *flags* column of any reminder with an `@g` goto link. Press `^g` with such a reminder selected to have the operating system open the link using the default application if the link can be interpreted as a file path or a url. E.g. if the link is a URL, then it would be opened using the default browser. If link can be interpreted as a shell command followed by arguments, then the command would be executed with the arguments.
 * An in-basket character, ⓘ , is appended to the right end of the status bar when a file named 'inbasket.text' is found in the etm root directory. This file should contain lines containing etm reminder entries - one on each line. It can be imported using the import file command bound to F5.
 * An update available character, 𝕦, is appended to the right end of the status bar when checking for updates is enabled and a later version of etm is available. Details for enabling checking for updates are in [configuration](#configuration).
-* Alerts and beginbys can be added to any reminder with an `@s` start date/time entry. Alerts require a datetime in `@s`; beginbys also allow a date in `@s`.
-* A beginby is specified by adding `@b n` to a reminder where `n` is a positive integer and is interpreted as a number of days. A reminder with such an entry will be displayed in *agenda view* on the current date provided that the current date is no more than `n` days before the start date/time of the reminder. Such a warning will appear n days before, n-1 days before and so forth until 1 day before the starting date/time of the reminder. The warning displays the type character `>`, the summary of the reminder and the number of days remaining.
+* Alerts and beginbys can be added to any reminder with an `@s` scheduled date/time entry. Alerts require a datetime in `@s`; beginbys also allow a date in `@s`.
+* A beginby is specified by adding `@b n` to a reminder where `n` is a positive integer and is interpreted as a number of days. A reminder with such an entry will be displayed in *agenda view* on the current date provided that the current date is no more than `n` days before the scheduled date/time of the reminder. Such a warning will appear n days before, n-1 days before and so forth until 1 day before the scheduled date/time of the reminder. The warning displays the type character `>`, the summary of the reminder and the number of days remaining.
 * An alert is specified by adding `@a <list of time periods>: <list of commands>` to a reminder. The time periods must be given in the usual etm format, e.g., `1h13m` for one hour and 13 minutes. The commands are single alphabetic characters, e.g., `a`, `b` and such. The commands used must either be `e` (email) or `t` (text) or be specified in the `alerts` section of the `cfg.yaml` file in your etm home directory. See [configuration](#configuration) for details about this file. Basically, it associates a command, such as `v` with a shell command to be invoked when an alert that includes `v` is triggered. E.g., the alert
 
 			@a 20m: v
 
     would be triggered 20 minutes before the datetime specified in the reminder's `@s` entry and at that time the shell command associated with `v` would be invoked. Both positive (before) and negative (after) time periods can be used. Thus this entry
 
 			@a 1d, -1h: v, w
@@ -1881,47 +1973,51 @@
 ### configuration {#configuration}
 
 Configuration settings for *etm* are specified in the file `cfg.yaml` located in your etm *home directory*. See [installation](#installation) for the location of this directory. When *etm* is running, you can press `F8` to open this configuration file using your system default editor for *yaml* (text) files. Note that any changes you make will not become effective until you stop and restart *etm*.
 
 Here are the options with their default values from that file. The lines beginning with `#` are comments that describe the settings.
 
     #### begin cfg.yaml ####
-	version: 4.9.1
-	# The current version of etm and this file. DO NOT EDIT. This is
-	# automatically updated when a new version of etm is installed.
+    etmversion: 4.11.18
+    # The current version of etm and this file. DO NOT EDIT. This is
+    # automatically updated when a new version of etm is installed.
 
     ampm: true
     # true or false. Use AM/PM format for datetimes if true else
-    # use 24 hour format.
+    # use 24 hour format. See also the show_minutes setting.
 
-    dayfirst:  true
+    show_minutes: false
+    # true or false. If true show ":00" in agenda and forthcoming views
+    # when displaying times with zero minutes else suppress zero minutes
+    # from being displayed. E.g., "9:00-10:30" if true else "9-10:30".
+    # When ampm if false and show_minutes is true, hours will be displayed
+    # with leading zeros applicable.
+
+    dayfirst:  false
     yearfirst: true
-    # true or false. Whenever an ambiguous date is parsed, dayfirst
+    # each true or false. Whenever an ambiguous date is parsed, dayfirst
     # and yearfirst parameters control how the information is processed
     # using this precedence:
-    #
-    #   If dayfirst is False and yearfirst is False:
-    #       MM-DD-YY
-    #       DD-MM-YY
-    #       YY-MM-DD
-    #
-    #   If dayfirst is True and yearfirst is False:
-    #       DD-MM-YY
-    #       MM-DD-YY
-    #       YY-MM-DD
-    #
-    #   If dayfirst is False and yearfirst is True:
-    #       YY-MM-DD
-    #       MM-DD-YY
-    #       DD-MM-YY
-    #
-    #   If dayfirst is True and yearfirst is True:
-    #       YY-MM-DD
-    #       DD-MM-YY
-    #       MM-DD-YY
+    # yearfirst: true
+    # 	dayfirst: true  => YDM
+    #   dayfirst: false => YMD
+    # yearfirst: false
+    # 	dayfirst: true  => DMY
+    #   dayfirst: false => MDY
+    # E.g., with both true, 3/4/5 would be interpreted as May 4, 2003.
+    # When possible, dates will also be displayed respecting these settings.
+    # I.e., the year will generally be displayed first when yearfirst is
+    # true and last otherwise. Similarly, the day will generally be displayed
+    # before the month when dayfirst is true and after the month otherwise.
+
+    beginbusy: 7
+    # non-negative integer. The number of hours after midnight to begin the
+    # busy view display of busy times for each day. The display continues
+    # for 14 hours after the begin_busy hour. E.g. with 'begin_busy: 7' the
+    # display would show busy times from 7am (7h) until 9pm (21h).
 
     updates_interval: 0
     # non-negative integer. If positive,  automatically check for updates
     # every 'updates_interval' minutes. If zero, do not automatically
     # check for updates. When enabled, a blackboard u symbol, 𝕦, will be
     # displayed at the right end of status bar when an update is available
     # or a question mark when the check cannot be completed as, for
@@ -1932,34 +2028,36 @@
     # for English (United States), "fr_FR" for French (France) and so
     # forth. Google "python locale abbreviatons" for a complete list."
 
     vi_mode: false
     # true or false. Use vi keybindings for editing if true else use emacs
     # style keybindings.
 
-    secret: KFI9R2AAaw
+    secret: HIr13FiYj3
     # string to use as the secret_key for @m masked entries. E.g.
     # 'X6i2SGWu6m'. In etm versions after 4.0.21, the default string is
     # randomly generated when this file is created or when the secret
     # value is removed and etm is restarted. WARNING: if this key is
     # changed, any @m entries that were made before the change will be
     # unreadable after the change.
 
     omit_extent:
     # A list of calendar names. Events with @c entries belonging to this
     # list will only have their starting times displayed in agenda view
     # and will neither appear nor cause conflicts in busy view.
 
-    keep_current: 0
-    # non-negative integer. If positive, the agenda for that integer
-    # number of weeks starting with the current week will be written to
-    # "current.txt" in your etm home directory and updated when necessary.
-    # You could, for example, create a link to this file in a pCloud or
-    # DropBox folder and have access to your current schedule on your
-    # mobile device.
+    keep_current: [0, 47]
+    # A list of two, non-negative integers for "weeks" and "width". If
+    # weeks is positive, the agenda for that integer number of weeks
+    # starting with the current week will be written to "current.txt" in
+    # your etm home directory and updated when necessary. The format will
+    # be scaled to fit "width". A width of 50, e.g, fits an iPhone display
+    # in portrait mode. You could, for example, create a link to
+    # "current.txt" in a pCloud or GoogleDrive folder and always have access
+    # to your current agenda on your mobile device.
 
     keep_next: false
     # true or false. If true, the 'do next' view will be written to
     # "next.txt" in your etm home directory. As with "current.txt", a link
     # to this file could be created in a pCloud or DropBox folder for
     # access from your mobile device.
 
@@ -1989,34 +2087,56 @@
     # current time.
 
     connecting_dots: false
     # true or false. If true, display dots connecting the item summary and
     # the right-hand details columns in tree views.
 
     usedtime_minutes: 1
-    # 1, 6, 12, 30 or 60. Round used times up to the nearest
-    # usedtime_minutes in used time views. With 1, no rounding is done and
-    # times are reported as hours and minutes. Otherwise, the prescribed
-    # rounding is done and times are reported as floating point hours.
-    # Note that each "@u" timeperiod is rounded before aggregation.
+    # 0, 1, 6, 12, 30 or 60. Round up used times. With 0, no rounding is done
+    # and times are reported in hours, minutes and seconds. With 1, after
+    # rounding up to the nearest minute, times are reported as hours and minutes.
+    # Otherwise, rounding is up to the nearest integer multiple of
+    # usedtime_minutes and times are reported as floating point hours. E.g.,
+    # with usedtime_minutes = 6, 1 minute would be rounded up to 6 minutes and
+    # reported as 0.1 hours. Similarly 13 minutes would be rounded up to 18
+    # minutes and reported as 0.3 hours. Note that when rounding is specified,
+    # each "@u" timeperiod is rounded before aggregation.
+
+    usedtime_hours: 6
+    # 0, 1, 2, ..., 24. The daily goal for used time. This is used in engaged
+    # view to control the display of the daily used time bars. The goal is to
+    # to maximize the granularity of the bar when displaying this number of hours
+    # in the space allowed by the terminal width.
+
+    journal_name: daily
+    # Journal items with this index entry and with an @s entry will have the
+    # year and month appended to the index. E.g., with the setting
+    #   journal_name: daily
+    # this journal entry
+    #   % visited Yellowstone @s 22/6/24 @i daily
+    # would be displayed in journal view as if the index entry were
+    #   @i daily/2022/ 6
+    # thus organizing such entries by the year and month of their scheduled dates.
+    # Within each month, entries will be also ordered by the month day.
 
     alerts:
     # A dictionary with single-character, "alert" keys and corresponding
     # "system command" values. Note that characters "t" (text message) and
     # "e" (email) are already used.  The "system command" string should be
     # a comand with any applicable arguments that could be run in a
     # terminal. Properties of the item triggering the alert can be
     # included in the command arguments using the syntax {prop}, e.g.,
     # {summary} in the command string would be replaced by the summary of
-    # the item. Similarly {start} by the starting time, {when} by the time
-    # remaining until the starting time, {location} by the @l entry and
-    # {description} by the @d entry. E.g., If the event "* sales meeting
-    # @s 2019-02-12 3p" triggered an alert 30 minutes before the starting
-    # time the string "{summary} {when}" would expand to "sales meeting in
-    # 30 minutes". E.g. on my macbook
+    # the item. Similarly {start} by the starting datetime, {time} by the
+    # starting time (omits the date for the current date), {when} by the time
+    # remaining until the starting datetime, {now} by the current time,
+    # {location} by the @l entry and {description} by the @d entry. E.g., If
+    # the event "* sales meeting @s 2019-02-12 3p" triggered an alert 30 minutes
+    # before the starting time the string "{summary} {when}" would expand to
+    # "sales meeting in 30 minutes". E.g. on my macbook
     #
     #    alerts:
     #        v:   /usr/bin/say -v "Alex" "{summary}, {when}"
     #        ...
     #
     # would make the alert 'v' use the builtin text to speech sytem
     # to speak the item's summary followed by a slight pause
@@ -2033,18 +2153,18 @@
     #        ...
     #
     # then when "@x tennis" is entered the popup completions for
     # "@x tennis" would offer replacement by the corresponding
     # "@e 1h30m @a 30m: d @i personal:exercise".
 
     sms:
-      body: "{location} {when}"
-      from:
-      server:
-      pw:
+    body: '{location} {when}'
+    from:
+    server:
+    pw:
     # Settings to send "t" (sms text message) alerts to the
     # list of phone numbers from the item's @n attendee
     # entries using the item's summary and the body as specified
     # in the template below as the message. E.g., suppose you
     # have a gmail account with email address "who457@gmail.com"
     # and want to text alerts to Verizon moble phone (123)
     # 456-7890. Then your sms entries should be
@@ -2057,19 +2177,19 @@
     # gateway for Verizon. Other common mms gateways are
     #     AT&T:     @mms.att.net
     #     Sprint:   @pm.sprint.com
     #     T-Mobile: @tmomail.net
     # Note. Google "mms gateway listing" for other alternatives.
 
     smtp:
-      body: "{location} {when}\n{description}"
-      from:
-      server:
-      id:
-      pw:
+    body: '{location} {when}\n{description}'
+    from:
+    server:
+    id:
+    pw:
     # Settings to send "e" (email message) alerts to the list of email
     # addresses from the item's @n attendee entries using the item's
     # summary as the subject and body as the message. E.g., if you have a
     # gmail account with email address "whatever457@gmail.com", then your
     # entries should be
     #     from: whatever457@gmail.com
     #     id: whatever457
@@ -2094,14 +2214,18 @@
     # values. Each "query" must be one that could be entered as the
     # command in query view. Keys can be any short string other than
     # 'a', 'u', 'c' or 'l' which are already in use.
     # queries:
     #    td: m l -q equals itemtype - and ~exists f
     #    mi: exists u and ~exists i
     #    arch: a exists itemtype
+    #    find: includes summary d {}
+    # The latter would allow you to enter, e.g., `find waldo` and have
+    # it expand to `includes summary d waldo` and thus locate all
+    # reminders with `waldo` either in the summary or d (the description).
 
     style: dark
     # dark or light. Set the defaults for dark or light terminal
     # backgounds. Some output may not be visible unless this is set
     # correctly for your display.
 
     type_colors:
@@ -2116,30 +2240,35 @@
     #  event           'LimeGreen',        'DarkGreen',
     #  finished        'DarkGrey',         'LightSlateGrey',
     #  inbox           'OrangeRed',        'MediumVioletRed',
     #  journal         'GoldenRod',        'Brown',
     #  pastdue         'LightSalmon',      'Red',
     #  plain           'Ivory',            'Black',
     #  today           'Ivory bold',       'Black bold',
+    #  used            'Khaki',            'DodgerBlue',
     #  waiting         'SlateGrey',        'DarkSlateBlue',
-	#  wrap            'SlateGrey',        'DarkSlateBlue',
-    #
+    #  wrap            'ForestGreen',      'LightGrey',
+    #  running         'OrangeRed',        'Gold',
+    #  paused          'MediumVioletRed',   'DarkViolet',
     # Explanations for the key names:
     #     available:    available task/job reminders
     #     begin:        begin by warnings
     #     event:        event reminders
     #     finished:     finished task/job reminders
     #     inbox:        inbox reminders
     #     journal:      journal reminders
     #     pastdue:      pasdue task warnings
     #     plain:        headings such as outline branches
     #     today:        the current and following agenda date headings
+    #     used:         used time rows in engaged and used time views
     #     waiting:      waiting job reminders (jobs with unfinished prereqs)
-	#     wrap:         before and after rows for events in agenda view with
-	#                   @w entries
+    #     wrap:         before and after rows for events in agenda view with
+    #                   @w entries
+    #     running:      status bar color for 'r', running timer
+    #     paused:       status bar color for 'p', paused timer
     #
     # E.g., with style 'dark', the default color for 'available' is
     # 'LightSkyBlue'. This entry
     #   colors:
     #       available: CornFlowerBlue
     # would change the 'available' color to 'CornflowerBlue' while leaving
     # the other 'dark' colors unchanged.
@@ -2155,15 +2284,15 @@
     #    [background, foreground, attribute]
     # components. background and foreground can either be named colors,
     # hex colors, or ''. Attribute is an optional font attribute such
     # as 'bold' which must, of course, be supported by the font used in
     # your terminal. The default settings are determined by the 'dark'
     # or 'light' style setting as follows:
     #
-    #    key                           dark                        light
+    #    key                       dark default                  light default
     # -------------------    -----------------------------  -----------------------------
     # ask:                    [grey2, Lime, bold]           [Cornsilk, Lime, bold]
     # button.focused:         [DarkGreen, White]            [DarkGreen, White]
     # details:                [, Ivory]                     [, Black]
     # dialog shadow:          [#444444, ]                   [#444444, ]
     # dialog:                 [DarkSlateGrey, White]        [DimGrey, White]
     # dialog-entry:           [White, Black]                [White, Black]
@@ -2189,20 +2318,23 @@
     #
     # Note that 'grey1' (#396060) and 'grey2' (#1d3030) are colors named
     # within etm itself. They are, respectively, one shade lighter and two
     # shades darker than DarkSlateGrey.
     #
     # Any of the style attributes above can be modified. E.g., with style
     # 'dark', the default for 'text-area' is [grey2, Ivory]. This entry
-    #   style_modifications:
+    #   window_colors:
     #       text-area: [Black, White]
     # would change the 'text-area' setting to 'Black' as the background color
     # and 'White' as the foreground color while leaving the other style settings
     # unchanged.
-	#### end cfg.yaml ####
+    #### end cfg.yaml ####
+
+
+See [Saved Queries](#saved-queries) for more information about queries that allow for replaceable parameters.
 
 Note that in the 'dictionary' entries above, the components must be indented (using 2 spaces not tabs). E.g., the illustrative alert entry would be:
 
 	alerts:
 		v: /usr/bin/say -v "Alex" "{summary}, {when}"
```

### Comparing `etm-dgraham-4.9.7/README.md` & `etm-dgraham-5.0.3/etm_dgraham.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,34 @@
+Metadata-Version: 2.1
+Name: etm-dgraham
+Version: 5.0.3
+Summary: event and task manager
+Home-page: https://dagraham.github.io/etm-dgraham/
+Author: Daniel A Graham
+Author-email: dnlgrhm@gmail.com
+License: GPL
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Office/Business
+Classifier: Topic :: Office/Business :: News/Diary
+Classifier: Topic :: Office/Business :: Scheduling
+Requires-Python: >=3.7.3
+Description-Content-Type: text/markdown
+
+
 <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/etmlogo.png" alt="etm" title="event and task manager" width="200px" />
 
-This is the etm user manual. It is best viewed at [GitHub.io](https://dagraham.github.io/etm-dgraham/) where all the internal, contents links work correctly. etm itself is available from [PyPi](https://pypi.org/project/etm-dgraham/) and [GitHub](https://github.com/dagraham/etm-dgraham) and further information from the etm discussion group at [groups.io](https://groups.io/g/etm) - note especially the [files](https://groups.io/g/etm/files/) folder. Brief how-to videos are available at [youtube](https://www.youtube.com/playlist?list=PLN2WQIqrwSxxh2eNY_YczO6YC-icpKWeG).
+This is the etm user manual. It is best viewed at [GitHub.io](https://dagraham.github.io/etm-dgraham/) where all the internal, contents links work correctly. etm itself is available from [PyPi](https://pypi.org/project/etm-dgraham/) and [GitHub](https://github.com/dagraham/etm-dgraham) and further information from the etm discussion group at [groups.io](https://groups.io/g/etm-dgraham). Brief how-to videos are available at [youtube](https://www.youtube.com/@etm-dgraham).
 
 
 # Contents {#contents}
 -   [Overview](#overview)
     -   [Reminders](#reminders)
         -   [examples](#examples)
         -   [text entry versus forms](#text-entry-versus-forms)
@@ -25,26 +49,29 @@
             -   [Simple query examples](#simple-query-examples)
             -   [Archive queries](#archive-queries)
             -   [Update queries](#update-queries)
             -   [Complex queries](#complex-queries)
             -   [Command History](#command-history)
             -   [Saved Queries](#saved-queries)
         -   [Common Features](#common-features)
+    -   [Mobile Access to your reminders](#mobile)
     -   [Menus](#menus)
         -   [etm menu notes](#etm-menu-notes)
         -   [view menu notes](#view-menu-notes)
         -   [editor menu notes](#editor-menu-notes)
         -   [selected menu notes](#selected-menu-notes)
     -   [Installation](#installation)
         -   [For personal use](#for-personal-use)
-        -   [for use in a virtual environment](#for-use-in-a-virtual-environment)
+        -   [for use in an isolated environment](#for-use-in-an-isolated-environment)
         -   [for use system wide](#for-use-system-wide)
     -   [Usage](#usage)
         -   [Terminal size and color](#terminal-size-and-color)
         -   [Home directory](#home-directory)
+        -   [Timers](#timers)
+        -   [lorem examples](#loremexamples)
         -   [Using etm+](#etmplus)
     -   [Deinstallation](#deinstallation)
         -   [From a virtual environment](#from-a-virtual-environment)
         -   [From a system wide installation](#from-a-system-wide-installation)
 -   [Details](#details)
     -   [Item Types](#item-types)
         -   [event](#event)
@@ -66,19 +93,21 @@
 			- [anniversary substitutions](#anniversary-substitutions)
         -   [archived reminders](#archived-reminders)
         -   [configuration](#configuration)
         -   [data storage](#data-storage)
 
 # Overview {#overview}
 
+*etm* began life in 2013 as *etm-qt* sporting a gui based on *Qt*. The intent was to provide an app supporting GTD (David Allen's Getting Things Done) and exploiting the power of python-dateutil. The name changed to *etmtk* in 2014 when *Tk* replaced *Qt*. Development of *etmtk* continued until 2019 when name changed to *etm-dgraham*, to honor the PyPi naming convention, and the interface changed to a terminal based one based on *promt_toolkit*. Features have changed over the years but the text based interface and basic format of the reminders has changed very little. The goal has always been to be the Swiss Army Knife of tools for managing reminders.
+
 ## Reminders {#reminders}
 
 *etm* offers a simple way to manage your events, tasks and other reminders.
 
-Rather than filling out fields in a form to create or edit reminders, a simple text-based format is used. Each reminder in *etm* begins with a *type character* followed by a brief *summary* of the item and then, perhaps, by one or more *@key value* pairs to specify other attributes of the reminder. Mnemonics are used to make the keys easy to remember, e.g, @s for starting datetime, @l for location, @d for description and so forth.
+Rather than filling out fields in a form to create or edit reminders, a simple text-based format is used. Each reminder in *etm* begins with a *type character* followed by a brief *summary* of the item and then, perhaps, by one or more *@key value* pairs to specify other attributes of the reminder. Mnemonics are used to make the keys easy to remember, e.g, @s for scheduled datetime, @l for location, @d for description and so forth.
 
 The 4 types of reminders in etm with their associated type characters:
 
 * task: **-**
 * event: **\***
 * journal: **%**
 * inbox: **!**
@@ -99,38 +128,38 @@
 
 * A journal entry (**%**): a favorite Churchill quotation that you heard at 2pm today with the quote itself as the [d]escription.
 
         % Give me a pig - Churchill @s 2p @d Dogs look up at
           you. Cats look down at you. Give me a pig - they
           look you in the eye and treat you as an equal.
 
+	The *summary*, "Give me a pig - Churchill" in this example, follows the type character and is meant to be brief - analagous to the subject of an email. The optional *description* follows the "@d" and is meant to be more expansive - analagous to the body of an email.
+
 * A task (**-**): build a dog house, with component [j]obs.
 
         - Build dog house @j pick up materials @j cut pieces
           @j assemble @j sand @j paint
 
-* Inbox (**!**): meet Alex for coffee Friday. This can be
-  changed to an event when the time is confirmed by
-  replacing the **!** with an **\*** and adding the time to `@s`.
+* Inbox (**!**): meet Alex for coffee Friday.
 
         ! Coffee with Alex @s fri @e 1h
 
-    This inbox entry will appear on the current day in *agenda view* until you make the changes.
+	This can be changed to an event when the details are confirmed by replacing the **!** with an **\*** and adding the time to `@s`.  This inbox entry will appear on the current day in *agenda view* until you make the changes.
 
 * An appointment (event) for a dental exam and cleaning at 2pm on Feb 5 and then again [@+] at 9am on Sep 3.
 
         * dental exam and cleaning @s 2p feb 5 2019 @e 45m
           @+ 9am Sep 3 2019
 
 [↺ contents](#contents)
 
 ### text entry versus forms {#text-entry-versus-forms}
 
 * Text entry removes the need to hunt for and click in the relevant entry box and allows you to keep your fingers on the keyboard.
-* Text entry supports the full flexibility of the superb Python *dateutil* package. Consider, for example, creating a reminder for Presidential election day which repeats every 4 years on the first Tuesday after a Monday in November (a monthday falling between 2 and 8). In *etm*, this event would be
+* Text entry supports the full flexibility of the superb Python *dateutil* package. Consider, for example, creating a reminder to vote for President election day which repeats every 4 years on the first Tuesday after a Monday in November (a Tuesday whose monthday falls between 2 and 8). In *etm*, this event would be
 
         * Presidential election day @s nov 1 2020 @r y &i 4 &M 11
           &m 2, 3, 4, 5, 6, 7, 8 &w tu
 
     Try this with a form based calendar application.
 
 [↺ contents](#contents)
@@ -138,14 +167,15 @@
 ### unobtrusive and timely entry assistance {#unobtrusive-and-timely-entry-assistance}
 
 When you want to create a new reminder or edit an exiting one, *etm* opens an area at the bottom of the screen that is divided into two parts by a horizontal line. The lower part is the entry area where what you type appears. The upper part is the prompt/feedback area where *etm* responds to your typing. This response might take the form of providing a suggestion about alternatives, information about the type of input required or feedback about how your current entry is being interpreted. It is important to realize that none of this interferes with your typing - you can blaze away as quickly as you like or even paste complete entries and never glance at the prompt if you like. This is the **unobtrusive** part of the prompt/feedback process.
 
 <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/new.png" alt="new" title="new entry" width="600px" hspace="20px"/>
 
 
+
 [↺ contents](#contents)
 
 #### just in time entry prompts and feedback {#just-in-time-entry-prompts-and-feedback}
 
 Let's create the election day reminder to illustrate the **timely** part of the process. Begin by pressing `N` to create a new reminder and notice that *etm* automatically prompts you for the item type character and suggests the alternatives.
 
         item type
@@ -162,35 +192,35 @@
 
         ────────────────────────────────────────────────────────────
         *_
 
 Enter the summary followed by an `@` and *etm* will automatically display the required and available `@-keys`.
 
         @-key
-        required: @s (start)
+        required: @s (scheduled)
         available: @+ (include), @- (exclude), @a (alerts),
         @b (beginby), @c (calendar), @d (description),
         @e (extent), @g (goto), @i (index), @l (location),
         @m (mask), @n (attendee), @o (overdue),
-        @r (repetition frequency), @s (start), @t (tag),
+        @r (repetition frequency), @s (scheduled), @t (tag),
         @u (used time), @x (expansion), @z (timezone)
         ────────────────────────────────────────────────────────────
         * Presidential election day @_
 
-You see that `@s` is required, so add the `s` and *etm* will prompt you for the value for the start option and describe the type of input required.
+You see that `@s` is required, so add the `s` and *etm* will prompt you for the value for the scheduled option and describe the type of input required.
 
-        start
-        starting date or datetime
+        scheduled
+        scheduled date or datetime
 
         ────────────────────────────────────────────────────────────
         * Presidential election day @s_
 
 As you enter the datetime, *etm* will display its interpretation of your entry.
 
-        start
+        scheduled
         Sun Nov 1 2020
 
         ────────────────────────────────────────────────────────────
         * Presidential election day @s nov 1 20_
 
 Now append an `@` to see the prompt for options and notice that `@s`, having been provided, is no longer listed.
 
@@ -279,15 +309,15 @@
             │   Tue Nov 2 2032                 │
             │   Tue Nov 4 2036                 │
             │                                  │
             │           <    OK    >           │
             │                                  │
             └──────────────────────────────────┘
 
-These are the first 5 repetitions on or after Nov 1 2020. Notice that the start value of Nov 1 2020 is not one of the repetitions since it doesn't satisfy the requirements. These appear correct, so press ^S to save the reminder.
+These are the first 5 repetitions on or after Nov 1 2020. Notice that the scheduled value of Nov 1 2020 is not one of the repetitions since it doesn't satisfy the requirements. These appear correct, so press ^S to save the reminder.
 
 
 General observations:
 
 * The general structure of this reminder is
 
 			* Presidential election day
@@ -304,67 +334,67 @@
 * The prompts provide "just in time" information relevant to the entry you are typing and need only be consulted if you are uncertain about your entry. With a little
 	experience, most reminders can be completed without a glance at the prompt.
 
 [↺ contents](#contents)
 
 #### fuzzy parsing of datetimes {#fuzzy-parsing-of-datetimes}
 
-Whenever *etm* expects a datetime entry as, for example, when you are entering an `@s` starting datetime, it applies fuzzy parsing to your entry.  Suppose it is Dec 17 2019, your computer is in the Eastern timezone and you have just entered `@s` for your lunch event
+Whenever *etm* expects a datetime entry as, for example, when you are entering an `@s` scheduled datetime, it applies fuzzy parsing to your entry.  Suppose it is Dec 17 2019, your computer is in the Eastern timezone and you have just entered `@s` for your lunch event
 
-        start
-        starting date or datetime
+        scheduled
+        scheduled date or datetime
 
         ────────────────────────────────────────────────────────────
         * lunch @s_
 
 If you enter `1`, *etm* will interpret it as 1am on the current date in the local timezone.
 
-        start
+        scheduled
         Tue Dec 17 2019 1:00am EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1_
 
 Adding `p` changes the interpretation to 1pm.
 
-        start
+        scheduled
         Tue Dec 17 2019 1:00pm EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p_
 
 Now start adding 'fri' by appending an 'f'.
 
-        start
+        scheduled
         '1p f' is incomplete or invalid
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p f_
 
 and *etm* will complain that the entry is now either incomplete or invalid. Add the remaining 'ri'.
 
-        start
+        scheduled
         Fri Dec 20 2019 1:00pm EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p fri_
 
 and *etm* understands that you want the coming Friday, Dec 20. Now suppose that you will be in California on Friday and you want Pacific, not Eastern time. Then add an entry for `@z`.
 
-        start
+        scheduled
         local datetime: Fri Dec 20 2019 4:00pm EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p fri_ @z US/Pacific
 
 Note that `local datetime` is now prepended to the result which is still displayed in the local timezone, since that is the location of your computer, but the time has changed to `4:00pm EST` which, of course, is the same time as `1:00pm PST`. *etm* **always** displays times in the current local time zone. When you save this item, the time will be converted to universal time and the `@z US/Pacific` will be deleted - once the time has been converted, the original timezone is no longer relevant.
 
 What if you had entered the 'fri' first?
 
-        start
+        scheduled
         Fri Dec 20 2019
 
         ────────────────────────────────────────────────────────────
         * lunch @s fri
 
 Here *etm* supposes again that you want the coming Friday, Dec 20 but without a time being specified, it is interpreted as a date rather than a datetime and thus without a timezone. Add the `1p` and timezone the result will be the same as before.
 
@@ -375,15 +405,15 @@
         or 'float' to specify a naive/floating datetime
 
         ────────────────────────────────────────────────────────────
         * lunch @s fri 1p @z
 
 and note that supplying 'float' as the timezone does the trick.
 
-        start
+        scheduled
         Fri Dec 20 2019 1:00pm
 
         ────────────────────────────────────────────────────────────
         * lunch @s fri 1p_ @z float
 
 The datetime now appears without either the 'local datetime' prefix or the 'EST' suffix which reveals that it is a naive/floating datetime.
 
@@ -466,54 +496,74 @@
 
 The display for each reminder shows the itemtype and summary column on the left followed by a *flags* column which displays a combination of letters from 'g' (goto), 'k' (connection), 'p' (pinned) and 't' (timer) reflecting the presence of these attributes in the reminder. This column is sometimes followed on the extreme right by another column whose contents depends on the view. E.g. in index and journal views the 'id' of the reminder is displayed while in history view, the last modification timestamp of the reminder is displayed.
 
   * a: Agenda: dated unfinished tasks and other reminders by year-week and week day
   * b: Busy: a graphical illustration of busy and conflicted times by year-week
   * c: Completed: finished tasks and jobs and used time entries by year-week and week day
   * d: Do Next: undated tasks grouped by location/context and ordered by priority (highest first) and extent (least first)
+  * e: Engaged: instances of reminders with used time entries with daily totals displayed graphically
   * f: Forthcoming: unfinished dated tasks and other dated reminders by next occurrence
   * h: History: all items by the latter of the modified or created datetimes in descending order, i.e., most recent first. Datetimes are displayed using a 5 character format where, e.g., 1:15pm today would be displayed as 13:15, November 7 of the current year as 11/17 and January 15 of 2012 as 12.01.
   * i: Index: all items grouped hierarchically by index entry
   * j: Journal: journal entries grouped hierarchically by index entry
   * k: Konnection: items with @k konnection links either to or from the selected item.
   * l: Location: items grouped hierarchically by location entry
   * m: Timers: items with timers.
   * p: Pinned: items whose pin status is on.
   * q: Query: items matching a user specified query. Enter ? for query usage.
   * r: Review: undated tasks sorted by the time since the task was last modified with the most recently modified last.
   * t: Tags: all items with @t tag entries grouped by tag
   * u: Used Time: all items with @u used time entries grouped by month and hierarchically by index
   * U: Used Summary: used time aggregates grouped by month and hierarchically by index
-  * y: Yearly Planning Calendar: compact monthly calendar by half year.
+  * y: Yearly Planning Calendar: compact monthly calendar.
 
 
 [↺ contents](#contents)
 
 ### Weekly Views {#weekly-views}
 
-The _weekly_ agenda, busy and completed views display one week at a time and are *synchronized* so that all three views always display the same week. Left or right cursor keys go backward or forward a week at a time and the pressing the space bar jumps to the week containing the current day. You can also press "J" and enter a date to jump to the week containing the date.
+The _agenda_, _busy_, _completed_ and _engaged_ views display one week at a time and are *synchronized* so that all four views always display the same week. Press the ▶ (right) or ◀ (left) cursor keys go forward or backward a week at a time or press the space bar to jump to the week containing the current day. You can also press "J" and enter a date to jump to the week containing the date.
+
+In _agenda_ view, only days with scheduled reminders are listed. If nothing is scheduled for the entire week, then "Nothing scheduled" is displayed.
+
+
+In _busy_ view, only days that have events with busy times (@e and/or @w entries) are displayed. Press the number of the weekday, [1→Mon, ..., 7→Sun], to show the details of the busy periods from that day or press the ▼ (down) or ▲ (up) cursor keys to show the details of the next or previous day with busy periods.
+
+_Completed_ view shows instances of completed tasks.
 
-In both agenda and completed views, only days with scheduled reminders are listed. If nothing is scheduled for the entire week, then "Nothing scheduled" is displayed.
+_Engaged_ view shows instances of reminders with used time entries with daily totals displayed graphically.
 
 The normal agenda listing for a week day:
 
 * all day events (events with dates as `@s` entries)
 * datetime items (reminders with datetimes as `@s` entries) by time
 * all day tasks (tasks with dates as `@s` entries)
 * all day journal enties (journal entries with dates as `@s` entries)
 
 And, on the current day only:
 
 * inbox items
 * *<* past due warnings in descending order of the number of days past due
 * *>* beginby warnings in ascending order of the number of days remaining
 
+Busy view requires a little explanation. Here is screen shot of agenda view for an illustrative week
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/agenda.png" alt="new" title="agenda view" width="600px" hspace="20px"/>
+
+along with one of busy view for the same week
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/busy.png" alt="new" title="busy view" width="600px" hspace="20px"/>
+
+The first thing to notice in busy view is that busy times are displayed each week day for the period between 7am and 9pm. This period is determined by the *beginbusy* setting in `cfg.yaml` which sets the number of hours after midnight that the display is to begin each day. The period ends 14 hours after *beginbusy*. In this case, it runs from 7 hours after midnight (*beginbusy*) to 7+14=21 hours after midnight or from 7am until 9pm. The resolution is 15 minute periods for each character *slot* so that, for example, the row for *Fr 2* shows a busy period with using 4 green (busy) characters for 10-10:15am, 10:15-10:30am, 10:30-10:45am and 10:45-11am. Now you might notice that this implies that the 4 character slots that begin at 8pm end just before the 9pm slot and that the 9pm slot actually corresponds to the interval 9-9:15pm. Since the actual display includes this last slot, it actually extends for 14 hours plus 15 minutes and thus actually ends at 9:15pm.
+
+The second thing to notice is the red, conflict bar in the display for *Mo 28*. Since the details for this day are displayed in the "busy times" panel at the bottom as well as in the agenda view, you will notice that the conflict corresponds to the overlap between the 6-8am event and the 7-9:30am event. This conflict from 7-8am is illustrated by the 4 red (conflict) characters. Notice also that the period for the first event extends from 6-7am before the period displayed begins at 7am. The single green character to the left of 7am indicates that there were busy times before the displayed period begins. Similarly, the green character to the right of 9-9:15pm on *We 30* indicates that there were busy times after 9:15pm on that day. This corresponds to the 8-10:30pm event shown in agenda view for Wednesday that extends from 9:15-10:30pm after the displayed period.
+
+As you might expect, if a conflict occurred either before or after the displayed period then the corresponding *before* or *after* character would be red instead of green.
+
 [↺ contents](#contents)
 
-### Timer view {#timer-view}
+### Timer View {#timer-view}
 
 This view lists all reminders with associated timers sorted by the elapsed time since the timer's *state* was last changed. The display for each reminder shows the itemtype and summary, any applicable *flags* and, in the right hand column, the elapsed time and *state* of the associated timer.
 
 The sort order assures that the reminder with the active timer will always be at the top of the list and followed by the reminders with the most recently modified timers. This makes it easy to switch back and forth between recent timers.
 
 [↺ contents](#contents)
 
@@ -550,26 +600,28 @@
 reminders with links from the selection
 : the list of items whose ids are included in the @k entries of the selected item
 
 [↺ contents](#contents)
 
 ### Used Time Views {#used-time-views}
 
-The *used time* and *used time summary* views are bound to `u` and `U` respectively. They report `@u` (used time) entries in your reminders grouped by year-month and then heirarchially by `@i` entries. I have a file of reminders with `@i` and `@u` entries such as
+The *used time* and *used time summary* views are bound to `u` and `U` respectively. They report `@u` (used time) entries in your reminders, rounded up according to the `usedtime_minutes` setting in your `cfg.yaml` file and grouped by year-month and then heirarchially by `@i` entries.
+
+I have a file of reminders with `@i` and `@u` entries such as
 
 		* Modi ut sit sed amet sit @s 2019-11-11 10:00am @e
 		   1h30m
 		@u 58m: 2019-11-11 10:58am @u 34m: 2019-11-11 10:34am
 		@i client A/project a1/correspondence
 		@d Aliquam non sed aliquam eius tempora quisquam dolorem.
 		Neque quiquia labore tempora magnam. Quiquia tempora
 		porro est ut. Ut tempora sed non ut eius neque porro.
 		Sed quaerat consectetur dolor sit.
 
-and the *used time view* for November begins with
+With `usedtime_minutes: 6`, the *used time view* for November begins with
 
 		November 2019
 		  client A
 			project a1
 			  correspondence
 				* Modi ut sit sed amet sit: 1.6h Nov 11
 				% Amet modi neque eius adipisci: 2.7h Nov 27
@@ -971,14 +1023,15 @@
 * monthend: 12am on the 1st of the following month
 
 and can be combined with period strings using M (month),
 w (week), d (day), h (hour) and m (minute). E.g.:
 * `weekbeg - 1w`  (the beginning of the previous week)
 * `monthend + 1M` (the end of the following month)
 
+
 [↺ contents](#contents)
 
 #### Command History {#command-history}
 
 Any query entered at the 'query:' prompt and submitted by pressing 'Enter' is added to the command history. These queries are kept as long as 'etm' is running and can be accessed using the up and down cursor keys in the query field. This means you can enter a query, check the result, press 'q' to reopen the query prompt, press the up cursor and you will have your previous query ready to modify and submit again. It is also possible to keep a permanent list of queries accessible by shortcuts. See 'Saved Queries' below.
 
 [↺ contents](#contents)
@@ -1082,14 +1135,31 @@
 	* While entering the search expression, push the `up` or `down` cursor keys to change the direction of search.
     * After entering the search expression, press “n” to search (cyclically) for other matches in the direction specified.
 	* Once a search is initiated, it remains active in all views with matches highlighted. To remove the highlighting, search for something unlikely to be matched, e.g., 3 consecutive commas.
 
 
 [↺ contents](#contents)
 
+## Mobile access to your reminders {#mobile}
+
+The files `current.txt` and `next.txt` in your etm home directory are created by *etm* but not displayed within *etm* itself. Whether or not these files are created depends on two settings in your `cfg.yaml`:
+
+* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary.
+
+* `keep_next`: true or false. If `true`, the contents of *do next* view will be written to `next.txt` in your etm home directory and updated whenever necessary.
+
+By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule and tasks on your mobile device.
+
+Here is a screen shot from an iPhone of an illustrative `current.txt`:
+
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/current_on_iphone.png" alt="new" title="current view" width="300px" hspace="20px"/>
+
+
+[↺ contents](#contents)
+
 ## Menus {#menus}
 
 Pressing F1 toggles the *etm* menu display - opening it if it is closed and closing it if it is open. There are four menu tabs labeled *etm*, *view*, *editor* and *selected* with the options listed below:
 
     etm
 		F1) activate/close menu
         F2) about etm
@@ -1102,35 +1172,38 @@
         ---
         ^q) quit
     view
         a) agenda
         b) busy
         c) completed
         d) do next
+        e) engaged
         f) forthcoming
         h) history
         i) index
         j) journal
         l) location
         p) pinned
         q) query
 		r) review
         t) tags
         u) used time
         U) used time summary
+        v) refresh views to fit resized terminal
         ---
         s) scheduled alerts for today
-        y) half yearly calendar
+        y) yearly calendar
         ---
         /) search forward
         ?) search backward
         n) next incrementally in search
         ^l) prompt for and jump to line number
         ^p) jump to next pinned item
-        ^c) copy active view to clipboars
+        ^c) copy active view to clipboard
+        ^t) start quick timer
         ---
         J) jump to date in a), b) and c)
         right) next in a), b), c), u), U) and y)
         left) previous in a), b), c), u), U) and y)
         space) current in a), b), c), u), U) and y)
     editor
         N) create new item
@@ -1151,16 +1224,17 @@
         g) open goto link
         k) show konnections
         ^r) show repetitions
 		^u) update last modified
         ^x) toggle archived status
         ---
         T) change timer to next state
-        TR) record usedtime and delete timer
+        TR) record usedtime and end timer or add usedtime
         TD) delete timer
+        ---
         TT) toggle paused/running for active timer
 
 
 [↺ contents](#contents)
 
 ### etm menu notes {#etm-menu-notes}
 
@@ -1186,14 +1260,15 @@
 
 [↺ contents](#contents)
 
 ### view menu notes {#view-menu-notes}
 
 The *view* menu provides access to all the *etm* views with the shortcut keys for these views. E.g., press `a` to open *agenda view*.
 
+The *start quick timer* option creates a new, inbox reminder with the current datetime as the subject, associates a timer with reminder and starts the timer. If another timer is active, it will be paused if necessary and made inactive. Subsequent invocations repeat this process.
 
 The entries here are pretty obvious and the views themselves are descibed elsewhere.
 
 [↺ contents](#contents)
 
 ### editor menu notes {#editor-menu-notes}
 
@@ -1214,102 +1289,86 @@
 * *reschedule* will prompt for a datetime. If the reminder is repeating, the provided datetime will replace the datetime of the selected instance. Otherwise it will be used either to replace the current value of `@s` or, if there is no `@s` entry, to create one.
 * *schedule new* will prompt for a datetime and add that instance to any other instances of the reminder.
 * *open goto* will use the system default application to open the file path or url specified in the selected reminders `@g` entry. Items with goto links are displayed with a 'g' in the *flags* column of normal views.
 * *toggle pin* toggles the pin status of an item between off and on. Items for which the pin status are displayed with a 'p', in the *flags* column of normal views and are also displayed in *pinned view*.
 * *show repetitions* pops up a display showing illustrative repetitions if the item is repeating.
 * *toggle archived status* moves the selected reminder from the items table if it is active to the archive table and vice versa if the archive table is active.
 * *change timer to next state*.
-    * these are the states for the timer associated with a reminder and the relevant status of any other timers:
+    * These are the states for the timer associated with a reminder and the relevant status of any other timers:
         * *n* (no timer is associated with this reminder)
             * *n-*: no other timer is active
             * *n+*: another timer is active
         * *i* (a timer is associated with this reminder and it is inactive)
             * *i-*: no other timer is active
             * *i+*: another timer is active
         * *r-*: running (a timer is associated with this reminder and it is running - there cannot be another active timer)
         * *p-*: paused (a timer is associated with this reminder and it is paused - there cannot be another active timer)
 
-       These are the "next" state transitions associated with this action:
+    * These are the "next" state transitions associated with this action:
         * *n+* ⇒ *i+*
-        * *n-* ⇒ *r-*
+        * *n-* ⇒ *p-*
         * *i-* ⇒ *r-*
         * *i+* ⇒ *r-*
         * *r-* ⇒ *p-*
         * *p-* ⇒ *r-*
 
     * Here are the details:
-        * If no timer is currently associated with the reminder, one will be created. If another timer is *active*, the new timer will be *inactive*, otherwise it will be *running*.
+        * If no timer is currently associated with the reminder, one will be created. If another timer is *active*, the new timer will be *inactive*, otherwise it will be *active* and *paused*.
         * If an *inactive* timer is already associated with the reminder. Its state will be changed to *running*. If another timer is *active*, that timer will be changed to *inactive* and, if *running*, its elapsed time will be incremented by the period it has been *running*.
         * If an *active* timer is already associated with the reminder, its state will be toggled between *paused* and *running*. With a transition from *running* to *paused*, the elapsed time for the timer in increased by the period since the timer's state changed to *running*.
 
       Additionally, if there is an *active* timer, its state, either *r* (running) or *p* (paused), is displayed in the *etm* status bar together with the relevant time period, either the total elapsed time or how long the timer has been paused. If there are *inactive* timers with non-zero elapsed times, the total of such elapsed times will also be reported in the status bar. E.g., this display in the status bar
 
             r:4m + i:13m
 
       would mean that the *active* timer is *running* with 4 minutes of unrecorded elapsed time and that there is an additional 13 minutes of unrecorded elapsed time in *inactive* timers.
+
 * *record used time* with a reminder selected, will:
     * If a timer is not currently associated with the reminder, prompt for a timeperiod and ending time to use in adding a usedtime entry to the reminder.
     * If a timer is currently associated with the reminder, use its elapsed time and the last moment it was running as the defaults in the prompt for a usedtime timeperiod and ending time. If the entry is saved, the elapsed time for the timer will be reset to zero and, additionally, if the timer is currently *running*, its status will be changed to *paused*.
 
-    **Important**: timer data is stored in memory and will be lost if *etm* is stopped. Be sure to record usedtime entries for timers with elapsed times before quitting etm. The status bar will always indicate if there is unrecorded elapsed time.
-
 
 [↺ contents](#contents)
 
 ## Installation {#installation}
 
 
 ### For personal use {#for-personal-use}
 
 The easiest way to install *etm* for personal use is to use *pip*:
 
 	$ python3 -m pip install -U etm-dgraham
 
-This will install *etm* with all the needed python supporting modules. You can then start *etm* with
+(This same command can be used to update *etm* when a new version is released.) This will install *etm* with all the needed python supporting modules. You can then start *etm* with
 
 	$ etm <path to home>
 
+
 See [Home directory](#home-directory) for details about `<path to home>`.
 
-<!--  [![etm: installing etm in a virtual environment](http://img.youtube.com/vi/fEPPG82AH7M/0.jpg)](http://www.youtube.com/watch?v=fEPPG82AH7M "installing etm in a virtual environment") -->
 
 [↺ contents](#contents)
 
-### For use in a virtual environment {#For-use-in-a-virtual-environment}
-
-Setting up a virtual environment for etm is only slightly more complicated. The steps for OS/X or linux are illustrated below. For details see [python-virtual-environments-a-primer](https://www.google.com/url?q=https%3A%2F%2Frealpython.com%2Fpython-virtual-environments-a-primer%2F&sa=D&sntz=1&usg=AFQjCNFh7QpJQ4rPCDjZ1eLrV1BRCCpSmw).
-
-Open a terminal and begin by creating a new directory/folder for the virtual environment, say `etm-pypi`, in your home directory:
-
-        $ mkdir ~/etm-pypi
-        $ cd ~/etm-pypi
-
-Now continue by creating the virtual environment (python >= 3.7.4 is required for etm):
-
-        $ python3 -m venv env
+### For use in an isolated environment {#For-use-in-an-isolated-environment}
 
-After a few seconds you will have an `./env` directory. Now activate the virtual environment:
+Installing etm in an isolated or virtual environment (sandbox) is only slightly more complicated. Begin by using *pip* to install *pipx*:
 
-        $ source env/bin/activate
+    $ python3 -m pip install -U pipx
 
-The prompt will now change to something containing `(env)` to indicate that the virtual environment is active. Updating pip is now recommended:
+Now run:
 
-        (env) $ pip install -U pip
+    $ pipx ensurepath
 
-Note that this invokes `./env/bin/pip`. Once this is finished, use pip to install etm:
+to ensure that directories necessary for *pipx* operation are in your PATH environment variable and finally to install *etm* itself:
 
-        (env) $ pip install -U etm-dgraham
+    $ pipx install etm-dgraham
 
-This will install etm and all its requirements in
+(To upgrade *etm* when a new version becomes available, simply replace "install" in this command with "upgrade".) You can then start *etm* as before with
 
-		./env/lib/python3.x/sitepackages
-
-and will also install an executable called `etm` in `./env/bin`.You can then start etm using
-
-        (env) $ etm <path to home>
+    $ etm <path to home>
 
 Details about `<path to home>` are in [Home directory](#home-directory).
 
 [↺ contents](#contents)
 
 ### For use system wide {#for-use-system-wide}
 
@@ -1341,28 +1400,30 @@
 
 [↺ contents](#contents)
 
 ## Usage {#usage}
 
 ### Terminal size and color scheme {#terminal-size-and-color-scheme}
 
-The suggested terminal size for etm is 60 (columns) by 32 or more (rows). The default color scheme is best with a dark terminal background. A scheme better suited to light backgrounds can be set using `style: light` in `cfg.yaml` in your home directory. Some of the *etm* display may not be visible unless `style` is set correctly for your display.
+The suggested terminal size for etm is 70 (columns) by 32 or more (rows). The default color scheme is best with a dark terminal background. A scheme better suited to light backgrounds can be set using `style: light` in `cfg.yaml` in your home directory. Some of the *etm* display may not be visible unless `style` is set correctly for your display.
 
 The size of the terminal is used when *etm* starts to set various display options so changing the terminal size, especially reducing the width, is best avoided once *etm* is running.
 
 [↺ contents](#contents)
 
 ### Home directory {#home-directory}
 
 Before you start etm, think about where you would like to keep your personal data and configuration files. This will be your etm *home* directory. The default is to use whatever directory you're in when you start _etm_ as your _etm_ home directory. If you start _etm_ in your virtual environment directory then the default will be to use that as your home directory as well. If this is not what you want, you can just give the path for whatever directory you would like to use when you start _etm_.
 
 	$ etm <path to home>
+
 Finally, if there is an environmental variable, `ETMHOME`, set to this path then you can just enter
 
 	$ etm
+
 and etm will use `ETMHOME` as its home directory.
 
 Home directory considerations:
 
 * If more than one person will be using etm on the same computer, you might want to have different *home* directories for each user.
 * If you want to use etm on more than one computer and use Dropbox, you might want to use `~/Dropbox/etm` to have access on each of your computers.
 * If you want to separate personal and professional reminders, you could use different _home_ directories for each. You can run two instances of _etm_ simultaneously, one for each directory, and have access to both at the same time.
@@ -1379,24 +1440,80 @@
 Here `cfg.yaml` is your user configuration file and `db.json` contains all your etm reminders. The folders `backups/` contains the 7 most recent daily backups of your `db.json` and `cfg.yaml` files. The folder `logs` contains the current `etm.log` file and the 7 most recent daily backups. Note that backup files are only created when the relevant file has been modified since the last backup.
 
 The file `cfg.yaml` can be edited and the options are documented in the file.
 See [configuration](#configuration) for details.
 
 [↺ contents](#contents)
 
+### Timers {#timers}
+
+For tracking time spent, *etm* supports the use of one or more timers. Each timer is associated with a particular reminder and, if a timer is recorded, a used time entry will be added to the associated reminder using this format:
+
+        @u <time spent>: <datetime recorded>
+
+The timer itself records seconds, but the used time entry for `<time spent>` depends upon the `usedtime_minutes` setting in `cfg.yaml` as follows:
+
+- 0: time is recorded in seconds after rounding to the nearest second
+- 1: time is recorded in minutes after rounding off to the nearest minute, e.g., 1m29s => 1m; 1m30s => 2m
+- 6: time is rounded up to the next one-tenth of an hour for reporting but recorded in minutes
+- 12: time is rounded up to the next two-tenths of an hour for reporting but recorded in minutes
+- 30: time is rounded up to the next half hour for reporting but recorded in minutes
+- 60: time is rounded up to the next hour for reporting but recorded in minutes
+
+The [Used Time Views](#used-time-views) show aggregations of these reported times by month and index entry. Any rounding up is done before aggregating.
+
+Used time entries can be recorded directly by editing the relevant reminder and adding one or more `@u` entries. It is also possible to use *etm* to create timers *attached* to particular reminders and control them with hotkeys.
+
+- T: with a reminder selected
+    - If a timer is not already associated with this reminder, then create a new timer and associate it with this reminder
+        - if another timer is active, make this timer inactive
+        - otherwise make this timer active and paused
+    - If a timer is already associated with this reminder
+        - if the timer is inactive, make it active and running
+        - otherwise toggle the state of the timer between paused and running
+- TR: if a reminder is selected with an associated timer
+    - open a dialog to record a used time entry with the current value of the timer and the current datetime
+    - if, after possible editing, recording is confirmed then add the used time entry and delete the timer
+- TD: if a reminder is selected with an associated timer
+    - open a dialog to confirm deleting the timer without recording the used time
+    - if deletion is confirmed then delete the timer
+- TT: if there is an active timer
+    - toggle the paused/running state for the active timer. Note that the reminder associated with the active timer *need not be selected*.
+    - Note that if there are one or more timers, *exactly one of them will be the active timer*, i.e., either running or paused. The others, if any, will be inactive.
+
+[Timer View](#timer-view), bound to `m`, provides a convenient way of manipulating multiple timers. It lists each existing timer with the active timer first and followed by the other timers in the order of most recently active. Pausing/running the active timer can be done from any view by pressing `TT`. To switch to another timer, change to timer view, press `TT` if necessary to pause the active timer, select the timer you want to start and press 'T' to change its state from 'inactive' to 'running'. It will move to the top of the list and the other timers will move down by one row.
+
+When there are one or more timers, their status is always displayed in the status bar. E.g., `r:6.3m + i:1h3.2` would mean that the active timer is running with 6.3m of elapsed time and there are other, inactive timers with a total of 1h3.2m of elapsed time.
+
+[↺ contents](#contents)
+
+### *lorem* examples {#loremexamples}
+
+If you are new to *etm*, you might find it very useful to install the *lorem* examples. If you press `F5`, enter 'lorem' at the prompt and press `return`, *etm* will generate a series of reminders all of which are tagged 'lorem'. These fall within a three month period including the month in which they were created as well as the previous and subsequent months. The examples are designed to illustrate nearly all of the etm views and features. You can play around with the examples as long as you wish and then remove them all at once by pressing `q` to open query view, entering the query 'any t lorem \| remove' and pressing `return`.
+
+These examples are named for and depend upon the python package *lorem* that can generate random words, phrases, sentences and paragraphs in 'lorem ipsum' text. E.g., "Lorem ipsum dolor sit amet, consectetur adipiscing elit ...". This is "a placeholder text commonly used to demonstrate the visual form of a document or a typeface without relying on meaningful content."
+
+[↺ contents](#contents)
+
 ### Using etm+ {#etmplus}
 
 An added bonus of setting `ETMHOME` to the path of your *home* directory is the possibility of using the `etm+` shortcut for creating reminders. E.g., entering
 
 	$ etm+ '* lunch with Peter @s fri 12p'
 would append the line `* lunch with Peter @s fri 12p` to the file `inbasket.text`in `ETMHOME`, creating the file if necessary. `etm+` also accepts input piped to it so that
 
 	$ echo '* lunch with Peter @s fri 12p' | etm+
 would produce exactly the same result.
 
+Finally, if `{T}` is included, it will be replaced with a time stamp corresponding to the moment the script was invoked. E.g.,
+
+	$ echo '% got the test result at {T}' | etm+
+
+would append something like `% got the test result at 2022-12-07 9:13:55 EST`.
+
 Important
 : The single quotes are necessary to keep the shell from expanding the "*" into the names of all the files in the current working directory and other such mischief.
 
 *etm* checks once every minute for the presence of a file named `inbasket.text`in `ETMHOME` and, if found, will display an inbasket character, ⓘ , at the right end of its status bar reminding you that inbasket items are available for importing. Just press F5 in etm to import the reminders from this file and, on successful completion, automatically remove the file.
 
 Note finally that `etm+` will accept quick notes which are not themselves valid etm reminders such as
 
@@ -1447,49 +1564,48 @@
 
 ### event {#event}
 
 Type character: **\***
 
 An event is something that happens at a particular date or datetime without any action from the user. Christmas, for example, is an event that happens whether or not the user does anything about it.
 
-- The `@s` entry is required and can be specified either as a date or as a datetime. It is interpreted as the starting date or datetime of the event.
+- The `@s` entry is required and can be specified either as a date or as a datetime. It is interpreted as the scheduled date or datetime at which the event begins.
 - If `@s` is a date, the event is regarded as an *occasion* or *all-day* event. Such occasions are displayed first on the relevant date.
 - If `@s` is a datetime, an `@e` entry is allowed and is interpreted as the extent or duration of the event - the end of the event is then given implicitly by starting datetime plus the extent and this period is treated as busy time.
 
 Corresponds to VEVENT in the vcalendar specification.
 
 [↺ contents](#contents)
 
 ### task {#task}
 
 Type character: **-**
 
 A task is something that requires action from the user and lasts, so to speak, until the task is completed and marked finished. Filing a tax return, for example, is a task.
 
-- The `@s` entry is optional and, if given, is interpreted as the date or datetime at which the task is due.
-    - Tasks with an `@s` datetime entry are regarded as past due after the datetime and are displayed in *Agenda View* on the relevant date according to the starting time.
+- The `@s` entry is optional and, if given, is interpreted as the date or datetime at which the task is scheduled to be completed.
+    - Tasks with an `@s` datetime entry are regarded as past due after the datetime and are displayed in *Agenda View* on the relevant date according to the scheduled time.
     - Tasks with `@s` date entry are regarded as past due after the due date and are displayed in *Agenda View* on the due date after all items with datetimes.
     - Tasks that are past due are also displayed in *Agenda View* on the current date using the type character `<` with an indication of the number of days that the task is past due.
 - Tasks without an `@s` entry are to be completed when possible and are sometimes called *todos*. They are regarded as *next* items in the *Getting Things Done* terminology and are displayed in *Do Next* view grouped by @l (location/context).
-- Tasks with an `@r` (repeat) entry can have an `@o` (overdue) setting.
-	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. mortage payments to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. Whenever a payment is sent, it applies to the oldest, past due one. This is the default when no `@o` entry is given.
-    - `@o p`: preserve. When an instance becomes past due, a new, non-repeating copy is created with the past due datetime as the `@s` entry and with an `@k` containing the document_id of the original item. Suppose, for example, that minutes are kept for a weekly meeting to be sent to the attendees after each meeting. Creating a task that repeats weekly with `@o p` recognizes the distinction between sending the minutes for `22/10/8` and `22/10/15` and, should both become past due, permits finishing the tasks in any convenient order.
-	- `@o r`: reset. Whenever completed, the next instance is due at the first datetime from the recurrance rule that falls after the current datetime. E.g., getting a haircut every 14 days is due 14 days after the last haircut. With this option, at most one instance can be past due.
-	- `@o s`: skip. Like 'keep' and 'reset' combined with the addition that past due instances are ignored. E.g., taking out the trash every Monday morning for pickup is due every Monday morning but, if a Monday passes without taking out the trash, the instance is better regarded as irrelevant than past due. With this option, an instance can never be past due.
+- Tasks with an `@r` (repeat) or an `@+` entry can have an `@o` (overdue) setting.
+	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. minutes from a monthly meeting to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. By default, a completion applies to the oldest, past due one, though other instances can be selected. This is the default when no `@o` entry is given.
+	- `@o r`: reset. Whenever completed, the next instance is due at the first datetime that falls after the current datetime. E.g., getting a haircut every 14 days is due 14 days after the last haircut. With this option, at most one instance can be past due.
+	- `@o s`: skip. Like 'keep' with the addition that past due instances are ignored. E.g., taking out the trash every Monday morning for pickup is due every Monday morning but, if a Monday passes without taking out the trash, the instance is better regarded as irrelevant than past due. With this option, an instance can never be past due.
 
 	    Furthermore, if the options setting `limit_skip_display` were true, then only the first instance of such a task would be displayed in agenda view. E.g., with the `limit_skip_display` setting true, then for the task
 
 			- meds @s +0d @r d &h 8,14,20 @o s
 
 		agenda view at 10am today would only display the first, 2pm (14h) instance of this task. If, on the other hand, this setting were false, then agenda view would display not only the 2pm instance but also the 8pm (20h) instances and all three instances on every future date.
 
 - Jobs
     - Tasks, both with and without @s entries can have component jobs using @j entries.
-    - For tasks with an @s entry, jobs can have an &s entry to set the due date/datetime for the job. It is entered as a timeperiod relative to  the starting datetime (+ before or - after) for the task. Zero minutes is the default when &s is not entered.
-    - For tasks with an @s entry, jobs can also have &a, alert, and &b, beginning soon, notices. The entry for &a is given as a time period relative to &s (+ before or - after) and the entry for &b is a positive integer number of days before the starting date/time to begin displaying "beginning soon" notices. The entry for @s in the task becomes the default for &s in each job.  E.g., with
+    - For tasks with an @s entry, jobs can have an &s entry to set the due date/datetime for the job. It is entered as a timeperiod relative to  the scheduled datetime (+ before or - after) for the task. Zero minutes is the default when &s is not entered.
+    - For tasks with an @s entry, jobs can also have &a, alert, and &b, beginning soon, notices. The entry for &a is given as a time period relative to &s (+ before or - after) and the entry for &b is a positive integer number of days before the scheduled date/time to begin displaying "beginning soon" notices. The entry for @s in the task becomes the default for &s in each job.  E.g., with
 
             - beginning soon example @s 1/30/2018
                 @j job A &s 5d &b 10
                 @j job B &b 5
 
         Beginning soon notices would begin on Jan 15 for job A (due Jan 25) and on January 25 for job B (due Jan 30).
     - Prerequisites
@@ -1557,15 +1673,15 @@
 
 [↺ contents](#contents)
 
 ### inbox {#inbox}
 
 Type character: **!**
 
-An inbox item can be regarded as a task that is always due on the current date. E.g., you have created an event to remind you of a lunch meeting but need to confirm the time. Just record it using **!** instead of **\*** and the entry  will appear highlighted in the agenda view on the current date until you confirm the starting time.
+An inbox item can be regarded as a task that is always due on the current date. E.g., you have created an event to remind you of a lunch meeting but need to confirm the time. Just record it using **!** instead of **\*** and the entry  will appear highlighted in the agenda view on the current date until you confirm the scheduled time.
 
 Corresponds to VTODO in the vcalendar specification.
 
 [↺ contents](#contents)
 
 ### status {#status}
 
@@ -1573,15 +1689,15 @@
 
 [↺ contents](#contents)
 
 #### beginning soon {#beginning-soon}
 
 Type character: **>**
 
-For unfinished tasks and other items with `@b` entries, when the starting date given by `@s` is within `@b` days of the current date, a warning that the item is beginning soon appears on the current date together with the item summary and the number of days remaining until the current date.
+For unfinished tasks and other items with `@b` entries, when the scheduled date given by `@s` is within `@b` days of the current date, a warning that the item is beginning soon appears on the current date together with the item summary and the number of days remaining until the current date.
 
 [↺ contents](#contents)
 
 #### past due {#past-due}
 
 Type character: **<**
 
@@ -1625,15 +1741,15 @@
 @ keys
 </h3>
 
 `@` followed by a character from the list below and a value appropriate to the key is used to apply attributes to an item. E.g.,
 
             @s mon 9a
 
-would specify the the starting datetime for the item is 9am on the Monday following the current date.
+would specify the the scheduled datetime for the item is 9am on the Monday following the current date.
 
 *  @+: include. list of datetimes to include
 *  @-: exclude. list of datetimes to exclude
 *  @a*: alert. list of + (before) or - (after) periods: list of commands
 *  @b: beginby. integer (number of days before)
 *  @c: calendar. string
 *  @d: description. string
@@ -1647,30 +1763,30 @@
 *  @l: location (aka context). forward slash delimited string. E.g., home/maintenance
 *  @m: mask. string stored in obfuscated form
 *  @n*: attendee. string using "[name:] address" format. If "address" begins with exactly 10 digits followed by an "@" it is treated as a mobile phone number. Otherwise it is treated as an email address. The optional "name:" can be used to facilitate autocompletion.
 *  @o: overdue. character from (r) restart, (s) skip, (k) keep, (p) preserve
 *  @p: priority. integer from 0 (none), 1 (low), 2 (normal), 3 (high), 4 (urgent)
 *  @r*: repetition frequency, a character from (y)early, (m)onthly, (w)eekly,
   (d)aily, (h)ourly or mi(n)utely, optionally followed by repetition &key entries
-*  @s: start. date or datetime
+*  @s: scheduled date or datetime
 *  @t*: tag. string
 *  @u*: usedtime. string using "timeperiod spent: ending datetime" format
 *  @w: wrap. A pair of before and after timeperiods to extend the busy period for an event, e.g., for travel time to and/or from the location of the event. Use `0m` as one of the timeperiods to avoid a wrap in that direction.
 *  @x*: expansion. string
 *  @z: timezone. string. A timezone specification, such as 'US/Eastern' or 'Europe/Paris' for aware datetimes or 'float', to indicate a naive or floating datetime. Datetime entries in the item are interpreted as belonging to the specified timezone when the entry is saved. The current timezone is the default when @z is not specified. Aware datetimes are converted to UTC (coordinated universal time) when stored and the @z entry, now irrelevant, is discarded.
 
 <h3 id="ampkeys">
 & keys
 </h3>
 
 & followed by a character from one of the lists below. These keys are only used with @j (job) and @r (repetition) entries.
 
 For use with @j:
 
-*  &s: start/due: period relative to @s entry (default 0m)
+*  &s: scheduled: period relative to @s entry (default 0m) at which job is scheduled to be completed
 *  &a: alert: list of + (before) or - (after) periods relative to &s: list of cmd names from the users configuration file
 *  &b: beginby. integer number of days before &s
 *  &d: description. string
 *  &e: extent. period
 *  &f: finished. datetime
 *  &l: location/context. string
 *  &m: masked. string stored in obfuscated form
@@ -1698,16 +1814,16 @@
 ## Notes {#notes}
 
 ### notices {#notices}
 
 * A link character, 'g', is appended to the *flags* column of any reminder with an `@g` goto link. Press `^g` with such a reminder selected to have the operating system open the link using the default application if the link can be interpreted as a file path or a url. E.g. if the link is a URL, then it would be opened using the default browser. If link can be interpreted as a shell command followed by arguments, then the command would be executed with the arguments.
 * An in-basket character, ⓘ , is appended to the right end of the status bar when a file named 'inbasket.text' is found in the etm root directory. This file should contain lines containing etm reminder entries - one on each line. It can be imported using the import file command bound to F5.
 * An update available character, 𝕦, is appended to the right end of the status bar when checking for updates is enabled and a later version of etm is available. Details for enabling checking for updates are in [configuration](#configuration).
-* Alerts and beginbys can be added to any reminder with an `@s` start date/time entry. Alerts require a datetime in `@s`; beginbys also allow a date in `@s`.
-* A beginby is specified by adding `@b n` to a reminder where `n` is a positive integer and is interpreted as a number of days. A reminder with such an entry will be displayed in *agenda view* on the current date provided that the current date is no more than `n` days before the start date/time of the reminder. Such a warning will appear n days before, n-1 days before and so forth until 1 day before the starting date/time of the reminder. The warning displays the type character `>`, the summary of the reminder and the number of days remaining.
+* Alerts and beginbys can be added to any reminder with an `@s` scheduled date/time entry. Alerts require a datetime in `@s`; beginbys also allow a date in `@s`.
+* A beginby is specified by adding `@b n` to a reminder where `n` is a positive integer and is interpreted as a number of days. A reminder with such an entry will be displayed in *agenda view* on the current date provided that the current date is no more than `n` days before the scheduled date/time of the reminder. Such a warning will appear n days before, n-1 days before and so forth until 1 day before the scheduled date/time of the reminder. The warning displays the type character `>`, the summary of the reminder and the number of days remaining.
 * An alert is specified by adding `@a <list of time periods>: <list of commands>` to a reminder. The time periods must be given in the usual etm format, e.g., `1h13m` for one hour and 13 minutes. The commands are single alphabetic characters, e.g., `a`, `b` and such. The commands used must either be `e` (email) or `t` (text) or be specified in the `alerts` section of the `cfg.yaml` file in your etm home directory. See [configuration](#configuration) for details about this file. Basically, it associates a command, such as `v` with a shell command to be invoked when an alert that includes `v` is triggered. E.g., the alert
 
 			@a 20m: v
 
     would be triggered 20 minutes before the datetime specified in the reminder's `@s` entry and at that time the shell command associated with `v` would be invoked. Both positive (before) and negative (after) time periods can be used. Thus this entry
 
 			@a 1d, -1h: v, w
@@ -1857,47 +1973,51 @@
 ### configuration {#configuration}
 
 Configuration settings for *etm* are specified in the file `cfg.yaml` located in your etm *home directory*. See [installation](#installation) for the location of this directory. When *etm* is running, you can press `F8` to open this configuration file using your system default editor for *yaml* (text) files. Note that any changes you make will not become effective until you stop and restart *etm*.
 
 Here are the options with their default values from that file. The lines beginning with `#` are comments that describe the settings.
 
     #### begin cfg.yaml ####
-	version: 4.9.1
-	# The current version of etm and this file. DO NOT EDIT. This is
-	# automatically updated when a new version of etm is installed.
+    etmversion: 4.11.18
+    # The current version of etm and this file. DO NOT EDIT. This is
+    # automatically updated when a new version of etm is installed.
 
     ampm: true
     # true or false. Use AM/PM format for datetimes if true else
-    # use 24 hour format.
+    # use 24 hour format. See also the show_minutes setting.
+
+    show_minutes: false
+    # true or false. If true show ":00" in agenda and forthcoming views
+    # when displaying times with zero minutes else suppress zero minutes
+    # from being displayed. E.g., "9:00-10:30" if true else "9-10:30".
+    # When ampm if false and show_minutes is true, hours will be displayed
+    # with leading zeros applicable.
 
-    dayfirst:  true
+    dayfirst:  false
     yearfirst: true
-    # true or false. Whenever an ambiguous date is parsed, dayfirst
+    # each true or false. Whenever an ambiguous date is parsed, dayfirst
     # and yearfirst parameters control how the information is processed
     # using this precedence:
-    #
-    #   If dayfirst is False and yearfirst is False:
-    #       MM-DD-YY
-    #       DD-MM-YY
-    #       YY-MM-DD
-    #
-    #   If dayfirst is True and yearfirst is False:
-    #       DD-MM-YY
-    #       MM-DD-YY
-    #       YY-MM-DD
-    #
-    #   If dayfirst is False and yearfirst is True:
-    #       YY-MM-DD
-    #       MM-DD-YY
-    #       DD-MM-YY
-    #
-    #   If dayfirst is True and yearfirst is True:
-    #       YY-MM-DD
-    #       DD-MM-YY
-    #       MM-DD-YY
+    # yearfirst: true
+    # 	dayfirst: true  => YDM
+    #   dayfirst: false => YMD
+    # yearfirst: false
+    # 	dayfirst: true  => DMY
+    #   dayfirst: false => MDY
+    # E.g., with both true, 3/4/5 would be interpreted as May 4, 2003.
+    # When possible, dates will also be displayed respecting these settings.
+    # I.e., the year will generally be displayed first when yearfirst is
+    # true and last otherwise. Similarly, the day will generally be displayed
+    # before the month when dayfirst is true and after the month otherwise.
+
+    beginbusy: 7
+    # non-negative integer. The number of hours after midnight to begin the
+    # busy view display of busy times for each day. The display continues
+    # for 14 hours after the begin_busy hour. E.g. with 'begin_busy: 7' the
+    # display would show busy times from 7am (7h) until 9pm (21h).
 
     updates_interval: 0
     # non-negative integer. If positive,  automatically check for updates
     # every 'updates_interval' minutes. If zero, do not automatically
     # check for updates. When enabled, a blackboard u symbol, 𝕦, will be
     # displayed at the right end of status bar when an update is available
     # or a question mark when the check cannot be completed as, for
@@ -1908,34 +2028,36 @@
     # for English (United States), "fr_FR" for French (France) and so
     # forth. Google "python locale abbreviatons" for a complete list."
 
     vi_mode: false
     # true or false. Use vi keybindings for editing if true else use emacs
     # style keybindings.
 
-    secret: KFI9R2AAaw
+    secret: HIr13FiYj3
     # string to use as the secret_key for @m masked entries. E.g.
     # 'X6i2SGWu6m'. In etm versions after 4.0.21, the default string is
     # randomly generated when this file is created or when the secret
     # value is removed and etm is restarted. WARNING: if this key is
     # changed, any @m entries that were made before the change will be
     # unreadable after the change.
 
     omit_extent:
     # A list of calendar names. Events with @c entries belonging to this
     # list will only have their starting times displayed in agenda view
     # and will neither appear nor cause conflicts in busy view.
 
-    keep_current: 0
-    # non-negative integer. If positive, the agenda for that integer
-    # number of weeks starting with the current week will be written to
-    # "current.txt" in your etm home directory and updated when necessary.
-    # You could, for example, create a link to this file in a pCloud or
-    # DropBox folder and have access to your current schedule on your
-    # mobile device.
+    keep_current: [0, 47]
+    # A list of two, non-negative integers for "weeks" and "width". If
+    # weeks is positive, the agenda for that integer number of weeks
+    # starting with the current week will be written to "current.txt" in
+    # your etm home directory and updated when necessary. The format will
+    # be scaled to fit "width". A width of 50, e.g, fits an iPhone display
+    # in portrait mode. You could, for example, create a link to
+    # "current.txt" in a pCloud or GoogleDrive folder and always have access
+    # to your current agenda on your mobile device.
 
     keep_next: false
     # true or false. If true, the 'do next' view will be written to
     # "next.txt" in your etm home directory. As with "current.txt", a link
     # to this file could be created in a pCloud or DropBox folder for
     # access from your mobile device.
 
@@ -1965,34 +2087,56 @@
     # current time.
 
     connecting_dots: false
     # true or false. If true, display dots connecting the item summary and
     # the right-hand details columns in tree views.
 
     usedtime_minutes: 1
-    # 1, 6, 12, 30 or 60. Round used times up to the nearest
-    # usedtime_minutes in used time views. With 1, no rounding is done and
-    # times are reported as hours and minutes. Otherwise, the prescribed
-    # rounding is done and times are reported as floating point hours.
-    # Note that each "@u" timeperiod is rounded before aggregation.
+    # 0, 1, 6, 12, 30 or 60. Round up used times. With 0, no rounding is done
+    # and times are reported in hours, minutes and seconds. With 1, after
+    # rounding up to the nearest minute, times are reported as hours and minutes.
+    # Otherwise, rounding is up to the nearest integer multiple of
+    # usedtime_minutes and times are reported as floating point hours. E.g.,
+    # with usedtime_minutes = 6, 1 minute would be rounded up to 6 minutes and
+    # reported as 0.1 hours. Similarly 13 minutes would be rounded up to 18
+    # minutes and reported as 0.3 hours. Note that when rounding is specified,
+    # each "@u" timeperiod is rounded before aggregation.
+
+    usedtime_hours: 6
+    # 0, 1, 2, ..., 24. The daily goal for used time. This is used in engaged
+    # view to control the display of the daily used time bars. The goal is to
+    # to maximize the granularity of the bar when displaying this number of hours
+    # in the space allowed by the terminal width.
+
+    journal_name: daily
+    # Journal items with this index entry and with an @s entry will have the
+    # year and month appended to the index. E.g., with the setting
+    #   journal_name: daily
+    # this journal entry
+    #   % visited Yellowstone @s 22/6/24 @i daily
+    # would be displayed in journal view as if the index entry were
+    #   @i daily/2022/ 6
+    # thus organizing such entries by the year and month of their scheduled dates.
+    # Within each month, entries will be also ordered by the month day.
 
     alerts:
     # A dictionary with single-character, "alert" keys and corresponding
     # "system command" values. Note that characters "t" (text message) and
     # "e" (email) are already used.  The "system command" string should be
     # a comand with any applicable arguments that could be run in a
     # terminal. Properties of the item triggering the alert can be
     # included in the command arguments using the syntax {prop}, e.g.,
     # {summary} in the command string would be replaced by the summary of
-    # the item. Similarly {start} by the starting time, {when} by the time
-    # remaining until the starting time, {location} by the @l entry and
-    # {description} by the @d entry. E.g., If the event "* sales meeting
-    # @s 2019-02-12 3p" triggered an alert 30 minutes before the starting
-    # time the string "{summary} {when}" would expand to "sales meeting in
-    # 30 minutes". E.g. on my macbook
+    # the item. Similarly {start} by the starting datetime, {time} by the
+    # starting time (omits the date for the current date), {when} by the time
+    # remaining until the starting datetime, {now} by the current time,
+    # {location} by the @l entry and {description} by the @d entry. E.g., If
+    # the event "* sales meeting @s 2019-02-12 3p" triggered an alert 30 minutes
+    # before the starting time the string "{summary} {when}" would expand to
+    # "sales meeting in 30 minutes". E.g. on my macbook
     #
     #    alerts:
     #        v:   /usr/bin/say -v "Alex" "{summary}, {when}"
     #        ...
     #
     # would make the alert 'v' use the builtin text to speech sytem
     # to speak the item's summary followed by a slight pause
@@ -2009,18 +2153,18 @@
     #        ...
     #
     # then when "@x tennis" is entered the popup completions for
     # "@x tennis" would offer replacement by the corresponding
     # "@e 1h30m @a 30m: d @i personal:exercise".
 
     sms:
-      body: "{location} {when}"
-      from:
-      server:
-      pw:
+    body: '{location} {when}'
+    from:
+    server:
+    pw:
     # Settings to send "t" (sms text message) alerts to the
     # list of phone numbers from the item's @n attendee
     # entries using the item's summary and the body as specified
     # in the template below as the message. E.g., suppose you
     # have a gmail account with email address "who457@gmail.com"
     # and want to text alerts to Verizon moble phone (123)
     # 456-7890. Then your sms entries should be
@@ -2033,19 +2177,19 @@
     # gateway for Verizon. Other common mms gateways are
     #     AT&T:     @mms.att.net
     #     Sprint:   @pm.sprint.com
     #     T-Mobile: @tmomail.net
     # Note. Google "mms gateway listing" for other alternatives.
 
     smtp:
-      body: "{location} {when}\n{description}"
-      from:
-      server:
-      id:
-      pw:
+    body: '{location} {when}\n{description}'
+    from:
+    server:
+    id:
+    pw:
     # Settings to send "e" (email message) alerts to the list of email
     # addresses from the item's @n attendee entries using the item's
     # summary as the subject and body as the message. E.g., if you have a
     # gmail account with email address "whatever457@gmail.com", then your
     # entries should be
     #     from: whatever457@gmail.com
     #     id: whatever457
@@ -2070,14 +2214,18 @@
     # values. Each "query" must be one that could be entered as the
     # command in query view. Keys can be any short string other than
     # 'a', 'u', 'c' or 'l' which are already in use.
     # queries:
     #    td: m l -q equals itemtype - and ~exists f
     #    mi: exists u and ~exists i
     #    arch: a exists itemtype
+    #    find: includes summary d {}
+    # The latter would allow you to enter, e.g., `find waldo` and have
+    # it expand to `includes summary d waldo` and thus locate all
+    # reminders with `waldo` either in the summary or d (the description).
 
     style: dark
     # dark or light. Set the defaults for dark or light terminal
     # backgounds. Some output may not be visible unless this is set
     # correctly for your display.
 
     type_colors:
@@ -2092,30 +2240,35 @@
     #  event           'LimeGreen',        'DarkGreen',
     #  finished        'DarkGrey',         'LightSlateGrey',
     #  inbox           'OrangeRed',        'MediumVioletRed',
     #  journal         'GoldenRod',        'Brown',
     #  pastdue         'LightSalmon',      'Red',
     #  plain           'Ivory',            'Black',
     #  today           'Ivory bold',       'Black bold',
+    #  used            'Khaki',            'DodgerBlue',
     #  waiting         'SlateGrey',        'DarkSlateBlue',
-	#  wrap            'SlateGrey',        'DarkSlateBlue',
-    #
+    #  wrap            'ForestGreen',      'LightGrey',
+    #  running         'OrangeRed',        'Gold',
+    #  paused          'MediumVioletRed',   'DarkViolet',
     # Explanations for the key names:
     #     available:    available task/job reminders
     #     begin:        begin by warnings
     #     event:        event reminders
     #     finished:     finished task/job reminders
     #     inbox:        inbox reminders
     #     journal:      journal reminders
     #     pastdue:      pasdue task warnings
     #     plain:        headings such as outline branches
     #     today:        the current and following agenda date headings
+    #     used:         used time rows in engaged and used time views
     #     waiting:      waiting job reminders (jobs with unfinished prereqs)
-	#     wrap:         before and after rows for events in agenda view with
-	#                   @w entries
+    #     wrap:         before and after rows for events in agenda view with
+    #                   @w entries
+    #     running:      status bar color for 'r', running timer
+    #     paused:       status bar color for 'p', paused timer
     #
     # E.g., with style 'dark', the default color for 'available' is
     # 'LightSkyBlue'. This entry
     #   colors:
     #       available: CornFlowerBlue
     # would change the 'available' color to 'CornflowerBlue' while leaving
     # the other 'dark' colors unchanged.
@@ -2131,15 +2284,15 @@
     #    [background, foreground, attribute]
     # components. background and foreground can either be named colors,
     # hex colors, or ''. Attribute is an optional font attribute such
     # as 'bold' which must, of course, be supported by the font used in
     # your terminal. The default settings are determined by the 'dark'
     # or 'light' style setting as follows:
     #
-    #    key                           dark                        light
+    #    key                       dark default                  light default
     # -------------------    -----------------------------  -----------------------------
     # ask:                    [grey2, Lime, bold]           [Cornsilk, Lime, bold]
     # button.focused:         [DarkGreen, White]            [DarkGreen, White]
     # details:                [, Ivory]                     [, Black]
     # dialog shadow:          [#444444, ]                   [#444444, ]
     # dialog:                 [DarkSlateGrey, White]        [DimGrey, White]
     # dialog-entry:           [White, Black]                [White, Black]
@@ -2165,20 +2318,23 @@
     #
     # Note that 'grey1' (#396060) and 'grey2' (#1d3030) are colors named
     # within etm itself. They are, respectively, one shade lighter and two
     # shades darker than DarkSlateGrey.
     #
     # Any of the style attributes above can be modified. E.g., with style
     # 'dark', the default for 'text-area' is [grey2, Ivory]. This entry
-    #   style_modifications:
+    #   window_colors:
     #       text-area: [Black, White]
     # would change the 'text-area' setting to 'Black' as the background color
     # and 'White' as the foreground color while leaving the other style settings
     # unchanged.
-	#### end cfg.yaml ####
+    #### end cfg.yaml ####
+
+
+See [Saved Queries](#saved-queries) for more information about queries that allow for replaceable parameters.
 
 Note that in the 'dictionary' entries above, the components must be indented (using 2 spaces not tabs). E.g., the illustrative alert entry would be:
 
 	alerts:
 		v: /usr/bin/say -v "Alex" "{summary}, {when}"
 
 
@@ -2225,8 +2381,8 @@
 
 Consider the entry `2019-12-23` for `@s`. To *etm* this is a pendulum date object. When *etm* stores this record, *TinyDB* recognizes that this attribute is a pendulum date object and encodes/serializes it as the string `"{D}:20191223"`. When *etm* retrieves this record from storage, *TinyDB* recognizes from the `{D}` that it is to be decoded and returned as a pendulum date object. All this is completely transparent - *etm* gives a date object to *TinyDB* which stores it as a string and when *etm* wants it back, *TinyDB* deserializes it and returns it as a date object.
 
 As another example, When the reminder is created by *etm* the `created` timestamp is handed to *TinyDB* as an aware pendulum datetime object with US/Eastern as the timezone. *TinyDB* recognizes this and, because it is an aware datetime, first converts it to Universal time and then encodes/serializes it as `"{T}:20191221T1526A"`. The `{T}` indicates that it is a datetime object and the appended `A` indicates that it is aware and thus has been converted to Universal time. When *etm* retrieves this record, *TinyDB* recognizes from the `{T}` and the `A` that this is an aware datetime object, decodes it as an aware datetime object and, because it is aware, converts it from Universal time to whatever the current local timezone happens to be before returning it. Had this been a naive datetime, an `N` would have been appended to the serialization and no conversion would have been done either way.
 
 These **date** and **datetime** serializations are extensions of *TinyDB* provided by *etm*. Three further extensions are also provided: **interval** for *pendulum duration* objects using the tag `{I}`, **weekday** for  *dateutil* weekday objects using the tag `{W}` and **mask** using the tag `{M}` for encoding/serializing *etm* strings in a masked or obfuscated manner.
 
-[↺ contents](#contents)
+[↺ contents](#contents)
```

### Comparing `etm-dgraham-4.9.7/bump.py` & `etm-dgraham-5.0.3/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/docs/index_konnections.md` & `etm-dgraham-5.0.3/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/docs/index_usedtime.md` & `etm-dgraham-5.0.3/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/docs/multiple_timers.md` & `etm-dgraham-5.0.3/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/etm/data.py` & `etm-dgraham-5.0.3/etm/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,14 +55,70 @@
         """
         if s[-1] == 'A':
             return pendulum.from_format(s[:-1], 'YYYYMMDDTHHmm', 'UTC').in_timezone('local')
         else:
             return pendulum.from_format(s[:-1], 'YYYYMMDDTHHmm').naive().in_timezone('local')
 
 
+class PendulumPeriodSerializer(Serializer):
+    """
+    This class handles both aware and 'factory' pendulum objects.
+
+    Encoding: If obj.tzinfo.abbrev is '-00' (tz=Factory), it is interpreted as naive, serialized without conversion and an 'N' is appended. Otherwise it is interpreted as aware, converted to UTC and an 'A' is appended.
+    Decoding: If the serialization ends with 'A', the pendulum object is treated as 'UTC' and converted to localtime. Otherwise, the object is treated as 'Factory' and no conversion is performed.
+
+    This serialization discards both seconds and microseconds but preserves hours and minutes.
+
+    """
+
+    OBJ_CLASS = pendulum.Period
+
+    def encode_datetime(self, obj):
+        if obj.format('Z') == '':
+            return obj.format('YYYYMMDDTHHmm[N]')
+        else:
+            return obj.in_tz('UTC').format('YYYYMMDDTHHmm[A]')
+
+    def decode_datetime(self, s):
+        if s[-1] == 'A':
+            return pendulum.from_format(s[:-1], 'YYYYMMDDTHHmm', 'UTC').in_timezone('local')
+        else:
+            return pendulum.from_format(s[:-1], 'YYYYMMDDTHHmm').naive().in_timezone('local')
+
+
+    def encode(self, obj):
+        """
+        Serialize naive objects (Z == '') without conversion but with 'N' for 'Naive' appended. Convert aware datetime objects to UTC and then serialize them with 'A' for 'Aware' appended.
+        >>> ps = PendulumPeriodSerializer()
+        >>> ps.encode(pendulum.period(pendulum.datetime(2018,7,30,10,45).naive(), pendulum.datetime(2018,7,25,10,27).naive()))
+        '20180730T1045N -> 20180725T1027N'
+        >>> ps.encode(pendulum.period(pendulum.datetime(2018,7,30,10,45,tz='US/Eastern'), pendulum.datetime(2018,7,25,10,27,tz='US/Pacific')))
+        '20180730T1445A -> 20180725T1727A'
+        """
+        start_fmt = self.encode_datetime(obj.start)
+        end_fmt = self.encode_datetime(obj.end)
+        return f"{start_fmt} -> {end_fmt}"
+
+
+    def decode(self, s):
+        """
+        Return the serialization as a period object. If the serializaton ends with 'A',  first converting to localtime and returning an aware datetime object in the local timezone. If the serialization ends with 'N', returning without conversion as an aware datetime object in the local timezone.
+        >>> ps = PendulumPeriodSerializer()
+        >>> ps.decode('20180730T1045N -> 20180725T1027N')
+        <Period [2018-07-30T10:45:00-04:00 -> 2018-07-25T10:27:00-04:00]>
+        >>> ps.decode('20180730T1445A -> 20180725T1727A')
+        <Period [2018-07-30T10:45:00-04:00 -> 2018-07-25T13:27:00-04:00]>
+        """
+
+        start, end = [x.strip() for x in s.split('->')]
+        start_enc = self.decode_datetime(start)
+        end_enc = self.decode_datetime(end)
+        return pendulum.period(start_enc, end_enc)
+
+
 class PendulumDateSerializer(Serializer):
     """
     This class handles pendulum date objects. Encode as date string and decode as a midnight datetime without conversion in the local timezone.
     >>> ds = PendulumDateSerializer()
     >>> ds.encode(pendulum.date(2018, 7, 25))
     '20180725'
     >>> ds.decode('20180725')
@@ -103,14 +159,15 @@
 
     def decode(self, s):
         """
         Return the serialization as a timedelta object.
         """
         return parse_duration(s)[1]
 
+
 class PendulumWeekdaySerializer(Serializer):
     """
     This class handles dateutil.rrule.weeday objects. Note in the following examples that unquoted weekdays, eg. MO(-3), are dateutil.rrule.weekday objects.
     >>> wds = PendulumWeekdaySerializer()
     >>> wds.encode(MO(-3))
     '-3MO'
     >>> wds.encode(SA(+3))
@@ -184,20 +241,14 @@
     def __repr__(self):
         return decode(secret, self.encoded)
 
 
 
 class MaskSerializer(Serializer):
     """
-    This class handles pendulum.duration (timedelta) objects.
-    >>> mask = MaskSerializer()
-    >>> mask.encode(Mask("when to the sessions")) # doctest: +NORMALIZE_WHITESPACE
-    'w5zDnMOSwo7CicOnwo_Cl8Ojw5bDicKFw6XDi8Oow5_CisOUw6LDoA=='
-    >>> mask.decode('    w5zDnMOSwo7CicOnwo_Cl8Ojw5bDicKFw6XDi8Oow5_CisOUw6LDoA==') # doctest: +NORMALIZE_WHITESPACE
-    when to the sessions
     """
     OBJ_CLASS = Mask
 
     def encode(self, obj):
         """
         Encode the string using base64
         """
@@ -215,14 +266,15 @@
 
 def initialize_tinydb(dbfile):
     """
     """
     serialization = SerializationMiddleware()
     serialization.register_serializer(PendulumDateTimeSerializer(), 'T') # Time
     serialization.register_serializer(PendulumDateSerializer(), 'D')     # Date
+    serialization.register_serializer(PendulumPeriodSerializer(), 'P')   # Period
     serialization.register_serializer(PendulumDurationSerializer(), 'I') # Interval
     serialization.register_serializer(PendulumWeekdaySerializer(), 'W')  # Wkday
     serialization.register_serializer(MaskSerializer(), 'M')             # Mask
     if tinydb_version >= '4.0.0':
         db = TinyDB(dbfile, storage=serialization,
                 indent=1, ensure_ascii=False)
         db.default_table_name='items'
@@ -246,14 +298,16 @@
             until.append(f"{obj.weeks}w")
         if obj.remaining_days:
             until.append(f"{obj.remaining_days}d")
         if obj.hours:
             until.append(f"{obj.hours}h")
         if obj.minutes:
             until.append(f"{obj.minutes}m")
+        if obj.remaining_seconds:
+            until.append(f"{obj.remaining_seconds}s")
         if not until:
             until.append("0m")
         ret = "".join(until)
         return "".join(until)
     except Exception as e:
         print('format_duration', e)
         print(obj)
@@ -263,20 +317,21 @@
     try:
         return ", ".join([format_duration(x) for x in obj_lst])
     except Exception as e:
         print('format_duration_list', e)
         print(obj_lst)
 
 
-period_regex = re.compile(r'(([+-]?)(\d+)([wdhm]))+?')
+period_regex = re.compile(r'(([+-]?)(\d+)([wdhms]))+?')
 threeday_regex = re.compile(r'(MON|TUE|WED|THU|FRI|SAT|SUN)', re.IGNORECASE)
 anniversary_regex = re.compile(r'!(\d{4})!')
 
 period_hsh = dict(
     z=pendulum.duration(seconds=0),
+    s=pendulum.duration(seconds=1),
     m=pendulum.duration(minutes=1),
     h=pendulum.duration(hours=1),
     d=pendulum.duration(days=1),
     w=pendulum.duration(weeks=1),
         )
 
 def parse_duration(s):
```

### Comparing `etm-dgraham-4.9.7/etm/ical.py` & `etm-dgraham-5.0.3/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/etm/model.py` & `etm-dgraham-5.0.3/etm/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 
 from operator import itemgetter
 from itertools import groupby, combinations
 
 from prompt_toolkit.styles import Style
 from prompt_toolkit import __version__ as prompt_toolkit_version
 
-settings = {'ampm': True}
 # These are set in _main_
 DBITEM = None
 DBARCH = None
 ETMDB = None
 data = None
 # NOTE: view.main() will override ampm using the configuration setting
 ampm = True
@@ -103,25 +102,14 @@
     'journal':      '#daa520',
     'event':        '#90ee90',
     'available':    '#1e90ff',
     'waiting':      '#6495ed',
     'finished':     '#191970',
 })
 
-type2style = {
-        '!': 'class:inbox',
-        '<': 'class:pastdue',
-        '>': 'class:begin',
-        '%': 'class:journal',
-        '*': 'class:event',
-        '-': 'class:available',
-        '+': 'class:waiting',
-        '✓': 'class:finished',
-        }
-
 FINISHED_CHAR = '✓'
 UPDATE_CHAR = "𝕦"
 INBASKET_CHAR = "𝕚"
 KONNECT_CHAR = 'k'
 LINK_CHAR = 'g'
 PIN_CHAR = 'p'
 ELLIPSiS_CHAR = '…'
@@ -130,15 +118,14 @@
 etmdir = None
 
 ETMFMT = "%Y%m%dT%H%M"
 ZERO = pendulum.duration(minutes=0)
 ONEMIN = pendulum.duration(minutes=1)
 DAY = pendulum.duration(days=1)
 
-# finished_char = u"\u2713"  #  ✓
 
 WKDAYS_DECODE = {"{0}{1}".format(n, d): "{0}({1})".format(d, n) if n else d for d in ['MO', 'TU', 'WE', 'TH', 'FR', 'SA', 'SU'] for n in ['-4', '-3', '-2', '-1', '', '1', '2', '3', '4']}
 WKDAYS_ENCODE = {"{0}({1})".format(d, n): "{0}{1}".format(n, d) if n else d for d in ['MO', 'TU', 'WE', 'TH', 'FR', 'SA', 'SU'] for n in ['-4', '-3', '-2', '-1', '+1', '+2', '+3', '+4']}
 for wkd in ['MO', 'TU', 'WE', 'TH', 'FR', 'SA', 'SU']:
     WKDAYS_ENCODE[wkd] = wkd
 
 type_keys = {
@@ -146,14 +133,17 @@
     "-": "task",
     "✓": "finished",
     "%": "journal",
     "!": "inbox",
     "~": "wrap",
 }
 
+wrapbefore = "↱"
+wrapafter = "↳"
+
 type_prompt = u"item type character:"
 
 item_types = """item type characters:\n    """ + """\n    """.join([f"{k}: {v}" for k, v in type_keys.items()])
 
 allowed = {}
 required = {}
 common_methods = [x for x in 'cdgiklmnstuxz']
@@ -181,51 +171,20 @@
 allowed['!'] = common_methods + datetime_methods + task_methods + repeating_methods
 
 requires = {
         'a': ['s'],
         'b': ['s'],
         '+': ['s'],
         '-': ['rr'],
-        'o': ['rr'],
         'rr': ['s'],
         'js': ['s'],
         'ja': ['s'],
         'jb': ['s'],
         }
 
-busy_template = """{week}
-         {WA[1]} {DD[1]}  {WA[2]} {DD[2]}  {WA[3]} {DD[3]}  {WA[4]} {DD[4]}  {WA[5]} {DD[5]}  {WA[6]} {DD[6]}  {WA[7]} {DD[7]}
-         _____  _____  _____  _____  _____  _____  _____
-{l[0]}   {h[0][1]}  {h[0][2]}  {h[0][3]}  {h[0][4]}  {h[0][5]}  {h[0][6]}  {h[0][7]}
-{l[1]}   {h[1][1]}  {h[1][2]}  {h[1][3]}  {h[1][4]}  {h[1][5]}  {h[1][6]}  {h[1][7]}
-{l[2]}   {h[2][1]}  {h[2][2]}  {h[2][3]}  {h[2][4]}  {h[2][5]}  {h[2][6]}  {h[2][7]}
-{l[3]}   {h[3][1]}  {h[3][2]}  {h[3][3]}  {h[3][4]}  {h[3][5]}  {h[3][6]}  {h[3][7]}
-{l[4]}   {h[4][1]}  {h[4][2]}  {h[4][3]}  {h[4][4]}  {h[4][5]}  {h[4][6]}  {h[4][7]}
-{l[5]}   {h[5][1]}  {h[5][2]}  {h[5][3]}  {h[5][4]}  {h[5][5]}  {h[5][6]}  {h[5][7]}
-{l[6]}   {h[6][1]}  {h[6][2]}  {h[6][3]}  {h[6][4]}  {h[6][5]}  {h[6][6]}  {h[6][7]}
-{l[7]}   {h[7][1]}  {h[7][2]}  {h[7][3]}  {h[7][4]}  {h[7][5]}  {h[7][6]}  {h[7][7]}
-{l[8]}   {h[8][1]}  {h[8][2]}  {h[8][3]}  {h[8][4]}  {h[8][5]}  {h[8][6]}  {h[8][7]}
-{l[9]}   {h[9][1]}  {h[9][2]}  {h[9][3]}  {h[9][4]}  {h[9][5]}  {h[9][6]}  {h[9][7]}
-{l[10]}   {h[10][1]}  {h[10][2]}  {h[10][3]}  {h[10][4]}  {h[10][5]}  {h[10][6]}  {h[10][7]}
-{l[11]}   {h[11][1]}  {h[11][2]}  {h[11][3]}  {h[11][4]}  {h[11][5]}  {h[11][6]}  {h[11][7]}
-{l[12]}   {h[12][1]}  {h[12][2]}  {h[12][3]}  {h[12][4]}  {h[12][5]}  {h[12][6]}  {h[12][7]}
-{l[13]}   {h[13][1]}  {h[13][2]}  {h[13][3]}  {h[13][4]}  {h[13][5]}  {h[13][6]}  {h[13][7]}
-{l[14]}   {h[14][1]}  {h[14][2]}  {h[14][3]}  {h[14][4]}  {h[14][5]}  {h[14][6]}  {h[14][7]}
-{l[15]}   {h[15][1]}  {h[15][2]}  {h[15][3]}  {h[15][4]}  {h[15][5]}  {h[15][6]}  {h[15][7]}
-{l[16]}   {h[16][1]}  {h[16][2]}  {h[16][3]}  {h[16][4]}  {h[16][5]}  {h[16][6]}  {h[16][7]}
-{l[17]}   {h[17][1]}  {h[17][2]}  {h[17][3]}  {h[17][4]}  {h[17][5]}  {h[17][6]}  {h[17][7]}
-{l[18]}   {h[18][1]}  {h[18][2]}  {h[18][3]}  {h[18][4]}  {h[18][5]}  {h[18][6]}  {h[18][7]}
-{l[19]}   {h[19][1]}  {h[19][2]}  {h[19][3]}  {h[19][4]}  {h[19][5]}  {h[19][6]}  {h[19][7]}
-{l[20]}   {h[20][1]}  {h[20][2]}  {h[20][3]}  {h[20][4]}  {h[20][5]}  {h[20][6]}  {h[20][7]}
-{l[21]}   {h[21][1]}  {h[21][2]}  {h[21][3]}  {h[21][4]}  {h[21][5]}  {h[21][6]}  {h[21][7]}
-{l[22]}   {h[22][1]}  {h[22][2]}  {h[22][3]}  {h[22][4]}  {h[22][5]}  {h[22][6]}  {h[22][7]}
-{l[23]}   {h[23][1]}  {h[23][2]}  {h[23][3]}  {h[23][4]}  {h[23][5]}  {h[23][6]}  {h[23][7]}
-         _____  _____  _____  _____  _____  _____  _____
-{t[0]}   {t[1]}  {t[2]}  {t[3]}  {t[4]}  {t[5]}  {t[6]}  {t[7]}
-"""
 
 def subsets(l):
     """
     Return a list of the possible subsets of the list of strings, l, together with the size of the subset. E.g., if l = ('blue', 'green', 'red'), return [(1, 'blue'), (1, 'green'), (1, 'red'), (2, 'blue & green'), (2, 'blue & red'), (2, 'green & red'), (3, 'blue & green & red')]
     """
     l.sort()
     ret = [('1', x) for x in l]
@@ -234,15 +193,15 @@
         ret.append((str(len(l)), ' & '.join(l)))
     if len(l) > 2:
         for i in range(2, len(l)):
             # add an element for each subset of length i of l
             tmp = list(combinations(l, i))
             for tup in tmp:
                 ret.append((str(i), ' & '.join(list(tup))))
-    else:
+    if len(l) == 0:
         ret.append(('~', '~'))
     return ret
 
 
 def busy_conf_minutes(lofp):
     """
     lofp is a list of tuples of (begin_minute, end_minute) busy times, e.g., [(b1, e1) , (b2, e2), ...]. By construction bi < ei. By sort, bi <= bi+1.
@@ -255,15 +214,15 @@
     >>> busy_conf_minutes([(540, 620), (600, 720), (660, 700)])
     ([(540, 600), (620, 660), (700, 720)], [(600, 620), (660, 700)], 180)
     """
     lofp.sort()
     busy_minutes = []
     conf_minutes = []
     if not lofp:
-        return ([], [], 0)
+        return ([], [])
     (b, e) = lofp.pop(0)
     while lofp:
         (B, E) = lofp.pop(0)
         if e <= B:  # no conflict
             busy_minutes.append((b, e))
             b = B
             e = E
@@ -274,18 +233,17 @@
                 b = e
                 e = E
             else:  # E < e
                 conf_minutes.append((B, E))
                 b = E
                 e = e
     busy_minutes.append((b, e))
-    total_minutes = sum(e - b for (b, e) in busy_minutes + conf_minutes)
-    return busy_minutes, conf_minutes, total_minutes
+    return busy_minutes, conf_minutes
 
-def busy_conf_day(lofp):
+def busy_conf_day(lofp, allday=False):
     """
     lofp is a list of tuples of (begin_minute, end_minute) busy times, e.g., [(b1, e1) , (b2, e2), ...]. By construction bi < ei. By sort, bi <= bi+1.
     Return a hash giving total minutes and appropriate symbols for busy hours.
     >>> busy_conf_day([(540, 600), (600, 720)])
     {'total': 180, 9: '  #  ', 10: '  #  ', 11: '  #  '}
     >>> busy_conf_day([(540, 620), (600, 720), (660, 700)])
     {'total': 180, 9: '  #  ', 10: ' ### ', 11: ' ### '}
@@ -293,43 +251,72 @@
     {'total': 180, 9: '  #  ', 10: '  #  ', 11: ' ### '}
     >>> busy_conf_day([])
     {'total': 0}
     >>> busy_conf_day([(0, 1439)])
     {0: '  #  ', 'total': 1439, 1: '  #  ', 2: '  #  ', 3: '  #  ', 4: '  #  ', 5: '  #  ', 6: '  #  ', 7: '  #  ', 8: '  #  ', 9: '  #  ', 10: '  #  ', 11: '  #  ', 12: '  #  ', 13: '  #  ', 14: '  #  ', 15: '  #  ', 16: '  #  ', 17: '  #  ', 18: '  #  ', 19: '  #  ', 20: '  #  ', 21: '  #  ', 22: '  #  ', 23: '  #  '}
     """
 
-    busy_ranges, conf_ranges, total = busy_conf_minutes(lofp)
-    busy_hours = []
-    conf_hours = []
+    busy_ranges, conf_ranges = busy_conf_minutes(lofp)
+    busy_quarters = []
+    conf_quarters = []
+    first_quarter = beginbusy*4
+    last_quarter = first_quarter + 14*4 + 1
 
     for (b, e) in conf_ranges:
-        h_b = b // 60
-        h_e = e // 60
-        if e % 60: h_e += 1
+        h_b = b // 15
+        h_e = e // 15
+        if e % 15: h_e += 1
         for i in range(h_b, h_e):
-            if i not in conf_hours:
-                conf_hours.append(i)
+            if i not in conf_quarters:
+                conf_quarters.append(i)
 
     for (b, e) in busy_ranges:
-        h_b = b // 60
-        h_e = e // 60
-        if e % 60: h_e += 1
+        h_b = b // 15
+        h_e = e // 15
+        if e % 15: h_e += 1
         for i in range(h_b, h_e):
-            if i not in conf_hours and i not in busy_hours:
-                busy_hours.append(i)
+            if i not in conf_quarters and i not in busy_quarters:
+                busy_quarters.append(i)
     h = {}
-    for i in range(24):
-        if i in busy_hours:
-            h[i] = '#'.center(5, ' ')
-        elif i in conf_hours:
-            h[i] = '###'.center(5, ' ')
-        # else:
-        #     h[i] = '.'.center(3, ' ')
-        h['total'] = total
-    return h
+    h[0] = '  '
+    h[58] = '  '
+    for i in range(1, 58):
+        h[i] = ' ' if (i-1) % 4 else VSEP
+    empty = "".join([h[i] for i in range(59)])
+    for i in range(1, 58):
+        if allday:
+            h[i] = ADAY # if (i-1) % 4 else VSEP
+        else:
+            h[i] = HSEP if (i-1) % 4 else VSEP
+
+    # quarters: 1 before start + 1 after start + 56 + 1 between = 59 slots 0, ... 58
+    conflict = False
+    busy = False
+    for i in range(first_quarter):
+        if i in conf_quarters:
+            conflict = True
+        if i in busy_quarters:
+            busy = True
+        h[0] = CONF+ ' ' if conflict else BUSY + ' ' if busy else '  '
+    conflict = False
+    busy = False
+    for i in range(last_quarter, 24*4):
+        if i in conf_quarters:
+            conflict = True
+        elif i in busy_quarters:
+            busy = True
+        h[58] = ' ' + CONF if conflict else ' ' + BUSY if busy else '  '
+    for i in range(first_quarter, last_quarter):
+        if i in conf_quarters:
+            h[i-first_quarter+1] = CONF
+        elif i in busy_quarters:
+            h[i-first_quarter+1] = BUSY
+    res = f"\n{empty}\n{''.join([h[i] for i in range(59)])}"
+    full = "".join([h[i] for i in range(59)])
+    return empty, full
 
 def process_entry(s, settings={}):
     """
     Return tuples containing key, value and postion tuples for the string s.
     0         1         2         3         4         5         6
     0123456789012345678901234567890123456789012345678901234567890123456789
     * evnt @s 2p fri @e 90m @r m &w 2fr &u 6/1 9a @c dag @l home
@@ -417,15 +404,14 @@
             aug_tups.append((key, value, beg, end))
 
     for key, value, beg, end in aug_tups:
         if key in ['@r', '@j']:
             pos_hsh[tuple([beg, end])] = (f"{key[-1]}{key[-1]}", value)
             adding = key[-1]
         elif key in ['@a', '@u']:
-            # pos_hsh[tuple((beg, end))] = (key[-1], value)
             pos_hsh[tuple((beg, end))] = (key[-1], value)
             adding = None
         elif key.startswith('&'):
             if adding:
                 pos_hsh[tuple((beg, end))] = (f"{adding}{key[-1]}", value)
         elif key in ['itemtype', 'summary']:
             adding = None
@@ -504,30 +490,29 @@
                 'summary': ["summary", "brief item description. Append an '@' to add an option.", self.do_summary],
                 '+': ["include", "list of datetimes to include", self.do_datetimes],
                 '-': ["exclude", "list of datetimes to exclude", self.do_datetimes],
                 'a': ["alerts", "list of alerts", do_alert],
                 'b': ["beginby", "number of days for beginby notices", do_beginby],
                 'c': ["calendar", "calendar", do_string],
                 'd': ["description", "item details", do_paragraph],
-                'e': ["extent", "timeperiod", do_period],
+                'e': ["extent", "timeperiod", do_duration],
                 'w': ["wrap", "list of two timeperiods", do_two_periods],
-                'f': ["finish", "completion datetime", self.do_datetime],
+                'f': ["finish", "completion datetime", self.do_completion],
                 'g': ["goto", "url or filepath", do_string],
-                'h': ["completions", "list of completion datetimes", self.do_datetimes],
+                'h': ["completions", "list of completion datetimes", self.do_completions],
                 'i': ["index", "forward slash delimited string", do_string],
                 'k': ["konnection", "document id", do_konnection],
                 'l': ["location", "location or context, e.g., home, office, errands", do_string],
                 'm': ["mask", "string to be masked", do_mask],
                 'n': ["attendee", "name <email address>", do_string],
-                'o': ["overdue", "character from (r)estart, (s)kip, (k)eep or (p)reserve", do_overdue],
+                'o': ["overdue", "character from (r)estart, (s)kip or (k)eep", do_overdue],
                 'p': ["priority", "priority from 0 (none) to 4 (urgent)", do_priority],
-                's': ["start", "starting date or datetime", self.do_datetime],
+                's': ["scheduled", "starting date or datetime", self.do_datetime],
                 't': ["tag", "tag", do_string],
                 'u': ["used time", "timeperiod: datetime", do_usedtime],
-                # 'w': ['who', 'who is responsible for this item', do_string],
                 'x': ["expansion", "expansion key", do_string],
                 'z': ["timezone", "a timezone entry such as 'US/Eastern' or 'Europe/Paris' or 'float' to specify a naive/floating datetime", self.do_timezone],
                 '?': ["@-key", "", self.do_at],
 
                 'rr': ["repetition frequency", "character from (y)ear, (m)onth, (w)eek,  (d)ay, (h)our, mi(n)ute. Append an '&' to add a repetition option.", do_frequency],
                 'ri': ["interval", "positive integer", do_interval],
                 'rm': ["monthdays", "list of integers 1 ... 31, possibly prepended with a minus sign to count backwards from the end of the month", do_monthdays],
@@ -539,24 +524,24 @@
                 'rW': ["week numbers", "list of integers in 1, ... 53", do_weeknumbers],
                 'rc': ["count", "integer number of repetitions", do_count],
                 'ru': ["until", "datetime", self.do_until],
                 'rs': ["set positions", "integer", do_setpositions],
                 'r?': ["repetition &-key", "enter &-key", self.do_ampr],
 
                 'jj': ["summary", "job summary. Append an '&' to add a job option.", do_string],
-                'ja': ["alert", "list of timeperiod before task start followed by a colon and a list of command", do_alert],
+                'ja': ["alert", "list of timeperiod before job is scheduled followed by a colon and a list of command", do_alert],
                 'jb': ["beginby", " integer number of days", do_beginby],
                 'jd': ["description", " string", do_paragraph],
-                'je': ["extent", " timeperiod", do_period],
-                'jf': ["finished", " datetime", self.do_datetime],
+                'je': ["extent", " timeperiod", do_duration],
+                'jf': ["finish", " datetime", self.do_completion],
                 'ji': ["unique id", " integer or string", do_string],
                 'jl': ["location", " string", do_string],
                 'jm': ["mask", "string to be masked", do_mask],
                 'jp': ["prerequisite ids", "list of ids of immediate prereqs", do_stringlist],
-                'js': ["start", "timeperiod before task start when job is due", do_period],
+                'js': ["scheduled", "timeperiod before task scheduled when job is scheduled", do_duration],
                 'ju': ["used time", "timeperiod: datetime", do_usedtime],
                 'j?': ["job &-key", "enter &-key", self.do_ampj],
                 }
         if not self.entry:
             self.text_changed('', 0, False)
 
     def __repr__(self):
@@ -622,19 +607,26 @@
             pairs = pairs[:num]
         elif pairs:
             showing = "All repetitions"
         else:
             showing = "No repetitions"
         return  showing, f"from {starting}:\n  " + "\n  ".join(pairs)
 
+
+    def do_update(self):
+        timer_update = TimeIt('***UPDATE***')
+        logger.debug(f"updating {self.doc_id} with {self.item_hsh}")
+        self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+        timer_update.stop()
+
+
     def edit_item(self, doc_id=None, entry=""):
         if not (doc_id and entry):
             return None
         item_hsh = self.db.get(doc_id=doc_id)
-        # item_hsh = self.dbquery.get(doc_id=doc_id)
         self.init_entry = entry
         if item_hsh:
             self.doc_id = doc_id
             self.is_new = False
             self.item_hsh = deepcopy(item_hsh) # created and modified entries
             self.keyvals = []
             self.text_changed(entry, 0, False)
@@ -665,16 +657,14 @@
             self.db.remove(doc_ids=[doc_id])
             return True
         except:
             return False
 
 
     def add_used(self, doc_id, usedtime):
-        # usedtime = "period_str: datetime_str"
-
         self.item_hsh = self.db.get(doc_id=doc_id)
         self.doc_id = doc_id
         self.created = self.item_hsh['created']
         ut = [x.strip() for x in usedtime.split(': ')]
         if len(ut) != 2:
             return False
 
@@ -686,15 +676,16 @@
             return False
 
         used_times = self.item_hsh.get("u", [])
         used_times.append([per, dt])
         self.item_hsh['u'] = used_times
         self.item_hsh['created'] = self.created
         self.item_hsh['modified'] = pendulum.now('local')
-        self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+        # self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+        self.do_update()
 
         return True
 
 
 
     def schedule_new(self, doc_id, new_dt):
         self.item_hsh = self.db.get(doc_id=doc_id)
@@ -708,15 +699,16 @@
         else:
             # works both with and without r
             self.item_hsh.setdefault('+', []).append(new_dt)
         changed = True
         if changed:
             self.item_hsh['created'] = self.created
             self.item_hsh['modified'] = pendulum.now('local')
-            self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+            # self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+            self.do_update()
         return changed
 
 
 
     def reschedule(self, doc_id, old_dt, new_dt):
         if old_dt == new_dt:
             return
@@ -724,15 +716,16 @@
         changed = False
         self.doc_id = doc_id
         self.item_hsh = self.db.get(doc_id=doc_id)
         if 'r' not in self.item_hsh and '+' not in self.item_hsh:
             # not repeating
             self.item_hsh['s'] = new_dt
             self.item_hsh['modified'] = pendulum.now('local')
-            self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+            # self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+            self.do_update()
             changed = True
         else:
             # repeating
             removed_old = False
             added_new = self.schedule_new(doc_id, new_dt)
             if added_new:
                 removed_old = self.delete_instances(doc_id, old_dt, 0)
@@ -769,117 +762,129 @@
                 else:
                     # should not happen
                     logger.warning(f"could not remove {instance} from {self.item_hsh}")
             if changed:
                 self.item_hsh['created'] = self.created
                 self.item_hsh['modified'] = pendulum.now('local')
 
-                self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+                # self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+                self.do_update()
         else: # 1
             # all instance - delete item
             changed = self.delete_item(doc_id)
 
         return changed
 
 
     def finish_item(self, item_id, job_id, completed_datetime, due_datetime):
         # item_id and job_id should have come from dataview.hsh ok, maybe_finish and thus be valid
+
+        # 23/5/29 FIXME with a repeating item either r or +, finishing an
+        # instance other than the oldest requires besides adding the instance to @h either
+        # deleting an @+ or adding an @- NOT changing @s!
+
+        # What to do about history? Make history a hash with done keys and
+        # lists of (done-due) or ZERO periods as values. Show competed on due
+        # date with period.days in right hand column if 2nd component is not
+        # ZERO. Why list of period values? done's resolution is one minute so
+        # more than one completion might be attributed to the same minute.
+
         save_item = False
         self.item_hsh = self.db.get(doc_id=item_id)
         self.doc_id = item_id
         self.created = self.item_hsh['created']
-        logger.debug(f"completed: {completed_datetime}; due: {due_datetime}")
+        completion_entry = pendulum.period(completed_datetime, due_datetime) if due_datetime else pendulum.period(completed_datetime, completed_datetime)
         if job_id:
             j = 0
             for job in self.item_hsh['j']:
                 if job['i'] == job_id:
-                    self.item_hsh['j'][j]['f'] = completed_datetime
+                    self.item_hsh['j'][j]['f'] = completion_entry
                     save_item = True
                     break
                 else:
                     j += 1
                     continue
             ok, jbs, last = jobs(self.item_hsh['j'], self.item_hsh)
             if ok:
                 self.item_hsh['j'] = jbs
                 if last:
-                    nxt = get_next_due(self.item_hsh, last, due_datetime)
-                    logger.debug(f"nxt: {nxt}")
+                    nxt = get_next_due(self.item_hsh, last, completion_entry.end)
                     if nxt:
                         if 'r' in self.item_hsh:
                             for i in range(len(self.item_hsh['r'])):
                                 if 'c' in self.item_hsh['r'][i] and self.item_hsh['r'][i]['c'] > 0:
-                                    logger.debug(f"item_hsh[i]: {self.item_hsh['r'][i]}")
                                     self.item_hsh['r'][i]['c'] -= 1
                                     break
                         self.item_hsh['s'] = nxt
-                        self.item_hsh.setdefault('h', []).append(completed_datetime)
+                        self.item_hsh.setdefault('h', []).append(completion_entry)
                         save_item = True
                     else:  # finished last instance
-                        self.item_hsh['f'] = completed_datetime
+                        self.item_hsh['f'] = completion_entry
                         save_item = True
 
         else:
             # no jobs
             if 's' in self.item_hsh:
                 if 'r' in self.item_hsh:
-                    nxt = get_next_due(self.item_hsh, completed_datetime, due_datetime)
-                    logger.debug(f"nxt: {nxt}")
+                    nxt = get_next_due(self.item_hsh, completed_datetime, completion_entry.end)
                     if nxt:
                         for i in range(len(self.item_hsh['r'])):
                             if 'c' in self.item_hsh['r'][i] and self.item_hsh['r'][i]['c'] > 0:
-                                logger.debug(f"item_hsh[i]: {self.item_hsh['r'][i]}")
                                 self.item_hsh['r'][i]['c'] -= 1
                                 break
                         self.item_hsh['s'] = nxt
-                        self.item_hsh.setdefault('h', []).append(completed_datetime)
+
+                        self.item_hsh.setdefault('h', []).append(completion_entry)
                         save_item = True
                     else:  # finished last instance
-                        self.item_hsh['f'] = completed_datetime
+                        self.item_hsh['f'] = completion_entry
                         save_item = True
 
                 elif '+' in self.item_hsh:
                     # simple repetition
                     tmp = [self.item_hsh['s']] + self.item_hsh['+']
                     tmp.sort()
                     due = tmp.pop(0)
                     if tmp:
                         self.item_hsh['s'] = tmp.pop(0)
                     if tmp:
                         self.item_hsh['+'] = tmp
-                        self.item_hsh.setdefault('h', []).append(completed_datetime)
+                        self.item_hsh.setdefault('h', []).append(completion_entry)
                         save_item = True
                     else:
                         del self.item_hsh['+']
-                        self.item_hsh['f'] = completed_datetime
+                        self.item_hsh['f'] = completion_entry
                         save_item = True
                 else:
-                    self.item_hsh['f'] = completed_datetime
+                    self.item_hsh['f'] = completion_entry
                     save_item = True
             else:
-                self.item_hsh['f'] = completed_datetime
+                self.item_hsh['f'] = completion_entry
                 save_item = True
 
         if save_item:
             num_finished = settings.get('num_finished', 0)
+
+
             if 'h' in self.item_hsh and num_finished:
                 ok = True
                 # only truncate completions for infinitely repeating tasks
                 for rr in self.item_hsh.get('r', {}):
                     if 'c' in rr or 'u' in rr:
                         # we have a count or an until: keep all completions
                         ok = False
                 if ok:
                     sh = self.item_hsh['h']
                     sh.sort(key=sortdt)
                     self.item_hsh['h'] = sh[-num_finished:]
 
             self.item_hsh['created'] = self.created
             self.item_hsh['modified'] = pendulum.now('local')
-            self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+            # self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+            self.do_update()
             return True
         return False
 
 
     def record_timer(self, item_id, job_id=None, completed_datetime=None, elapsed_time=None):
         if not (item_id and completed_datetime and elapsed_time):
             return
@@ -899,15 +904,16 @@
                     continue
         else:
             self.item_hsh.setdefault('u', []).append([elapsed_time, completed_datetime])
             save_item = True
         if save_item:
             self.item_hsh['created'] = self.created
             self.item_hsh['modified'] = pendulum.now('local')
-            self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+            # self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+            self.do_update()
 
 
     def cursor_changed(self, pos):
         # ((17, 24), ('e', '90m'))
         self.interval, self.active = active_from_pos(self.pos_hsh, pos)
 
 
@@ -969,19 +975,16 @@
                         if kv in self.object_hsh:
                             del self.object_hsh[kv]
             self.askreply[kv] = (ask, reply)
         else:
             display_key = f"@{key}" if len(key) == 1 else f"&{key[-1]}"
             self.askreply[kv] = ('unrecognized key', f'{display_key} is invalid')
 
-    # def set_item_hsh(self, hsh={}):
-    #     self.item_hsh = hsh
 
     def check_item_hsh(self):
-        logger.debug(f"item_hsh: {self.item_hsh}")
         created = self.item_hsh.get('created', None)
         self.item_hsh = {'created': created}
         cur_hsh = {}
         cur_key = None
         msg = []
         for pos, (k, v) in self.pos_hsh.items():
             obj = self.object_hsh.get((k, v))
@@ -1020,14 +1023,15 @@
             cur_hsh = {}
 
         if 'j' in self.item_hsh:
             ok, res, last = jobs(self.item_hsh['j'], self.item_hsh)
             if ok:
                 self.item_hsh['j'] = res
                 if last:
+                    #FIXME
                     self.item_hsh['f'] = last
             else:
                 msg.extend(res)
         if self.item_hsh.get('z', None) not in [None, 'float']:
             del self.item_hsh['z']
         if msg:
             logger.debug(f"{msg}")
@@ -1040,31 +1044,29 @@
 
         links = self.item_hsh.get('k', [])
         if links:
             # make sure the doc_id refers to an actual document
             self.item_hsh['k'] = [x for x in links if self.db.contains(doc_id=x)]
 
         if self.is_modified and not msg:
-            logger.debug(f"{repr(self)}")
             now = pendulum.now('local')
             if self.is_new:
                 # creating a new item or editing a copy of an existing item
                 self.item_hsh['created'] = now
                 if self.doc_id is None:
-                    logger.debug(f"inserting: {self.item_hsh}")
                     self.doc_id = self.db.insert(self.item_hsh)
                 else:
-                    self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+                    self.do_update()
             else:
                 # editing an existing item
                 if 'k' in self.item_hsh and self.doc_id in self.item_hsh['k']:
                     # remove self referential konnections
                     self.item_hsh['k'].remove(self.doc_id)
                 self.item_hsh['modified'] = now
-                self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
+                self.do_update()
 
 
     def check_requires(self, key):
         """
         Check that key has the prerequisite entries.
         if key in requires, check that each key in requires[k] has a corresponding key, val in keyvals: [(k, v), (k, v), ...]
         """
@@ -1262,15 +1264,16 @@
         >>> print(item.do_datetimes('2019-1-25 2p, 2019-1-30 4p, 2019-2-29 8a')[1])
         datetimes: 2019-01-25 2:00pm, 2019-01-30 4:00pm
         incomplete or invalid datetimes:  2019-2-29 8a
         """
         rep = args
         obj = None
         tz = self.item_hsh.get('z', None)
-        args = [x.strip() for x in args.split(',')]
+        if not isinstance(args, list):
+            args = [x.strip() for x in args.split(',')]
         obj = []
         rep = []
         bad = []
         all_ok = True
         for arg in args:
             if not arg:
                 continue
@@ -1283,14 +1286,59 @@
                 bad.append(arg)
         obj = obj if all_ok else None
         rep = f"local datetimes: {', '.join(rep)}" if (tz is not None and tz != 'float') else f"datetimes: {', '.join(rep)}"
         if bad:
             rep += f"\nincomplete or invalid datetimes:  {', '.join(bad)}"
         return obj, rep
 
+    def do_completions(self, args):
+        tz = self.item_hsh.get('z', None)
+        args = [x.strip() for x in args.split(',')]
+        all_ok = True
+        obj_lst = []
+        rep_lst = []
+        bad_lst = []
+        completions = []
+        # arg_lst will be a list of pendulum periods
+        for arg in args:
+            if not arg:
+                continue
+            obj, rep  = self.do_completion(arg)
+            if obj:
+                obj_lst.append(obj)
+                rep_lst.append(rep)
+            else:
+                all_ok = False
+                bad_lst.append(arg)
+
+
+        obj = obj_lst if all_ok else None
+        rep = f"periods: {', '.join(rep_lst)}"
+        if bad_lst:
+            rep += f"\nincomplete or invalid completions: {', '.join(bad_lst)}"
+
+        return obj, rep
+
+
+    def do_completion(self, arg):
+        obj = None
+        tz = self.item_hsh.get('z', None)
+        args = [x.strip() for x in arg.split('->')]
+        obj, rep = self.do_datetimes(args)
+        parts = [date_to_datetime(x) for x in obj] if obj else []
+        if len(parts) > 1:
+            start_dt, end_dt = parts[:2]
+            obj = pendulum.period(parts[0], parts[1])
+            rep = f"{format_datetime(start_dt, short=True)[1]} -> {format_datetime(end_dt, short=True)[1]}"
+        else:
+            obj = None
+            rep = f"\nincomplete or invalid completion: {rep}"
+        return obj, rep
+
+
     def do_timezone(self, arg=None):
         """
         >>> item = Item("")
         >>> item.do_timezone()
         ('local', 'local')
         >>> item.do_timezone('float')
         ('float', 'float')
@@ -1378,15 +1426,16 @@
     'Sun Apr 7 2019 7:45AM CEST'
     """
     date_calc_regex = re.compile(r'^\s*(.+)\s+([+-])\s+(.+)\s*$')
     timezone_regex = re.compile(r'^(.+)\s+([A-Za-z]+/[A-Za-z]+)$')
     period_string_regex = re.compile(r'^\s*(([+-]?\d+[wdhmMy])+\s*$)')
 
     ampm = settings.get('ampm', True)
-    datetime_fmt = "ddd MMM D YYYY h:mmA zz" if ampm else "ddd MMM D YYYY H:mm zz"
+    wkday_fmt = "ddd D MMM" if settings['dayfirst'] else "ddd MMM D"
+    datetime_fmt = f"{wkday_fmt} YYYY h:mmA zz" if ampm else f"{wkday_fmt} YYYY H:mm zz"
     m = date_calc_regex.match(s)
     if not m:
         return f'Could not parse "{s}"'
     x, pm, y = [z.strip() for z in m.groups()]
     xz = 'local'
     nx = timezone_regex.match(x)
     if nx:
@@ -1559,24 +1608,37 @@
     2p on Nov 7 of this year -> 11/07
     11a on Jan 17 of 2012 -> 12.01
     """
     if type(obj) != pendulum.DateTime:
         obj = pendulum.instance(obj)
     now = pendulum.now('local')
 
+    md_fmt = "DD/MM" if settings['dayfirst'] else "MM/DD"
+    ym_fmt = "YY.MM" if settings['yearfirst'] else f"MM.YY"
+
     if obj.year == now.year:
         if obj.month == now.month:
             if obj.day == now.day:
                 return obj.format("HH:mm")
             else:
-                return obj.format("MM/DD")
+                return obj.format(md_fmt)
         else:
-            return obj.format("MM/DD")
+            return obj.format(md_fmt)
     else:
-        return obj.format("YY.MM")
+        return obj.format(ym_fmt)
+
+def format_date(obj):
+    dayfirst = settings.get('dayfirst', False)
+    yearfirst = settings.get('yearfirst', False)
+    md = "D/M" if dayfirst else "M/D"
+    date_fmt = f"YY/{md}" if yearfirst else f"{md}/YY"
+    if type(obj) != pendulum.Date and type(obj) != pendulum.DateTime:
+        return False, ""
+    else:
+        return True, obj.format(date_fmt)
 
 
 def format_datetime(obj, short=False):
     """
     >>> format_datetime(parse_datetime("20160710T1730")[1])
     (True, 'Sun Jul 10 2016 5:30pm EDT')
     >>> format_datetime(parse_datetime("2015-07-10 5:30p", "float")[1])
@@ -1591,30 +1653,33 @@
     (True, 'Thu Jan 31 2019 6:30pm EST')
     >>> format_datetime(parse_datetime("2019-01-31 11:30p", "Europe/Paris")[1])
     (True, 'Thu Jan 31 2019 5:30pm EST')
     """
     ampm = settings.get('ampm', True)
     dayfirst = settings.get('dayfirst', False)
     yearfirst = settings.get('yearfirst', False)
-    logger.debug(f"model dayfirst: {dayfirst}; yearfirst: {yearfirst}")
     md = "D/M" if dayfirst else "M/D"
-    ymd = f"YY/{md}" if yearfirst else f"{md}/YY"
+    if short:
+        md = "D/M" if dayfirst else "M/D"
+        date_fmt = f"YY/{md}" if yearfirst else f"{md}/YY"
+    else:
+        md = "ddd D MMM" if dayfirst else "ddd MMM D"
+        date_fmt = f"{md}, YYYY" if yearfirst else f"{md} YYYY"
 
-    date_fmt = ymd if short else "ddd MMM D YYYY"
     time_fmt = "h:mmA" if ampm else "H:mm"
 
 
     if type(obj) == pendulum.Date:
         return True, obj.format(date_fmt)
 
-    if type(obj) != pendulum.DateTime:
+    if not isinstance(obj, pendulum.DateTime):
         try:
             obj = pendulum.instance(obj)
-        except:
-            return False, "a pendulum date or datetime."
+        except Exception as e:
+            return False, f"Error: {e}"
 
     # we want all-day events to display as dates
     if (obj.hour, obj.minute, obj.second, obj.microsecond) == (0, 0, 0, 0):
         # treat as date
         return True, obj.format(date_fmt)
 
     if obj.format('Z') == '':
@@ -1628,71 +1693,127 @@
         if not short: time_fmt += " zz"
     res = obj.format(f"{date_fmt} {time_fmt}")
     if ampm:
         res = res.replace('AM', 'am')
         res = res.replace('PM', 'pm')
     return True, res
 
+def format_period(obj):
+    if not isinstance(obj, pendulum.Period):
+        logger.debug(f"obj: {obj}")
+        return obj
+    start = obj.start
+    end = obj.end
+    return f"{format_datetime(start, short=True)[1]} -> {format_datetime(end, short=True)[1]}"
+
+def format_period_list(obj_lst):
+    if not isinstance(obj_lst, list):
+        obj_lst = [obj_lst]
+    return ", ".join([format_period(x) for x in obj_lst])
+
 
 def format_datetime_list(obj_lst):
     return ", ".join([format_datetime(x)[1] for x in obj_lst])
 
 
 def plain_datetime_list(obj_lst):
     return ", ".join([plain_datetime(x)[1] for x in obj_lst])
 
 def format_hours_and_tenths(obj):
     """
     Convert a pendulum duration object into hours and tenths of an hour rounding up to the nearest tenth.
     """
     if not isinstance(obj, pendulum.Duration):
         return None
-    usedtime_minutes = settings.get('usedtime_minutes', 1)
+    UT_MIN = settings.get('usedtime_minutes', 1)
+    if UT_MIN >= 1:
+        obj = round_minutes(obj)
     try:
-        if usedtime_minutes == 1:
+        if UT_MIN <= 1:
+            # hours, minutes and seconds if not rounded up
             return format_duration(obj, short=True)
         minutes = 0
         if obj.weeks:
             minutes += obj.weeks * 7 * 24 * 60
         if obj.remaining_days:
             minutes += obj.remaining_days * 24 * 60
         if obj.hours:
             minutes += obj.hours * 60
         if obj.minutes:
             minutes += obj.minutes
         if minutes:
-            return f"{math.ceil(minutes/usedtime_minutes)/(60/usedtime_minutes)}h"
+            return f"{math.ceil(minutes/UT_MIN)/(60/UT_MIN)}h"
         else:
             return "0m"
 
     except Exception as e:
         logger.error(f"error: {e} formatting {obj}")
-        return None
+        return obj
+
+def dt2minutes(obj):
+    return obj.hour * 60 + obj.minute
+
+
+def datetimes2busy(dta, dtb):
+    # a for after, b for before
+    ret = []
+    beg_dt = dtb
+    count = 0
+    while beg_dt < dta and count<5:
+        count += 1
+        by, bw, begin_day = beg_dt.isocalendar()
+        begin_week = (by, bw)
+        beg_min = dt2minutes(beg_dt)
+        if beg_dt.date() < dta.date():
+            # midnight - 1 minute
+            end_min = 1439
+        else:
+            # when dta ends
+            end_min = dt2minutes(dta)
+        ret.append((begin_week, begin_day, (beg_min, end_min)))
+        beg_dt = beg_dt + pendulum.duration(minutes=end_min - beg_min + 1)
+    return ret
 
 
 def round_minutes(obj):
-    """
-    if hours, show hours and minutes
-    otherwise, minutes and seconds
-    """
-    seconds = 60 if obj.remaining_seconds >= 30 else obj.remaining_seconds
-    return pendulum.duration(weeks=obj.weeks, days=obj.remaining_days, hours=obj.hours, minutes=obj.minutes, seconds=seconds)
+    seconds = obj.remaining_seconds
+    # round up
+    if seconds:
+        return obj + pendulum.duration(seconds = 60-seconds)
+    else:
+        return obj
+
+def usedminutes2bar(minutes):
+    # leave room for indent and weekday
+    chars = shutil.get_terminal_size()[0] - 18
+    # goal in hours to minutes
+    used_minutes = int(minutes)
+    used_fmt = format_duration(used_minutes*ONEMIN, short=True).center(6, ' ')
+    if usedtime_hours:
+        goal_minutes = int(usedtime_hours) * 60
+        numchars = math.ceil((used_minutes/goal_minutes)/(1/chars))
+        if numchars <= chars:
+            bar = f"{numchars*BUSY:<50}"
+        else:
+            bar = f"{chars*BUSY} {BUSY}"
+        return used_fmt, bar
+    else:
+        return used_fmt, ""
 
 
 
 def format_duration(obj, short=False):
     """
     if short report only hours and minutes, else include weeks and days
     >>> td = pendulum.duration(weeks=1, days=2, hours=3, minutes=27)
     >>> format_duration(td)
     '1w2d3h27m'
     """
     if not isinstance(obj, pendulum.Duration):
         return None
-    obj = round_minutes(obj)
     hours = obj.hours
     try:
         until =[]
         if obj.weeks:
             if short:
                 hours += obj.weeks * 7 * 24
             else:
@@ -1700,55 +1821,140 @@
 
         if obj.remaining_days:
             if short:
                 hours += obj.remaining_days * 24
             else:
                 until.append(f"{obj.remaining_days}d")
         minutes = obj.minutes
-
+        seconds = obj.remaining_seconds
         if hours:
             until.append(f"{hours}h")
         if minutes:
             until.append(f"{minutes}m")
+        if seconds:
+            until.append(f"{seconds}s")
         if not until:
             until.append("0m")
         return "".join(until)
     except Exception as e:
         logger.error(f"{obj}: {e}")
         return None
 
 
+def status_duration(obj):
+    """
+    hours, minutes and tenths of minutes for display in the status bar
+    """
+    if not isinstance(obj, pendulum.Duration):
+        return None
+    hours = obj.hours
+    try:
+        until =[]
+        if obj.weeks:
+            hours += obj.weeks * 7 * 24
+
+        if obj.remaining_days:
+            hours += obj.remaining_days * 24
+
+        if hours:
+            until.append(f"{hours}h")
+
+        minutes = obj.minutes
+        seconds = obj.remaining_seconds
+        if seconds:
+            if refresh_interval == 6:
+                until.append(f"{minutes}.{seconds//6}m")
+            else:
+                until.append(f"{minutes}m")
+        elif minutes:
+            until.append(f"{minutes}m")
+        if not until:
+            until.append("0m")
+        return "".join(until)
+    except Exception as e:
+        logger.error(f"{obj}: {e}")
+        return None
+
+def fmt_dur(obj):
+    """
+    From data.py - no rounding
+    >>> td = pendulum.duration(weeks=1, days=2, hours=3, minutes=27)
+    >>> format_duration(td)
+    '1w2d3h27m'
+    """
+    if not isinstance(obj, pendulum.Duration):
+        return None
+    try:
+        until =[]
+        if obj.weeks:
+            until.append(f"{obj.weeks}w")
+        if obj.remaining_days:
+            until.append(f"{obj.remaining_days}d")
+        if obj.hours:
+            until.append(f"{obj.hours}h")
+        if obj.minutes:
+            until.append(f"{obj.minutes}m")
+        if obj.remaining_seconds:
+            until.append(f"{obj.remaining_seconds}s")
+        if not until:
+            until.append("0m")
+        ret = "".join(until)
+        return "".join(until)
+    except Exception as e:
+        print('format_duration', e)
+        print(obj)
+        return None
+
+
 def format_duration_list(obj_lst):
     try:
         return ", ".join([format_duration(x) for x in obj_lst])
     except Exception as e:
         logger.error(f"{obj_lst}: {e}")
 
 
-period_regex = re.compile(r'(([+-]?)(\d+)([wdhmMy]))+?')
+period_regex = re.compile(r'(([+-]?)(\d+)([wdhmMys]))+?')
 expanded_period_regex = re.compile(r'(([+-]?)(\d+)\s(week|day|hour|minute|month|year)s?)+?')
-relative_regex = re.compile(r'(([+-])(\d+)([wdhmMy]))+?')
+relative_regex = re.compile(r'(([+-])(\d+)([wdhmMys]))+?')
 threeday_regex = re.compile(r'([+-]?[1234])(MON|TUE|WED|THU|FRI|SAT|SUN)', re.IGNORECASE)
 anniversary_regex = re.compile(r'!(\d{4})!')
 
 
+def parse_durations(s):
+    periods = [x.strip() for x in s.split('+')]
+    total = ZERO
+    bad = []
+    for d in periods:
+        ok, p = parse_duration(d)
+        if ok:
+            total += p
+        else:
+            bad.append(d)
+    if bad:
+        return False, bad
+    else:
+        return True, total
+
+
+
 def parse_duration(s):
     """\
     Take a period string and return a corresponding pendulum.duration.
     Examples:
         parse_duration('-2w3d4h5m')= Duration(weeks=-2,days=3,hours=4,minutes=5)
         parse_duration('1h30m') = Duration(hours=1, minutes=30)
         parse_duration('-10m') = Duration(minutes=10)
     where:
         y: years
         M: months
         w: weeks
         d: days
         h: hours
         m: minutes
+        s: seconds
 
     >>> 3*60*60+5*60
     11100
     >>> parse_duration("2d-3h5m")[1]
     Duration(days=1, hours=21, minutes=5)
     >>> pendulum.datetime(2015, 10, 15, 9, 0, tz='local') + parse_duration("-25m")[1]
     DateTime(2015, 10, 15, 8, 35, 0, tzinfo=Timezone('America/New_York'))
@@ -1771,23 +1977,27 @@
             'days': 'days',
             'h': 'hours',
             'hour': 'hours',
             'hours': 'hours',
             'm': 'minutes',
             'minute': 'minutes',
             'minutes': 'minutes',
+            's': 'seconds',
+            'second': 'seconds',
+            'seconds': 'seconds'
             }
 
     kwds = {
             'years': 0,
             'months': 0,
             'weeks': 0,
             'days': 0,
             'hours': 0,
-            'minutes': 0
+            'minutes': 0,
+            'seconds': 0
             }
 
     m = period_regex.findall(str(s))
     if not m:
         m = expanded_period_regex.findall(str(s))
         if not m:
             return False, f"Invalid period string '{s}'"
@@ -1805,49 +2015,44 @@
 
 sys_platform = platform.system()
 mac = sys.platform == 'darwin'
 windoz = sys_platform in ('Windows', 'Microsoft')
 
 from time import perf_counter as timer
 
-# FIXME: is this still used?
 class TimeIt(object):
-    def __init__(self, loglevel=1, label=""):
+    def __init__(self, label=""):
         self.loglevel = loglevel
         self.label = label
-        msg = "{0} timer started; loglevel: {1}".format(self.label, self.loglevel)
-        if self.loglevel in [1, 2]:
+        if self.loglevel == 1:
+            msg = "timer {0} started; loglevel: {1}".format(self.label, self.loglevel)
             logger.debug(msg)
-        elif self.loglevel == 3:
-            logger.warning(msg)
-        self.start = timer()
+            self.start = timer()
 
     def stop(self, *args):
-        self.end = timer()
-        self.secs = self.end - self.start
-        self.msecs = self.secs * 1000  # millisecs
-        msg = "{0} timer stopped; elapsed time: {1} milliseconds".format(self.label, self.msecs)
-        if self.loglevel in [1, 2]:
+        if self.loglevel == 1:
+            self.end = timer()
+            self.secs = self.end - self.start
+            self.msecs = self.secs * 1000  # millisecs
+            msg = "timer {0} stopped; elapsed time: {1} milliseconds".format(self.label, self.msecs)
             logger.debug(msg)
-        elif self.loglevel == 3:
-            logger.warning(msg)
 
 
 class NDict(dict):
     """
     Constructed from rows of (path, values) tuples. The path will be split using 'split_char' to produce the nodes leading to 'values'. The last element in values is presumed to be the 'id' of the item that generated the row.
     """
 
-    # tab = " " * 2
     tab = 2
 
-    def __init__(self, split_char='/'):
+    def __init__(self, split_char='/', compact=False):
         self.split_char = split_char
-        self.width = shutil.get_terminal_size()[0] - 2
+        self.width = shutil.get_terminal_size()[0]-2
         self.row = 0
+        self.compact = compact
         self.row2id = {}
         self.output = []
         self.flag_len = 4 # gkptp
 
     def __missing__(self, key):
         self[key] = NDict()
         return self[key]
@@ -1888,47 +2093,61 @@
                 self = self[key]
             elif keys_left:
                 self.setdefault("/".join(keys[j:]), []).append(values)
                 break
 
     def as_tree(self, t={}, depth = 0, level=0):
         """ return an indented tree """
+        self.width = shutil.get_terminal_size()[0]-2
         for k in t.keys():
             indent = NDict.tab * depth * " "
-            self.output.append(f"{indent}{k}")
+            # replace any newlines in the title with spaces
+            K = re.sub(' *\n+ *', ' ', k)
+            self.output.append(f"{indent}{K}")
             self.row += 1
             depth += 1
             if level and depth > level:
                 depth -= 1
                 continue
 
             if type(t[k]) == NDict:
                 self.as_tree(t[k], depth, level)
             else:
                 # we have a list of leaves
                 for leaf in t[k]:
                     indent = NDict.tab * depth * " "
                     l_indent = len(indent)
-                    # width - indent - 2 (type and space) - flags - 1 (space) - rhc
-                    summary_width = self.width - l_indent - 2 - self.flag_len - 2 - len(leaf[3])
+                    # replace any newlines in the summary with spaces
+                    leaf[0] = re.sub(' *\n+ *', ' ', leaf[0])
+                    leaf[1] = re.sub(' *\n+ *', ' ', leaf[1])
+                    if self.compact:
+                        summary_width = self.width - l_indent - 2 - len(leaf[3])
+                    else:
+                        summary_width = self.width - l_indent - 2 - len(leaf[2]) - 2 - len(leaf[3])
                     if settings['connecting_dots'] and (leaf[2].strip() or leaf[3].strip()):
                         times = leaf[3].rstrip() if leaf[3].strip() else ''
-                        details = f" {leaf[2]} {times}".replace('   ', LINEDOT)
+                        if self.compact:
+                            details = f" {times}".replace('   ', LINEDOT)
+                        else:
+                            details = f" {leaf[2]} {times}".replace('   ', LINEDOT)
                         fill = summary_width - len(leaf[1])
                         if fill < 0:
                             summary = leaf[1][:summary_width - 1] + ELLIPSiS_CHAR
                         elif fill >= 3:
                             pad = ' '*(fill%3) if fill%3 else ''
                             summary = f"{leaf[1][:summary_width - 1]}{pad}{LINEDOT*(fill//3)}"
                         else:
                             summary = leaf[1][:summary_width - 1].ljust(summary_width, ' ')
                         tmp = f"{indent}{leaf[0]} {summary}{details}"
                     else:
                         summary = leaf[1][:summary_width - 1] + ELLIPSiS_CHAR if len(leaf[1]) > summary_width else leaf[1].ljust(summary_width-1, ' ')
-                        tmp = f"{indent}{leaf[0]} {summary} {leaf[2]} {leaf[3]}"
+                        if self.compact:
+                            tmp = f"{indent}{leaf[0]} {summary} {leaf[3]}"
+                        else:
+                            tmp = f"{indent}{leaf[0]} {summary} {leaf[2]} {leaf[3]}"
 
                     self.output.append(tmp)
                     self.row2id[self.row] = leaf[4]
                     self.row += 1
                     if len(leaf) > 5:
                         lines = self.leaf_detail(leaf[5], depth)
                         for line in lines:
@@ -1937,26 +2156,30 @@
             depth -= 1
         return "\n".join(self.output), self.row2id
 
 
 class DataView(object):
 
     def __init__(self, etmdir):
+        timer_database = TimeIt('***DATABASE***')
         self.active_item = None
         self.active_view = 'agenda'
         self.prior_view = 'agenda'
         self.current = []
         self.alerts = []
         self.row2id = []
         self.id2relevant = {}
+        self.wkday2busy_details = {}
+        self.busy_row = 0
         self.link_list = []
         self.pinned_list = []
         self.current_row = 0
         self.agenda_view = ""
         self.done_view = ""
+        self.engaged_view = ""
         self.busy_view = ""
         self.calendar_view = ""
         self.query_view = ""
         self.query_text = ""
         self.query_items = []
         self.query_mode = "items table"
         self.report_view = ""
@@ -1965,14 +2188,15 @@
         self.cal_locale = None
         self.history_view = ""
         self.cache = {}
         self.itemcache = {}
         self.used_summary = {}
         self.used_details = {}
         self.used_details2id = {}
+        self.effort_details = {}
         self.currMonth()
         self.completions = []
         self.konnections_from = {}
         self.konnections_to = {}
         self.konnected = []
         if os.path.exists(timers_file):
             with open(timers_file, 'rb') as fn:
@@ -1983,20 +2207,22 @@
                     self.active_timer = x
                     break
         else:
             self.timers = {}
             self.active_timer = None
         self.saved_timers = deepcopy(self.timers)
         self.archive_after = 0
+
         self.set_etmdir(etmdir)
         self.views = {
                 'a': 'agenda',
                 'b': 'busy',
                 'c': 'completed',
                 'd': 'do next',
+                'e': 'engaged',
                 'f': 'forthcoming',
                 'h': 'history',
                 'i': 'index',
                 'k': 'konnected',
                 'l': 'location',
                 'm': 'timers',
                 'p': 'pinned',
@@ -2012,23 +2238,37 @@
         self.completion_keys = ['c', 'g', 'i', 'k', 'l', 'n', 't']
         self.edit_item = None
         self.is_showing_details = False
         self.is_showing_query = False
         self.is_showing_help = False
         self.is_editing = False
         self.is_showing_items = True
+        if needs_update:
+            timer_update = TimeIt('***UPDATE***')
+            self.update_datetimes_to_periods()
+            timer_update.stop()
         self.get_completions()
-        self.refresh_konnections()
+        timer_konnections = TimeIt('***KONNECTIONS***')
+        self.refreshKonnections()
+        timer_konnections.stop()
+        self.currYrWk()
+        timer_relevant = TimeIt('***RELEVANT***')
         self.refreshRelevant()
-        self.activeYrWk = self.currentYrWk
-        self.calAdv = pendulum.today().month // 7
-
-        self.refreshAgenda()
+        timer_relevant.stop()
+        timer_current = TimeIt('***CURRENT***')
         self.refreshCurrent()
+        timer_current.stop()
+        timer_agenda = TimeIt('***AGENDA***')
+        self.refreshAgenda()
+        timer_agenda.stop()
+        timer_archive = TimeIt('***ARCHIVE***')
+        self.possible_archive()
+        timer_archive.stop()
         self.currcal()
+        timer_database.stop()
 
     def set_etmdir(self, etmdir):
         self.etmdir = etmdir
         self.backupdir = os.path.join(self.etmdir, 'backups')
         # need these files for backups
         self.dbfile = os.path.normpath(os.path.join(etmdir, 'db.json'))
         self.cfgfile = os.path.normpath(os.path.join(etmdir, 'cfg.yaml'))
@@ -2068,15 +2308,14 @@
                 self.archive_after = int(self.settings['archive_after'])
             except Exception as e:
                 logger.error(f"An integer is required for archive_after - got {self.settings['archive_after']}. {e}")
 
         self.db = DBITEM
         self.dbarch = DBARCH
         logger.info(f"items: {len(DBITEM)}; archive: {len(DBARCH)}")
-        self.possible_archive()
         self.update_links()
 
     def use_archive(self):
         self.query_mode = "archive table"
         self.db = DBARCH
 
     def use_items(self):
@@ -2147,38 +2386,44 @@
                 self.konnections_to[link].remove(item.doc_id)
 
         # now update konnected to reflect the changes
         konnected = [x for x in self.konnections_to] + [x for x in self.konnections_from]
         self.konnected = list(set(konnected))
 
 
-
-    def refresh_konnections(self):
+    def refreshKonnections(self):
         """
         to_hsh: ID -> ids of items with @k ID
         from_hsh ID -> ids in @k
         """
         self.konnections_to = {}
         self.konnections_from = {}
         self.konnected = []
+        ids = []
+        ids_with_k = []
+
         for item in self.db:
+            doc_id = item.doc_id
+            ids.append(doc_id)
+            if 'k' in item:
+                ids_with_k.append(doc_id)
+
+        for item_id in ids_with_k:
             # from item to link by @k entry
-            links = [x for x in item.get('k', []) if self.db.contains(doc_id=x)]
+            item = self.db.get(doc_id=item_id)
+            links = [x for x in item.get('k', []) if x in ids]
+
             if links:
-                self.konnections_from[item.doc_id] = links
+                self.konnections_from[item_id] = links
                 # append the to links
                 for link in links:
-                    self.konnections_to.setdefault(link, []).append(item.doc_id)
-
+                    self.konnections_to.setdefault(link, []).append(item_id)
         konnected = [x for x in self.konnections_to] + [x for x in self.konnections_from]
         self.konnected = list(set(konnected))
 
-    # def refresh_konnected(self):
-    #     konnected = [x for x in self.konnections_to] + [x for x in self.konnections_from]
-    #     self.konnected = list(set(konnected))
 
     def handle_backups(self):
         removefiles = []
         timestamp = pendulum.now('UTC').format("YYYY-MM-DD")
         filelist = os.listdir(self.backupdir)
         # deal with db.json
         dbmtime = os.path.getctime(self.dbfile)
@@ -2218,14 +2463,33 @@
             cfgfiles.insert(0, f"cfg-{timestamp}.yaml")
             cfgfiles.sort(reverse=True)
             removefiles.extend([os.path.join(self.backupdir, x) for x in
                 cfgfiles[7:]])
         else:
             logger.info(f"{self.cfgfile} unchanged - skipping backup")
 
+        if os.path.exists(self.currfile):
+            currtime = os.path.getctime(self.currfile)
+            currfiles = [x for x in filelist if x.startswith('curr')]
+            currfiles.sort(reverse=True)
+            if currfiles:
+                lastcurrtime = os.path.getctime(os.path.join(self.backupdir, currfiles[0]))
+            else:
+                lastcurrtime = None
+            if lastcurrtime is None or currtime > lastcfgtime:
+                backupfile = os.path.join(self.backupdir, f"curr-{timestamp}.txt")
+                shutil.copy2(self.currfile, backupfile)
+                logger.info(f"backed up {self.currfile} to {backupfile}")
+                currfiles.insert(0, f"curr-{timestamp}.yaml")
+                currfiles.sort(reverse=True)
+                removefiles.extend([os.path.join(self.backupdir, x) for x in
+                    currfiles[7:]])
+            else:
+                logger.info(f"{self.currfile} unchanged - skipping backup")
+
         # maybe delete older backups
         if removefiles:
             logger.info(f"removing old files: {removefiles}")
             for f in removefiles:
                 os.remove(f)
         return True
 
@@ -2236,20 +2500,18 @@
             if state == 'r':
                 now = pendulum.now('local')
                 period += now - start
                 state = 'p'
                 timers[self.active_timer] = [state, now, period]
         if timers:
             if timers != self.saved_timers:
-                logger.debug(f"timers changed - dumping to {timers_file}")
                 with open(timers_file, 'wb') as fn:
                     pickle.dump(timers, fn)
                 self.saved_timers = timers
-            else:
-                logger.debug(f"timers unchanged - skipping dump to {timers_file}")
+
         elif os.path.exists(timers_file):
             logger.debug(f"removing {timers_file}")
             os.remove(timers_file)
         # this return is necessary to avoid blocking event_handler
         return
 
 
@@ -2274,23 +2536,23 @@
         states for this reminder's timer
             n: does not exist
             i: inactive
             r: running
             p: paused
         other timers:
             -: none active
-            +: one is active
+            +: one is active (running or paused)
 
         transitions:
-            n- -> r-
-            n+ -> i+
-            i- -> r-
-            i+ -> r-
-            r- -> p-
-            p- -> r-
+            n- -> r-   n- -> p-
+            n+ -> i+   n+ -> i+
+            i- -> r-   i- -> r-
+            i+ -> r-   i+ -> r-
+            r- -> p-   r- -> p-
+            p- -> r-   p- -> r-
         """
         if not doc_id:
             return
         other_timers = deepcopy(self.timers)
         if doc_id in other_timers:
             del other_timers[doc_id]
         active = [x for x, v in other_timers.items() if v[0] in ['r', 'p']]
@@ -2316,52 +2578,52 @@
                 period = period + now - start if state == 'r' else period
                 # toggle the state
                 state = 'p' if state == 'r' else 'r'
             self.active_timer = doc_id
             self.timers[doc_id] = state, now, period
         elif doc_id:
             # there is no timer for this item
-            # create the timer
+            # create the timer but don't start it
             if active:
                 state = 'i'
             else:
-                # no other timer is active so start this timer
-                state = 'r'
+                # no other timer is active so make this timer's state paused
+                state = 'p'
                 self.active_timer = doc_id
             self.timers[doc_id] = [state, now, ZERO]
 
-        logger.debug(f"next timer state for doc_id {doc_id}: {self.timers[doc_id]}")
         self.save_timers()
         return True, doc_id, active
 
 
     # for status bar report
     def timer_report(self):
         if not self.timers:
-            return ''
-        active = unrecorded = ""
+            return '', ''
+        active = inactive = status = ""
         zero = pendulum.Duration()
         delta = zero
         if self.active_timer:
             status, started, elapsed = self.timers[self.active_timer]
             delta = pendulum.now('local') - started
             if status == 'r': # running
                 delta += elapsed
-            active = f"{status}:{format_duration(delta, short=True)}"
+            active = f"{status}:{status_duration(delta)}"
+            # active = f"{status_duration(delta)}"
         if len(self.timers) > 1:
             timers = deepcopy(self.timers)
             if self.active_timer in timers:
                 del timers[self.active_timer]
-            relevant = [round_minutes(v[2]) for k, v in timers.items() if v[2] > zero]
+            relevant = [v[2] for k, v in timers.items() if v[2] > zero]
             if relevant:
                 total = zero
                 for v in relevant:
                     total += v
-                unrecorded = f" + i:{format_duration(total, short=True)}"
-        return f"{active}{unrecorded}  "
+                inactive = f" i:{status_duration(total)}"
+        return active, inactive
 
 
     def unsaved_timers(self):
         return len(self.timers)
 
 
     def timer_clear(self, doc_id=None):
@@ -2374,40 +2636,45 @@
         self.save_timers()
         self.show_active_view()
 
 
     def set_now(self):
         self.now = pendulum.now('local')
 
-    def set_active_item(self, id):
-        self.active_item = id
+    def set_active_item(self, doc_id):
+        self.active_item = doc_id
 
     def set_active_view(self, c):
         self.current_row = None
         self.prior_view = self.active_view
         self.active_view = self.views.get(c, 'agenda')
+        logger.debug(f"setting active view from c {c}: {self.active_view}")
         if self.active_view != 'query':
             self.use_items()
 
 
     def show_active_view(self):
         if self.active_view != 'query':
             self.hide_query()
         if self.active_view == 'agenda':
             self.refreshAgenda()
             return self.agenda_view
         if self.active_view == 'completed':
             self.refreshAgenda()
             self.row2id = self.done2id
             return self.done_view
+        if self.active_view == 'engaged':
+            self.refreshAgenda()
+            self.row2id = self.engaged2id
+            return self.engaged_view
         if self.active_view == 'busy':
             self.refreshAgenda()
             return self.busy_view
         if self.active_view == 'yearly':
-            # self.refreshCalendar()
+            self.refreshCalendar()
             return self.calendar_view
         if self.active_view == 'history':
             self.history_view, self.row2id = show_history(self.db, True, self.pinned_list, self.link_list, self.konnected, self.timers)
             return self.history_view
         if self.active_view == 'timers':
             self.timers_view, self.row2id = show_timers(self.db, self.pinned_list, self.link_list, self.konnected, self.timers, self.active_timer)
             return self.timers_view
@@ -2483,16 +2750,14 @@
         self.refreshAgenda()
 
 
     def currYrWk(self):
         """Set the active week to one containing today."""
         self.set_now()
         self.currentYrWk = self.activeYrWk = getWeekNum(self.now)
-        self.refreshAgenda()
-
 
     def dtYrWk(self, dtstr):
         dt = pendulum.parse(dtstr, strict=False)
         self.activeYrWk = getWeekNum(dt)
         self.refreshAgenda()
 
 
@@ -2510,59 +2775,64 @@
         self.active_month = dt.format("YYYY-MM")
 
 
     def refreshRelevant(self):
         """
         Called to set the relevant items for the current date and to change the currentYrWk and activeYrWk to that containing the current date.
         """
-        logger.debug(f"in refreshRelevant")
         self.set_now()
         self.currentYrWk = getWeekNum(self.now)
         dirty = True
         while dirty:
             self.current, self.alerts, self.id2relevant, dirty = relevant(self.db, self.now, self.pinned_list, self.link_list, self.konnected, self.timers)
             if dirty:
-                self.refresh_konnections()
-
+                self.refreshKonnections()
         self.refreshCache()
 
 
     def refreshAgenda(self):
         if self.activeYrWk not in self.cache:
             self.cache.update(schedule(self.db, yw=self.activeYrWk, current=self.current, now=self.now, pinned_list=self.pinned_list, link_list=self.link_list, konnect_list=self.konnected, timers=self.timers))
         # agenda, done, busy, row2id, done2id
-        self.agenda_view, self.done_view, self.busy_view, self.row2id, self.done2id = self.cache[self.activeYrWk]
+        self.agenda_view, self.done_view, self.engaged_view, self.busy_view, self.row2id, self.done2id, self.engaged2id, self.busy_details = self.cache[self.activeYrWk]
 
 
     def refreshCurrent(self):
         """
-        Agenda for the current and following 2 weeks
+        Agenda for the current and following 'keep_current' weeks
         """
         if self.currfile is not None:
             weeks = []
+            self.set_now()
+            curr_lines = []
             this_week = getWeekNum(self.now)
-            for _ in range(self.settings['keep_current']):
+            num_weeks = self.settings['keep_current'][0]
+            for _ in range(num_weeks):
+                # weeks corresponding to 0, ..., num_weeks-1
                 weeks.append(this_week)
                 this_week = nextWeek(this_week)
-            current = []
+
+            tmp_cache = self.cache
             for week in weeks:
-                if week not in self.cache:
-                    self.cache.update(schedule(self.db, yw=week, current=self.current, now=self.now, pinned_list=self.pinned_list, link_list= self.link_list))
-                agenda, done, busy, num2id, row2id = self.cache[week]
-                current.append(agenda)
-            with open(self.currfile, 'w', encoding='utf-8') as fo:
-                fo.write("\n\n".join([re.sub(' {5,}', ' ', x.strip()) for x in current]))
-                # fo.write("\n\n".join([x.lstrip() for x in current]))
-            logger.info(f"saved current schedule to {self.currfile}")
+                if week in self.cache:
+                    # append the agenda component
+                    curr_lines.append(self.cache[week][0])
+                else:
+                    logger.debug(f"week {week} missing from cache")
+            if curr_lines:
+                with open(self.currfile, 'w', encoding='utf-8') as fo:
+                    fo.write("\n\n".join([x.strip() for x in curr_lines]))
+                logger.info(f"saved {len(curr_lines)} weeks from current schedule to {self.currfile}")
+            else:
+                logger.info("current schedule empty - did not save")
 
         if self.nextfile is not None:
             next_view, row2id = show_next(self.db, self.pinned_list, self.link_list, self.konnected, self.timers)
             with open(self.nextfile, 'w', encoding='utf-8') as fo:
                 fo.write(re.sub(' {3,}', ' ', next_view))
-                # fo.write(next_view)
             logger.info(f"saved do next to {self.nextfile}")
 
 
     def show_query(self):
         self.is_showing_query = True
 
     def hide_query(self):
@@ -2682,15 +2952,16 @@
         res = self.get_row_details(row)
         if not res:
             return False
         doc_id, instance, job_id = res
         now = pendulum.now('local')
         item_hsh = self.db.get(doc_id=doc_id)
         item_hsh['modified'] = pendulum.now('local')
-        self.db.update(db_replace(item_hsh), doc_ids=[doc_id])
+        # self.db.update(db_replace(item_hsh), doc_ids=[doc_id])
+        self.do_update()
         return True
 
 
     def maybe_finish(self, row):
         """
         For tasks, '-', not already finished.
         No reps and no jobs add @f
@@ -2739,29 +3010,163 @@
 
     def clearCache(self):
         self.cache = {}
 
 
     def refreshCache(self):
         self.cache = schedule(ETMDB, self.currentYrWk, self.current, self.now, 5, 20, self.pinned_list, self.link_list, self.konnected, self.timers)
-        self.used_details, self.used_details2id, self.used_summary = get_usedtime(self.db, self.pinned_list, self.link_list, self.konnected, self.timers)
+        self.used_details, self.used_details2id, self.used_summary, self.effort_details = get_usedtime(self.db, self.pinned_list, self.link_list, self.konnected, self.timers)
 
     def update_links(self):
         """
         Look for items with @g entries and add their ids
         to link_list.
         """
         for item in self.db:
             if 'g' in item:
                 if item.doc_id not in self.link_list:
                     self.link_list.append(item.doc_id)
             else:
                 if item.doc_id in self.link_list:
                     self.link_list.remove(item_id)
 
+    def update_datetimes_to_periods(self):
+        """
+        For items with 'h' and/or 'f' entries, make sure entry is a pendulum period. Also for clones
+        created because of @o p, remove @k entries doc_ids that do not exist and remove @h entries.
+        if db.json exists and etm.json does not, then copy db.json to etm.json and run this script
+        using etm.json.
+        """
+        items_to_update = []
+        old_parent = {}       # doc_id of parent -> parent item for items with @o p entries
+        possible_clones = []  # items with @k entries
+        doc_ids = []
+        for item in self.db:
+            doc_ids.append(item.doc_id)
+            if item['itemtype'] == '-':
+                changed = False
+                if 'f' in item:
+                    if not isinstance(item['f'], pendulum.Period):
+                        start = date_to_datetime(item['f'])
+                        end = date_to_datetime(item.get('s', item['f']))
+                        item['f'] = pendulum.period(start, end)
+                        changed = True
+
+                if 'o' in item:
+                    if item['o'] == 'p':
+                        item['o'] = 'k'
+                        old_parent[item.doc_id] = item
+                        changed = True
+
+                if 'k' in item:
+                    possible_clones.append(item)
+
+                h_changed = False
+                if 'h' in item and not ('r' in item or '+' in item):
+                    # not repeating - should not have an @h
+                    del item['h']
+                    changed = True
+
+                if 'h' in item:
+                # deal with old to new history format
+                    curr_hist = item.get('h', [])
+                    new_hist = []
+                    h_changed = False
+                    for x in curr_hist:
+                        if isinstance(x, pendulum.Period):
+                            new_hist.append(x)
+                        else:
+                            x = date_to_datetime(x)
+                            new_hist.append( pendulum.period(x, x) )
+                            h_changed = True
+
+                    if h_changed:
+                        item['h'] = new_hist
+                        changed = True
+
+
+                if 'j' in item:
+                    j_changed = False
+                    new_jobs = []
+                    for job in item.get('j', []):
+                        if 'f' not in job:
+                            new_jobs.append(job)
+                        elif isinstance(job['f'], pendulum.Period):
+                            new_jobs.append(job)
+                        else:
+                            dt = date_to_datetime(job['f'])
+                            job['f'] = pendulum.period(dt, dt)
+                            new_jobs.append(job)
+                            j_changed = True
+                    if j_changed:
+                        item['j'] = new_jobs
+                        changed = True
+
+                if changed:
+                    items_to_update.append(item)
+
+
+        if items_to_update:
+            # backup db
+            updated_items = []
+            for item in items_to_update:
+                update_db(self.db, item.doc_id, item)
+                updated_items.append(item.doc_id)
+            logger.info(f"updated datetimes to periods for {len(updated_items)} items with these doc_ids:\n  {updated_items}")
+
+        items_to_update = []
+        items_to_remove = []
+        items_with_bad_links = []
+
+        for item in possible_clones:
+            for link in item.get('k', []):
+                if link in doc_ids:
+                    # the item corresponding to the link exists in the database
+                    if link in old_parent and item['summary'].startswith(old_parent[link]['summary']):
+                        # we have a clone - the summary of the clone begins with the summary from the possible parent
+                        parent = old_parent[link]
+                        if 'f' in item:
+                            # clone finished - add completion to parent
+                            if isinstance(item['f'], pendulum.Period):
+                                completion = item['f']
+                            else:
+                                start = date_to_datetime(item['f'])
+                                end = date_to_datetime(item.get('s', item['f']))
+                                completion = pendulum.period(start, end)
+                            parent.setdefault('h', []).append(completion)
+                            items_to_update.append(parent)
+                        elif 's' in item:
+                            # clone unfinished - add datetime to parent
+                            parent.setdefault('+', []).append(item['s'])
+                            items_to_update.append(parent)
+                        # remove the clone
+                        items_to_remove.append(item)
+                else:
+                    # dead link
+                    item['k'].remove(link)
+                    items_to_update.append(item)
+            if 'k' in item and not item['k']:
+                del item['k']
+
+        if items_to_update:
+            # backup db
+            updated_items = []
+            for item in items_to_update:
+                update_db(self.db, item.doc_id, item)
+                updated_items.append(item.doc_id)
+            logger.info(f"updated parents of clones for {len(updated_items)} items with these doc_ids:\n  {updated_items}")
+
+        if items_to_remove:
+            # backup db
+            removed_ids = []
+            for item in items_to_remove:
+                self.db.remove(doc_ids=[item.doc_id])
+                removed_ids.append(item.doc_id)
+            logger.info(f"removed clones for {len(removed_ids)} items with these doc_ids:\n  {removed_ids}")
+
 
     def possible_archive(self):
         """
         Collect old finished tasks, (repeating or not), old non-repeating events,
         and repeating events with old @u entries. Do not collect journal.
         """
         if not self.archive_after:
@@ -2770,24 +3175,45 @@
         old = pendulum.now() - pendulum.duration(years=self.archive_after)
         rows = []
         for item in self.db:
             if item['itemtype'] == '%':
                 # keep journal
                 continue
             elif 'f' in item:
-                if isinstance(item['f'], pendulum.DateTime):
-                    if item['f'] < old:
-                        # toss old finished tasks including repeating ones
-                        rows.append(item)
-                        continue
-                elif isinstance(item['f'], pendulum.Date):
-                    if item['f'] < old.date():
+                if isinstance(item['f'], pendulum.Period):
+                    if item['f'].start < old and item['f'].end < old:
                         # toss old finished tasks including repeating ones
                         rows.append(item)
                         continue
+                # elif isinstance(item['f'], pendulum.Date):
+                #     if item['f'] < old.date():
+                #         # toss old finished tasks including repeating ones
+                #         rows.append(item)
+                #         continue
+            elif '+' in item:
+                toss = True
+                for dt in item['+']:
+                    if isinstance(dt, pendulum.Date):
+                        # could be date or datetime
+                        if isinstance(dt, pendulum.DateTime):
+                            # datetime
+                            if dt.date() >= old.date():
+                                toss = False
+                                break
+                        else:
+                            # date
+                            if dt >= old.date():
+                                toss = False
+                                break
+                    else:
+                        prov = dt
+                    # FIXME: complicated whether or not to archive other repeating items with 't' so keep them
+                if toss:
+                    rows.append(item)
+                    continue
             elif 'r' in item:
                 toss = True
                 for rr in item['r']:
                     if 'u' not in rr:
                         toss = False
                         break
                     elif isinstance(rr['u'], pendulum.Date):
@@ -2804,43 +3230,47 @@
                                 break
                     else:
                         prov = rr['u']
                     # FIXME: complicated whether or not to archive other repeating items with 't' so keep them
                 # got here so 'u' item with u < datetime
                 if toss:
                     rows.append(item)
-                    continue
+
             elif item['itemtype'] == '*':
                 start = item.get('s', None)
                 if isinstance(start, pendulum.DateTime):
                     if start < old:
                         # toss old, non-repeating events
                         rows.append(item)
                         continue
                 elif isinstance(start, pendulum.Date):
                     if start < old.date():
                         # toss old, non-repeating events
                         rows.append(item)
                         continue
             else:
                 continue
-        logger.info(f"items to archive {len(rows)}: {[item.doc_id for item in rows]}")
-        add_items = []
+
+        # one at a time
+        archive_ids = [item.doc_id for item in rows]
+        failed_ids = []
         rem_ids = []
+        logger.info(f"items to archive {len(archive_ids)}: {archive_ids}")
         for item in rows:
-            rem_ids.append(item.doc_id)
-            add_items.append(item)
-
-        try:
-            self.dbarch.insert_multiple(add_items)
-        except:
-            logger.error(f"archive failed for doc_ids: {rem_ids}")
-        else:
-            self.db.remove(doc_ids=rem_ids)
-
+            try:
+                self.dbarch.insert(item)
+            except Exception as e:
+                failed_ids.append(f"{item.doc_id}; {e}")
+            else:
+                self.db.remove(doc_ids=[item.doc_id])
+                rem_ids.append(item.doc_id)
+        if rem_ids:
+            logger.info(f"archived doc_ids: {rem_ids}")
+        if failed_ids:
+            logger.error(f"archive failed for doc_ids: {failed_ids}")
         return rows
 
     def move_item(self, row=None):
         res = self.get_row_details(row)
         if not (res and res[0]):
             return False
         item_id = res[0]
@@ -2950,40 +3380,40 @@
     def refreshCalendar(self):
         """
         Advance = 0 shows the half year containing the current month. Advance
         = n shows the half year containing the month that is 6 x n months in
         the future if n > 0 or the past if n < 0.
         """
         width = shutil.get_terminal_size()[0]
-        indent = int((width - 45)/2) * " "
+        indent = int((width - 67)/2) * " "
         today = pendulum.today()
         y = today.year
         try:
 
             c = calendar.LocaleTextCalendar(0, self.cal_locale)
         except:
             logger.warning(f"error using locale {self.cal_locale}")
             c = calendar.LocaleTextCalendar(0)
         cal = []
-        m = 1
-        m += 6 * self.calAdv
+        m = 0
+        m += 12 * self.calAdv
         y += m // 12
         m %= 12
-        for i in range(6): # months in the half year
-            cal.append(c.formatmonth(y, m+i, w=2).split('\n'))
+        for i in range(12): # months in the half year
+            cal.append(c.formatmonth(y, 1+i, w=2).split('\n'))
         ret = ['']
-        for r in range(0, 6, 2):  # 6 months in columns of 2 months
-            l = max(len(cal[r]), len(cal[r + 1]))
-            for i in range(2):
+        for r in range(0, 12, 3):  # 12 months in columns of 3 months
+            l = max(len(cal[r]), len(cal[r + 1]), len(cal[r+2]))
+            for i in range(3):
                 if len(cal[r + i]) < l:
-                    for _ in range(len(cal[r + i]), l + 1):
+                    for _ in range(len(cal[r + i]), l + 2):
                         cal[r + i].append('')
             for j in range(l):  # rows from each of the 2 months
-                ret.append((u'%-20s     %-20s ' % (cal[r][j], cal[r +
-                    1][j])))
+                ret.append((u'%-20s   %-20s   %-20s ' % (cal[r][j], cal[r +
+                    1][j], cal[r + 2][j])))
 
         ret_lines = [f"{indent}{line}" for line in ret]
         ret_str = "\n".join(ret_lines)
         self.calendar_view = ret_str
 
 
     def nextcal(self):
@@ -2993,15 +3423,15 @@
 
     def prevcal(self):
         self.calAdv -= 1
         self.refreshCalendar()
 
 
     def currcal(self):
-        self.calAdv = pendulum.today().month // 7
+        self.calAdv = pendulum.today().month // 13
         self.refreshCalendar()
 
 def nowrap(txt, indent=3, width=shutil.get_terminal_size()[0]-3):
     return txt
 
 def wrap(txt, indent=3, width=shutil.get_terminal_size()[0]-3):
     """
@@ -3034,15 +3464,14 @@
     """
 
     """
     if not ('{XXX}' in summary and
             isinstance(start, pendulum.Date) and
             isinstance(relevant, pendulum.Date) and
             freq in ['y', 'm', 'w', 'd']):
-        # return unchanged summary
         return summary
     relevant_date = relevant.date() if isinstance(relevant, pendulum.DateTime) else relevant
     start_date = start.date() if isinstance(start, pendulum.DateTime) else start
     diff = relevant_date - start_date
     replacement = 0
     if freq == 'y':
         replacement = diff.in_years()
@@ -3073,22 +3502,14 @@
     if num < 4 or (num > 20 and num % 10 < 4):
         suffix = SUFFIXES[num % 10]
     else:
         suffix = SUFFIXES[0]
     return "{0}{1}".format(str(num), suffix)
 
 
-# def anniversary_string(startyear, endyear):
-#     """
-#     Compute the integer difference between startyear and endyear and
-#     append the appropriate English suffix.
-#     """
-#     return ordinal(int(endyear) - int(startyear))
-
-
 def one_or_more(s):
     if type(s) is list:
         return ", ".join([str(x) for x in s])
     else:
         return str(s)
 
 
@@ -3299,15 +3720,15 @@
 {%- if 'e' in h %}{{ " @e {}".format(in2str(h['e'])) }}{% endif %}\
 {%- if 'w' in h %}{{ " @w {}".format(inlst2str(h['w'])) }}{% endif %}\
 {%- if 'b' in h %}{{ " @b {}".format(h['b']) }}{% endif %}\
 {%- if 'z' in h %}{{ " @z {}".format(h['z']) }}{% endif %}\
 {%- endset %}\
 {{ nowrap(title) }} \
 {% if 'f' in h %}\
-{{ "@f {} ".format(dt2str(h['f'])[1]) }} \
+{{ "@f {} ".format(prd2str(h['f'])) }} \
 {% endif -%}\
 {% if 'a' in h %}\
 {%- set alerts %}\
 {% for x in h['a'] %}{{ "@a {}: {} ".format(inlst2str(x[0]), ", ".join(x[1])) }}{% endfor %}\
 {% endset %}\
 {{ nowrap(alerts) }} \
 {% endif %}\
@@ -3331,40 +3752,43 @@
 {% endif %}\
 {%- if 'k' in h %}
 {% for x in h['k'] %}{{ "@k {} ".format(x) }}{% endfor %}\
 {% endif %}\
 {%- if 'n' in h %}
 {% for x in h['n'] %}{{ "@n {} ".format(x) }}{% endfor %}\
 {% endif %}\
+{% if 'h' in h and h['h'] %}
+@h {{ nowrap(prdlst2str(h['h'])) }} \
+{%- endif %}\
 {%- set ls = namespace(found=false) -%}\
 {%- set location -%}\
 {%- for k in ['l', 'm', 'g', 'x', 'p'] -%}\
 {%- if k in h %}@{{ k }} {{ h[k] }}{% set ls.found = true %} {% endif -%}\
 {%- endfor -%}\
 {%- endset -%}\
 {%- if ls.found -%}\
 {{ nowrap(location) }} \
 {% endif -%}\
 {%- if 'r' in h -%}\
 {%- for x in h['r'] -%}\
 {%- if 'r' in x and x['r'] -%}\
 {%- set rrule %}\
 {{ x['r'] }}\
-{%- for k in ['i', 's', 'M', 'm', 'n', 'w', 'h', 'E', 'c'] -%}
+{%- for k in ['i', 's', 'M', 'm', 'n', 'w', 'E', 'c'] -%}
 {%- if k in x %} {{ "&{} {}".format(k, one_or_more(x[k])) }}{%- endif %}\
 {%- endfor %}
 {% if isinstance(x, dict) and 'u' in x %}{{ " &u {} ".format(dt2str(x['u'])[1]) }}{% endif %}\
 {%- endset %}
 @r {{ nowrap(rrule) }} \
 {% endif -%}\
 {%- endfor %}\
 {% if 'o' in h %}\
 @o {{ h['o'] }}{% endif %} \
 {% endif %}\
-{% for k in ['+', '-', 'h'] %}\
+{% for k in ['+', '-'] %}\
 {% if k in h and h[k] %}
 @{{ k }} {{ nowrap(dtlst2str(h[k])) }} \
 {%- endif %}\
 {%- endfor %}\
 {% if 'd' in h %}
 @d {{ nowrap(h['d'], 0) }} \
 {% endif -%}
@@ -3383,15 +3807,15 @@
 {%- endif %}\
 {% if 'u' in x %}\
 {%- set used %}\
 {% for u in x['u'] %}{{ "&u {}: {} ".format(in2str(u[0]), dt2str(u[1])[1]) }}{% endfor %}\
 {% endset %}
 {{ nowrap(used) }} \
 {% endif %}\
-{% if 'f' in x %}{{ " &f {}".format(dt2str(x['f'])[1]) }}{% endif %}\
+{% if 'f' in x %}{{ " &f {}".format(prd2str(x['f'])) }}{% endif %}\
 {%- endset %}
 @j {{ nowrap(job) }} \
 {%- endfor %}\
 {%- endif %}
 """
 
 # This duplication seems silly but seemed necessary to use nowrap in entry and wrap in display
@@ -3403,15 +3827,15 @@
 {%- if 'e' in h %}{{ " @e {}".format(in2str(h['e'])) }}{% endif %}\
 {%- if 'w' in h %}{{ " @w {}".format(inlst2str(h['w'])) }}{% endif %}\
 {%- if 'b' in h %}{{ " @b {}".format(h['b']) }}{% endif %}\
 {%- if 'z' in h %}{{ " @z {}".format(h['z']) }}{% endif %}\
 {%- endset %}\
 {{ wrap(title) }} \
 {% if 'f' in h %}\
-{{ "@f {} ".format(dt2str(h['f'])[1]) }} \
+{{ "@f {} ".format(prd2str(h['f'])) }} \
 {% endif -%}\
 {% if 'a' in h %}\
 {%- set alerts %}\
 {% for x in h['a'] %}{{ "@a {}: {} ".format(inlst2str(x[0]), ", ".join(x[1])) }}{% endfor %}\
 {% endset %}\
 {{ wrap(alerts) }} \
 {% endif %}\
@@ -3435,40 +3859,43 @@
 {% endif %}\
 {%- if 'k' in h %}
 {% for x in h['k'] %}{{ "@k {} ".format(x) }}{% endfor %}\
 {% endif %}\
 {%- if 'n' in h %}
 {% for x in h['n'] %}{{ "@n {} ".format(x) }}{% endfor %}\
 {% endif %}\
+{% if 'h' in h and h['h'] %}
+@h {{ prdlst2str(h['h']) }} \
+{%- endif %}\
 {%- set ls = namespace(found=false) -%}\
 {%- set location -%}\
 {%- for k in ['l', 'm', 'g', 'x', 'p'] -%}\
 {%- if k in h %}@{{ k }} {{ h[k] }}{% set ls.found = true %} {% endif -%}\
 {%- endfor -%}\
 {%- endset -%}\
 {%- if ls.found -%}\
 {{ wrap(location) }} \
 {% endif -%}\
 {%- if 'r' in h -%}\
 {%- for x in h['r'] -%}\
 {%- if 'r' in x and x['r'] -%}\
 {%- set rrule %}\
 {{ x['r'] }}\
-{%- for k in ['i', 's', 'M', 'm', 'n', 'w', 'h', 'E', 'c'] -%}
+{%- for k in ['i', 's', 'M', 'm', 'n', 'w', 'E', 'c'] -%}
 {%- if k in x %} {{ "&{} {}".format(k, one_or_more(x[k])) }}{%- endif %}\
 {%- endfor %}
 {% if isinstance(x, dict) and 'u' in x %}{{ " &u {} ".format(dt2str(x['u'])[1]) }}{% endif %}\
 {%- endset %}
 @r {{ wrap(rrule) }} \
 {% endif -%}\
 {%- endfor %}\
 {% if 'o' in h %}\
 @o {{ h['o'] }}{% endif %} \
 {% endif %}\
-{% for k in ['+', '-', 'h'] %}\
+{% for k in ['+', '-'] %}\
 {% if k in h and h[k] %}
 @{{ k }} {{ wrap(dtlst2str(h[k])) }} \
 {%- endif %}\
 {%- endfor %}\
 {% if 'd' in h %}
 @d {{ wrap(h['d'], 0) }} \
 {% endif -%}
@@ -3487,15 +3914,15 @@
 {%- endif %}\
 {% if 'u' in x %}\
 {%- set used %}\
 {% for u in x['u'] %}{{ "&u {}: {} ".format(in2str(u[0]), dt2str(u[1])[1]) }}{% endfor %}\
 {% endset %}\
 {{ wrap(used) }} \
 {% endif %}\
-{% if 'f' in x %}{{ " &f {}".format(dt2str(x['f'])[1]) }}{% endif %}\
+{% if 'f' in x %}{{ " &f {}".format(prd2str(x['f'])) }}{% endif %}\
 {%- endset %}
 @j {{ wrap(job) }} \
 {%- endfor %}\
 {%- endif %}
 
 {% if h.doc_id %}\
 {{ h.doc_id }}: \
@@ -3506,31 +3933,36 @@
 {% if 'modified' in h %}\
 ; {{ dt2str(h.modified)[1] }}\
 {%- endif %}\
 """
 
 jinja_entry_template = Template(entry_tmpl)
 jinja_entry_template.globals['dt2str'] = plain_datetime
-jinja_entry_template.globals['in2str'] = format_duration
+jinja_entry_template.globals['in2str'] = fmt_dur
 jinja_entry_template.globals['dtlst2str'] = plain_datetime_list
 jinja_entry_template.globals['inlst2str'] = format_duration_list
+jinja_entry_template.globals['prd2str'] = format_period
+jinja_entry_template.globals['prdlst2str'] = format_period_list
 jinja_entry_template.globals['one_or_more'] = one_or_more
 jinja_entry_template.globals['isinstance'] = isinstance
 jinja_entry_template.globals['nowrap'] = nowrap
 
 jinja_display_template = Template(display_tmpl)
 jinja_display_template.globals['dt2str'] = plain_datetime
-jinja_display_template.globals['in2str'] = format_duration
+jinja_display_template.globals['in2str'] = fmt_dur
 jinja_display_template.globals['dtlst2str'] = format_datetime_list
 jinja_display_template.globals['inlst2str'] = format_duration_list
+jinja_display_template.globals['prd2str'] = format_period
+jinja_display_template.globals['prdlst2str'] = format_period_list
 jinja_display_template.globals['one_or_more'] = one_or_more
 jinja_display_template.globals['isinstance'] = isinstance
 jinja_display_template.globals['wrap'] = wrap
 
 
+
 def do_beginby(arg):
     beginby_str = "an integer number of days"
     if not arg:
         return None, beginby_str
     ok, res = integer(arg, 1, None, False)
     if ok:
         obj = res
@@ -3569,18 +4001,18 @@
         return None, ''
     got_period = got_datetime = False
     rep_period = 'period'
     rep_datetime = 'datetime'
     parts = arg.split(': ')
     period = parts.pop(0)
     if period:
-        ok, res = parse_duration(period)
+        ok, res = parse_durations(period)
         if ok:
             obj_period = res
-            rep_period = format_duration(res)
+            rep_period = fmt_dur(res)
             got_period = True
         else:
             rep_period = res
     if parts:
         dt = parts.pop(0)
         ok, res, z = parse_datetime(dt)
         if ok:
@@ -3642,21 +4074,21 @@
             rep += f"\ncommmand is required but missing"
         else:
             obj = [obj_periods, commands]
 
     return obj, rep
 
 
-def do_period(arg):
+def do_duration(arg):
     """
-    >>> do_period('')
+    >>> do_duration('')
     (None, 'time period')
-    >>> do_period('90')
+    >>> do_duration('90')
     (None, 'incomplete or invalid period: 90')
-    >>> do_period('90m')
+    >>> do_duration('90m')
     (Duration(hours=1, minutes=30), '1h30m')
     """
     if not arg:
         return None, f"time period"
     ok, res = parse_duration(arg)
     if ok:
         obj = res
@@ -4224,15 +4656,21 @@
     return the next due datetime for an @r repetition
     """
     lofh = item.get('r')
     if not lofh:
         return ''
     rset = rruleset()
     overdue = item.get('o', 'k') # make 'k' the default for 'o'
-    dtstart = item['s']
+    start = item['s']
+    dtstart = date_to_datetime(item['s'])
+    if due > dtstart:
+        # we've finished a between instance
+        return dtstart
+    # we're finishing the oldest instance
+    due = dtstart if not due else due
     if overdue == 'k':
         aft = due
         inc = False
     elif overdue == 'r':
         aft = done
         dtstart = done
         inc = False
@@ -4241,18 +4679,17 @@
         if due < today:
             aft = today
             inc = True
         else:
             aft = due
             inc = False
     using_dates = False
-    if isinstance(dtstart, pendulum.Date) and not isinstance(dtstart, pendulum.DateTime):
+    if isinstance(start, pendulum.Date) and not isinstance(start, pendulum.DateTime):
         using_dates = True
-        dtstart = pendulum.datetime(year=dtstart.year, month=dtstart.month, day=dtstart.day, hour=0, minute=0)
-        aft = pendulum.datetime(year=aft.year, month=aft.month, day=aft.day, hour=0, minute=0)
+        aft = date_to_datetime(aft)
     for hsh in lofh:
         freq, kwd = rrule_args(hsh)
         kwd['dtstart'] = dtstart
         try:
             rset.rrule(rrule(freq, **kwd))
         except Exception as e:
             logger.error(f"error processing {hsh}: {e}")
@@ -4270,17 +4707,17 @@
         nxt = pendulum.instance(nxt_rset)
         if using_dates:
             nxt = nxt.date()
     else:
         nxt = None
     return nxt
 
-def date_to_datetime(dt):
+def date_to_datetime(dt, hour=0, minute=0):
     if isinstance(dt, pendulum.Date) and not isinstance(dt, pendulum.DateTime):
-        dt= pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=0, minute=0, tz='local')
+        dt= pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=hour, minute=minute, tz='local')
     return dt
 
 
 def item_instances(item, aft_dt, bef_dt=1):
     """
     Dates and datetimes decoded from the data store will all be aware and in the local timezone. aft_dt and bef_dt must therefore also be aware and in the local timezone.
     In dateutil, the starting datetime (dtstart) is not the first recurrence instance, unless it does fit in the specified rules.  Notice that you can easily get the original behavior by using a rruleset and adding the dtstart as an rdate recurrence.
@@ -4383,50 +4820,58 @@
             else:
                 instances = [pendulum.instance(x) for x in tmp if x] if tmp else []
         else:
             instances = [pendulum.instance(x) for x in rset.between(aft_dt, bef_dt, inc=True)]
 
     elif '+' in item:
         # no @r but @+ => simple repetition
-        tmp = [dtstart, *item['+']]
-        tmp = [date_to_datetime(x) for x in tmp]
+        s_hour = dtstart.hour
+        s_minute = dtstart.minute
+        # use hours and minutes from @s - they will be 0 if it is a date
+        tmp = [date_to_datetime(x, s_hour, s_minute) for x in item['+']]
+        tmp.append(dtstart)
         tmp.sort()
         if isinstance(bef_dt, int):
             instances = [x for x in tmp if (x >= aft_dt)][:bef_dt]
         else:
             instances = [x for x in tmp if (x >= aft_dt and x <= bef_dt)]
 
     else:
         # dtstart >= aft_dt
         if isinstance(bef_dt, int):
             instances = [dtstart] if dtstart >= aft_dt else []
         else:
             instances = [dtstart] if aft_dt <= dtstart <= bef_dt else []
 
     pairs = []
-    for instance in instances: # FIXME: task don't get item['e']
-        # multidays only for events
+    today = pendulum.today(tz=item.get('z', None))
+    for instance in instances:
         if item['itemtype'] == "*" and 'e' in item:
             for pair in beg_ends(instance, item['e'], item.get('z', 'local')):
                 pairs.append(pair)
-        elif item['itemtype'] == "-" and item.get('o', 'k') == 's':
-            if pairs and settings['limit_skip_display']:
-                # only keep the first instance that falls during or after today/now
-                break
-            if isinstance(instance, pendulum.Date) and not isinstance(instance, pendulum.DateTime) and instance >= pendulum.now().date():
-                pairs.append((instance, None))
-                logger.debug(f"appended overdue skip date instance: {instance}")
-            # elif instance.replace(hour=23, minute=59, second=59) >= pendulum.now(tz=item.get('z', None)):
-            elif instance >= pendulum.now(tz=item.get('z', None)):
+        elif item['itemtype'] == "-":
+            # handle tasks repeating or not, extent or not and overdue skip or not
+            if item.get('o', 'k') == 's':
+                if (instance.year, instance.month, instance.day) >= (today.year, today.month, today.day):
+                    if 'e' in item:
+                        for pair in beg_ends(instance, item['e'], item.get('z', 'local')):
+                            pairs.append(pair)
+                    else:
+                        pairs.append((instance, None))
+                    if pairs and settings['limit_skip_display']:
+                        # only keep the first instance that falls during or after today/now
+                        break
+            elif 'e' in item:
+                for pair in beg_ends(instance, item['e'], item.get('z', 'local')):
+                    pairs.append(pair)
+            else:
                 pairs.append((instance, None))
-                logger.debug(f"appended overdue skip datetime instance: {instance}")
-                logger.debug(f"overdue skip datetime pairs: {pairs}")
         else:
             pairs.append((instance, None))
-    pairs.sort()
+    pairs.sort(key = itemgetter(0))
 
     return pairs
 
 ########################
 ### end rrule setup ####
 ########################
 
@@ -4891,14 +5336,20 @@
     return weeks
 
 
 ######################
 ### end week/month ###
 ######################
 
+def period_from_fmt(s, z='local'):
+    """
+    """
+    start, end = [pendulum.from_format(x.strip(), "YYYYMMDDTHHmm", z) for x in s.split('->')]
+    return pendulum.period(start, end)
+
 def pen_from_fmt(s, z='local'):
     """
     >>> pen_from_fmt("20120622T0000")
     Date(2012, 6, 22)
     """
     dt = pendulum.from_format(s, "YYYYMMDDTHHmm", z)
     if z in ['local', 'Factory'] and dt.hour == dt.minute == 0:
@@ -4913,24 +5364,31 @@
     """
     >>> drop_zero_minutes(parse('2018-03-07 10am'))
     '10'
     >>> drop_zero_minutes(parse('2018-03-07 2:45pm'))
     '2:45'
     """
     ampm = settings['ampm']
-    if dt.minute == 0:
+    show_minutes = settings['show_minutes']
+    if show_minutes:
         if ampm:
-            return dt.format("h")
+            return dt.format("h:mm")
         else:
-            return dt.format("H")
+            return dt.format("HH:mm")
     else:
-        if ampm:
-            return dt.format("h:mm")
+        if dt.minute == 0:
+            if ampm:
+                return dt.format("h")
+            else:
+                return dt.format("H")
         else:
-            return dt.format("H:mm")
+            if ampm:
+                return dt.format("h:mm")
+            else:
+                return dt.format("HH:mm")
 
 
 def fmt_extent(beg_dt, end_dt):
     """
     >>> beg_dt = parse('2018-03-07 10am')
     >>> end_dt = parse('2018-03-07 11:30am')
     >>> fmt_extent(beg_dt, end_dt)
@@ -4957,17 +5415,19 @@
     end_fmt = drop_zero_minutes(end_dt)
 
     return f"{beg_fmt}{beg_suffix}-{end_fmt}{end_suffix}"
 
 
 def fmt_time(dt, ignore_midnight=True):
     ampm = settings['ampm']
+    show_minutes = settings['show_minutes']
     if ignore_midnight and dt.hour == 0 and dt.minute == 0 and dt.second == 0:
         return ""
     suffix = dt.format("A").lower() if ampm else ""
+
     dt_fmt = drop_zero_minutes(dt)
     return f"{dt_fmt}{suffix}"
 
 
 def beg_ends(starting_dt, extent_duration, z=None):
     """
     >>> starting = parse('2018-03-02 9am')
@@ -5006,15 +5466,14 @@
         print()
 
 
 def item_details(item, edit=False):
     """
 
     """
-    logger.debug(f"item: {item}, entry: {jinja_entry_template.render(h=item)}")
     try:
         if edit:
             return jinja_entry_template.render(h=item)
         else:
             return jinja_display_template.render(h=item)
 
     except Exception as e:
@@ -5030,80 +5489,82 @@
     'Dec 31 - Jan 6, 2019 #1'
     """
     dt_year, dt_week = yrwk
     # dt_week = dt_obj.week_of_year
     # year_week = f"{dt_year} Week {dt_week}"
     wkbeg = pendulum.parse(f"{dt_year}-W{str(dt_week).rjust(2, '0')}")
     wkend = pendulum.parse(f"{dt_year}-W{str(dt_week).rjust(2, '0')}-7")
-    week_begin = wkbeg.format("MMM D")
-    if wkbeg.month == wkend.month:
-        week_end = wkend.format("D")
+    if settings['dayfirst']:
+        week_end = wkend.format("D MMM")
+        week_begin = wkbeg.format("D") if wkbeg.month == wkend.month else wkbeg.format("D MMM")
     else:
-        week_end = wkend.format("MMM D")
-    # return f"{dt_year} Week {dt_week}: {week_begin} - {week_end}"
+        week_end = wkend.format("D") if wkbeg.month == wkend.month else wkend.format("MMM D")
+        week_begin = wkbeg.format("MMM D")
+
     return f"{week_begin} - {week_end}, {dt_year} #{dt_week}"
 
 
-def get_item(id):
+def get_item(doc_id):
     """
-    Return the hash correponding to id.
+    Return the hash correponding to doc_id.
     """
     pass
 
 
 def relevant(db, now=pendulum.now(), pinned_list=[], link_list=[], konnect_list=[], timers={}):
     """
     Collect the relevant datetimes, inbox, pastdues, beginbys and alerts. Note that jobs are only relevant for the relevant instance of a task
     Called by dataview.refreshRelevant
     """
-    # These need to be local times since all times from the datastore and rrule will be local times
+
+    wkday_fmt = "ddd D MMM" if settings['dayfirst'] else "ddd MMM D"
     dirty = False
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     summary_width = width - 7 - 16
     ampm = settings['ampm']
     rhc_width = 15 if ampm else 11
 
     today = pendulum.today()
     tomorrow = today + DAY
-    inbox_fmt = today.format("YYYYMMDD24@@")
-    pastdue_fmt = today.format("YYYYMMDD24^^")
-    begby_fmt = today.format("YYYYMMDD24~~")
+    inbox_fmt = today.format("YYYYMMDD    ")   # first
+    pastdue_fmt = today.format("YYYYMMDD^^^^") # after all day and timed
+    begby_fmt = today.format("YYYYMMDD~~~~")   # after past due
 
     id2relevant = {}
     inbox = []
     pastdue = []
     beginbys = []
     alerts = []
     current = []
 
     for item in db:
         instance_interval = []
         possible_beginby = None
         possible_alerts = []
         all_tds = []
-        id = item.doc_id
+        doc_id = item.doc_id
         if 'itemtype' not in item:
             logger.warning(f"no itemtype: {item}")
             item['itemtype'] = '?'
             # continue
         if 'g' in item:
-            if id not in link_list:
-                link_list.append(id)
+            if doc_id not in link_list:
+                link_list.append(doc_id)
         else:
-            if id in link_list:
-                link_list.remove(id)
+            if doc_id in link_list:
+                link_list.remove(doc_id)
 
         summary = item.get('summary', "~")
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
         if item['itemtype'] == '!':
             inbox.append([0, summary, item.doc_id, None, None])
             relevant = today
 
         elif 'f' in item:
-            relevant = item['f']
+            relevant = item['f'].end
             if isinstance(relevant, pendulum.Date) and not isinstance(relevant, pendulum.DateTime):
                 relevant = pendulum.datetime(year=relevant.year, month=relevant.month, day=relevant.day, hour=0, minute=0, tz='local')
 
         elif 's' in item:
             dtstart = item['s']
             has_a = 'a' in item
             has_b = 'b' in item
@@ -5136,16 +5597,16 @@
                         # td > 0m => earlier than startdt; dt < 0m => later than startdt
                         possible_alerts.append([td, cmd])
 
             # this catches all alerts and beginbys for the item
             if all_tds:
                 instance_interval = [today + min(all_tds), tomorrow + max(all_tds)]
 
-            if 'r' in item:
-                lofh = item['r']
+            if 'r' in item or '+' in item:
+                lofh = item.get('r', [])
                 rset = rruleset()
 
                 for hsh in lofh:
                     freq, kwd = rrule_args(hsh)
                     kwd['dtstart'] = dtstart
                     try:
                         rset.rrule(rrule(freq, **kwd))
@@ -5165,72 +5626,33 @@
                 if '+' in item:
                     for dt in item['+']:
                         if type(dt) == pendulum.Date:
                             dt = pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=0, minute=0, tz='local')
                         rset.rdate(dt)
 
                 if item['itemtype'] == '-':
-                    if item.get('o', 'k') == 's':
-                        relevant = rset.after(today, inc=True)
-                        if relevant:
-                            if item['s'] != pendulum.instance(relevant):
-                                item['s'] = pendulum.instance(relevant)
-                                update_db(db, item.doc_id, item)
-                    elif item.get('o', 'k') == 'p':
-                        # this is the first instance after 12am today
-                        relevant = rset.after(today, inc=True)
-                        # these are the instances to be preserved
-                        using_datetimes = isinstance(item['s'], pendulum.DateTime)
-                        # make sure we have a starting datetime for between
-                        start = item['s'] if using_datetimes else pendulum.datetime(
-                                item['s'].year, item['s'].month, item['s'].day)
-                        between = rset.between(start, today - ONEMIN, inc=True)
-                        if relevant and not between:
-                            # shouldn't happen
-                            logger.debug(f"relevant, {relevant}, but not between for {item}")
-                        summary = item['summary']
-
-                        if relevant and item['s'].format('YYYYMMDD') < today.format('YYYYMMDD'):
-                            # the due date for the repeating version of the item needs to be reset
-                            # keep a copy with the original @s for the instances to be preserved
-                            orig_id = item.doc_id
-                            hsh_copy = deepcopy(item)
-                            # remove @r and @o from the copy
-                            hsh_copy.pop('r')
-                            hsh_copy.pop('o')
-                            hsh_copy.setdefault('k', []).append(orig_id)
-                            hsh_copy['created'] = pendulum.now()
-                            if 'modified' in hsh_copy:
-                                hsh_copy.pop('modified')
-
-                            # update @s for the repeating item
+                    switch = item.get('o', 'k')
+                    relevant = rset.after(today, inc=True)
+                    if switch == 's':
+                        if relevant and item['s'] != pendulum.instance(relevant):
                             item['s'] = pendulum.instance(relevant)
-                            # update the repeating item in the db
-                            update_db(db, orig_id, item)
-
-                        for dt in between:
-                            pdt = pendulum.instance(dt)
-                            hsh_copy['s'] = pdt
-
-                            if using_datetimes:
-                                # hsh_copy['summary'] = f"{summary} ({pdt.format('YY/M/D H:mm')})"
-                                hsh_copy['summary'] = f"{summary} ({format_datetime(pdt, short=True)[1]})"
-                            else:
-                                # hsh_copy['summary'] = f"{summary} ({pdt.format('YY/M/D')})"
-                                hsh_copy['summary'] = f"{summary} ({format_datetime(pdt, short=True)[1]})"
-
-                            # set the new id to avoid a conflict
-                            new_id = db._get_next_id()
-                            logger.debug(f"inserting: {new_id}:  {hsh_copy}")
-                            db.insert(Document(hsh_copy, doc_id=new_id))
-                            dirty = True
-
-                    else:
-                        # for a restart or keep task, relevant is dtstart
-                        relevant = dtstart
+                            update_db(db, item.doc_id, item)
+                    else: # k or p
+                        relevant = rset.after(today, inc=True)
+                        already_done = [x.end for x in item.get('h', [])]
+                        # relevant will be the first instance after 12am today
+                        # it will be the @s entry for the updated repeating item
+                        # these are @s entries for the instances to be preserved
+                        between = rset.between(dtstart, today-ONEMIN, inc=True)
+                        remaining = [x for x in between if x not in already_done]
+                        # once instances have been created, between will be empty until
+                        # the current date falls after item['s'] and relevant is reset
+                        summary = f"{item['summary']} ({len(remaining)})"
+                        if dtstart.date() < today.date():
+                            pastdue.append([(dtstart.date() - today.date()).days, summary, item.doc_id, None, None])
                 else:
                     # get the first instance after today
                     try:
                         relevant = rset.after(today, inc=True)
                     except Exception as e:
                         logger.error(f"error processing {item}; {repr(e)}")
                     if not relevant:
@@ -5240,29 +5662,27 @@
 
                 # rset
                 if instance_interval:
                     instances = rset.between(instance_interval[0], instance_interval[1], inc=True)
                     if possible_beginby:
                         for instance in instances:
                             if today + DAY <= instance <= tomorrow + possible_beginby:
-                                id = item.doc_id
+                                doc_id = item.doc_id
                                 if 'r' in item:
                                     # use the freq from the first recurrence rule
                                     freq = item['r'][0].get('r', 'y')
                                 else:
                                     freq = 'y'
-                                # relevant = id2relevant[id]
-                                # summary = set_summary(item['summary'], item.get('s', None), relevant, freq)
                                 summary = set_summary(summary, item.get('s', None), pendulum.instance(instance).date(), freq)
                                 beginbys.append([(instance.date() - today.date()).days, summary, item.doc_id, None, instance])
                     if possible_alerts:
                         for instance in instances:
                             for possible_alert in possible_alerts:
                                 if today <= instance - possible_alert[0] <= tomorrow:
-                                    alerts.append([instance - possible_alert[0], instance, possible_alert[1], item['summary'], item.doc_id])
+                                    alerts.append([instance - possible_alert[0], instance, possible_alert[1], item['itemtype'],item['summary'], item.doc_id])
 
             elif '+' in item:
                 # no @r but @+ => simple repetition
                 tmp = [dtstart]
                 tmp.extend(item['+'])
                 tmp = [date_to_datetime(x) for x in tmp]
                 tmp.sort()
@@ -5277,28 +5697,28 @@
                     for instance in aft:
                         if today + DAY <= instance <= tomorrow + possible_beginby:
                             beginbys.append([(instance.date() - today.date()).days, summary, item.doc_id, None, instance])
                 if possible_alerts:
                     for instance in aft + bef:
                         for possible_alert in possible_alerts:
                             if today <= instance - possible_alert[0] <= tomorrow:
-                                alerts.append([instance - possible_alert[0], instance, possible_alert[1], item['summary'], item.doc_id])
+                                alerts.append([instance - possible_alert[0], instance, possible_alert[1], item['itemtype'], item['summary'], item.doc_id])
 
             else:
                 # 's' but not 'r' or '+'
                 relevant = dtstart
                 if (
                     possible_beginby
                     and today + DAY <= dtstart <= tomorrow + possible_beginby
                 ):
                     beginbys.append([(relevant.date() - today.date()).days, summary,  item.doc_id, None, None])
                 if possible_alerts:
                     for possible_alert in possible_alerts:
                         if today <= dtstart - possible_alert[0] <= tomorrow:
-                            alerts.append([dtstart - possible_alert[0], dtstart, possible_alert[1], item['summary'], item.doc_id])
+                            alerts.append([dtstart - possible_alert[0], dtstart, possible_alert[1], item['itemtype'], item['summary'], item.doc_id])
         else:
             # no 's', no 'f'
             relevant = None
 
         if not relevant:
             continue
         else:
@@ -5326,50 +5746,54 @@
                     days = int(job['b']) * DAY
                     if today + DAY <= jobstart <= tomorrow + days:
                         beginbys.append([(jobstart.date() - today.date()).days, job_summary, item.doc_id, job_id, None])
                 if 'a' in job:
                     for alert in job['a']:
                         for td in alert[0]:
                             if today <= jobstart - td <= tomorrow:
-                                alerts.append([dtstart - td, dtstart, alert[1],  job['summary'], item.doc_id, job_id, None])
+                                alerts.append([dtstart - td, dtstart, alert[1], '-', job['summary'], item.doc_id, job_id, None])
 
         id2relevant[item.doc_id] = relevant
 
         if item['itemtype'] == '-' and 'f' not in item and not pastdue_jobs and relevant.date() < today.date():
             pastdue.append([(relevant.date() - today.date()).days, summary, item.doc_id, None, None])
 
     inbox.sort()
     pastdue.sort()
     beginbys.sort()
     alerts.sort()
+    # alerts: alert datetime, start datetime, commands, summary, doc_id
     week = today.isocalendar()[:2]
-    day = (today.format("ddd MMM D"), )
+    day = (today.format(wkday_fmt), )
     for item in inbox:
         item_0 = ' '
         rhc = item_0.center(rhc_width, ' ')
-        id = item[2]
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
-        current.append({'id': item[2], 'job': None, 'instance': None, 'sort': (inbox_fmt, 1), 'week': week, 'day': day, 'columns': ['!', item[1], flags, rhc, id]})
+        doc_id = item[2]
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
+        current.append({'id': item[2], 'job': None, 'instance': None, 'sort': (inbox_fmt, 1), 'week': week, 'day': day, 'columns': ['!', item[1], flags, rhc, doc_id]})
 
     for item in pastdue:
         item_0 = str(item[0]) if item[0] in item else ""
         rhc = item_0.center(rhc_width, ' ')
-        id = item[2]
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        doc_id = item[2]
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
         try:
-            current.append({'id': item[2], 'job': item[3], 'instance': item[4], 'sort': (pastdue_fmt, 2, item[0]), 'week': week, 'day': day, 'columns': ['<', item[1], flags, rhc, id]})
+            current.append({'id': item[2], 'job': item[3], 'instance': item[4], 'sort': (pastdue_fmt, 2, item[0]), 'week': week, 'day': day, 'columns': ['<', item[1], flags, rhc, doc_id]})
         except Exception as e:
             logger.warning(f"could not append item: {item}; e: {e}")
 
     for item in beginbys:
-        item_0 = str(item[0]) if item[0] in item else ""
+        if item[0] in item:
+            item_0 = str(item[0]) if item[0] <= 0 else f"+{item[0]}"
+        else:
+            item_0 = ""
         rhc = item_0.center(rhc_width, ' ')
-        id = item[2]
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
-        current.append({'id': item[2], 'job': item[3], 'instance': item[4], 'sort': (begby_fmt, 3, item[0]), 'week': week, 'day': day, 'columns': ['>', item[1], flags, rhc, id]})
+        doc_id = item[2]
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
+        current.append({'id': item[2], 'job': item[3], 'instance': item[4], 'sort': (begby_fmt, 3, item[0]), 'week': week, 'day': day, 'columns': ['>', item[1], flags, rhc, doc_id]})
 
     return current, alerts, id2relevant, dirty
 
 
 def db_replace(new):
     """
     Used with update to replace the original doc with new.
@@ -5380,26 +5804,26 @@
         # remove any key/values from doc that are not in new
         for k in list(doc.keys()):
             if k not in new:
                 del doc[k]
     return transform
 
 
-def update_db(db, id, hsh={}):
-    old = db.get(doc_id=id)
+def update_db(db, doc_id, hsh={}):
+    old = db.get(doc_id=doc_id)
     if not old:
-        logger.error(f"Could not get document corresponding to id {id}")
+        logger.error(f"Could not get document corresponding to doc_id {doc_id}")
         return
     if old == hsh:
         return
     hsh['modified'] = pendulum.now()
     try:
-        db.update(db_replace(hsh), doc_ids=[id])
+        db.update(db_replace(hsh), doc_ids=[doc_id])
     except Exception as e:
-        logger.error(f"Error updating document corresponding to id {id}\nhsh {hsh}\nexception: {repr(e)}")
+        logger.error(f"Error updating document corresponding to doc_id {doc_id}\nhsh {hsh}\nexception: {repr(e)}")
 
 def write_back(db, docs):
     for doc in docs:
         try:
             doc_id = doc.doc_id
             update_db(db, doc_id, doc)
         except Exception as e:
@@ -5417,182 +5841,182 @@
     try:
         db.insert(hsh)
     except Exception as e:
         logger.error(f"Error updating database:\nhsh {hsh}\ne {repr(e)}")
 
 
 def show_forthcoming(db, id2relevant, pinned_list=[], link_list=[], konnect_list=[], timers={}):
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     summary_width = width - 19
     rows = []
     today = pendulum.today()
+    md_fmt = "DD/MM" if settings['dayfirst'] else "MM/DD"
     for item in db:
         if item.doc_id not in id2relevant:
             continue
 
-        id = item.doc_id
+        doc_id = item.doc_id
         if 'r' in item:
             # use the freq from the first recurrence rule
             freq = item['r'][0].get('r', 'y')
         else:
             freq = 'y'
         relevant = id2relevant[item.doc_id]
         if relevant < today:
             continue
         year = relevant.format("YYYY")
-        monthday = relevant.format("MMM D")
+        monthday = relevant.format(md_fmt)
         time = fmt_time(relevant)
-        rhc = f"{monthday} {time}".ljust(14, ' ')
+        rhc = f"{monthday:>6} {time:^7}".ljust(14, ' ')
 
         itemtype = FINISHED_CHAR if 'f' in item else item['itemtype']
         summary = set_summary(item['summary'], item.get('s', None), relevant, freq)
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
 
         rows.append(
                 {
-                    'id': id,
+                    'id': doc_id,
                     'sort': relevant,
                     'path': year,
                     'values': [
                         itemtype,
                         summary,
                         flags,
                         rhc,
-                        id
+                        doc_id
                         ],
                 }
                 )
 
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         path = row['path']
         values = row['values']
         rdict.add(path, values)
     tree, row2id = rdict.as_tree(rdict, level=0)
     return tree, row2id
 
-def get_flags(id, link_list=[], konnect_list=[], pinned_list=[], timers={}):
+def get_flags(doc_id, link_list=[], konnect_list=[], pinned_list=[], timers={}):
     """
     Always length = 4, space or character in each slot
     """
     flags = ""
-    if id in link_list:
+    if doc_id in link_list:
         flags += LINK_CHAR
-    if id in konnect_list:
+    if doc_id in konnect_list:
         flags += KONNECT_CHAR
-    if id in pinned_list:
+    if doc_id in pinned_list:
         flags += PIN_CHAR
-    if id in timers:
+    if doc_id in timers:
         flags += "t"
     return flags.rjust(4, ' ')
 
 def show_query_items(text, items=[], pinned_list=[], link_list=[], konnect_list=[], timers={}):
     rows = []
     if not items or not isinstance(items, list):
         return f"query: {text}\n   none matching", {}
     item_count = f" [{len(items)}]"
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     summary_width = width - len(item_count) - 7
     for item in items:
         mt = item.get('modified', None)
         if mt is not None:
             dt, label = mt, 'm'
         else:
             dt, label = item.get('created', None), 'c'
-        id = item.doc_id
+        doc_id = item.doc_id
         year = dt.format("YYYY")
         itemtype = FINISHED_CHAR if 'f' in item else item['itemtype']
         summary = item['summary']
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
-        rhc = f"{id: >6}"
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
+        rhc = f"{doc_id: >6}"
         rows.append(
                 {
                     'sort': dt,
                     'path': year,
                     'values': [
                         itemtype,
                         summary,
                         flags,
                         rhc,
-                        id],
+                        doc_id],
                 }
                 )
     rdict = NDict()
     path = f"query: {text[:summary_width]}{item_count}"
     for row in rows:
         values = row['values']
         rdict.add(path, values)
     tree, row2id = rdict.as_tree(rdict, level=0)
     return tree, row2id
 
 
 def show_history(db, reverse=True, pinned_list=[], link_list=[], konnect_list=[], timers={}):
-    width = shutil.get_terminal_size()[0] - 2
+    md_fmt = "DD/MM" if settings['dayfirst'] else "MM/DD"
+    ymd_fmt = f"YY/{md_fmt}" if settings['yearfirst'] else f"{md_fmt}/YY"
+    width = shutil.get_terminal_size()[0] - 3
     rows = []
     summary_width = width - 25
     for item in db:
         mt = item.get('modified', None)
         if mt is not None:
             dt, label = mt, 'm'
         else:
             dt, label = item.get('created', None), 'c'
         if dt is not None:
-            id = item.doc_id
-            year = dt.format("YYYY")
-            monthday = dt.format("MMM D").ljust(6, ' ')
-            c5dt = fivechar_datetime(dt)
-            # time = fmt_time(dt).rjust(7, ' ')
-            rhc = f" {c5dt} {label}"
+            doc_id = item.doc_id
+            ymd = dt.format(ymd_fmt)
+            rhc = f" {ymd} {label}"
             itemtype = FINISHED_CHAR if 'f' in item else item.get('itemtype', '?')
             summary = item.get('summary', "~")
-            flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+            flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
             path = '    m: last modified; c: created; most recent first'
             rows.append(
                     {
                         'sort': dt,
                         'path': path,
                         'values': [
                             itemtype,
                             summary,
                             flags,
                             rhc,
-                            id
+                            doc_id
                             ],
                     }
                     )
     try:
         rows.sort(key=itemgetter('sort'), reverse=reverse)
-    except:
+    except Exception as e:
         logger.error(f"sort exception: {e}: {[type(x['sort']) for x in rows]}")
     rdict = NDict()
     for row in rows:
         path = row['path']
         values = row['values']
         rdict.add(path, values)
     tree, row2id = rdict.as_tree(rdict, level=0)
     return tree, row2id
 
 
 def show_review(db, pinned_list=[], link_list=[], konnect_list=[], timers={}):
     """
     Unfinished, undated tasks and jobs
     """
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     rows = []
     locations = set([])
     summary_width = width - 18
     for item in db:
         if item.get('itemtype', None) not in ['-'] or 's' in item or 'f' in item:
             continue
-        id = item.doc_id
+        doc_id = item.doc_id
         rhc = item.get('l', '~')[:10].ljust(10, ' ')
         itemtype = item['itemtype']
         summary = item['summary']
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
         modified = item['modified'] if 'modified' in item else item['created']
 
         weeks = (pendulum.now() - modified).days // 7
         if weeks == 0:
             wkfmt = " This week"
         elif weeks == 1:
             wkfmt = " Last week"
@@ -5603,15 +6027,15 @@
                     'path': wkfmt,
                     'sort': modified,
                     'values': [
                         itemtype,
                         summary,
                         flags,
                         rhc, # location
-                        id,
+                        doc_id,
                         ]
                 }
                 )
     try:
         rows.sort(key=itemgetter('sort'), reverse=False)
     except Exception as e:
         logger.error(f"sort exception: {e}: {[type(x['sort']) for x in rows]}")
@@ -5623,60 +6047,60 @@
     tree, row2id = rdict.as_tree(rdict, level=0)
     return tree, row2id
 
 def show_timers(db, pinned_list=[], link_list=[], konnect_list=[], timers={}, active_timer=None):
     """
     timers
     """
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     rows = []
     locations = set([])
     summary_width = width - 18
     now = pendulum.now('local')
     state2sort = {
             'i': 'inactive',
             'r': 'active',
             'p': 'active'
             }
     total_time = ZERO
     num_timers = 0
     timer_ids = [x for x in timers if x]
-    for id in timer_ids:
-        item = db.get(doc_id=id)
+    for doc_id in timer_ids:
+        item = db.get(doc_id=doc_id)
         if not item:
             continue
-        state, start, elapsed = timers[id]
+        state, start, elapsed = timers[doc_id]
         if state == 'r':
-            elapsed += round_minutes(now - start)
+            elapsed += now - start
         num_timers += 1
         total_time += elapsed
         sort = state2sort[state]
-        rhc = f"{format_duration(elapsed, short=True)}  {state}".rjust(10, ' ')
+        rhc = f"{status_duration(elapsed)}  {state}".rjust(10, ' ')
         itemtype = item['itemtype']
         summary = item['summary']
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
         rows.append(
                 {
                     'sort': (sort, now - start),
                     'values': [
                         itemtype,
                         summary,
                         flags,
                         rhc, # status
-                        id,
+                        doc_id,
                         ]
                 }
                 )
     try:
         rows.sort(key=itemgetter('sort'), reverse=False)
     except Exception as e:
         logger.error(f"sort exception: {e}: {[type(x['sort']) for x in rows]}")
     rdict = NDict()
     timers_fmt = "timers" if num_timers > 1 else "timer"
-    path = f"{num_timers} {timers_fmt}: {format_duration(total_time, short=True)}".center(width, ' ')
+    path = f"{num_timers} {timers_fmt}: {status_duration(total_time)}".center(width, ' ')
     for row in rows:
         values = row['values']
         rdict.add(path, values)
     tree, row2id = rdict.as_tree(rdict, level=0)
     return tree, row2id
 
 def show_konnected(db, pinned_list=[], link_list=[], konnect_list=[], timers={}, selected_id=None, from_ids={}, to_ids={}):
@@ -5688,47 +6112,47 @@
     selected_item = db.get(doc_id=selected_id)
     if selected_item is None:
         return [], {}
 
     relevant = []
     relevant.append([' Selection', selected_item])
 
-    for id in from_ids.get(selected_id, []):
-        tmp = db.get(doc_id=id)
+    for doc_id in from_ids.get(selected_id, []):
+        tmp = db.get(doc_id=doc_id)
         if tmp:
             relevant.append([' From the selection', tmp])
 
-    for id in to_ids.get(selected_id, []):
-        tmp = db.get(doc_id=id)
+    for doc_id in to_ids.get(selected_id, []):
+        tmp = db.get(doc_id=doc_id)
         if tmp:
             relevant.append([' To the selection', tmp])
 
     if len(relevant) < 2:
         # from and to are empty
         return [], {}
 
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     rows = []
     summary_width = width - 11
     for path, item in relevant:
-        id = item.doc_id
-        rhc = str(id).rjust(5, ' ')
+        doc_id = item.doc_id
+        rhc = str(doc_id).rjust(5, ' ')
         itemtype = FINISHED_CHAR if 'f' in item else item.get('itemtype', '?')
         summary = item['summary']
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
         rows.append(
                 {
                     'path': path,
-                    'sort': (path, -id),
+                    'sort': (path, -doc_id),
                     'values': [
                         itemtype,
                         summary,
                         flags,
                         rhc,
-                        id,
+                        doc_id,
                         ]
                 }
                 )
     try:
         rows.sort(key=itemgetter('sort'), reverse=True)
     except Exception as e:
         logger.error(f"sort exception: {e}: {[type(x['sort']) for x in rows]}")
@@ -5741,15 +6165,15 @@
     return tree, row2id
 
 
 def show_next(db, pinned_list=[], link_list=[], konnect_list=[], timers={}):
     """
     Unfinished, undated tasks and jobs
     """
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     rows = []
     locations = set([])
     group_names = []
     groups = settings.get('locations', {})
     using_groups = True if groups else False
     if using_groups:
         group_names = groups.keys()
@@ -5757,16 +6181,16 @@
         for group, locations in groups.items():
             for location in locations:
                 location2groups.setdefault(location, []).append(group)
 
     for item in db:
         if item.get('itemtype', None) not in ['-'] or 's' in item or 'f' in item:
             continue
-        id = item.doc_id
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        doc_id = item.doc_id
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
         if 'j' in item:
             task_location = item.get('l', '~')
             priority = int(item.get('p', 0))
             sort_priority = 4 - int(priority)
             show_priority = str(priority) if priority > 0 else ""
             for job in item['j']:
                 if job.get('f'):
@@ -5779,50 +6203,50 @@
                 # status 1 -> waiting, status 0 -> available
                 rhc = " ".join([show_priority, extent]).center(7, ' ')
                 summary = job.get('summary')
                 job_id = job.get('i', None)
                 job_sort = str(job_id)
                 rows.append(
                     {
-                        'id': item.doc_id,
+                        'id': doc_id,
                         'job': job_id,
                         'instance': None,
                         'sort': (location, status, sort_priority, job_sort, job.get('summary', '')),
                         'location': location,
                         'columns': [
                             job.get('status', ''),
                             summary,
                             flags,
                             rhc,
-                            (id, None, job_id)
+                            (doc_id, None, job_id)
                             ]
                     }
                 )
         else:
             location = item.get('l', '~')
             priority = int(item.get('p', 0))
             extent = item.get('e', '')
             extent = format_duration(extent) if extent else ""
             sort_priority = 4 - int(priority)
             show_priority = str(priority) if priority > 0 else ""
             rhc = " ".join([show_priority, extent]).center(7, ' ')
             summary = item['summary']
             rows.append(
                     {
-                        'id': item.doc_id,
+                        'id': doc_id,
                         'job': None,
                         'instance': None,
                         'sort': (location, sort_priority, extent, item['summary']),
                         'location': location,
                         'columns': [
                             item['itemtype'],
                             summary,
                             flags,
                             rhc,
-                            (id, None, None)
+                            (doc_id, None, None)
                             ]
                     }
                     )
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         if using_groups:
@@ -5839,37 +6263,49 @@
     return tree, row2id
 
 
 def show_journal(db, id2relevant, pinned_list=[], link_list=[], konnect_list=[], timers={}):
     """
     journal grouped by index entry
     """
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     rows = []
     summary_width = width - 14
-    # indices = set([])
     for item in db:
-        id = item.doc_id
+        doc_id = item.doc_id
         if item['itemtype'] != '%':
             continue
-        rhc = str(id).rjust(5, ' ')
+        s = item.get('s', None)
+        if s:
+            rhc = format_date(s)[1]
+            ymd = s.format("YYYY/M/D").split('/')
+            year = ymd.pop(0)
+            month, day = [f"{x: >2}" for x in ymd]
+            ss = f"{year}/{month}/{day}"
+        else:
+            rhc = " "
+            ss = ""
+            year = month = day = ""
+        rhc = f"{rhc: ^8}"
         index = item.get('i', '~')
+        if index == settings['journal_name'] and year:
+            index = f"{index}/{year}/{month}"
         itemtype = item['itemtype']
-        summary = item['summary']
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        summary = item['summary'][:summary_width]
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
 
         rows.append({
-                    'sort': (index, item['summary']),
+                    'sort': (index, ss, item['summary']),
                     'path': index,
                     'values': [
                         itemtype,
                         summary,
                         flags,
                         rhc,
-                        id
+                        doc_id
                         ],
                     })
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         path = row['path']
         values = row['values']
@@ -5878,34 +6314,34 @@
     return tree, row2id
 
 
 def show_tags(db, id2relevant, pinned_list=[], link_list=[], konnect_list=[], timers={}):
     """
     tagged items grouped by tag
     """
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     rows = []
     for item in db:
-        id = item.doc_id
-        rhc = str(id).rjust(5, ' ')
+        doc_id = item.doc_id
+        rhc = str(doc_id).rjust(5, ' ')
         tags = item.get('t', [])
         itemtype = FINISHED_CHAR if 'f' in item else item.get('itemtype', '?')
         summary = item['summary']
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
 
         for tag in subsets(tags):
             rows.append({
                         'sort': (tag, item['itemtype'], item['summary']),
                         'path': tag[1],
                         'values': [
                             itemtype,
                             summary,
                             flags,
                             rhc,
-                            id
+                            doc_id
                             ],
                         })
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         path = row['path']
         values = row['values']
@@ -5914,33 +6350,33 @@
     return tree, row2id
 
 
 def show_location(db, id2relevant, pinned_list=[], link_list=[], konnect_list=[], timers={}):
     """
     items with location entries grouped by location
     """
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     rows = []
     for item in db:
-        id = item.doc_id
-        rhc = str(id).rjust(5, ' ')
+        doc_id = item.doc_id
+        rhc = str(doc_id).rjust(5, ' ')
         location = item.get('l', '~')
         itemtype = FINISHED_CHAR if 'f' in item else item.get('itemtype', '?')
         summary = item['summary']
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
 
         rows.append({
                     'sort': (location, item['itemtype'], item['summary']),
                     'path': location,
                     'values': [
                         itemtype,
                         summary,
                         flags,
                         rhc,
-                        id
+                        doc_id
                         ],
                     })
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         path = row['path']
         values = row['values']
@@ -5950,32 +6386,37 @@
 
 
 def show_index(db, id2relevant, pinned_list=[], link_list=[], konnect_list=[], timers={}):
     """
     All items grouped by index entry
     """
     rows = []
+    width = shutil.get_terminal_size()[0] - 3
+    summary_width = width - 14
     for item in db:
-        # if item['itemtype'] == '%':
-        #     continue
-        id = item.doc_id
-        rhc = str(id).rjust(5, ' ')
+        doc_id = item.doc_id
         index = item.get('i', '~')
         itemtype = FINISHED_CHAR if 'f' in item else item.get('itemtype', '?')
-        summary = item['summary']
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        summary = item['summary'][:summary_width]
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
+        s = item.get('s', None)
+        if s:
+            rhc = format_date(s)[1]
+        else:
+            rhc = " "
+        rhc = f"{rhc: ^8}"
         rows.append({
                     'sort': (index, item['summary']),
                     'path': index,
                     'values': [
                         itemtype,
                         summary,
                         flags,
                         rhc,
-                        id],
+                        doc_id],
                     })
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         path = row['path']
         values = row['values']
         try:
@@ -5983,43 +6424,45 @@
         except:
             logger.error(f"error adding path: {path}, values: {values}")
     tree, row2id = rdict.as_tree(rdict, level=0)
     return tree, row2id
 
 
 def show_pinned(items, pinned_list=[], link_list=[], konnect_list=[], timers={}):
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     rows = []
     rhc_width = 8
+    md_fmt = "D MMM" if settings['dayfirst'] else "MMM D"
+
     for item in items:
         mt = item.get('modified', None)
         if mt is not None:
             dt, label = mt, 'm'
         else:
             dt, label = item.get('created', None), 'c'
         if dt is not None:
-            id = item.doc_id
+            doc_id = item.doc_id
             year = dt.format("YYYY")
-            monthday = dt.format("MMM D")
+            monthday = dt.format(md_fmt)
             time = fmt_time(dt)
-            rhc = f"{str(id).rjust(6)}"
+            rhc = f"{str(doc_id).rjust(6)}"
             itemtype = FINISHED_CHAR if 'f' in item else item.get('itemtype', '?')
             summary = item['summary']
-            flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+            flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
 
             rows.append(
                     {
                         'sort': (itemtype, dt),
                         'path': type_keys[itemtype],
                         'values': [
                             itemtype,
                             summary,
                             flags,
                             rhc,
-                            id
+                            doc_id
                             ],
                     }
                     )
 
     rows.sort(key=itemgetter('sort'), reverse=False)
     rdict = NDict()
     for row in rows:
@@ -6032,70 +6475,82 @@
 def get_usedtime(db, pinned_list=[], link_list=[], konnect_list=[], timers={}):
     """
     All items with used entries grouped by month, index entry and day
 
     """
     UT_MIN = settings.get('usedtime_minutes', 1)
 
-    width = shutil.get_terminal_size()[0] - 2
+    width = shutil.get_terminal_size()[0] - 3
     summary_width = width - 21
 
     used_details = {}
     used_details2id = {}
     used_summary = {}
-
+    effort_details = {}
     month_rows = {}
     used_time = {}
     detail_rows = []
     months = set([])
     for item in db:
         used = item.get('u') # this will be a list of 'period, datetime' tuples
-        if not used:
+        if item['itemtype'] == '!' or not used:
             continue
         index = item.get('i', '~')
         id_used = {}
         index_tup = index.split('/')
-        id = item.doc_id
+        doc_id = item.doc_id
         itemtype = item['itemtype']
         summary = item['summary']
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
 
         for period, dt in used:
             if isinstance(dt, pendulum.Date) and not isinstance(dt, pendulum.DateTime):
                 dt = pendulum.parse(dt.format("YYYYMMDD"), tz='local')
                 dt.set(hour=23, minute=59, second=59)
-            # for id2used
-            if UT_MIN != 1:
-                res = period.minutes % UT_MIN
+
+            rhc_cols = 17 if UT_MIN == 0 else 14
+
+            if UT_MIN > 0:
+                seconds = period.remaining_seconds
+                if seconds:
+                    # round up to the next minute
+                    period = period + pendulum.duration(seconds = 60-seconds)
+                res = period.in_minutes() % UT_MIN
                 if res:
                     period += (UT_MIN - res) * ONEMIN
 
+            yr, wk, dayofweek = dt.isocalendar()
+            week = (yr, wk)
+            row = wkday2row(dayofweek)
+            effort_details.setdefault(week, {})
+            effort_details[week].setdefault(dayofweek, ZERO)
+            effort_details[week][dayofweek] += period
+
             monthday = dt.date()
             id_used.setdefault(monthday, ZERO)
             id_used[monthday] += period
-            # for used_time
             month = dt.format("YYYY-MM")
             used_time.setdefault(tuple((month,)), ZERO)
             used_time[tuple((month, ))] += period
             for i in range(len(index_tup)):
                 used_time.setdefault(tuple((month, *index_tup[:i+1])), ZERO)
                 used_time[tuple((month, *index_tup[:i+1]))] += period
         for monthday in id_used:
             month = monthday.format("YYYY-MM")
-            rhc = f"{monthday.format('M/DD')}: {format_hours_and_tenths(id_used[monthday])}".ljust(14, ' ')
+            rhc = f"{monthday.format('M/DD')} {format_hours_and_tenths(id_used[monthday])}".ljust(rhc_cols, ' ')
             detail_rows.append({
                         'sort': (month, index_tup, monthday, itemtype, summary),
                         'month': month,
                         'path': f"{monthday.format('MMMM YYYY')}/{index}",
                         'values': [
-                            itemtype,
-                            summary,
+                            '◦',
+                            f"{itemtype} {summary}",
                             flags,
                             rhc,
-                            id],
+                            doc_id],
                         })
 
     try:
         detail_rows.sort(key=itemgetter('sort'))
     except Exception as e:
         # report the components of sort other than the last, the summary
         logger.error(f"error sorting detail_rows: f{e}\nsort: {[x['sort'][:-1] for x in detail_rows]}")
@@ -6135,74 +6590,87 @@
             rhc = f"{format_hours_and_tenths(period)}"
             summary = f"{indent}{key[-1]}: {rhc}"[:summary_width].ljust(summary_width, ' ')
             month_rows[key[0]].append(f"{summary}")
 
     for key, val in month_rows.items():
         used_summary[key] = "\n".join(val)
 
-    return used_details, used_details2id, used_summary
+    return used_details, used_details2id, used_summary, effort_details
 
 
 def fmt_class(txt, cls=None, plain=False):
     if not plain and cls is not None:
         return cls, txt
     else:
         return txt
 
 
 def no_busy_periods(week, width):
-    ampm = settings['ampm']
-    LL = {}
-    for hour in range(24):
-        if hour % 6 == 0:
-            if ampm:
-                suffix = 'am' if hour < 12 else 'pm'
-                if hour == 0:
-                    hr = 12
-                elif hour <= 12:
-                    hr = hour
-                elif hour > 12:
-                    hr = hour - 12
-                LL[hour] = f"{hr}{suffix}".rjust(6, ' ')
-            else:
-                LL[hour] = f"{hour}h".rjust(6, ' ')
-        else:
-            LL[hour] = ' '.rjust(6, ' ')
 
+    # The weekday 2-char abbreviation and the month day
+    width = shutil.get_terminal_size()[0]
+    dent = int((width - 69)/2) * " "
     monday = pendulum_parse(f"{week[0]}-W{str(week[1]).zfill(2)}-1")
     DD = {}
+    for i in range(1, 8):
+        DD[i] = f"{WA[i]} {monday.add(days=i-1).format('D')}".ljust(5, ' ')
+
     h = {}
-    t = {0: 'total'.rjust(6, ' ')}
-    for i in range(7):
-        DD[i+1] = monday.add(days=i).format("D").ljust(2, ' ')
+    h[0] = '  '
+    h[58] = '  '
+    for i in range(1, 58):
+        h[i] = ' ' if (i-1) % 4 else VSEP
+    empty = "".join([h[i] for i in range(59)])
+    for i in range(1, 58):
+        h[i] = HSEP if (i-1) % 4 else VSEP
+    full = "".join([h[i] for i in range(59)])
+
+    empty_hsh = {}
+    wk_fmt = fmt_week(week).center(width, ' ').rstrip()
+    empty_hsh[0] = f"""\
+{wk_fmt}
 
+{dent}{8*' '}{HB}
+"""
     for weekday in range(1, 8):
-        t[weekday] = '0'.center(5, ' ')
+        empty_hsh[weekday] = f"""\
+{dent}{7*' '}{empty}
+{dent} {DD[weekday] : <6}{full}
+"""
+    return  "".join([empty_hsh[i] for i in range(0, 8)])
 
-    for hour in range(24):
-        h.setdefault(hour, {})
-        for weekday in range(1, 8):
-            h[hour][weekday] = '  .  '
-    return busy_template.format(week = 8 * ' ' + fmt_week(week).center(47, ' '), WA=WA, DD=DD, t=t, h=h, l=LL)
 
-def summary_pin(text, width, id, pinned_list, link_list, konnected_list):
+def summary_pin(text, width, doc_id, pinned_list, link_list, konnected_list):
     in_konnected = False
-    if id in konnected_list:
+    if doc_id in konnected_list:
         in_konnected = True
         text = (text[:width-3].rstrip() +  KONNECT_CHAR)
-    if id in link_list:
+    if doc_id in link_list:
         text = (text[:width-3].rstrip() +  LINK_CHAR)
-    if id in pinned_list:
+    if doc_id in pinned_list:
         ret = (text[:width-1] + PIN_CHAR).ljust(width-1, ' ')
     else:
         ret = text[:width].ljust(width, ' ')
     return ret
 
-
-def schedule(db, yw=getWeekNum(), current=[], now=pendulum.now(), weeks_before=0, weeks_after=0, pinned_list=[], link_list=[], konnect_list=[], timers={}):
+def wkday2row(wkday):
+    # week day number in 1, ..., 7 to row number in busy view
+    # 1 -> 5, ..., 6 -> 15, 0 -> 17  (pendulum thinks Sunday is first)
+    return 3+ 2*wkday if wkday else 17
+
+def schedule(db, yw=getWeekNum(), current=[], now=pendulum.now(), weeks_before=0, weeks_after=0, pinned_list=[], link_list=[], konnect_list=[], timers={}, mk_current=False):
+    wkday_fmt = "ddd D MMM" if settings['dayfirst'] else "ddd MMM D"
+    timer_schedule = TimeIt('***SCHEDULE***')
+    if mk_current:
+        weeks_after = settings['keep_current'][0]
+        width = settings['keep_current'][1]-1
+        compact = True
+    else:
+        width = shutil.get_terminal_size()[0]-3
+        compact = False
     ampm = settings['ampm']
     omit = settings['omit_extent']
     UT_MIN = settings.get('usedtime_minutes', 1)
     # yw will be the active week, but now will be the current moment
     LL = {}
     for hour in range(24):
         if hour % 6 == 0:
@@ -6216,134 +6684,209 @@
                     hr = hour - 12
                 LL[hour] = f"{hr}{suffix}".rjust(6, ' ')
             else:
                 LL[hour] = f"{hour}h".rjust(6, ' ')
         else:
             LL[hour] = ' '.rjust(6, ' ')
 
-    width = shutil.get_terminal_size()[0] - 2
     # xx:xxam-xx:xxpm
     rhc_width = 15 if ampm else 11
     flag_width = 6
     indent_to_summary = 6
-    summary_width = width - indent_to_summary - flag_width - rhc_width
+    if mk_current:
+        summary_width = width - indent_to_summary - rhc_width
+    else:
+        summary_width = width - indent_to_summary - flag_width - rhc_width
 
     d = iso_to_gregorian((yw[0], yw[1], 1))
     dt = pendulum.datetime(d.year, d.month, d.day, 0, 0, 0, tz='local')
     week_numbers = getWeekNumbers(dt, weeks_before, weeks_after)
     if yw not in week_numbers:
         week_numbers.append(yw)
         week_numbers.sort()
     aft_dt, bef_dt = get_period(dt, weeks_before, weeks_after)
 
+    # for the individual weeks
+    agenda_hsh = {}     # yw -> agenda_view
+    done_hsh = {}       # yw -> done_view
+    busy_hsh = {}       # yw -> busy_view
+    row2id_hsh = {}     # yw -> row2id
+    done2id_hsh = {}     # yw -> row2id
+    engaged_hsh = {}
+    engaged2id_hsh = {}     # yw -> row2id
+    week2day2engaged = {}   # year, week -> dayofweek -> period total for day
+    week2day2heading = {}
+    weeks = set([])
     rows = []
     done = []
-    busy = []
+    engaged = []
+    # busy = []
 
+    #XXX year, week -> dayofweek -> list of [time interval, summary, period]
+    busy_details = {}
+    week2day2busy = {}
+    week2day2allday = {}
+
+    #XXX main loop begins
+    todayYMD = now.format("YYYYMMDD")
+    tomorrowYMD = (now + 1*DAY).format("YYYYMMDD")
     for item in db:
         if item.get('itemtype', None) == None:
             logger.error(f"itemtype missing from {item}")
             continue
         if item['itemtype'] in "!?":
             continue
+
+        doc_id = item.doc_id
+        itemtype = item['itemtype']
         summary = item.get('summary', "~")
-        id = item.doc_id
-        flags = get_flags(id, link_list, konnect_list, pinned_list, timers)
-        if 'u' in item:
-            used = item.get('u') # this will be a list of @u entries
-            itemtype = item['itemtype']
+        start = item.get('s', None)
+        extent = item.get('e', None)
+        wraps = item.get('w', [])
+        flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
+        used = item.get('u', None)
+        finished = item.get('f', None)
+        history = item.get('h', None)
+        jobs = item.get('j', None)
+
+        if itemtype == "*" and start and extent and 'r' not in item:
+            dt = start
+            if (isinstance(dt, pendulum.Date) and not isinstance(dt, pendulum.DateTime)):
+                dt = pendulum.parse(dt.format("YYYYMMDD"), tz='local')
+                dt.set(hour=0, minute=0, second=1)
+
+        if used:
             dates_to_periods = {}
             for period, dt in used:
                 if isinstance(dt, pendulum.Date) and not isinstance(dt, pendulum.DateTime):
                     pass
                 else:
                     dt = dt.date()
-                if UT_MIN != 1:
-                    # round up minutes
-                    res = period.minutes % UT_MIN
-                    if res:
-                        period += (UT_MIN - res) * ONEMIN
+                if UT_MIN > 0:
+                    seconds = period.remaining_seconds
+                    if seconds:
+                        # round up minutes - consistent with used time views
+                        period = period + pendulum.duration(seconds = 60-seconds)
+
                 dates_to_periods.setdefault(dt, []).append(period)
             for dt in dates_to_periods:
+                week = dt.isocalendar()[:2]
+                weekday = dt.format(wkday_fmt)
+                week2day2engaged.setdefault(week, {})
+                week2day2engaged[week].setdefault(weekday, ZERO)
                 total = ZERO
                 for p in dates_to_periods[dt]:
                     total += p
-                rhc = format_hours_and_tenths(total).center(rhc_width, ' ')
-                done.append(
+                if total is not None:
+                    week2day2engaged[week][weekday] += total
+                    used = format_duration(total, short=True)
+                else:
+                    used = ''
+                engaged.append(
                         {
-                            'id': id,
+                            'id': doc_id,
                             'job': None,
                             'instance': None,
                             'sort': (dt.format("YYYYMMDD"), 1),
                             'week': (
-                                dt.isocalendar()[:2]
+                                week
                                 ),
                             'day': (
-                                dt.format("ddd MMM D"),
+                                weekday,
                                 ),
                             'columns': [
-                                itemtype,
-                                summary,
+                                USED,
+                                # '~',
+                                f'{used:<6} {itemtype} {summary}',
                                 flags,
-                                rhc,
-                                (id, None, None)
+                                '',
+                                (doc_id, None, None)
                             ],
                         }
                     )
 
-        if item['itemtype'] == '-':
-            d = []
-            if 'f' in item:
-                d.append([item['f'], summary, item.doc_id, None])
-            if 'h' in item:
-                for dt in item['h']:
-                    d.append([dt, summary, item.doc_id, None])
-            if 'j' in item:
-                for job in item['j']:
+
+        if itemtype == '-':
+            d = [] # d for done
+            if isinstance(finished, pendulum.Period):
+                # finished will be false if the period is ZERO
+                d.append([finished.start, summary, doc_id, format_date(finished.end)[1]])
+            if history:
+                for dt in history:
+                    d.append([dt.start, summary, doc_id, format_date(dt.end)[1]])
+            if jobs:
+                for job in jobs:
                     job_summary = job.get('summary', '')
                     if 'f' in job:
-                        d.append([job['f'], job_summary, item.doc_id, job['i']])
+                        # FIXME
+                        d.append([job['f'].start, job_summary, doc_id, job['i']])
             if d:
                 for row in d:
                     dt = row[0]
                     if isinstance(dt, pendulum.Date) and not isinstance(dt, pendulum.DateTime):
                         dt = pendulum.parse(dt.format("YYYYMMDD"), tz='local')
                         dt.set(hour=23, minute=59, second=59)
 
-                    rhc = ''
+                    rhc = str(row[3]) if len(row) > 3 else ""
                     if dt < aft_dt or dt > bef_dt:
                         continue
 
                     done.append(
                             {
                                 'id': row[2],
                                 'job': row[3],
                                 'instance': None,
                                 'sort': (dt.format("YYYYMMDDHHmm"), 1),
                                 'week': (
                                     dt.isocalendar()[:2]
                                     ),
                                 'day': (
-                                    dt.format("ddd MMM D"),
+                                    dt.format(wkday_fmt),
                                     ),
                                 'columns': [FINISHED_CHAR,
                                     row[1],
                                     flags,
                                     rhc,
                                     (row[2], None, row[3])
                                     ],
                             }
                             )
 
-        if 's' not in item or 'f' in item:
+        if not start or finished is not None:
             continue
 
-        # get the instances
+        # XXX INSTANCES
+
+        # keep these for reference for this item
+        end_dt = None
+
         for dt, et in item_instances(item, aft_dt, bef_dt):
-            start_dt = item['s']
+            yr, wk, dayofweek = dt.isocalendar()
+            week = (yr, wk)
+            wk_fmt = fmt_week(week).center(width, ' ').rstrip()
+            itemday = dt.format("YYYYMMDD")
+            dayDM = dt.format(wkday_fmt)
+            if itemday == todayYMD:
+                dayDM += " (Today)"
+            elif itemday == tomorrowYMD:
+                dayDM += " (Tomorrow)"
+            week2day2busy.setdefault(week, {})
+            week2day2busy[week].setdefault(dayofweek, [])
+            week2day2allday.setdefault(week, {})
+            week2day2allday[week].setdefault(dayofweek, [False, [f"{dayDM}", f"All day"]])
+
+            if item['itemtype'] == '*' and dt.hour == 0 and dt.minute == 0 and 'e' not in item:
+                week2day2allday[week][dayofweek][0] = True
+                if 'r' in item:
+                    freq = item['r'][0].get('r', 'y')
+                else:
+                    freq = 'y'
+                tmp_summary = set_summary(item['summary'], item['s'], dt, freq)
+                week2day2allday[week][dayofweek][1].append(f"{item['itemtype']} {tmp_summary}")
+
             if 'r' in item:
                 freq = item['r'][0].get('r', 'y')
             else:
                 freq = 'y'
             instance = dt if '+' in item or 'r' in item else None
             if 'j' in item:
                 for job in item['j']:
@@ -6353,242 +6896,401 @@
                     jobstart = dt - job.get('s', ZERO)
                     job_id = job.get('i', None)
                     job_sort = str(job_id)
 
                     rhc = fmt_time(dt).center(rhc_width, ' ')
                     rows.append(
                         {
-                            'id': item.doc_id,
+                            'id': doc_id,
                             'job': job_id,
                             'instance': instance,
                             'sort': (jobstart.format("YYYYMMDDHHmm"), job_sort),
                             'week': (
                                 jobstart.isocalendar()[:2]
                                 ),
+                            'week_fmt': (
+                                wk_fmt
+                                ),
+                            'dayofweek': (
+                                dayofweek
+                                ),
                             'day': (
-                                jobstart.format("ddd MMM D"),
+                                jobstart.format(wkday_fmt),
                                 ),
                             'columns': [job['status'],
-                                set_summary(job_summary, start_dt,  jobstart, freq),
+                                set_summary(job_summary, start,  jobstart, freq),
                                 flags,
                                 rhc,
-                                (item.doc_id, instance, job_id)
+                                (doc_id, instance, job_id)
                                 ]
                         }
                     )
 
             else:
-                if item['itemtype'] == '-':
-                    rhc = fmt_time(dt).center(rhc_width, ' ')
-                elif 'e' in item:
-                    if omit and 'c' in item and item['c'] in omit:
-                        et = None
-                        rhc = fmt_time(dt).center(rhc_width, ' ')
-                    else:
-                        rhc = fmt_extent(dt, et).center(rhc_width, ' ')
-                else:
-                    rhc = fmt_time(dt).center(rhc_width, ' ')
-
+                dateonly = False
                 sort_dt = dt.format("YYYYMMDDHHmm")
                 if sort_dt.endswith('0000'):
+                    dateonly = True
                     if item['itemtype'] == '*':
-                        sort_dt = sort_dt[:-4] + '$$$$'
+                        sort_dt = sort_dt[:-4] + '00$$'
                     elif item['itemtype'] in ['-']:
                         sort_dt = sort_dt[:-4] + '24$$'
                     elif item['itemtype'] in ['%']:
                         sort_dt = sort_dt[:-4] + '24%%'
 
+                if 'e' in item:
+                    if omit and 'c' in item and item['c'] in omit:
+                        et = None
+                        rhc = fmt_time(dt).center(rhc_width, ' ')
+                    else:
+                        if item['itemtype'] == '-' and dateonly:
+                            rhc = fmt_dur(item['e']).center(rhc_width, ' ')
+                        else:
+                            rhc = fmt_extent(dt, et).center(rhc_width, ' ')
+                else:
+                    rhc = fmt_time(dt).center(rhc_width, ' ')
+
+                dtb = dt
 
-                dtb = None
-                dta = None
+                dta = et if et else None
 
-                if item['itemtype'] == '*' and 'w' in item:
+                # temp - just for this item
+                wrap = []
+                before = after = {}
+                wrapped = ""
+                if 'w' in item and dta and dtb:
+                    # adjust for wrap
                     b, a = item['w']
-                    dtb = dt - b if b else None
-                    if dtb:
-                        itemtype = "↱"
-                        sort_b = dtb.format("YYYYMMDDHHmm")
-                        rhb = fmt_time(dtb).ljust(rhc_width, ' ')
-                        rows.append(
-                                {
-                                    'id': item.doc_id,
+                    if b:
+                        dtb -= b
+                    if a:
+                        dta += a
+                    wrapped = fmt_extent(dtb, dta).center(rhc_width, ' ')
+
+                    wrap = item['w']
+                    wraps = [format_duration(x) for x in wrap] if wrap else ""
+                    if wraps:
+                        wraps[0] = f"{wrapbefore}{wraps[0]}"
+                        wraps[1] = f"{wrapafter}{wraps[1]}"
+                        wrapper = f"\n{22*' '}+ {', '.join(wraps)}"
+                    else:
+                        wrapper = ""
+
+
+                    if b and b > ZERO:
+                        itemtype = wrapbefore #  "↱"
+                        sort_b = (dt-ONEMIN).format("YYYYMMDDHHmm")
+                        rhb = fmt_time(dtb).center(rhc_width, ' ')
+                        before = {
+                                    'id': doc_id,
                                     'job': None,
                                     'instance': instance,
-                                    'sort': (sort_dt, 0),
+                                    'sort': (sort_b, 0),
                                     'week': (
                                         dtb.isocalendar()[:2]
                                         ),
+                                    'dayofweek': (
+                                        dtb.isocalendar()[-1]
+                                        ),
                                     'day': (
-                                        dtb.format("ddd MMM D"),
+                                        dtb.format(wkday_fmt),
                                         ),
                                     'columns': [itemtype,
                                         set_summary("", item['s'], dtb, freq),
                                         " "*4,
                                         rhb,
-                                        (item.doc_id, instance, None)
+                                        (doc_id, instance, None)
                                         ]
                                 }
-                            )
 
-                rows.append(
-                        {
-                            'id': item.doc_id,
-                            'job': None,
-                            'instance': instance,
-                            'sort': (sort_dt, 0),
-                            'week': (
-                                dt.isocalendar()[:2]
-                                ),
-                            'day': (
-                                dt.format("ddd MMM D"),
-                                ),
-                            'columns': [item['itemtype'],
-                                set_summary(summary, item['s'], dt, freq),
-                                flags,
-                                rhc,
-                                (item.doc_id, instance, None)
-                                ]
-                        }
-                    )
-
-                if item['itemtype'] == '*' and 'w' in item:
-                    if 'e' in item:
-                        dta = dt + item['e'] + a if a else None
-                    else:
-                        dta = dt + a if a else None
-
-                    if dta:
-                        itemtype = "↳"
-                        sort_a = dta.format("YYYYMMDDHHmm")
-                        rha = fmt_time(dta).rjust(rhc_width, ' ')
-                        rows.append(
-                                {
-                                    'id': item.doc_id,
+                    if a and a > ZERO:
+                        itemtype = wrapafter  # "↳"
+                        sort_a = (dt+ONEMIN).format("YYYYMMDDHHmm")
+                        rha = fmt_time(dta).center(rhc_width, ' ')
+                        after = {
+                                    'id': doc_id,
                                     'job': None,
                                     'instance': instance,
                                     'sort': (sort_a, 0),
                                     'week': (
                                         dta.isocalendar()[:2]
                                         ),
+                                    'dayofweek': (
+                                        dta.isocalendar()[-1]
+                                        ),
                                     'day': (
-                                        dta.format("ddd MMM D"),
+                                        dta.format(wkday_fmt),
                                         ),
                                     'columns': [itemtype,
                                         set_summary("", item['s'], dta, freq),
                                         " "*4,
                                         rha,
-                                        (item.doc_id, instance, None)
+                                        (doc_id, instance, None)
                                         ]
                                 }
-                            )
-            if et:
-                beg_min = dtb.hour * 60 + dtb.minute if dtb else dt.hour * 60 + dt.minute
-                end_min = dta.hour * 60 + dta.minute if dta else et.hour * 60 + et.minute
-                y, w, d = dt.isocalendar()
-                #             x[0] x[1]  x[2]     x[3]
-                busy.append({'sort': dt.format("YYYYMMDDHHmm"), 'week': (y, w), 'day': d, 'period': (beg_min, end_min)})
+
+                else:
+                    wrapped = rhc
+
+                if before:
+                    rows.append(before)
+
+                if omit and 'c' in item and item['c'] in omit:
+                    busyperiod = None
+                elif dta and dta > dtb:
+                    # a for after, b for before
+                    busyperiod = None
+                    dtad = dta.date()
+                    dtbd = dtb.date()
+                    if dtad == dtbd:
+                        busyperiod = (dt2minutes(dtb), dt2minutes(dta))
+                        week2day2busy[week][dayofweek].append(busyperiod)
+                    elif dtad > dtbd:
+                        busyperiods = datetimes2busy(dta, dtb)
+                        for w, wd, periods in busyperiods:
+                            if w == week and wd == dayofweek:
+                                busyperiod = periods
+                                week2day2busy[week][dayofweek].append(busyperiod)
+                                break
+                else:
+                    busyperiod = None
+
+                tmp_summary = set_summary(summary, item['s'], dt, freq)
+
+                columns = [item['itemtype'],
+                                tmp_summary,
+                                flags,
+                                rhc,
+                                (doc_id, instance, None)
+                                ]
+
+                path = f"{wk_fmt}/{dayDM}**"
+
+                rows.append(
+                        {
+                            'id': doc_id,
+                            'job': None,
+                            'instance': instance,
+                            'sort': (sort_dt, 0),
+                            'week': (
+                                week
+                                ),
+                            'week_fmt': (
+                                wk_fmt
+                                ),
+                            'dayofweek': (
+                                dayofweek
+                                ),
+                            'day': (
+                                dt.format(wkday_fmt),
+                                ),
+                            'busyperiod': (
+                                busyperiod
+                                ),
+                            'wrap': (
+                                wrap
+                                ),
+                            'wrapped': wrapped,
+                            'columns': columns
+                        }
+                    )
+
+                if after:
+                    rows.append(after)
+
     if yw == getWeekNum(now):
         rows.extend(current)
     rows.sort(key=itemgetter('sort'))
     done.sort(key=itemgetter('sort'))
-    busy.sort(key=itemgetter('sort'))
+    engaged.sort(key=itemgetter('sort'))
 
-    # for the individual weeks
-    agenda_hsh = {}     # yw -> agenda_view
-    done_hsh = {}       # yw -> done_view
-    busy_hsh = {}       # yw -> busy_view
-    row2id_hsh = {}     # yw -> row2id
-    done2id_hsh = {}     # yw -> row2id
-    weeks = set([])
+    busy_details = {}
+    allday_details = {}
+    dent = int((width - 69)/2) * " "
+
+    ### item/agenda loop 2
+    today = now.format(wkday_fmt)
+    tomorrow = (now + 1*DAY).format(wkday_fmt)
 
-    for week, items in groupby(busy, key=itemgetter('week')):
+    for week in week2day2allday:
+        week2day2heading.setdefault(week, {})
         weeks.add(week)
-        busy_tups = []
-        for day, period in groupby(items, key=itemgetter('day')):
-            for p in period:
-                busy_tups.append([day, p['period']])
-        busy_tups.sort()
-        h = {}
-        busy = {}
-        t = {0: 'total'.rjust(6, ' ')}
+        allday_details.setdefault(week, {})
+        for dayofweek in week2day2allday[week]:
+            allday, lst = week2day2allday[week][dayofweek]
+            if allday and lst:
+                row = wkday2row(dayofweek)
+                week2day2heading[week][row] = lst.pop(0)
+                day_ = row
+                allday_details[week][row] = f"\n  ".join([f"{x}" for x in lst])
 
-        monday = pendulum_parse(f"{week[0]}-W{str(week[1]).zfill(2)}-1")
-        DD = {}
-        for i in range(7):
-            DD[i+1] = monday.add(days=i).format("D").ljust(2, ' ')
+    for week, items in groupby(rows, key=itemgetter('week')):
+        weeks.add(week)
+        week2day2heading.setdefault(week, {})
+        rdict = NDict(compact=compact)
+        busy_details.setdefault(week, {})
+        wk_fmt = fmt_week(week).center(width, ' ').rstrip()
+        for row in items:
+            doc_id = row['id']
+            day_ = row['day'][0]
+            dayofweek = row.get('dayofweek', 1)
+            if day_ == today:
+                day_ += " (Today)"
+            elif day_ == tomorrow:
+                day_ += " (Tomorrow)"
+            path = f"{wk_fmt}/{day_}"
+            values = row['columns']
+            # heading = f"Busy periods for {day_}"
+            if values[0] in ["*", "-"]:
+                values[1] = re.sub(' *\n+ *', ' ', values[1])
+                busyperiod = row.get('busyperiod', "")
+                if busyperiod:
+                    wrap = row.get('wrap', [])
+                    wrapped = row.get('wrapped', "")
+                    row = wkday2row(dayofweek)
+                    week2day2heading[week][row] = day_
+                    summary = values[1].ljust(width-20, ' ')
+                    busy_row = f"{values[0]} {summary} {wrapped:^15}".rstrip()
+                    if settings['connecting_dots']:
+                        busy_row = f"  {busy_row}".replace('   ', LINEDOT)
 
-        for weekday in range(1, 8):
-            t[weekday] = '0'.center(5, ' ')
+                    busy_details[week].setdefault(row, [f"Busy"]).append(
+                            busy_row
+                            )
 
-        for hour in range(24):
-            h.setdefault(hour, {})
-            for weekday in range(1, 8):
-                h[hour][weekday] = '  .  '
+            rdict.add(path, values)
 
-        for tup in busy_tups:
+        for d, v in busy_details[week].items():
+            busy_details[week][d] = "\n".join([x.rstrip() for x in v])
+
+
+        tree, row2id = rdict.as_tree(rdict, level=0)
+        agenda_hsh[week] = tree
+        row2id_hsh[week] = row2id
+
+    busyday_details = {}
+    for week in allday_details:
+        busyday_details.setdefault(week, {})
+        for day in allday_details[week]:
+            busyday_details[week].setdefault(day, []).append(allday_details[week][day])
+    for week in busy_details:
+        busyday_details.setdefault(week, {})
+        for day in busy_details[week]:
+            busyday_details[week].setdefault(day, []).append(busy_details[week][day].rstrip())
+
+    for week in busyday_details:
+        for row in busyday_details[week]:
+            lst = [week2day2heading[week].get(row, f"{week} {row}").center(width, ' ').rstrip(),]
+            lst += [x for x in busyday_details[week][row] if x.strip()]
+            busyday_details[week][row] = "\n".join(lst)
+
+
+    busy = {}
+    for week, dayhsh in week2day2busy.items():
+        busy_tuples = []
+        days = [d for d in dayhsh.keys()]
+        days.sort()
+        for day in days:
+            periods = dayhsh[day]
+            periods.sort()
+            busy_tuples.append([day, periods])
+
+        monday = pendulum_parse(f"{week[0]}-W{str(week[1]).zfill(2)}-1")
+        DD = {}
+        for i in range(1, 8):
+            DD[i] = f"{WA[i]} {monday.add(days=i-1).format('D')}".ljust(5, ' ')
+
+        for tup in busy_tuples:
             #                 d             (beg_min, end_min)
-            busy.setdefault(tup[0], []).append(tup[1])
+            busy[tup[0]] = tup[1]
+        wk_fmt = fmt_week(week).center(width, ' ').rstrip()
+        busy_hsh[0] = f"""\
+{wk_fmt}
+
+{dent}{8*' '}{HB}
+"""
         for weekday in range(1, 8):
             lofp = busy.get(weekday, [])
-            hours = busy_conf_day(lofp)
-            t[weekday] = str(hours['total']).center(5, ' ')
-            for hour in range(24):
-                if hour in hours:
-                    h[hour][weekday] = hours[hour]
-
-        busy_hsh[week] = busy_template.format(week = 8 * ' ' + fmt_week(week).center(47, ' '), WA=WA, DD=DD, t=t, h=h, l=LL)
+            alldayitems = ""
+            allday = False
+            if week in week2day2allday and weekday in week2day2allday[week]:
+                allday, lst = week2day2allday[week][weekday]
+
+            empty, full = busy_conf_day(lofp, allday)
+            busy_hsh[weekday] = f"""\
+{dent}{7*' '}{empty}
+{dent} {DD[weekday] : <6}{full}
+"""
+        busy_hsh[week] = "".join([busy_hsh[i] for i in range(0, 8)])
 
-    for week, items in groupby(rows, key=itemgetter('week')):
+    for week, items in groupby(done, key=itemgetter('week')):
         weeks.add(week)
         rdict = NDict()
-        wk_fmt = fmt_week(week).center(width, ' ')
-        today = now.format("ddd MMM D")
-        tomorrow = (now + 1*DAY).format("ddd MMM D")
+        wk_fmt = fmt_week(week).center(width, ' ').rstrip()
         for row in items:
-            day = row['day'][0]
-            if day == today:
-                day += " (Today)"
-            elif day == tomorrow:
-                day += " (Tomorrow)"
-            path = f"{wk_fmt}/{day}"
+            day_ = row['day'][0]
+            if day_ == today:
+                day_ += " (Today)"
+            elif day_ == tomorrow:
+                day_ += " (Tomorrow)"
+            path = f"{wk_fmt}/{day_}"
             values = row['columns']
             rdict.add(path, values)
         tree, row2id = rdict.as_tree(rdict, level=0)
-        agenda_hsh[week] = tree
-        row2id_hsh[week] = row2id
+        done_hsh[week] = tree
+        done2id_hsh[week] = row2id
 
-    for week, items in groupby(done, key=itemgetter('week')):
+    for week, items in groupby(engaged, key=itemgetter('week')):
         weeks.add(week)
         rdict = NDict()
-        wk_fmt = fmt_week(week).center(width, ' ')
-        today = now.format("ddd MMM D")
+        wk_fmt = fmt_week(week).center(width, ' ').rstrip()
         for row in items:
-            day = row['day'][0]
-            if day == today:
-                day += " (Today)"
-            path = f"{wk_fmt}/{day}"
+            day_ = row['day'][0]
+            total = (week2day2engaged[week][day_] if day_ in week2day2engaged[week] else ZERO).in_minutes()
+            used_fmt = bar_fmt = ""
+            if total:
+                used, bar = usedminutes2bar(total)
+                if usedtime_hours:
+                    bar_fmt = f"{bar.ljust(width-12, ' ')}"
+                    used_fmt = used.center(6, ' ')
+                else:
+                    bar_fmt = " "
+                    used_fmt = used
+            if day_ == today:
+                day_ += " (Today)"
+            elif day_ == tomorrow:
+                day_ += " (Tomorrow)"
+            path = f"{wk_fmt}/{day_}/{used_fmt} {bar_fmt}"
             values = row['columns']
             rdict.add(path, values)
         tree, row2id = rdict.as_tree(rdict, level=0)
-        done_hsh[week] = tree
-        done2id_hsh[week] = row2id
+        engaged_hsh[week] = tree
+        engaged2id_hsh[week] = row2id
+
 
     cache = {}
     for week in week_numbers:
         tup = []
         # agenda
         if week in agenda_hsh:
             tup.append(agenda_hsh[week])
         else:
-            tup.append("{}\n   Nothing scheduled".format(fmt_week(week).center(width, ' ')))
+            tup.append("{}\n   Nothing scheduled".format(fmt_week(week).center(width, ' ').rstrip()))
         # done
         if week in done_hsh:
             tup.append(done_hsh[week])
         else:
-            tup.append("{}\n   Nothing completed".format(fmt_week(week).center(width, ' ')))
+            tup.append("{}\n   Nothing completed".format(fmt_week(week).center(width, ' ').rstrip()))
+
+        # engaged
+        if week in engaged_hsh:
+            tup.append(engaged_hsh[week])
+        else:
+            tup.append("{}\n   No used times recorded".format(fmt_week(week).center(width, ' ').rstrip()))
+
         # busy
         if week in busy_hsh:
             tup.append(busy_hsh[week])
         else:
             tup.append(no_busy_periods(week, width))
         # row2id
         if week in row2id_hsh:
@@ -6596,26 +7298,41 @@
         else:
             tup.append({})
         # done2id
         if week in done2id_hsh:
             tup.append(done2id_hsh[week])
         else:
             tup.append({})
-        # agenda, done, busy, row2id, done2id
+        # engaged2id
+        if week in engaged2id_hsh:
+            tup.append(engaged2id_hsh[week])
+        else:
+            tup.append({})
+
+        if week in busyday_details:
+            tup.append(busyday_details[week])
+        else:
+            tup.append({})
+        # agenda, done, engaged, busy, row2id, done2id, engaged2id, busy_details
         cache[week] = tup
 
+    timer_schedule.stop()
     return cache
 
 
 def import_file(import_file=None):
     if not import_file:
         return False, ""
+    import_file = import_file.strip()
+    if import_file.lower() == 'lorem':
+        return True, import_examples()
+
     import_file = os.path.normpath(os.path.expanduser(import_file))
-    if not os.path.exists(import_file):
-        return False, f"could not locate: {import_file}"
+    if not os.path.isfile(import_file):
+        return False, f'"{import_file}"\n   either does not exist or is not a regular file'
     filename, extension = os.path.splitext(import_file)
     if extension == '.json':
         return True, import_json(import_file)
     elif extension == '.text':
         return True, import_text(import_file)
     elif extension == '.ics':
         return True, import_ics(import_file)
@@ -6662,14 +7379,53 @@
     if ids:
         msg += f"\n  ids: {ids[0]}-{ids[-1]}."
     if dups:
         msg += f"\n  rejected {dups} items as duplicates"
     return msg
 
 
+def import_examples():
+    docs = []
+    examples = make_examples()
+
+    results = []
+    good = []
+    bad = []
+    items = []
+
+    num_examples = len(examples)
+    count = 0
+    for s in examples:
+        ok = True
+        count += 1
+        if not s: continue
+        item = Item()  # use ETMDB by default
+        item.new_item()
+        item.text_changed(s, 1)
+        if item.item_hsh.get('itemtype', None) is None:
+            ok = False
+
+        if item.item_hsh.get('summary', None) is None:
+            ok = False
+
+        if ok:
+            item.update_item_hsh()
+            good.append(f"{item.doc_id}")
+        else:
+            bad.append(s)
+
+    res = f"imported {len(good)} items"
+    if good:
+        res += f"\n  ids: {good[0]} - {good[-1]}"
+    if bad:
+        res += f"\nrejected {bad} items:\n  "
+        res += "\n  ".join(results)
+    return res
+
+
 def import_text(import_file=None):
     docs = []
     with open(import_file, 'r') as fo:
         results = []
         good = []
         bad = 0
         reminders = []
@@ -6684,15 +7440,14 @@
                 reminder = [s]
             else:
                 # append to the existing reminder
                 reminder.append(s)
         if reminder:
             reminders.append(reminder)
     for reminder in reminders:
-        logger.debug(f"processing {reminder}")
         ok = True
         s = "\n".join(reminder)
         if not s: continue
         item = Item()  # use ETMDB by default
         item.new_item()
         item.text_changed(s, 1)
         if item.item_hsh.get('itemtype', None) is None:
@@ -6703,21 +7458,20 @@
 
         if not ok:
             bad += 1
             results.append(f"   {s}")
             continue
 
         # update_item_hsh stores the item in ETMDB
-        logger.debug(f"updating {item}")
         item.update_item_hsh()
         good.append(f"{item.doc_id}")
 
+
     res = f"imported {len(good)} items"
     if good:
-        # ids = ETMDB.insert_multiple(docs)
         res += f"\n  ids: {good[0]} - {good[-1]}"
     if bad:
         res += f"\nrejected {bad} items:\n  "
         res += "\n  ".join(results)
     return res
 
 
@@ -6737,22 +7491,21 @@
         summary = item_hsh.get('summary')
         if not summary:
             continue
         z = item_hsh.get('z', 'Factory')
         bad_keys = [x for x in item_hsh if not item_hsh[x]]
         for key in bad_keys:
             del item_hsh[key]
-        # z = item_hsh.get('z')
         if 's' in item_hsh:
             item_hsh['s'] = pen_from_fmt(item_hsh['s'], z)
         if 'f' in item_hsh:
-            item_hsh['f'] = pen_from_fmt(item_hsh['f'], z)
+            item_hsh['f'] = period_from_fmt(item_hsh['f'], z)
         item_hsh['created'] = pendulum.now('UTC')
         if 'h' in item_hsh:
-            item_hsh['h'] = [pen_from_fmt(x, z) for x in item_hsh['h']]
+            item_hsh['h'] = [period_from_fmt(x, z) for x in item_hsh['h']]
         if '+' in item_hsh:
             item_hsh['+'] = [pen_from_fmt(x, z) for x in item_hsh['+'] ]
         if '-' in item_hsh:
             item_hsh['-'] = [pen_from_fmt(x, z) for x in item_hsh['-'] ]
         if 'e' in item_hsh:
             item_hsh['e'] = parse_duration(item_hsh['e'])[1]
         if 'w' in item_hsh:
@@ -6842,24 +7595,22 @@
     new = []
     dups = 0
     for x in ETMDB:
         exst.append({
                     'itemtype': x.get('itemtype'),
                     'summary': x.get('summary'),
                     's': x.get('s'),
-                    # 'f': x.get('f')
                     })
     i = 0
     for x in docs:
         i += 1
         y = {
                     'itemtype': x.get('itemtype'),
                     'summary': x.get('summary'),
                     's': x.get('s'),
-                    # 'f': x.get('f')
                     }
         if exst and y in exst:
             dups += 1
         else:
             new.append(x)
 
     ids = []
```

### Comparing `etm-dgraham-4.9.7/etm/options.py` & `etm-dgraham-5.0.3/etm/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import string
 import random
 import re
 import locale
 from copy import deepcopy
 from prompt_toolkit.styles.named_colors import NAMED_COLORS
 import etm.__version__ as version
-etm_version = version.version
+etmversion = version.version
 
 locale_regex = re.compile(r'[a-z]{2}_[A-Z]{2}')
 
 def randomString(stringLength=10):
     """Generate a random string with the combination of lowercase and uppercase letters and digits """
 
     letters = string.ascii_letters + 2*'0123456789'
@@ -70,33 +70,39 @@
     default_type_colors = {
         'dark': {
             'available':    'LightSkyBlue',
             'begin':        'Gold',
             'event':        'LimeGreen',
             'finished':     'DarkGrey',
             'inbox':        'OrangeRed',
-            'journal':       'GoldenRod',
+            'journal':      'GoldenRod',
             'pastdue':      'LightSalmon',
             'plain':        'Ivory',
             'today':        'Ivory bold',
+            'used':         'Khaki',
             'waiting':      'SlateGrey',
             'wrap':         'ForestGreen',
+            'running':      'OrangeRed',
+            'paused':       'Gold',
             },
         'light': {
             'available':    'DarkBlue',
             'begin':        'DarkViolet',
             'event':        'Green',
             'finished':     'LightSlateGrey',
             'inbox':        'MediumVioletRed',
             'journal':      'Brown',
             'pastdue':      'Red',
             'plain':        'Black',
             'today':        'Black bold',
+            'used':         'DodgerBlue',
             'waiting':      'DarkSlateBlue',
             'wrap':         'LightGrey',
+            'running':      'MediumVioletRed',
+            'paused':       'DarkViolet',
             },
     }
 
     default_window_colors = {
         'dark': {
             'ask':                     ['grey2', 'Lime', 'bold'],
             'button.focused':          ['DarkGreen', 'White'],
@@ -150,103 +156,117 @@
             'text-area':               ['Cornsilk', 'Black'],
             'window.border shadow':    ['', '#444444'],
             'window.border':           ['', '#888888'],
             }
         }
 
     ampm = "true"
+    show_minutes = "false"
     yearfirst = "true"
     dayfirst = "false"
+    beginbusy = 7
     updates_interval = 0
     locale = "en_US"
     vi_mode = "false"
     secret = randomString(10)
     omit_extent = ""
-    keep_current = 0
+    keep_current = [0, 47]
     keep_next = "false"
     archive_after = 0
+    refresh_interval = 60
     num_finished = 0
     limit_skip_display = "true"
     connecting_dots = "false"
     usedtime_minutes = 1
+    usedtime_hours = 6
     alerts = ""
     expansions = ""
     sms = {"body": "{location} {when}", "from": "", "server": "", "pw": ""}
     smtp = {"body": "{location} {when}\n{description}", "from": "", "server": "", "id": "", "pw": ""}
     locations = ""
     queries = ""
     style = "dark"
     type_colors = ""
     window_colors = ""
+    journal_name = "daily"
 
     # use these to format the template
     settings_hsh = {
         "ampm" : ampm,
+        "show_minutes": show_minutes,
         "dayfirst" : dayfirst,
         "yearfirst" : yearfirst,
+        'beginbusy' : beginbusy,
         "updates_interval" : updates_interval,
         "locale" : locale,
         "vi_mode" : vi_mode,
         "secret" : secret,
         "omit_extent" : omit_extent,
         "keep_current" : keep_current,
         "keep_next" : keep_next,
         "archive_after" : archive_after,
+        "refresh_interval" : refresh_interval,
         "num_finished" : num_finished,
         "limit_skip_display" : limit_skip_display,
         "connecting_dots" : connecting_dots,
         "usedtime_minutes" : usedtime_minutes,
+        "usedtime_hours" : usedtime_hours,
         "alerts" : dict2yaml(alerts),
         "expansions" : dict2yaml(expansions),
         "sms": dict2yaml(sms),
         "smtp": dict2yaml(smtp),
         "locations": dict2yaml(locations),
         "queries": dict2yaml(queries),
         "style" : style,
         "type_colors" : dict2yaml(type_colors),        # user modifications only
         "window_colors" : dict2yaml(window_colors),    # user modifications only
-        "etmversion": etm_version
+        "journal_name": journal_name,
+        "etmversion": etmversion
 }
 
 
     template = """\
 #### begin cfg.yaml ####
-version: {etmversion}
+etmversion: {etmversion}
 # The current version of etm and this file. DO NOT EDIT. This is
 # automatically updated when a new version of etm is installed.
 
 ampm: {ampm}
 # true or false. Use AM/PM format for datetimes if true else
-# use 24 hour format.
+# use 24 hour format. See also the show_minutes setting.
+
+show_minutes: {show_minutes}
+# true or false. If true show ":00" in agenda and forthcoming views
+# when displaying times with zero minutes else suppress zero minutes
+# from being displayed. E.g., "9:00-10:30" if true else "9-10:30".
+# When ampm if false and show_minutes is true, hours will be displayed
+# with leading zeros applicable.
 
 dayfirst:  {dayfirst}
 yearfirst: {yearfirst}
 # each true or false. Whenever an ambiguous date is parsed, dayfirst
 # and yearfirst parameters control how the information is processed
 # using this precedence:
-#
-#   If dayfirst is False and yearfirst is False:
-#       MM-DD-YY
-#       DD-MM-YY
-#       YY-MM-DD
-#
-#   If dayfirst is True and yearfirst is False:
-#       DD-MM-YY
-#       MM-DD-YY
-#       YY-MM-DD
-#
-#   If dayfirst is False and yearfirst is True:
-#       YY-MM-DD
-#       MM-DD-YY
-#       DD-MM-YY
-#
-#   If dayfirst is True and yearfirst is True:
-#       YY-MM-DD
-#       DD-MM-YY
-#       MM-DD-YY
+# yearfirst: true
+# 	dayfirst: true  => YDM
+#   dayfirst: false => YMD
+# yearfirst: false
+# 	dayfirst: true  => DMY
+#   dayfirst: false => MDY
+# E.g., with both true, 3/4/5 would be interpreted as May 4, 2003.
+# When possible, dates will also be displayed respecting these settings.
+# I.e., the year will generally be displayed first when yearfirst is
+# true and last otherwise. Similarly, the day will generally be displayed
+# before the month when dayfirst is true and after the month otherwise.
+
+beginbusy: {beginbusy}
+# non-negative integer. The number of hours after midnight to begin the
+# busy view display of busy times for each day. The display continues
+# for 14 hours after the begin_busy hour. E.g. with 'begin_busy: 7' the
+# display would show busy times from 7am (7h) until 9pm (21h).
 
 updates_interval: {updates_interval}
 # non-negative integer. If positive,  automatically check for updates
 # every 'updates_interval' minutes. If zero, do not automatically
 # check for updates. When enabled, a blackboard u symbol, 𝕦, will be
 # displayed at the right end of status bar when an update is available
 # or a question mark when the check cannot be completed as, for
@@ -271,35 +291,42 @@
 
 omit_extent: {omit_extent}
 # A list of calendar names. Events with @c entries belonging to this
 # list will only have their starting times displayed in agenda view
 # and will neither appear nor cause conflicts in busy view.
 
 keep_current: {keep_current}
-# non-negative integer. If positive, the agenda for that integer
-# number of weeks starting with the current week will be written to
-# "current.txt" in your etm home directory and updated when necessary.
-# You could, for example, create a link to this file in a pCloud or
-# DropBox folder and have access to your current schedule on your
-# mobile device.
+# A list of two, non-negative integers for "weeks" and "width". If
+# weeks is positive, the agenda for that integer number of weeks
+# starting with the current week will be written to "current.txt" in
+# your etm home directory and updated when necessary. The format will
+# be scaled to fit "width". A width of 50, e.g, fits an iPhone display
+# in portrait mode. You could, for example, create a link to
+# "current.txt" in a pCloud or GoogleDrive folder and always have access
+# to your current agenda on your mobile device.
 
 keep_next: {keep_next}
 # true or false. If true, the 'do next' view will be written to
 # "next.txt" in your etm home directory. As with "current.txt", a link
 # to this file could be created in a pCloud or DropBox folder for
 # access from your mobile device.
 
 archive_after: {archive_after}
 # non-negative integer. If zero, do not archive items. If positive,
 # finished tasks and events with last datetimes falling more than this
 # number of years before the current date will automatically be
 # archived on a daily basis.  Archived items are moved from the
 # "items" table in the database to the "archive" table and will no
 # longer appear in normal views. Note that unfinished tasks and
-# records are not archived.
+# journal entries are not archived.
+
+refresh_interval: {refresh_interval}
+# 6, 12, 30 or 60. The event loop responsible for refreshing
+# etm caches, updating alerts, timers and so forth, repeats once
+# every refresh_interval seconds.
 
 num_finished: {num_finished}
 # non-negative integer
 # If positive, when saving retain only the most recent
 # "num_finished" completions of an infinitely repeating task,
 # i.e., repeating without an "&c" count or an "&u" until
 # attribute. If zero or not infinitely repeating, save all
@@ -314,34 +341,61 @@
 # current time.
 
 connecting_dots: {connecting_dots}
 # true or false. If true, display dots connecting the item summary and
 # the right-hand details columns in tree views.
 
 usedtime_minutes: {usedtime_minutes}
-# 1, 6, 12, 30 or 60. Round used times up to the nearest
-# usedtime_minutes in used time views. With 1, no rounding is done and
-# times are reported as hours and minutes. Otherwise, the prescribed
-# rounding is done and times are reported as floating point hours.
-# Note that each "@u" timeperiod is rounded before aggregation.
+# 0, 1, 6, 12, 30 or 60. Round up used times. With 0, no rounding is done
+# and times are reported in hours, minutes and seconds. With 1, after
+# rounding up to the nearest minute, times are reported as hours and minutes.
+# Otherwise, rounding is up to the nearest integer multiple of
+# usedtime_minutes and times are reported as floating point hours. E.g.,
+# with usedtime_minutes = 6, 1 minute would be rounded up to 6 minutes and
+# reported as 0.1 hours. Similarly 13 minutes would be rounded up to 18
+# minutes and reported as 0.3 hours. The numbers 6, 12, 30 and 60 are
+# characterized by the fact that each is an integer multiple of 6 and 60 is
+# evenly divisible by each. This allows reported times to be expressed as
+# hours and tenths of an hour for each. Note that when rounding is specified,
+# each "@u" timeperiod is rounded before aggregation. Whatever the setting,
+# a used time record created using the timer is accurate to the nearest
+# second.
+
+usedtime_hours: {usedtime_hours}
+# 0, 1, 2, ..., 24. The daily goal for used time. This is used in engaged
+# view to control the display of the daily used time bars. The goal is to
+# to maximize the granularity of the bar when displaying this number of hours
+# in the space allowed by the terminal width.
+
+journal_name: {journal_name}
+# Journal items with this index entry and with an @s entry will have the
+# year and month appended to the index. E.g., with the setting
+#   journal_name: daily
+# this journal entry
+#   % visited Yellowstone @s 22/6/24 @i daily
+# would be displayed in journal view as if the index entry were
+#   @i daily/2022/ 6
+# thus organizing such entries by the year and month of their scheduled dates.
+# Within each month, entries will be also ordered by the month day.
 
 alerts: {alerts}
 # A dictionary with single-character, "alert" keys and corresponding
 # "system command" values. Note that characters "t" (text message) and
 # "e" (email) are already used.  The "system command" string should be
 # a comand with any applicable arguments that could be run in a
 # terminal. Properties of the item triggering the alert can be
 # included in the command arguments using the syntax {{prop}}, e.g.,
 # {{summary}} in the command string would be replaced by the summary of
-# the item. Similarly {{start}} by the starting time, {{when}} by the time
-# remaining until the starting time, {{location}} by the @l entry and
-# {{description}} by the @d entry. E.g., If the event "* sales meeting
-# @s 2019-02-12 3p" triggered an alert 30 minutes before the starting
-# time the string "{{summary}} {{when}}" would expand to "sales meeting in
-# 30 minutes". E.g. on my macbook
+# the item. Similarly {{start}} by the starting datetime, {{time}} by the
+# starting time (omits the date for the current date), {{when}} by the time
+# remaining until the starting datetime, {{now}} by the current time,
+# {{location}} by the @l entry and {{description}} by the @d entry. E.g., If
+# the event "* sales meeting @s 2019-02-12 3p" triggered an alert 30 minutes
+# before the starting time the string "{{summary}} {{when}}" would expand to
+# "sales meeting in 30 minutes". E.g. on my macbook
 #
 #    alerts:
 #        v:   /usr/bin/say -v "Alex" "{{summary}}, {{when}}"
 #        ...
 #
 # would make the alert 'v' use the builtin text to speech sytem
 # to speak the item's summary followed by a slight pause
@@ -410,14 +464,18 @@
 # values. Each "query" must be one that could be entered as the
 # command in query view. Keys can be any short string other than
 # 'a', 'u', 'c' or 'l' which are already in use.
 # queries:
 #    td: m l -q equals itemtype - and ~exists f
 #    mi: exists u and ~exists i
 #    arch: a exists itemtype
+#    find: includes summary d {{}}
+# The latter would allow you to enter, e.g., `find waldo` and have
+# it expand to `includes summary d waldo` and thus locate all
+# reminders with `waldo` either in the summary or d (the description).
 
 style: {style}
 # dark or light. Set the defaults for dark or light terminal
 # backgounds. Some output may not be visible unless this is set
 # correctly for your display.
 
 type_colors: {type_colors}
@@ -432,30 +490,35 @@
 #  event           'LimeGreen',        'DarkGreen',
 #  finished        'DarkGrey',         'LightSlateGrey',
 #  inbox           'OrangeRed',        'MediumVioletRed',
 #  journal         'GoldenRod',        'Brown',
 #  pastdue         'LightSalmon',      'Red',
 #  plain           'Ivory',            'Black',
 #  today           'Ivory bold',       'Black bold',
+#  used            'Khaki',            'DodgerBlue',
 #  waiting         'SlateGrey',        'DarkSlateBlue',
 #  wrap            'ForestGreen',      'LightGrey',
-#
+#  running         'OrangeRed',        'Gold',
+#  paused          'MediumVioletRed',   'DarkViolet',
 # Explanations for the key names:
 #     available:    available task/job reminders
 #     begin:        begin by warnings
 #     event:        event reminders
 #     finished:     finished task/job reminders
 #     inbox:        inbox reminders
 #     journal:      journal reminders
 #     pastdue:      pasdue task warnings
 #     plain:        headings such as outline branches
 #     today:        the current and following agenda date headings
+#     used:         used time rows in engaged and used time views
 #     waiting:      waiting job reminders (jobs with unfinished prereqs)
 #     wrap:         before and after rows for events in agenda view with
 #                   @w entries
+#     running:      status bar color for 'r', running timer
+#     paused:       status bar color for 'p', paused timer
 #
 # E.g., with style 'dark', the default color for 'available' is
 # 'LightSkyBlue'. This entry
 #   colors:
 #       available: CornFlowerBlue
 # would change the 'available' color to 'CornflowerBlue' while leaving
 # the other 'dark' colors unchanged.
@@ -505,15 +568,15 @@
 #
 # Note that 'grey1' (#396060) and 'grey2' (#1d3030) are colors named
 # within etm itself. They are, respectively, one shade lighter and two
 # shades darker than DarkSlateGrey.
 #
 # Any of the style attributes above can be modified. E.g., with style
 # 'dark', the default for 'text-area' is [grey2, Ivory]. This entry
-#   style_modifications:
+#   window_colors:
 #       text-area: [Black, White]
 # would change the 'text-area' setting to 'Black' as the background color
 # and 'White' as the foreground color while leaving the other style settings
 # unchanged.
 #### end cfg.yaml ####\
 """
 
@@ -523,19 +586,19 @@
         self.settings = {}
         default_template = Settings.template.format(**Settings.settings_hsh)
         self.settings.update(self.settings_hsh)
         # self.settings = yaml_nort.load(default_template) # uses RoundTripLoader (comments)
         # yaml = YAML(typ='safe', pure=True)
         # load defaults
         active_style = self.settings_hsh['style']
-        logger.debug(f"default style: {active_style}")
+        # logger.debug(f"default style: {active_style}")
         default_type_colors = self.default_type_colors[active_style]
-        logger.debug(f"default type_colors: {default_type_colors}")
+        # logger.debug(f"default type_colors: {default_type_colors}")
         default_window_colors = self.default_window_colors[active_style]
-        logger.debug(f"default window_colors: {default_window_colors}")
+        # logger.debug(f"default window_colors: {default_window_colors}")
         # override the settings_hsh values for type_colors and window_colors so that
         # settings will have all the possible keys
         self.settings['type_colors'] = default_type_colors
         self.settings['window_colors'] = default_window_colors
         self.cfgfile = os.path.normpath(
                 os.path.join(etmdir, 'cfg.yaml'))
         if os.path.exists(self.cfgfile):
@@ -553,42 +616,43 @@
             else:
                 self.user = {}
         else:
             self.user = {}
 
         if self.user:
             # we have user settings that need to be checked
-            logger.debug("calling check_options")
+            # logger.debug("calling check_options")
             self.changes = self.check_options()
         else:
             # we need to populate cfg.yaml
             self.changes = None
             with open(self.cfgfile, 'w') as fn:
                 fn.writelines(default_template)
 
         if self.changes:
             updated_template = Settings.template.format(**self.settings_hsh)
             with open(self.cfgfile, 'w') as fn:
                 fn.writelines(updated_template)
-            logger.info(f"updated {self.cfgfile}: {', '.join(self.changes)}")
+            changes = "\n    - ".join(self.changes)
+            logger.info(f"updated {self.cfgfile}:\n    - {changes}")
         else:
             logger.info(f"using settings from {self.cfgfile}")
 
 
     def check_options(self):
         changed = []
         new = deepcopy(self.user)
         active_style = new.get('style', self.settings_hsh['style'])
         if active_style not in ['dark', 'light']:
             active_style = self.settings_hsh['style']
-        logger.debug(f"active style: {active_style}")
+        # logger.debug(f"active style: {active_style}")
         self.settings['type_colors'] = self.default_type_colors[active_style]
-        logger.debug(f"active type_colors: {self.settings['type_colors']}")
+        # logger.debug(f"active type_colors: {self.settings['type_colors']}")
         self.settings['window_colors'] = self.default_window_colors[active_style]
-        logger.debug(f"active window_colors: {self.settings['window_colors']}")
+        # logger.debug(f"active window_colors: {self.settings['window_colors']}")
 
         cfg = deepcopy(self.settings_hsh)
         # add missing default keys
         for key, value in self.settings_hsh.items():
             if key in ["colors", "type_colors", "window_colors"]:
                 continue
             if isinstance(self.settings_hsh[key], dict):
@@ -599,23 +663,26 @@
                     for k, v in self.settings_hsh[key].items():
                         if k not in new[key]:
                             new[key][k] = self.settings_hsh[key][k]
                             changed.append(f"retaining default {key}.{k}: {self.settings_hsh[key][k]}")
             elif key not in new:
                 new[key] = self.settings_hsh[key]
                 changed.append(f"retaining default {key}: {self.settings_hsh[key]}")
+        if "etmversion" not in new or new["etmversion"] != etmversion:
+            new['etmversion'] = etmversion
+            changed.append(f"set etmversion {etmversion}")
         # remove invalid user keys/values
         tmp = deepcopy(new) # avoid modifying ordered_dict during iteration
         for key in tmp:
-            # if key in ["summary", "prop", "start", "when", "location", "description", "etm_version"]:
+            # if key in ["summary", "prop", "start", "when", "location", "description", "etmversion"]:
             #     continue
             if key not in self.settings_hsh:
                 # not a valid option
                 del new[key]
-                changed.append(f"removed {key}: {self.user[key]}")
+                changed.append(f"removed {key}: {self.user[key]} - not in settings_hsh")
             elif key in ['type_colors', 'window_colors']:
                 # only allow the specified subfields for these keys
                 ks = tmp[key] or []
                 for k in ks:
                     if k not in self.settings[key]:
                         changed.append(f"removed {key}.{k}: {new[key][k]}")
                         del new[key][k]
@@ -657,39 +724,50 @@
             if deleted:
                 new['window_colors'] = tmp
 
             if new['window_colors']:
                 self.settings_hsh['window_colors'] = dict2yaml(new['window_colors'])
                 self.settings['window_colors'].update(new['window_colors'])
 
+        if 'keep_current' in new and not isinstance(new['keep_current'], list):
+            if isinstance(new['keep_current'], int):
+                weeks = new['keep_current']
+            elif isinstance(new['keep_current'], bool):
+                weeks = 3 if new['keep_current'] else 0
+            else:
+                weeks = 0
+            changed.append(f"Converting 'keep_current' from {new['keep_current']} to [{weeks}, 50]")
+            new['keep_current'] = [weeks, 50]
 
         if not locale_regex.match(new['locale']):
             tmp = new['locale']
             new['locale'] = self.settings['locale']
             changed.append(f"retaining default for 'locale': {self.settings['locale']}. The provided setting, {tmp}, does have the required format.")
 
 
         if not isinstance(new['updates_interval'], int) or new['updates_interval'] < 0:
             new['updates_interval'] = self.settings['updates_interval']
             changed.append(f"retaining default for 'updates_interval': {self.settings['updates_interval']}")
 
-        if new['usedtime_minutes'] not in [1, 6, 12, 30, 60]:
+        if new['refresh_interval'] not in [6, 12, 30, 60]:
+            changed.append(f"{new['usedtime_minutes']} is invalid for usedtime_minute. Using default value: 60.")
+            new['refresh_interval'] = 60
+        if new['usedtime_minutes'] not in [0, 1, 6, 12, 30, 60]:
             changed.append(f"{new['usedtime_minutes']} is invalid for usedtime_minute. Using default value: 1.")
             new['usedtime_minutes'] = 1
+        if new['usedtime_hours'] not in [x for x in range(0, 25)]:
+            changed.append(f"{new['usedtime_hours']} is invalid for usedtime_minute. Using default value: 6.")
+            new['usedtime_hours'] = 6
         if  new['style'] not in ['dark', 'light']:
             new['style'] = self.settings['style']
             changed.append(f"retaining default for 'style': {self.settings['style']}")
         if  not isinstance(new['vi_mode'], bool):
             new['vi_mode'] = self.settings['vi_mode']
             changed.append(f"retaining default for 'vi_mode': {self.settings['vi_mode']}")
 
-        if isinstance(new['keep_current'], bool):
-            new['keep_current'] = 3 if new['keep_current'] else 0
-            changed.append(f"Converting 'keep_current' from boolian to integer {new['keep_current']}")
-
         for key in self.settings_hsh:
             if key in ['type_colors', 'window_colors']:
                 # already processed these
                 continue
             new_value = new.get(key, '')
             if new_value is not None and new_value != self.settings_hsh.get(key, ''):
                 tmp = self.settings_hsh[key]
```

### Comparing `etm-dgraham-4.9.7/etm/report.py` & `etm-dgraham-5.0.3/etm/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 def maybe_round(obj):
     """
     round up to the nearest UT_MIN minutes.
     """
     if not isinstance(obj, pendulum.Duration):
         return None
     try:
-        if UT_MIN == 1:
+        if UT_MIN <= 1:
             return obj
         minutes = 0
         if obj.weeks:
             minutes += obj.weeks * 7 * 24 * 60
         if obj.remaining_days:
             minutes += obj.remaining_days * 24 * 60
         if obj.hours:
```

### Comparing `etm-dgraham-4.9.7/etm/view.py` & `etm-dgraham-5.0.3/etm/view.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,43 +29,44 @@
 from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.layout.controls import BufferControl
 from prompt_toolkit.layout import Dimension
 from prompt_toolkit.widgets import HorizontalLine
 from prompt_toolkit.layout.menus import CompletionsMenu
 from prompt_toolkit.key_binding.bindings.focus import focus_next, focus_previous
 from prompt_toolkit.layout import Float
-from prompt_toolkit.widgets import Dialog, Label, Button
+from prompt_toolkit.widgets import Box, Dialog, Label, Button
+from packaging.version import parse as parse_version
 
 import shutil
+from shlex import split as qsplit
+import time
 
 import requests
 import asyncio
 
 import pendulum
 from pendulum import parse as pendulum_parse
 def parse(s, **kwd):
     return pendulum_parse(s, strict=False, **kwd)
 
-
 import re
-
 import subprocess # for check_output
 
 # for openWithDefault
 import platform
 import os
+import contextlib, io
 
 import pyperclip
 # set in __main__
 logger = None
 
 dataview = None
 item = None
 style = None
-type_colors = None
 application = None
 
 ############ begin query ###############################
 from tinydb import where
 from tinydb import Query
 from pygments.lexer import RegexLexer
 from pygments.token import Keyword
@@ -82,14 +83,15 @@
 
     def set_status(self, new):
         self.status = new
 
     def get_status(self):
         return self.status
 
+
 class TDBLexer(RegexLexer):
 
     name = 'TDB'
     aliases = ['tdb']
     filenames = '*.*'
     flags = re.MULTILINE | re.DOTALL
 
@@ -98,14 +100,15 @@
                 (r'\b(begins|includes|in|equals|more|less|exists|any|all|one)\b', Keyword),
                 (r'\b(replace|remove|archive|delete|set|provide|attach|detach)\b', Keyword),
                 (r'\b(itemtype|summary)\b', Literal),
                 (r'\b(and|or|info)\b', Keyword),
                 ],
             }
 
+
 def format_week(dt, fmt="WWW"):
     """
     """
     if fmt == "W":
         return dt.week_of_year
     if fmt == "WW":
         return dt.strftime("%W")
@@ -158,15 +161,15 @@
                 'attach': self.attach,      # a, b
                 'detach': self.detach,      # a, b
                 }
 
         self.changed = False
 
         self.lexer = PygmentsLexer(TDBLexer)
-        self.style = type_colors
+        # self.style = type_colors
         self.Item = Query()
 
         self.allowed_commands = ", ".join([x for x in self.filters])
 
 
     def replace(self, a, rgx, rep, items):
         """
@@ -459,15 +462,15 @@
         if not isinstance(b, list):
             b = [b]
         return where(a).one_of(b)
 
     def info(self, a):
         # field 'a' exists
         item = dataview.db.get(doc_id=int(a))
-        return  f"{item_details(item, False)}"
+        return  item if item else f"doc_id {a} not found"
 
 
     def dt(self, a, b):
         if b[0]  == '?':
             if b[1] == 'time':
                 return self.Item[a].test(self.is_datetime)
             elif b[1] == 'date':
@@ -542,15 +545,14 @@
             openWithDefault(query_help)
             return False, "opened query help using default browser"
         try:
             ok, test, updt = self.process_query(query)
             if not ok:
                 return False, test
             if isinstance(test, str):
-                # info
                 return False, test
             else:
                 items = dataview.db.search(test)
                 if updt:
                     self.update[updt[0]](*updt[1:], items)
                     if self.changed:
                         loop = asyncio.get_event_loop()
@@ -621,44 +623,55 @@
 
         def accept_text(buf):
             get_app().layout.focus(ok_button)
             buf.complete_state = None
             return True
 
         def accept():
+            self.set_label('\nworking ...\n')
+            get_app().invalidate()
+            time.sleep(.1)
             self.future.set_result(self.text_area.text)
 
         def cancel():
             self.future.set_result(None)
 
         self.text_area = TextArea(
             completer=completer,
             text=default,
             style='class:dialog-entry',
             multiline=False,
             width=D(preferred=shutil.get_terminal_size()[0]-padding),
             accept_handler=accept_text)
 
+        self.label = Label(
+                text=label_text
+                )
+
         ok_button = Button(text='OK', handler=accept)
         cancel_button = Button(text='Cancel', handler=cancel)
 
         self.dialog = Dialog(
             title=title,
             body=HSplit([
-                Label(text=label_text),
+                self.label,
                 self.text_area
             ]),
             buttons=[ok_button, cancel_button],
             # buttons=[ok_button],
             width=D(preferred=shutil.get_terminal_size()[0]-10),
             modal=True)
 
+    def set_label(self, txt):
+        self.label.text = txt
+
     def __pt_container__(self):
         return self.dialog
 
+
 class RadioListDialog(object):
     def __init__(self, title='', text='', label='', values=[], padding=4, completer=None):
         self.future = asyncio.Future()
 
         self.radios = RadioList(values=values)
         # radios.current_value will contain the first component of the selected tuple
         # title = "Delete"
@@ -681,15 +694,14 @@
 
         self.dialog = Dialog(
             title=title,
             body=HSplit([
                 Label(text=text),
                 Frame(title=label, body=self.radios)
             ]),
-            # body= Frame(title=label, body=self.radios),
             buttons=[ok_button, cancel_button],
             width=D(preferred=shutil.get_terminal_size()[0]-10),
             modal=True)
 
     def __pt_container__(self):
         return self.dialog
 
@@ -783,15 +795,14 @@
 
     return result
 
 
 # Key bindings.
 bindings = KeyBindings()
 
-
 @bindings.add('f2')
 def do_about(*event):
     show_message('etm information', about(2)[0], 0)
 
 @bindings.add('f4')
 def do_check_updates(*event):
     status, res = check_update()
@@ -809,15 +820,18 @@
         # split(' ')[-1] will give "'4.7.2'" and url_version will then be '4.7.2'
     except:
         url_version = None
     if url_version is None:
         res = "update information is unavailable"
         status_char = "?"
     else:
-        if url_version > etm_version:
+        # kluge for purely numeric versions
+        # if [int(x) for x in url_version.split('.')] > [int(x) for x in etm_version.split('.')]:
+        # from packaging.version parse
+        if parse_version(url_version) > parse_version(etm_version):
             status_char = UPDATE_CHAR
             res = f"an update is available to {url_version}"
         else:
             status_char = ''
             res = f"the installed version, {etm_version}, is the latest available"
 
     return status_char, res
@@ -906,29 +920,31 @@
             'i': "inactive",
             'r': "running",
             'p': "paused",
             }
 
     now = pendulum.now('local')
     if doc_id in dataview.timers:
+        title = 'active timer - record used time and end timer'
         state, start, elapsed = dataview.timers[doc_id]
         if state == 'r':
             elapsed += now - start
             start = now
         timer = f"\ntimer:\n  status: {state2fmt[state]}\n  last change: {format_datetime(start, short=True)[1]}\n  elapsed time: {format_duration(elapsed, short=True)}"
         entry = f"{format_duration(elapsed, short=True)}: {format_datetime(start, short=True)[1]}"
     else:
+        title = 'no active timer - add used time entry'
         state = None
         timer = "\ntimer: None"
         entry = " : now"
 
     def coroutine():
         dialog = TextInputDialog(
-            title='add usedtime',
-            label_text=f"selected:\n  {hsh['itemtype']} {hsh['summary']}\n  @i {hsh.get('i', '~')}{timer}\n\nadd usedtime using the format:\n    period: datetime\n",
+            title=title,
+            label_text=f"selected:\n  {hsh['itemtype']} {hsh['summary']}\n  @i {hsh.get('i', '~')}{timer}\n\nused time format:\n    period: datetime\n",
             default=entry,
             )
         usedtime = yield from show_dialog_as_float(dialog)
 
         if not usedtime:
             # None (cancelled) or null string
             return
@@ -941,15 +957,15 @@
             if doc_id in dataview.itemcache:
                 del dataview.itemcache[doc_id]
             application.layout.focus(text_area)
             set_text(dataview.show_active_view())
             loop = asyncio.get_event_loop()
             loop.call_later(0, data_changed, loop)
         else:
-            show_message('add usedtime', f"Cancelled, '{usedtime}' is invalid.\nThe required entry format is:\n   used timeperiod: ending datetime")
+            show_message('add used time', f"Cancelled, '{usedtime}' is invalid.\nThe required entry format is:\n   period: datetime")
 
 
     asyncio.ensure_future(coroutine())
 
 
 today = pendulum.today()
 calyear = today.year
@@ -1004,15 +1020,15 @@
             focus_previous(event)
         else:
             event.app.layout.focus(root_container.window)
 
 
 @Condition
 def is_item_view():
-    return dataview.active_view in ['agenda', 'completed', 'history', 'index', 'tags', 'journal', 'do next', 'used time', 'relevant', 'forthcoming', 'query', 'pinned', 'review', 'konnected', 'timers', 'location']
+    return dataview.active_view in ['agenda', 'completed', 'engaged', 'history', 'index', 'tags', 'journal', 'do next', 'used time', 'relevant', 'forthcoming', 'query', 'pinned', 'review', 'konnected', 'timers', 'location']
 
 @Condition
 def is_dated_view():
     return dataview.active_view in ['agenda', 'completed', 'busy'] and get_app().layout.has_focus(text_area)
 
 @Condition
 def is_editing():
@@ -1023,20 +1039,24 @@
     return not dataview.is_editing
 
 @Condition
 def is_not_searching():
     return not application.layout.is_searching
 
 @Condition
+def is_busy_view():
+    return dataview.active_view == 'busy'
+
+@Condition
 def is_not_busy_view():
     return dataview.active_view != 'busy'
 
 @Condition
 def is_agenda_view():
-    return dataview.active_view in ['agenda', 'busy', 'completed']
+    return dataview.active_view in ['agenda', 'busy', 'completed', 'engaged']
 
 @Condition
 def is_used_view():
     return dataview.active_view in ['used time', 'used summary']
 
 @Condition
 def is_query_view():
@@ -1129,62 +1149,29 @@
         fg = f"{grey_colors[fg]}"
     else:
         # foreground colors from NAMED_COLORS if possible
         fg = f"{NAMED_COLORS.get(fg, fg)}" if fg else ""
     return f"{bg} {fg} {attr}".rstrip()
 
 
-# color_dict = {
-#         'ask':                     (['grey2', 'Lime', 'bold'],          ['Cornsilk', 'Lime', 'bold']),
-#         'button.focused':          (['DarkGreen', 'White'],             ['DarkGreen', 'White']),
-#         'details':                 (['', 'Ivory'],                      ['', 'Black']),
-#         'dialog shadow':           (['#444444', ''],                    ['#444444', '']),
-#         'dialog':                  (['DarkSlateGrey', 'White'],         ['DimGrey', 'White']),
-#         'dialog-entry':            (['White', 'Black'],                 ['White', 'Black']),
-#         'dialog-output':           (['DarkSlateGrey', 'Lime'],          ['DimGrey', 'Lime']),
-#         'dialog.body label':       (['', 'White'],                      ['', 'White']),
-#         'dialog.body':             (['DarkSlateGrey', 'White'],         ['DimGrey', 'White']),
-#         'entry':                   (['grey2', 'LightGoldenRodYellow'],  ['Cornsilk', 'LightGoldenRodYellow']),
-#         'frame.label':             (['DarkSlateGrey', 'White'],         ['DimGrey', 'White']),
-#         'menu':                    (['DarkSlateGrey', 'White'],         ['DimGrey', 'White']),
-#         'menu-bar':                (['grey1', 'White'],                 ['grey1', 'White']),
-#         'menu-bar.selected-item':  (['#ffffff', '#000000'],             ['#ffffff', '#000000']),
-#         'menu.border':             (['', '#aaaaaa'],                    ['', '#aaaaaa']),
-#         'not-searching':           (['', '#222222'],                    ['', '#777777']),
-#         'query':                   (['', 'Ivory'],                      ['', 'Black']),
-#         'reply':                   (['grey2', 'DeepSkyBlue'],           ['Cornsilk', 'DeepSkyBlue']),
-#         'shadow':                  (['#222222', ''],                    ['#222222', '']),
-#         'status':                  (['grey1', 'White'],                 ['grey1', 'White']),
-#         'status.key':              (['', '#ffaa00'],                    ['', '#ffaa00']),
-#         'status.position':         (['', '#aaaa00'],                    ['', '#aaaa00']),
-#         'text-area':               (['grey2', 'Ivory'],                 ['Cornsilk', 'Black']),
-#         'window.border shadow':    (['', '#444444'],                    ['', '#444444']),
-#         'window.border':           (['', '#888888'],                    ['', '#888888']),
-#         }
-
-
 def get_style(style_dict):
-    # col = 0 if style == 'dark' else 1
-    # style_dict = {k: v[col] for k, v in color_dict.items()}
-    # style_dict = dark_dict if style == 'dark' else light_dict
-    # if settings['window_colors']:
-    #     style_dict.update(settings['style_modifications'])
     window_colors = {k: get_colors(*v) for k, v in style_dict.items()}
     return Style.from_dict(window_colors)
 
 type2style = {
         '!': 'inbox',
         '<': 'pastdue',
         '>': 'begin',
         '%': 'journal',
         '*': 'event',
         '-': 'available',
         '+': 'waiting',
         '✓': 'finished',
         '~': 'missing',
+        '◦': 'used',
         '↱': 'wrap',
         '↳': 'wrap',
         }
 
 def first_char(s):
     """
     Return the first non-whitespace character in s.
@@ -1197,41 +1184,51 @@
         return s[len(m.group(0))]
     else:
         # no leading spaces
         return None
 
 # Create one text buffer for the main content.
 class ETMLexer(Lexer):
+
     def lex_document(self, document):
 
         def get_line(lineno):
             tmp = document.lines[lineno]
             typ = first_char(tmp)
             if typ in type2style:
                 sty = type2style[typ]
                 if sty in type_colors:
                     return [(type_colors[sty], tmp)]
                 else:
+                    logger.debug(f"problem with typ {typ} from {tmp}")
                     logger.debug(f"sty: {sty}; type_colors.keys: {type_colors.keys()}")
             if tmp.rstrip().endswith("(Today)") or tmp.rstrip().endswith("(Tomorrow)"):
                 return [(type_colors['today'], f"{tmp} ")]
-            return [(type_colors['plain'], tmp)]
-            # return [(type_colors[type2style.get(typ, 'plain')], tmp)]
+
+            return [
+                (busy_colors.get(c, type_colors['plain']), c)
+                for i, c in enumerate(document.lines[lineno])
+            ]
+
 
         return get_line
 
+
 def status_time(dt):
     """
     >>> status_time(parse('2018-03-07 10am'))
     '10am Wed Mar 7'
     >>> status_time(parse('2018-03-07 2:45pm'))
     '2:45pm Wed Mar 7'
     """
     ampm = settings['ampm']
-    d_fmt = dt.format("ddd MMM D")
+    if settings['dayfirst']:
+        d_fmt = dt.format("ddd D MMM")
+    else:
+        d_fmt = dt.format("ddd MMM D")
     suffix = dt.format("A").lower() if ampm else ""
     if dt.minute == 0:
         t_fmt = dt.format("h") if ampm else dt.format("H")
     else:
         t_fmt = dt.format("h:mm") if ampm else dt.format("H:mm")
     return f"{t_fmt}{suffix} {d_fmt}"
 
@@ -1241,65 +1238,79 @@
             and item.doc_id not in dataview.timers):
         if dataview.active_timer:
             state = 'i'
         else:
             state = 'r'
             dataview.active_timer = item.doc_id
         dataview.timers[item.doc_id] = [state, pendulum.now('local'), pendulum.Duration()]
-    # dataview.update_completions(item)
     dataview.get_completions()
     dataview.update_konnections(item)
     data_changed(loop)
 
 def data_changed(loop):
     dataview.refreshRelevant()
     dataview.refreshAgenda()
     set_text(dataview.show_active_view())
     dataview.refreshCurrent()
     if dataview.current_row:
         text_area.buffer.cursor_position = text_area.buffer.document.translate_row_col_to_index(dataview.current_row, 0)
     get_app().invalidate()
 
 async def new_day(loop):
-    dataview.refreshRelevant()
-    dataview.activeYrWk = dataview.currentYrWk
+    logger.debug("XXX new day XXX")
+    dataview.currYrWk()
+    dataview.refreshRelevant()  # sets now, currentYrWk, current
     dataview.refreshAgenda()
     dataview.refreshCurrent()
-    dataview.currcal()
     dataview.set_active_view('a')
     set_text(dataview.show_active_view())
+    dataview.currcal()
     get_app().invalidate()
     dataview.handle_backups()
     dataview.possible_archive()
     logger.info(f"new_day currentYrWk: {dataview.currentYrWk}")
     return True
 
 current_datetime = pendulum.now('local')
 
 async def save_timers():
     dataview.save_timers()
     return True
 
 def alerts():
-    alerts = []
+    # alerts = []
+    alert_hsh = {}
     now = pendulum.now('local')
+    #            0            1         2          3         4       5
+    # alerts: alert time, start time, commands, itemtype, summary, doc_id
     for alert in dataview.alerts:
         trigger_time = pendulum.instance(alert[0])
         start_time = pendulum.instance(alert[1])
         if start_time.date() == now.date():
             start = format_time(start_time)[1]
         else:
             start = format_datetime(start_time, short=True)[1]
         trigger = format_time(trigger_time)[1]
         command = ", ".join(alert[2])
-        summary = alert[3]
-        prefix = '#' if trigger_time < now else ' '
-        alerts.append(f"{prefix} {trigger} ({command}) {summary} {start}")
+        itemtype = alert[3]
+        summary = alert[4]
+        doc_id = alert[5]
+        prefix = '✓' if trigger_time < now else '•' # '⧖'
+        alert_hsh.setdefault((alert[5], itemtype, summary), []).append([prefix, trigger, start, command])
     if alerts:
-        return "\n".join(alerts)
+        output = []
+        for key, values in alert_hsh.items():
+            output.append(f"{key[1]} {key[2]}")
+            for value in values:
+                output.append(f"  {value[0]} {value[1]:>7} ⭢  {value[2]:>7}:  {value[3]}")
+        output.append('')
+        output.append('✓ already activated')
+        output.append('• not yet activated')
+        return "\n".join(output)
+
     else:
         return "There are no alerts for today."
 
 def get_row_col():
     row_number = text_area.document.cursor_position_row
     col_number = text_area.document.cursor_position_col
     return row_number, col_number
@@ -1307,20 +1318,19 @@
 def restore_row_col(row_number, col_number):
     text_area.buffer.cursor_position = \
                     text_area.buffer.document.translate_row_col_to_index(row_number, col_number)
 
 
 
 async def maybe_alerts(now):
-    global current_datetime
+    # global current_datetime
     row, col = get_row_col()
-    dataview.refreshRelevant()
-    dataview.refreshAgenda()
     set_text(dataview.show_active_view())
-    dataview.refreshCurrent()
+    #            0            1         2          3         4       5
+    # alerts: alert time, start time, commands, itemtype, summary, doc_id
     restore_row_col(row, col)
     if dataview.alerts and not ('alerts' in settings and settings['alerts']):
         logger.warning("alerts have not been configured")
         return
     bad = []
     for alert in dataview.alerts:
         if alert[0].hour == now.hour and alert[0].minute == now.minute:
@@ -1336,67 +1346,74 @@
             if startdt > alertdt:
                 when = f"in {(startdt-alertdt).in_words()}"
             elif startdt == alertdt:
                 when = f"now"
             else:
                 when = f"{(alertdt-startdt).in_words()} ago"
             start = format_datetime(startdt)[1]
-            summary = alert[3]
-            doc_id = alert[4]
+            time = format_time(startdt)[1] if startdt.date() == today.date() else format_datetime(startdt, short=True)[1]
+            summary = alert[4]
+            doc_id = alert[5]
             command_list = alert[2]
             item = dataview.db.get(doc_id=doc_id)
             location = item.get('l', '')
             description = item.get('d', '')
             if 'e' in command_list:
                 command_list.remove('e')
                 dataview.send_mail(doc_id)
             if 't' in command_list:
                 command_list.remove('t')
                 dataview.send_text(doc_id)
-            commands = [settings['alerts'][x].format(start=start, when=when, summary=summary, location=location, description=description) for x in command_list if x in settings['alerts']]
+            commands = [settings['alerts'][x].format(start=start, time=time, when=when, now=format_time(now)[1], summary=summary, location=location, description=description) for x in command_list if x in settings['alerts']]
             for command in commands:
                 if command:
                     check_output(command)
             if len(commands) < len(command_list):
                 bad.extend([x for x in command_list if x not in settings['alerts']])
 
     if bad:
         logger.error(f"unrecognized alert commands: {bad}")
-        # show_message(f"unrecognized alert commands", f"{bad}", 0)
 
 
 async def event_handler():
     global current_datetime
+    logger.debug(f"current_datetime: {current_datetime}")
     # check for updates every interval minutes
     interval = settings.get('updates_interval', 0)
+    refresh_interval = settings.get('refresh_interval', 60)
     minutes = 0
     try:
         while True:
-            now = pendulum.now()
-            current_today = dataview.now.format("YYYYMMDD")
-            asyncio.ensure_future(maybe_alerts(now))
+            now = pendulum.now('local')
             current_datetime = status_time(now)
-            today = now.format("YYYYMMDD")
-            wait = 60 - now.second
-            if interval:
-                if minutes == 0:
-                    minutes = 1
+            wait = refresh_interval - now.second % refresh_interval # residual
+            if now.second < 6:
+                current_today = dataview.now.format("YYYYMMDD")
+                asyncio.ensure_future(maybe_alerts(now))
+                current_datetime = status_time(now)
+                today = now.format("YYYYMMDD")
+
+                if interval:
+                    if minutes == 0:
+                        minutes = 1
+                        loop = asyncio.get_event_loop()
+                        asyncio.ensure_future(auto_check_loop(loop))
+                    else:
+                        minutes += 1
+                        minutes = minutes % interval
+
+                if today != current_today:
                     loop = asyncio.get_event_loop()
-                    asyncio.ensure_future(auto_check_loop(loop))
-                else:
-                    minutes += 1
-                    minutes = minutes % interval
+                    asyncio.ensure_future(new_day(loop))
 
-            if today != current_today:
-                loop = asyncio.get_event_loop()
-                asyncio.ensure_future(new_day(loop))
+            asyncio.ensure_future(save_timers())
             if dataview.active_view == 'timers':
+                row, col = get_row_col()
                 set_text(dataview.show_active_view())
-            asyncio.ensure_future(save_timers())
-            logger.debug(f"sleeping for {wait} seconds in event_handler loop")
+                restore_row_col(row, col)
             get_app().invalidate()
             await asyncio.sleep(wait)
     except asyncio.CancelledError:
         logger.info(f"Background task cancelled.")
 
 
 def get_edit_mode():
@@ -1440,73 +1457,87 @@
     return [ ('class:status',  f' {current_datetime}'), ]
 
 def get_statusbar_center_text():
     if dataview.is_editing:
         return [ ('class:status',  f' {get_edit_mode()}'), ]
     if dataview.is_showing_query:
         return [ ('class:status',  f' {dataview.query_mode}'), ]
+    if loglevel == 1:
+        # show current row number and associated id in the status bar
+        current_row = text_area.document.cursor_position_row
+        current_id = dataview.row2id.get(current_row, '~')
+        if isinstance(current_id, tuple):
+            current_id = current_id[0]
+        return [ ('class:status',  f'{current_row}: {current_id}'), ]
+
     return [ ('class:status',  14 * ' '), ]
 
 
 def get_statusbar_right_text():
     inbasket = INBASKET_CHAR if os.path.exists(inbasket_file) else ""
-    return [ ('class:status',  f"{dataview.timer_report()}{dataview.active_view} {inbasket}{update_status.get_status()}"), ]
+    active, inactive = dataview.timer_report()
+    if active:
+        active_part = (type_colors['running'], active) if active.startswith('r') else (type_colors['paused'], active)
+        inactive_part = ('class:status', f"{inactive}  ")
+    else:
+        active_part = inactive_part = ('class:status', "")
+
+    return [ active_part, inactive_part,  ('class:status',  f"{dataview.active_view} {inbasket}{update_status.get_status()}"), ]
 
 def openWithDefault(path):
-    parts = [x.strip() for x in path.split(" ")]
-    if len(parts) > 1:
-        logger.debug(f"path: {path}")
-        res =subprocess.Popen([parts[0], ' '.join(parts[1:])], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-        ok = True if res else False
+    if " " in path:
+        parts = qsplit(path)
+        logger.debug(f"path: {path}\n    Popen args: {parts}")
+        if parts:
+            # wrapper to catch 'Exception Ignored' messages
+            output = io.StringIO()
+            with contextlib.redirect_stderr(output):
+                # the pid business is evidently needed to avoid waiting
+                pid = subprocess.Popen(parts, stdin=subprocess.DEVNULL, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL).pid
+                res = output.getvalue()
+                if res:
+                    logger.error(f"caught by contextlib:\n'{res}'")
+
+
     else:
         path = os.path.normpath(os.path.expanduser(path))
         logger.debug(f"path: {path}")
         sys_platform = platform.system()
         if platform.system() == 'Darwin':       # macOS
-            res = subprocess.run(('open', path), stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+            subprocess.run(('open', path), stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         elif platform.system() == 'Windows':    # Windows
-            res = os.startfile(path)
+            os.startfile(path)
         else:                                   # linux
-            res = subprocess.run(('xdg-open', path), stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+            subprocess.run(('xdg-open', path), stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
-        # res = subprocess.run([cmd, path], check=True)
-        ret_code = res.returncode
-        ok = ret_code == 0
-        logger.debug(f"res: {res}; ret_code: {ret_code}")
-    if ok:
-        logger.debug(f"ok True; res: '{res}'")
-    else:
-        logger.debug(f"ok False; res: '{res}'")
-        show_message('goto', f"failed to open '{path}'")
     return
 
 search_field = SearchToolbar(text_if_not_searching=[
     ('class:not-searching', "Press '/' to start searching.")], ignore_case=True)
 
 content = ""
+etmlexer = ETMLexer()
 text_area = TextArea(
     text="",
     read_only=True,
     scrollbar=True,
     search_field=search_field,
     focus_on_click=True,
-    lexer=ETMLexer()
+    lexer=etmlexer,
     )
 
-
 # expansions will come from cfg.yaml
 expansions = {
         }
 
 
 class AtCompleter(Completer):
     # pat = re.compile(r'@[cgilntxz]\s?\S*')
     pat = re.compile(r'@[cgiklntxz]\s?[^@&]*')
 
-
     def get_completions(self, document, complete_event):
         cur_line = document.current_line_before_cursor
         matches = re.findall(AtCompleter.pat, cur_line)
         word = matches[-1] if matches else ""
         if word:
             word_len = len(word)
             word = word.rstrip()
@@ -1539,16 +1570,14 @@
 
 edit_bindings = KeyBindings()
 ask_buffer = Buffer()
 entry_buffer = Buffer(multiline=True, completer=at_completer, complete_while_typing=True, accept_handler=process_input)
 
 reply_buffer = Buffer(multiline=True)
 
-# reply_dimension = 2
-# entry_dimension = 10
 reply_dimension = Dimension(min=1, weight=1)
 entry_dimension = Dimension(min=2, weight=3)
 
 entry_window = Window(BufferControl(buffer=entry_buffer, focusable=True, focus_on_click=True, key_bindings=edit_bindings), height=entry_dimension, wrap_lines=True, style='class:entry')
 ask_window = Window(BufferControl(buffer=ask_buffer, focusable=False), height=1, style='class:ask')
 reply_window = Window(BufferControl(buffer=reply_buffer, focusable=False), height=reply_dimension, wrap_lines=True, style='class:reply')
 
@@ -1563,14 +1592,59 @@
 details_area = TextArea(
     text="",
     style='class:details',
     read_only=True,
     search_field=search_field,
     )
 
+
+busy_area = TextArea(
+    text="",
+    style='class:details',
+    read_only=True,
+    search_field=search_field,
+    )
+
+
+width = shutil.get_terminal_size()[0] - 4
+
+def get_busy_text():
+    return get_busy_text_and_keys(0)
+
+def get_busy_keys():
+    return get_busy_text_and_keys(1)
+
+def get_busy_text_and_keys(n):
+
+    weekdays = {
+            5:  f"1→{WA[1]}",
+            7:  f"2→{WA[2]}",
+            9:  f"3→{WA[3]}",
+            11: f"4→{WA[4]}",
+            13: f"5→{WA[5]}",
+            15: f"6→{WA[6]}",
+            17: f"7→{WA[7]}",
+            }
+    busy_details = dataview.busy_details
+    active_days = "  ".join([v for k, v in weekdays.items() if k in busy_details.keys()])
+    no_busy_times = "There are no days with busy periods this week.".center(width, ' ')
+    busy_times = wrap(f"Press the number of a weekday, [{weekdays[5]}, ..., {weekdays[17]}], to show the details of the busy periods from that day or press the ▼ (down) or ▲ (up) cursor keys to show the details of the next or previous day with busy periods.", indent=0)
+    active_keys = f"{active_days}  ▼→next  ▲→previous".center(width, ' ')
+
+    if n == 0: # text
+        return busy_times if dataview.busy_details else ""
+    else: # n=1, keys
+        return active_keys if dataview.busy_details else no_busy_times
+
+
+busy_container = HSplit([
+    busy_area,
+    Window(FormattedTextControl(get_busy_keys), style='class:status', height=1),
+    ], style='class:entry')
+
 query_bindings = KeyBindings()
 
 @query_bindings.add('enter', filter=is_querying)
 def accept(buff):
     set_text('processing query ...')
     if query_window.text:
         text = query_window.text
@@ -1585,27 +1659,25 @@
 Enter <key> at the prompt and press 'enter' to
 replace <key> with <query>. Submit this query as
 is or edit it first and then submit.
 
   """ + query_str
 
             show_message('query information', tmp)
-            # set_text(tmp)
             return False
         if text.strip() in ['quit', 'exit']:
             # quitting
             dataview.active_view = dataview.prior_view
             application.layout.focus(text_area)
             set_text(dataview.show_active_view())
             return False
         parts = [x.strip() for x in text.split(' ')]
         if queries and parts[0] in queries:
             set_text("")
             text = queries[parts.pop(0)]
-            # if '{}' in text:
             m =  re.search('{\d*}', text)
             if m:
                 # make the substitutions
                 num_needed = text.count('{}')
                 num_given = len(parts)
                 if num_needed and num_given != num_needed:
                     tmp = f"""\
@@ -1613,27 +1685,24 @@
     {text}
 needs {num_needed} argument(s) to replace the '{{}}' but
 {num_given} were actually provided:
     {", ".join(parts)}
 Please correct and resubmit.
                             """
                     show_message('query error', tmp)
-                    # set_text(tmp)
                     return False
                 try:
                     text = text.format(*parts)
-                    # text = text.replace('\s', ' ')
                     query_window.text = text
                 except IndexError as e:
                     tmp = f"""\
 Error processing {text}:
 {e}
 """
                     show_message('query error', tmp)
-                    # set_text(tmp)
                     return True
             else:
                 query_window.text = text
                 # don't reset the query area buffer we just set
                 return True
 
         loop = asyncio.get_event_loop()
@@ -1648,16 +1717,14 @@
 
     return False
 
 
 query = ETMQuery()
 
 query_buffer = Buffer(multiline=False, completer=None, complete_while_typing=False, accept_handler=accept)
-# query_window = Window(BufferControl(buffer=query_buffer, focusable=True, focus_on_click=True, key_bindings=edit_bindings), height=reply_dimension, wrap_lines=True, style='class:query')
-
 
 
 query_window = TextArea(
     style='class:query',
     lexer=query.lexer,
     multiline=False,
     focusable=True,
@@ -1669,14 +1736,15 @@
 query_window.accept_handler = accept
 
 query_area = HSplit([
     ask_window,
     query_window,
     ], style='class:entry')
 
+
 def do_complex_query(text, loop):
     text, *updt = [x.strip() for x in text.split(' | ')]
     updt = f" | {updt[0]}" if updt else ""
     if text.startswith('a '):
         text = text[2:]
         dataview.use_archive()
         item.use_archive()
@@ -1715,25 +1783,26 @@
     ])
 
 def default_buffer_changed(_):
     """
     """
     item.text_changed(entry_buffer.text, entry_buffer.cursor_position)
 
+
 def default_cursor_position_changed(_):
     """
     """
     item.cursor_changed(entry_buffer.cursor_position)
     set_askreply('_')
 
+
 # This is slick - add a call to default_buffer_changed
 entry_buffer.on_text_changed += default_buffer_changed
 entry_buffer.on_cursor_position_changed += default_cursor_position_changed
 
-
 status_area = VSplit([
             Window(FormattedTextControl(get_statusbar_text), style='class:status'),
             Window(FormattedTextControl(get_statusbar_center_text),
                    style='class:status', width=14, align=WindowAlign.CENTER),
             Window(FormattedTextControl(get_statusbar_right_text),
                    style='class:status', width=26, align=WindowAlign.RIGHT),
         ], height=1)
@@ -1742,14 +1811,17 @@
 body = HSplit([
     text_area,      # main content
     status_area,    # toolbar
     ConditionalContainer(
         content=details_area,
         filter=is_showing_details & is_not_busy_view),
     ConditionalContainer(
+        content=busy_container,
+        filter=is_busy_view),
+    ConditionalContainer(
         content=query_area,
         filter=is_querying),
     ConditionalContainer(
         content=edit_container,
         filter=is_editing),
     search_field,
     ])
@@ -1805,16 +1877,14 @@
     if instance is None and 's' in hsh:
         instance = hsh['s']
 
     is_date = (isinstance(instance, pendulum.Date) and not isinstance(instance, pendulum.DateTime))
 
     date_required = is_date or (instance.hour == 0 and instance.minute == 0)
 
-    # instance = pendulum.instance(instance)
-
     instance = instance.date() if date_required and not is_date else instance
     new = "new date" if date_required else "new datetime"
 
     def coroutine():
         dialog = TextInputDialog(
             title='reschedule instance',
             label_text=f"selected: {hsh['itemtype']} {hsh['summary']}\ninstance: {format_datetime(instance)[1]}\n\n{new}:")
@@ -2047,49 +2117,143 @@
     else:
         show_message('Update last-modified', "Update last-modified failed")
 
 
 @bindings.add('F', filter=is_viewing_or_details & is_item_view)
 def do_finish(*event):
 
-    ok, show, item_id, job_id, due = dataview.maybe_finish(text_area.document.cursor_position_row)
-    ampm = settings['ampm']
-    fmt = "ddd M/D h:mmA" if ampm else "ddd M/D H:mm"
-
-    if not ok:
+    doc_id, instance, job = dataview.get_row_details(text_area.document.cursor_position_row)
+    if not doc_id:
         return
 
-    def coroutine():
+    logger.debug(f"doc_id: {doc_id}; instance: {instance}; job: {job}")
+
+    hsh = DBITEM.get(doc_id=doc_id)
+    has_timer = doc_id in dataview.timers
+    timer_warning = " and\nits associated timer" if has_timer else ""
+    repeating = 'r' in hsh or '+' in hsh
+
+    between = []
+    due = ""
+
+    title = "Finish"
+    if instance:
+        need = 2
+        between = [hsh['s'], instance]
+        values = [
+            f"{format_datetime(hsh['s'])[1]} (oldest)",
+            f"{format_datetime(instance)[1]} (selected)",
+            ]
+
+        values_list = []
+        count = -1
+        for x in values:
+            count += 1
+            values_list.append(f"    {count}: {x}")
+
+        values_str = "\n".join(values_list)
+
+        text= f"""\
+Selected: {hsh['itemtype']} {hsh['summary']}
+
+{values_str}
+
+The number of the instance to finish and
+the completion datetime to use?
+number : datetime\
+        """
+        entry = "1 : now"
+        due = ""
+
+
+    elif repeating:
+        already_done = [x.end for x in hsh.get('h', [])]
+        need = 2
+        between = [x[0] for x in model.item_instances(hsh, hsh['s'], pendulum.now().replace(hour=0, minute=0, second=0, microsecond=0)) if x[0] not in already_done]
+        logger.debug(f"between: {between}")
+        values_list = []
+        # values.append( (0, format_datetime(between[0][0])[1]) )
+        count = -1
+        for x in between:
+            count += 1
+            values_list.append(f"   {count}: {format_datetime(x)[1]}")
 
+        values_str = "\n".join(values_list)
+
+        text= f"""\
+Selected: {hsh['itemtype']} {hsh['summary']}
+
+{values_str}
+
+The number of the instance to finish and
+the completion datetime to use?
+number : datetime\
+        """
+
+        entry = "0 : now"
+        due = ""
+
+    else:
+        need = 1
+        between = [hsh.get('s', None)]
+        entry =  "now"
+        due = hsh.get('s', "")
+        start = f"\nDue: {format_datetime(hsh['s'])[1]}" if 's' in hsh else ""
+
+        text= f"""\
+Selected: {hsh['itemtype']} {hsh['summary']}{start}
+
+Enter <completion datetime>
+        """
+
+    def coroutine():
+        global hsh
         dialog = TextInputDialog(
-            title='finish task/job',
-            label_text=f"selected: {show}\ndatetime completed:",
-            default='now'
+            title=title,
+            label_text=text,
+            default=entry,
             )
-
         done_str = yield from show_dialog_as_float(dialog)
-        if done_str:
-            try:
-                # done = parse_datetime(done_str, tz='local')
-                done = parse_datetime(done_str, z='local')[1]
 
-                ok = True
-            except:
-                ok = False
-            if ok:
-                # valid done
-                res = item.finish_item(item_id, job_id, done, due)
-                # dataview.itemcache[item.doc_id] = {}
-                if res:
-                    if item_id in dataview.itemcache:
-                        del dataview.itemcache[item_id]
-                    loop = asyncio.get_event_loop()
-                    loop.call_later(0, data_changed, loop)
-            else:
-                show_message('Finish task/job?', f"Invalid finished datetime: {done_str}")
+        if not done_str:
+            # None (cancelled) or null string
+            return
+
+        done_parts = [x.strip() for x in done_str.split(':')]
+
+        num_parts = len(done_parts)
+        if num_parts != need:
+            show_message('finish 1', f"Cancelled, {done_str} is invalid")
+            return
+
+        elif num_parts == 2:
+            num = int(done_parts[0])
+            # only return due for instance other than the oldest
+            # due = between[num] if num else ""
+            due = between[num]
+            done = parse_datetime(done_parts[1], z='local')[1]
+        elif num_parts == 1:
+            done = parse_datetime(done_str, z='local')[1]
+            due = between[0] if between[0] else done
+
+        done = model.date_to_datetime(done)
+
+
+        changed = item.finish_item(doc_id, job, done, due)
+
+        if changed:
+            if doc_id in dataview.itemcache:
+                del dataview.itemcache[doc_id]
+            application.layout.focus(text_area)
+            set_text(dataview.show_active_view())
+            loop = asyncio.get_event_loop()
+            loop.call_later(0, data_changed, loop)
+        else:
+            show_message('finish', f"Cancelled, '{done_str}' is invalid.")
+            return
 
     asyncio.ensure_future(coroutine())
 
 @bindings.add('C', filter=is_viewing_or_details & is_item_view & is_items_table)
 def edit_copy(*event):
     global item
     global starting_buffer_text
@@ -2098,28 +2262,35 @@
     if dataview.is_showing_details:
         application.layout.focus(text_area)
         dataview.hide_details()
     dataview.is_editing = True
     doc_id, entry = dataview.get_details(text_area.document.cursor_position_row, True)
     item.edit_copy(doc_id, entry)
     entry_buffer.text = item.entry
-    starting_buffer_text = ""
+    starting_buffer_text = item.entry
     default_buffer_changed(event)
     default_cursor_position_changed(event)
     application.layout.focus(entry_buffer)
 
 @bindings.add('g', filter=is_viewing & is_not_editing)
 def do_goto(*event):
     row = text_area.document.cursor_position_row
+    if not row:
+        logger.debug(f"do_goto failed to return a row for cursor position {cursor_position_row}")
+        return
     res = dataview.get_row_details(row) # item_id, instance, job_id
-    doc_id = res[0]
-    if not doc_id:
+    if res:
+        logger.debug(f"get_row_details for row {row} returned {res} ")
+    else:
         return
+    doc_id = res[0]
+    # we have a row and a doc_id
     ok, goto = dataview.get_goto(row)
-    if ok:
+    logger.debug(f"calling get_goto on row {row} with doc_id {res[0]} - returned: {ok}, {goto}")
+    if ok and goto:
         res = openWithDefault(goto)
         if res:
             show_message("goto", res, 8)
     else:
         show_message("goto", goto, 8)
 
 
@@ -2159,87 +2330,149 @@
     text_area.buffer.cursor_position = \
                     text_area.buffer.document.translate_row_col_to_index(row, 0)
 
 @bindings.add('f5')
 def do_import_file(*event):
     inbasket = os.path.join(etmhome, "inbasket.text")
     default = inbasket if os.path.exists(os.path.expanduser(inbasket)) else etmhome
-    # default = inbasket
     msg = ""
     def coroutine():
         global msg
         dialog = TextInputDialog(
             title='import file',
             completer=PathCompleter(expanduser=True),
             default=default,
             label_text=f"""\
-It is possible to import data from files with
-one of the following extensions:
+It is possible to import data from files with one
+of the following extensions:
   .json  a json file exported from etm 3.2.x
   .text  a text file with etm entries as lines
   .ics   an iCalendar file
+or a collection of internally generated examples
+by entering the single word:
+   lorem
+Each of the examples is tagged 'lorem' and thus
+can easily be removed with a single query:
+   any t lorem | remove
 
-Warning: files imported from the directory
+Files imported from the etm home directory
    {etmhome}
-will be removed after importing.
+will be removed after importing to avoid possible
+duplications.
 
-Enter the path of the file to import:""")
+Enter the full path of the file to import or
+'lorem':
+""")
 
         file_path = yield from show_dialog_as_float(dialog)
-        if file_path:
-            file_path = os.path.normpath(os.path.expanduser(file_path))
-            ok, msg = import_file(file_path)
+        if not file_path:
+           return
+        if file_path.strip().lower() == 'lorem':
+            logger.debug(f"calling import_file")
+            ok, msg = import_file('lorem')
             if ok:
-                etm_dir = os.path.normpath(os.path.expanduser(etmdir))
-
-                if os.path.dirname(file_path) == etm_dir:
-                    os.remove(file_path)
-                    filehome = os.path.join("~", os.path.split(file_path)[1])
-                    msg += f"\n and removed {filehome}"
                 dataview.refreshRelevant()
                 dataview.refreshAgenda()
                 dataview.refreshCurrent()
-                dataview.refresh_konnections()
+                dataview.refreshKonnections()
                 loop = asyncio.get_event_loop()
                 loop.call_later(0, data_changed, loop)
-            show_message('import file', msg)
+            show_message('import lorem', msg)
+
+        else:
+            if file_path:
+                file_path = os.path.normpath(os.path.expanduser(file_path))
+                ok, msg = import_file(file_path)
+                if ok:
+                    etm_dir = os.path.normpath(os.path.expanduser(etmdir))
+
+                    if os.path.dirname(file_path) == etm_dir:
+                        os.remove(file_path)
+                        filehome = os.path.join("~", os.path.split(file_path)[1])
+                        msg += f"\n and removed {filehome}"
+                    dataview.refreshRelevant()
+                    dataview.refreshAgenda()
+                    dataview.refreshCurrent()
+                    dataview.refreshKonnections()
+                    loop = asyncio.get_event_loop()
+                    loop.call_later(0, data_changed, loop)
+                show_message('import file', msg)
 
     asyncio.ensure_future(coroutine())
 
 
 @bindings.add('c-t', 'c-t', filter=is_viewing & is_item_view)
 def do_whatever(*event):
     """
     For testing whatever
     """
-    logger.debug("t, t")
+    dataview.update_datetimes_to_periods()
+    set_text(dataview.show_active_view())
+
+
+@bindings.add('v', filter=is_viewing)
+def refresh_views(*event):
+    """
+    Refresh all views to fit current window dimensions and redraw the active view
+    """
+    dataview.refreshCache()
+    set_text(dataview.show_active_view())
+    return True
+
+
+@bindings.add('c-t', filter=is_viewing & is_item_view)
+def quick_timer(*event):
+    now = format_datetime(pendulum.now(), short=True)[1]
+    def coroutine():
+        dialog = TextInputDialog(
+            title='Quick timer summary',
+            label_text='summary:',
+            default=now)
+
+        summary = yield from show_dialog_as_float(dialog)
+
+        if summary:
+            item_hsh = {
+                    'itemtype': '!',
+                    'summary': summary,
+                    'created': pendulum.now('UTC')
+                    }
+
+            doc_id = ETMDB.insert(item_hsh)
+            if doc_id:
+                dataview.next_timer_state(doc_id)
+                dataview.next_timer_state(doc_id)
+                dataview.refreshRelevant()
+                dataview.refreshAgenda()
+                dataview.refreshCurrent()
+                dataview.refreshKonnections()
+                loop = asyncio.get_event_loop()
+                loop.call_later(0, data_changed, loop)
+    asyncio.ensure_future(coroutine())
 
 
 @bindings.add('c-x', filter=is_viewing & is_item_view)
 def toggle_archived_status(*event):
     """
     If using items table move the selected item to the archive table and vice versa.
     """
-    # row = text_area.document.cursor_position_row
-    # dataview.get_arch_id(text_area.document.cursor_position_row)
     res = dataview.move_item(text_area.document.cursor_position_row)
     if not res:
         return
     application.layout.focus(text_area)
     loop = asyncio.get_event_loop()
     if dataview.query_mode == "items table":
         set_text(dataview.show_active_view())
         loop.call_later(0, data_changed, loop)
     else:
         set_text("The reminder has been moved to items table.\nRun the previous query again to update the display")
         text = f"a { dataview.query_text }"
         dataview.use_items()
         item.use_items()
         loop.call_later(0, data_changed, loop)
-        # loop.call_later(0, do_show_processing, loop)
         loop.call_later(.1, do_complex_query, text, loop)
     return
 
 
 @bindings.add('c-q')
 def exit(*event):
     tmp = []
@@ -2271,14 +2504,20 @@
 @bindings.add('a', filter=is_viewing)
 def agenda_view(*event):
     set_view('a')
 
 @bindings.add('b', filter=is_viewing)
 def busy_view(*event):
     set_view('b')
+    busy_details = dataview.busy_details
+    if dataview.busy_row:
+        text_area.buffer.cursor_position = \
+            text_area.buffer.document.translate_row_col_to_index(dataview.busy_row-1, 0)
+    else:
+        busy_area.text = get_busy_text()
 
 @bindings.add('c', filter=is_viewing)
 def completed_view(*event):
     set_view('c')
 
 @bindings.add('q', filter=is_viewing)
 def query_view(*event):
@@ -2316,14 +2555,18 @@
 def forthcoming_view(*event):
     set_view('f')
 
 @bindings.add('d', filter=is_viewing)
 def next_view(*event):
     set_view('d')
 
+@bindings.add('e', filter=is_viewing)
+def engaged_view(*event):
+    set_view('e')
+
 @bindings.add('j', filter=is_viewing)
 def journal_view(*event):
     set_view('j')
 
 @bindings.add('r', filter=is_viewing)
 def review_view(*event):
     set_view('r')
@@ -2348,14 +2591,151 @@
     set_view('l')
 
 def set_view(view):
     dataview.set_active_view(view)
     item.use_items()
     set_text(dataview.show_active_view())
 
+def get_busy_day(d):
+    busy_details = dataview.busy_details
+    r = 5 + 2*(d-1)
+    if not r in busy_details.keys():
+        return
+    text_area.buffer.cursor_position = \
+        text_area.buffer.document.translate_row_col_to_index(r-1, 0)
+    busy_area.text = busy_details.get(r, get_busy_text())
+    dataview.busy_row = r
+
+
+@bindings.add('1', filter=is_busy_view & is_viewing)
+def get_busy_1(*event):
+    get_busy_day(1)
+
+
+@bindings.add('2', filter=is_busy_view & is_viewing)
+def get_busy_1(*event):
+    get_busy_day(2)
+
+
+@bindings.add('3', filter=is_busy_view & is_viewing)
+def get_busy_1(*event):
+    get_busy_day(3)
+
+
+@bindings.add('4', filter=is_busy_view & is_viewing)
+def get_busy_1(*event):
+    get_busy_day(4)
+
+
+@bindings.add('5', filter=is_busy_view & is_viewing)
+def get_busy_1(*event):
+    get_busy_day(5)
+
+
+@bindings.add('6', filter=is_busy_view & is_viewing)
+def get_busy_1(*event):
+    get_busy_day(6)
+
+
+@bindings.add('7', filter=is_busy_view & is_viewing)
+def get_busy_1(*event):
+    get_busy_day(7)
+
+
+
+@bindings.add('enter', filter=is_busy_view & is_viewing)
+def curr_busy(*event):
+    busy_details = dataview.busy_details
+    if not busy_details:
+        return
+    current_row = text_area.document.cursor_position_row + 1
+    busy_area.text = busy_details.get(current_row, get_busy_text())
+
+
+@bindings.add('down', filter=is_busy_view & is_viewing)
+def next_busy(*event):
+    busy_details = dataview.busy_details
+    if not busy_details:
+        return
+    rows = [x for x in busy_details.keys()]
+    rows.sort()
+    current_row = text_area.document.cursor_position_row + 1
+    next_row = rows[-1]
+    for r in rows:
+        if r > current_row:
+            next_row = r
+            break
+    text_area.buffer.cursor_position = \
+        text_area.buffer.document.translate_row_col_to_index(next_row-1, 0)
+    busy_area.text = busy_details.get(next_row, get_busy_text())
+    dataview.busy_row = next_row
+
+
+@bindings.add('up', filter=is_busy_view & is_viewing)
+def previous_busy(*event):
+    busy_details = dataview.busy_details
+    if not busy_details:
+        return
+    rows = [x for x in busy_details.keys()]
+    rows.sort(reverse=True)
+    current_row = text_area.document.cursor_position_row + 1
+    next_row = 1
+    for r in rows:
+        if r < current_row:
+            next_row = r
+            break
+    text_area.buffer.cursor_position = \
+        text_area.buffer.document.translate_row_col_to_index(next_row-1, 0)
+    busy_area.text = busy_details.get(next_row, "")
+    dataview.busy_row = next_row
+
+
+@bindings.add('down', filter=is_not_busy_view & is_not_yearly_view & is_viewing)
+def next_id(*event):
+    row2id = dataview.row2id
+    if not row2id:
+        return
+    rows = [x for x in row2id.keys()]
+    rows.sort()
+    current_row = text_area.document.cursor_position_row
+    next_row = rows[-1]
+    for r in rows:
+        if r > current_row:
+            next_row = r
+            break
+    if next_row in rows:
+        next_id = row2id[next_row][0] if isinstance(row2id[next_row], tuple) else row2id[next_row]
+    else:
+        next_id = "?"
+    text_area.buffer.cursor_position = \
+        text_area.buffer.document.translate_row_col_to_index(next_row, 0)
+
+
+
+@bindings.add('up', filter=is_not_busy_view & is_not_yearly_view & is_viewing)
+def previous_id(*event):
+    row2id = dataview.row2id
+    if not row2id:
+        return
+    rows = [x for x in row2id.keys()]
+    rows.sort(reverse=True)
+    current_row = text_area.document.cursor_position_row
+    next_row = 1
+    for r in rows:
+        if r < current_row:
+            next_row = r
+            break
+    if next_row in rows:
+        next_id = row2id[next_row][0] if isinstance(row2id[next_row], tuple) else row2id[next_row]
+    else:
+        next_id = "?"
+    text_area.buffer.cursor_position = \
+        text_area.buffer.document.translate_row_col_to_index(next_row, 0)
+
+
 @bindings.add('c-p', filter=is_viewing)
 def next_pinned(*event):
     """
     Move the cursor to the next row corresponding to a pinned id if there is such a row and to row 0 otherwise.
     """
     pinned = dataview.pinned_list
     if not pinned:
@@ -2363,18 +2743,16 @@
     rows = [(k, v) for k, v in dataview.row2id.items() if v in pinned]
     if not rows:
         return
     rows.sort()
     cur_row = text_area.document.cursor_position_row
     nxt = 0
     for k, v in rows:
-        logger.debug(f"k: {k}; v: {v}")
         if k > cur_row:
             nxt = k
-            logger.debug(f"found row: {nxt} for id:  {v}")
             break
     text_area.buffer.cursor_position = \
         text_area.buffer.document.translate_row_col_to_index(nxt, 0)
 
 
 @bindings.add('Z', filter=is_viewing)
 def toggle_goto_id(*event):
@@ -2384,24 +2762,34 @@
     dataview.goto_id = None if dataview.goto_id else dataview.get_details(text_area.document.cursor_position_row)[0]
 
 
 
 @bindings.add('right', filter=is_agenda_view & is_viewing)
 def nextweek(*event):
     dataview.nextYrWk()
+    dataview.busy_row = 0
+    busy_details = dataview.busy_details
+    busy_area.text = '' # get_busy_text()
     set_text(dataview.show_active_view())
 
+
 @bindings.add('left', filter=is_agenda_view & is_viewing)
 def prevweek(*event):
     dataview.prevYrWk()
+    dataview.busy_row = 0
+    busy_details = dataview.busy_details
+    busy_area.text = '' # get_busy_text()
     set_text(dataview.show_active_view())
 
 @bindings.add('space', filter=is_agenda_view & is_viewing)
 def currweek(*event):
     dataview.currYrWk()
+    dataview.busy_row = 0
+    busy_details = dataview.busy_details
+    busy_area.text = ""
     set_text(dataview.show_active_view())
 
 @bindings.add('right', filter=is_yearly_view & is_viewing)
 def nextcal(*event):
     dataview.nextcal()
     set_text(dataview.show_active_view())
 
@@ -2447,26 +2835,27 @@
 @bindings.add('c-z', filter=is_editing, eager=True)
 def close_edit(*event):
     global text_area
     row, col = get_row_col()
     if entry_buffer_changed():
         save_before_quit()
     else:
-        # item.is_modified = False
         app = get_app()
         app.editing_mode = EditingMode.EMACS
         dataview.is_editing = False
         application.layout.focus(text_area)
         set_text(dataview.show_active_view())
     restore_row_col(row, col)
 
 @edit_bindings.add('c-s', filter=is_editing, eager=True)
 def save_changes(*event):
     if entry_buffer_changed():
+        timer_save = TimeIt('***SAVE***')
         maybe_save(item)
+        timer_save.stop()
     else:
         # no changes to save - close editor
         dataview.is_editing = False
         application.layout.focus(text_area)
         set_text(dataview.show_active_view())
         app = get_app()
         app.editing_mode = EditingMode.EMACS
@@ -2519,35 +2908,38 @@
         MenuItem('^q) quit', handler=exit),
     ]),
     MenuItem('view', children=[
         MenuItem('a) agenda', handler=agenda_view),
         MenuItem('b) busy', handler=busy_view),
         MenuItem('c) completed', handler=completed_view),
         MenuItem('d) do next', handler=next_view),
+        MenuItem('e) engaged', handler=engaged_view),
         MenuItem('f) forthcoming', handler=forthcoming_view),
         MenuItem('h) history', handler=history_view),
         MenuItem('i) index', handler=index_view),
         MenuItem('j) journal', handler=journal_view),
         MenuItem('l) location', handler=location_view),
         MenuItem('m) timers', handler=timers_view),
         MenuItem('p) pinned', handler=pinned_view),
         MenuItem('q) query', handler=query_view),
         MenuItem('r) review', handler=review_view),
         MenuItem('t) tags', handler=tag_view),
         MenuItem('u) used time', handler=used_view),
         MenuItem('U) used summary', handler=used_summary_view),
+        MenuItem('v) refresh views to fit resized terminal', handler=refresh_views),
         MenuItem('-', disabled=True),
         MenuItem("s) scheduled alerts for today", handler=do_alerts),
-        MenuItem('y) half yearly calendar', handler=yearly_view),
+        MenuItem('y) yearly calendar', handler=yearly_view),
         MenuItem('-', disabled=True),
         MenuItem('/|?|,,) search forward|backward|clear search'),
         MenuItem('n) next incrementally in search'),
         MenuItem('^l) prompt for and jump to line number', handler=do_go_to_line),
         MenuItem('^p) jump to next pinned item', handler=next_pinned),
         MenuItem('^c) copy active view to clipboard', handler=copy_active_view),
+        MenuItem('^t) start quick timer', handler=quick_timer),
         MenuItem('-', disabled=True),
         MenuItem('J) jump to date in a), b) and c)', handler=do_jump_to_date),
         MenuItem('right) next in a), b), c), u), U) and y)'),
         MenuItem('left) previous in a), b), c), u), U) and y)'),
         MenuItem('space) current in a), b), c), u), U) and y)'),
     ]),
     MenuItem('editor', children=[
@@ -2569,18 +2961,18 @@
         MenuItem('S) schedule new', handler=do_schedule_new),
         MenuItem('g) open goto link', handler=do_goto),
         MenuItem('k) show konnections', handler=show_konnections),
         MenuItem('^r) show repetitions', handler=not_editing_reps),
         MenuItem('^u) update last modified', handler=do_touch),
         MenuItem('^x) toggle archived status', handler=toggle_archived_status),
         MenuItem('-', disabled=True),
-        MenuItem('T) change timer to next state ', handler=next_timer_state),
-        MenuItem("TR) record usedtime and delete timer", handler=record_time),
+        MenuItem('T) activate timer if none active ', handler=next_timer_state),
+        MenuItem("TR) add usedtime / record usedtime and end timer", handler=record_time),
         MenuItem('TD) delete timer', handler=maybe_delete_timer),
-        MenuItem('TT) toggle paused/running for active timer', handler=toggle_active_timer),
+        MenuItem('TT) toggle paused/running for the active timer', handler=toggle_active_timer),
     ]),
 ], floats=[
     Float(xcursor=True,
           ycursor=True,
           content=CompletionsMenu(
               max_height=16,
               scroll_offset=1)),
@@ -2595,35 +2987,45 @@
     else:
         ask, reply = ('', '')
     ask_buffer.text = ask
     reply_buffer.text = wrap(reply, 0)
 
 
 async def main(etmdir=""):
-    global item, settings, ampm, style, type_colors, application
+    global item, settings, ampm, style, type_colors, application, busy_colors
+    timer_view = TimeIt('***VIEW***')
     ampm = settings['ampm']
+    window_colors = settings['window_colors']
     type_colors = settings['type_colors']
-    logger.debug(f"main type_colors: {type_colors}")
     window_colors = settings['window_colors']
-    logger.debug(f"main window_colors: {window_colors}")
+    busy_colors = {
+            VSEP    : type_colors['wrap'],
+            HSEP    : type_colors['wrap'],
+            BUSY    : type_colors['event'],
+            CONF    : type_colors['inbox'],
+            ADAY    : type_colors['wrap'],
+            }
+    # query = ETMQuery()
     style = get_style(window_colors)
     agenda_view()
 
     application = Application(
         layout=Layout(
             root_container,
             focused_element=text_area,
         ),
         # set editing_mode in the entry buffer, use default elsewhere
         key_bindings=bindings,
         enable_page_navigation_bindings=True,
         mouse_support=True,
         style=style,
         full_screen=True)
+    logger.debug("XX starting event_handler XX")
     background_task = asyncio.create_task(event_handler())
+    timer_view.stop()
     try:
         await application.run_async()
     finally:
         background_task.cancel()
         logger.info("Quitting event loop.")
```

### Comparing `etm-dgraham-4.9.7/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,10 @@
-Metadata-Version: 2.1
-Name: etm-dgraham
-Version: 4.9.7
-Summary: event and task manager
-Home-page: https://dagraham.github.io/etm-dgraham/
-Author: Daniel A Graham
-Author-email: dnlgrhm@gmail.com
-License: GPL
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Office/Business
-Classifier: Topic :: Office/Business :: News/Diary
-Classifier: Topic :: Office/Business :: Scheduling
-Requires-Python: >=3.7.3
-Description-Content-Type: text/markdown
-
-
 <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/etmlogo.png" alt="etm" title="event and task manager" width="200px" />
 
-This is the etm user manual. It is best viewed at [GitHub.io](https://dagraham.github.io/etm-dgraham/) where all the internal, contents links work correctly. etm itself is available from [PyPi](https://pypi.org/project/etm-dgraham/) and [GitHub](https://github.com/dagraham/etm-dgraham) and further information from the etm discussion group at [groups.io](https://groups.io/g/etm) - note especially the [files](https://groups.io/g/etm/files/) folder. Brief how-to videos are available at [youtube](https://www.youtube.com/playlist?list=PLN2WQIqrwSxxh2eNY_YczO6YC-icpKWeG).
+This is the etm user manual. It is best viewed at [GitHub.io](https://dagraham.github.io/etm-dgraham/) where all the internal, contents links work correctly. etm itself is available from [PyPi](https://pypi.org/project/etm-dgraham/) and [GitHub](https://github.com/dagraham/etm-dgraham) and further information from the etm discussion group at [groups.io](https://groups.io/g/etm-dgraham). Brief how-to videos are available at [youtube](https://www.youtube.com/@etm-dgraham).
 
 
 # Contents {#contents}
 -   [Overview](#overview)
     -   [Reminders](#reminders)
         -   [examples](#examples)
         -   [text entry versus forms](#text-entry-versus-forms)
@@ -49,26 +25,29 @@
             -   [Simple query examples](#simple-query-examples)
             -   [Archive queries](#archive-queries)
             -   [Update queries](#update-queries)
             -   [Complex queries](#complex-queries)
             -   [Command History](#command-history)
             -   [Saved Queries](#saved-queries)
         -   [Common Features](#common-features)
+    -   [Mobile Access to your reminders](#mobile)
     -   [Menus](#menus)
         -   [etm menu notes](#etm-menu-notes)
         -   [view menu notes](#view-menu-notes)
         -   [editor menu notes](#editor-menu-notes)
         -   [selected menu notes](#selected-menu-notes)
     -   [Installation](#installation)
         -   [For personal use](#for-personal-use)
-        -   [for use in a virtual environment](#for-use-in-a-virtual-environment)
+        -   [for use in an isolated environment](#for-use-in-an-isolated-environment)
         -   [for use system wide](#for-use-system-wide)
     -   [Usage](#usage)
         -   [Terminal size and color](#terminal-size-and-color)
         -   [Home directory](#home-directory)
+        -   [Timers](#timers)
+        -   [lorem examples](#loremexamples)
         -   [Using etm+](#etmplus)
     -   [Deinstallation](#deinstallation)
         -   [From a virtual environment](#from-a-virtual-environment)
         -   [From a system wide installation](#from-a-system-wide-installation)
 -   [Details](#details)
     -   [Item Types](#item-types)
         -   [event](#event)
@@ -90,19 +69,21 @@
 			- [anniversary substitutions](#anniversary-substitutions)
         -   [archived reminders](#archived-reminders)
         -   [configuration](#configuration)
         -   [data storage](#data-storage)
 
 # Overview {#overview}
 
+*etm* began life in 2013 as *etm-qt* sporting a gui based on *Qt*. The intent was to provide an app supporting GTD (David Allen's Getting Things Done) and exploiting the power of python-dateutil. The name changed to *etmtk* in 2014 when *Tk* replaced *Qt*. Development of *etmtk* continued until 2019 when name changed to *etm-dgraham*, to honor the PyPi naming convention, and the interface changed to a terminal based one based on *promt_toolkit*. Features have changed over the years but the text based interface and basic format of the reminders has changed very little. The goal has always been to be the Swiss Army Knife of tools for managing reminders.
+
 ## Reminders {#reminders}
 
 *etm* offers a simple way to manage your events, tasks and other reminders.
 
-Rather than filling out fields in a form to create or edit reminders, a simple text-based format is used. Each reminder in *etm* begins with a *type character* followed by a brief *summary* of the item and then, perhaps, by one or more *@key value* pairs to specify other attributes of the reminder. Mnemonics are used to make the keys easy to remember, e.g, @s for starting datetime, @l for location, @d for description and so forth.
+Rather than filling out fields in a form to create or edit reminders, a simple text-based format is used. Each reminder in *etm* begins with a *type character* followed by a brief *summary* of the item and then, perhaps, by one or more *@key value* pairs to specify other attributes of the reminder. Mnemonics are used to make the keys easy to remember, e.g, @s for scheduled datetime, @l for location, @d for description and so forth.
 
 The 4 types of reminders in etm with their associated type characters:
 
 * task: **-**
 * event: **\***
 * journal: **%**
 * inbox: **!**
@@ -123,38 +104,38 @@
 
 * A journal entry (**%**): a favorite Churchill quotation that you heard at 2pm today with the quote itself as the [d]escription.
 
         % Give me a pig - Churchill @s 2p @d Dogs look up at
           you. Cats look down at you. Give me a pig - they
           look you in the eye and treat you as an equal.
 
+	The *summary*, "Give me a pig - Churchill" in this example, follows the type character and is meant to be brief - analagous to the subject of an email. The optional *description* follows the "@d" and is meant to be more expansive - analagous to the body of an email.
+
 * A task (**-**): build a dog house, with component [j]obs.
 
         - Build dog house @j pick up materials @j cut pieces
           @j assemble @j sand @j paint
 
-* Inbox (**!**): meet Alex for coffee Friday. This can be
-  changed to an event when the time is confirmed by
-  replacing the **!** with an **\*** and adding the time to `@s`.
+* Inbox (**!**): meet Alex for coffee Friday.
 
         ! Coffee with Alex @s fri @e 1h
 
-    This inbox entry will appear on the current day in *agenda view* until you make the changes.
+	This can be changed to an event when the details are confirmed by replacing the **!** with an **\*** and adding the time to `@s`.  This inbox entry will appear on the current day in *agenda view* until you make the changes.
 
 * An appointment (event) for a dental exam and cleaning at 2pm on Feb 5 and then again [@+] at 9am on Sep 3.
 
         * dental exam and cleaning @s 2p feb 5 2019 @e 45m
           @+ 9am Sep 3 2019
 
 [↺ contents](#contents)
 
 ### text entry versus forms {#text-entry-versus-forms}
 
 * Text entry removes the need to hunt for and click in the relevant entry box and allows you to keep your fingers on the keyboard.
-* Text entry supports the full flexibility of the superb Python *dateutil* package. Consider, for example, creating a reminder for Presidential election day which repeats every 4 years on the first Tuesday after a Monday in November (a monthday falling between 2 and 8). In *etm*, this event would be
+* Text entry supports the full flexibility of the superb Python *dateutil* package. Consider, for example, creating a reminder to vote for President election day which repeats every 4 years on the first Tuesday after a Monday in November (a Tuesday whose monthday falls between 2 and 8). In *etm*, this event would be
 
         * Presidential election day @s nov 1 2020 @r y &i 4 &M 11
           &m 2, 3, 4, 5, 6, 7, 8 &w tu
 
     Try this with a form based calendar application.
 
 [↺ contents](#contents)
@@ -162,14 +143,15 @@
 ### unobtrusive and timely entry assistance {#unobtrusive-and-timely-entry-assistance}
 
 When you want to create a new reminder or edit an exiting one, *etm* opens an area at the bottom of the screen that is divided into two parts by a horizontal line. The lower part is the entry area where what you type appears. The upper part is the prompt/feedback area where *etm* responds to your typing. This response might take the form of providing a suggestion about alternatives, information about the type of input required or feedback about how your current entry is being interpreted. It is important to realize that none of this interferes with your typing - you can blaze away as quickly as you like or even paste complete entries and never glance at the prompt if you like. This is the **unobtrusive** part of the prompt/feedback process.
 
 <img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/new.png" alt="new" title="new entry" width="600px" hspace="20px"/>
 
 
+
 [↺ contents](#contents)
 
 #### just in time entry prompts and feedback {#just-in-time-entry-prompts-and-feedback}
 
 Let's create the election day reminder to illustrate the **timely** part of the process. Begin by pressing `N` to create a new reminder and notice that *etm* automatically prompts you for the item type character and suggests the alternatives.
 
         item type
@@ -186,35 +168,35 @@
 
         ────────────────────────────────────────────────────────────
         *_
 
 Enter the summary followed by an `@` and *etm* will automatically display the required and available `@-keys`.
 
         @-key
-        required: @s (start)
+        required: @s (scheduled)
         available: @+ (include), @- (exclude), @a (alerts),
         @b (beginby), @c (calendar), @d (description),
         @e (extent), @g (goto), @i (index), @l (location),
         @m (mask), @n (attendee), @o (overdue),
-        @r (repetition frequency), @s (start), @t (tag),
+        @r (repetition frequency), @s (scheduled), @t (tag),
         @u (used time), @x (expansion), @z (timezone)
         ────────────────────────────────────────────────────────────
         * Presidential election day @_
 
-You see that `@s` is required, so add the `s` and *etm* will prompt you for the value for the start option and describe the type of input required.
+You see that `@s` is required, so add the `s` and *etm* will prompt you for the value for the scheduled option and describe the type of input required.
 
-        start
-        starting date or datetime
+        scheduled
+        scheduled date or datetime
 
         ────────────────────────────────────────────────────────────
         * Presidential election day @s_
 
 As you enter the datetime, *etm* will display its interpretation of your entry.
 
-        start
+        scheduled
         Sun Nov 1 2020
 
         ────────────────────────────────────────────────────────────
         * Presidential election day @s nov 1 20_
 
 Now append an `@` to see the prompt for options and notice that `@s`, having been provided, is no longer listed.
 
@@ -303,15 +285,15 @@
             │   Tue Nov 2 2032                 │
             │   Tue Nov 4 2036                 │
             │                                  │
             │           <    OK    >           │
             │                                  │
             └──────────────────────────────────┘
 
-These are the first 5 repetitions on or after Nov 1 2020. Notice that the start value of Nov 1 2020 is not one of the repetitions since it doesn't satisfy the requirements. These appear correct, so press ^S to save the reminder.
+These are the first 5 repetitions on or after Nov 1 2020. Notice that the scheduled value of Nov 1 2020 is not one of the repetitions since it doesn't satisfy the requirements. These appear correct, so press ^S to save the reminder.
 
 
 General observations:
 
 * The general structure of this reminder is
 
 			* Presidential election day
@@ -328,67 +310,67 @@
 * The prompts provide "just in time" information relevant to the entry you are typing and need only be consulted if you are uncertain about your entry. With a little
 	experience, most reminders can be completed without a glance at the prompt.
 
 [↺ contents](#contents)
 
 #### fuzzy parsing of datetimes {#fuzzy-parsing-of-datetimes}
 
-Whenever *etm* expects a datetime entry as, for example, when you are entering an `@s` starting datetime, it applies fuzzy parsing to your entry.  Suppose it is Dec 17 2019, your computer is in the Eastern timezone and you have just entered `@s` for your lunch event
+Whenever *etm* expects a datetime entry as, for example, when you are entering an `@s` scheduled datetime, it applies fuzzy parsing to your entry.  Suppose it is Dec 17 2019, your computer is in the Eastern timezone and you have just entered `@s` for your lunch event
 
-        start
-        starting date or datetime
+        scheduled
+        scheduled date or datetime
 
         ────────────────────────────────────────────────────────────
         * lunch @s_
 
 If you enter `1`, *etm* will interpret it as 1am on the current date in the local timezone.
 
-        start
+        scheduled
         Tue Dec 17 2019 1:00am EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1_
 
 Adding `p` changes the interpretation to 1pm.
 
-        start
+        scheduled
         Tue Dec 17 2019 1:00pm EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p_
 
 Now start adding 'fri' by appending an 'f'.
 
-        start
+        scheduled
         '1p f' is incomplete or invalid
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p f_
 
 and *etm* will complain that the entry is now either incomplete or invalid. Add the remaining 'ri'.
 
-        start
+        scheduled
         Fri Dec 20 2019 1:00pm EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p fri_
 
 and *etm* understands that you want the coming Friday, Dec 20. Now suppose that you will be in California on Friday and you want Pacific, not Eastern time. Then add an entry for `@z`.
 
-        start
+        scheduled
         local datetime: Fri Dec 20 2019 4:00pm EST
 
         ────────────────────────────────────────────────────────────
         * lunch @s 1p fri_ @z US/Pacific
 
 Note that `local datetime` is now prepended to the result which is still displayed in the local timezone, since that is the location of your computer, but the time has changed to `4:00pm EST` which, of course, is the same time as `1:00pm PST`. *etm* **always** displays times in the current local time zone. When you save this item, the time will be converted to universal time and the `@z US/Pacific` will be deleted - once the time has been converted, the original timezone is no longer relevant.
 
 What if you had entered the 'fri' first?
 
-        start
+        scheduled
         Fri Dec 20 2019
 
         ────────────────────────────────────────────────────────────
         * lunch @s fri
 
 Here *etm* supposes again that you want the coming Friday, Dec 20 but without a time being specified, it is interpreted as a date rather than a datetime and thus without a timezone. Add the `1p` and timezone the result will be the same as before.
 
@@ -399,15 +381,15 @@
         or 'float' to specify a naive/floating datetime
 
         ────────────────────────────────────────────────────────────
         * lunch @s fri 1p @z
 
 and note that supplying 'float' as the timezone does the trick.
 
-        start
+        scheduled
         Fri Dec 20 2019 1:00pm
 
         ────────────────────────────────────────────────────────────
         * lunch @s fri 1p_ @z float
 
 The datetime now appears without either the 'local datetime' prefix or the 'EST' suffix which reveals that it is a naive/floating datetime.
 
@@ -490,54 +472,74 @@
 
 The display for each reminder shows the itemtype and summary column on the left followed by a *flags* column which displays a combination of letters from 'g' (goto), 'k' (connection), 'p' (pinned) and 't' (timer) reflecting the presence of these attributes in the reminder. This column is sometimes followed on the extreme right by another column whose contents depends on the view. E.g. in index and journal views the 'id' of the reminder is displayed while in history view, the last modification timestamp of the reminder is displayed.
 
   * a: Agenda: dated unfinished tasks and other reminders by year-week and week day
   * b: Busy: a graphical illustration of busy and conflicted times by year-week
   * c: Completed: finished tasks and jobs and used time entries by year-week and week day
   * d: Do Next: undated tasks grouped by location/context and ordered by priority (highest first) and extent (least first)
+  * e: Engaged: instances of reminders with used time entries with daily totals displayed graphically
   * f: Forthcoming: unfinished dated tasks and other dated reminders by next occurrence
   * h: History: all items by the latter of the modified or created datetimes in descending order, i.e., most recent first. Datetimes are displayed using a 5 character format where, e.g., 1:15pm today would be displayed as 13:15, November 7 of the current year as 11/17 and January 15 of 2012 as 12.01.
   * i: Index: all items grouped hierarchically by index entry
   * j: Journal: journal entries grouped hierarchically by index entry
   * k: Konnection: items with @k konnection links either to or from the selected item.
   * l: Location: items grouped hierarchically by location entry
   * m: Timers: items with timers.
   * p: Pinned: items whose pin status is on.
   * q: Query: items matching a user specified query. Enter ? for query usage.
   * r: Review: undated tasks sorted by the time since the task was last modified with the most recently modified last.
   * t: Tags: all items with @t tag entries grouped by tag
   * u: Used Time: all items with @u used time entries grouped by month and hierarchically by index
   * U: Used Summary: used time aggregates grouped by month and hierarchically by index
-  * y: Yearly Planning Calendar: compact monthly calendar by half year.
+  * y: Yearly Planning Calendar: compact monthly calendar.
 
 
 [↺ contents](#contents)
 
 ### Weekly Views {#weekly-views}
 
-The _weekly_ agenda, busy and completed views display one week at a time and are *synchronized* so that all three views always display the same week. Left or right cursor keys go backward or forward a week at a time and the pressing the space bar jumps to the week containing the current day. You can also press "J" and enter a date to jump to the week containing the date.
+The _agenda_, _busy_, _completed_ and _engaged_ views display one week at a time and are *synchronized* so that all four views always display the same week. Press the ▶ (right) or ◀ (left) cursor keys go forward or backward a week at a time or press the space bar to jump to the week containing the current day. You can also press "J" and enter a date to jump to the week containing the date.
+
+In _agenda_ view, only days with scheduled reminders are listed. If nothing is scheduled for the entire week, then "Nothing scheduled" is displayed.
+
+
+In _busy_ view, only days that have events with busy times (@e and/or @w entries) are displayed. Press the number of the weekday, [1→Mon, ..., 7→Sun], to show the details of the busy periods from that day or press the ▼ (down) or ▲ (up) cursor keys to show the details of the next or previous day with busy periods.
+
+_Completed_ view shows instances of completed tasks.
 
-In both agenda and completed views, only days with scheduled reminders are listed. If nothing is scheduled for the entire week, then "Nothing scheduled" is displayed.
+_Engaged_ view shows instances of reminders with used time entries with daily totals displayed graphically.
 
 The normal agenda listing for a week day:
 
 * all day events (events with dates as `@s` entries)
 * datetime items (reminders with datetimes as `@s` entries) by time
 * all day tasks (tasks with dates as `@s` entries)
 * all day journal enties (journal entries with dates as `@s` entries)
 
 And, on the current day only:
 
 * inbox items
 * *<* past due warnings in descending order of the number of days past due
 * *>* beginby warnings in ascending order of the number of days remaining
 
+Busy view requires a little explanation. Here is screen shot of agenda view for an illustrative week
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/agenda.png" alt="new" title="agenda view" width="600px" hspace="20px"/>
+
+along with one of busy view for the same week
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/busy.png" alt="new" title="busy view" width="600px" hspace="20px"/>
+
+The first thing to notice in busy view is that busy times are displayed each week day for the period between 7am and 9pm. This period is determined by the *beginbusy* setting in `cfg.yaml` which sets the number of hours after midnight that the display is to begin each day. The period ends 14 hours after *beginbusy*. In this case, it runs from 7 hours after midnight (*beginbusy*) to 7+14=21 hours after midnight or from 7am until 9pm. The resolution is 15 minute periods for each character *slot* so that, for example, the row for *Fr 2* shows a busy period with using 4 green (busy) characters for 10-10:15am, 10:15-10:30am, 10:30-10:45am and 10:45-11am. Now you might notice that this implies that the 4 character slots that begin at 8pm end just before the 9pm slot and that the 9pm slot actually corresponds to the interval 9-9:15pm. Since the actual display includes this last slot, it actually extends for 14 hours plus 15 minutes and thus actually ends at 9:15pm.
+
+The second thing to notice is the red, conflict bar in the display for *Mo 28*. Since the details for this day are displayed in the "busy times" panel at the bottom as well as in the agenda view, you will notice that the conflict corresponds to the overlap between the 6-8am event and the 7-9:30am event. This conflict from 7-8am is illustrated by the 4 red (conflict) characters. Notice also that the period for the first event extends from 6-7am before the period displayed begins at 7am. The single green character to the left of 7am indicates that there were busy times before the displayed period begins. Similarly, the green character to the right of 9-9:15pm on *We 30* indicates that there were busy times after 9:15pm on that day. This corresponds to the 8-10:30pm event shown in agenda view for Wednesday that extends from 9:15-10:30pm after the displayed period.
+
+As you might expect, if a conflict occurred either before or after the displayed period then the corresponding *before* or *after* character would be red instead of green.
+
 [↺ contents](#contents)
 
-### Timer view {#timer-view}
+### Timer View {#timer-view}
 
 This view lists all reminders with associated timers sorted by the elapsed time since the timer's *state* was last changed. The display for each reminder shows the itemtype and summary, any applicable *flags* and, in the right hand column, the elapsed time and *state* of the associated timer.
 
 The sort order assures that the reminder with the active timer will always be at the top of the list and followed by the reminders with the most recently modified timers. This makes it easy to switch back and forth between recent timers.
 
 [↺ contents](#contents)
 
@@ -574,26 +576,28 @@
 reminders with links from the selection
 : the list of items whose ids are included in the @k entries of the selected item
 
 [↺ contents](#contents)
 
 ### Used Time Views {#used-time-views}
 
-The *used time* and *used time summary* views are bound to `u` and `U` respectively. They report `@u` (used time) entries in your reminders grouped by year-month and then heirarchially by `@i` entries. I have a file of reminders with `@i` and `@u` entries such as
+The *used time* and *used time summary* views are bound to `u` and `U` respectively. They report `@u` (used time) entries in your reminders, rounded up according to the `usedtime_minutes` setting in your `cfg.yaml` file and grouped by year-month and then heirarchially by `@i` entries.
+
+I have a file of reminders with `@i` and `@u` entries such as
 
 		* Modi ut sit sed amet sit @s 2019-11-11 10:00am @e
 		   1h30m
 		@u 58m: 2019-11-11 10:58am @u 34m: 2019-11-11 10:34am
 		@i client A/project a1/correspondence
 		@d Aliquam non sed aliquam eius tempora quisquam dolorem.
 		Neque quiquia labore tempora magnam. Quiquia tempora
 		porro est ut. Ut tempora sed non ut eius neque porro.
 		Sed quaerat consectetur dolor sit.
 
-and the *used time view* for November begins with
+With `usedtime_minutes: 6`, the *used time view* for November begins with
 
 		November 2019
 		  client A
 			project a1
 			  correspondence
 				* Modi ut sit sed amet sit: 1.6h Nov 11
 				% Amet modi neque eius adipisci: 2.7h Nov 27
@@ -995,14 +999,15 @@
 * monthend: 12am on the 1st of the following month
 
 and can be combined with period strings using M (month),
 w (week), d (day), h (hour) and m (minute). E.g.:
 * `weekbeg - 1w`  (the beginning of the previous week)
 * `monthend + 1M` (the end of the following month)
 
+
 [↺ contents](#contents)
 
 #### Command History {#command-history}
 
 Any query entered at the 'query:' prompt and submitted by pressing 'Enter' is added to the command history. These queries are kept as long as 'etm' is running and can be accessed using the up and down cursor keys in the query field. This means you can enter a query, check the result, press 'q' to reopen the query prompt, press the up cursor and you will have your previous query ready to modify and submit again. It is also possible to keep a permanent list of queries accessible by shortcuts. See 'Saved Queries' below.
 
 [↺ contents](#contents)
@@ -1106,14 +1111,31 @@
 	* While entering the search expression, push the `up` or `down` cursor keys to change the direction of search.
     * After entering the search expression, press “n” to search (cyclically) for other matches in the direction specified.
 	* Once a search is initiated, it remains active in all views with matches highlighted. To remove the highlighting, search for something unlikely to be matched, e.g., 3 consecutive commas.
 
 
 [↺ contents](#contents)
 
+## Mobile access to your reminders {#mobile}
+
+The files `current.txt` and `next.txt` in your etm home directory are created by *etm* but not displayed within *etm* itself. Whether or not these files are created depends on two settings in your `cfg.yaml`:
+
+* `keep_current`:  non-negative integers for `weeks` and `width`.  If `weeks` is positive, the agenda for that integer number of weeks starting with the current week will be scaled to fit `width` and written to `current.txt` and updated whenever necessary.
+
+* `keep_next`: true or false. If `true`, the contents of *do next* view will be written to `next.txt` in your etm home directory and updated whenever necessary.
+
+By creating links to these files in, e.g., a GoogleDrive folder, you can have access to your current schedule and tasks on your mobile device.
+
+Here is a screen shot from an iPhone of an illustrative `current.txt`:
+
+<img src="https://raw.githubusercontent.com/dagraham/etm-dgraham/master/current_on_iphone.png" alt="new" title="current view" width="300px" hspace="20px"/>
+
+
+[↺ contents](#contents)
+
 ## Menus {#menus}
 
 Pressing F1 toggles the *etm* menu display - opening it if it is closed and closing it if it is open. There are four menu tabs labeled *etm*, *view*, *editor* and *selected* with the options listed below:
 
     etm
 		F1) activate/close menu
         F2) about etm
@@ -1126,35 +1148,38 @@
         ---
         ^q) quit
     view
         a) agenda
         b) busy
         c) completed
         d) do next
+        e) engaged
         f) forthcoming
         h) history
         i) index
         j) journal
         l) location
         p) pinned
         q) query
 		r) review
         t) tags
         u) used time
         U) used time summary
+        v) refresh views to fit resized terminal
         ---
         s) scheduled alerts for today
-        y) half yearly calendar
+        y) yearly calendar
         ---
         /) search forward
         ?) search backward
         n) next incrementally in search
         ^l) prompt for and jump to line number
         ^p) jump to next pinned item
-        ^c) copy active view to clipboars
+        ^c) copy active view to clipboard
+        ^t) start quick timer
         ---
         J) jump to date in a), b) and c)
         right) next in a), b), c), u), U) and y)
         left) previous in a), b), c), u), U) and y)
         space) current in a), b), c), u), U) and y)
     editor
         N) create new item
@@ -1175,16 +1200,17 @@
         g) open goto link
         k) show konnections
         ^r) show repetitions
 		^u) update last modified
         ^x) toggle archived status
         ---
         T) change timer to next state
-        TR) record usedtime and delete timer
+        TR) record usedtime and end timer or add usedtime
         TD) delete timer
+        ---
         TT) toggle paused/running for active timer
 
 
 [↺ contents](#contents)
 
 ### etm menu notes {#etm-menu-notes}
 
@@ -1210,14 +1236,15 @@
 
 [↺ contents](#contents)
 
 ### view menu notes {#view-menu-notes}
 
 The *view* menu provides access to all the *etm* views with the shortcut keys for these views. E.g., press `a` to open *agenda view*.
 
+The *start quick timer* option creates a new, inbox reminder with the current datetime as the subject, associates a timer with reminder and starts the timer. If another timer is active, it will be paused if necessary and made inactive. Subsequent invocations repeat this process.
 
 The entries here are pretty obvious and the views themselves are descibed elsewhere.
 
 [↺ contents](#contents)
 
 ### editor menu notes {#editor-menu-notes}
 
@@ -1238,102 +1265,86 @@
 * *reschedule* will prompt for a datetime. If the reminder is repeating, the provided datetime will replace the datetime of the selected instance. Otherwise it will be used either to replace the current value of `@s` or, if there is no `@s` entry, to create one.
 * *schedule new* will prompt for a datetime and add that instance to any other instances of the reminder.
 * *open goto* will use the system default application to open the file path or url specified in the selected reminders `@g` entry. Items with goto links are displayed with a 'g' in the *flags* column of normal views.
 * *toggle pin* toggles the pin status of an item between off and on. Items for which the pin status are displayed with a 'p', in the *flags* column of normal views and are also displayed in *pinned view*.
 * *show repetitions* pops up a display showing illustrative repetitions if the item is repeating.
 * *toggle archived status* moves the selected reminder from the items table if it is active to the archive table and vice versa if the archive table is active.
 * *change timer to next state*.
-    * these are the states for the timer associated with a reminder and the relevant status of any other timers:
+    * These are the states for the timer associated with a reminder and the relevant status of any other timers:
         * *n* (no timer is associated with this reminder)
             * *n-*: no other timer is active
             * *n+*: another timer is active
         * *i* (a timer is associated with this reminder and it is inactive)
             * *i-*: no other timer is active
             * *i+*: another timer is active
         * *r-*: running (a timer is associated with this reminder and it is running - there cannot be another active timer)
         * *p-*: paused (a timer is associated with this reminder and it is paused - there cannot be another active timer)
 
-       These are the "next" state transitions associated with this action:
+    * These are the "next" state transitions associated with this action:
         * *n+* ⇒ *i+*
-        * *n-* ⇒ *r-*
+        * *n-* ⇒ *p-*
         * *i-* ⇒ *r-*
         * *i+* ⇒ *r-*
         * *r-* ⇒ *p-*
         * *p-* ⇒ *r-*
 
     * Here are the details:
-        * If no timer is currently associated with the reminder, one will be created. If another timer is *active*, the new timer will be *inactive*, otherwise it will be *running*.
+        * If no timer is currently associated with the reminder, one will be created. If another timer is *active*, the new timer will be *inactive*, otherwise it will be *active* and *paused*.
         * If an *inactive* timer is already associated with the reminder. Its state will be changed to *running*. If another timer is *active*, that timer will be changed to *inactive* and, if *running*, its elapsed time will be incremented by the period it has been *running*.
         * If an *active* timer is already associated with the reminder, its state will be toggled between *paused* and *running*. With a transition from *running* to *paused*, the elapsed time for the timer in increased by the period since the timer's state changed to *running*.
 
       Additionally, if there is an *active* timer, its state, either *r* (running) or *p* (paused), is displayed in the *etm* status bar together with the relevant time period, either the total elapsed time or how long the timer has been paused. If there are *inactive* timers with non-zero elapsed times, the total of such elapsed times will also be reported in the status bar. E.g., this display in the status bar
 
             r:4m + i:13m
 
       would mean that the *active* timer is *running* with 4 minutes of unrecorded elapsed time and that there is an additional 13 minutes of unrecorded elapsed time in *inactive* timers.
+
 * *record used time* with a reminder selected, will:
     * If a timer is not currently associated with the reminder, prompt for a timeperiod and ending time to use in adding a usedtime entry to the reminder.
     * If a timer is currently associated with the reminder, use its elapsed time and the last moment it was running as the defaults in the prompt for a usedtime timeperiod and ending time. If the entry is saved, the elapsed time for the timer will be reset to zero and, additionally, if the timer is currently *running*, its status will be changed to *paused*.
 
-    **Important**: timer data is stored in memory and will be lost if *etm* is stopped. Be sure to record usedtime entries for timers with elapsed times before quitting etm. The status bar will always indicate if there is unrecorded elapsed time.
-
 
 [↺ contents](#contents)
 
 ## Installation {#installation}
 
 
 ### For personal use {#for-personal-use}
 
 The easiest way to install *etm* for personal use is to use *pip*:
 
 	$ python3 -m pip install -U etm-dgraham
 
-This will install *etm* with all the needed python supporting modules. You can then start *etm* with
+(This same command can be used to update *etm* when a new version is released.) This will install *etm* with all the needed python supporting modules. You can then start *etm* with
 
 	$ etm <path to home>
 
+
 See [Home directory](#home-directory) for details about `<path to home>`.
 
-<!--  [![etm: installing etm in a virtual environment](http://img.youtube.com/vi/fEPPG82AH7M/0.jpg)](http://www.youtube.com/watch?v=fEPPG82AH7M "installing etm in a virtual environment") -->
 
 [↺ contents](#contents)
 
-### For use in a virtual environment {#For-use-in-a-virtual-environment}
-
-Setting up a virtual environment for etm is only slightly more complicated. The steps for OS/X or linux are illustrated below. For details see [python-virtual-environments-a-primer](https://www.google.com/url?q=https%3A%2F%2Frealpython.com%2Fpython-virtual-environments-a-primer%2F&sa=D&sntz=1&usg=AFQjCNFh7QpJQ4rPCDjZ1eLrV1BRCCpSmw).
-
-Open a terminal and begin by creating a new directory/folder for the virtual environment, say `etm-pypi`, in your home directory:
-
-        $ mkdir ~/etm-pypi
-        $ cd ~/etm-pypi
-
-Now continue by creating the virtual environment (python >= 3.7.4 is required for etm):
-
-        $ python3 -m venv env
+### For use in an isolated environment {#For-use-in-an-isolated-environment}
 
-After a few seconds you will have an `./env` directory. Now activate the virtual environment:
+Installing etm in an isolated or virtual environment (sandbox) is only slightly more complicated. Begin by using *pip* to install *pipx*:
 
-        $ source env/bin/activate
+    $ python3 -m pip install -U pipx
 
-The prompt will now change to something containing `(env)` to indicate that the virtual environment is active. Updating pip is now recommended:
+Now run:
 
-        (env) $ pip install -U pip
+    $ pipx ensurepath
 
-Note that this invokes `./env/bin/pip`. Once this is finished, use pip to install etm:
+to ensure that directories necessary for *pipx* operation are in your PATH environment variable and finally to install *etm* itself:
 
-        (env) $ pip install -U etm-dgraham
+    $ pipx install etm-dgraham
 
-This will install etm and all its requirements in
+(To upgrade *etm* when a new version becomes available, simply replace "install" in this command with "upgrade".) You can then start *etm* as before with
 
-		./env/lib/python3.x/sitepackages
-
-and will also install an executable called `etm` in `./env/bin`.You can then start etm using
-
-        (env) $ etm <path to home>
+    $ etm <path to home>
 
 Details about `<path to home>` are in [Home directory](#home-directory).
 
 [↺ contents](#contents)
 
 ### For use system wide {#for-use-system-wide}
 
@@ -1365,28 +1376,30 @@
 
 [↺ contents](#contents)
 
 ## Usage {#usage}
 
 ### Terminal size and color scheme {#terminal-size-and-color-scheme}
 
-The suggested terminal size for etm is 60 (columns) by 32 or more (rows). The default color scheme is best with a dark terminal background. A scheme better suited to light backgrounds can be set using `style: light` in `cfg.yaml` in your home directory. Some of the *etm* display may not be visible unless `style` is set correctly for your display.
+The suggested terminal size for etm is 70 (columns) by 32 or more (rows). The default color scheme is best with a dark terminal background. A scheme better suited to light backgrounds can be set using `style: light` in `cfg.yaml` in your home directory. Some of the *etm* display may not be visible unless `style` is set correctly for your display.
 
 The size of the terminal is used when *etm* starts to set various display options so changing the terminal size, especially reducing the width, is best avoided once *etm* is running.
 
 [↺ contents](#contents)
 
 ### Home directory {#home-directory}
 
 Before you start etm, think about where you would like to keep your personal data and configuration files. This will be your etm *home* directory. The default is to use whatever directory you're in when you start _etm_ as your _etm_ home directory. If you start _etm_ in your virtual environment directory then the default will be to use that as your home directory as well. If this is not what you want, you can just give the path for whatever directory you would like to use when you start _etm_.
 
 	$ etm <path to home>
+
 Finally, if there is an environmental variable, `ETMHOME`, set to this path then you can just enter
 
 	$ etm
+
 and etm will use `ETMHOME` as its home directory.
 
 Home directory considerations:
 
 * If more than one person will be using etm on the same computer, you might want to have different *home* directories for each user.
 * If you want to use etm on more than one computer and use Dropbox, you might want to use `~/Dropbox/etm` to have access on each of your computers.
 * If you want to separate personal and professional reminders, you could use different _home_ directories for each. You can run two instances of _etm_ simultaneously, one for each directory, and have access to both at the same time.
@@ -1403,24 +1416,80 @@
 Here `cfg.yaml` is your user configuration file and `db.json` contains all your etm reminders. The folders `backups/` contains the 7 most recent daily backups of your `db.json` and `cfg.yaml` files. The folder `logs` contains the current `etm.log` file and the 7 most recent daily backups. Note that backup files are only created when the relevant file has been modified since the last backup.
 
 The file `cfg.yaml` can be edited and the options are documented in the file.
 See [configuration](#configuration) for details.
 
 [↺ contents](#contents)
 
+### Timers {#timers}
+
+For tracking time spent, *etm* supports the use of one or more timers. Each timer is associated with a particular reminder and, if a timer is recorded, a used time entry will be added to the associated reminder using this format:
+
+        @u <time spent>: <datetime recorded>
+
+The timer itself records seconds, but the used time entry for `<time spent>` depends upon the `usedtime_minutes` setting in `cfg.yaml` as follows:
+
+- 0: time is recorded in seconds after rounding to the nearest second
+- 1: time is recorded in minutes after rounding off to the nearest minute, e.g., 1m29s => 1m; 1m30s => 2m
+- 6: time is rounded up to the next one-tenth of an hour for reporting but recorded in minutes
+- 12: time is rounded up to the next two-tenths of an hour for reporting but recorded in minutes
+- 30: time is rounded up to the next half hour for reporting but recorded in minutes
+- 60: time is rounded up to the next hour for reporting but recorded in minutes
+
+The [Used Time Views](#used-time-views) show aggregations of these reported times by month and index entry. Any rounding up is done before aggregating.
+
+Used time entries can be recorded directly by editing the relevant reminder and adding one or more `@u` entries. It is also possible to use *etm* to create timers *attached* to particular reminders and control them with hotkeys.
+
+- T: with a reminder selected
+    - If a timer is not already associated with this reminder, then create a new timer and associate it with this reminder
+        - if another timer is active, make this timer inactive
+        - otherwise make this timer active and paused
+    - If a timer is already associated with this reminder
+        - if the timer is inactive, make it active and running
+        - otherwise toggle the state of the timer between paused and running
+- TR: if a reminder is selected with an associated timer
+    - open a dialog to record a used time entry with the current value of the timer and the current datetime
+    - if, after possible editing, recording is confirmed then add the used time entry and delete the timer
+- TD: if a reminder is selected with an associated timer
+    - open a dialog to confirm deleting the timer without recording the used time
+    - if deletion is confirmed then delete the timer
+- TT: if there is an active timer
+    - toggle the paused/running state for the active timer. Note that the reminder associated with the active timer *need not be selected*.
+    - Note that if there are one or more timers, *exactly one of them will be the active timer*, i.e., either running or paused. The others, if any, will be inactive.
+
+[Timer View](#timer-view), bound to `m`, provides a convenient way of manipulating multiple timers. It lists each existing timer with the active timer first and followed by the other timers in the order of most recently active. Pausing/running the active timer can be done from any view by pressing `TT`. To switch to another timer, change to timer view, press `TT` if necessary to pause the active timer, select the timer you want to start and press 'T' to change its state from 'inactive' to 'running'. It will move to the top of the list and the other timers will move down by one row.
+
+When there are one or more timers, their status is always displayed in the status bar. E.g., `r:6.3m + i:1h3.2` would mean that the active timer is running with 6.3m of elapsed time and there are other, inactive timers with a total of 1h3.2m of elapsed time.
+
+[↺ contents](#contents)
+
+### *lorem* examples {#loremexamples}
+
+If you are new to *etm*, you might find it very useful to install the *lorem* examples. If you press `F5`, enter 'lorem' at the prompt and press `return`, *etm* will generate a series of reminders all of which are tagged 'lorem'. These fall within a three month period including the month in which they were created as well as the previous and subsequent months. The examples are designed to illustrate nearly all of the etm views and features. You can play around with the examples as long as you wish and then remove them all at once by pressing `q` to open query view, entering the query 'any t lorem \| remove' and pressing `return`.
+
+These examples are named for and depend upon the python package *lorem* that can generate random words, phrases, sentences and paragraphs in 'lorem ipsum' text. E.g., "Lorem ipsum dolor sit amet, consectetur adipiscing elit ...". This is "a placeholder text commonly used to demonstrate the visual form of a document or a typeface without relying on meaningful content."
+
+[↺ contents](#contents)
+
 ### Using etm+ {#etmplus}
 
 An added bonus of setting `ETMHOME` to the path of your *home* directory is the possibility of using the `etm+` shortcut for creating reminders. E.g., entering
 
 	$ etm+ '* lunch with Peter @s fri 12p'
 would append the line `* lunch with Peter @s fri 12p` to the file `inbasket.text`in `ETMHOME`, creating the file if necessary. `etm+` also accepts input piped to it so that
 
 	$ echo '* lunch with Peter @s fri 12p' | etm+
 would produce exactly the same result.
 
+Finally, if `{T}` is included, it will be replaced with a time stamp corresponding to the moment the script was invoked. E.g.,
+
+	$ echo '% got the test result at {T}' | etm+
+
+would append something like `% got the test result at 2022-12-07 9:13:55 EST`.
+
 Important
 : The single quotes are necessary to keep the shell from expanding the "*" into the names of all the files in the current working directory and other such mischief.
 
 *etm* checks once every minute for the presence of a file named `inbasket.text`in `ETMHOME` and, if found, will display an inbasket character, ⓘ , at the right end of its status bar reminding you that inbasket items are available for importing. Just press F5 in etm to import the reminders from this file and, on successful completion, automatically remove the file.
 
 Note finally that `etm+` will accept quick notes which are not themselves valid etm reminders such as
 
@@ -1471,49 +1540,48 @@
 
 ### event {#event}
 
 Type character: **\***
 
 An event is something that happens at a particular date or datetime without any action from the user. Christmas, for example, is an event that happens whether or not the user does anything about it.
 
-- The `@s` entry is required and can be specified either as a date or as a datetime. It is interpreted as the starting date or datetime of the event.
+- The `@s` entry is required and can be specified either as a date or as a datetime. It is interpreted as the scheduled date or datetime at which the event begins.
 - If `@s` is a date, the event is regarded as an *occasion* or *all-day* event. Such occasions are displayed first on the relevant date.
 - If `@s` is a datetime, an `@e` entry is allowed and is interpreted as the extent or duration of the event - the end of the event is then given implicitly by starting datetime plus the extent and this period is treated as busy time.
 
 Corresponds to VEVENT in the vcalendar specification.
 
 [↺ contents](#contents)
 
 ### task {#task}
 
 Type character: **-**
 
 A task is something that requires action from the user and lasts, so to speak, until the task is completed and marked finished. Filing a tax return, for example, is a task.
 
-- The `@s` entry is optional and, if given, is interpreted as the date or datetime at which the task is due.
-    - Tasks with an `@s` datetime entry are regarded as past due after the datetime and are displayed in *Agenda View* on the relevant date according to the starting time.
+- The `@s` entry is optional and, if given, is interpreted as the date or datetime at which the task is scheduled to be completed.
+    - Tasks with an `@s` datetime entry are regarded as past due after the datetime and are displayed in *Agenda View* on the relevant date according to the scheduled time.
     - Tasks with `@s` date entry are regarded as past due after the due date and are displayed in *Agenda View* on the due date after all items with datetimes.
     - Tasks that are past due are also displayed in *Agenda View* on the current date using the type character `<` with an indication of the number of days that the task is past due.
 - Tasks without an `@s` entry are to be completed when possible and are sometimes called *todos*. They are regarded as *next* items in the *Getting Things Done* terminology and are displayed in *Do Next* view grouped by @l (location/context).
-- Tasks with an `@r` (repeat) entry can have an `@o` (overdue) setting.
-	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. mortage payments to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. Whenever a payment is sent, it applies to the oldest, past due one. This is the default when no `@o` entry is given.
-    - `@o p`: preserve. When an instance becomes past due, a new, non-repeating copy is created with the past due datetime as the `@s` entry and with an `@k` containing the document_id of the original item. Suppose, for example, that minutes are kept for a weekly meeting to be sent to the attendees after each meeting. Creating a task that repeats weekly with `@o p` recognizes the distinction between sending the minutes for `22/10/8` and `22/10/15` and, should both become past due, permits finishing the tasks in any convenient order.
-	- `@o r`: reset. Whenever completed, the next instance is due at the first datetime from the recurrance rule that falls after the current datetime. E.g., getting a haircut every 14 days is due 14 days after the last haircut. With this option, at most one instance can be past due.
-	- `@o s`: skip. Like 'keep' and 'reset' combined with the addition that past due instances are ignored. E.g., taking out the trash every Monday morning for pickup is due every Monday morning but, if a Monday passes without taking out the trash, the instance is better regarded as irrelevant than past due. With this option, an instance can never be past due.
+- Tasks with an `@r` (repeat) or an `@+` entry can have an `@o` (overdue) setting.
+	- `@o k`: keep. Whenever completed, the next instance is due at the datetime specified in the recurrance rule even if that datetime has already passed. E.g. minutes from a monthly meeting to be made on the 1st of the month are due for each prior month in which they have not been made. With this option, many instances can be past due. By default, a completion applies to the oldest, past due one, though other instances can be selected. This is the default when no `@o` entry is given.
+	- `@o r`: reset. Whenever completed, the next instance is due at the first datetime that falls after the current datetime. E.g., getting a haircut every 14 days is due 14 days after the last haircut. With this option, at most one instance can be past due.
+	- `@o s`: skip. Like 'keep' with the addition that past due instances are ignored. E.g., taking out the trash every Monday morning for pickup is due every Monday morning but, if a Monday passes without taking out the trash, the instance is better regarded as irrelevant than past due. With this option, an instance can never be past due.
 
 	    Furthermore, if the options setting `limit_skip_display` were true, then only the first instance of such a task would be displayed in agenda view. E.g., with the `limit_skip_display` setting true, then for the task
 
 			- meds @s +0d @r d &h 8,14,20 @o s
 
 		agenda view at 10am today would only display the first, 2pm (14h) instance of this task. If, on the other hand, this setting were false, then agenda view would display not only the 2pm instance but also the 8pm (20h) instances and all three instances on every future date.
 
 - Jobs
     - Tasks, both with and without @s entries can have component jobs using @j entries.
-    - For tasks with an @s entry, jobs can have an &s entry to set the due date/datetime for the job. It is entered as a timeperiod relative to  the starting datetime (+ before or - after) for the task. Zero minutes is the default when &s is not entered.
-    - For tasks with an @s entry, jobs can also have &a, alert, and &b, beginning soon, notices. The entry for &a is given as a time period relative to &s (+ before or - after) and the entry for &b is a positive integer number of days before the starting date/time to begin displaying "beginning soon" notices. The entry for @s in the task becomes the default for &s in each job.  E.g., with
+    - For tasks with an @s entry, jobs can have an &s entry to set the due date/datetime for the job. It is entered as a timeperiod relative to  the scheduled datetime (+ before or - after) for the task. Zero minutes is the default when &s is not entered.
+    - For tasks with an @s entry, jobs can also have &a, alert, and &b, beginning soon, notices. The entry for &a is given as a time period relative to &s (+ before or - after) and the entry for &b is a positive integer number of days before the scheduled date/time to begin displaying "beginning soon" notices. The entry for @s in the task becomes the default for &s in each job.  E.g., with
 
             - beginning soon example @s 1/30/2018
                 @j job A &s 5d &b 10
                 @j job B &b 5
 
         Beginning soon notices would begin on Jan 15 for job A (due Jan 25) and on January 25 for job B (due Jan 30).
     - Prerequisites
@@ -1581,15 +1649,15 @@
 
 [↺ contents](#contents)
 
 ### inbox {#inbox}
 
 Type character: **!**
 
-An inbox item can be regarded as a task that is always due on the current date. E.g., you have created an event to remind you of a lunch meeting but need to confirm the time. Just record it using **!** instead of **\*** and the entry  will appear highlighted in the agenda view on the current date until you confirm the starting time.
+An inbox item can be regarded as a task that is always due on the current date. E.g., you have created an event to remind you of a lunch meeting but need to confirm the time. Just record it using **!** instead of **\*** and the entry  will appear highlighted in the agenda view on the current date until you confirm the scheduled time.
 
 Corresponds to VTODO in the vcalendar specification.
 
 [↺ contents](#contents)
 
 ### status {#status}
 
@@ -1597,15 +1665,15 @@
 
 [↺ contents](#contents)
 
 #### beginning soon {#beginning-soon}
 
 Type character: **>**
 
-For unfinished tasks and other items with `@b` entries, when the starting date given by `@s` is within `@b` days of the current date, a warning that the item is beginning soon appears on the current date together with the item summary and the number of days remaining until the current date.
+For unfinished tasks and other items with `@b` entries, when the scheduled date given by `@s` is within `@b` days of the current date, a warning that the item is beginning soon appears on the current date together with the item summary and the number of days remaining until the current date.
 
 [↺ contents](#contents)
 
 #### past due {#past-due}
 
 Type character: **<**
 
@@ -1649,15 +1717,15 @@
 @ keys
 </h3>
 
 `@` followed by a character from the list below and a value appropriate to the key is used to apply attributes to an item. E.g.,
 
             @s mon 9a
 
-would specify the the starting datetime for the item is 9am on the Monday following the current date.
+would specify the the scheduled datetime for the item is 9am on the Monday following the current date.
 
 *  @+: include. list of datetimes to include
 *  @-: exclude. list of datetimes to exclude
 *  @a*: alert. list of + (before) or - (after) periods: list of commands
 *  @b: beginby. integer (number of days before)
 *  @c: calendar. string
 *  @d: description. string
@@ -1671,30 +1739,30 @@
 *  @l: location (aka context). forward slash delimited string. E.g., home/maintenance
 *  @m: mask. string stored in obfuscated form
 *  @n*: attendee. string using "[name:] address" format. If "address" begins with exactly 10 digits followed by an "@" it is treated as a mobile phone number. Otherwise it is treated as an email address. The optional "name:" can be used to facilitate autocompletion.
 *  @o: overdue. character from (r) restart, (s) skip, (k) keep, (p) preserve
 *  @p: priority. integer from 0 (none), 1 (low), 2 (normal), 3 (high), 4 (urgent)
 *  @r*: repetition frequency, a character from (y)early, (m)onthly, (w)eekly,
   (d)aily, (h)ourly or mi(n)utely, optionally followed by repetition &key entries
-*  @s: start. date or datetime
+*  @s: scheduled date or datetime
 *  @t*: tag. string
 *  @u*: usedtime. string using "timeperiod spent: ending datetime" format
 *  @w: wrap. A pair of before and after timeperiods to extend the busy period for an event, e.g., for travel time to and/or from the location of the event. Use `0m` as one of the timeperiods to avoid a wrap in that direction.
 *  @x*: expansion. string
 *  @z: timezone. string. A timezone specification, such as 'US/Eastern' or 'Europe/Paris' for aware datetimes or 'float', to indicate a naive or floating datetime. Datetime entries in the item are interpreted as belonging to the specified timezone when the entry is saved. The current timezone is the default when @z is not specified. Aware datetimes are converted to UTC (coordinated universal time) when stored and the @z entry, now irrelevant, is discarded.
 
 <h3 id="ampkeys">
 & keys
 </h3>
 
 & followed by a character from one of the lists below. These keys are only used with @j (job) and @r (repetition) entries.
 
 For use with @j:
 
-*  &s: start/due: period relative to @s entry (default 0m)
+*  &s: scheduled: period relative to @s entry (default 0m) at which job is scheduled to be completed
 *  &a: alert: list of + (before) or - (after) periods relative to &s: list of cmd names from the users configuration file
 *  &b: beginby. integer number of days before &s
 *  &d: description. string
 *  &e: extent. period
 *  &f: finished. datetime
 *  &l: location/context. string
 *  &m: masked. string stored in obfuscated form
@@ -1722,16 +1790,16 @@
 ## Notes {#notes}
 
 ### notices {#notices}
 
 * A link character, 'g', is appended to the *flags* column of any reminder with an `@g` goto link. Press `^g` with such a reminder selected to have the operating system open the link using the default application if the link can be interpreted as a file path or a url. E.g. if the link is a URL, then it would be opened using the default browser. If link can be interpreted as a shell command followed by arguments, then the command would be executed with the arguments.
 * An in-basket character, ⓘ , is appended to the right end of the status bar when a file named 'inbasket.text' is found in the etm root directory. This file should contain lines containing etm reminder entries - one on each line. It can be imported using the import file command bound to F5.
 * An update available character, 𝕦, is appended to the right end of the status bar when checking for updates is enabled and a later version of etm is available. Details for enabling checking for updates are in [configuration](#configuration).
-* Alerts and beginbys can be added to any reminder with an `@s` start date/time entry. Alerts require a datetime in `@s`; beginbys also allow a date in `@s`.
-* A beginby is specified by adding `@b n` to a reminder where `n` is a positive integer and is interpreted as a number of days. A reminder with such an entry will be displayed in *agenda view* on the current date provided that the current date is no more than `n` days before the start date/time of the reminder. Such a warning will appear n days before, n-1 days before and so forth until 1 day before the starting date/time of the reminder. The warning displays the type character `>`, the summary of the reminder and the number of days remaining.
+* Alerts and beginbys can be added to any reminder with an `@s` scheduled date/time entry. Alerts require a datetime in `@s`; beginbys also allow a date in `@s`.
+* A beginby is specified by adding `@b n` to a reminder where `n` is a positive integer and is interpreted as a number of days. A reminder with such an entry will be displayed in *agenda view* on the current date provided that the current date is no more than `n` days before the scheduled date/time of the reminder. Such a warning will appear n days before, n-1 days before and so forth until 1 day before the scheduled date/time of the reminder. The warning displays the type character `>`, the summary of the reminder and the number of days remaining.
 * An alert is specified by adding `@a <list of time periods>: <list of commands>` to a reminder. The time periods must be given in the usual etm format, e.g., `1h13m` for one hour and 13 minutes. The commands are single alphabetic characters, e.g., `a`, `b` and such. The commands used must either be `e` (email) or `t` (text) or be specified in the `alerts` section of the `cfg.yaml` file in your etm home directory. See [configuration](#configuration) for details about this file. Basically, it associates a command, such as `v` with a shell command to be invoked when an alert that includes `v` is triggered. E.g., the alert
 
 			@a 20m: v
 
     would be triggered 20 minutes before the datetime specified in the reminder's `@s` entry and at that time the shell command associated with `v` would be invoked. Both positive (before) and negative (after) time periods can be used. Thus this entry
 
 			@a 1d, -1h: v, w
@@ -1881,47 +1949,51 @@
 ### configuration {#configuration}
 
 Configuration settings for *etm* are specified in the file `cfg.yaml` located in your etm *home directory*. See [installation](#installation) for the location of this directory. When *etm* is running, you can press `F8` to open this configuration file using your system default editor for *yaml* (text) files. Note that any changes you make will not become effective until you stop and restart *etm*.
 
 Here are the options with their default values from that file. The lines beginning with `#` are comments that describe the settings.
 
     #### begin cfg.yaml ####
-	version: 4.9.1
-	# The current version of etm and this file. DO NOT EDIT. This is
-	# automatically updated when a new version of etm is installed.
+    etmversion: 4.11.18
+    # The current version of etm and this file. DO NOT EDIT. This is
+    # automatically updated when a new version of etm is installed.
 
     ampm: true
     # true or false. Use AM/PM format for datetimes if true else
-    # use 24 hour format.
+    # use 24 hour format. See also the show_minutes setting.
+
+    show_minutes: false
+    # true or false. If true show ":00" in agenda and forthcoming views
+    # when displaying times with zero minutes else suppress zero minutes
+    # from being displayed. E.g., "9:00-10:30" if true else "9-10:30".
+    # When ampm if false and show_minutes is true, hours will be displayed
+    # with leading zeros applicable.
 
-    dayfirst:  true
+    dayfirst:  false
     yearfirst: true
-    # true or false. Whenever an ambiguous date is parsed, dayfirst
+    # each true or false. Whenever an ambiguous date is parsed, dayfirst
     # and yearfirst parameters control how the information is processed
     # using this precedence:
-    #
-    #   If dayfirst is False and yearfirst is False:
-    #       MM-DD-YY
-    #       DD-MM-YY
-    #       YY-MM-DD
-    #
-    #   If dayfirst is True and yearfirst is False:
-    #       DD-MM-YY
-    #       MM-DD-YY
-    #       YY-MM-DD
-    #
-    #   If dayfirst is False and yearfirst is True:
-    #       YY-MM-DD
-    #       MM-DD-YY
-    #       DD-MM-YY
-    #
-    #   If dayfirst is True and yearfirst is True:
-    #       YY-MM-DD
-    #       DD-MM-YY
-    #       MM-DD-YY
+    # yearfirst: true
+    # 	dayfirst: true  => YDM
+    #   dayfirst: false => YMD
+    # yearfirst: false
+    # 	dayfirst: true  => DMY
+    #   dayfirst: false => MDY
+    # E.g., with both true, 3/4/5 would be interpreted as May 4, 2003.
+    # When possible, dates will also be displayed respecting these settings.
+    # I.e., the year will generally be displayed first when yearfirst is
+    # true and last otherwise. Similarly, the day will generally be displayed
+    # before the month when dayfirst is true and after the month otherwise.
+
+    beginbusy: 7
+    # non-negative integer. The number of hours after midnight to begin the
+    # busy view display of busy times for each day. The display continues
+    # for 14 hours after the begin_busy hour. E.g. with 'begin_busy: 7' the
+    # display would show busy times from 7am (7h) until 9pm (21h).
 
     updates_interval: 0
     # non-negative integer. If positive,  automatically check for updates
     # every 'updates_interval' minutes. If zero, do not automatically
     # check for updates. When enabled, a blackboard u symbol, 𝕦, will be
     # displayed at the right end of status bar when an update is available
     # or a question mark when the check cannot be completed as, for
@@ -1932,34 +2004,36 @@
     # for English (United States), "fr_FR" for French (France) and so
     # forth. Google "python locale abbreviatons" for a complete list."
 
     vi_mode: false
     # true or false. Use vi keybindings for editing if true else use emacs
     # style keybindings.
 
-    secret: KFI9R2AAaw
+    secret: HIr13FiYj3
     # string to use as the secret_key for @m masked entries. E.g.
     # 'X6i2SGWu6m'. In etm versions after 4.0.21, the default string is
     # randomly generated when this file is created or when the secret
     # value is removed and etm is restarted. WARNING: if this key is
     # changed, any @m entries that were made before the change will be
     # unreadable after the change.
 
     omit_extent:
     # A list of calendar names. Events with @c entries belonging to this
     # list will only have their starting times displayed in agenda view
     # and will neither appear nor cause conflicts in busy view.
 
-    keep_current: 0
-    # non-negative integer. If positive, the agenda for that integer
-    # number of weeks starting with the current week will be written to
-    # "current.txt" in your etm home directory and updated when necessary.
-    # You could, for example, create a link to this file in a pCloud or
-    # DropBox folder and have access to your current schedule on your
-    # mobile device.
+    keep_current: [0, 47]
+    # A list of two, non-negative integers for "weeks" and "width". If
+    # weeks is positive, the agenda for that integer number of weeks
+    # starting with the current week will be written to "current.txt" in
+    # your etm home directory and updated when necessary. The format will
+    # be scaled to fit "width". A width of 50, e.g, fits an iPhone display
+    # in portrait mode. You could, for example, create a link to
+    # "current.txt" in a pCloud or GoogleDrive folder and always have access
+    # to your current agenda on your mobile device.
 
     keep_next: false
     # true or false. If true, the 'do next' view will be written to
     # "next.txt" in your etm home directory. As with "current.txt", a link
     # to this file could be created in a pCloud or DropBox folder for
     # access from your mobile device.
 
@@ -1989,34 +2063,56 @@
     # current time.
 
     connecting_dots: false
     # true or false. If true, display dots connecting the item summary and
     # the right-hand details columns in tree views.
 
     usedtime_minutes: 1
-    # 1, 6, 12, 30 or 60. Round used times up to the nearest
-    # usedtime_minutes in used time views. With 1, no rounding is done and
-    # times are reported as hours and minutes. Otherwise, the prescribed
-    # rounding is done and times are reported as floating point hours.
-    # Note that each "@u" timeperiod is rounded before aggregation.
+    # 0, 1, 6, 12, 30 or 60. Round up used times. With 0, no rounding is done
+    # and times are reported in hours, minutes and seconds. With 1, after
+    # rounding up to the nearest minute, times are reported as hours and minutes.
+    # Otherwise, rounding is up to the nearest integer multiple of
+    # usedtime_minutes and times are reported as floating point hours. E.g.,
+    # with usedtime_minutes = 6, 1 minute would be rounded up to 6 minutes and
+    # reported as 0.1 hours. Similarly 13 minutes would be rounded up to 18
+    # minutes and reported as 0.3 hours. Note that when rounding is specified,
+    # each "@u" timeperiod is rounded before aggregation.
+
+    usedtime_hours: 6
+    # 0, 1, 2, ..., 24. The daily goal for used time. This is used in engaged
+    # view to control the display of the daily used time bars. The goal is to
+    # to maximize the granularity of the bar when displaying this number of hours
+    # in the space allowed by the terminal width.
+
+    journal_name: daily
+    # Journal items with this index entry and with an @s entry will have the
+    # year and month appended to the index. E.g., with the setting
+    #   journal_name: daily
+    # this journal entry
+    #   % visited Yellowstone @s 22/6/24 @i daily
+    # would be displayed in journal view as if the index entry were
+    #   @i daily/2022/ 6
+    # thus organizing such entries by the year and month of their scheduled dates.
+    # Within each month, entries will be also ordered by the month day.
 
     alerts:
     # A dictionary with single-character, "alert" keys and corresponding
     # "system command" values. Note that characters "t" (text message) and
     # "e" (email) are already used.  The "system command" string should be
     # a comand with any applicable arguments that could be run in a
     # terminal. Properties of the item triggering the alert can be
     # included in the command arguments using the syntax {prop}, e.g.,
     # {summary} in the command string would be replaced by the summary of
-    # the item. Similarly {start} by the starting time, {when} by the time
-    # remaining until the starting time, {location} by the @l entry and
-    # {description} by the @d entry. E.g., If the event "* sales meeting
-    # @s 2019-02-12 3p" triggered an alert 30 minutes before the starting
-    # time the string "{summary} {when}" would expand to "sales meeting in
-    # 30 minutes". E.g. on my macbook
+    # the item. Similarly {start} by the starting datetime, {time} by the
+    # starting time (omits the date for the current date), {when} by the time
+    # remaining until the starting datetime, {now} by the current time,
+    # {location} by the @l entry and {description} by the @d entry. E.g., If
+    # the event "* sales meeting @s 2019-02-12 3p" triggered an alert 30 minutes
+    # before the starting time the string "{summary} {when}" would expand to
+    # "sales meeting in 30 minutes". E.g. on my macbook
     #
     #    alerts:
     #        v:   /usr/bin/say -v "Alex" "{summary}, {when}"
     #        ...
     #
     # would make the alert 'v' use the builtin text to speech sytem
     # to speak the item's summary followed by a slight pause
@@ -2033,18 +2129,18 @@
     #        ...
     #
     # then when "@x tennis" is entered the popup completions for
     # "@x tennis" would offer replacement by the corresponding
     # "@e 1h30m @a 30m: d @i personal:exercise".
 
     sms:
-      body: "{location} {when}"
-      from:
-      server:
-      pw:
+    body: '{location} {when}'
+    from:
+    server:
+    pw:
     # Settings to send "t" (sms text message) alerts to the
     # list of phone numbers from the item's @n attendee
     # entries using the item's summary and the body as specified
     # in the template below as the message. E.g., suppose you
     # have a gmail account with email address "who457@gmail.com"
     # and want to text alerts to Verizon moble phone (123)
     # 456-7890. Then your sms entries should be
@@ -2057,19 +2153,19 @@
     # gateway for Verizon. Other common mms gateways are
     #     AT&T:     @mms.att.net
     #     Sprint:   @pm.sprint.com
     #     T-Mobile: @tmomail.net
     # Note. Google "mms gateway listing" for other alternatives.
 
     smtp:
-      body: "{location} {when}\n{description}"
-      from:
-      server:
-      id:
-      pw:
+    body: '{location} {when}\n{description}'
+    from:
+    server:
+    id:
+    pw:
     # Settings to send "e" (email message) alerts to the list of email
     # addresses from the item's @n attendee entries using the item's
     # summary as the subject and body as the message. E.g., if you have a
     # gmail account with email address "whatever457@gmail.com", then your
     # entries should be
     #     from: whatever457@gmail.com
     #     id: whatever457
@@ -2094,14 +2190,18 @@
     # values. Each "query" must be one that could be entered as the
     # command in query view. Keys can be any short string other than
     # 'a', 'u', 'c' or 'l' which are already in use.
     # queries:
     #    td: m l -q equals itemtype - and ~exists f
     #    mi: exists u and ~exists i
     #    arch: a exists itemtype
+    #    find: includes summary d {}
+    # The latter would allow you to enter, e.g., `find waldo` and have
+    # it expand to `includes summary d waldo` and thus locate all
+    # reminders with `waldo` either in the summary or d (the description).
 
     style: dark
     # dark or light. Set the defaults for dark or light terminal
     # backgounds. Some output may not be visible unless this is set
     # correctly for your display.
 
     type_colors:
@@ -2116,30 +2216,35 @@
     #  event           'LimeGreen',        'DarkGreen',
     #  finished        'DarkGrey',         'LightSlateGrey',
     #  inbox           'OrangeRed',        'MediumVioletRed',
     #  journal         'GoldenRod',        'Brown',
     #  pastdue         'LightSalmon',      'Red',
     #  plain           'Ivory',            'Black',
     #  today           'Ivory bold',       'Black bold',
+    #  used            'Khaki',            'DodgerBlue',
     #  waiting         'SlateGrey',        'DarkSlateBlue',
-	#  wrap            'SlateGrey',        'DarkSlateBlue',
-    #
+    #  wrap            'ForestGreen',      'LightGrey',
+    #  running         'OrangeRed',        'Gold',
+    #  paused          'MediumVioletRed',   'DarkViolet',
     # Explanations for the key names:
     #     available:    available task/job reminders
     #     begin:        begin by warnings
     #     event:        event reminders
     #     finished:     finished task/job reminders
     #     inbox:        inbox reminders
     #     journal:      journal reminders
     #     pastdue:      pasdue task warnings
     #     plain:        headings such as outline branches
     #     today:        the current and following agenda date headings
+    #     used:         used time rows in engaged and used time views
     #     waiting:      waiting job reminders (jobs with unfinished prereqs)
-	#     wrap:         before and after rows for events in agenda view with
-	#                   @w entries
+    #     wrap:         before and after rows for events in agenda view with
+    #                   @w entries
+    #     running:      status bar color for 'r', running timer
+    #     paused:       status bar color for 'p', paused timer
     #
     # E.g., with style 'dark', the default color for 'available' is
     # 'LightSkyBlue'. This entry
     #   colors:
     #       available: CornFlowerBlue
     # would change the 'available' color to 'CornflowerBlue' while leaving
     # the other 'dark' colors unchanged.
@@ -2155,15 +2260,15 @@
     #    [background, foreground, attribute]
     # components. background and foreground can either be named colors,
     # hex colors, or ''. Attribute is an optional font attribute such
     # as 'bold' which must, of course, be supported by the font used in
     # your terminal. The default settings are determined by the 'dark'
     # or 'light' style setting as follows:
     #
-    #    key                           dark                        light
+    #    key                       dark default                  light default
     # -------------------    -----------------------------  -----------------------------
     # ask:                    [grey2, Lime, bold]           [Cornsilk, Lime, bold]
     # button.focused:         [DarkGreen, White]            [DarkGreen, White]
     # details:                [, Ivory]                     [, Black]
     # dialog shadow:          [#444444, ]                   [#444444, ]
     # dialog:                 [DarkSlateGrey, White]        [DimGrey, White]
     # dialog-entry:           [White, Black]                [White, Black]
@@ -2189,20 +2294,23 @@
     #
     # Note that 'grey1' (#396060) and 'grey2' (#1d3030) are colors named
     # within etm itself. They are, respectively, one shade lighter and two
     # shades darker than DarkSlateGrey.
     #
     # Any of the style attributes above can be modified. E.g., with style
     # 'dark', the default for 'text-area' is [grey2, Ivory]. This entry
-    #   style_modifications:
+    #   window_colors:
     #       text-area: [Black, White]
     # would change the 'text-area' setting to 'Black' as the background color
     # and 'White' as the foreground color while leaving the other style settings
     # unchanged.
-	#### end cfg.yaml ####
+    #### end cfg.yaml ####
+
+
+See [Saved Queries](#saved-queries) for more information about queries that allow for replaceable parameters.
 
 Note that in the 'dictionary' entries above, the components must be indented (using 2 spaces not tabs). E.g., the illustrative alert entry would be:
 
 	alerts:
 		v: /usr/bin/say -v "Alex" "{summary}, {when}"
 
 
@@ -2249,8 +2357,8 @@
 
 Consider the entry `2019-12-23` for `@s`. To *etm* this is a pendulum date object. When *etm* stores this record, *TinyDB* recognizes that this attribute is a pendulum date object and encodes/serializes it as the string `"{D}:20191223"`. When *etm* retrieves this record from storage, *TinyDB* recognizes from the `{D}` that it is to be decoded and returned as a pendulum date object. All this is completely transparent - *etm* gives a date object to *TinyDB* which stores it as a string and when *etm* wants it back, *TinyDB* deserializes it and returns it as a date object.
 
 As another example, When the reminder is created by *etm* the `created` timestamp is handed to *TinyDB* as an aware pendulum datetime object with US/Eastern as the timezone. *TinyDB* recognizes this and, because it is an aware datetime, first converts it to Universal time and then encodes/serializes it as `"{T}:20191221T1526A"`. The `{T}` indicates that it is a datetime object and the appended `A` indicates that it is aware and thus has been converted to Universal time. When *etm* retrieves this record, *TinyDB* recognizes from the `{T}` and the `A` that this is an aware datetime object, decodes it as an aware datetime object and, because it is aware, converts it from Universal time to whatever the current local timezone happens to be before returning it. Had this been a naive datetime, an `N` would have been appended to the serialization and no conversion would have been done either way.
 
 These **date** and **datetime** serializations are extensions of *TinyDB* provided by *etm*. Three further extensions are also provided: **interval** for *pendulum duration* objects using the tag `{I}`, **weekday** for  *dateutil* weekday objects using the tag `{W}` and **mask** using the tag `{M}` for encoding/serializing *etm* strings in a masked or obfuscated manner.
 
-[↺ contents](#contents)
+[↺ contents](#contents)
```

### Comparing `etm-dgraham-4.9.7/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.0.3/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.0.3/etm_dgraham.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 docs/index_usedtime.md
 docs/multiple_timers.md
 etm/__init__.py
 etm/__main__.py
 etm/__version__.py
 etm/data.py
 etm/ical.py
+etm/make_examples.py
 etm/model.py
 etm/options.py
 etm/report.py
 etm/view.py
 etm_dgraham.egg-info/PKG-INFO
 etm_dgraham.egg-info/PKG-INFO [conflicted]
 etm_dgraham.egg-info/SOURCES [conflicted].txt
@@ -32,9 +33,8 @@
 etm_dgraham.egg-info/requires.txt
 etm_dgraham.egg-info/top_level [conflicted].txt
 etm_dgraham.egg-info/top_level.txt
 test/test_parser.py
 utilities/colons_to_slashes.py
 utilities/etm_in
 utilities/inbasket
-utilities/make_examples.py
 utilities/open_in_mutt
```

### Comparing `etm-dgraham-4.9.7/etmlogo.png` & `etm-dgraham-5.0.3/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/etmlogo_small.png` & `etm-dgraham-5.0.3/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/etmview_agenda.png` & `etm-dgraham-5.0.3/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/namedcolors.py` & `etm-dgraham-5.0.3/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/new.png` & `etm-dgraham-5.0.3/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/setup.py` & `etm-dgraham-5.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 REQUIRES_PYTHON = '>=3.7.3'
 VERSION = version
 
 # What packages are required for this module to be executed?
 REQUIRED = [
         "icalendar>=4.0.3",
         "Jinja2>=2.10",
+        "lorem>=0.1.1",
         "MarkupSafe>=1.1.0",
         "pendulum>=2.0.4",
         "prompt-toolkit>=3.0.2",
         "Pygments>=2.5.2",
         "pyperclip>=1.7.0",
         "python-dateutil>=2.7.3",
         "pytz>=2018.9",
@@ -37,15 +38,16 @@
         "requests>=2.25.1",
         "six>=1.11.0",
         "style>=1.1.6",
         "tinydb>=3.12.2",
         "tinydb-serialization>=1.0.4",
         "tinydb-smartcache>=1.0.2",
         "tzlocal>=1.5.1",
-        "wcwidth>=0.1.7"
+        "wcwidth>=0.1.7",
+        "packaging>=22.0"
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
@@ -115,24 +117,18 @@
             self.status('Removing previous builds…')
             rmtree(os.path.join(here, 'dist'))
         except OSError as e:
             print("error removing dist tree:", e)
 
         self.status('Building Source and Wheel (universal) distribution…')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-        # os.system('{0} setup.py sdist'.format(sys.executable))
 
         self.status('Uploading the package to PyPI via Twine…')
         os.system('twine upload --verbose --repository-url https://upload.pypi.org/legacy/ dist/*')
 
-
-        # self.status('Pushing git tags…')
-        # os.system('git tag v{0}'.format(about['__version__']))
-        # os.system('git push --tags')
-
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
     version=about['__version__'],
@@ -149,21 +145,17 @@
     # py_modules=['mypackage'],
     entry_points={
         'console_scripts': [
             'etm=etm.__main__:main',
             'etm+=etm.__main__:inbasket',
         ],
     },
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='GPL',
     classifiers=CLASSIFIERS,
-    # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
 )
```

### Comparing `etm-dgraham-4.9.7/test/test_parser.py` & `etm-dgraham-5.0.3/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/utilities/colons_to_slashes.py` & `etm-dgraham-5.0.3/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/utilities/etm_in` & `etm-dgraham-5.0.3/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/utilities/inbasket` & `etm-dgraham-5.0.3/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-4.9.7/utilities/open_in_mutt` & `etm-dgraham-5.0.3/utilities/open_in_mutt`

 * *Files identical despite different names*

