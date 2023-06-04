# Comparing `tmp/flika-0.2.9.tar.gz` & `tmp/flika-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flika-0.2.9.tar", last modified: Fri Mar 31 03:04:48 2017, max compression
+gzip compressed data, was "flika-0.3.0.tar", last modified: Sun Jun  4 16:11:24 2023, max compression
```

## Comparing `flika-0.2.9.tar` & `flika-0.3.0.tar`

### file list

```diff
@@ -1,103 +1,88 @@
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/app/
--rw-rw-rw-   0        0        0    12589 2017-03-30 23:08:44.000000 flika-0.2.9/flika/app/application.py
--rw-rw-rw-   0        0        0     5001 2017-03-21 17:03:55.000000 flika-0.2.9/flika/app/ipythonWidget.ui
--rw-rw-rw-   0        0        0     5329 2017-03-27 18:08:19.000000 flika-0.2.9/flika/app/main.ui
--rw-rw-rw-   0        0        0    21250 2017-03-27 18:11:57.000000 flika-0.2.9/flika/app/plugin_manager.py
--rw-rw-rw-   0        0        0     8407 2017-03-27 18:08:25.000000 flika-0.2.9/flika/app/plugin_manager.ui
--rw-rw-rw-   0        0        0     9884 2017-03-27 18:05:51.000000 flika-0.2.9/flika/app/script_editor.py
--rw-rw-rw-   0        0        0      783 2017-03-30 23:08:44.000000 flika-0.2.9/flika/app/script_namespace.py
--rw-rw-rw-   0        0        0     7368 2017-03-27 18:42:46.000000 flika-0.2.9/flika/app/settings_editor.py
--rw-rw-rw-   0        0        0     6243 2017-03-21 17:03:55.000000 flika-0.2.9/flika/app/syntax.py
--rw-rw-rw-   0        0        0    10593 2017-03-27 18:08:31.000000 flika-0.2.9/flika/app/terminal.py
--rw-rw-rw-   0        0        0        0 2017-03-21 17:03:55.000000 flika-0.2.9/flika/app/__init__.py
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/docs/
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/docs/_build/
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      756 2017-03-23 16:42:34.000000 flika-0.2.9/flika/docs/_build/html/_static/comment-bright.png
--rw-rw-rw-   0        0        0      829 2017-03-23 16:42:34.000000 flika-0.2.9/flika/docs/_build/html/_static/comment-close.png
--rw-rw-rw-   0        0        0      641 2017-03-23 16:42:34.000000 flika-0.2.9/flika/docs/_build/html/_static/comment.png
--rw-rw-rw-   0        0        0      222 2017-03-23 16:42:34.000000 flika-0.2.9/flika/docs/_build/html/_static/down-pressed.png
--rw-rw-rw-   0        0        0      202 2017-03-23 16:42:34.000000 flika-0.2.9/flika/docs/_build/html/_static/down.png
--rw-rw-rw-   0        0        0    16446 2017-03-21 17:03:55.000000 flika-0.2.9/flika/docs/_build/html/_static/favicon.ico
--rw-rw-rw-   0        0        0      286 2017-03-23 16:42:34.000000 flika-0.2.9/flika/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0     4660 2017-03-21 17:03:55.000000 flika-0.2.9/flika/docs/_build/html/_static/flika.png
--rw-rw-rw-   0        0        0     2944 2017-03-23 19:33:44.000000 flika-0.2.9/flika/docs/_build/html/_static/flika_logo.png
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/docs/_build/html/_static/img/
--rw-rw-rw-   0        0        0    16446 2017-03-21 17:03:55.000000 flika-0.2.9/flika/docs/_build/html/_static/img/favicon.ico
--rw-rw-rw-   0        0        0     2944 2017-03-23 19:33:44.000000 flika-0.2.9/flika/docs/_build/html/_static/img/flika.png
--rw-rw-rw-   0        0        0     2944 2017-03-23 19:33:44.000000 flika-0.2.9/flika/docs/_build/html/_static/img/flika_logo.png
--rw-rw-rw-   0        0        0       90 2017-03-23 16:42:34.000000 flika-0.2.9/flika/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2017-03-23 16:42:34.000000 flika-0.2.9/flika/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0      214 2017-03-23 16:42:34.000000 flika-0.2.9/flika/docs/_build/html/_static/up-pressed.png
--rw-rw-rw-   0        0        0      203 2017-03-23 16:42:34.000000 flika-0.2.9/flika/docs/_build/html/_static/up.png
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/docs/_static/
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/docs/_static/img/
--rw-rw-rw-   0        0        0    16446 2017-03-21 17:03:55.000000 flika-0.2.9/flika/docs/_static/img/favicon.ico
--rw-rw-rw-   0        0        0     2944 2017-03-23 19:33:44.000000 flika-0.2.9/flika/docs/_static/img/flika_logo.png
--rw-rw-rw-   0        0        0     4035 2017-03-31 02:48:05.000000 flika-0.2.9/flika/flika.py
--rw-rw-rw-   0        0        0     7589 2017-03-27 18:09:41.000000 flika-0.2.9/flika/global_vars.py
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/images/
--rw-rw-rw-   0        0        0      616 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/check.png
--rw-rw-rw-   0        0        0      882 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/exclamation.png
--rw-rw-rw-   0        0        0    16446 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/favicon.ico
--rw-rw-rw-   0        0        0     4660 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/favicon.png
--rw-rw-rw-   0        0        0     1357 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/freehand.png
--rw-rw-rw-   0        0        0     2023 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/line.png
--rw-rw-rw-   0        0        0     2596 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/mouse.png
--rw-rw-rw-   0        0        0     1106 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/point.png
--rw-rw-rw-   0        0        0      958 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/rect.png
--rw-rw-rw-   0        0        0    10924 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/rect_line.png
--rw-rw-rw-   0        0        0     4327 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/refresh.png
--rw-rw-rw-   0        0        0      572 2017-03-21 17:03:55.000000 flika-0.2.9/flika/images/search.png
--rw-rw-rw-   0        0        0      795 2017-03-27 18:05:51.000000 flika-0.2.9/flika/images/__init__.py
--rw-rw-rw-   0        0        0      289 2017-03-22 02:38:31.000000 flika-0.2.9/flika/logger.py
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/process/
--rw-rw-rw-   0        0        0    16165 2017-03-27 18:05:51.000000 flika-0.2.9/flika/process/BaseProcess.py
--rw-rw-rw-   0        0        0    23294 2017-03-27 18:05:51.000000 flika-0.2.9/flika/process/binary.py
--rw-rw-rw-   0        0        0     1344 2017-03-27 18:05:51.000000 flika-0.2.9/flika/process/color.py
--rw-rw-rw-   0        0        0    19679 2017-03-30 23:08:44.000000 flika-0.2.9/flika/process/file_.py
--rw-rw-rw-   0        0        0    34755 2017-03-27 18:05:51.000000 flika-0.2.9/flika/process/filters.py
--rw-rw-rw-   0        0        0    10615 2017-03-30 23:08:44.000000 flika-0.2.9/flika/process/math_.py
--rw-rw-rw-   0        0        0     8133 2017-03-27 18:05:51.000000 flika-0.2.9/flika/process/measure.py
--rw-rw-rw-   0        0        0    12466 2017-03-28 21:52:17.000000 flika-0.2.9/flika/process/overlay.py
--rw-rw-rw-   0        0        0     9932 2017-03-27 18:43:04.000000 flika-0.2.9/flika/process/progress_bar.py
--rw-rw-rw-   0        0        0     3900 2017-03-27 18:05:51.000000 flika-0.2.9/flika/process/roi.py
--rw-rw-rw-   0        0        0    20128 2017-03-30 23:08:44.000000 flika-0.2.9/flika/process/stacks.py
--rw-rw-rw-   0        0        0     3662 2017-03-27 18:09:46.000000 flika-0.2.9/flika/process/__init__.py
--rw-rw-rw-   0        0        0    38934 2017-03-30 23:08:44.000000 flika-0.2.9/flika/roi.py
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/tests/
--rw-rw-rw-   0        0        0      171 2017-03-21 22:57:44.000000 flika-0.2.9/flika/tests/conftest.py
--rw-rw-rw-   0        0        0     1201 2017-03-30 23:08:44.000000 flika-0.2.9/flika/tests/test_file.py
--rw-rw-rw-   0        0        0     1732 2017-03-21 23:45:17.000000 flika-0.2.9/flika/tests/test_macros.py
--rw-rw-rw-   0        0        0     8377 2017-03-21 22:57:44.000000 flika-0.2.9/flika/tests/test_processes.py
--rw-rw-rw-   0        0        0     1369 2017-03-21 22:57:44.000000 flika-0.2.9/flika/tests/test_settings.py
--rw-rw-rw-   0        0        0    10797 2017-03-30 23:08:44.000000 flika-0.2.9/flika/tests/test_window.py
--rw-rw-rw-   0        0        0        0 2017-03-21 17:03:55.000000 flika-0.2.9/flika/tests/__init__.py
--rw-rw-rw-   0        0        0    12773 2017-03-30 23:08:44.000000 flika-0.2.9/flika/tracefig.py
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/utils/
--rw-rw-rw-   0        0        0      610 2017-03-21 17:03:55.000000 flika-0.2.9/flika/utils/app.py
--rw-rw-rw-   0        0        0        0 2017-03-21 17:03:55.000000 flika-0.2.9/flika/utils/decorators.py
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika/utils/io/
--rw-rw-rw-   0        0        0   126069 2017-03-21 17:03:55.000000 flika-0.2.9/flika/utils/io/tifffile.py
--rw-rw-rw-   0        0        0        0 2017-03-22 23:28:00.000000 flika-0.2.9/flika/utils/io/__init__.py
--rw-rw-rw-   0        0        0     6068 2017-03-22 23:27:55.000000 flika-0.2.9/flika/utils/misc.py
--rw-rw-rw-   0        0        0      138 2017-03-21 17:03:55.000000 flika-0.2.9/flika/utils/__init__.py
--rw-rw-rw-   0        0        0       21 2017-03-31 03:04:40.000000 flika-0.2.9/flika/version.py
--rw-rw-rw-   0        0        0    24775 2017-03-30 23:08:44.000000 flika-0.2.9/flika/window.py
--rw-rw-rw-   0        0        0      835 2017-03-30 23:08:44.000000 flika-0.2.9/flika/__init__.py
--rw-rw-rw-   0        0        0      148 2017-03-27 18:07:53.000000 flika-0.2.9/flika.desktop
-drwxrwxrwx   0        0        0        0 2017-03-31 03:04:48.000000 flika-0.2.9/flika.egg-info/
--rw-rw-rw-   0        0        0        1 2017-03-31 03:04:48.000000 flika-0.2.9/flika.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2017-03-31 03:04:48.000000 flika-0.2.9/flika.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1420 2017-03-31 03:04:48.000000 flika-0.2.9/flika.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2017-03-31 03:04:48.000000 flika-0.2.9/flika.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2357 2017-03-31 03:04:48.000000 flika-0.2.9/flika.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2017-03-31 03:04:48.000000 flika-0.2.9/flika.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2017-03-21 17:03:55.000000 flika-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1420 2017-03-31 03:04:48.000000 flika-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      537 2017-03-27 18:05:51.000000 flika-0.2.9/README.rst
--rw-rw-rw-   0        0        0       42 2017-03-31 03:04:48.000000 flika-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2836 2017-03-31 03:04:31.000000 flika-0.2.9/setup.py
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.698967 flika-0.3.0/
+-rw-r--r--   0 kylenv     (501) staff       (20)       72 2023-06-03 04:54:52.000000 flika-0.3.0/AUTHORS.rst
+-rw-r--r--   0 kylenv     (501) staff       (20)     1093 2023-06-03 04:54:52.000000 flika-0.3.0/LICENSE
+-rw-r--r--   0 kylenv     (501) staff       (20)       80 2023-06-03 04:54:52.000000 flika-0.3.0/MANIFEST.in
+-rw-r--r--   0 kylenv     (501) staff       (20)     1062 2023-06-04 16:11:24.698760 flika-0.3.0/PKG-INFO
+-rw-r--r--   0 kylenv     (501) staff       (20)      514 2023-06-03 04:54:52.000000 flika-0.3.0/README.rst
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.683241 flika-0.3.0/flika/
+-rw-r--r--   0 kylenv     (501) staff       (20)      215 2023-06-03 04:54:52.000000 flika-0.3.0/flika/__init__.py
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.687219 flika-0.3.0/flika/app/
+-rw-r--r--   0 kylenv     (501) staff       (20)        0 2023-06-03 04:54:52.000000 flika-0.3.0/flika/app/__init__.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    15294 2023-06-03 07:57:41.000000 flika-0.3.0/flika/app/application.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     5662 2023-06-03 04:54:52.000000 flika-0.3.0/flika/app/ipythonWidget.ui
+-rw-r--r--   0 kylenv     (501) staff       (20)     5802 2023-06-03 04:54:52.000000 flika-0.3.0/flika/app/main.ui
+-rw-r--r--   0 kylenv     (501) staff       (20)    23503 2023-06-03 05:01:57.000000 flika-0.3.0/flika/app/plugin_manager.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     8359 2023-06-03 04:54:52.000000 flika-0.3.0/flika/app/plugin_manager.ui
+-rw-r--r--   0 kylenv     (501) staff       (20)    11427 2023-06-03 04:54:52.000000 flika-0.3.0/flika/app/script_editor.py
+-rw-r--r--   0 kylenv     (501) staff       (20)      787 2023-06-03 04:54:52.000000 flika-0.3.0/flika/app/script_namespace.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     8553 2023-06-04 15:58:20.000000 flika-0.3.0/flika/app/settings_editor.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     6128 2023-06-04 03:48:00.000000 flika-0.3.0/flika/app/syntax.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     9476 2023-06-04 03:48:00.000000 flika-0.3.0/flika/app/terminal.py
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.676253 flika-0.3.0/flika/docs/
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.676298 flika-0.3.0/flika/docs/_static/
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.687956 flika-0.3.0/flika/docs/_static/img/
+-rw-r--r--   0 kylenv     (501) staff       (20)    16446 2023-06-03 04:54:52.000000 flika-0.3.0/flika/docs/_static/img/favicon.ico
+-rw-r--r--   0 kylenv     (501) staff       (20)     2944 2023-06-03 04:54:52.000000 flika-0.3.0/flika/docs/_static/img/flika_logo.png
+-rw-r--r--   0 kylenv     (501) staff       (20)     4741 2023-06-03 04:54:52.000000 flika-0.3.0/flika/flika.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     6984 2023-06-04 03:48:00.000000 flika-0.3.0/flika/global_vars.py
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.692184 flika-0.3.0/flika/images/
+-rw-r--r--   0 kylenv     (501) staff       (20)      767 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/__init__.py
+-rw-r--r--   0 kylenv     (501) staff       (20)      616 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/check.png
+-rw-r--r--   0 kylenv     (501) staff       (20)      882 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/exclamation.png
+-rw-r--r--   0 kylenv     (501) staff       (20)    16446 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/favicon.ico
+-rw-r--r--   0 kylenv     (501) staff       (20)     4660 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/favicon.png
+-rw-r--r--   0 kylenv     (501) staff       (20)     1357 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/freehand.png
+-rw-r--r--   0 kylenv     (501) staff       (20)     2023 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/line.png
+-rw-r--r--   0 kylenv     (501) staff       (20)     2596 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/mouse.png
+-rw-r--r--   0 kylenv     (501) staff       (20)     1344 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/pencil.png
+-rw-r--r--   0 kylenv     (501) staff       (20)     1106 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/point.png
+-rw-r--r--   0 kylenv     (501) staff       (20)      958 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/rect.png
+-rw-r--r--   0 kylenv     (501) staff       (20)    10924 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/rect_line.png
+-rw-r--r--   0 kylenv     (501) staff       (20)     4327 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/refresh.png
+-rw-r--r--   0 kylenv     (501) staff       (20)      572 2023-06-03 04:54:52.000000 flika-0.3.0/flika/images/search.png
+-rw-r--r--   0 kylenv     (501) staff       (20)     2154 2023-06-03 04:54:52.000000 flika-0.3.0/flika/logger.py
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.694929 flika-0.3.0/flika/process/
+-rw-r--r--   0 kylenv     (501) staff       (20)     4090 2023-06-03 04:54:52.000000 flika-0.3.0/flika/process/__init__.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    22428 2023-06-04 03:48:00.000000 flika-0.3.0/flika/process/binary.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     1460 2023-06-03 04:54:52.000000 flika-0.3.0/flika/process/color.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    24547 2023-06-04 15:58:20.000000 flika-0.3.0/flika/process/file_.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    40365 2023-06-04 03:48:00.000000 flika-0.3.0/flika/process/filters.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    12915 2023-06-03 04:54:52.000000 flika-0.3.0/flika/process/math_.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     8116 2023-06-03 07:57:41.000000 flika-0.3.0/flika/process/measure.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    12330 2023-06-03 04:54:52.000000 flika-0.3.0/flika/process/overlay.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     9784 2023-06-04 03:48:00.000000 flika-0.3.0/flika/process/progress_bar.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     3529 2023-06-03 04:54:52.000000 flika-0.3.0/flika/process/roi.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    19896 2023-06-03 04:54:52.000000 flika-0.3.0/flika/process/stacks.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    40747 2023-06-04 03:48:00.000000 flika-0.3.0/flika/roi.py
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.696691 flika-0.3.0/flika/tests/
+-rw-r--r--   0 kylenv     (501) staff       (20)        1 2023-06-04 03:48:00.000000 flika-0.3.0/flika/tests/__init__.py
+-rw-r--r--   0 kylenv     (501) staff       (20)      165 2023-06-03 04:54:52.000000 flika-0.3.0/flika/tests/conftest.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     1284 2023-06-03 05:01:57.000000 flika-0.3.0/flika/tests/test_file.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     1657 2023-06-03 05:01:57.000000 flika-0.3.0/flika/tests/test_macros.py
+-rw-r--r--   0 kylenv     (501) staff       (20)      538 2023-06-03 04:54:52.000000 flika-0.3.0/flika/tests/test_misc.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     8073 2023-06-03 04:54:52.000000 flika-0.3.0/flika/tests/test_processes.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     1331 2023-06-03 04:54:52.000000 flika-0.3.0/flika/tests/test_settings.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    12180 2023-06-04 03:48:00.000000 flika-0.3.0/flika/tests/test_window.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    17759 2023-06-04 03:48:00.000000 flika-0.3.0/flika/tracefig.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     5894 2023-06-03 05:01:57.000000 flika-0.3.0/flika/update_flika.py
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.697708 flika-0.3.0/flika/utils/
+-rw-r--r--   0 kylenv     (501) staff       (20)    19215 2023-06-04 15:58:20.000000 flika-0.3.0/flika/utils/BaseProcess.py
+-rw-r--r--   0 kylenv     (501) staff       (20)      108 2023-06-03 04:54:52.000000 flika-0.3.0/flika/utils/__init__.py
+-rw-r--r--   0 kylenv     (501) staff       (20)      905 2023-06-03 07:57:45.000000 flika-0.3.0/flika/utils/app.py
+-rw-r--r--   0 kylenv     (501) staff       (20)      334 2023-06-03 04:54:52.000000 flika-0.3.0/flika/utils/imports.py
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.698056 flika-0.3.0/flika/utils/io/
+-rw-r--r--   0 kylenv     (501) staff       (20)        0 2023-06-03 04:54:52.000000 flika-0.3.0/flika/utils/io/__init__.py
+-rw-r--r--   0 kylenv     (501) staff       (20)   239828 2023-06-04 03:48:00.000000 flika-0.3.0/flika/utils/io/tifffile.py
+-rw-r--r--   0 kylenv     (501) staff       (20)     8964 2023-06-03 05:01:57.000000 flika-0.3.0/flika/utils/misc.py
+-rw-r--r--   0 kylenv     (501) staff       (20)       21 2023-06-04 16:05:06.000000 flika-0.3.0/flika/version.py
+-rw-r--r--   0 kylenv     (501) staff       (20)    33649 2023-06-04 15:58:20.000000 flika-0.3.0/flika/window.py
+-rw-r--r--   0 kylenv     (501) staff       (20)      141 2023-06-03 04:54:52.000000 flika-0.3.0/flika.desktop
+drwxr-xr-x   0 kylenv     (501) staff       (20)        0 2023-06-04 16:11:24.684920 flika-0.3.0/flika.egg-info/
+-rw-r--r--   0 kylenv     (501) staff       (20)     1062 2023-06-04 16:11:24.000000 flika-0.3.0/flika.egg-info/PKG-INFO
+-rw-r--r--   0 kylenv     (501) staff       (20)     1736 2023-06-04 16:11:24.000000 flika-0.3.0/flika.egg-info/SOURCES.txt
+-rw-r--r--   0 kylenv     (501) staff       (20)        1 2023-06-04 16:11:24.000000 flika-0.3.0/flika.egg-info/dependency_links.txt
+-rw-r--r--   0 kylenv     (501) staff       (20)       90 2023-06-04 16:11:24.000000 flika-0.3.0/flika.egg-info/entry_points.txt
+-rw-r--r--   0 kylenv     (501) staff       (20)      238 2023-06-04 16:11:24.000000 flika-0.3.0/flika.egg-info/requires.txt
+-rw-r--r--   0 kylenv     (501) staff       (20)        6 2023-06-04 16:11:24.000000 flika-0.3.0/flika.egg-info/top_level.txt
+-rw-r--r--   0 kylenv     (501) staff       (20)       38 2023-06-04 16:11:24.699008 flika-0.3.0/setup.cfg
+-rw-r--r--   0 kylenv     (501) staff       (20)     2703 2023-06-04 16:04:36.000000 flika-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flika-0.2.9/flika/app/plugin_manager.py` & `flika-0.3.0/flika/app/plugin_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1329 +1,1469 @@
 00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0d 0a66 726f 6d20 676c  f-8 -*-..from gl
-00000020: 6f62 2069 6d70 6f72 7420 676c 6f62 0d0a  ob import glob..
-00000030: 696d 706f 7274 206f 732c 2073 7973 2c20  import os, sys, 
-00000040: 6469 6666 6c69 622c 207a 6970 6669 6c65  difflib, zipfile
-00000050: 2c20 7469 6d65 2c20 7368 7574 696c 2c20  , time, shutil, 
-00000060: 7472 6163 6562 6163 6b0d 0a69 6d70 6f72  traceback..impor
-00000070: 7420 696d 706f 7274 6c69 622e 7574 696c  t importlib.util
-00000080: 0d0a 6672 6f6d 206f 732e 7061 7468 2069  ..from os.path i
-00000090: 6d70 6f72 7420 6578 7061 6e64 7573 6572  mport expanduser
-000000a0: 0d0a 6672 6f6d 2071 7470 7920 696d 706f  ..from qtpy impo
-000000b0: 7274 2051 7447 7569 2c20 5174 5769 6467  rt QtGui, QtWidg
-000000c0: 6574 732c 2051 7443 6f72 650d 0a66 726f  ets, QtCore..fro
-000000d0: 6d20 7572 6c6c 6962 2e72 6571 7565 7374  m urllib.request
-000000e0: 2069 6d70 6f72 7420 7572 6c6f 7065 6e0d   import urlopen.
-000000f0: 0a66 726f 6d20 7572 6c6c 6962 2e65 7272  .from urllib.err
-00000100: 6f72 2069 6d70 6f72 7420 4854 5450 4572  or import HTTPEr
-00000110: 726f 720d 0a66 726f 6d20 7572 6c6c 6962  ror..from urllib
-00000120: 2e70 6172 7365 2069 6d70 6f72 7420 7572  .parse import ur
-00000130: 6c6a 6f69 6e0d 0a66 726f 6d20 706b 675f  ljoin..from pkg_
-00000140: 7265 736f 7572 6365 7320 696d 706f 7274  resources import
-00000150: 2070 6172 7365 5f76 6572 7369 6f6e 0d0a   parse_version..
-00000160: 696d 706f 7274 2070 6b67 5f72 6573 6f75  import pkg_resou
-00000170: 7263 6573 2c20 6f73 0d0a 696d 706f 7274  rces, os..import
-00000180: 2074 6872 6561 6469 6e67 0d0a 696d 706f   threading..impo
-00000190: 7274 2070 6970 2c20 7465 6d70 6669 6c65  rt pip, tempfile
-000001a0: 0d0a 6672 6f6d 2078 6d6c 2e65 7472 6565  ..from xml.etree
-000001b0: 2069 6d70 6f72 7420 456c 656d 656e 7454   import ElementT
-000001c0: 7265 650d 0a69 6d70 6f72 7420 706c 6174  ree..import plat
-000001d0: 666f 726d 0d0a 0d0a 6672 6f6d 202e 2e20  form....from .. 
-000001e0: 696d 706f 7274 2067 6c6f 6261 6c5f 7661  import global_va
-000001f0: 7273 2061 7320 670d 0a66 726f 6d20 2e2e  rs as g..from ..
-00000200: 7574 696c 732e 6d69 7363 2069 6d70 6f72  utils.misc impor
-00000210: 7420 6c6f 6164 5f75 690d 0a66 726f 6d20  t load_ui..from 
-00000220: 2e2e 696d 6167 6573 2069 6d70 6f72 7420  ..images import 
-00000230: 696d 6167 655f 7061 7468 0d0a 0d0a 706c  image_path....pl
-00000240: 7567 696e 5f6c 6973 7420 3d20 7b0d 0a20  ugin_list = {.. 
-00000250: 2020 2027 476c 6f62 616c 2041 6e61 6c79     'Global Analy
-00000260: 7369 7327 3a20 2027 6874 7470 733a 2f2f  sis':  'https://
-00000270: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00000280: 6e74 656e 742e 636f 6d2f 4272 6574 744a  ntent.com/BrettJ
-00000290: 5365 7474 6c65 2f47 6c6f 6261 6c41 6e61  Settle/GlobalAna
-000002a0: 6c79 7369 7350 6c75 6769 6e2f 6d61 7374  lysisPlugin/mast
-000002b0: 6572 2f27 2c0d 0a20 2020 2027 4265 616d  er/',..    'Beam
-000002c0: 2053 706c 6974 7465 7227 3a20 2020 2027   Splitter':    '
-000002d0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-000002e0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-000002f0: 6d2f 4272 6574 744a 5365 7474 6c65 2f42  m/BrettJSettle/B
-00000300: 6561 6d53 706c 6974 7465 722f 6d61 7374  eamSplitter/mast
-00000310: 6572 2f27 2c0d 0a20 2020 2027 526f 6465  er/',..    'Rode
-00000320: 6e74 2054 7261 636b 6572 273a 2020 2027  nt Tracker':   '
-00000330: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00000340: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00000350: 6d2f 6b79 6c65 656c 6c65 6673 656e 2f72  m/kyleellefsen/r
-00000360: 6f64 656e 7454 7261 636b 6572 2f6d 6173  odentTracker/mas
-00000370: 7465 722f 272c 0d0a 2020 2020 2744 6574  ter/',..    'Det
-00000380: 6563 7420 5075 6666 7327 3a20 2020 2020  ect Puffs':     
-00000390: 2768 7474 7073 3a2f 2f72 6177 2e67 6974  'https://raw.git
+00000010: 662d 3820 2d2a 2d0a 6672 6f6d 202e 2e6c  f-8 -*-.from ..l
+00000020: 6f67 6765 7220 696d 706f 7274 206c 6f67  ogger import log
+00000030: 6765 720a 6c6f 6767 6572 2e64 6562 7567  ger.logger.debug
+00000040: 2822 5374 6172 7465 6420 2772 6561 6469  ("Started 'readi
+00000050: 6e67 2061 7070 2f70 6c75 6769 6e5f 6d61  ng app/plugin_ma
+00000060: 6e61 6765 722e 7079 2722 290a 0a66 726f  nager.py'")..fro
+00000070: 6d20 676c 6f62 2069 6d70 6f72 7420 676c  m glob import gl
+00000080: 6f62 0a69 6d70 6f72 7420 6f73 2c20 7379  ob.import os, sy
+00000090: 732c 2064 6966 666c 6962 2c20 7a69 7066  s, difflib, zipf
+000000a0: 696c 652c 2074 696d 652c 2073 6875 7469  ile, time, shuti
+000000b0: 6c2c 2074 7261 6365 6261 636b 2c20 7375  l, traceback, su
+000000c0: 6270 726f 6365 7373 0a66 726f 6d20 6f73  bprocess.from os
+000000d0: 2e70 6174 6820 696d 706f 7274 2065 7870  .path import exp
+000000e0: 616e 6475 7365 720a 6672 6f6d 2071 7470  anduser.from qtp
+000000f0: 7920 696d 706f 7274 2051 7447 7569 2c20  y import QtGui, 
+00000100: 5174 5769 6467 6574 732c 2051 7443 6f72  QtWidgets, QtCor
+00000110: 650a 6672 6f6d 2075 726c 6c69 622e 7265  e.from urllib.re
+00000120: 7175 6573 7420 696d 706f 7274 2075 726c  quest import url
+00000130: 6f70 656e 0a66 726f 6d20 7572 6c6c 6962  open.from urllib
+00000140: 2e65 7272 6f72 2069 6d70 6f72 7420 4854  .error import HT
+00000150: 5450 4572 726f 720a 6672 6f6d 2075 726c  TPError.from url
+00000160: 6c69 622e 7061 7273 6520 696d 706f 7274  lib.parse import
+00000170: 2075 726c 6a6f 696e 0a69 6d70 6f72 7420   urljoin.import 
+00000180: 7468 7265 6164 696e 670a 696d 706f 7274  threading.import
+00000190: 2074 656d 7066 696c 650a 6672 6f6d 2078   tempfile.from x
+000001a0: 6d6c 2e65 7472 6565 2069 6d70 6f72 7420  ml.etree import 
+000001b0: 456c 656d 656e 7454 7265 650a 696d 706f  ElementTree.impo
+000001c0: 7274 2070 6c61 7466 6f72 6d0a 696d 706f  rt platform.impo
+000001d0: 7274 2070 6b67 5f72 6573 6f75 7263 6573  rt pkg_resources
+000001e0: 0a0a 6672 6f6d 202e 2e20 696d 706f 7274  ..from .. import
+000001f0: 2067 6c6f 6261 6c5f 7661 7273 2061 7320   global_vars as 
+00000200: 670a 6672 6f6d 202e 2e75 7469 6c73 2e6d  g.from ..utils.m
+00000210: 6973 6320 696d 706f 7274 206c 6f61 645f  isc import load_
+00000220: 7569 0a66 726f 6d20 2e2e 696d 6167 6573  ui.from ..images
+00000230: 2069 6d70 6f72 7420 696d 6167 655f 7061   import image_pa
+00000240: 7468 0a0a 706c 7567 696e 5f6c 6973 7420  th..plugin_list 
+00000250: 3d20 7b0a 2020 2020 2742 6561 6d20 5370  = {.    'Beam Sp
+00000260: 6c69 7474 6572 273a 2020 2020 2768 7474  litter':    'htt
+00000270: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000280: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f42  sercontent.com/B
+00000290: 7265 7474 4a53 6574 746c 652f 4265 616d  rettJSettle/Beam
+000002a0: 5370 6c69 7474 6572 2f6d 6173 7465 722f  Splitter/master/
+000002b0: 272c 0a20 2020 2027 4465 7465 6374 2050  ',.    'Detect P
+000002c0: 7566 6673 273a 2020 2020 2027 6874 7470  uffs':     'http
+000002d0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+000002e0: 6572 636f 6e74 656e 742e 636f 6d2f 6b79  ercontent.com/ky
+000002f0: 6c65 656c 6c65 6673 656e 2f64 6574 6563  leellefsen/detec
+00000300: 745f 7075 6666 732f 6d61 7374 6572 2f27  t_puffs/master/'
+00000310: 2c0a 2020 2020 2747 6c6f 6261 6c20 416e  ,.    'Global An
+00000320: 616c 7973 6973 273a 2020 2768 7474 7073  alysis':  'https
+00000330: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000340: 7263 6f6e 7465 6e74 2e63 6f6d 2f42 7265  rcontent.com/Bre
+00000350: 7474 4a53 6574 746c 652f 476c 6f62 616c  ttJSettle/Global
+00000360: 416e 616c 7973 6973 506c 7567 696e 2f6d  AnalysisPlugin/m
+00000370: 6173 7465 722f 272c 0a20 2020 2027 5079  aster/',.    'Py
+00000380: 6e73 6967 6874 273a 2020 2020 2020 2020  nsight':        
+00000390: 2027 6874 7470 3a2f 2f72 6177 2e67 6974   'http://raw.git
 000003a0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
 000003b0: 6f6d 2f6b 796c 6565 6c6c 6566 7365 6e2f  om/kyleellefsen/
-000003c0: 6465 7465 6374 5f70 7566 6673 2f6d 6173  detect_puffs/mas
-000003d0: 7465 722f 272c 0d0a 2020 2020 2750 796e  ter/',..    'Pyn
-000003e0: 7369 6768 7427 3a20 2020 2020 2020 2020  sight':         
-000003f0: 2768 7474 703a 2f2f 7261 772e 6769 7468  'http://raw.gith
-00000400: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00000410: 6d2f 6b79 6c65 656c 6c65 6673 656e 2f70  m/kyleellefsen/p
-00000420: 796e 7369 6768 742f 6d61 7374 6572 2f27  ynsight/master/'
-00000430: 0d0a 7d0d 0a0d 0a68 656c 7048 544d 4c20  ..}....helpHTML 
-00000440: 3d20 2727 270d 0a3c 6831 2073 7479 6c65  = '''..<h1 style
-00000450: 3d22 7769 6474 683a 3130 3025 3b20 7465  ="width:100%; te
-00000460: 7874 2d61 6c69 676e 3a63 656e 7465 7222  xt-align:center"
-00000470: 3e57 656c 636f 6d65 2074 6865 2074 6865  >Welcome the the
-00000480: 2066 6c69 6b61 2050 6c75 6769 6e20 4d61   flika Plugin Ma
-00000490: 6e61 6765 723c 2f68 313e 0d0a 3c70 3e55  nager</h1>..<p>U
-000004a0: 7365 2074 6865 2073 6561 7263 6820 6261  se the search ba
-000004b0: 7220 746f 2074 6865 206c 6566 7420 746f  r to the left to
-000004c0: 2066 696e 6420 6120 7370 6563 6966 6963   find a specific
-000004d0: 2070 6c75 6769 6e2c 206f 7220 6272 6f77   plugin, or brow
-000004e0: 7365 2074 6865 206c 6973 7420 6265 6c6f  se the list belo
-000004f0: 7720 6974 2e3c 2f70 3e0d 0a0d 0a3c 6469  w it.</p>....<di
-00000500: 763e 0d0a 2020 2020 3c68 333e 4465 7665  v>..    <h3>Deve
-00000510: 6c6f 7020 6120 6e65 7720 706c 7567 696e  lop a new plugin
-00000520: 3c2f 6833 3e0d 0a20 2020 203c 703e 2049  </h3>..    <p> I
-00000530: 6620 796f 7520 776f 756c 6420 6c69 6b65  f you would like
-00000540: 2074 6f20 6465 7665 6c6f 7020 796f 7572   to develop your
-00000550: 206f 776e 2070 6c75 6769 6e20 666f 7220   own plugin for 
-00000560: 666c 696b 612c 2066 6f6c 6c6f 7720 7468  flika, follow th
-00000570: 6573 6520 7369 6d70 6c65 2073 7465 7073  ese simple steps
-00000580: 3a3c 2f70 3e0d 0a20 2020 203c 756c 206c  :</p>..    <ul l
-00000590: 6973 742d 7374 796c 653d 6e6f 6e65 3e0d  ist-style=none>.
-000005a0: 0a20 2020 2020 2020 203c 6c69 3e31 2e20  .        <li>1. 
-000005b0: 446f 776e 6c6f 6164 203c 6120 6872 6566  Download <a href
-000005c0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-000005d0: 2e63 6f6d 2f66 6c69 6b61 2d6f 7267 2f66  .com/flika-org/f
-000005e0: 6c69 6b61 5f70 6c75 6769 6e5f 7465 6d70  lika_plugin_temp
-000005f0: 6c61 7465 223e 666c 696b 6120 506c 7567  late">flika Plug
-00000600: 696e 2054 656d 706c 6174 653c 2f61 3e20  in Template</a> 
-00000610: 616e 6420 706c 6163 6520 6974 2069 6e20  and place it in 
-00000620: 796f 7572 202e 464c 494b 412f 706c 7567  your .FLIKA/plug
-00000630: 696e 7320 6469 7265 6374 6f72 793c 2f6c  ins directory</l
-00000640: 693e 0d0a 2020 2020 2020 2020 3c6c 693e  i>..        <li>
-00000650: 322e 2055 7064 6174 6520 7468 6520 696e  2. Update the in
-00000660: 666f 2e78 6d6c 2066 696c 6520 666f 7220  fo.xml file for 
-00000670: 796f 7572 2070 6c75 6769 6e3c 2f6c 693e  your plugin</li>
-00000680: 0d0a 2020 2020 2020 2020 3c6c 693e 332e  ..        <li>3.
-00000690: 2052 6566 6572 2074 6f20 7468 6520 3c61   Refer to the <a
-000006a0: 2068 7265 663d 2268 7474 703a 2f2f 666c   href="http://fl
-000006b0: 696b 612d 6f72 672e 6769 7468 7562 2e69  ika-org.github.i
-000006c0: 6f2f 7772 6974 696e 675f 706c 7567 696e  o/writing_plugin
-000006d0: 732e 6874 6d6c 223e 666c 696b 6120 446f  s.html">flika Do
-000006e0: 6375 6d65 6e74 6174 696f 6e3c 2f61 3e20  cumentation</a> 
-000006f0: 666f 7220 6173 7369 7374 616e 6365 2064  for assistance d
-00000700: 6576 656c 6f70 696e 6720 796f 7572 2070  eveloping your p
-00000710: 6c75 6769 6e2e 3c2f 6c69 3e0d 0a20 2020  lugin.</li>..   
-00000720: 2020 2020 203c 6c69 3e34 2e20 5570 6461       <li>4. Upda
-00000730: 7465 2074 6865 2064 6573 6372 6970 7469  te the descripti
-00000740: 6f6e 2e68 746d 6c20 6669 6c65 2066 6f72  on.html file for
-00000750: 2079 6f75 7220 706c 7567 696e 3c2f 6c69   your plugin</li
-00000760: 3e0d 0a20 2020 2020 2020 203c 6c69 3e35  >..        <li>5
-00000770: 2e20 5365 6e64 2079 6f75 7220 706c 7567  . Send your plug
-00000780: 696e 2072 6570 6f20 746f 2075 7320 616e  in repo to us an
-00000790: 6420 7765 276c 6c20 6164 6420 6974 2074  d we'll add it t
-000007a0: 6f20 7468 6520 506c 7567 696e 204d 616e  o the Plugin Man
-000007b0: 6167 6572 213c 2f6c 693e 0d0a 2020 2020  ager!</li>..    
-000007c0: 3c2f 756c 3e0d 0a3c 6469 763e 0d0a 2727  </ul>..<div>..''
-000007d0: 270d 0a0d 0a0d 0a64 6566 2067 6574 5f70  '......def get_p
-000007e0: 6c75 6769 6e5f 6469 7265 6374 6f72 7928  lugin_directory(
-000007f0: 293a 0d0a 2020 2020 6c6f 6361 6c5f 666c  ):..    local_fl
-00000800: 696b 615f 6469 7265 6374 6f72 7920 3d20  ika_directory = 
-00000810: 6f73 2e70 6174 682e 6a6f 696e 2865 7870  os.path.join(exp
-00000820: 616e 6475 7365 7228 227e 2229 2c20 272e  anduser("~"), '.
-00000830: 464c 494b 4127 290d 0a20 2020 2070 6c75  FLIKA')..    plu
-00000840: 6769 6e5f 6469 7265 6374 6f72 7920 3d20  gin_directory = 
-00000850: 6f73 2e70 6174 682e 6a6f 696e 2865 7870  os.path.join(exp
-00000860: 616e 6475 7365 7228 227e 2229 2c20 272e  anduser("~"), '.
-00000870: 464c 494b 4127 2c20 2770 6c75 6769 6e73  FLIKA', 'plugins
-00000880: 2720 290d 0a20 2020 2069 6620 6e6f 7420  ' )..    if not 
-00000890: 6f73 2e70 6174 682e 6578 6973 7473 2870  os.path.exists(p
-000008a0: 6c75 6769 6e5f 6469 7265 6374 6f72 7929  lugin_directory)
-000008b0: 3a0d 0a20 2020 2020 2020 206f 732e 6d61  :..        os.ma
-000008c0: 6b65 6469 7273 2870 6c75 6769 6e5f 6469  kedirs(plugin_di
-000008d0: 7265 6374 6f72 7929 0d0a 2020 2020 6966  rectory)..    if
-000008e0: 206e 6f74 206f 732e 7061 7468 2e69 7366   not os.path.isf
-000008f0: 696c 6528 6f73 2e70 6174 682e 6a6f 696e  ile(os.path.join
-00000900: 2870 6c75 6769 6e5f 6469 7265 6374 6f72  (plugin_director
-00000910: 792c 2027 5f5f 696e 6974 5f5f 2e70 7927  y, '__init__.py'
-00000920: 2929 3a0d 0a20 2020 2020 2020 206f 7065  )):..        ope
-00000930: 6e28 6f73 2e70 6174 682e 6a6f 696e 2870  n(os.path.join(p
-00000940: 6c75 6769 6e5f 6469 7265 6374 6f72 792c  lugin_directory,
-00000950: 2027 5f5f 696e 6974 5f5f 2e70 7927 292c   '__init__.py'),
-00000960: 2027 6127 292e 636c 6f73 6528 2920 2023   'a').close()  #
-00000970: 2043 7265 6174 6520 656d 7074 7920 5f5f   Create empty __
-00000980: 696e 6974 5f5f 2e70 7920 6669 6c65 0d0a  init__.py file..
-00000990: 2020 2020 6966 2070 6c75 6769 6e5f 6469      if plugin_di
-000009a0: 7265 6374 6f72 7920 6e6f 7420 696e 2073  rectory not in s
-000009b0: 7973 2e70 6174 683a 0d0a 2020 2020 2020  ys.path:..      
-000009c0: 2020 7379 732e 7061 7468 2e61 7070 656e    sys.path.appen
-000009d0: 6428 706c 7567 696e 5f64 6972 6563 746f  d(plugin_directo
-000009e0: 7279 290d 0a20 2020 2069 6620 6c6f 6361  ry)..    if loca
-000009f0: 6c5f 666c 696b 615f 6469 7265 6374 6f72  l_flika_director
-00000a00: 7920 6e6f 7420 696e 2073 7973 2e70 6174  y not in sys.pat
-00000a10: 683a 0d0a 2020 2020 2020 2020 7379 732e  h:..        sys.
-00000a20: 7061 7468 2e61 7070 656e 6428 6c6f 6361  path.append(loca
-00000a30: 6c5f 666c 696b 615f 6469 7265 6374 6f72  l_flika_director
-00000a40: 7929 0d0a 2020 2020 7265 7475 726e 2070  y)..    return p
-00000a50: 6c75 6769 6e5f 6469 7265 6374 6f72 790d  lugin_directory.
-00000a60: 0a0d 0a0d 0a64 6566 2070 6172 7365 2878  .....def parse(x
-00000a70: 293a 0d0a 2020 2020 7472 6565 203d 2045  ):..    tree = E
-00000a80: 6c65 6d65 6e74 5472 6565 2e66 726f 6d73  lementTree.froms
-00000a90: 7472 696e 6728 7829 0d0a 2020 2020 6465  tring(x)..    de
-00000aa0: 6620 7374 6570 2869 7465 6d29 3a0d 0a20  f step(item):.. 
-00000ab0: 2020 2020 2020 2064 203d 207b 7d0d 0a20         d = {}.. 
-00000ac0: 2020 2020 2020 2069 6620 6974 656d 2e74         if item.t
-00000ad0: 6578 7420 616e 6420 6974 656d 2e74 6578  ext and item.tex
-00000ae0: 742e 7374 7269 7028 293a 0d0a 2020 2020  t.strip():..    
-00000af0: 2020 2020 2020 2020 645b 2723 7465 7874          d['#text
-00000b00: 275d 203d 2069 7465 6d2e 7465 7874 2e73  '] = item.text.s
-00000b10: 7472 6970 2829 0d0a 2020 2020 2020 2020  trip()..        
-00000b20: 666f 7220 6b2c 2076 2069 6e20 6974 656d  for k, v in item
-00000b30: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
-00000b40: 2020 2020 2020 2064 5b27 4025 7327 2025         d['@%s' %
-00000b50: 206b 5d20 3d20 760d 0a20 2020 2020 2020   k] = v..       
-00000b60: 2066 6f72 206b 2069 6e20 6974 656d 2e67   for k in item.g
-00000b70: 6574 6368 696c 6472 656e 2829 3a0d 0a20  etchildren():.. 
-00000b80: 2020 2020 2020 2020 2020 2069 6620 6b2e             if k.
-00000b90: 7461 6720 6e6f 7420 696e 2064 3a0d 0a20  tag not in d:.. 
-00000ba0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00000bb0: 5b6b 2e74 6167 5d20 3d20 7374 6570 286b  [k.tag] = step(k
-00000bc0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00000bd0: 6c69 6620 7479 7065 2864 5b6b 2e74 6167  lif type(d[k.tag
-00000be0: 5d29 203d 3d20 6c69 7374 3a0d 0a20 2020  ]) == list:..   
-00000bf0: 2020 2020 2020 2020 2020 2020 2064 5b6b               d[k
-00000c00: 2e74 6167 5d2e 6170 7065 6e64 2873 7465  .tag].append(ste
-00000c10: 7028 6b29 290d 0a20 2020 2020 2020 2020  p(k))..         
-00000c20: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000c30: 2020 2020 2020 2020 2020 645b 6b2e 7461            d[k.ta
-00000c40: 675d 203d 205b 645b 6b2e 7461 675d 2c20  g] = [d[k.tag], 
-00000c50: 7374 6570 286b 295d 0d0a 2020 2020 2020  step(k)]..      
-00000c60: 2020 6966 206c 656e 2864 2920 3d3d 2031    if len(d) == 1
-00000c70: 2061 6e64 2027 2374 6578 7427 2069 6e20   and '#text' in 
-00000c80: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
-00000c90: 7265 7475 726e 2064 5b27 2374 6578 7427  return d['#text'
-00000ca0: 5d0d 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
-00000cb0: 6e20 640d 0a20 2020 2072 6574 7572 6e20  n d..    return 
-00000cc0: 7374 6570 2874 7265 6529 0d0a 0d0a 636c  step(tree)....cl
-00000cd0: 6173 7320 506c 7567 696e 496d 706f 7274  ass PluginImport
-00000ce0: 4572 726f 7228 4578 6365 7074 696f 6e29  Error(Exception)
-00000cf0: 3a0d 0a20 2020 2070 6173 730d 0a0d 0a64  :..    pass....d
-00000d00: 6566 2073 7472 3266 756e 6328 706c 7567  ef str2func(plug
-00000d10: 696e 5f6e 616d 652c 2066 696c 655f 6c6f  in_name, file_lo
-00000d20: 6361 7469 6f6e 2c20 6675 6e63 7469 6f6e  cation, function
-00000d30: 293a 0d0a 2020 2020 2727 270d 0a20 2020  ):..    '''..   
-00000d40: 2074 616b 6573 2070 6c75 6769 6e5f 6e61   takes plugin_na
-00000d50: 6d65 2c20 7061 7468 2074 6f20 6f62 6a65  me, path to obje
-00000d60: 6374 2c20 6675 6e63 7469 6f6e 2061 7320  ct, function as 
-00000d70: 6172 6775 6d65 6e74 730d 0a20 2020 2069  arguments..    i
-00000d80: 6d70 6f72 7473 2070 6c75 6769 6e5f 6e61  mports plugin_na
-00000d90: 6d65 2e70 6174 6820 616e 6420 6765 7473  me.path and gets
-00000da0: 2074 6865 2066 756e 6374 696f 6e20 6672   the function fr
-00000db0: 6f6d 2074 6861 7420 696d 706f 7274 6564  om that imported
-00000dc0: 206f 626a 6563 740d 0a20 2020 2074 6f20   object..    to 
-00000dd0: 6265 2072 756e 2077 6865 6e20 616e 2061  be run when an a
-00000de0: 6374 696f 6e20 6973 2063 6c69 636b 6564  ction is clicked
-00000df0: 0d0a 2020 2020 2727 270d 0a20 2020 205f  ..    '''..    _
-00000e00: 5f69 6d70 6f72 745f 5f28 706c 7567 696e  _import__(plugin
-00000e10: 5f6e 616d 6529 0d0a 0d0a 2020 2020 706c  _name)....    pl
-00000e20: 7567 696e 5f64 6972 203d 2022 706c 7567  ugin_dir = "plug
-00000e30: 696e 732e 7b7d 2e7b 7d22 2e66 6f72 6d61  ins.{}.{}".forma
-00000e40: 7428 706c 7567 696e 5f6e 616d 652c 2066  t(plugin_name, f
-00000e50: 696c 655f 6c6f 6361 7469 6f6e 290d 0a20  ile_location).. 
-00000e60: 2020 206c 6576 656c 7320 3d20 6675 6e63     levels = func
-00000e70: 7469 6f6e 2e73 706c 6974 2827 2e27 290d  tion.split('.').
-00000e80: 0a20 2020 2074 7279 3a0d 0a20 2020 2020  .    try:..     
-00000e90: 2020 206d 6f64 756c 6520 3d20 5f5f 696d     module = __im
-00000ea0: 706f 7274 5f5f 2870 6c75 6769 6e5f 6469  port__(plugin_di
-00000eb0: 722c 2066 726f 6d6c 6973 743d 5b6c 6576  r, fromlist=[lev
-00000ec0: 656c 735b 305d 5d29 2e5f 5f64 6963 745f  els[0]]).__dict_
-00000ed0: 5f5b 6c65 7665 6c73 5b30 5d5d 0d0a 2020  _[levels[0]]..  
-00000ee0: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
-00000ef0: 2020 2072 6169 7365 2050 6c75 6769 6e49     raise PluginI
-00000f00: 6d70 6f72 7445 7272 6f72 2822 4661 696c  mportError("Fail
-00000f10: 6564 2074 6f20 696d 706f 7274 2025 7320  ed to import %s 
-00000f20: 6672 6f6d 206d 6f64 756c 6520 2573 2e5c  from module %s.\
-00000f30: 6e25 7322 2025 2028 6c65 7665 6c73 5b30  n%s" % (levels[0
-00000f40: 5d2c 2070 6c75 6769 6e5f 6469 722c 2074  ], plugin_dir, t
-00000f50: 7261 6365 6261 636b 2e66 6f72 6d61 745f  raceback.format_
-00000f60: 6578 6328 2929 290d 0a20 2020 2020 2020  exc()))..       
-00000f70: 2072 6574 7572 6e20 4e6f 6e65 0d0a 2020   return None..  
-00000f80: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00000f90: 2831 2c20 6c65 6e28 6c65 7665 6c73 2929  (1, len(levels))
-00000fa0: 3a0d 0a20 2020 2020 2020 2074 7279 3a0d  :..        try:.
-00000fb0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-00000fc0: 756c 6520 3d20 6765 7461 7474 7228 6d6f  ule = getattr(mo
-00000fd0: 6475 6c65 2c20 6c65 7665 6c73 5b69 5d29  dule, levels[i])
-00000fe0: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-00000ff0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00001000: 6169 7365 2050 6c75 6769 6e49 6d70 6f72  aise PluginImpor
-00001010: 7445 7272 6f72 2822 4661 696c 6564 2074  tError("Failed t
-00001020: 6f20 696d 706f 7274 2025 7320 6672 6f6d  o import %s from
-00001030: 206d 6f64 756c 6520 2573 2e20 4368 6563   module %s. Chec
-00001040: 6b20 6e61 6d65 2061 6e64 2074 7279 2061  k name and try a
-00001050: 6761 696e 2e22 2025 2028 6c65 7665 6c73  gain." % (levels
-00001060: 5b69 5d2c 206d 6f64 756c 6529 2920 2320  [i], module)) # 
-00001070: 6f6e 6c79 2061 6c65 7274 7320 6f6e 2070  only alerts on p
-00001080: 7974 686f 6e20 333f 0d0a 2020 2020 2020  ython 3?..      
-00001090: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-000010a0: 650d 0a20 2020 2072 6574 7572 6e20 6d6f  e..    return mo
-000010b0: 6475 6c65 0d0a 0d0a 6465 6620 6275 696c  dule....def buil
-000010c0: 645f 7375 626d 656e 7528 6d6f 6475 6c65  d_submenu(module
-000010d0: 5f6e 616d 652c 2070 6172 656e 745f 6d65  _name, parent_me
-000010e0: 6e75 2c20 6c61 796f 7574 5f64 6963 7429  nu, layout_dict)
-000010f0: 3a0d 0a20 2020 2066 6f72 206b 6579 2c20  :..    for key, 
-00001100: 7661 6c75 6520 696e 206c 6179 6f75 745f  value in layout_
-00001110: 6469 6374 2e69 7465 6d73 2829 3a0d 0a20  dict.items():.. 
-00001120: 2020 2020 2020 2069 6620 7479 7065 2876         if type(v
-00001130: 616c 7565 2920 213d 206c 6973 743a 0d0a  alue) != list:..
-00001140: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-00001150: 6520 3d20 5b76 616c 7565 5d0d 0a20 2020  e = [value]..   
-00001160: 2020 2020 2069 6620 6b65 7920 3d3d 2027       if key == '
-00001170: 6d65 6e75 273a 0d0a 2020 2020 2020 2020  menu':..        
-00001180: 2020 2020 666f 7220 7620 696e 2076 616c      for v in val
-00001190: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
-000011a0: 2020 2020 206d 656e 7520 3d20 7061 7265       menu = pare
-000011b0: 6e74 5f6d 656e 752e 6164 644d 656e 7528  nt_menu.addMenu(
-000011c0: 765b 2240 6e61 6d65 225d 290d 0a20 2020  v["@name"])..   
-000011d0: 2020 2020 2020 2020 2020 2020 2062 7569               bui
-000011e0: 6c64 5f73 7562 6d65 6e75 286d 6f64 756c  ld_submenu(modul
-000011f0: 655f 6e61 6d65 2c20 6d65 6e75 2c20 7629  e_name, menu, v)
-00001200: 0d0a 2020 2020 2020 2020 656c 6966 206b  ..        elif k
-00001210: 6579 203d 3d20 2761 6374 696f 6e27 3a0d  ey == 'action':.
-00001220: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00001230: 206f 6420 696e 2076 616c 7565 3a0d 0a20   od in value:.. 
-00001240: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00001250: 6574 686f 6420 3d20 7374 7232 6675 6e63  ethod = str2func
-00001260: 286d 6f64 756c 655f 6e61 6d65 2c20 6f64  (module_name, od
-00001270: 5b27 406c 6f63 6174 696f 6e27 5d2c 206f  ['@location'], o
-00001280: 645b 2740 6675 6e63 7469 6f6e 275d 290d  d['@function']).
-00001290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000012a0: 2069 6620 6d65 7468 6f64 2069 7320 6e6f   if method is no
-000012b0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-000012c0: 2020 2020 2020 2020 2020 2020 2061 6374               act
-000012d0: 696f 6e20 3d20 5174 5769 6467 6574 732e  ion = QtWidgets.
-000012e0: 5141 6374 696f 6e28 6f64 5b27 2374 6578  QAction(od['#tex
-000012f0: 7427 5d2c 2070 6172 656e 745f 6d65 6e75  t'], parent_menu
-00001300: 2c20 7472 6967 6765 7265 6420 3d20 6d65  , triggered = me
-00001310: 7468 6f64 290d 0a20 2020 2020 2020 2020  thod)..         
-00001320: 2020 2020 2020 2020 2020 2070 6172 656e             paren
-00001330: 745f 6d65 6e75 2e61 6464 4163 7469 6f6e  t_menu.addAction
-00001340: 2861 6374 696f 6e29 0d0a 0d0a 0d0a 636c  (action)......cl
-00001350: 6173 7320 506c 7567 696e 2829 3a0d 0a20  ass Plugin():.. 
-00001360: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00001370: 7365 6c66 2c20 6e61 6d65 2c20 696e 666f  self, name, info
-00001380: 5f75 726c 3d4e 6f6e 6529 3a0d 0a20 2020  _url=None):..   
-00001390: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
-000013a0: 206e 616d 650d 0a20 2020 2020 2020 2073   name..        s
-000013b0: 656c 662e 6469 7265 6374 6f72 7920 3d20  elf.directory = 
-000013c0: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
-000013d0: 6c66 2e75 726c 203d 204e 6f6e 650d 0a20  lf.url = None.. 
-000013e0: 2020 2020 2020 2073 656c 662e 6175 7468         self.auth
-000013f0: 6f72 203d 204e 6f6e 650d 0a20 2020 2020  or = None..     
-00001400: 2020 2073 656c 662e 646f 6375 6d65 6e74     self.document
-00001410: 6174 696f 6e20 3d20 4e6f 6e65 0d0a 2020  ation = None..  
-00001420: 2020 2020 2020 7365 6c66 2e76 6572 7369        self.versi
-00001430: 6f6e 203d 2027 270d 0a20 2020 2020 2020  on = ''..       
-00001440: 2073 656c 662e 6c61 7465 7374 5f76 6572   self.latest_ver
-00001450: 7369 6f6e 203d 2027 270d 0a20 2020 2020  sion = ''..     
-00001460: 2020 2073 656c 662e 6d65 6e75 203d 204e     self.menu = N
-00001470: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
-00001480: 662e 6c69 7374 5769 6467 6574 203d 2051  f.listWidget = Q
-00001490: 7457 6964 6765 7473 2e51 4c69 7374 5769  tWidgets.QListWi
-000014a0: 6467 6574 4974 656d 2873 656c 662e 6e61  dgetItem(self.na
-000014b0: 6d65 290d 0a20 2020 2020 2020 2073 656c  me)..        sel
-000014c0: 662e 696e 7374 616c 6c65 6420 3d20 4661  f.installed = Fa
-000014d0: 6c73 650d 0a20 2020 2020 2020 2073 656c  lse..        sel
-000014e0: 662e 6465 7363 7269 7074 696f 6e20 3d20  f.description = 
-000014f0: 2727 0d0a 2020 2020 2020 2020 7365 6c66  ''..        self
-00001500: 2e64 6570 656e 6465 6e63 6965 7320 3d20  .dependencies = 
-00001510: 5b5d 0d0a 2020 2020 2020 2020 7365 6c66  []..        self
-00001520: 2e6c 6f61 6465 6420 3d20 4661 6c73 650d  .loaded = False.
-00001530: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00001540: 666f 5f75 726c 203d 2069 6e66 6f5f 7572  fo_url = info_ur
-00001550: 6c0d 0a20 2020 2020 2020 2069 6620 696e  l..        if in
-00001560: 666f 5f75 726c 3a0d 0a20 2020 2020 2020  fo_url:..       
-00001570: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
-00001580: 5f69 6e66 6f28 290d 0a0d 0a20 2020 2064  _info()....    d
-00001590: 6566 2072 656c 6f61 6428 7365 6c66 293a  ef reload(self):
-000015a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-000015b0: 656e 7520 3d20 5174 5769 6467 6574 732e  enu = QtWidgets.
-000015c0: 514d 656e 7528 7365 6c66 2e6e 616d 6529  QMenu(self.name)
-000015d0: 0d0a 2020 2020 2020 2020 6275 696c 645f  ..        build_
-000015e0: 7375 626d 656e 7528 7365 6c66 2e64 6972  submenu(self.dir
-000015f0: 6563 746f 7279 2c20 7365 6c66 2e6d 656e  ectory, self.men
-00001600: 752c 2073 656c 662e 6d65 6e75 5f6c 6179  u, self.menu_lay
-00001610: 6f75 7429 0d0a 0d0a 2020 2020 6465 6620  out)....    def 
-00001620: 6c61 7374 4d6f 6469 6669 6564 2873 656c  lastModified(sel
-00001630: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00001640: 7572 6e20 6f73 2e70 6174 682e 6765 746d  urn os.path.getm
-00001650: 7469 6d65 286f 732e 7061 7468 2e6a 6f69  time(os.path.joi
-00001660: 6e28 6765 745f 706c 7567 696e 5f64 6972  n(get_plugin_dir
-00001670: 6563 746f 7279 2829 2c20 7365 6c66 2e64  ectory(), self.d
-00001680: 6972 6563 746f 7279 2929 0d0a 0d0a 2020  irectory))....  
-00001690: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
-000016a0: 0a20 2020 2064 6566 2066 726f 6d4c 6f63  .    def fromLoc
-000016b0: 616c 2870 6174 6829 3a0d 0a20 2020 2020  al(path):..     
-000016c0: 2020 2074 6578 7420 3d20 6f70 656e 286f     text = open(o
-000016d0: 732e 7061 7468 2e6a 6f69 6e28 7061 7468  s.path.join(path
-000016e0: 2c20 2769 6e66 6f2e 786d 6c27 292c 2027  , 'info.xml'), '
-000016f0: 7227 292e 7265 6164 2829 0d0a 2020 2020  r').read()..    
-00001700: 2020 2020 696e 666f 203d 2070 6172 7365      info = parse
-00001710: 2874 6578 7429 0d0a 2020 2020 2020 2020  (text)..        
-00001720: 7020 3d20 506c 7567 696e 2869 6e66 6f5b  p = Plugin(info[
-00001730: 2740 6e61 6d65 275d 290d 0a20 2020 2020  '@name'])..     
-00001740: 2020 2070 2e64 6972 6563 746f 7279 203d     p.directory =
-00001750: 2069 6e66 6f5b 2764 6972 6563 746f 7279   info['directory
-00001760: 275d 0d0a 2020 2020 2020 2020 702e 7665  ']..        p.ve
-00001770: 7273 696f 6e20 3d20 696e 666f 5b27 7665  rsion = info['ve
-00001780: 7273 696f 6e27 5d0d 0a20 2020 2020 2020  rsion']..       
-00001790: 2070 2e6c 6174 6573 745f 7665 7273 696f   p.latest_versio
-000017a0: 6e20 3d20 702e 7665 7273 696f 6e0d 0a20  n = p.version.. 
-000017b0: 2020 2020 2020 2070 2e61 7574 686f 7220         p.author 
-000017c0: 3d20 696e 666f 5b27 6175 7468 6f72 275d  = info['author']
-000017d0: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-000017e0: 2020 2020 2020 2020 2020 2020 702e 6465              p.de
-000017f0: 7363 7269 7074 696f 6e20 3d20 7374 7228  scription = str(
-00001800: 6f70 656e 286f 732e 7061 7468 2e6a 6f69  open(os.path.joi
-00001810: 6e28 7061 7468 2c20 2761 626f 7574 2e68  n(path, 'about.h
-00001820: 746d 6c27 292c 2027 7227 292e 7265 6164  tml'), 'r').read
-00001830: 2829 290d 0a20 2020 2020 2020 2065 7863  ())..        exc
-00001840: 6570 7420 4669 6c65 4e6f 7446 6f75 6e64  ept FileNotFound
-00001850: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
-00001860: 2020 2020 702e 6465 7363 7269 7074 696f      p.descriptio
-00001870: 6e20 3d20 224e 6f20 6c6f 6361 6c20 6465  n = "No local de
-00001880: 7363 7269 7074 696f 6e20 6669 6c65 2066  scription file f
-00001890: 6f75 6e64 220d 0a0d 0a20 2020 2020 2020  ound"....       
-000018a0: 2070 2e75 726c 203d 2069 6e66 6f5b 2775   p.url = info['u
-000018b0: 726c 275d 2069 6620 2775 726c 2720 696e  rl'] if 'url' in
-000018c0: 2069 6e66 6f20 656c 7365 204e 6f6e 650d   info else None.
-000018d0: 0a20 2020 2020 2020 2070 2e64 6f63 756d  .        p.docum
-000018e0: 656e 7461 7469 6f6e 203d 2069 6e66 6f5b  entation = info[
-000018f0: 2764 6f63 756d 656e 7461 7469 6f6e 275d  'documentation']
-00001900: 2069 6620 2764 6f63 756d 656e 7461 7469   if 'documentati
-00001910: 6f6e 2720 696e 2069 6e66 6f20 656c 7365  on' in info else
-00001920: 204e 6f6e 650d 0a0d 0a20 2020 2020 2020   None....       
-00001930: 2069 6620 2764 6570 656e 6465 6e63 6965   if 'dependencie
-00001940: 7327 2069 6e20 696e 666f 2061 6e64 2027  s' in info and '
-00001950: 6465 7065 6e64 656e 6379 2720 696e 2069  dependency' in i
-00001960: 6e66 6f5b 2764 6570 656e 6465 6e63 6965  nfo['dependencie
-00001970: 7327 5d3a 0d0a 2020 2020 2020 2020 2020  s']:..          
-00001980: 2020 6465 7073 203d 2069 6e66 6f5b 2764    deps = info['d
-00001990: 6570 656e 6465 6e63 6965 7327 5d5b 2764  ependencies']['d
-000019a0: 6570 656e 6465 6e63 7927 5d0d 0a20 2020  ependency']..   
-000019b0: 2020 2020 2020 2020 2070 2e64 6570 656e           p.depen
-000019c0: 6465 6e63 6965 7320 3d20 5b64 5b27 406e  dencies = [d['@n
-000019d0: 616d 6527 5d20 666f 7220 6420 696e 2064  ame'] for d in d
-000019e0: 6570 735d 2069 6620 6973 696e 7374 616e  eps] if isinstan
-000019f0: 6365 2864 6570 732c 206c 6973 7429 2065  ce(deps, list) e
-00001a00: 6c73 6520 5b64 6570 735b 2740 6e61 6d65  lse [deps['@name
-00001a10: 275d 5d0d 0a0d 0a20 2020 2020 2020 2070  ']]....        p
-00001a20: 2e6d 656e 755f 6c61 796f 7574 203d 2069  .menu_layout = i
-00001a30: 6e66 6f2e 706f 7028 276d 656e 755f 6c61  nfo.pop('menu_la
-00001a40: 796f 7574 2729 0d0a 2020 2020 2020 2020  yout')..        
-00001a50: 702e 6d65 6e75 203d 2051 7457 6964 6765  p.menu = QtWidge
-00001a60: 7473 2e51 4d65 6e75 2870 2e6e 616d 6529  ts.QMenu(p.name)
-00001a70: 0d0a 2020 2020 2020 2020 6275 696c 645f  ..        build_
-00001a80: 7375 626d 656e 7528 702e 6469 7265 6374  submenu(p.direct
-00001a90: 6f72 792c 2070 2e6d 656e 752c 2070 2e6d  ory, p.menu, p.m
-00001aa0: 656e 755f 6c61 796f 7574 290d 0a20 2020  enu_layout)..   
-00001ab0: 2020 2020 200d 0a20 2020 2020 2020 2070       ..        p
-00001ac0: 2e6c 6973 7457 6964 6765 7420 3d20 5174  .listWidget = Qt
-00001ad0: 5769 6467 6574 732e 514c 6973 7457 6964  Widgets.QListWid
-00001ae0: 6765 7449 7465 6d28 702e 6e61 6d65 290d  getItem(p.name).
-00001af0: 0a20 2020 2020 2020 2070 2e6c 6973 7457  .        p.listW
-00001b00: 6964 6765 742e 7365 7449 636f 6e28 5174  idget.setIcon(Qt
-00001b10: 4775 692e 5149 636f 6e28 696d 6167 655f  Gui.QIcon(image_
-00001b20: 7061 7468 2827 6368 6563 6b2e 706e 6727  path('check.png'
-00001b30: 2929 290d 0a0d 0a20 2020 2020 2020 2070  )))....        p
-00001b40: 2e6c 6f61 6465 6420 3d20 5472 7565 0d0a  .loaded = True..
-00001b50: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00001b60: 0d0a 0d0a 2020 2020 6465 6620 7570 6461  ....    def upda
-00001b70: 7465 5f69 6e66 6f28 7365 6c66 293a 0d0a  te_info(self):..
-00001b80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00001b90: 696e 666f 5f75 726c 2069 7320 4e6f 6e65  info_url is None
-00001ba0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00001bb0: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
-00001bc0: 2020 2020 2069 6e66 6f5f 7572 6c20 3d20       info_url = 
-00001bd0: 7572 6c6a 6f69 6e28 7365 6c66 2e69 6e66  urljoin(self.inf
-00001be0: 6f5f 7572 6c2c 2027 696e 666f 2e78 6d6c  o_url, 'info.xml
-00001bf0: 2729 0d0a 2020 2020 2020 2020 7472 793a  ')..        try:
-00001c00: 0d0a 2020 2020 2020 2020 2020 2020 7478  ..            tx
-00001c10: 7420 3d20 7572 6c6f 7065 6e28 696e 666f  t = urlopen(info
-00001c20: 5f75 726c 292e 7265 6164 2829 0d0a 2020  _url).read()..  
-00001c30: 2020 2020 2020 6578 6365 7074 2048 5454        except HTT
-00001c40: 5045 7272 6f72 2061 7320 653a 0d0a 2020  PError as e:..  
-00001c50: 2020 2020 2020 2020 2020 672e 616c 6572            g.aler
-00001c60: 7428 2246 6169 6c65 6420 746f 2075 7064  t("Failed to upd
-00001c70: 6174 6520 696e 666f 726d 6174 696f 6e20  ate information 
-00001c80: 666f 7220 7b7d 2e5c 6e5c 747b 7d22 2e66  for {}.\n\t{}".f
-00001c90: 6f72 6d61 7428 7365 6c66 2e6e 616d 652c  ormat(self.name,
-00001ca0: 2065 2929 0d0a 2020 2020 2020 2020 2020   e))..          
-00001cb0: 2020 7265 7475 726e 0d0a 0d0a 2020 2020    return....    
-00001cc0: 2020 2020 6e65 775f 696e 666f 203d 2070      new_info = p
-00001cd0: 6172 7365 2874 7874 290d 0a20 2020 2020  arse(txt)..     
-00001ce0: 2020 2064 6573 6372 6970 7469 6f6e 5f75     description_u
-00001cf0: 726c 203d 2075 726c 6a6f 696e 2873 656c  rl = urljoin(sel
-00001d00: 662e 696e 666f 5f75 726c 2c20 2761 626f  f.info_url, 'abo
-00001d10: 7574 2e68 746d 6c27 290d 0a20 2020 2020  ut.html')..     
-00001d20: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00001d30: 2020 2020 206e 6577 5f69 6e66 6f5b 2764       new_info['d
-00001d40: 6573 6372 6970 7469 6f6e 275d 203d 2075  escription'] = u
-00001d50: 726c 6f70 656e 2864 6573 6372 6970 7469  rlopen(descripti
-00001d60: 6f6e 5f75 726c 292e 7265 6164 2829 2e64  on_url).read().d
-00001d70: 6563 6f64 6528 2775 7466 2d38 2729 0d0a  ecode('utf-8')..
-00001d80: 2020 2020 2020 2020 6578 6365 7074 2048          except H
-00001d90: 5454 5045 7272 6f72 3a0d 0a20 2020 2020  TTPError:..     
-00001da0: 2020 2020 2020 206e 6577 5f69 6e66 6f5b         new_info[
-00001db0: 2764 6573 6372 6970 7469 6f6e 275d 203d  'description'] =
-00001dc0: 2022 556e 6162 6c65 2074 6f20 6765 7420   "Unable to get 
-00001dd0: 6465 7363 7269 7074 696f 6e20 666f 7220  description for 
-00001de0: 7b30 7d20 6672 6f6d 203c 6120 6872 6566  {0} from <a href
-00001df0: 3d7b 317d 3e7b 317d 3c2f 613e 222e 666f  ={1}>{1}</a>".fo
-00001e00: 726d 6174 2873 656c 662e 6e61 6d65 2c20  rmat(self.name, 
-00001e10: 6465 7363 7269 7074 696f 6e5f 7572 6c29  description_url)
-00001e20: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-00001e30: 656e 755f 6c61 796f 7574 203d 206e 6577  enu_layout = new
-00001e40: 5f69 6e66 6f2e 706f 7028 276d 656e 755f  _info.pop('menu_
-00001e50: 6c61 796f 7574 2729 0d0a 2020 2020 2020  layout')..      
-00001e60: 2020 6966 2027 6461 7465 2720 696e 206e    if 'date' in n
-00001e70: 6577 5f69 6e66 6f3a 0d0a 2020 2020 2020  ew_info:..      
-00001e80: 2020 2020 2020 6e65 775f 696e 666f 5b27        new_info['
-00001e90: 7665 7273 696f 6e27 5d20 3d20 272e 272e  version'] = '.'.
-00001ea0: 6a6f 696e 286e 6577 5f69 6e66 6f5b 2764  join(new_info['d
-00001eb0: 6174 6527 5d2e 7370 6c69 7428 272f 2729  ate'].split('/')
-00001ec0: 5b32 3a5d 202b 206e 6577 5f69 6e66 6f5b  [2:] + new_info[
-00001ed0: 2764 6174 6527 5d2e 7370 6c69 7428 272f  'date'].split('/
-00001ee0: 2729 5b3a 325d 290d 0a20 2020 2020 2020  ')[:2])..       
-00001ef0: 2020 2020 206e 6577 5f69 6e66 6f2e 706f       new_info.po
-00001f00: 7028 2764 6174 6527 290d 0a20 2020 2020  p('date')..     
-00001f10: 2020 206e 6577 5f69 6e66 6f5b 276c 6174     new_info['lat
-00001f20: 6573 745f 7665 7273 696f 6e27 5d20 3d20  est_version'] = 
-00001f30: 6e65 775f 696e 666f 2e70 6f70 2827 7665  new_info.pop('ve
-00001f40: 7273 696f 6e27 290d 0a20 2020 2020 2020  rsion')..       
-00001f50: 2069 6620 2764 6570 656e 6465 6e63 6965   if 'dependencie
-00001f60: 7327 2069 6e20 6e65 775f 696e 666f 2061  s' in new_info a
-00001f70: 6e64 2027 6465 7065 6e64 656e 6379 2720  nd 'dependency' 
-00001f80: 696e 206e 6577 5f69 6e66 6f5b 2764 6570  in new_info['dep
-00001f90: 656e 6465 6e63 6965 7327 5d3a 0d0a 2020  endencies']:..  
-00001fa0: 2020 2020 2020 2020 2020 6465 7073 203d            deps =
-00001fb0: 206e 6577 5f69 6e66 6f2e 706f 7028 2764   new_info.pop('d
-00001fc0: 6570 656e 6465 6e63 6965 7327 295b 2764  ependencies')['d
-00001fd0: 6570 656e 6465 6e63 7927 5d0d 0a20 2020  ependency']..   
-00001fe0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00001ff0: 7065 6e64 656e 6369 6573 203d 205b 645b  pendencies = [d[
-00002000: 2740 6e61 6d65 275d 2066 6f72 2064 2069  '@name'] for d i
-00002010: 6e20 6465 7073 5d20 6966 2069 7369 6e73  n deps] if isins
-00002020: 7461 6e63 6528 6465 7073 2c20 6c69 7374  tance(deps, list
-00002030: 2920 656c 7365 205b 6465 7073 5b27 406e  ) else [deps['@n
-00002040: 616d 6527 5d5d 0d0a 2020 2020 2020 2020  ame']]..        
-00002050: 7365 6c66 2e5f 5f64 6963 745f 5f2e 7570  self.__dict__.up
-00002060: 6461 7465 286e 6577 5f69 6e66 6f29 0d0a  date(new_info)..
-00002070: 2020 2020 2020 2020 7365 6c66 2e6c 6f61          self.loa
-00002080: 6465 6420 3d20 5472 7565 0d0a 2020 2020  ded = True..    
-00002090: 2020 2020 0d0a 0d0a 636c 6173 7320 506c      ....class Pl
-000020a0: 7567 696e 4d61 6e61 6765 7228 5174 5769  uginManager(QtWi
-000020b0: 6467 6574 732e 514d 6169 6e57 696e 646f  dgets.QMainWindo
-000020c0: 7729 3a0d 0a20 2020 2070 6c75 6769 6e73  w):..    plugins
-000020d0: 203d 207b 7d0d 0a20 2020 206c 6f61 6454   = {}..    loadT
-000020e0: 6872 6561 6420 3d20 4e6f 6e65 0d0a 2020  hread = None..  
-000020f0: 2020 7369 6750 6c75 6769 6e4c 6f61 6465    sigPluginLoade
-00002100: 6420 3d20 5174 436f 7265 2e53 6967 6e61  d = QtCore.Signa
-00002110: 6c28 7374 7229 0d0a 2020 2020 2727 270d  l(str)..    '''.
-00002120: 0a20 2020 2050 6c75 6769 6e4d 616e 6167  .    PluginManag
-00002130: 6572 2068 616e 646c 6573 2069 6e73 7461  er handles insta
-00002140: 6c6c 6564 2070 6c75 6769 6e73 2061 6e64  lled plugins and
-00002150: 2074 6865 206f 6e6c 696e 6520 706c 7567   the online plug
-00002160: 696e 2064 6174 6162 6173 650d 0a20 2020  in database..   
-00002170: 207c 2073 686f 7728 2920 3a20 696e 6974   | show() : init
-00002180: 6961 6c69 7a65 7320 6120 6775 6920 6173  ializes a gui as
-00002190: 2061 2073 7461 7469 6320 7661 7269 6162   a static variab
-000021a0: 6c65 206f 6620 7468 6520 636c 6173 732c  le of the class,
-000021b0: 2069 6620 6e65 6365 7373 6172 792c 2061   if necessary, a
-000021c0: 6e64 2064 6973 706c 6179 7320 6974 2e20  nd displays it. 
-000021d0: 4361 6c6c 2069 6e20 706c 6163 6520 6f66  Call in place of
-000021e0: 2063 6f6e 7374 7275 6374 6f72 0d0a 2020   constructor..  
-000021f0: 2020 7c20 636c 6f73 6528 2920 3a20 636c    | close() : cl
-00002200: 6f73 6573 2074 6865 2067 7569 2069 6620  oses the gui if 
-00002210: 6974 2065 7869 7374 730d 0a20 2020 2027  it exists..    '
-00002220: 2727 0d0a 2020 2020 4073 7461 7469 636d  ''..    @staticm
-00002230: 6574 686f 640d 0a20 2020 2064 6566 2073  ethod..    def s
-00002240: 686f 7728 293a 0d0a 2020 2020 2020 2020  how():..        
-00002250: 6966 206e 6f74 2068 6173 6174 7472 2850  if not hasattr(P
-00002260: 6c75 6769 6e4d 616e 6167 6572 2c20 2767  luginManager, 'g
-00002270: 7569 2729 3a0d 0a20 2020 2020 2020 2020  ui'):..         
-00002280: 2020 2050 6c75 6769 6e4d 616e 6167 6572     PluginManager
-00002290: 2e67 7569 203d 2050 6c75 6769 6e4d 616e  .gui = PluginMan
-000022a0: 6167 6572 2829 0d0a 2020 2020 2020 2020  ager()..        
-000022b0: 506c 7567 696e 4d61 6e61 6765 722e 6775  PluginManager.gu
-000022c0: 692e 7368 6f77 506c 7567 696e 7328 290d  i.showPlugins().
-000022d0: 0a20 2020 2020 2020 2023 506c 7567 696e  .        #Plugin
-000022e0: 4d61 6e61 6765 722e 6c6f 6164 5f6f 6e6c  Manager.load_onl
-000022f0: 696e 655f 706c 7567 696e 7328 290d 0a20  ine_plugins().. 
-00002300: 2020 2020 2020 2051 7457 6964 6765 7473         QtWidgets
-00002310: 2e51 4d61 696e 5769 6e64 6f77 2e73 686f  .QMainWindow.sho
-00002320: 7728 506c 7567 696e 4d61 6e61 6765 722e  w(PluginManager.
-00002330: 6775 6929 0d0a 2020 2020 2020 2020 6966  gui)..        if
-00002340: 206e 6f74 206f 732e 6163 6365 7373 2867   not os.access(g
-00002350: 6574 5f70 6c75 6769 6e5f 6469 7265 6374  et_plugin_direct
-00002360: 6f72 7928 292c 206f 732e 575f 4f4b 293a  ory(), os.W_OK):
-00002370: 0d0a 2020 2020 2020 2020 2020 2020 672e  ..            g.
-00002380: 616c 6572 7428 2250 6c75 6769 6e20 666f  alert("Plugin fo
-00002390: 6c64 6572 2077 7269 7465 2070 6572 6d69  lder write permi
-000023a0: 7373 696f 6e20 6465 6e69 6564 2e20 5265  ssion denied. Re
-000023b0: 7374 6172 7420 666c 696b 6120 6173 2061  start flika as a
-000023c0: 646d 696e 6973 7472 6174 6f72 2074 6f20  dministrator to 
-000023d0: 656e 6162 6c65 2070 6c75 6769 6e20 696e  enable plugin in
-000023e0: 7374 616c 6c61 7469 6f6e 2e22 290d 0a0d  stallation.")...
-000023f0: 0a20 2020 2020 2020 2050 6c75 6769 6e4d  .        PluginM
-00002400: 616e 6167 6572 2e67 7569 2e73 686f 7748  anager.gui.showH
-00002410: 656c 7053 6372 6565 6e28 290d 0a0d 0a0d  elpScreen().....
-00002420: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-00002430: 6f64 0d0a 2020 2020 6465 6620 7265 6672  od..    def refr
-00002440: 6573 685f 6f6e 6c69 6e65 5f70 6c75 6769  esh_online_plugi
-00002450: 6e73 2829 3a0d 0a20 2020 2020 2020 2066  ns():..        f
-00002460: 6f72 2070 2069 6e20 706c 7567 696e 5f6c  or p in plugin_l
-00002470: 6973 742e 6b65 7973 2829 3a0d 0a20 2020  ist.keys():..   
-00002480: 2020 2020 2020 2020 2050 6c75 6769 6e4d           PluginM
-00002490: 616e 6167 6572 2e6c 6f61 645f 6f6e 6c69  anager.load_onli
-000024a0: 6e65 5f70 6c75 6769 6e28 7029 0d0a 0d0a  ne_plugin(p)....
-000024b0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-000024c0: 640d 0a20 2020 2064 6566 206c 6f61 645f  d..    def load_
-000024d0: 6f6e 6c69 6e65 5f70 6c75 6769 6e28 7029  online_plugin(p)
-000024e0: 3a0d 0a20 2020 2020 2020 2069 6620 7020  :..        if p 
-000024f0: 6e6f 7420 696e 2070 6c75 6769 6e5f 6c69  not in plugin_li
-00002500: 7374 206f 7220 506c 7567 696e 4d61 6e61  st or PluginMana
-00002510: 6765 722e 6c6f 6164 5468 7265 6164 2069  ger.loadThread i
-00002520: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2050  s not None and P
-00002530: 6c75 6769 6e4d 616e 6167 6572 2e6c 6f61  luginManager.loa
-00002540: 6454 6872 6561 642e 6973 5f61 6c69 7665  dThread.is_alive
-00002550: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00002560: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
-00002570: 2064 6566 206c 6f61 6454 6872 6561 6428   def loadThread(
-00002580: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00002590: 706c 7567 203d 2050 6c75 6769 6e4d 616e  plug = PluginMan
-000025a0: 6167 6572 2e70 6c75 6769 6e73 5b70 5d0d  ager.plugins[p].
-000025b0: 0a20 2020 2020 2020 2020 2020 2070 6c75  .            plu
-000025c0: 672e 696e 666f 5f75 726c 203d 2070 6c75  g.info_url = plu
-000025d0: 6769 6e5f 6c69 7374 5b70 5d0d 0a20 2020  gin_list[p]..   
-000025e0: 2020 2020 2020 2020 2070 6c75 672e 7570           plug.up
-000025f0: 6461 7465 5f69 6e66 6f28 290d 0a20 2020  date_info()..   
-00002600: 2020 2020 2020 2020 2050 6c75 6769 6e4d           PluginM
-00002610: 616e 6167 6572 2e67 7569 2e73 6967 506c  anager.gui.sigPl
-00002620: 7567 696e 4c6f 6164 6564 2e65 6d69 7428  uginLoaded.emit(
-00002630: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
-00002640: 2350 6c75 6769 6e4d 616e 6167 6572 2e67  #PluginManager.g
-00002650: 7569 2e73 7461 7475 7342 6172 2e73 686f  ui.statusBar.sho
-00002660: 774d 6573 7361 6765 2827 506c 7567 696e  wMessage('Plugin
-00002670: 2069 6e66 6f72 6d61 7469 6f6e 206c 6f61   information loa
-00002680: 6465 6420 7375 6363 6573 7366 756c 6c79  ded successfully
-00002690: 2729 0d0a 0d0a 2020 2020 2020 2020 506c  ')....        Pl
-000026a0: 7567 696e 4d61 6e61 6765 722e 6c6f 6164  uginManager.load
-000026b0: 5468 7265 6164 203d 2074 6872 6561 6469  Thread = threadi
-000026c0: 6e67 2e54 6872 6561 6428 4e6f 6e65 2c20  ng.Thread(None, 
-000026d0: 6c6f 6164 5468 7265 6164 290d 0a20 2020  loadThread)..   
-000026e0: 2020 2020 2050 6c75 6769 6e4d 616e 6167       PluginManag
-000026f0: 6572 2e67 7569 2e73 7461 7475 7342 6172  er.gui.statusBar
-00002700: 2e73 686f 774d 6573 7361 6765 2827 4c6f  .showMessage('Lo
-00002710: 6164 696e 6720 706c 7567 696e 2069 6e66  ading plugin inf
-00002720: 6f72 6d61 7469 6f6e 2066 6f72 207b 7d2e  ormation for {}.
-00002730: 2e2e 272e 666f 726d 6174 2870 2929 0d0a  ..'.format(p))..
-00002740: 2020 2020 2020 2020 506c 7567 696e 4d61          PluginMa
-00002750: 6e61 6765 722e 6c6f 6164 5468 7265 6164  nager.loadThread
-00002760: 2e73 7461 7274 2829 0d0a 0d0a 2020 2020  .start()....    
-00002770: 6465 6620 636c 6f73 6545 7665 6e74 2873  def closeEvent(s
-00002780: 656c 662c 2065 7629 3a0d 0a20 2020 2020  elf, ev):..     
-00002790: 2020 2069 6620 7365 6c66 2e6c 6f61 6454     if self.loadT
+000003c0: 7079 6e73 6967 6874 2f6d 6173 7465 722f  pynsight/master/
+000003d0: 272c 0a20 2020 2027 5175 616e 7469 4d75  ',.    'QuantiMu
+000003e0: 7327 3a20 2020 2020 2020 2027 6874 7470  s':        'http
+000003f0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000400: 7263 6f6e 7465 6e74 2e63 6f6d 2f51 7561  rcontent.com/Qua
+00000410: 6e74 696d 7573 2f71 7561 6e74 696d 7573  ntimus/quantimus
+00000420: 2f6d 6173 7465 722f 272c 0a20 2020 2027  /master/',.    '
+00000430: 526f 6465 6e74 2054 7261 636b 6572 273a  Rodent Tracker':
+00000440: 2020 2027 6874 7470 733a 2f2f 7261 772e     'https://raw.
+00000450: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000460: 742e 636f 6d2f 6b79 6c65 656c 6c65 6673  t.com/kyleellefs
+00000470: 656e 2f72 6f64 656e 7454 7261 636b 6572  en/rodentTracker
+00000480: 2f6d 6173 7465 722f 270a 7d0a 0a68 656c  /master/'.}..hel
+00000490: 7048 544d 4c20 3d20 2727 270a 3c68 3120  pHTML = '''.<h1 
+000004a0: 7374 796c 653d 2277 6964 7468 3a31 3030  style="width:100
+000004b0: 253b 2074 6578 742d 616c 6967 6e3a 6365  %; text-align:ce
+000004c0: 6e74 6572 223e 5765 6c63 6f6d 6520 746f  nter">Welcome to
+000004d0: 2074 6865 2066 6c69 6b61 2050 6c75 6769   the flika Plugi
+000004e0: 6e20 4d61 6e61 6765 723c 2f68 313e 0a3c  n Manager</h1>.<
+000004f0: 703e 5573 6520 7468 6520 7365 6172 6368  p>Use the search
+00000500: 2062 6172 2074 6f20 7468 6520 6c65 6674   bar to the left
+00000510: 2074 6f20 6669 6e64 2061 2073 7065 6369   to find a speci
+00000520: 6669 6320 706c 7567 696e 2c20 6f72 2062  fic plugin, or b
+00000530: 726f 7773 6520 7468 6520 6c69 7374 2062  rowse the list b
+00000540: 656c 6f77 2069 742e 3c2f 703e 0a0a 3c64  elow it.</p>..<d
+00000550: 6976 3e0a 2020 2020 3c68 333e 4465 7665  iv>.    <h3>Deve
+00000560: 6c6f 7020 6120 6e65 7720 706c 7567 696e  lop a new plugin
+00000570: 3c2f 6833 3e0a 2020 2020 3c70 3e20 4966  </h3>.    <p> If
+00000580: 2079 6f75 2077 6f75 6c64 206c 696b 6520   you would like 
+00000590: 746f 2064 6576 656c 6f70 2079 6f75 7220  to develop your 
+000005a0: 6f77 6e20 706c 7567 696e 2066 6f72 2066  own plugin for f
+000005b0: 6c69 6b61 2c20 666f 6c6c 6f77 2074 6865  lika, follow the
+000005c0: 7365 2073 696d 706c 6520 7374 6570 733a  se simple steps:
+000005d0: 3c2f 703e 0a20 2020 203c 756c 206c 6973  </p>.    <ul lis
+000005e0: 742d 7374 796c 653d 6e6f 6e65 3e0a 2020  t-style=none>.  
+000005f0: 2020 2020 2020 3c6c 693e 312e 2044 6f77        <li>1. Dow
+00000600: 6e6c 6f61 6420 3c61 2068 7265 663d 2268  nload <a href="h
+00000610: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000620: 6d2f 666c 696b 612d 6f72 672f 666c 696b  m/flika-org/flik
+00000630: 615f 706c 7567 696e 5f74 656d 706c 6174  a_plugin_templat
+00000640: 6522 3e66 6c69 6b61 2050 6c75 6769 6e20  e">flika Plugin 
+00000650: 5465 6d70 6c61 7465 3c2f 613e 2061 6e64  Template</a> and
+00000660: 2070 6c61 6365 2069 7420 696e 2079 6f75   place it in you
+00000670: 7220 2e46 4c49 4b41 2f70 6c75 6769 6e73  r .FLIKA/plugins
+00000680: 2064 6972 6563 746f 7279 3c2f 6c69 3e0a   directory</li>.
+00000690: 2020 2020 2020 2020 3c6c 693e 322e 2055          <li>2. U
+000006a0: 7064 6174 6520 7468 6520 696e 666f 2e78  pdate the info.x
+000006b0: 6d6c 2066 696c 6520 666f 7220 796f 7572  ml file for your
+000006c0: 2070 6c75 6769 6e3c 2f6c 693e 0a20 2020   plugin</li>.   
+000006d0: 2020 2020 203c 6c69 3e33 2e20 5265 6665       <li>3. Refe
+000006e0: 7220 746f 2074 6865 203c 6120 6872 6566  r to the <a href
+000006f0: 3d22 6874 7470 3a2f 2f66 6c69 6b61 2d6f  ="http://flika-o
+00000700: 7267 2e67 6974 6875 622e 696f 2f77 7269  rg.github.io/wri
+00000710: 7469 6e67 5f70 6c75 6769 6e73 2e68 746d  ting_plugins.htm
+00000720: 6c22 3e66 6c69 6b61 2044 6f63 756d 656e  l">flika Documen
+00000730: 7461 7469 6f6e 3c2f 613e 2066 6f72 2061  tation</a> for a
+00000740: 7373 6973 7461 6e63 6520 6465 7665 6c6f  ssistance develo
+00000750: 7069 6e67 2079 6f75 7220 706c 7567 696e  ping your plugin
+00000760: 2e3c 2f6c 693e 0a20 2020 2020 2020 203c  .</li>.        <
+00000770: 6c69 3e34 2e20 5570 6461 7465 2074 6865  li>4. Update the
+00000780: 2064 6573 6372 6970 7469 6f6e 2e68 746d   description.htm
+00000790: 6c20 6669 6c65 2066 6f72 2079 6f75 7220  l file for your 
+000007a0: 706c 7567 696e 3c2f 6c69 3e0a 2020 2020  plugin</li>.    
+000007b0: 2020 2020 3c6c 693e 352e 2053 656e 6420      <li>5. Send 
+000007c0: 796f 7572 2070 6c75 6769 6e20 7265 706f  your plugin repo
+000007d0: 2074 6f20 7573 2061 6e64 2077 6527 6c6c   to us and we'll
+000007e0: 2061 6464 2069 7420 746f 2074 6865 2050   add it to the P
+000007f0: 6c75 6769 6e20 4d61 6e61 6765 7221 3c2f  lugin Manager!</
+00000800: 6c69 3e0a 2020 2020 3c2f 756c 3e0a 3c64  li>.    </ul>.<d
+00000810: 6976 3e0a 2727 270a 0a0a 6465 6620 6765  iv>.'''...def ge
+00000820: 745f 706c 7567 696e 5f64 6972 6563 746f  t_plugin_directo
+00000830: 7279 2829 3a0a 2020 2020 6c6f 6767 6572  ry():.    logger
+00000840: 2e64 6562 7567 2827 4361 6c6c 696e 6720  .debug('Calling 
+00000850: 6170 702e 706c 7567 696e 5f6d 616e 6167  app.plugin_manag
+00000860: 6572 2e67 6574 5f70 6c75 6769 6e5f 6469  er.get_plugin_di
+00000870: 7265 6374 6f72 7927 290a 2020 2020 6c6f  rectory').    lo
+00000880: 6361 6c5f 666c 696b 615f 6469 7265 6374  cal_flika_direct
+00000890: 6f72 7920 3d20 6f73 2e70 6174 682e 6a6f  ory = os.path.jo
+000008a0: 696e 2865 7870 616e 6475 7365 7228 227e  in(expanduser("~
+000008b0: 2229 2c20 272e 464c 494b 4127 290a 2020  "), '.FLIKA').  
+000008c0: 2020 706c 7567 696e 5f64 6972 6563 746f    plugin_directo
+000008d0: 7279 203d 206f 732e 7061 7468 2e6a 6f69  ry = os.path.joi
+000008e0: 6e28 6578 7061 6e64 7573 6572 2822 7e22  n(expanduser("~"
+000008f0: 292c 2027 2e46 4c49 4b41 272c 2027 706c  ), '.FLIKA', 'pl
+00000900: 7567 696e 7327 2029 0a20 2020 2069 6620  ugins' ).    if 
+00000910: 6e6f 7420 6f73 2e70 6174 682e 6578 6973  not os.path.exis
+00000920: 7473 2870 6c75 6769 6e5f 6469 7265 6374  ts(plugin_direct
+00000930: 6f72 7929 3a0a 2020 2020 2020 2020 6f73  ory):.        os
+00000940: 2e6d 616b 6564 6972 7328 706c 7567 696e  .makedirs(plugin
+00000950: 5f64 6972 6563 746f 7279 290a 2020 2020  _directory).    
+00000960: 6966 206e 6f74 206f 732e 7061 7468 2e69  if not os.path.i
+00000970: 7366 696c 6528 6f73 2e70 6174 682e 6a6f  sfile(os.path.jo
+00000980: 696e 2870 6c75 6769 6e5f 6469 7265 6374  in(plugin_direct
+00000990: 6f72 792c 2027 5f5f 696e 6974 5f5f 2e70  ory, '__init__.p
+000009a0: 7927 2929 3a0a 2020 2020 2020 2020 6f70  y')):.        op
+000009b0: 656e 286f 732e 7061 7468 2e6a 6f69 6e28  en(os.path.join(
+000009c0: 706c 7567 696e 5f64 6972 6563 746f 7279  plugin_directory
+000009d0: 2c20 275f 5f69 6e69 745f 5f2e 7079 2729  , '__init__.py')
+000009e0: 2c20 2761 2729 2e63 6c6f 7365 2829 2020  , 'a').close()  
+000009f0: 2320 4372 6561 7465 2065 6d70 7479 205f  # Create empty _
+00000a00: 5f69 6e69 745f 5f2e 7079 2066 696c 650a  _init__.py file.
+00000a10: 2020 2020 6966 2070 6c75 6769 6e5f 6469      if plugin_di
+00000a20: 7265 6374 6f72 7920 6e6f 7420 696e 2073  rectory not in s
+00000a30: 7973 2e70 6174 683a 0a20 2020 2020 2020  ys.path:.       
+00000a40: 2073 7973 2e70 6174 682e 6170 7065 6e64   sys.path.append
+00000a50: 2870 6c75 6769 6e5f 6469 7265 6374 6f72  (plugin_director
+00000a60: 7929 0a20 2020 2069 6620 6c6f 6361 6c5f  y).    if local_
+00000a70: 666c 696b 615f 6469 7265 6374 6f72 7920  flika_directory 
+00000a80: 6e6f 7420 696e 2073 7973 2e70 6174 683a  not in sys.path:
+00000a90: 0a20 2020 2020 2020 2073 7973 2e70 6174  .        sys.pat
+00000aa0: 682e 6170 7065 6e64 286c 6f63 616c 5f66  h.append(local_f
+00000ab0: 6c69 6b61 5f64 6972 6563 746f 7279 290a  lika_directory).
+00000ac0: 2020 2020 7265 7475 726e 2070 6c75 6769      return plugi
+00000ad0: 6e5f 6469 7265 6374 6f72 790a 0a70 6c75  n_directory..plu
+00000ae0: 6769 6e5f 6469 7220 3d20 6765 745f 706c  gin_dir = get_pl
+00000af0: 7567 696e 5f64 6972 6563 746f 7279 2829  ugin_directory()
+00000b00: 0a0a 0a64 6566 2070 6172 7365 2878 293a  ...def parse(x):
+00000b10: 0a20 2020 2023 6c6f 6767 6572 2e64 6562  .    #logger.deb
+00000b20: 7567 2827 4361 6c6c 696e 6720 6170 702e  ug('Calling app.
+00000b30: 706c 7567 696e 5f6d 616e 6167 6572 2e70  plugin_manager.p
+00000b40: 6172 7365 2729 0a20 2020 2074 7265 6520  arse').    tree 
+00000b50: 3d20 456c 656d 656e 7454 7265 652e 6672  = ElementTree.fr
+00000b60: 6f6d 7374 7269 6e67 2878 290a 2020 2020  omstring(x).    
+00000b70: 6465 6620 7374 6570 2869 7465 6d29 3a0a  def step(item):.
+00000b80: 2020 2020 2020 2020 6420 3d20 7b7d 0a20          d = {}. 
+00000b90: 2020 2020 2020 2069 6620 6974 656d 2e74         if item.t
+00000ba0: 6578 7420 616e 6420 6974 656d 2e74 6578  ext and item.tex
+00000bb0: 742e 7374 7269 7028 293a 0a20 2020 2020  t.strip():.     
+00000bc0: 2020 2020 2020 2064 5b27 2374 6578 7427         d['#text'
+00000bd0: 5d20 3d20 6974 656d 2e74 6578 742e 7374  ] = item.text.st
+00000be0: 7269 7028 290a 2020 2020 2020 2020 666f  rip().        fo
+00000bf0: 7220 6b2c 2076 2069 6e20 6974 656d 2e69  r k, v in item.i
+00000c00: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00000c10: 2020 2020 645b 2740 2573 2720 2520 6b5d      d['@%s' % k]
+00000c20: 203d 2076 0a20 2020 2020 2020 2066 6f72   = v.        for
+00000c30: 206b 2069 6e20 6c69 7374 2869 7465 6d29   k in list(item)
+00000c40: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00000c50: 206b 2e74 6167 206e 6f74 2069 6e20 643a   k.tag not in d:
+00000c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c70: 2064 5b6b 2e74 6167 5d20 3d20 7374 6570   d[k.tag] = step
+00000c80: 286b 290a 2020 2020 2020 2020 2020 2020  (k).            
+00000c90: 656c 6966 2074 7970 6528 645b 6b2e 7461  elif type(d[k.ta
+00000ca0: 675d 2920 3d3d 206c 6973 743a 0a20 2020  g]) == list:.   
+00000cb0: 2020 2020 2020 2020 2020 2020 2064 5b6b               d[k
+00000cc0: 2e74 6167 5d2e 6170 7065 6e64 2873 7465  .tag].append(ste
+00000cd0: 7028 6b29 290a 2020 2020 2020 2020 2020  p(k)).          
+00000ce0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00000cf0: 2020 2020 2020 2020 645b 6b2e 7461 675d          d[k.tag]
+00000d00: 203d 205b 645b 6b2e 7461 675d 2c20 7374   = [d[k.tag], st
+00000d10: 6570 286b 295d 0a20 2020 2020 2020 2069  ep(k)].        i
+00000d20: 6620 6c65 6e28 6429 203d 3d20 3120 616e  f len(d) == 1 an
+00000d30: 6420 2723 7465 7874 2720 696e 2064 3a0a  d '#text' in d:.
+00000d40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000d50: 726e 2064 5b27 2374 6578 7427 5d0a 2020  rn d['#text'].  
+00000d60: 2020 2020 2020 7265 7475 726e 2064 0a20        return d. 
+00000d70: 2020 2072 6574 7572 6e20 7374 6570 2874     return step(t
+00000d80: 7265 6529 0a0a 0a64 6566 2073 7472 3266  ree)...def str2f
+00000d90: 756e 6328 706c 7567 696e 5f6e 616d 652c  unc(plugin_name,
+00000da0: 2066 696c 655f 6c6f 6361 7469 6f6e 2c20   file_location, 
+00000db0: 6675 6e63 7469 6f6e 293a 0a20 2020 2027  function):.    '
+00000dc0: 2727 0a20 2020 2074 616b 6573 2070 6c75  ''.    takes plu
+00000dd0: 6769 6e5f 6e61 6d65 2c20 7061 7468 2074  gin_name, path t
+00000de0: 6f20 6f62 6a65 6374 2c20 6675 6e63 7469  o object, functi
+00000df0: 6f6e 2061 7320 6172 6775 6d65 6e74 730a  on as arguments.
+00000e00: 2020 2020 696d 706f 7274 7320 706c 7567      imports plug
+00000e10: 696e 5f6e 616d 652e 7061 7468 2061 6e64  in_name.path and
+00000e20: 2067 6574 7320 7468 6520 6675 6e63 7469   gets the functi
+00000e30: 6f6e 2066 726f 6d20 7468 6174 2069 6d70  on from that imp
+00000e40: 6f72 7465 6420 6f62 6a65 6374 0a20 2020  orted object.   
+00000e50: 2074 6f20 6265 2072 756e 2077 6865 6e20   to be run when 
+00000e60: 616e 2061 6374 696f 6e20 6973 2063 6c69  an action is cli
+00000e70: 636b 6564 0a20 2020 2027 2727 0a20 2020  cked.    '''.   
+00000e80: 2023 6c6f 6767 6572 2e64 6562 7567 2822   #logger.debug("
+00000e90: 5374 6172 7465 6420 2761 7070 2e70 6c75  Started 'app.plu
+00000ea0: 6769 6e5f 6d61 6e61 6765 722e 7374 7232  gin_manager.str2
+00000eb0: 6675 6e63 287b 7d2c 207b 7d2c 207b 7d29  func({}, {}, {})
+00000ec0: 2722 2e66 6f72 6d61 7428 706c 7567 696e  '".format(plugin
+00000ed0: 5f6e 616d 652c 2066 696c 655f 6c6f 6361  _name, file_loca
+00000ee0: 7469 6f6e 2c20 6675 6e63 7469 6f6e 2929  tion, function))
+00000ef0: 0a20 2020 205f 5f69 6d70 6f72 745f 5f28  .    __import__(
+00000f00: 706c 7567 696e 5f6e 616d 6529 0a20 2020  plugin_name).   
+00000f10: 2070 6c75 6769 6e5f 6469 7220 3d20 2270   plugin_dir = "p
+00000f20: 6c75 6769 6e73 2e7b 7d2e 7b7d 222e 666f  lugins.{}.{}".fo
+00000f30: 726d 6174 2870 6c75 6769 6e5f 6e61 6d65  rmat(plugin_name
+00000f40: 2c20 6669 6c65 5f6c 6f63 6174 696f 6e29  , file_location)
+00000f50: 0a20 2020 206c 6576 656c 7320 3d20 6675  .    levels = fu
+00000f60: 6e63 7469 6f6e 2e73 706c 6974 2827 2e27  nction.split('.'
+00000f70: 290a 2020 2020 6d6f 6475 6c65 203d 205f  ).    module = _
+00000f80: 5f69 6d70 6f72 745f 5f28 706c 7567 696e  _import__(plugin
+00000f90: 5f64 6972 2c20 6672 6f6d 6c69 7374 3d5b  _dir, fromlist=[
+00000fa0: 6c65 7665 6c73 5b30 5d5d 292e 5f5f 6469  levels[0]]).__di
+00000fb0: 6374 5f5f 5b6c 6576 656c 735b 305d 5d0a  ct__[levels[0]].
+00000fc0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00000fd0: 6765 2831 2c20 6c65 6e28 6c65 7665 6c73  ge(1, len(levels
+00000fe0: 2929 3a0a 2020 2020 2020 2020 6d6f 6475  )):.        modu
+00000ff0: 6c65 203d 2067 6574 6174 7472 286d 6f64  le = getattr(mod
+00001000: 756c 652c 206c 6576 656c 735b 695d 290a  ule, levels[i]).
+00001010: 2020 2020 236c 6f67 6765 722e 6465 6275      #logger.debu
+00001020: 6728 2243 6f6d 706c 6574 6564 2027 6170  g("Completed 'ap
+00001030: 702e 706c 7567 696e 5f6d 616e 6167 6572  p.plugin_manager
+00001040: 2e73 7472 3266 756e 6328 7b7d 2c20 7b7d  .str2func({}, {}
+00001050: 2c20 7b7d 2927 222e 666f 726d 6174 2870  , {})'".format(p
+00001060: 6c75 6769 6e5f 6e61 6d65 2c20 6669 6c65  lugin_name, file
+00001070: 5f6c 6f63 6174 696f 6e2c 2066 756e 6374  _location, funct
+00001080: 696f 6e29 290a 2020 2020 7265 7475 726e  ion)).    return
+00001090: 206d 6f64 756c 650a 0a0a 6465 6620 6661   module...def fa
+000010a0: 6b65 5f73 7472 3266 756e 6328 706c 7567  ke_str2func(plug
+000010b0: 696e 5f6e 616d 652c 2066 696c 655f 6c6f  in_name, file_lo
+000010c0: 6361 7469 6f6e 2c20 6675 6e63 7469 6f6e  cation, function
+000010d0: 293a 0a20 2020 2064 6566 2066 616b 655f  ):.    def fake_
+000010e0: 6675 6e28 293a 0a20 2020 2020 2020 2070  fun():.        p
+000010f0: 7269 6e74 2873 7472 2866 756e 6374 696f  rint(str(functio
+00001100: 6e29 290a 2020 2020 2020 2020 7072 696e  n)).        prin
+00001110: 7428 2779 6179 2729 0a20 2020 2072 6574  t('yay').    ret
+00001120: 7572 6e20 6661 6b65 5f66 756e 0a0a 6465  urn fake_fun..de
+00001130: 6620 6275 696c 645f 7375 626d 656e 7528  f build_submenu(
+00001140: 6d6f 6475 6c65 5f6e 616d 652c 2070 6172  module_name, par
+00001150: 656e 745f 6d65 6e75 2c20 6c61 796f 7574  ent_menu, layout
+00001160: 5f64 6963 7429 3a0a 2020 2020 236c 6f67  _dict):.    #log
+00001170: 6765 722e 6465 6275 6728 2743 616c 6c69  ger.debug('Calli
+00001180: 6e67 2061 7070 2e70 6c75 6769 6e5f 6d61  ng app.plugin_ma
+00001190: 6e61 6765 722e 6275 696c 645f 7375 626d  nager.build_subm
+000011a0: 656e 7527 290a 2020 2020 6966 206c 656e  enu').    if len
+000011b0: 286c 6179 6f75 745f 6469 6374 2920 3d3d  (layout_dict) ==
+000011c0: 2030 3a0a 2020 2020 2020 2020 672e 616c   0:.        g.al
+000011d0: 6572 7428 2245 7272 6f72 2062 7569 6c64  ert("Error build
+000011e0: 696e 6720 7375 626d 656e 7520 666f 7220  ing submenu for 
+000011f0: 7468 6520 706c 7567 696e 2027 7b7d 272e  the plugin '{}'.
+00001200: 204e 6f20 6974 656d 7320 666f 756e 6420   No items found 
+00001210: 696e 2027 6d65 6e75 5f6c 6179 6f75 7427  in 'menu_layout'
+00001220: 2069 6e20 7468 6520 696e 666f 2e78 6d6c   in the info.xml
+00001230: 2066 696c 652e 222e 666f 726d 6174 286d   file.".format(m
+00001240: 6f64 756c 655f 6e61 6d65 2929 0a20 2020  odule_name)).   
+00001250: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
+00001260: 696e 206c 6179 6f75 745f 6469 6374 2e69  in layout_dict.i
+00001270: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00001280: 6966 2074 7970 6528 7661 6c75 6529 2021  if type(value) !
+00001290: 3d20 6c69 7374 3a0a 2020 2020 2020 2020  = list:.        
+000012a0: 2020 2020 7661 6c75 6520 3d20 5b76 616c      value = [val
+000012b0: 7565 5d0a 2020 2020 2020 2020 6966 206b  ue].        if k
+000012c0: 6579 203d 3d20 276d 656e 7527 3a0a 2020  ey == 'menu':.  
+000012d0: 2020 2020 2020 2020 2020 666f 7220 7620            for v 
+000012e0: 696e 2076 616c 7565 3a0a 2020 2020 2020  in value:.      
+000012f0: 2020 2020 2020 2020 2020 6d65 6e75 203d            menu =
+00001300: 2070 6172 656e 745f 6d65 6e75 2e61 6464   parent_menu.add
+00001310: 4d65 6e75 2876 5b22 406e 616d 6522 5d29  Menu(v["@name"])
+00001320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001330: 2062 7569 6c64 5f73 7562 6d65 6e75 286d   build_submenu(m
+00001340: 6f64 756c 655f 6e61 6d65 2c20 6d65 6e75  odule_name, menu
+00001350: 2c20 7629 0a20 2020 2020 2020 2065 6c69  , v).        eli
+00001360: 6620 6b65 7920 3d3d 2027 6163 7469 6f6e  f key == 'action
+00001370: 273a 0a20 2020 2020 2020 2020 2020 2066  ':.            f
+00001380: 6f72 206f 6420 696e 2076 616c 7565 3a0a  or od in value:.
+00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013a0: 6d65 7468 6f64 203d 2073 7472 3266 756e  method = str2fun
+000013b0: 6328 6d6f 6475 6c65 5f6e 616d 652c 206f  c(module_name, o
+000013c0: 645b 2740 6c6f 6361 7469 6f6e 275d 2c20  d['@location'], 
+000013d0: 6f64 5b27 4066 756e 6374 696f 6e27 5d29  od['@function'])
+000013e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000013f0: 2069 6620 6d65 7468 6f64 2069 7320 6e6f   if method is no
+00001400: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00001410: 2020 2020 2020 2020 2020 2020 6163 7469              acti
+00001420: 6f6e 203d 2051 7457 6964 6765 7473 2e51  on = QtWidgets.Q
+00001430: 4163 7469 6f6e 286f 645b 2723 7465 7874  Action(od['#text
+00001440: 275d 2c20 7061 7265 6e74 5f6d 656e 752c  '], parent_menu,
+00001450: 2074 7269 6767 6572 6564 203d 206d 6574   triggered = met
+00001460: 686f 6429 0a20 2020 2020 2020 2020 2020  hod).           
+00001470: 2020 2020 2020 2020 2070 6172 656e 745f           parent_
+00001480: 6d65 6e75 2e61 6464 4163 7469 6f6e 2861  menu.addAction(a
+00001490: 6374 696f 6e29 0a0a 0a63 6c61 7373 2050  ction)...class P
+000014a0: 6c75 6769 6e28 293a 0a20 2020 2064 6566  lugin():.    def
+000014b0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+000014c0: 6e61 6d65 3d4e 6f6e 652c 2069 6e66 6f5f  name=None, info_
+000014d0: 7572 6c3d 4e6f 6e65 293a 0a20 2020 2020  url=None):.     
+000014e0: 2020 2073 656c 662e 6e61 6d65 203d 206e     self.name = n
+000014f0: 616d 650a 2020 2020 2020 2020 7365 6c66  ame.        self
+00001500: 2e64 6972 6563 746f 7279 203d 204e 6f6e  .directory = Non
+00001510: 650a 2020 2020 2020 2020 7365 6c66 2e75  e.        self.u
+00001520: 726c 203d 204e 6f6e 650a 2020 2020 2020  rl = None.      
+00001530: 2020 7365 6c66 2e61 7574 686f 7220 3d20    self.author = 
+00001540: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+00001550: 662e 646f 6375 6d65 6e74 6174 696f 6e20  f.documentation 
+00001560: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00001570: 656c 662e 7665 7273 696f 6e20 3d20 2727  elf.version = ''
+00001580: 0a20 2020 2020 2020 2073 656c 662e 6c61  .        self.la
+00001590: 7465 7374 5f76 6572 7369 6f6e 203d 2027  test_version = '
+000015a0: 270a 2020 2020 2020 2020 7365 6c66 2e6d  '.        self.m
+000015b0: 656e 7520 3d20 4e6f 6e65 0a20 2020 2020  enu = None.     
+000015c0: 2020 2073 656c 662e 6c69 7374 5769 6467     self.listWidg
+000015d0: 6574 203d 2051 7457 6964 6765 7473 2e51  et = QtWidgets.Q
+000015e0: 4c69 7374 5769 6467 6574 4974 656d 2873  ListWidgetItem(s
+000015f0: 656c 662e 6e61 6d65 290a 2020 2020 2020  elf.name).      
+00001600: 2020 7365 6c66 2e69 6e73 7461 6c6c 6564    self.installed
+00001610: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00001620: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+00001630: 6e20 3d20 2727 0a20 2020 2020 2020 2073  n = ''.        s
+00001640: 656c 662e 6465 7065 6e64 656e 6369 6573  elf.dependencies
+00001650: 203d 205b 5d0a 2020 2020 2020 2020 7365   = [].        se
+00001660: 6c66 2e6c 6f61 6465 6420 3d20 4661 6c73  lf.loaded = Fals
+00001670: 650a 2020 2020 2020 2020 7365 6c66 2e69  e.        self.i
+00001680: 6e66 6f5f 7572 6c20 3d20 696e 666f 5f75  nfo_url = info_u
+00001690: 726c 0a20 2020 2020 2020 2069 6620 696e  rl.        if in
+000016a0: 666f 5f75 726c 3a0a 2020 2020 2020 2020  fo_url:.        
+000016b0: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
+000016c0: 696e 666f 2829 0a0a 2020 2020 6465 6620  info()..    def 
+000016d0: 6c61 7374 4d6f 6469 6669 6564 2873 656c  lastModified(sel
+000016e0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+000016f0: 726e 206f 732e 7061 7468 2e67 6574 6d74  rn os.path.getmt
+00001700: 696d 6528 6f73 2e70 6174 682e 6a6f 696e  ime(os.path.join
+00001710: 2870 6c75 6769 6e5f 6469 722c 2073 656c  (plugin_dir, sel
+00001720: 662e 6469 7265 6374 6f72 7929 290a 0a20  f.directory)).. 
+00001730: 2020 2064 6566 2066 726f 6d4c 6f63 616c     def fromLocal
+00001740: 2873 656c 662c 2070 6174 6829 3a0a 2020  (self, path):.  
+00001750: 2020 2020 2020 236c 6f67 6765 722e 6465        #logger.de
+00001760: 6275 6728 2743 616c 6c69 6e67 2061 7070  bug('Calling app
+00001770: 2e70 6c75 6769 6e5f 6d61 6e61 6765 722e  .plugin_manager.
+00001780: 506c 7567 696e 2e66 726f 6d4c 6f63 616c  Plugin.fromLocal
+00001790: 2729 0a20 2020 2020 2020 2077 6974 6820  ').        with 
+000017a0: 6f70 656e 286f 732e 7061 7468 2e6a 6f69  open(os.path.joi
+000017b0: 6e28 7061 7468 2c20 2769 6e66 6f2e 786d  n(path, 'info.xm
+000017c0: 6c27 292c 2027 7227 2920 6173 2066 3a0a  l'), 'r') as f:.
+000017d0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+000017e0: 203d 2066 2e72 6561 6428 290a 2020 2020   = f.read().    
+000017f0: 2020 2020 696e 666f 203d 2070 6172 7365      info = parse
+00001800: 2874 6578 7429 0a20 2020 2020 2020 2073  (text).        s
+00001810: 656c 662e 6e61 6d65 203d 2069 6e66 6f5b  elf.name = info[
+00001820: 2740 6e61 6d65 275d 0a20 2020 2020 2020  '@name'].       
+00001830: 2073 656c 662e 6469 7265 6374 6f72 7920   self.directory 
+00001840: 3d20 696e 666f 5b27 6469 7265 6374 6f72  = info['director
+00001850: 7927 5d0a 2020 2020 2020 2020 7365 6c66  y'].        self
+00001860: 2e76 6572 7369 6f6e 203d 2069 6e66 6f5b  .version = info[
+00001870: 2776 6572 7369 6f6e 275d 0a20 2020 2020  'version'].     
+00001880: 2020 2073 656c 662e 6c61 7465 7374 5f76     self.latest_v
+00001890: 6572 7369 6f6e 203d 2073 656c 662e 7665  ersion = self.ve
+000018a0: 7273 696f 6e0a 2020 2020 2020 2020 7365  rsion.        se
+000018b0: 6c66 2e61 7574 686f 7220 3d20 696e 666f  lf.author = info
+000018c0: 5b27 6175 7468 6f72 275d 0a20 2020 2020  ['author'].     
+000018d0: 2020 2077 6974 6820 6f70 656e 286f 732e     with open(os.
+000018e0: 7061 7468 2e6a 6f69 6e28 7061 7468 2c20  path.join(path, 
+000018f0: 2761 626f 7574 2e68 746d 6c27 292c 2027  'about.html'), '
+00001900: 7227 2920 6173 2066 3a0a 2020 2020 2020  r') as f:.      
+00001910: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00001920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001930: 6465 7363 7269 7074 696f 6e20 3d20 7374  description = st
+00001940: 7228 662e 7265 6164 2829 290a 2020 2020  r(f.read()).    
+00001950: 2020 2020 2020 2020 6578 6365 7074 2046          except F
+00001960: 696c 654e 6f74 466f 756e 6445 7272 6f72  ileNotFoundError
+00001970: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001980: 2020 7365 6c66 2e64 6573 6372 6970 7469    self.descripti
+00001990: 6f6e 203d 2022 4e6f 206c 6f63 616c 2064  on = "No local d
+000019a0: 6573 6372 6970 7469 6f6e 2066 696c 6520  escription file 
+000019b0: 666f 756e 6422 0a20 2020 2020 2020 2073  found".        s
+000019c0: 656c 662e 7572 6c20 3d20 696e 666f 5b27  elf.url = info['
+000019d0: 7572 6c27 5d20 6966 2027 7572 6c27 2069  url'] if 'url' i
+000019e0: 6e20 696e 666f 2065 6c73 6520 4e6f 6e65  n info else None
+000019f0: 0a20 2020 2020 2020 2073 656c 662e 646f  .        self.do
+00001a00: 6375 6d65 6e74 6174 696f 6e20 3d20 696e  cumentation = in
+00001a10: 666f 5b27 646f 6375 6d65 6e74 6174 696f  fo['documentatio
+00001a20: 6e27 5d20 6966 2027 646f 6375 6d65 6e74  n'] if 'document
+00001a30: 6174 696f 6e27 2069 6e20 696e 666f 2065  ation' in info e
+00001a40: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
+00001a50: 2069 6620 2764 6570 656e 6465 6e63 6965   if 'dependencie
+00001a60: 7327 2069 6e20 696e 666f 2061 6e64 2027  s' in info and '
+00001a70: 6465 7065 6e64 656e 6379 2720 696e 2069  dependency' in i
+00001a80: 6e66 6f5b 2764 6570 656e 6465 6e63 6965  nfo['dependencie
+00001a90: 7327 5d3a 0a20 2020 2020 2020 2020 2020  s']:.           
+00001aa0: 2064 6570 7320 3d20 696e 666f 5b27 6465   deps = info['de
+00001ab0: 7065 6e64 656e 6369 6573 275d 5b27 6465  pendencies']['de
+00001ac0: 7065 6e64 656e 6379 275d 0a20 2020 2020  pendency'].     
+00001ad0: 2020 2020 2020 2073 656c 662e 6465 7065         self.depe
+00001ae0: 6e64 656e 6369 6573 203d 205b 645b 2740  ndencies = [d['@
+00001af0: 6e61 6d65 275d 2066 6f72 2064 2069 6e20  name'] for d in 
+00001b00: 6465 7073 5d20 6966 2069 7369 6e73 7461  deps] if isinsta
+00001b10: 6e63 6528 6465 7073 2c20 6c69 7374 2920  nce(deps, list) 
+00001b20: 656c 7365 205b 6465 7073 5b27 406e 616d  else [deps['@nam
+00001b30: 6527 5d5d 0a20 2020 2020 2020 2073 656c  e']].        sel
+00001b40: 662e 6d65 6e75 5f6c 6179 6f75 7420 3d20  f.menu_layout = 
+00001b50: 696e 666f 2e70 6f70 2827 6d65 6e75 5f6c  info.pop('menu_l
+00001b60: 6179 6f75 7427 290a 2020 2020 2020 2020  ayout').        
+00001b70: 7365 6c66 2e6c 6973 7457 6964 6765 7420  self.listWidget 
+00001b80: 3d20 5174 5769 6467 6574 732e 514c 6973  = QtWidgets.QLis
+00001b90: 7457 6964 6765 7449 7465 6d28 7365 6c66  tWidgetItem(self
+00001ba0: 2e6e 616d 6529 0a20 2020 2020 2020 2073  .name).        s
+00001bb0: 656c 662e 6c69 7374 5769 6467 6574 2e73  elf.listWidget.s
+00001bc0: 6574 4963 6f6e 2851 7447 7569 2e51 4963  etIcon(QtGui.QIc
+00001bd0: 6f6e 2869 6d61 6765 5f70 6174 6828 2763  on(image_path('c
+00001be0: 6865 636b 2e70 6e67 2729 2929 0a20 2020  heck.png'))).   
+00001bf0: 2020 2020 2073 656c 662e 6c6f 6164 6564       self.loaded
+00001c00: 203d 2054 7275 650a 0a20 2020 2064 6566   = True..    def
+00001c10: 2062 696e 645f 6d65 6e75 5f61 6e64 5f6d   bind_menu_and_m
+00001c20: 6574 686f 6473 2873 656c 6629 3a0a 2020  ethods(self):.  
+00001c30: 2020 2020 2020 6966 206c 656e 2873 656c        if len(sel
+00001c40: 662e 6d65 6e75 5f6c 6179 6f75 7429 203e  f.menu_layout) >
+00001c50: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00001c60: 7365 6c66 2e6d 656e 7520 3d20 5174 5769  self.menu = QtWi
+00001c70: 6467 6574 732e 514d 656e 7528 7365 6c66  dgets.QMenu(self
+00001c80: 2e6e 616d 6529 0a20 2020 2020 2020 2020  .name).         
+00001c90: 2020 2062 7569 6c64 5f73 7562 6d65 6e75     build_submenu
+00001ca0: 2873 656c 662e 6469 7265 6374 6f72 792c  (self.directory,
+00001cb0: 2073 656c 662e 6d65 6e75 2c20 7365 6c66   self.menu, self
+00001cc0: 2e6d 656e 755f 6c61 796f 7574 290a 2020  .menu_layout).  
+00001cd0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00001ce0: 2020 2020 2020 2020 7365 6c66 2e6d 656e          self.men
+00001cf0: 7520 3d20 4e6f 6e65 0a0a 0a20 2020 2064  u = None...    d
+00001d00: 6566 2075 7064 6174 655f 696e 666f 2873  ef update_info(s
+00001d10: 656c 6629 3a0a 2020 2020 2020 2020 6c6f  elf):.        lo
+00001d20: 6767 6572 2e64 6562 7567 2827 4361 6c6c  gger.debug('Call
+00001d30: 696e 6720 6170 702e 706c 7567 696e 5f6d  ing app.plugin_m
+00001d40: 616e 6167 6572 2e75 7064 6174 655f 696e  anager.update_in
+00001d50: 666f 2729 0a20 2020 2020 2020 2069 6620  fo').        if 
+00001d60: 7365 6c66 2e69 6e66 6f5f 7572 6c20 6973  self.info_url is
+00001d70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00001d80: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00001d90: 2020 2020 2020 2020 696e 666f 5f75 726c          info_url
+00001da0: 203d 2075 726c 6a6f 696e 2873 656c 662e   = urljoin(self.
+00001db0: 696e 666f 5f75 726c 2c20 2769 6e66 6f2e  info_url, 'info.
+00001dc0: 786d 6c27 290a 2020 2020 2020 2020 7472  xml').        tr
+00001dd0: 793a 0a20 2020 2020 2020 2020 2020 2074  y:.            t
+00001de0: 7874 203d 2075 726c 6f70 656e 2869 6e66  xt = urlopen(inf
+00001df0: 6f5f 7572 6c29 2e72 6561 6428 290a 2020  o_url).read().  
+00001e00: 2020 2020 2020 6578 6365 7074 2048 5454        except HTT
+00001e10: 5045 7272 6f72 2061 7320 653a 0a20 2020  PError as e:.   
+00001e20: 2020 2020 2020 2020 2067 2e61 6c65 7274           g.alert
+00001e30: 2822 4661 696c 6564 2074 6f20 7570 6461  ("Failed to upda
+00001e40: 7465 2069 6e66 6f72 6d61 7469 6f6e 2066  te information f
+00001e50: 6f72 207b 7d2e 5c6e 5c74 7b7d 222e 666f  or {}.\n\t{}".fo
+00001e60: 726d 6174 2873 656c 662e 6e61 6d65 2c20  rmat(self.name, 
+00001e70: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+00001e80: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
+00001e90: 6e65 775f 696e 666f 203d 2070 6172 7365  new_info = parse
+00001ea0: 2874 7874 290a 2020 2020 2020 2020 6465  (txt).        de
+00001eb0: 7363 7269 7074 696f 6e5f 7572 6c20 3d20  scription_url = 
+00001ec0: 7572 6c6a 6f69 6e28 7365 6c66 2e69 6e66  urljoin(self.inf
+00001ed0: 6f5f 7572 6c2c 2027 6162 6f75 742e 6874  o_url, 'about.ht
+00001ee0: 6d6c 2729 0a20 2020 2020 2020 2074 7279  ml').        try
+00001ef0: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+00001f00: 775f 696e 666f 5b27 6465 7363 7269 7074  w_info['descript
+00001f10: 696f 6e27 5d20 3d20 7572 6c6f 7065 6e28  ion'] = urlopen(
+00001f20: 6465 7363 7269 7074 696f 6e5f 7572 6c29  description_url)
+00001f30: 2e72 6561 6428 292e 6465 636f 6465 2827  .read().decode('
+00001f40: 7574 662d 3827 290a 2020 2020 2020 2020  utf-8').        
+00001f50: 6578 6365 7074 2048 5454 5045 7272 6f72  except HTTPError
+00001f60: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
+00001f70: 775f 696e 666f 5b27 6465 7363 7269 7074  w_info['descript
+00001f80: 696f 6e27 5d20 3d20 2255 6e61 626c 6520  ion'] = "Unable 
+00001f90: 746f 2067 6574 2064 6573 6372 6970 7469  to get descripti
+00001fa0: 6f6e 2066 6f72 207b 307d 2066 726f 6d20  on for {0} from 
+00001fb0: 3c61 2068 7265 663d 7b31 7d3e 7b31 7d3c  <a href={1}>{1}<
+00001fc0: 2f61 3e22 2e66 6f72 6d61 7428 7365 6c66  /a>".format(self
+00001fd0: 2e6e 616d 652c 2064 6573 6372 6970 7469  .name, descripti
+00001fe0: 6f6e 5f75 726c 290a 2020 2020 2020 2020  on_url).        
+00001ff0: 7365 6c66 2e6d 656e 755f 6c61 796f 7574  self.menu_layout
+00002000: 203d 206e 6577 5f69 6e66 6f2e 706f 7028   = new_info.pop(
+00002010: 276d 656e 755f 6c61 796f 7574 2729 0a20  'menu_layout'). 
+00002020: 2020 2020 2020 2069 6620 2764 6174 6527         if 'date'
+00002030: 2069 6e20 6e65 775f 696e 666f 3a0a 2020   in new_info:.  
+00002040: 2020 2020 2020 2020 2020 6e65 775f 696e            new_in
+00002050: 666f 5b27 7665 7273 696f 6e27 5d20 3d20  fo['version'] = 
+00002060: 272e 272e 6a6f 696e 286e 6577 5f69 6e66  '.'.join(new_inf
+00002070: 6f5b 2764 6174 6527 5d2e 7370 6c69 7428  o['date'].split(
+00002080: 272f 2729 5b32 3a5d 202b 206e 6577 5f69  '/')[2:] + new_i
+00002090: 6e66 6f5b 2764 6174 6527 5d2e 7370 6c69  nfo['date'].spli
+000020a0: 7428 272f 2729 5b3a 325d 290a 2020 2020  t('/')[:2]).    
+000020b0: 2020 2020 2020 2020 6e65 775f 696e 666f          new_info
+000020c0: 2e70 6f70 2827 6461 7465 2729 0a20 2020  .pop('date').   
+000020d0: 2020 2020 206e 6577 5f69 6e66 6f5b 276c       new_info['l
+000020e0: 6174 6573 745f 7665 7273 696f 6e27 5d20  atest_version'] 
+000020f0: 3d20 6e65 775f 696e 666f 2e70 6f70 2827  = new_info.pop('
+00002100: 7665 7273 696f 6e27 290a 2020 2020 2020  version').      
+00002110: 2020 6966 2027 6465 7065 6e64 656e 6369    if 'dependenci
+00002120: 6573 2720 696e 206e 6577 5f69 6e66 6f20  es' in new_info 
+00002130: 616e 6420 2764 6570 656e 6465 6e63 7927  and 'dependency'
+00002140: 2069 6e20 6e65 775f 696e 666f 5b27 6465   in new_info['de
+00002150: 7065 6e64 656e 6369 6573 275d 3a0a 2020  pendencies']:.  
+00002160: 2020 2020 2020 2020 2020 6465 7073 203d            deps =
+00002170: 206e 6577 5f69 6e66 6f2e 706f 7028 2764   new_info.pop('d
+00002180: 6570 656e 6465 6e63 6965 7327 295b 2764  ependencies')['d
+00002190: 6570 656e 6465 6e63 7927 5d0a 2020 2020  ependency'].    
+000021a0: 2020 2020 2020 2020 7365 6c66 2e64 6570          self.dep
+000021b0: 656e 6465 6e63 6965 7320 3d20 5b64 5b27  endencies = [d['
+000021c0: 406e 616d 6527 5d20 666f 7220 6420 696e  @name'] for d in
+000021d0: 2064 6570 735d 2069 6620 6973 696e 7374   deps] if isinst
+000021e0: 616e 6365 2864 6570 732c 206c 6973 7429  ance(deps, list)
+000021f0: 2065 6c73 6520 5b64 6570 735b 2740 6e61   else [deps['@na
+00002200: 6d65 275d 5d0a 2020 2020 2020 2020 7365  me']].        se
+00002210: 6c66 2e5f 5f64 6963 745f 5f2e 7570 6461  lf.__dict__.upda
+00002220: 7465 286e 6577 5f69 6e66 6f29 0a20 2020  te(new_info).   
+00002230: 2020 2020 2073 656c 662e 6c6f 6164 6564       self.loaded
+00002240: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+00002250: 0a0a 636c 6173 7320 506c 7567 696e 4d61  ..class PluginMa
+00002260: 6e61 6765 7228 5174 5769 6467 6574 732e  nager(QtWidgets.
+00002270: 514d 6169 6e57 696e 646f 7729 3a0a 2020  QMainWindow):.  
+00002280: 2020 706c 7567 696e 7320 3d20 7b7d 0a20    plugins = {}. 
+00002290: 2020 206c 6f61 6454 6872 6561 6420 3d20     loadThread = 
+000022a0: 4e6f 6e65 0a20 2020 2073 6967 506c 7567  None.    sigPlug
+000022b0: 696e 4c6f 6164 6564 203d 2051 7443 6f72  inLoaded = QtCor
+000022c0: 652e 5369 676e 616c 2873 7472 290a 2020  e.Signal(str).  
+000022d0: 2020 2727 270a 2020 2020 506c 7567 696e    '''.    Plugin
+000022e0: 4d61 6e61 6765 7220 6861 6e64 6c65 7320  Manager handles 
+000022f0: 696e 7374 616c 6c65 6420 706c 7567 696e  installed plugin
+00002300: 7320 616e 6420 7468 6520 6f6e 6c69 6e65  s and the online
+00002310: 2070 6c75 6769 6e20 6461 7461 6261 7365   plugin database
+00002320: 0a20 2020 207c 2073 686f 7728 2920 3a20  .    | show() : 
+00002330: 696e 6974 6961 6c69 7a65 7320 6120 6775  initializes a gu
+00002340: 6920 6173 2061 2073 7461 7469 6320 7661  i as a static va
+00002350: 7269 6162 6c65 206f 6620 7468 6520 636c  riable of the cl
+00002360: 6173 732c 2069 6620 6e65 6365 7373 6172  ass, if necessar
+00002370: 792c 2061 6e64 2064 6973 706c 6179 7320  y, and displays 
+00002380: 6974 2e20 4361 6c6c 2069 6e20 706c 6163  it. Call in plac
+00002390: 6520 6f66 2063 6f6e 7374 7275 6374 6f72  e of constructor
+000023a0: 0a20 2020 207c 2063 6c6f 7365 2829 203a  .    | close() :
+000023b0: 2063 6c6f 7365 7320 7468 6520 6775 6920   closes the gui 
+000023c0: 6966 2069 7420 6578 6973 7473 0a20 2020  if it exists.   
+000023d0: 2027 2727 0a20 2020 2040 7374 6174 6963   '''.    @static
+000023e0: 6d65 7468 6f64 0a20 2020 2064 6566 2073  method.    def s
+000023f0: 686f 7728 293a 0a20 2020 2020 2020 206c  how():.        l
+00002400: 6f67 6765 722e 6465 6275 6728 2743 616c  ogger.debug('Cal
+00002410: 6c69 6e67 2061 7070 2e70 6c75 6769 6e5f  ling app.plugin_
+00002420: 6d61 6e61 6765 722e 506c 7567 696e 4d61  manager.PluginMa
+00002430: 6e61 6765 722e 7368 6f77 2729 0a20 2020  nager.show').   
+00002440: 2020 2020 2069 6620 6e6f 7420 6861 7361       if not hasa
+00002450: 7474 7228 506c 7567 696e 4d61 6e61 6765  ttr(PluginManage
+00002460: 722c 2027 6775 6927 293a 0a20 2020 2020  r, 'gui'):.     
+00002470: 2020 2020 2020 2050 6c75 6769 6e4d 616e         PluginMan
+00002480: 6167 6572 2e67 7569 203d 2050 6c75 6769  ager.gui = Plugi
+00002490: 6e4d 616e 6167 6572 2829 0a20 2020 2020  nManager().     
+000024a0: 2020 2050 6c75 6769 6e4d 616e 6167 6572     PluginManager
+000024b0: 2e67 7569 2e73 686f 7750 6c75 6769 6e73  .gui.showPlugins
+000024c0: 2829 0a20 2020 2020 2020 2023 506c 7567  ().        #Plug
+000024d0: 696e 4d61 6e61 6765 722e 6c6f 6164 5f6f  inManager.load_o
+000024e0: 6e6c 696e 655f 706c 7567 696e 7328 290a  nline_plugins().
+000024f0: 2020 2020 2020 2020 5174 5769 6467 6574          QtWidget
+00002500: 732e 514d 6169 6e57 696e 646f 772e 7368  s.QMainWindow.sh
+00002510: 6f77 2850 6c75 6769 6e4d 616e 6167 6572  ow(PluginManager
+00002520: 2e67 7569 290a 2020 2020 2020 2020 6966  .gui).        if
+00002530: 206e 6f74 206f 732e 6163 6365 7373 2870   not os.access(p
+00002540: 6c75 6769 6e5f 6469 722c 206f 732e 575f  lugin_dir, os.W_
+00002550: 4f4b 293a 0a20 2020 2020 2020 2020 2020  OK):.           
+00002560: 2067 2e61 6c65 7274 2822 506c 7567 696e   g.alert("Plugin
+00002570: 2066 6f6c 6465 7220 7772 6974 6520 7065   folder write pe
+00002580: 726d 6973 7369 6f6e 2064 656e 6965 642e  rmission denied.
+00002590: 2052 6573 7461 7274 2066 6c69 6b61 2061   Restart flika a
+000025a0: 7320 6164 6d69 6e69 7374 7261 746f 7220  s administrator 
+000025b0: 746f 2065 6e61 626c 6520 706c 7567 696e  to enable plugin
+000025c0: 2069 6e73 7461 6c6c 6174 696f 6e2e 2229   installation.")
+000025d0: 0a0a 2020 2020 2020 2020 506c 7567 696e  ..        Plugin
+000025e0: 4d61 6e61 6765 722e 6775 692e 7368 6f77  Manager.gui.show
+000025f0: 4865 6c70 5363 7265 656e 2829 0a0a 0a20  HelpScreen()... 
+00002600: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00002610: 0a20 2020 2064 6566 2072 6566 7265 7368  .    def refresh
+00002620: 5f6f 6e6c 696e 655f 706c 7567 696e 7328  _online_plugins(
+00002630: 293a 0a20 2020 2020 2020 206c 6f67 6765  ):.        logge
+00002640: 722e 6465 6275 6728 2743 616c 6c69 6e67  r.debug('Calling
+00002650: 2061 7070 2e70 6c75 6769 6e5f 6d61 6e61   app.plugin_mana
+00002660: 6765 722e 506c 7567 696e 4d61 6e61 6765  ger.PluginManage
+00002670: 722e 7265 6672 6573 685f 6f6e 6c69 6e65  r.refresh_online
+00002680: 5f70 6c75 6769 6e73 2829 2729 0a20 2020  _plugins()').   
+00002690: 2020 2020 2066 6f72 2070 2069 6e20 706c       for p in pl
+000026a0: 7567 696e 5f6c 6973 742e 6b65 7973 2829  ugin_list.keys()
+000026b0: 3a0a 2020 2020 2020 2020 2020 2020 506c  :.            Pl
+000026c0: 7567 696e 4d61 6e61 6765 722e 6c6f 6164  uginManager.load
+000026d0: 5f6f 6e6c 696e 655f 706c 7567 696e 2870  _online_plugin(p
+000026e0: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
+000026f0: 7468 6f64 0a20 2020 2064 6566 206c 6f61  thod.    def loa
+00002700: 645f 6f6e 6c69 6e65 5f70 6c75 6769 6e28  d_online_plugin(
+00002710: 7029 3a0a 2020 2020 2020 2020 6c6f 6767  p):.        logg
+00002720: 6572 2e64 6562 7567 2827 4361 6c6c 696e  er.debug('Callin
+00002730: 6720 6170 702e 706c 7567 696e 5f6d 616e  g app.plugin_man
+00002740: 6167 6572 2e50 6c75 6769 6e4d 616e 6167  ager.PluginManag
+00002750: 6572 2e6c 6f61 645f 6f6e 6c69 6e65 5f70  er.load_online_p
+00002760: 6c75 6769 6e28 2927 290a 2020 2020 2020  lugin()').      
+00002770: 2020 6966 2070 206e 6f74 2069 6e20 706c    if p not in pl
+00002780: 7567 696e 5f6c 6973 7420 6f72 2050 6c75  ugin_list or Plu
+00002790: 6769 6e4d 616e 6167 6572 2e6c 6f61 6454  ginManager.loadT
 000027a0: 6872 6561 6420 6973 206e 6f74 204e 6f6e  hread is not Non
-000027b0: 6520 616e 6420 7365 6c66 2e6c 6f61 6454  e and self.loadT
-000027c0: 6872 6561 642e 6973 5f61 6c69 7665 2829  hread.is_alive()
-000027d0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000027e0: 656c 662e 6c6f 6164 5468 7265 6164 2e6a  elf.loadThread.j
-000027f0: 6f69 6e28 3029 0d0a 0d0a 2020 2020 4073  oin(0)....    @s
-00002800: 7461 7469 636d 6574 686f 640d 0a20 2020  taticmethod..   
-00002810: 2064 6566 2063 6c6f 7365 2829 3a0d 0a20   def close():.. 
-00002820: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
-00002830: 7228 506c 7567 696e 4d61 6e61 6765 722c  r(PluginManager,
-00002840: 2027 6775 6927 293a 0d0a 2020 2020 2020   'gui'):..      
-00002850: 2020 2020 2020 5174 5769 6467 6574 732e        QtWidgets.
-00002860: 514d 6169 6e57 696e 646f 772e 636c 6f73  QMainWindow.clos
-00002870: 6528 506c 7567 696e 4d61 6e61 6765 722e  e(PluginManager.
-00002880: 6775 6929 0d0a 0d0a 2020 2020 6465 6620  gui)....    def 
-00002890: 5f5f 696e 6974 5f5f 2873 656c 6629 3a0d  __init__(self):.
-000028a0: 0a20 2020 2020 2020 2073 7570 6572 2850  .        super(P
-000028b0: 6c75 6769 6e4d 616e 6167 6572 2c73 656c  luginManager,sel
-000028c0: 6629 2e5f 5f69 6e69 745f 5f28 290d 0a20  f).__init__().. 
-000028d0: 2020 2020 2020 206c 6f61 645f 7569 2822         load_ui("
-000028e0: 706c 7567 696e 5f6d 616e 6167 6572 2e75  plugin_manager.u
-000028f0: 6922 2c20 7365 6c66 2c20 6469 7265 6374  i", self, direct
-00002900: 6f72 793d 6f73 2e70 6174 682e 6469 726e  ory=os.path.dirn
-00002910: 616d 6528 5f5f 6669 6c65 5f5f 2929 0d0a  ame(__file__))..
-00002920: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00002930: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00002940: 6372 6f6c 6c41 7265 6157 6964 6765 7443  crollAreaWidgetC
-00002950: 6f6e 7465 6e74 732e 7365 7443 6f6e 7465  ontents.setConte
-00002960: 6e74 734d 6172 6769 6e73 2831 302c 2031  ntsMargins(10, 1
-00002970: 302c 2031 302c 2031 3029 0d0a 2020 2020  0, 10, 10)..    
-00002980: 2020 2020 6578 6365 7074 3a0d 0a20 2020      except:..   
-00002990: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
-000029a0: 2020 2020 2020 2023 7365 6c66 2e70 6c75         #self.plu
-000029b0: 6769 6e4c 6973 742e 6974 656d 436c 6963  ginList.itemClic
-000029c0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-000029d0: 2e70 6c75 6769 6e53 656c 6563 7465 6429  .pluginSelected)
-000029e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-000029f0: 7574 6f72 6961 6c42 7574 746f 6e2e 636c  utorialButton.cl
-00002a00: 6963 6b65 642e 636f 6e6e 6563 7428 6c61  icked.connect(la
-00002a10: 6d62 6461 203a 2051 7447 7569 2e51 4465  mbda : QtGui.QDe
-00002a20: 736b 746f 7053 6572 7669 6365 732e 6f70  sktopServices.op
-00002a30: 656e 5572 6c28 5174 436f 7265 2e51 5572  enUrl(QtCore.QUr
-00002a40: 6c28 2268 7474 7073 3a2f 2f67 6974 6875  l("https://githu
-00002a50: 622e 636f 6d2f 666c 696b 612d 6f72 672f  b.com/flika-org/
-00002a60: 666c 696b 615f 706c 7567 696e 5f74 656d  flika_plugin_tem
-00002a70: 706c 6174 6522 2929 290d 0a20 2020 2020  plate")))..     
-00002a80: 2020 2073 656c 662e 646f 776e 6c6f 6164     self.download
-00002a90: 4275 7474 6f6e 2e63 6c69 636b 6564 2e63  Button.clicked.c
-00002aa0: 6f6e 6e65 6374 2873 656c 662e 646f 776e  onnect(self.down
-00002ab0: 6c6f 6164 436c 6963 6b65 6429 0d0a 2020  loadClicked)..  
-00002ac0: 2020 2020 2020 7365 6c66 2e70 6c75 6769        self.plugi
-00002ad0: 6e4c 6973 742e 6375 7272 656e 7449 7465  nList.currentIte
-00002ae0: 6d43 6861 6e67 6564 2e63 6f6e 6e65 6374  mChanged.connect
-00002af0: 286c 616d 6264 6120 6e65 772c 206f 6c64  (lambda new, old
-00002b00: 3a20 7365 6c66 2e70 6c75 6769 6e53 656c  : self.pluginSel
-00002b10: 6563 7465 6428 6e65 7729 290d 0a20 2020  ected(new))..   
-00002b20: 2020 2020 2073 656c 662e 646f 6375 6d65       self.docume
-00002b30: 6e74 6174 696f 6e42 7574 746f 6e2e 636c  ntationButton.cl
-00002b40: 6963 6b65 642e 636f 6e6e 6563 7428 7365  icked.connect(se
-00002b50: 6c66 2e64 6f63 756d 656e 7461 7469 6f6e  lf.documentation
-00002b60: 436c 6963 6b65 6429 0d0a 2020 2020 2020  Clicked)..      
-00002b70: 2020 7365 6c66 2e75 7064 6174 6542 7574    self.updateBut
-00002b80: 746f 6e2e 636c 6963 6b65 642e 636f 6e6e  ton.clicked.conn
-00002b90: 6563 7428 7365 6c66 2e75 7064 6174 6543  ect(self.updateC
-00002ba0: 6c69 636b 6564 290d 0a20 2020 2020 2020  licked)..       
-00002bb0: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-00002bc0: 7365 6172 6368 426f 782e 7465 7874 4368  searchBox.textCh
-00002bd0: 616e 6765 642e 636f 6e6e 6563 7428 7365  anged.connect(se
-00002be0: 6c66 2e73 686f 7750 6c75 6769 6e73 290d  lf.showPlugins).
-00002bf0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00002c00: 6172 6368 4275 7474 6f6e 2e63 6c69 636b  archButton.click
-00002c10: 6564 2e63 6f6e 6e65 6374 286c 616d 6264  ed.connect(lambd
-00002c20: 6120 663a 2073 656c 662e 7368 6f77 506c  a f: self.showPl
-00002c30: 7567 696e 7328 7365 6172 6368 5f73 7472  ugins(search_str
-00002c40: 3d73 7472 2873 656c 662e 7365 6172 6368  =str(self.search
-00002c50: 426f 782e 7465 7874 2829 2929 290d 0a20  Box.text()))).. 
-00002c60: 2020 2020 2020 2073 656c 662e 6465 7363         self.desc
-00002c70: 7269 7074 696f 6e4c 6162 656c 2e73 6574  riptionLabel.set
-00002c80: 4f70 656e 4578 7465 726e 616c 4c69 6e6b  OpenExternalLink
-00002c90: 7328 5472 7565 290d 0a20 2020 2020 2020  s(True)..       
-00002ca0: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-00002cb0: 7265 6672 6573 6842 7574 746f 6e2e 7072  refreshButton.pr
-00002cc0: 6573 7365 642e 636f 6e6e 6563 7428 7365  essed.connect(se
-00002cd0: 6c66 2e72 6566 7265 7368 5f6f 6e6c 696e  lf.refresh_onlin
-00002ce0: 655f 706c 7567 696e 7329 0d0a 2020 2020  e_plugins)..    
-00002cf0: 2020 2020 6465 6620 7570 6461 7465 506c      def updatePl
-00002d00: 7567 696e 2861 293a 0d0a 2020 2020 2020  ugin(a):..      
-00002d10: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00002d20: 7342 6172 2e73 686f 774d 6573 7361 6765  sBar.showMessage
-00002d30: 2822 4669 6e69 7368 6564 206c 6f61 6469  ("Finished loadi
-00002d40: 6e67 207b 7d22 2e66 6f72 6d61 7428 6129  ng {}".format(a)
-00002d50: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00002d60: 6620 506c 7567 696e 4d61 6e61 6765 722e  f PluginManager.
-00002d70: 706c 7567 696e 735b 615d 2e6c 6973 7457  plugins[a].listW
-00002d80: 6964 6765 742e 6973 5365 6c65 6374 6564  idget.isSelected
-00002d90: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00002da0: 2020 2020 2050 6c75 6769 6e4d 616e 6167       PluginManag
-00002db0: 6572 2e67 7569 2e70 6c75 6769 6e53 656c  er.gui.pluginSel
-00002dc0: 6563 7465 6428 6129 0d0a 2020 2020 2020  ected(a)..      
-00002dd0: 2020 2020 2020 2365 6c73 653a 0d0a 2020        #else:..  
-00002de0: 2020 2020 2020 2020 2020 2020 2020 2373                #s
-00002df0: 656c 662e 7368 6f77 506c 7567 696e 7328  elf.showPlugins(
-00002e00: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00002e10: 7369 6750 6c75 6769 6e4c 6f61 6465 642e  sigPluginLoaded.
-00002e20: 636f 6e6e 6563 7428 7570 6461 7465 506c  connect(updatePl
-00002e30: 7567 696e 290d 0a0d 0a20 2020 2020 2020  ugin)....       
-00002e40: 2073 656c 662e 7365 7457 696e 646f 7754   self.setWindowT
-00002e50: 6974 6c65 2827 506c 7567 696e 204d 616e  itle('Plugin Man
-00002e60: 6167 6572 2729 0d0a 2020 2020 2020 2020  ager')..        
-00002e70: 7365 6c66 2e73 686f 7750 6c75 6769 6e73  self.showPlugins
-00002e80: 2829 0d0a 0d0a 2020 2020 6465 6620 7368  ()....    def sh
-00002e90: 6f77 4865 6c70 5363 7265 656e 2873 656c  owHelpScreen(sel
-00002ea0: 6629 3a0d 0a20 2020 2020 2020 2073 656c  f):..        sel
-00002eb0: 662e 706c 7567 696e 4c61 6265 6c2e 7365  f.pluginLabel.se
-00002ec0: 7454 6578 7428 2222 290d 0a20 2020 2020  tText("")..     
-00002ed0: 2020 2073 656c 662e 6465 7363 7269 7074     self.descript
-00002ee0: 696f 6e4c 6162 656c 2e73 6574 4874 6d6c  ionLabel.setHtml
-00002ef0: 2868 656c 7048 544d 4c29 0d0a 2020 2020  (helpHTML)..    
-00002f00: 2020 2020 7365 6c66 2e64 6f77 6e6c 6f61      self.downloa
-00002f10: 6442 7574 746f 6e2e 7365 7456 6973 6962  dButton.setVisib
-00002f20: 6c65 2846 616c 7365 290d 0a20 2020 2020  le(False)..     
-00002f30: 2020 2073 656c 662e 646f 6375 6d65 6e74     self.document
-00002f40: 6174 696f 6e42 7574 746f 6e2e 7365 7456  ationButton.setV
-00002f50: 6973 6962 6c65 2846 616c 7365 290d 0a20  isible(False).. 
-00002f60: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
-00002f70: 7465 4275 7474 6f6e 2e73 6574 5669 7369  teButton.setVisi
-00002f80: 626c 6528 4661 6c73 6529 0d0a 2020 2020  ble(False)..    
-00002f90: 2020 2020 7365 6c66 2e69 6e66 6f4c 6162      self.infoLab
-00002fa0: 656c 2e73 6574 5465 7874 2822 2229 0d0a  el.setText("")..
-00002fb0: 0d0a 2020 2020 6465 6620 646f 776e 6c6f  ..    def downlo
-00002fc0: 6164 436c 6963 6b65 6428 7365 6c66 293a  adClicked(self):
-00002fd0: 0d0a 2020 2020 2020 2020 7020 3d20 7374  ..        p = st
-00002fe0: 7228 7365 6c66 2e70 6c75 6769 6e4c 6973  r(self.pluginLis
-00002ff0: 742e 6375 7272 656e 7449 7465 6d28 292e  t.currentItem().
-00003000: 7465 7874 2829 290d 0a20 2020 2020 2020  text())..       
-00003010: 2070 6c75 6769 6e20 3d20 7365 6c66 2e70   plugin = self.p
-00003020: 6c75 6769 6e73 5b70 5d0d 0a20 2020 2020  lugins[p]..     
-00003030: 2020 2069 6620 7365 6c66 2e64 6f77 6e6c     if self.downl
-00003040: 6f61 6442 7574 746f 6e2e 7465 7874 2829  oadButton.text()
-00003050: 203d 3d20 2749 6e73 7461 6c6c 273a 0d0a   == 'Install':..
-00003060: 2020 2020 2020 2020 2020 2020 506c 7567              Plug
-00003070: 696e 4d61 6e61 6765 722e 646f 776e 6c6f  inManager.downlo
-00003080: 6164 506c 7567 696e 2870 6c75 6769 6e29  adPlugin(plugin)
-00003090: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-000030a0: 0a20 2020 2020 2020 2020 2020 2050 6c75  .            Plu
-000030b0: 6769 6e4d 616e 6167 6572 2e72 656d 6f76  ginManager.remov
-000030c0: 6550 6c75 6769 6e28 706c 7567 696e 290d  ePlugin(plugin).
-000030d0: 0a0d 0a20 2020 2064 6566 2064 6f63 756d  ...    def docum
-000030e0: 656e 7461 7469 6f6e 436c 6963 6b65 6428  entationClicked(
-000030f0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00003100: 7020 3d20 7374 7228 7365 6c66 2e70 6c75  p = str(self.plu
-00003110: 6769 6e4c 6973 742e 6375 7272 656e 7449  ginList.currentI
-00003120: 7465 6d28 292e 7465 7874 2829 290d 0a20  tem().text()).. 
-00003130: 2020 2020 2020 2070 6c75 6769 6e20 3d20         plugin = 
-00003140: 7365 6c66 2e70 6c75 6769 6e73 5b70 5d0d  self.plugins[p].
-00003150: 0a20 2020 2020 2020 2069 6620 6861 7361  .        if hasa
-00003160: 7474 7228 706c 7567 696e 2c20 2264 6f63  ttr(plugin, "doc
-00003170: 756d 656e 7461 7469 6f6e 2229 3a0d 0a20  umentation"):.. 
-00003180: 2020 2020 2020 2020 2020 2051 7447 7569             QtGui
-00003190: 2e51 4465 736b 746f 7053 6572 7669 6365  .QDesktopService
-000031a0: 732e 6f70 656e 5572 6c28 5174 436f 7265  s.openUrl(QtCore
-000031b0: 2e51 5572 6c28 706c 7567 696e 2e64 6f63  .QUrl(plugin.doc
-000031c0: 756d 656e 7461 7469 6f6e 2929 0d0a 0d0a  umentation))....
-000031d0: 2020 2020 6465 6620 7570 6461 7465 436c      def updateCl
-000031e0: 6963 6b65 6428 7365 6c66 293a 0d0a 2020  icked(self):..  
-000031f0: 2020 2020 2020 7020 3d20 7374 7228 7365        p = str(se
-00003200: 6c66 2e70 6c75 6769 6e4c 6973 742e 6375  lf.pluginList.cu
-00003210: 7272 656e 7449 7465 6d28 292e 7465 7874  rrentItem().text
-00003220: 2829 290d 0a20 2020 2020 2020 2070 6c75  ())..        plu
-00003230: 6769 6e20 3d20 7365 6c66 2e70 6c75 6769  gin = self.plugi
-00003240: 6e73 5b70 5d0d 0a20 2020 2020 2020 2050  ns[p]..        P
-00003250: 6c75 6769 6e4d 616e 6167 6572 2e72 656d  luginManager.rem
-00003260: 6f76 6550 6c75 6769 6e28 706c 7567 696e  ovePlugin(plugin
-00003270: 290d 0a20 2020 2020 2020 2050 6c75 6769  )..        Plugi
-00003280: 6e4d 616e 6167 6572 2e64 6f77 6e6c 6f61  nManager.downloa
-00003290: 6450 6c75 6769 6e28 706c 7567 696e 290d  dPlugin(plugin).
-000032a0: 0a0d 0a20 2020 2064 6566 2070 6c75 6769  ...    def plugi
-000032b0: 6e53 656c 6563 7465 6428 7365 6c66 2c20  nSelected(self, 
-000032c0: 6974 656d 293a 0d0a 2020 2020 2020 2020  item):..        
-000032d0: 6966 2069 7465 6d20 6973 204e 6f6e 653a  if item is None:
-000032e0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000032f0: 2073 656c 662e 706c 7567 696e 4c61 6265   self.pluginLabe
-00003300: 6c2e 7465 7874 2829 3a0d 0a20 2020 2020  l.text():..     
-00003310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003320: 706c 7567 696e 5365 6c65 6374 6564 2850  pluginSelected(P
-00003330: 6c75 6769 6e4d 616e 6167 6572 2e70 6c75  luginManager.plu
-00003340: 6769 6e73 5b73 656c 662e 706c 7567 696e  gins[self.plugin
-00003350: 4c61 6265 6c2e 7465 7874 2829 5d2e 6c69  Label.text()].li
-00003360: 7374 5769 6467 6574 290d 0a20 2020 2020  stWidget)..     
-00003370: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
-00003380: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00003390: 616e 6365 2869 7465 6d2c 2073 7472 293a  ance(item, str):
-000033a0: 0d0a 2020 2020 2020 2020 2020 2020 7320  ..            s 
-000033b0: 3d20 6974 656d 0d0a 2020 2020 2020 2020  = item..        
-000033c0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000033d0: 2020 2073 203d 2073 7472 2869 7465 6d2e     s = str(item.
-000033e0: 7465 7874 2829 290d 0a20 2020 2020 2020  text())..       
-000033f0: 2070 6c75 6769 6e20 3d20 7365 6c66 2e70   plugin = self.p
-00003400: 6c75 6769 6e73 5b73 5d0d 0a20 2020 2020  lugins[s]..     
-00003410: 2020 2073 656c 662e 706c 7567 696e 4c61     self.pluginLa
-00003420: 6265 6c2e 7365 7454 6578 7428 7329 0d0a  bel.setText(s)..
-00003430: 2020 2020 2020 2020 6966 206e 6f74 2070          if not p
-00003440: 6c75 6769 6e2e 6c6f 6164 6564 3a0d 0a20  lugin.loaded:.. 
-00003450: 2020 2020 2020 2020 2020 2069 6e66 6f20             info 
-00003460: 3d20 224c 6f61 6469 6e67 2069 6e66 6f72  = "Loading infor
-00003470: 6d61 7469 6f6e 220d 0a20 2020 2020 2020  mation"..       
-00003480: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00003490: 2020 2020 696e 666f 203d 2027 4279 207b      info = 'By {
-000034a0: 7d2c 204c 6174 6573 743a 207b 7d27 2e66  }, Latest: {}'.f
-000034b0: 6f72 6d61 7428 706c 7567 696e 2e61 7574  ormat(plugin.aut
-000034c0: 686f 722c 2070 6c75 6769 6e2e 6c61 7465  hor, plugin.late
-000034d0: 7374 5f76 6572 7369 6f6e 290d 0a20 2020  st_version)..   
-000034e0: 2020 2020 2020 2020 2073 656c 662e 646f           self.do
-000034f0: 776e 6c6f 6164 4275 7474 6f6e 2e73 6574  wnloadButton.set
-00003500: 5669 7369 626c 6528 5472 7565 290d 0a20  Visible(True).. 
-00003510: 2020 2020 2020 2076 6572 7369 6f6e 203d         version =
-00003520: 2070 6172 7365 5f76 6572 7369 6f6e 2870   parse_version(p
-00003530: 6c75 6769 6e2e 7665 7273 696f 6e29 0d0a  lugin.version)..
-00003540: 2020 2020 2020 2020 6c61 7465 7374 5f76          latest_v
-00003550: 6572 7369 6f6e 203d 2070 6172 7365 5f76  ersion = parse_v
-00003560: 6572 7369 6f6e 2870 6c75 6769 6e2e 6c61  ersion(plugin.la
-00003570: 7465 7374 5f76 6572 7369 6f6e 290d 0a20  test_version).. 
-00003580: 2020 2020 2020 2069 6620 706c 7567 696e         if plugin
-00003590: 2e76 6572 7369 6f6e 2061 6e64 2076 6572  .version and ver
-000035a0: 7369 6f6e 203c 206c 6174 6573 745f 7665  sion < latest_ve
-000035b0: 7273 696f 6e3a 0d0a 2020 2020 2020 2020  rsion:..        
-000035c0: 2020 2020 696e 666f 202b 3d20 223b 203c      info += "; <
-000035d0: 623e 5570 6461 7465 2041 7661 696c 6162  b>Update Availab
-000035e0: 6c65 213c 2f62 3e22 0d0a 0d0a 2020 2020  le!</b>"....    
-000035f0: 2020 2020 7365 6c66 2e75 7064 6174 6542      self.updateB
-00003600: 7574 746f 6e2e 7365 7456 6973 6962 6c65  utton.setVisible
-00003610: 2870 6c75 6769 6e2e 7665 7273 696f 6e20  (plugin.version 
-00003620: 213d 2027 2720 616e 6420 7665 7273 696f  != '' and versio
-00003630: 6e20 3c20 6c61 7465 7374 5f76 6572 7369  n < latest_versi
-00003640: 6f6e 290d 0a20 2020 2020 2020 2073 656c  on)..        sel
-00003650: 662e 646f 776e 6c6f 6164 4275 7474 6f6e  f.downloadButton
-00003660: 2e73 6574 5465 7874 2822 496e 7374 616c  .setText("Instal
-00003670: 6c22 2069 6620 706c 7567 696e 2e76 6572  l" if plugin.ver
-00003680: 7369 6f6e 203d 3d20 2727 2065 6c73 6520  sion == '' else 
-00003690: 2755 6e69 6e73 7461 6c6c 2729 0d0a 2020  'Uninstall')..  
-000036a0: 2020 2020 2020 7365 6c66 2e64 6f63 756d        self.docum
-000036b0: 656e 7461 7469 6f6e 4275 7474 6f6e 2e73  entationButton.s
-000036c0: 6574 5669 7369 626c 6528 706c 7567 696e  etVisible(plugin
-000036d0: 2e64 6f63 756d 656e 7461 7469 6f6e 2021  .documentation !
-000036e0: 3d20 4e6f 6e65 290d 0a0d 0a20 2020 2020  = None)....     
-000036f0: 2020 2073 656c 662e 696e 666f 4c61 6265     self.infoLabe
-00003700: 6c2e 7365 7454 6578 7428 696e 666f 290d  l.setText(info).
-00003710: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
-00003720: 7363 7269 7074 696f 6e4c 6162 656c 2e73  scriptionLabel.s
-00003730: 6574 4874 6d6c 2870 6c75 6769 6e2e 6465  etHtml(plugin.de
-00003740: 7363 7269 7074 696f 6e29 0d0a 2020 2020  scription)..    
-00003750: 2020 2020 6966 2070 6c75 6769 6e2e 696e      if plugin.in
-00003760: 666f 5f75 726c 203d 3d20 4e6f 6e65 3a0d  fo_url == None:.
-00003770: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003780: 662e 6c6f 6164 5f6f 6e6c 696e 655f 706c  f.load_online_pl
-00003790: 7567 696e 2870 6c75 6769 6e2e 6e61 6d65  ugin(plugin.name
-000037a0: 290d 0a0d 0a20 2020 2040 7374 6174 6963  )....    @static
-000037b0: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
-000037c0: 6c6f 6361 6c5f 706c 7567 696e 5f70 6174  local_plugin_pat
-000037d0: 6873 2829 3a0d 0a20 2020 2020 2020 2070  hs():..        p
-000037e0: 6174 6873 203d 205b 5d0d 0a20 2020 2020  aths = []..     
-000037f0: 2020 2066 6f72 2070 6174 6820 696e 2067     for path in g
-00003800: 6c6f 6228 6f73 2e70 6174 682e 6a6f 696e  lob(os.path.join
-00003810: 2867 6574 5f70 6c75 6769 6e5f 6469 7265  (get_plugin_dire
-00003820: 6374 6f72 7928 292c 2022 2a22 2929 3a0d  ctory(), "*")):.
-00003830: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003840: 6f73 2e70 6174 682e 6973 6469 7228 7061  os.path.isdir(pa
-00003850: 7468 2920 616e 6420 6f73 2e70 6174 682e  th) and os.path.
-00003860: 6578 6973 7473 286f 732e 7061 7468 2e6a  exists(os.path.j
-00003870: 6f69 6e28 7061 7468 2c20 2769 6e66 6f2e  oin(path, 'info.
-00003880: 786d 6c27 2929 3a0d 0a20 2020 2020 2020  xml')):..       
-00003890: 2020 2020 2020 2020 2070 6174 6873 2e61           paths.a
-000038a0: 7070 656e 6428 7061 7468 290d 0a20 2020  ppend(path)..   
-000038b0: 2020 2020 2072 6574 7572 6e20 7061 7468       return path
-000038c0: 730d 0a0d 0a20 2020 2064 6566 2063 6c65  s....    def cle
-000038d0: 6172 4c69 7374 2873 656c 6629 3a0d 0a20  arList(self):.. 
-000038e0: 2020 2020 2020 2077 6869 6c65 2073 656c         while sel
-000038f0: 662e 706c 7567 696e 4c69 7374 2e63 6f75  f.pluginList.cou
-00003900: 6e74 2829 203e 2030 3a0d 0a20 2020 2020  nt() > 0:..     
-00003910: 2020 2020 2020 2073 656c 662e 706c 7567         self.plug
-00003920: 696e 4c69 7374 2e74 616b 6549 7465 6d28  inList.takeItem(
-00003930: 3029 0d0a 0d0a 2020 2020 6465 6620 7368  0)....    def sh
-00003940: 6f77 506c 7567 696e 7328 7365 6c66 2c20  owPlugins(self, 
-00003950: 7365 6172 6368 5f73 7472 3d4e 6f6e 6529  search_str=None)
-00003960: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-00003970: 636c 6561 724c 6973 7428 290d 0a20 2020  clearList()..   
-00003980: 2020 2020 2069 6620 7365 6172 6368 5f73       if search_s
-00003990: 7472 203d 3d20 4e6f 6e65 206f 7220 6c65  tr == None or le
-000039a0: 6e28 7365 6172 6368 5f73 7472 2920 3d3d  n(search_str) ==
-000039b0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-000039c0: 206e 616d 6573 203d 2073 6f72 7465 6428   names = sorted(
-000039d0: 7365 6c66 2e70 6c75 6769 6e73 2e6b 6579  self.plugins.key
-000039e0: 7328 2929 0d0a 2020 2020 2020 2020 656c  s())..        el
-000039f0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00003a00: 2064 6566 2073 6f72 745f 6675 6e63 286e   def sort_func(n
-00003a10: 616d 6529 3a0d 0a20 2020 2020 2020 2020  ame):..         
-00003a20: 2020 2020 2020 206e 616d 6520 3d20 7374         name = st
-00003a30: 7228 6e61 6d65 290d 0a20 2020 2020 2020  r(name)..       
-00003a40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00003a50: 2d64 6966 666c 6962 2e53 6571 7565 6e63  -difflib.Sequenc
-00003a60: 654d 6174 6368 6572 284e 6f6e 652c 206e  eMatcher(None, n
-00003a70: 616d 652e 6c6f 7765 7228 292c 2073 6561  ame.lower(), sea
-00003a80: 7263 685f 7374 722e 6c6f 7765 7228 2929  rch_str.lower())
-00003a90: 2e72 6174 696f 2829 202d 2069 6e74 2873  .ratio() - int(s
-00003aa0: 6561 7263 685f 7374 722e 6c6f 7765 7228  earch_str.lower(
-00003ab0: 2920 696e 206e 616d 652e 6c6f 7765 7228  ) in name.lower(
-00003ac0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00003ad0: 6420 3d20 7b6e 616d 653a 2073 6f72 745f  d = {name: sort_
-00003ae0: 6675 6e63 286e 616d 6529 2066 6f72 206e  func(name) for n
-00003af0: 616d 6520 696e 2073 656c 662e 706c 7567  ame in self.plug
-00003b00: 696e 732e 6b65 7973 2829 2069 6620 736f  ins.keys() if so
-00003b10: 7274 5f66 756e 6328 6e61 6d65 2920 213d  rt_func(name) !=
-00003b20: 2030 7d0d 0a20 2020 2020 2020 2020 2020   0}..           
-00003b30: 206e 616d 6573 203d 2073 6f72 7465 6428   names = sorted(
-00003b40: 642e 6b65 7973 2829 2c20 6b65 793d 6c61  d.keys(), key=la
-00003b50: 6d62 6461 2061 3a20 645b 615d 290d 0a20  mbda a: d[a]).. 
-00003b60: 2020 2020 2020 2066 6f72 206e 616d 6520         for name 
-00003b70: 696e 206e 616d 6573 3a0d 0a20 2020 2020  in names:..     
-00003b80: 2020 2020 2020 2070 6c75 6720 3d20 506c         plug = Pl
-00003b90: 7567 696e 4d61 6e61 6765 722e 706c 7567  uginManager.plug
-00003ba0: 696e 735b 6e61 6d65 5d0d 0a20 2020 2020  ins[name]..     
-00003bb0: 2020 2020 2020 2069 6620 706c 7567 2e76         if plug.v
-00003bc0: 6572 7369 6f6e 203d 3d20 2727 3a0d 0a20  ersion == '':.. 
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00003be0: 6c75 672e 6c69 7374 5769 6467 6574 2e73  lug.listWidget.s
-00003bf0: 6574 4963 6f6e 2851 7447 7569 2e51 4963  etIcon(QtGui.QIc
-00003c00: 6f6e 2829 290d 0a20 2020 2020 2020 2020  on())..         
-00003c10: 2020 2065 6c69 6620 7061 7273 655f 7665     elif parse_ve
-00003c20: 7273 696f 6e28 706c 7567 2e76 6572 7369  rsion(plug.versi
-00003c30: 6f6e 2920 3c20 7061 7273 655f 7665 7273  on) < parse_vers
-00003c40: 696f 6e28 706c 7567 2e6c 6174 6573 745f  ion(plug.latest_
-00003c50: 7665 7273 696f 6e29 3a0d 0a20 2020 2020  version):..     
-00003c60: 2020 2020 2020 2020 2020 2070 6c75 672e             plug.
-00003c70: 6c69 7374 5769 6467 6574 2e73 6574 4963  listWidget.setIc
-00003c80: 6f6e 2851 7447 7569 2e51 4963 6f6e 2869  on(QtGui.QIcon(i
-00003c90: 6d61 6765 5f70 6174 6828 2765 7863 6c61  mage_path('excla
-00003ca0: 6d61 7469 6f6e 2e70 6e67 2729 2929 0d0a  mation.png')))..
-00003cb0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00003cc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003cd0: 2020 2070 6c75 672e 6c69 7374 5769 6467     plug.listWidg
-00003ce0: 6574 2e73 6574 4963 6f6e 2851 7447 7569  et.setIcon(QtGui
-00003cf0: 2e51 4963 6f6e 2869 6d61 6765 5f70 6174  .QIcon(image_pat
-00003d00: 6828 2763 6865 636b 2e70 6e67 2729 2929  h('check.png')))
-00003d10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00003d20: 6c66 2e70 6c75 6769 6e4c 6973 742e 6164  lf.pluginList.ad
-00003d30: 6449 7465 6d28 706c 7567 2e6c 6973 7457  dItem(plug.listW
-00003d40: 6964 6765 7429 0d0a 0d0a 2020 2020 4073  idget)....    @s
-00003d50: 7461 7469 636d 6574 686f 640d 0a20 2020  taticmethod..   
-00003d60: 2064 6566 2072 656d 6f76 6550 6c75 6769   def removePlugi
-00003d70: 6e28 706c 7567 696e 293a 0d0a 2020 2020  n(plugin):..    
-00003d80: 2020 2020 506c 7567 696e 4d61 6e61 6765      PluginManage
-00003d90: 722e 6775 692e 7374 6174 7573 4261 722e  r.gui.statusBar.
-00003da0: 7368 6f77 4d65 7373 6167 6528 2255 6e69  showMessage("Uni
-00003db0: 6e73 7461 6c6c 696e 6720 7b7d 222e 666f  nstalling {}".fo
-00003dc0: 726d 6174 2870 6c75 6769 6e2e 6e61 6d65  rmat(plugin.name
-00003dd0: 2929 0d0a 2020 2020 2020 2020 6966 206f  ))..        if o
-00003de0: 732e 7061 7468 2e69 7364 6972 286f 732e  s.path.isdir(os.
-00003df0: 7061 7468 2e6a 6f69 6e28 6765 745f 706c  path.join(get_pl
-00003e00: 7567 696e 5f64 6972 6563 746f 7279 2829  ugin_directory()
-00003e10: 2c20 706c 7567 696e 2e64 6972 6563 746f  , plugin.directo
-00003e20: 7279 2c20 272e 6769 7427 2929 3a0d 0a20  ry, '.git')):.. 
-00003e30: 2020 2020 2020 2020 2020 2067 2e61 6c65             g.ale
-00003e40: 7274 2822 5468 6973 2070 6c75 6769 6e27  rt("This plugin'
-00003e50: 7320 6469 7265 6374 6f72 7920 6973 206d  s directory is m
-00003e60: 616e 6167 6564 2062 7920 6769 742e 2054  anaged by git. T
-00003e70: 6f20 7265 6d6f 7665 2c20 6d61 6e75 616c  o remove, manual
-00003e80: 6c79 2064 656c 6574 6520 7468 6520 6469  ly delete the di
-00003e90: 7265 6374 6f72 7922 290d 0a20 2020 2020  rectory")..     
-00003ea0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00003eb0: 6c73 650d 0a20 2020 2020 2020 2074 7279  lse..        try
-00003ec0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00003ed0: 6875 7469 6c2e 726d 7472 6565 286f 732e  hutil.rmtree(os.
-00003ee0: 7061 7468 2e6a 6f69 6e28 6765 745f 706c  path.join(get_pl
-00003ef0: 7567 696e 5f64 6972 6563 746f 7279 2829  ugin_directory()
-00003f00: 2c20 706c 7567 696e 2e64 6972 6563 746f  , plugin.directo
-00003f10: 7279 292c 2069 676e 6f72 655f 6572 726f  ry), ignore_erro
-00003f20: 7273 3d54 7275 6529 0d0a 2020 2020 2020  rs=True)..      
-00003f30: 2020 2020 2020 706c 7567 696e 2e76 6572        plugin.ver
-00003f40: 7369 6f6e 203d 2027 270d 0a20 2020 2020  sion = ''..     
-00003f50: 2020 2020 2020 2070 6c75 6769 6e2e 6d65         plugin.me
-00003f60: 6e75 203d 204e 6f6e 650d 0a20 2020 2020  nu = None..     
-00003f70: 2020 2020 2020 2070 6c75 6769 6e2e 6c69         plugin.li
-00003f80: 7374 5769 6467 6574 2e73 6574 4963 6f6e  stWidget.setIcon
-00003f90: 2851 7447 7569 2e51 4963 6f6e 2829 290d  (QtGui.QIcon()).
-00003fa0: 0a20 2020 2020 2020 2020 2020 2050 6c75  .            Plu
-00003fb0: 6769 6e4d 616e 6167 6572 2e67 7569 2e73  ginManager.gui.s
-00003fc0: 7461 7475 7342 6172 2e73 686f 774d 6573  tatusBar.showMes
-00003fd0: 7361 6765 2827 7b7d 2073 7563 6365 7373  sage('{} success
-00003fe0: 6675 6c6c 7920 756e 696e 7374 616c 6c65  fully uninstalle
-00003ff0: 6427 2e66 6f72 6d61 7428 706c 7567 696e  d'.format(plugin
-00004000: 2e6e 616d 6529 290d 0a20 2020 2020 2020  .name))..       
-00004010: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00004020: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
-00004030: 2020 2020 2067 2e61 6c65 7274 2874 6974       g.alert(tit
-00004040: 6c65 3d22 506c 7567 696e 2055 6e69 6e73  le="Plugin Unins
-00004050: 7461 6c6c 2046 6169 6c65 6422 2c20 6d73  tall Failed", ms
-00004060: 673d 2255 6e61 626c 6520 746f 2072 656d  g="Unable to rem
-00004070: 6f76 6520 7468 6520 666f 6c64 6572 2061  ove the folder a
-00004080: 7420 2573 5c6e 2573 5c6e 4465 6c65 7465  t %s\n%s\nDelete
-00004090: 2074 6865 2066 6f6c 6465 7220 6d61 6e75   the folder manu
-000040a0: 616c 6c79 2074 6f20 756e 696e 7374 616c  ally to uninstal
-000040b0: 6c20 7468 6520 706c 7567 696e 2220 2520  l the plugin" % 
-000040c0: 2870 6c75 6769 6e2e 6e61 6d65 2c20 6529  (plugin.name, e)
-000040d0: 2c20 6963 6f6e 3d51 7457 6964 6765 7473  , icon=QtWidgets
-000040e0: 2e51 4d65 7373 6167 6542 6f78 2e57 6172  .QMessageBox.War
-000040f0: 6e69 6e67 290d 0a0d 0a20 2020 2020 2020  ning)....       
-00004100: 2050 6c75 6769 6e4d 616e 6167 6572 2e67   PluginManager.g
-00004110: 7569 2e70 6c75 6769 6e53 656c 6563 7465  ui.pluginSelecte
-00004120: 6428 706c 7567 696e 2e6c 6973 7457 6964  d(plugin.listWid
-00004130: 6765 7429 0d0a 2020 2020 2020 2020 706c  get)..        pl
-00004140: 7567 696e 2e69 6e73 7461 6c6c 6564 203d  ugin.installed =
-00004150: 2046 616c 7365 0d0a 0d0a 2020 2020 4073   False....    @s
-00004160: 7461 7469 636d 6574 686f 640d 0a20 2020  taticmethod..   
-00004170: 2064 6566 2064 6f77 6e6c 6f61 6450 6c75   def downloadPlu
-00004180: 6769 6e28 706c 7567 696e 293a 0d0a 2020  gin(plugin):..  
-00004190: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-000041a0: 6e63 6528 706c 7567 696e 2c20 7374 7229  nce(plugin, str)
-000041b0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-000041c0: 6620 706c 7567 696e 2069 6e20 506c 7567  f plugin in Plug
-000041d0: 696e 4d61 6e61 6765 722e 706c 7567 696e  inManager.plugin
-000041e0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000041f0: 2020 2020 706c 7567 696e 203d 2050 6c75      plugin = Plu
-00004200: 6769 6e4d 616e 6167 6572 2e70 6c75 6769  ginManager.plugi
-00004210: 6e73 5b70 6c75 6769 6e5d 0d0a 2020 2020  ns[plugin]..    
-00004220: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00004230: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004240: 6574 7572 6e0d 0a20 2020 2020 2020 2069  eturn..        i
-00004250: 6620 706c 7567 696e 2e75 726c 2069 7320  f plugin.url is 
-00004260: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00004270: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
-00004280: 2020 2066 6169 6c65 6420 3d20 5b5d 0d0a     failed = []..
-00004290: 2020 2020 2020 2020 6469 7374 7320 3d20          dists = 
-000042a0: 5b61 2e70 726f 6a65 6374 5f6e 616d 6520  [a.project_name 
-000042b0: 666f 7220 6120 696e 2070 6970 2e67 6574  for a in pip.get
-000042c0: 5f69 6e73 7461 6c6c 6564 5f64 6973 7472  _installed_distr
-000042d0: 6962 7574 696f 6e73 2829 5d0d 0a20 2020  ibutions()]..   
-000042e0: 2020 2020 2050 6c75 6769 6e4d 616e 6167       PluginManag
-000042f0: 6572 2e67 7569 2e73 7461 7475 7342 6172  er.gui.statusBar
-00004300: 2e73 686f 774d 6573 7361 6765 2822 496e  .showMessage("In
-00004310: 7374 616c 6c69 6e67 2064 6570 656e 6465  stalling depende
-00004320: 6e63 6965 7320 666f 7220 2573 2220 2520  ncies for %s" % 
-00004330: 706c 7567 696e 2e6e 616d 6529 0d0a 2020  plugin.name)..  
-00004340: 2020 2020 2020 666f 7220 706c 2069 6e20        for pl in 
-00004350: 706c 7567 696e 2e64 6570 656e 6465 6e63  plugin.dependenc
-00004360: 6965 733a 0d0a 2020 2020 2020 2020 2020  ies:..          
-00004370: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00004380: 2020 2020 2020 2020 6966 2070 6c20 696e          if pl in
-00004390: 2064 6973 7473 3a0d 0a20 2020 2020 2020   dists:..       
-000043a0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000043b0: 7469 6e75 650d 0a20 2020 2020 2020 2020  tinue..         
-000043c0: 2020 2020 2020 2061 203d 205f 5f69 6d70         a = __imp
-000043d0: 6f72 745f 5f28 706c 290d 0a20 2020 2020  ort__(pl)..     
-000043e0: 2020 2020 2020 2065 7863 6570 7420 496d         except Im
-000043f0: 706f 7274 4572 726f 723a 0d0a 2020 2020  portError:..    
-00004400: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-00004410: 3d20 7069 702e 6d61 696e 285b 2769 6e73  = pip.main(['ins
-00004420: 7461 6c6c 272c 2070 6c2c 2027 2d2d 6e6f  tall', pl, '--no
-00004430: 2d63 6163 6865 2d64 6972 275d 290d 0a20  -cache-dir']).. 
-00004440: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004450: 6620 7265 7320 213d 2030 3a0d 0a20 2020  f res != 0:..   
-00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004470: 2066 6169 6c65 642e 6170 7065 6e64 2870   failed.append(p
-00004480: 6c29 0d0a 2020 2020 2020 2020 6966 2066  l)..        if f
-00004490: 6169 6c65 643a 0d0a 2020 2020 2020 2020  ailed:..        
-000044a0: 2020 2020 6966 2070 6c61 7466 6f72 6d2e      if platform.
-000044b0: 7379 7374 656d 2829 203d 3d20 2757 696e  system() == 'Win
-000044c0: 646f 7773 273a 0d0a 2020 2020 2020 2020  dows':..        
-000044d0: 2020 2020 2020 2020 5174 4775 692e 5144          QtGui.QD
-000044e0: 6573 6b74 6f70 5365 7276 6963 6573 2e6f  esktopServices.o
-000044f0: 7065 6e55 726c 2851 7443 6f72 652e 5155  penUrl(QtCore.QU
-00004500: 726c 2822 6874 7470 3a2f 2f77 7777 2e6c  rl("http://www.l
-00004510: 6664 2e75 6369 2e65 6475 2f7e 676f 686c  fd.uci.edu/~gohl
-00004520: 6b65 2f70 7974 686f 6e6c 6962 732f 2322  ke/pythonlibs/#"
-00004530: 2b70 6c29 290d 0a20 2020 2020 2020 2020  +pl))..         
-00004540: 2020 2020 2020 2076 203d 2073 7472 2873         v = str(s
-00004550: 7973 2e76 6572 7369 6f6e 5f69 6e66 6f2e  ys.version_info.
-00004560: 6d61 6a6f 7229 202b 2073 7472 2873 7973  major) + str(sys
-00004570: 2e76 6572 7369 6f6e 5f69 6e66 6f2e 6d69  .version_info.mi
-00004580: 6e6f 7229 0d0a 2020 2020 2020 2020 2020  nor)..          
-00004590: 2020 2020 2020 6966 2070 6c61 7466 6f72        if platfor
-000045a0: 6d2e 6172 6368 6974 6563 7475 7265 2829  m.architecture()
-000045b0: 5b30 5d3d 3d27 3634 6269 7427 3a0d 0a20  [0]=='64bit':.. 
-000045c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045d0: 2020 2061 7263 6820 3d20 275f 616d 6436     arch = '_amd6
-000045e0: 3427 0d0a 2020 2020 2020 2020 2020 2020  4'..            
-000045f0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00004600: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00004610: 7263 6820 3d20 2733 3227 0d0a 2020 2020  rch = '32'..    
-00004620: 2020 2020 2020 2020 2020 2020 672e 616c              g.al
-00004630: 6572 7428 2222 2246 6169 6c65 6420 746f  ert("""Failed to
-00004640: 2069 6e73 7461 6c6c 2074 6865 2064 6570   install the dep
-00004650: 656e 6465 6e63 7920 277b 307d 272e 2059  endency '{0}'. Y
-00004660: 6f75 206d 7573 7420 696e 7374 616c 6c20  ou must install 
-00004670: 7b30 7d20 6d61 6e75 616c 6c79 2e0d 0a44  {0} manually...D
-00004680: 6f77 6e6c 6f61 6420 7b30 7d2d 782d 6370  ownload {0}-x-cp
-00004690: 7b31 7d2d 6370 7b31 7d6d 2d77 696e 7b32  {1}-cp{1}m-win{2
-000046a0: 7d2e 7768 6c2e 0d0a 0d0a 4f6e 6365 2074  }.whl.....Once t
-000046b0: 6865 2077 6865 656c 2069 7320 646f 776e  he wheel is down
-000046c0: 6c6f 6164 6564 2c20 6472 6167 2069 7420  loaded, drag it 
-000046d0: 696e 746f 2066 6c69 6b61 2074 6f20 696e  into flika to in
-000046e0: 7374 616c 6c2e 0d0a 0d0a 5468 656e 2074  stall.....Then t
-000046f0: 7279 2069 6e73 7461 6c6c 696e 6720 7468  ry installing th
-00004700: 6520 706c 7567 696e 2061 6761 696e 2e22  e plugin again."
-00004710: 2222 2e66 6f72 6d61 7428 706c 2c20 762c  "".format(pl, v,
-00004720: 2061 7263 6829 290d 0a20 2020 2020 2020   arch))..       
-00004730: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00004740: 2020 2020 2020 2020 2020 2020 672e 616c              g.al
-00004750: 6572 7428 2246 6169 6c65 6420 746f 2069  ert("Failed to i
-00004760: 6e73 7461 6c6c 2064 6570 656e 6465 6e63  nstall dependenc
-00004770: 6965 7320 666f 7220 7b7d 3a5c 6e7b 7d5c  ies for {}:\n{}\
-00004780: 6e59 6f75 206d 7573 7420 696e 7374 616c  nYou must instal
-00004790: 6c20 7468 656d 206f 6e20 796f 7572 206f  l them on your o
-000047a0: 776e 2062 6566 6f72 6520 696e 7374 616c  wn before instal
-000047b0: 6c69 6e67 2074 6869 7320 706c 7567 696e  ling this plugin
-000047c0: 2e22 2e66 6f72 6d61 7428 706c 7567 696e  .".format(plugin
-000047d0: 2e6e 616d 652c 2027 2c20 272e 6a6f 696e  .name, ', '.join
-000047e0: 2866 6169 6c65 6429 2929 0d0a 0d0a 2020  (failed)))....  
-000047f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00004800: 0d0a 0d0a 2020 2020 2020 2020 6966 206f  ....        if o
-00004810: 732e 7061 7468 2e65 7869 7374 7328 6f73  s.path.exists(os
-00004820: 2e70 6174 682e 6a6f 696e 2867 6574 5f70  .path.join(get_p
-00004830: 6c75 6769 6e5f 6469 7265 6374 6f72 7928  lugin_directory(
-00004840: 292c 2070 6c75 6769 6e2e 6469 7265 6374  ), plugin.direct
-00004850: 6f72 7929 293a 0d0a 2020 2020 2020 2020  ory)):..        
-00004860: 2020 2020 672e 616c 6572 7428 2241 2066      g.alert("A f
-00004870: 6f6c 6465 7220 7769 7468 206e 616d 6520  older with name 
-00004880: 7b7d 2061 6c72 6561 6479 2065 7869 7374  {} already exist
-00004890: 7320 696e 2074 6865 2070 6c75 6769 6e73  s in the plugins
-000048a0: 2064 6972 6563 746f 7279 2e20 506c 6561   directory. Plea
-000048b0: 7365 2072 656d 6f76 6520 6974 2074 6f20  se remove it to 
-000048c0: 696e 7374 616c 6c20 7468 6973 2070 6c75  install this plu
-000048d0: 6769 6e21 222e 666f 726d 6174 2870 6c75  gin!".format(plu
-000048e0: 6769 6e2e 6469 7265 6374 6f72 7929 290d  gin.directory)).
-000048f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00004900: 7572 6e0d 0a0d 0a20 2020 2020 2020 2050  urn....        P
-00004910: 6c75 6769 6e4d 616e 6167 6572 2e67 7569  luginManager.gui
-00004920: 2e73 7461 7475 7342 6172 2e73 686f 774d  .statusBar.showM
-00004930: 6573 7361 6765 2827 4f70 656e 696e 6720  essage('Opening 
-00004940: 2573 2720 2520 706c 7567 696e 2e75 726c  %s' % plugin.url
-00004950: 290d 0a20 2020 2020 2020 2074 7279 3a0d  )..        try:.
-00004960: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00004970: 6120 3d20 7572 6c6f 7065 6e28 706c 7567  a = urlopen(plug
-00004980: 696e 2e75 726c 292e 7265 6164 2829 0d0a  in.url).read()..
-00004990: 2020 2020 2020 2020 6578 6365 7074 3a0d          except:.
-000049a0: 0a20 2020 2020 2020 2020 2020 2067 2e61  .            g.a
-000049b0: 6c65 7274 2874 6974 6c65 3d22 446f 776e  lert(title="Down
-000049c0: 6c6f 6164 2045 7272 6f72 222c 206d 7367  load Error", msg
-000049d0: 3d22 4661 696c 6564 2074 6f20 636f 6e6e  ="Failed to conn
-000049e0: 6563 7420 746f 2025 7320 746f 2069 6e73  ect to %s to ins
-000049f0: 7461 6c6c 2074 6865 2025 7320 666c 696b  tall the %s flik
-00004a00: 6120 506c 7567 696e 2e20 4368 6563 6b20  a Plugin. Check 
-00004a10: 796f 7572 2069 6e74 6572 6e65 7420 636f  your internet co
-00004a20: 6e6e 6563 7469 6f6e 2061 6e64 2074 7279  nnection and try
-00004a30: 2061 6761 696e 2c20 6f72 2064 6f77 6e6c   again, or downl
-00004a40: 6f61 6420 7468 6520 706c 7567 696e 206d  oad the plugin m
-00004a50: 616e 7561 6c6c 792e 2220 2520 2850 6c75  anually." % (Plu
-00004a60: 6769 6e4d 616e 6167 6572 2e67 7569 2e6c  ginManager.gui.l
-00004a70: 696e 6b2c 2070 6c75 6769 6e2e 6e61 6d65  ink, plugin.name
-00004a80: 292c 2069 636f 6e3d 5174 5769 6467 6574  ), icon=QtWidget
-00004a90: 732e 514d 6573 7361 6765 426f 782e 5761  s.QMessageBox.Wa
-00004aa0: 726e 696e 6729 0d0a 2020 2020 2020 2020  rning)..        
-00004ab0: 2020 2020 7265 7475 726e 0d0a 0d0a 2020      return....  
-00004ac0: 2020 2020 2020 7472 793a 0d0a 0d0a 2020        try:....  
-00004ad0: 2020 2020 2020 2020 2020 7769 7468 2074            with t
-00004ae0: 656d 7066 696c 652e 5465 6d70 6f72 6172  empfile.Temporar
-00004af0: 7946 696c 6528 2920 6173 2074 663a 0d0a  yFile() as tf:..
-00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b10: 7466 2e77 7269 7465 2864 6174 6129 0d0a  tf.write(data)..
-00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b30: 7466 2e73 6565 6b28 3029 0d0a 2020 2020  tf.seek(0)..    
-00004b40: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00004b50: 207a 6970 6669 6c65 2e5a 6970 4669 6c65   zipfile.ZipFile
-00004b60: 2874 6629 2061 7320 7a3a 0d0a 2020 2020  (tf) as z:..    
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b80: 666f 6c64 6572 5f6e 616d 6520 3d20 6f73  folder_name = os
-00004b90: 2e70 6174 682e 6469 726e 616d 6528 7a2e  .path.dirname(z.
-00004ba0: 6e61 6d65 6c69 7374 2829 5b30 5d29 0d0a  namelist()[0])..
-00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 2020 2020 7a2e 6578 7472 6163 7461 6c6c      z.extractall
-00004bd0: 2867 6574 5f70 6c75 6769 6e5f 6469 7265  (get_plugin_dire
-00004be0: 6374 6f72 7928 2929 0d0a 0d0a 2020 2020  ctory())....    
-00004bf0: 2020 2020 2020 2020 706c 7567 696e 203d          plugin =
-00004c00: 2050 6c75 6769 6e4d 616e 6167 6572 2e70   PluginManager.p
-00004c10: 6c75 6769 6e73 5b70 6c75 6769 6e2e 6e61  lugins[plugin.na
-00004c20: 6d65 5d0d 0a20 2020 2020 2020 2020 2020  me]..           
-00004c30: 2064 6972 6563 746f 7279 203d 206f 732e   directory = os.
-00004c40: 7061 7468 2e6a 6f69 6e28 6765 745f 706c  path.join(get_pl
-00004c50: 7567 696e 5f64 6972 6563 746f 7279 2829  ugin_directory()
-00004c60: 2c20 706c 7567 696e 2e64 6972 6563 746f  , plugin.directo
-00004c70: 7279 290d 0a20 2020 2020 2020 2020 2020  ry)..           
-00004c80: 206f 732e 7265 6e61 6d65 286f 732e 7061   os.rename(os.pa
-00004c90: 7468 2e6a 6f69 6e28 6765 745f 706c 7567  th.join(get_plug
-00004ca0: 696e 5f64 6972 6563 746f 7279 2829 2c20  in_directory(), 
-00004cb0: 666f 6c64 6572 5f6e 616d 6529 2c20 6469  folder_name), di
-00004cc0: 7265 6374 6f72 7929 0d0a 2020 2020 2020  rectory)..      
-00004cd0: 2020 6578 6365 7074 2028 5065 726d 6973    except (Permis
-00004ce0: 7369 6f6e 4572 726f 722c 2045 7863 6570  sionError, Excep
-00004cf0: 7469 6f6e 2920 6173 2065 3a0d 0a20 2020  tion) as e:..   
-00004d00: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
-00004d10: 6174 682e 6578 6973 7473 2866 6f6c 6465  ath.exists(folde
-00004d20: 725f 6e61 6d65 293a 0d0a 2020 2020 2020  r_name):..      
-00004d30: 2020 2020 2020 2020 2020 7368 7574 696c            shutil
-00004d40: 2e72 6d74 7265 6528 666f 6c64 6572 5f6e  .rmtree(folder_n
-00004d50: 616d 6529 0d0a 2020 2020 2020 2020 2020  ame)..          
-00004d60: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00004d70: 652c 2050 6572 6d69 7373 696f 6e45 7272  e, PermissionErr
-00004d80: 6f72 293a 0d0a 2020 2020 2020 2020 2020  or):..          
-00004d90: 2020 2020 2020 672e 616c 6572 7428 2255        g.alert("U
-00004da0: 6e61 626c 6520 746f 2064 6f77 6e6c 6f61  nable to downloa
-00004db0: 6420 706c 7567 696e 2074 6f20 7b7d 2e20  d plugin to {}. 
-00004dc0: 5265 7275 6e20 666c 696b 6120 6173 2061  Rerun flika as a
-00004dd0: 646d 696e 6973 7472 6174 6f72 2061 6e64  dministrator and
-00004de0: 2064 6f77 6e6c 6f61 6420 7468 6520 706c   download the pl
-00004df0: 7567 696e 2061 6761 696e 2e22 2e66 6f72  ugin again.".for
-00004e00: 6d61 7428 706c 7567 696e 2e6e 616d 6529  mat(plugin.name)
-00004e10: 2c20 7469 746c 653d 2750 6572 6d69 7373  , title='Permiss
-00004e20: 696f 6e20 4465 6e69 6564 2729 0d0a 2020  ion Denied')..  
-00004e30: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00004e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e50: 2067 2e61 6c65 7274 2822 4572 726f 7220   g.alert("Error 
-00004e60: 6f63 6375 7272 6564 2077 6869 6c65 2069  occurred while i
-00004e70: 6e73 7461 6c6c 696e 6720 7b7d 2e5c 6e5c  nstalling {}.\n\
-00004e80: 747b 7d22 2e66 6f72 6d61 7428 706c 7567  t{}".format(plug
-00004e90: 696e 2e6e 616d 652c 2065 292c 2074 6974  in.name, e), tit
-00004ea0: 6c65 3d27 506c 7567 696e 2049 6e73 7461  le='Plugin Insta
-00004eb0: 6c6c 2046 6169 6c65 6427 2920 2020 200d  ll Failed')    .
-00004ec0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-00004ed0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00004ee0: 6e0d 0a20 2020 2020 2020 200d 0a20 2020  n..        ..   
-00004ef0: 2020 2020 2050 6c75 6769 6e4d 616e 6167       PluginManag
-00004f00: 6572 2e67 7569 2e73 7461 7475 7342 6172  er.gui.statusBar
-00004f10: 2e73 686f 774d 6573 7361 6765 2827 4578  .showMessage('Ex
-00004f20: 7472 6163 7469 6e67 2020 2573 2720 2520  tracting  %s' % 
-00004f30: 706c 7567 696e 2e6e 616d 6529 0d0a 2020  plugin.name)..  
-00004f40: 2020 2020 2020 706c 7567 696e 2e76 6572        plugin.ver
-00004f50: 7369 6f6e 203d 2070 6c75 6769 6e2e 6c61  sion = plugin.la
-00004f60: 7465 7374 5f76 6572 7369 6f6e 0d0a 2020  test_version..  
-00004f70: 2020 2020 2020 706c 7567 696e 2e6c 6973        plugin.lis
-00004f80: 7457 6964 6765 742e 7365 7449 636f 6e28  tWidget.setIcon(
-00004f90: 5174 4775 692e 5149 636f 6e28 696d 6167  QtGui.QIcon(imag
-00004fa0: 655f 7061 7468 2822 6368 6563 6b2e 706e  e_path("check.pn
-00004fb0: 6722 2929 290d 0a20 2020 2020 2020 2023  g")))..        #
-00004fc0: 706c 7567 696e 2e6d 656e 7520 3d20 6d61  plugin.menu = ma
-00004fd0: 6b65 5f70 6c75 6769 6e5f 6d65 6e75 2870  ke_plugin_menu(p
-00004fe0: 6c75 6769 6e29 0d0a 2020 2020 2020 2020  lugin)..        
-00004ff0: 706c 7567 696e 2e6d 656e 7520 3d20 5174  plugin.menu = Qt
-00005000: 5769 6467 6574 732e 514d 656e 7528 706c  Widgets.QMenu(pl
-00005010: 7567 696e 2e6e 616d 6529 0d0a 2020 2020  ugin.name)..    
-00005020: 2020 2020 6275 696c 645f 7375 626d 656e      build_submen
-00005030: 7528 706c 7567 696e 2e64 6972 6563 746f  u(plugin.directo
-00005040: 7279 2c20 706c 7567 696e 2e6d 656e 752c  ry, plugin.menu,
-00005050: 2070 6c75 6769 6e2e 6d65 6e75 5f6c 6179   plugin.menu_lay
-00005060: 6f75 7429 0d0a 2020 2020 2020 2020 0d0a  out)..        ..
-00005070: 2020 2020 2020 2020 506c 7567 696e 4d61          PluginMa
-00005080: 6e61 6765 722e 6775 692e 7374 6174 7573  nager.gui.status
-00005090: 4261 722e 7368 6f77 4d65 7373 6167 6528  Bar.showMessage(
-000050a0: 2753 7563 6365 7373 6675 6c6c 7920 696e  'Successfully in
-000050b0: 7374 616c 6c65 6420 7b7d 2061 6e64 2069  stalled {} and i
-000050c0: 745c 2773 2064 6570 656e 6465 6e63 6965  t\'s dependencie
-000050d0: 7327 2e66 6f72 6d61 7428 706c 7567 696e  s'.format(plugin
-000050e0: 2e6e 616d 6529 290d 0a20 2020 2020 2020  .name))..       
-000050f0: 2050 6c75 6769 6e4d 616e 6167 6572 2e67   PluginManager.g
-00005100: 7569 2e70 6c75 6769 6e53 656c 6563 7465  ui.pluginSelecte
-00005110: 6428 706c 7567 696e 2e6c 6973 7457 6964  d(plugin.listWid
-00005120: 6765 7429 0d0a 2020 2020 2020 2020 706c  get)..        pl
-00005130: 7567 696e 2e69 6e73 7461 6c6c 6564 203d  ugin.installed =
-00005140: 2054 7275 650d 0a0d 0a64 6566 206c 6f61   True....def loa
-00005150: 645f 6c6f 6361 6c5f 706c 7567 696e 7328  d_local_plugins(
-00005160: 293a 0d0a 2020 2020 506c 7567 696e 4d61  ):..    PluginMa
-00005170: 6e61 6765 722e 706c 7567 696e 7320 3d20  nager.plugins = 
-00005180: 7b6e 3a20 506c 7567 696e 286e 2920 666f  {n: Plugin(n) fo
-00005190: 7220 6e20 696e 2070 6c75 6769 6e5f 6c69  r n in plugin_li
-000051a0: 7374 7d0d 0a20 2020 2066 6f72 2070 6c75  st}..    for plu
-000051b0: 6769 6e50 6174 6820 696e 2050 6c75 6769  ginPath in Plugi
-000051c0: 6e4d 616e 6167 6572 2e6c 6f63 616c 5f70  nManager.local_p
-000051d0: 6c75 6769 6e5f 7061 7468 7328 293a 0d0a  lugin_paths():..
-000051e0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-000051f0: 2020 2020 2020 2020 2020 7020 3d20 506c            p = Pl
-00005200: 7567 696e 2e66 726f 6d4c 6f63 616c 2870  ugin.fromLocal(p
-00005210: 6c75 6769 6e50 6174 6829 0d0a 2020 2020  luginPath)..    
-00005220: 2020 2020 2020 2020 702e 696e 7374 616c          p.instal
-00005230: 6c65 6420 3d20 5472 7565 0d0a 2020 2020  led = True..    
-00005240: 2020 2020 2020 2020 506c 7567 696e 4d61          PluginMa
-00005250: 6e61 6765 722e 706c 7567 696e 735b 702e  nager.plugins[p.
-00005260: 6e61 6d65 5d20 3d20 700d 0a20 2020 2020  name] = p..     
-00005270: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00005280: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-00005290: 2020 2020 2020 2067 2e61 6c65 7274 2822         g.alert("
-000052a0: 436f 756c 6420 6e6f 7420 6c6f 6164 207b  Could not load {
-000052b0: 7d2e 5c6e 5c74 7b7d 222e 666f 726d 6174  }.\n\t{}".format
-000052c0: 2870 6c75 6769 6e50 6174 682c 2074 7261  (pluginPath, tra
-000052d0: 6365 6261 636b 2e66 6f72 6d61 745f 6578  ceback.format_ex
-000052e0: 6328 2929 2c20 7469 746c 653d 2250 6c75  c()), title="Plu
-000052f0: 6769 6e20 4c6f 6164 2045 7272 6f72 2229  gin Load Error")
-00005300: 0d0a                                     ..
+000027b0: 6520 616e 6420 506c 7567 696e 4d61 6e61  e and PluginMana
+000027c0: 6765 722e 6c6f 6164 5468 7265 6164 2e69  ger.loadThread.i
+000027d0: 735f 616c 6976 6528 293a 0a20 2020 2020  s_alive():.     
+000027e0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000027f0: 2020 2020 2020 6465 6620 6c6f 6164 5468        def loadTh
+00002800: 7265 6164 2829 3a0a 2020 2020 2020 2020  read():.        
+00002810: 2020 2020 706c 7567 203d 2050 6c75 6769      plug = Plugi
+00002820: 6e4d 616e 6167 6572 2e70 6c75 6769 6e73  nManager.plugins
+00002830: 5b70 5d0a 2020 2020 2020 2020 2020 2020  [p].            
+00002840: 706c 7567 2e69 6e66 6f5f 7572 6c20 3d20  plug.info_url = 
+00002850: 706c 7567 696e 5f6c 6973 745b 705d 0a20  plugin_list[p]. 
+00002860: 2020 2020 2020 2020 2020 2070 6c75 672e             plug.
+00002870: 7570 6461 7465 5f69 6e66 6f28 290a 2020  update_info().  
+00002880: 2020 2020 2020 2020 2020 506c 7567 696e            Plugin
+00002890: 4d61 6e61 6765 722e 6775 692e 7369 6750  Manager.gui.sigP
+000028a0: 6c75 6769 6e4c 6f61 6465 642e 656d 6974  luginLoaded.emit
+000028b0: 2870 290a 2020 2020 2020 2020 2020 2020  (p).            
+000028c0: 2350 6c75 6769 6e4d 616e 6167 6572 2e67  #PluginManager.g
+000028d0: 7569 2e73 7461 7475 7342 6172 2e73 686f  ui.statusBar.sho
+000028e0: 774d 6573 7361 6765 2827 506c 7567 696e  wMessage('Plugin
+000028f0: 2069 6e66 6f72 6d61 7469 6f6e 206c 6f61   information loa
+00002900: 6465 6420 7375 6363 6573 7366 756c 6c79  ded successfully
+00002910: 2729 0a0a 2020 2020 2020 2020 506c 7567  ')..        Plug
+00002920: 696e 4d61 6e61 6765 722e 6c6f 6164 5468  inManager.loadTh
+00002930: 7265 6164 203d 2074 6872 6561 6469 6e67  read = threading
+00002940: 2e54 6872 6561 6428 4e6f 6e65 2c20 6c6f  .Thread(None, lo
+00002950: 6164 5468 7265 6164 290a 2020 2020 2020  adThread).      
+00002960: 2020 506c 7567 696e 4d61 6e61 6765 722e    PluginManager.
+00002970: 6775 692e 7374 6174 7573 4261 722e 7368  gui.statusBar.sh
+00002980: 6f77 4d65 7373 6167 6528 274c 6f61 6469  owMessage('Loadi
+00002990: 6e67 2070 6c75 6769 6e20 696e 666f 726d  ng plugin inform
+000029a0: 6174 696f 6e20 666f 7220 7b7d 2e2e 2e27  ation for {}...'
+000029b0: 2e66 6f72 6d61 7428 7029 290a 2020 2020  .format(p)).    
+000029c0: 2020 2020 506c 7567 696e 4d61 6e61 6765      PluginManage
+000029d0: 722e 6c6f 6164 5468 7265 6164 2e73 7461  r.loadThread.sta
+000029e0: 7274 2829 0a0a 2020 2020 6465 6620 636c  rt()..    def cl
+000029f0: 6f73 6545 7665 6e74 2873 656c 662c 2065  oseEvent(self, e
+00002a00: 7629 3a0a 2020 2020 2020 2020 6966 2073  v):.        if s
+00002a10: 656c 662e 6c6f 6164 5468 7265 6164 2069  elf.loadThread i
+00002a20: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
+00002a30: 656c 662e 6c6f 6164 5468 7265 6164 2e69  elf.loadThread.i
+00002a40: 735f 616c 6976 6528 293a 0a20 2020 2020  s_alive():.     
+00002a50: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
+00002a60: 5468 7265 6164 2e6a 6f69 6e28 3029 0a0a  Thread.join(0)..
+00002a70: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+00002a80: 640a 2020 2020 6465 6620 636c 6f73 6528  d.    def close(
+00002a90: 293a 0a20 2020 2020 2020 2069 6620 6861  ):.        if ha
+00002aa0: 7361 7474 7228 506c 7567 696e 4d61 6e61  sattr(PluginMana
+00002ab0: 6765 722c 2027 6775 6927 293a 0a20 2020  ger, 'gui'):.   
+00002ac0: 2020 2020 2020 2020 2051 7457 6964 6765           QtWidge
+00002ad0: 7473 2e51 4d61 696e 5769 6e64 6f77 2e63  ts.QMainWindow.c
+00002ae0: 6c6f 7365 2850 6c75 6769 6e4d 616e 6167  lose(PluginManag
+00002af0: 6572 2e67 7569 290a 0a20 2020 2064 6566  er.gui)..    def
+00002b00: 205f 5f69 6e69 745f 5f28 7365 6c66 293a   __init__(self):
+00002b10: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00002b20: 6465 6275 6728 2743 616c 6c69 6e67 2061  debug('Calling a
+00002b30: 7070 2e70 6c75 6769 6e5f 6d61 6e61 6765  pp.plugin_manage
+00002b40: 722e 506c 7567 696e 4d61 6e61 6765 722e  r.PluginManager.
+00002b50: 6c6f 6164 5f6f 6e6c 696e 655f 706c 7567  load_online_plug
+00002b60: 696e 2829 2729 0a0a 2020 2020 2020 2020  in()')..        
+00002b70: 7375 7065 7228 506c 7567 696e 4d61 6e61  super(PluginMana
+00002b80: 6765 722c 7365 6c66 292e 5f5f 696e 6974  ger,self).__init
+00002b90: 5f5f 2829 0a20 2020 2020 2020 206c 6f61  __().        loa
+00002ba0: 645f 7569 2822 706c 7567 696e 5f6d 616e  d_ui("plugin_man
+00002bb0: 6167 6572 2e75 6922 2c20 7365 6c66 2c20  ager.ui", self, 
+00002bc0: 6469 7265 6374 6f72 793d 6f73 2e70 6174  directory=os.pat
+00002bd0: 682e 6469 726e 616d 6528 5f5f 6669 6c65  h.dirname(__file
+00002be0: 5f5f 2929 0a20 2020 2020 2020 2074 7279  __)).        try
+00002bf0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00002c00: 6c66 2e73 6372 6f6c 6c41 7265 6157 6964  lf.scrollAreaWid
+00002c10: 6765 7443 6f6e 7465 6e74 732e 7365 7443  getContents.setC
+00002c20: 6f6e 7465 6e74 734d 6172 6769 6e73 2831  ontentsMargins(1
+00002c30: 302c 2031 302c 2031 302c 2031 3029 0a20  0, 10, 10, 10). 
+00002c40: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
+00002c50: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+00002c60: 2020 2020 2020 2020 2373 656c 662e 706c          #self.pl
+00002c70: 7567 696e 4c69 7374 2e69 7465 6d43 6c69  uginList.itemCli
+00002c80: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002c90: 662e 706c 7567 696e 5365 6c65 6374 6564  f.pluginSelected
+00002ca0: 290a 2020 2020 2020 2020 7365 6c66 2e74  ).        self.t
+00002cb0: 7574 6f72 6961 6c42 7574 746f 6e2e 636c  utorialButton.cl
+00002cc0: 6963 6b65 642e 636f 6e6e 6563 7428 6c61  icked.connect(la
+00002cd0: 6d62 6461 203a 2051 7447 7569 2e51 4465  mbda : QtGui.QDe
+00002ce0: 736b 746f 7053 6572 7669 6365 732e 6f70  sktopServices.op
+00002cf0: 656e 5572 6c28 5174 436f 7265 2e51 5572  enUrl(QtCore.QUr
+00002d00: 6c28 2268 7474 7073 3a2f 2f67 6974 6875  l("https://githu
+00002d10: 622e 636f 6d2f 666c 696b 612d 6f72 672f  b.com/flika-org/
+00002d20: 666c 696b 615f 706c 7567 696e 5f74 656d  flika_plugin_tem
+00002d30: 706c 6174 6522 2929 290a 2020 2020 2020  plate"))).      
+00002d40: 2020 7365 6c66 2e6f 7065 6e5f 706c 7567    self.open_plug
+00002d50: 696e 735f 6469 7265 6374 6f72 795f 6275  ins_directory_bu
+00002d60: 7474 6f6e 2e63 6c69 636b 6564 2e63 6f6e  tton.clicked.con
+00002d70: 6e65 6374 286c 616d 6264 613a 2051 7447  nect(lambda: QtG
+00002d80: 7569 2e51 4465 736b 746f 7053 6572 7669  ui.QDesktopServi
+00002d90: 6365 732e 6f70 656e 5572 6c28 5174 436f  ces.openUrl(QtCo
+00002da0: 7265 2e51 5572 6c28 2266 696c 653a 2f2f  re.QUrl("file://
+00002db0: 2f22 202b 206f 732e 7061 7468 2e65 7870  /" + os.path.exp
+00002dc0: 616e 6475 7365 7228 277e 2f2e 464c 494b  anduser('~/.FLIK
+00002dd0: 412f 706c 7567 696e 732f 2729 2929 290a  A/plugins/')))).
+00002de0: 0a20 2020 2020 2020 2073 656c 662e 646f  .        self.do
+00002df0: 776e 6c6f 6164 4275 7474 6f6e 2e63 6c69  wnloadButton.cli
+00002e00: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
+00002e10: 662e 646f 776e 6c6f 6164 436c 6963 6b65  f.downloadClicke
+00002e20: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00002e30: 706c 7567 696e 4c69 7374 2e63 7572 7265  pluginList.curre
+00002e40: 6e74 4974 656d 4368 616e 6765 642e 636f  ntItemChanged.co
+00002e50: 6e6e 6563 7428 6c61 6d62 6461 206e 6577  nnect(lambda new
+00002e60: 2c20 6f6c 643a 2073 656c 662e 706c 7567  , old: self.plug
+00002e70: 696e 5365 6c65 6374 6564 286e 6577 2929  inSelected(new))
+00002e80: 0a20 2020 2020 2020 2073 656c 662e 646f  .        self.do
+00002e90: 6375 6d65 6e74 6174 696f 6e42 7574 746f  cumentationButto
+00002ea0: 6e2e 636c 6963 6b65 642e 636f 6e6e 6563  n.clicked.connec
+00002eb0: 7428 7365 6c66 2e64 6f63 756d 656e 7461  t(self.documenta
+00002ec0: 7469 6f6e 436c 6963 6b65 6429 0a20 2020  tionClicked).   
+00002ed0: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
+00002ee0: 4275 7474 6f6e 2e63 6c69 636b 6564 2e63  Button.clicked.c
+00002ef0: 6f6e 6e65 6374 2873 656c 662e 7570 6461  onnect(self.upda
+00002f00: 7465 436c 6963 6b65 6429 0a20 2020 2020  teClicked).     
+00002f10: 2020 200a 2020 2020 2020 2020 7365 6c66     .        self
+00002f20: 2e73 6561 7263 6842 6f78 2e74 6578 7443  .searchBox.textC
+00002f30: 6861 6e67 6564 2e63 6f6e 6e65 6374 2873  hanged.connect(s
+00002f40: 656c 662e 7368 6f77 506c 7567 696e 7329  elf.showPlugins)
+00002f50: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00002f60: 6172 6368 4275 7474 6f6e 2e63 6c69 636b  archButton.click
+00002f70: 6564 2e63 6f6e 6e65 6374 286c 616d 6264  ed.connect(lambd
+00002f80: 6120 663a 2073 656c 662e 7368 6f77 506c  a f: self.showPl
+00002f90: 7567 696e 7328 7365 6172 6368 5f73 7472  ugins(search_str
+00002fa0: 3d73 7472 2873 656c 662e 7365 6172 6368  =str(self.search
+00002fb0: 426f 782e 7465 7874 2829 2929 290a 2020  Box.text()))).  
+00002fc0: 2020 2020 2020 7365 6c66 2e64 6573 6372        self.descr
+00002fd0: 6970 7469 6f6e 4c61 6265 6c2e 7365 744f  iptionLabel.setO
+00002fe0: 7065 6e45 7874 6572 6e61 6c4c 696e 6b73  penExternalLinks
+00002ff0: 2854 7275 6529 0a20 2020 2020 2020 200a  (True).        .
+00003000: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00003010: 7265 7368 4275 7474 6f6e 2e70 7265 7373  reshButton.press
+00003020: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00003030: 7265 6672 6573 685f 6f6e 6c69 6e65 5f70  refresh_online_p
+00003040: 6c75 6769 6e73 290a 2020 2020 2020 2020  lugins).        
+00003050: 6465 6620 7570 6461 7465 506c 7567 696e  def updatePlugin
+00003060: 2861 293a 0a20 2020 2020 2020 2020 2020  (a):.           
+00003070: 2073 656c 662e 7374 6174 7573 4261 722e   self.statusBar.
+00003080: 7368 6f77 4d65 7373 6167 6528 2246 696e  showMessage("Fin
+00003090: 6973 6865 6420 6c6f 6164 696e 6720 7b7d  ished loading {}
+000030a0: 222e 666f 726d 6174 2861 2929 0a20 2020  ".format(a)).   
+000030b0: 2020 2020 2020 2020 2069 6620 506c 7567           if Plug
+000030c0: 696e 4d61 6e61 6765 722e 706c 7567 696e  inManager.plugin
+000030d0: 735b 615d 2e6c 6973 7457 6964 6765 742e  s[a].listWidget.
+000030e0: 6973 5365 6c65 6374 6564 2829 3a0a 2020  isSelected():.  
+000030f0: 2020 2020 2020 2020 2020 2020 2020 506c                Pl
+00003100: 7567 696e 4d61 6e61 6765 722e 6775 692e  uginManager.gui.
+00003110: 706c 7567 696e 5365 6c65 6374 6564 2861  pluginSelected(a
+00003120: 290a 2020 2020 2020 2020 2020 2020 2365  ).            #e
+00003130: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00003140: 2020 2020 2023 7365 6c66 2e73 686f 7750       #self.showP
+00003150: 6c75 6769 6e73 2829 0a20 2020 2020 2020  lugins().       
+00003160: 2073 656c 662e 7369 6750 6c75 6769 6e4c   self.sigPluginL
+00003170: 6f61 6465 642e 636f 6e6e 6563 7428 7570  oaded.connect(up
+00003180: 6461 7465 506c 7567 696e 290a 0a20 2020  datePlugin)..   
+00003190: 2020 2020 2073 656c 662e 7365 7457 696e       self.setWin
+000031a0: 646f 7754 6974 6c65 2827 506c 7567 696e  dowTitle('Plugin
+000031b0: 204d 616e 6167 6572 2729 0a20 2020 2020   Manager').     
+000031c0: 2020 2073 656c 662e 7368 6f77 506c 7567     self.showPlug
+000031d0: 696e 7328 290a 0a20 2020 2064 6566 2073  ins()..    def s
+000031e0: 686f 7748 656c 7053 6372 6565 6e28 7365  howHelpScreen(se
+000031f0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+00003200: 662e 706c 7567 696e 4c61 6265 6c2e 7365  f.pluginLabel.se
+00003210: 7454 6578 7428 2222 290a 2020 2020 2020  tText("").      
+00003220: 2020 7365 6c66 2e64 6573 6372 6970 7469    self.descripti
+00003230: 6f6e 4c61 6265 6c2e 7365 7448 746d 6c28  onLabel.setHtml(
+00003240: 6865 6c70 4854 4d4c 290a 2020 2020 2020  helpHTML).      
+00003250: 2020 7365 6c66 2e64 6f77 6e6c 6f61 6442    self.downloadB
+00003260: 7574 746f 6e2e 7365 7456 6973 6962 6c65  utton.setVisible
+00003270: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+00003280: 7365 6c66 2e64 6f63 756d 656e 7461 7469  self.documentati
+00003290: 6f6e 4275 7474 6f6e 2e73 6574 5669 7369  onButton.setVisi
+000032a0: 626c 6528 4661 6c73 6529 0a20 2020 2020  ble(False).     
+000032b0: 2020 2073 656c 662e 7570 6461 7465 4275     self.updateBu
+000032c0: 7474 6f6e 2e73 6574 5669 7369 626c 6528  tton.setVisible(
+000032d0: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
+000032e0: 656c 662e 696e 666f 4c61 6265 6c2e 7365  elf.infoLabel.se
+000032f0: 7454 6578 7428 2222 290a 0a20 2020 2064  tText("")..    d
+00003300: 6566 2064 6f77 6e6c 6f61 6443 6c69 636b  ef downloadClick
+00003310: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
+00003320: 2020 7020 3d20 7374 7228 7365 6c66 2e70    p = str(self.p
+00003330: 6c75 6769 6e4c 6973 742e 6375 7272 656e  luginList.curren
+00003340: 7449 7465 6d28 292e 7465 7874 2829 290a  tItem().text()).
+00003350: 2020 2020 2020 2020 706c 7567 696e 203d          plugin =
+00003360: 2073 656c 662e 706c 7567 696e 735b 705d   self.plugins[p]
+00003370: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00003380: 2e64 6f77 6e6c 6f61 6442 7574 746f 6e2e  .downloadButton.
+00003390: 7465 7874 2829 203d 3d20 2749 6e73 7461  text() == 'Insta
+000033a0: 6c6c 273a 0a20 2020 2020 2020 2020 2020  ll':.           
+000033b0: 2050 6c75 6769 6e4d 616e 6167 6572 2e64   PluginManager.d
+000033c0: 6f77 6e6c 6f61 6450 6c75 6769 6e28 706c  ownloadPlugin(pl
+000033d0: 7567 696e 290a 2020 2020 2020 2020 656c  ugin).        el
+000033e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000033f0: 506c 7567 696e 4d61 6e61 6765 722e 7265  PluginManager.re
+00003400: 6d6f 7665 506c 7567 696e 2870 6c75 6769  movePlugin(plugi
+00003410: 6e29 0a0a 2020 2020 6465 6620 646f 6375  n)..    def docu
+00003420: 6d65 6e74 6174 696f 6e43 6c69 636b 6564  mentationClicked
+00003430: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00003440: 7020 3d20 7374 7228 7365 6c66 2e70 6c75  p = str(self.plu
+00003450: 6769 6e4c 6973 742e 6375 7272 656e 7449  ginList.currentI
+00003460: 7465 6d28 292e 7465 7874 2829 290a 2020  tem().text()).  
+00003470: 2020 2020 2020 706c 7567 696e 203d 2073        plugin = s
+00003480: 656c 662e 706c 7567 696e 735b 705d 0a20  elf.plugins[p]. 
+00003490: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+000034a0: 7228 706c 7567 696e 2c20 2264 6f63 756d  r(plugin, "docum
+000034b0: 656e 7461 7469 6f6e 2229 3a0a 2020 2020  entation"):.    
+000034c0: 2020 2020 2020 2020 5174 4775 692e 5144          QtGui.QD
+000034d0: 6573 6b74 6f70 5365 7276 6963 6573 2e6f  esktopServices.o
+000034e0: 7065 6e55 726c 2851 7443 6f72 652e 5155  penUrl(QtCore.QU
+000034f0: 726c 2870 6c75 6769 6e2e 646f 6375 6d65  rl(plugin.docume
+00003500: 6e74 6174 696f 6e29 290a 0a20 2020 2064  ntation))..    d
+00003510: 6566 2075 7064 6174 6543 6c69 636b 6564  ef updateClicked
+00003520: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00003530: 7020 3d20 7374 7228 7365 6c66 2e70 6c75  p = str(self.plu
+00003540: 6769 6e4c 6973 742e 6375 7272 656e 7449  ginList.currentI
+00003550: 7465 6d28 292e 7465 7874 2829 290a 2020  tem().text()).  
+00003560: 2020 2020 2020 706c 7567 696e 203d 2073        plugin = s
+00003570: 656c 662e 706c 7567 696e 735b 705d 0a20  elf.plugins[p]. 
+00003580: 2020 2020 2020 2050 6c75 6769 6e4d 616e         PluginMan
+00003590: 6167 6572 2e72 656d 6f76 6550 6c75 6769  ager.removePlugi
+000035a0: 6e28 706c 7567 696e 290a 2020 2020 2020  n(plugin).      
+000035b0: 2020 506c 7567 696e 4d61 6e61 6765 722e    PluginManager.
+000035c0: 646f 776e 6c6f 6164 506c 7567 696e 2870  downloadPlugin(p
+000035d0: 6c75 6769 6e29 0a0a 2020 2020 6465 6620  lugin)..    def 
+000035e0: 706c 7567 696e 5365 6c65 6374 6564 2873  pluginSelected(s
+000035f0: 656c 662c 2069 7465 6d29 3a0a 2020 2020  elf, item):.    
+00003600: 2020 2020 6672 6f6d 2070 6b67 5f72 6573      from pkg_res
+00003610: 6f75 7263 6573 2069 6d70 6f72 7420 7061  ources import pa
+00003620: 7273 655f 7665 7273 696f 6e0a 2020 2020  rse_version.    
+00003630: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00003640: 2827 4361 6c6c 696e 6720 6170 702e 706c  ('Calling app.pl
+00003650: 7567 696e 5f6d 616e 6167 6572 2e50 6c75  ugin_manager.Plu
+00003660: 6769 6e4d 616e 6167 6572 2e70 6c75 6769  ginManager.plugi
+00003670: 6e53 656c 6563 7465 6428 2927 290a 2020  nSelected()').  
+00003680: 2020 2020 2020 6966 2069 7465 6d20 6973        if item is
+00003690: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000036a0: 2020 2069 6620 7365 6c66 2e70 6c75 6769     if self.plugi
+000036b0: 6e4c 6162 656c 2e74 6578 7428 293a 0a20  nLabel.text():. 
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000036d0: 656c 662e 706c 7567 696e 5365 6c65 6374  elf.pluginSelect
+000036e0: 6564 2850 6c75 6769 6e4d 616e 6167 6572  ed(PluginManager
+000036f0: 2e70 6c75 6769 6e73 5b73 656c 662e 706c  .plugins[self.pl
+00003700: 7567 696e 4c61 6265 6c2e 7465 7874 2829  uginLabel.text()
+00003710: 5d2e 6c69 7374 5769 6467 6574 290a 2020  ].listWidget).  
+00003720: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00003730: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00003740: 7374 616e 6365 2869 7465 6d2c 2073 7472  stance(item, str
+00003750: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00003760: 203d 2069 7465 6d0a 2020 2020 2020 2020   = item.        
+00003770: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00003780: 2020 7320 3d20 7374 7228 6974 656d 2e74    s = str(item.t
+00003790: 6578 7428 2929 0a20 2020 2020 2020 2070  ext()).        p
+000037a0: 6c75 6769 6e20 3d20 7365 6c66 2e70 6c75  lugin = self.plu
+000037b0: 6769 6e73 5b73 5d0a 2020 2020 2020 2020  gins[s].        
+000037c0: 7365 6c66 2e70 6c75 6769 6e4c 6162 656c  self.pluginLabel
+000037d0: 2e73 6574 5465 7874 2873 290a 2020 2020  .setText(s).    
+000037e0: 2020 2020 6966 206e 6f74 2070 6c75 6769      if not plugi
+000037f0: 6e2e 6c6f 6164 6564 3a0a 2020 2020 2020  n.loaded:.      
+00003800: 2020 2020 2020 696e 666f 203d 2022 4c6f        info = "Lo
+00003810: 6164 696e 6720 696e 666f 726d 6174 696f  ading informatio
+00003820: 6e22 0a20 2020 2020 2020 2065 6c73 653a  n".        else:
+00003830: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
+00003840: 6f20 3d20 2742 7920 7b7d 2c20 4c61 7465  o = 'By {}, Late
+00003850: 7374 3a20 7b7d 272e 666f 726d 6174 2870  st: {}'.format(p
+00003860: 6c75 6769 6e2e 6175 7468 6f72 2c20 706c  lugin.author, pl
+00003870: 7567 696e 2e6c 6174 6573 745f 7665 7273  ugin.latest_vers
+00003880: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
+00003890: 2073 656c 662e 646f 776e 6c6f 6164 4275   self.downloadBu
+000038a0: 7474 6f6e 2e73 6574 5669 7369 626c 6528  tton.setVisible(
+000038b0: 5472 7565 290a 2020 2020 2020 2020 7665  True).        ve
+000038c0: 7273 696f 6e20 3d20 7061 7273 655f 7665  rsion = parse_ve
+000038d0: 7273 696f 6e28 706c 7567 696e 2e76 6572  rsion(plugin.ver
+000038e0: 7369 6f6e 290a 2020 2020 2020 2020 6c61  sion).        la
+000038f0: 7465 7374 5f76 6572 7369 6f6e 203d 2070  test_version = p
+00003900: 6172 7365 5f76 6572 7369 6f6e 2870 6c75  arse_version(plu
+00003910: 6769 6e2e 6c61 7465 7374 5f76 6572 7369  gin.latest_versi
+00003920: 6f6e 290a 2020 2020 2020 2020 6966 2070  on).        if p
+00003930: 6c75 6769 6e2e 7665 7273 696f 6e20 616e  lugin.version an
+00003940: 6420 7665 7273 696f 6e20 3c20 6c61 7465  d version < late
+00003950: 7374 5f76 6572 7369 6f6e 3a0a 2020 2020  st_version:.    
+00003960: 2020 2020 2020 2020 696e 666f 202b 3d20          info += 
+00003970: 223b 203c 623e 5570 6461 7465 2041 7661  "; <b>Update Ava
+00003980: 696c 6162 6c65 213c 2f62 3e22 0a0a 2020  ilable!</b>"..  
+00003990: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
+000039a0: 6542 7574 746f 6e2e 7365 7456 6973 6962  eButton.setVisib
+000039b0: 6c65 2870 6c75 6769 6e2e 7665 7273 696f  le(plugin.versio
+000039c0: 6e20 213d 2027 2720 616e 6420 7665 7273  n != '' and vers
+000039d0: 696f 6e20 3c20 6c61 7465 7374 5f76 6572  ion < latest_ver
+000039e0: 7369 6f6e 290a 2020 2020 2020 2020 7365  sion).        se
+000039f0: 6c66 2e64 6f77 6e6c 6f61 6442 7574 746f  lf.downloadButto
+00003a00: 6e2e 7365 7454 6578 7428 2249 6e73 7461  n.setText("Insta
+00003a10: 6c6c 2220 6966 2070 6c75 6769 6e2e 7665  ll" if plugin.ve
+00003a20: 7273 696f 6e20 3d3d 2027 2720 656c 7365  rsion == '' else
+00003a30: 2027 556e 696e 7374 616c 6c27 290a 2020   'Uninstall').  
+00003a40: 2020 2020 2020 7365 6c66 2e64 6f63 756d        self.docum
+00003a50: 656e 7461 7469 6f6e 4275 7474 6f6e 2e73  entationButton.s
+00003a60: 6574 5669 7369 626c 6528 706c 7567 696e  etVisible(plugin
+00003a70: 2e64 6f63 756d 656e 7461 7469 6f6e 2021  .documentation !
+00003a80: 3d20 4e6f 6e65 290a 2020 2020 2020 2020  = None).        
+00003a90: 6966 2070 6c75 6769 6e2e 7665 7273 696f  if plugin.versio
+00003aa0: 6e20 3d3d 2027 273a 0a20 2020 2020 2020  n == '':.       
+00003ab0: 2020 2020 2070 6c75 6769 6e2e 6c69 7374       plugin.list
+00003ac0: 5769 6467 6574 2e73 6574 4963 6f6e 2851  Widget.setIcon(Q
+00003ad0: 7447 7569 2e51 4963 6f6e 2829 290a 2020  tGui.QIcon()).  
+00003ae0: 2020 2020 2020 656c 6966 2070 6172 7365        elif parse
+00003af0: 5f76 6572 7369 6f6e 2870 6c75 6769 6e2e  _version(plugin.
+00003b00: 7665 7273 696f 6e29 203c 2070 6172 7365  version) < parse
+00003b10: 5f76 6572 7369 6f6e 2870 6c75 6769 6e2e  _version(plugin.
+00003b20: 6c61 7465 7374 5f76 6572 7369 6f6e 293a  latest_version):
+00003b30: 0a20 2020 2020 2020 2020 2020 2070 6c75  .            plu
+00003b40: 6769 6e2e 6c69 7374 5769 6467 6574 2e73  gin.listWidget.s
+00003b50: 6574 4963 6f6e 2851 7447 7569 2e51 4963  etIcon(QtGui.QIc
+00003b60: 6f6e 2869 6d61 6765 5f70 6174 6828 2765  on(image_path('e
+00003b70: 7863 6c61 6d61 7469 6f6e 2e70 6e67 2729  xclamation.png')
+00003b80: 2929 0a20 2020 2020 2020 2065 6c73 653a  )).        else:
+00003b90: 0a20 2020 2020 2020 2020 2020 2070 6c75  .            plu
+00003ba0: 6769 6e2e 6c69 7374 5769 6467 6574 2e73  gin.listWidget.s
+00003bb0: 6574 4963 6f6e 2851 7447 7569 2e51 4963  etIcon(QtGui.QIc
+00003bc0: 6f6e 2869 6d61 6765 5f70 6174 6828 2763  on(image_path('c
+00003bd0: 6865 636b 2e70 6e67 2729 2929 0a0a 2020  heck.png')))..  
+00003be0: 2020 2020 2020 7365 6c66 2e69 6e66 6f4c        self.infoL
+00003bf0: 6162 656c 2e73 6574 5465 7874 2869 6e66  abel.setText(inf
+00003c00: 6f29 0a20 2020 2020 2020 2073 656c 662e  o).        self.
+00003c10: 6465 7363 7269 7074 696f 6e4c 6162 656c  descriptionLabel
+00003c20: 2e73 6574 4874 6d6c 2870 6c75 6769 6e2e  .setHtml(plugin.
+00003c30: 6465 7363 7269 7074 696f 6e29 0a20 2020  description).   
+00003c40: 2020 2020 2069 6620 706c 7567 696e 2e69       if plugin.i
+00003c50: 6e66 6f5f 7572 6c20 3d3d 204e 6f6e 653a  nfo_url == None:
+00003c60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003c70: 662e 6c6f 6164 5f6f 6e6c 696e 655f 706c  f.load_online_pl
+00003c80: 7567 696e 2870 6c75 6769 6e2e 6e61 6d65  ugin(plugin.name
+00003c90: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
+00003ca0: 7468 6f64 0a20 2020 2064 6566 206c 6f63  thod.    def loc
+00003cb0: 616c 5f70 6c75 6769 6e5f 7061 7468 7328  al_plugin_paths(
+00003cc0: 293a 0a20 2020 2020 2020 2070 6174 6873  ):.        paths
+00003cd0: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+00003ce0: 7220 7061 7468 2069 6e20 676c 6f62 286f  r path in glob(o
+00003cf0: 732e 7061 7468 2e6a 6f69 6e28 706c 7567  s.path.join(plug
+00003d00: 696e 5f64 6972 2c20 222a 2229 293a 0a20  in_dir, "*")):. 
+00003d10: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+00003d20: 2e70 6174 682e 6973 6469 7228 7061 7468  .path.isdir(path
+00003d30: 2920 616e 6420 6f73 2e70 6174 682e 6578  ) and os.path.ex
+00003d40: 6973 7473 286f 732e 7061 7468 2e6a 6f69  ists(os.path.joi
+00003d50: 6e28 7061 7468 2c20 2769 6e66 6f2e 786d  n(path, 'info.xm
+00003d60: 6c27 2929 3a0a 2020 2020 2020 2020 2020  l')):.          
+00003d70: 2020 2020 2020 7061 7468 732e 6170 7065        paths.appe
+00003d80: 6e64 2870 6174 6829 0a20 2020 2020 2020  nd(path).       
+00003d90: 2072 6574 7572 6e20 7061 7468 730a 0a20   return paths.. 
+00003da0: 2020 2064 6566 2063 6c65 6172 4c69 7374     def clearList
+00003db0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00003dc0: 7768 696c 6520 7365 6c66 2e70 6c75 6769  while self.plugi
+00003dd0: 6e4c 6973 742e 636f 756e 7428 2920 3e20  nList.count() > 
+00003de0: 303a 0a20 2020 2020 2020 2020 2020 2073  0:.            s
+00003df0: 656c 662e 706c 7567 696e 4c69 7374 2e74  elf.pluginList.t
+00003e00: 616b 6549 7465 6d28 3029 0a0a 2020 2020  akeItem(0)..    
+00003e10: 6465 6620 7368 6f77 506c 7567 696e 7328  def showPlugins(
+00003e20: 7365 6c66 2c20 7365 6172 6368 5f73 7472  self, search_str
+00003e30: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00003e40: 6672 6f6d 2070 6b67 5f72 6573 6f75 7263  from pkg_resourc
+00003e50: 6573 2069 6d70 6f72 7420 7061 7273 655f  es import parse_
+00003e60: 7665 7273 696f 6e0a 2020 2020 2020 2020  version.        
+00003e70: 7365 6c66 2e63 6c65 6172 4c69 7374 2829  self.clearList()
+00003e80: 0a20 2020 2020 2020 2069 6620 7365 6172  .        if sear
+00003e90: 6368 5f73 7472 203d 3d20 4e6f 6e65 206f  ch_str == None o
+00003ea0: 7220 6c65 6e28 7365 6172 6368 5f73 7472  r len(search_str
+00003eb0: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
+00003ec0: 2020 2020 6e61 6d65 7320 3d20 736f 7274      names = sort
+00003ed0: 6564 2873 656c 662e 706c 7567 696e 732e  ed(self.plugins.
+00003ee0: 6b65 7973 2829 290a 2020 2020 2020 2020  keys()).        
+00003ef0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00003f00: 2020 6465 6620 736f 7274 5f66 756e 6328    def sort_func(
+00003f10: 6e61 6d65 293a 0a20 2020 2020 2020 2020  name):.         
+00003f20: 2020 2020 2020 206e 616d 6520 3d20 7374         name = st
+00003f30: 7228 6e61 6d65 290a 2020 2020 2020 2020  r(name).        
+00003f40: 2020 2020 2020 2020 7265 7475 726e 202d          return -
+00003f50: 6469 6666 6c69 622e 5365 7175 656e 6365  difflib.Sequence
+00003f60: 4d61 7463 6865 7228 4e6f 6e65 2c20 6e61  Matcher(None, na
+00003f70: 6d65 2e6c 6f77 6572 2829 2c20 7365 6172  me.lower(), sear
+00003f80: 6368 5f73 7472 2e6c 6f77 6572 2829 292e  ch_str.lower()).
+00003f90: 7261 7469 6f28 2920 2d20 696e 7428 7365  ratio() - int(se
+00003fa0: 6172 6368 5f73 7472 2e6c 6f77 6572 2829  arch_str.lower()
+00003fb0: 2069 6e20 6e61 6d65 2e6c 6f77 6572 2829   in name.lower()
+00003fc0: 290a 2020 2020 2020 2020 2020 2020 6420  ).            d 
+00003fd0: 3d20 7b6e 616d 653a 2073 6f72 745f 6675  = {name: sort_fu
+00003fe0: 6e63 286e 616d 6529 2066 6f72 206e 616d  nc(name) for nam
+00003ff0: 6520 696e 2073 656c 662e 706c 7567 696e  e in self.plugin
+00004000: 732e 6b65 7973 2829 2069 6620 736f 7274  s.keys() if sort
+00004010: 5f66 756e 6328 6e61 6d65 2920 213d 2030  _func(name) != 0
+00004020: 7d0a 2020 2020 2020 2020 2020 2020 6e61  }.            na
+00004030: 6d65 7320 3d20 736f 7274 6564 2864 2e6b  mes = sorted(d.k
+00004040: 6579 7328 292c 206b 6579 3d6c 616d 6264  eys(), key=lambd
+00004050: 6120 613a 2064 5b61 5d29 0a20 2020 2020  a a: d[a]).     
+00004060: 2020 2066 6f72 206e 616d 6520 696e 206e     for name in n
+00004070: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
+00004080: 2020 706c 7567 203d 2050 6c75 6769 6e4d    plug = PluginM
+00004090: 616e 6167 6572 2e70 6c75 6769 6e73 5b6e  anager.plugins[n
+000040a0: 616d 655d 0a20 2020 2020 2020 2020 2020  ame].           
+000040b0: 2069 6620 706c 7567 2e76 6572 7369 6f6e   if plug.version
+000040c0: 203d 3d20 2727 3a0a 2020 2020 2020 2020   == '':.        
+000040d0: 2020 2020 2020 2020 706c 7567 2e6c 6973          plug.lis
+000040e0: 7457 6964 6765 742e 7365 7449 636f 6e28  tWidget.setIcon(
+000040f0: 5174 4775 692e 5149 636f 6e28 2929 0a20  QtGui.QIcon()). 
+00004100: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00004110: 7061 7273 655f 7665 7273 696f 6e28 706c  parse_version(pl
+00004120: 7567 2e76 6572 7369 6f6e 2920 3c20 7061  ug.version) < pa
+00004130: 7273 655f 7665 7273 696f 6e28 706c 7567  rse_version(plug
+00004140: 2e6c 6174 6573 745f 7665 7273 696f 6e29  .latest_version)
+00004150: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004160: 2020 706c 7567 2e6c 6973 7457 6964 6765    plug.listWidge
+00004170: 742e 7365 7449 636f 6e28 5174 4775 692e  t.setIcon(QtGui.
+00004180: 5149 636f 6e28 696d 6167 655f 7061 7468  QIcon(image_path
+00004190: 2827 6578 636c 616d 6174 696f 6e2e 706e  ('exclamation.pn
+000041a0: 6727 2929 290a 2020 2020 2020 2020 2020  g'))).          
+000041b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000041c0: 2020 2020 2020 2020 706c 7567 2e6c 6973          plug.lis
+000041d0: 7457 6964 6765 742e 7365 7449 636f 6e28  tWidget.setIcon(
+000041e0: 5174 4775 692e 5149 636f 6e28 696d 6167  QtGui.QIcon(imag
+000041f0: 655f 7061 7468 2827 6368 6563 6b2e 706e  e_path('check.pn
+00004200: 6727 2929 290a 2020 2020 2020 2020 2020  g'))).          
+00004210: 2020 7365 6c66 2e70 6c75 6769 6e4c 6973    self.pluginLis
+00004220: 742e 6164 6449 7465 6d28 706c 7567 2e6c  t.addItem(plug.l
+00004230: 6973 7457 6964 6765 7429 0a0a 2020 2020  istWidget)..    
+00004240: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00004250: 2020 6465 6620 7265 6d6f 7665 506c 7567    def removePlug
+00004260: 696e 2870 6c75 6769 6e29 3a0a 2020 2020  in(plugin):.    
+00004270: 2020 2020 506c 7567 696e 4d61 6e61 6765      PluginManage
+00004280: 722e 6775 692e 7374 6174 7573 4261 722e  r.gui.statusBar.
+00004290: 7368 6f77 4d65 7373 6167 6528 2255 6e69  showMessage("Uni
+000042a0: 6e73 7461 6c6c 696e 6720 7b7d 222e 666f  nstalling {}".fo
+000042b0: 726d 6174 2870 6c75 6769 6e2e 6e61 6d65  rmat(plugin.name
+000042c0: 2929 0a20 2020 2020 2020 2069 6620 6f73  )).        if os
+000042d0: 2e70 6174 682e 6973 6469 7228 6f73 2e70  .path.isdir(os.p
+000042e0: 6174 682e 6a6f 696e 2870 6c75 6769 6e5f  ath.join(plugin_
+000042f0: 6469 722c 2070 6c75 6769 6e2e 6469 7265  dir, plugin.dire
+00004300: 6374 6f72 792c 2027 2e67 6974 2729 293a  ctory, '.git')):
+00004310: 0a20 2020 2020 2020 2020 2020 2067 2e61  .            g.a
+00004320: 6c65 7274 2822 5468 6973 2070 6c75 6769  lert("This plugi
+00004330: 6e27 7320 6469 7265 6374 6f72 7920 6973  n's directory is
+00004340: 206d 616e 6167 6564 2062 7920 6769 742e   managed by git.
+00004350: 2054 6f20 7265 6d6f 7665 2c20 6d61 6e75   To remove, manu
+00004360: 616c 6c79 2064 656c 6574 6520 7468 6520  ally delete the 
+00004370: 6469 7265 6374 6f72 7922 290a 2020 2020  directory").    
+00004380: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00004390: 616c 7365 0a20 2020 2020 2020 2074 7279  alse.        try
+000043a0: 3a0a 2020 2020 2020 2020 2020 2020 7368  :.            sh
+000043b0: 7574 696c 2e72 6d74 7265 6528 6f73 2e70  util.rmtree(os.p
+000043c0: 6174 682e 6a6f 696e 2870 6c75 6769 6e5f  ath.join(plugin_
+000043d0: 6469 722c 2070 6c75 6769 6e2e 6469 7265  dir, plugin.dire
+000043e0: 6374 6f72 7929 2c20 6967 6e6f 7265 5f65  ctory), ignore_e
+000043f0: 7272 6f72 733d 5472 7565 290a 2020 2020  rrors=True).    
+00004400: 2020 2020 2020 2020 706c 7567 696e 2e76          plugin.v
+00004410: 6572 7369 6f6e 203d 2027 270a 2020 2020  ersion = ''.    
+00004420: 2020 2020 2020 2020 706c 7567 696e 2e6d          plugin.m
+00004430: 656e 7520 3d20 4e6f 6e65 0a20 2020 2020  enu = None.     
+00004440: 2020 2020 2020 2070 6c75 6769 6e2e 6c69         plugin.li
+00004450: 7374 5769 6467 6574 2e73 6574 4963 6f6e  stWidget.setIcon
+00004460: 2851 7447 7569 2e51 4963 6f6e 2829 290a  (QtGui.QIcon()).
+00004470: 2020 2020 2020 2020 2020 2020 506c 7567              Plug
+00004480: 696e 4d61 6e61 6765 722e 6775 692e 7374  inManager.gui.st
+00004490: 6174 7573 4261 722e 7368 6f77 4d65 7373  atusBar.showMess
+000044a0: 6167 6528 277b 7d20 7375 6363 6573 7366  age('{} successf
+000044b0: 756c 6c79 2075 6e69 6e73 7461 6c6c 6564  ully uninstalled
+000044c0: 272e 666f 726d 6174 2870 6c75 6769 6e2e  '.format(plugin.
+000044d0: 6e61 6d65 2929 0a20 2020 2020 2020 2065  name)).        e
+000044e0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+000044f0: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00004500: 2020 672e 616c 6572 7428 7469 746c 653d    g.alert(title=
+00004510: 2250 6c75 6769 6e20 556e 696e 7374 616c  "Plugin Uninstal
+00004520: 6c20 4661 696c 6564 222c 206d 7367 3d22  l Failed", msg="
+00004530: 556e 6162 6c65 2074 6f20 7265 6d6f 7665  Unable to remove
+00004540: 2074 6865 2066 6f6c 6465 7220 6174 2025   the folder at %
+00004550: 735c 6e25 735c 6e44 656c 6574 6520 7468  s\n%s\nDelete th
+00004560: 6520 666f 6c64 6572 206d 616e 7561 6c6c  e folder manuall
+00004570: 7920 746f 2075 6e69 6e73 7461 6c6c 2074  y to uninstall t
+00004580: 6865 2070 6c75 6769 6e22 2025 2028 706c  he plugin" % (pl
+00004590: 7567 696e 2e6e 616d 652c 2065 292c 2069  ugin.name, e), i
+000045a0: 636f 6e3d 5174 5769 6467 6574 732e 514d  con=QtWidgets.QM
+000045b0: 6573 7361 6765 426f 782e 5761 726e 696e  essageBox.Warnin
+000045c0: 6729 0a0a 2020 2020 2020 2020 506c 7567  g)..        Plug
+000045d0: 696e 4d61 6e61 6765 722e 6775 692e 706c  inManager.gui.pl
+000045e0: 7567 696e 5365 6c65 6374 6564 2870 6c75  uginSelected(plu
+000045f0: 6769 6e2e 6c69 7374 5769 6467 6574 290a  gin.listWidget).
+00004600: 2020 2020 2020 2020 706c 7567 696e 2e69          plugin.i
+00004610: 6e73 7461 6c6c 6564 203d 2046 616c 7365  nstalled = False
+00004620: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00004630: 686f 640a 2020 2020 6465 6620 646f 776e  hod.    def down
+00004640: 6c6f 6164 506c 7567 696e 2870 6c75 6769  loadPlugin(plugi
+00004650: 6e29 3a0a 2020 2020 2020 2020 506c 7567  n):.        Plug
+00004660: 696e 4d61 6e61 6765 722e 6775 692e 7374  inManager.gui.st
+00004670: 6174 7573 4261 722e 7368 6f77 4d65 7373  atusBar.showMess
+00004680: 6167 6528 2249 6e73 7461 6c6c 696e 6720  age("Installing 
+00004690: 706c 7567 696e 2229 0a20 2020 2020 2020  plugin").       
+000046a0: 2069 6620 6973 696e 7374 616e 6365 2870   if isinstance(p
+000046b0: 6c75 6769 6e2c 2073 7472 293a 0a20 2020  lugin, str):.   
+000046c0: 2020 2020 2020 2020 2069 6620 706c 7567           if plug
+000046d0: 696e 2069 6e20 506c 7567 696e 4d61 6e61  in in PluginMana
+000046e0: 6765 722e 706c 7567 696e 733a 0a20 2020  ger.plugins:.   
+000046f0: 2020 2020 2020 2020 2020 2020 2070 6c75               plu
+00004700: 6769 6e20 3d20 506c 7567 696e 4d61 6e61  gin = PluginMana
+00004710: 6765 722e 706c 7567 696e 735b 706c 7567  ger.plugins[plug
+00004720: 696e 5d0a 2020 2020 2020 2020 2020 2020  in].            
+00004730: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00004740: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00004750: 2020 2020 2069 6620 706c 7567 696e 2e75       if plugin.u
+00004760: 726c 2069 7320 4e6f 6e65 3a0a 2020 2020  rl is None:.    
+00004770: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00004780: 2020 2020 2020 2066 6169 6c65 6420 3d20         failed = 
+00004790: 5b5d 0a20 2020 2020 2020 2064 6973 7473  [].        dists
+000047a0: 203d 205b 612e 7072 6f6a 6563 745f 6e61   = [a.project_na
+000047b0: 6d65 2066 6f72 2061 2069 6e20 706b 675f  me for a in pkg_
+000047c0: 7265 736f 7572 6365 732e 776f 726b 696e  resources.workin
+000047d0: 675f 7365 745d 0a20 2020 2020 2020 2050  g_set].        P
+000047e0: 6c75 6769 6e4d 616e 6167 6572 2e67 7569  luginManager.gui
+000047f0: 2e73 7461 7475 7342 6172 2e73 686f 774d  .statusBar.showM
+00004800: 6573 7361 6765 2822 496e 7374 616c 6c69  essage("Installi
+00004810: 6e67 2064 6570 656e 6465 6e63 6965 7320  ng dependencies 
+00004820: 666f 7220 2573 2220 2520 706c 7567 696e  for %s" % plugin
+00004830: 2e6e 616d 6529 0a20 2020 2020 2020 2066  .name).        f
+00004840: 6f72 2070 6c20 696e 2070 6c75 6769 6e2e  or pl in plugin.
+00004850: 6465 7065 6e64 656e 6369 6573 3a0a 2020  dependencies:.  
+00004860: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00004870: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004880: 6620 706c 2069 6e20 6469 7374 733a 0a20  f pl in dists:. 
+00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048a0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+000048b0: 2020 2020 2020 2020 2020 2020 6120 3d20              a = 
+000048c0: 5f5f 696d 706f 7274 5f5f 2870 6c29 0a20  __import__(pl). 
+000048d0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+000048e0: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
+000048f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004900: 6573 203d 2073 7562 7072 6f63 6573 732e  es = subprocess.
+00004910: 6361 6c6c 285b 7379 732e 6578 6563 7574  call([sys.execut
+00004920: 6162 6c65 2c20 272d 6d27 2c20 2770 6970  able, '-m', 'pip
+00004930: 272c 2027 696e 7374 616c 6c27 2c20 277b  ', 'install', '{
+00004940: 7d27 2e66 6f72 6d61 7428 706c 292c 2027  }'.format(pl), '
+00004950: 2d2d 6e6f 2d63 6163 6865 2d64 6972 275d  --no-cache-dir']
+00004960: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004970: 2020 6966 2072 6573 2021 3d20 303a 0a20    if res != 0:. 
+00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004990: 2020 2066 6169 6c65 642e 6170 7065 6e64     failed.append
+000049a0: 2870 6c29 0a20 2020 2020 2020 2069 6620  (pl).        if 
+000049b0: 6661 696c 6564 3a0a 2020 2020 2020 2020  failed:.        
+000049c0: 2020 2020 6966 2070 6c61 7466 6f72 6d2e      if platform.
+000049d0: 7379 7374 656d 2829 203d 3d20 2757 696e  system() == 'Win
+000049e0: 646f 7773 273a 0a20 2020 2020 2020 2020  dows':.         
+000049f0: 2020 2020 2020 2051 7447 7569 2e51 4465         QtGui.QDe
+00004a00: 736b 746f 7053 6572 7669 6365 732e 6f70  sktopServices.op
+00004a10: 656e 5572 6c28 5174 436f 7265 2e51 5572  enUrl(QtCore.QUr
+00004a20: 6c28 2268 7474 703a 2f2f 7777 772e 6c66  l("http://www.lf
+00004a30: 642e 7563 692e 6564 752f 7e67 6f68 6c6b  d.uci.edu/~gohlk
+00004a40: 652f 7079 7468 6f6e 6c69 6273 2f23 222b  e/pythonlibs/#"+
+00004a50: 706c 2929 0a20 2020 2020 2020 2020 2020  pl)).           
+00004a60: 2020 2020 2076 203d 2073 7472 2873 7973       v = str(sys
+00004a70: 2e76 6572 7369 6f6e 5f69 6e66 6f2e 6d61  .version_info.ma
+00004a80: 6a6f 7229 202b 2073 7472 2873 7973 2e76  jor) + str(sys.v
+00004a90: 6572 7369 6f6e 5f69 6e66 6f2e 6d69 6e6f  ersion_info.mino
+00004aa0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+00004ab0: 2020 2069 6620 706c 6174 666f 726d 2e61     if platform.a
+00004ac0: 7263 6869 7465 6374 7572 6528 295b 305d  rchitecture()[0]
+00004ad0: 3d3d 2736 3462 6974 273a 0a20 2020 2020  =='64bit':.     
+00004ae0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00004af0: 7263 6820 3d20 275f 616d 6436 3427 0a20  rch = '_amd64'. 
+00004b00: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00004b10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00004b20: 2020 2020 2020 2020 2061 7263 6820 3d20           arch = 
+00004b30: 2733 3227 0a20 2020 2020 2020 2020 2020  '32'.           
+00004b40: 2020 2020 2067 2e61 6c65 7274 2822 2222       g.alert("""
+00004b50: 4661 696c 6564 2074 6f20 696e 7374 616c  Failed to instal
+00004b60: 6c20 7468 6520 6465 7065 6e64 656e 6379  l the dependency
+00004b70: 2027 7b30 7d27 2e20 596f 7520 6d75 7374   '{0}'. You must
+00004b80: 2069 6e73 7461 6c6c 207b 307d 206d 616e   install {0} man
+00004b90: 7561 6c6c 792e 0a44 6f77 6e6c 6f61 6420  ually..Download 
+00004ba0: 7b30 7d2d 782d 6370 7b31 7d2d 6370 7b31  {0}-x-cp{1}-cp{1
+00004bb0: 7d6d 2d77 696e 7b32 7d2e 7768 6c2e 0a0a  }m-win{2}.whl...
+00004bc0: 4f6e 6365 2074 6865 2077 6865 656c 2069  Once the wheel i
+00004bd0: 7320 646f 776e 6c6f 6164 6564 2c20 6472  s downloaded, dr
+00004be0: 6167 2069 7420 696e 746f 2066 6c69 6b61  ag it into flika
+00004bf0: 2074 6f20 696e 7374 616c 6c2e 0a0a 5468   to install...Th
+00004c00: 656e 2074 7279 2069 6e73 7461 6c6c 696e  en try installin
+00004c10: 6720 7468 6520 706c 7567 696e 2061 6761  g the plugin aga
+00004c20: 696e 2e22 2222 2e66 6f72 6d61 7428 706c  in.""".format(pl
+00004c30: 2c20 762c 2061 7263 6829 290a 2020 2020  , v, arch)).    
+00004c40: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00004c50: 2020 2020 2020 2020 2020 2020 2020 672e                g.
+00004c60: 616c 6572 7428 2246 6169 6c65 6420 746f  alert("Failed to
+00004c70: 2069 6e73 7461 6c6c 2064 6570 656e 6465   install depende
+00004c80: 6e63 6965 7320 666f 7220 7b7d 3a5c 6e7b  ncies for {}:\n{
+00004c90: 7d5c 6e59 6f75 206d 7573 7420 696e 7374  }\nYou must inst
+00004ca0: 616c 6c20 7468 656d 206f 6e20 796f 7572  all them on your
+00004cb0: 206f 776e 2062 6566 6f72 6520 696e 7374   own before inst
+00004cc0: 616c 6c69 6e67 2074 6869 7320 706c 7567  alling this plug
+00004cd0: 696e 2e22 2e66 6f72 6d61 7428 706c 7567  in.".format(plug
+00004ce0: 696e 2e6e 616d 652c 2027 2c20 272e 6a6f  in.name, ', '.jo
+00004cf0: 696e 2866 6169 6c65 6429 2929 0a0a 2020  in(failed)))..  
+00004d00: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00004d10: 0a0a 2020 2020 2020 2020 6966 206f 732e  ..        if os.
+00004d20: 7061 7468 2e65 7869 7374 7328 6f73 2e70  path.exists(os.p
+00004d30: 6174 682e 6a6f 696e 2870 6c75 6769 6e5f  ath.join(plugin_
+00004d40: 6469 722c 2070 6c75 6769 6e2e 6469 7265  dir, plugin.dire
+00004d50: 6374 6f72 7929 293a 0a20 2020 2020 2020  ctory)):.       
+00004d60: 2020 2020 2067 2e61 6c65 7274 2822 4120       g.alert("A 
+00004d70: 666f 6c64 6572 2077 6974 6820 6e61 6d65  folder with name
+00004d80: 207b 7d20 616c 7265 6164 7920 6578 6973   {} already exis
+00004d90: 7473 2069 6e20 7468 6520 706c 7567 696e  ts in the plugin
+00004da0: 7320 6469 7265 6374 6f72 792e 2050 6c65  s directory. Ple
+00004db0: 6173 6520 7265 6d6f 7665 2069 7420 746f  ase remove it to
+00004dc0: 2069 6e73 7461 6c6c 2074 6869 7320 706c   install this pl
+00004dd0: 7567 696e 2122 2e66 6f72 6d61 7428 706c  ugin!".format(pl
+00004de0: 7567 696e 2e64 6972 6563 746f 7279 2929  ugin.directory))
+00004df0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00004e00: 7572 6e0a 0a20 2020 2020 2020 2050 6c75  urn..        Plu
+00004e10: 6769 6e4d 616e 6167 6572 2e67 7569 2e73  ginManager.gui.s
+00004e20: 7461 7475 7342 6172 2e73 686f 774d 6573  tatusBar.showMes
+00004e30: 7361 6765 2827 4f70 656e 696e 6720 2573  sage('Opening %s
+00004e40: 2720 2520 706c 7567 696e 2e75 726c 290a  ' % plugin.url).
+00004e50: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00004e60: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+00004e70: 7572 6c6f 7065 6e28 706c 7567 696e 2e75  urlopen(plugin.u
+00004e80: 726c 292e 7265 6164 2829 0a20 2020 2020  rl).read().     
+00004e90: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+00004ea0: 2020 2020 2020 2067 2e61 6c65 7274 2874         g.alert(t
+00004eb0: 6974 6c65 3d22 446f 776e 6c6f 6164 2045  itle="Download E
+00004ec0: 7272 6f72 222c 206d 7367 3d22 4661 696c  rror", msg="Fail
+00004ed0: 6564 2074 6f20 636f 6e6e 6563 7420 746f  ed to connect to
+00004ee0: 2025 7320 746f 2069 6e73 7461 6c6c 2074   %s to install t
+00004ef0: 6865 2025 7320 666c 696b 6120 506c 7567  he %s flika Plug
+00004f00: 696e 2e20 4368 6563 6b20 796f 7572 2069  in. Check your i
+00004f10: 6e74 6572 6e65 7420 636f 6e6e 6563 7469  nternet connecti
+00004f20: 6f6e 2061 6e64 2074 7279 2061 6761 696e  on and try again
+00004f30: 2c20 6f72 2064 6f77 6e6c 6f61 6420 7468  , or download th
+00004f40: 6520 706c 7567 696e 206d 616e 7561 6c6c  e plugin manuall
+00004f50: 792e 2220 2520 2850 6c75 6769 6e4d 616e  y." % (PluginMan
+00004f60: 6167 6572 2e67 7569 2e6c 696e 6b2c 2070  ager.gui.link, p
+00004f70: 6c75 6769 6e2e 6e61 6d65 292c 2069 636f  lugin.name), ico
+00004f80: 6e3d 5174 5769 6467 6574 732e 514d 6573  n=QtWidgets.QMes
+00004f90: 7361 6765 426f 782e 5761 726e 696e 6729  sageBox.Warning)
+00004fa0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00004fb0: 7572 6e0a 0a20 2020 2020 2020 2074 7279  urn..        try
+00004fc0: 3a0a 0a20 2020 2020 2020 2020 2020 2077  :..            w
+00004fd0: 6974 6820 7465 6d70 6669 6c65 2e54 656d  ith tempfile.Tem
+00004fe0: 706f 7261 7279 4669 6c65 2829 2061 7320  poraryFile() as 
+00004ff0: 7466 3a0a 2020 2020 2020 2020 2020 2020  tf:.            
+00005000: 2020 2020 7466 2e77 7269 7465 2864 6174      tf.write(dat
+00005010: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+00005020: 2020 2074 662e 7365 656b 2830 290a 2020     tf.seek(0).  
+00005030: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00005040: 7468 207a 6970 6669 6c65 2e5a 6970 4669  th zipfile.ZipFi
+00005050: 6c65 2874 6629 2061 7320 7a3a 0a20 2020  le(tf) as z:.   
+00005060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005070: 2066 6f6c 6465 725f 6e61 6d65 203d 206f   folder_name = o
+00005080: 732e 7061 7468 2e64 6972 6e61 6d65 287a  s.path.dirname(z
+00005090: 2e6e 616d 656c 6973 7428 295b 305d 290a  .namelist()[0]).
+000050a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050b0: 2020 2020 7a2e 6578 7472 6163 7461 6c6c      z.extractall
+000050c0: 2870 6c75 6769 6e5f 6469 7229 0a0a 2020  (plugin_dir)..  
+000050d0: 2020 2020 2020 2020 2020 706c 7567 696e            plugin
+000050e0: 203d 2050 6c75 6769 6e4d 616e 6167 6572   = PluginManager
+000050f0: 2e70 6c75 6769 6e73 5b70 6c75 6769 6e2e  .plugins[plugin.
+00005100: 6e61 6d65 5d0a 2020 2020 2020 2020 2020  name].          
+00005110: 2020 6469 7265 6374 6f72 7920 3d20 6f73    directory = os
+00005120: 2e70 6174 682e 6a6f 696e 2870 6c75 6769  .path.join(plugi
+00005130: 6e5f 6469 722c 2070 6c75 6769 6e2e 6469  n_dir, plugin.di
+00005140: 7265 6374 6f72 7929 0a20 2020 2020 2020  rectory).       
+00005150: 2020 2020 206f 732e 7265 6e61 6d65 286f       os.rename(o
+00005160: 732e 7061 7468 2e6a 6f69 6e28 706c 7567  s.path.join(plug
+00005170: 696e 5f64 6972 2c20 666f 6c64 6572 5f6e  in_dir, folder_n
+00005180: 616d 6529 2c20 6469 7265 6374 6f72 7929  ame), directory)
+00005190: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000051a0: 2850 6572 6d69 7373 696f 6e45 7272 6f72  (PermissionError
+000051b0: 2c20 4578 6365 7074 696f 6e29 2061 7320  , Exception) as 
+000051c0: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+000051d0: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
+000051e0: 2866 6f6c 6465 725f 6e61 6d65 293a 0a20  (folder_name):. 
+000051f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005200: 6875 7469 6c2e 726d 7472 6565 2866 6f6c  hutil.rmtree(fol
+00005210: 6465 725f 6e61 6d65 290a 2020 2020 2020  der_name).      
+00005220: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00005230: 6e63 6528 652c 2050 6572 6d69 7373 696f  nce(e, Permissio
+00005240: 6e45 7272 6f72 293a 0a20 2020 2020 2020  nError):.       
+00005250: 2020 2020 2020 2020 2067 2e61 6c65 7274           g.alert
+00005260: 2822 556e 6162 6c65 2074 6f20 646f 776e  ("Unable to down
+00005270: 6c6f 6164 2070 6c75 6769 6e20 746f 207b  load plugin to {
+00005280: 7d2e 2052 6572 756e 2066 6c69 6b61 2061  }. Rerun flika a
+00005290: 7320 6164 6d69 6e69 7374 7261 746f 7220  s administrator 
+000052a0: 616e 6420 646f 776e 6c6f 6164 2074 6865  and download the
+000052b0: 2070 6c75 6769 6e20 6167 6169 6e2e 222e   plugin again.".
+000052c0: 666f 726d 6174 2870 6c75 6769 6e2e 6e61  format(plugin.na
+000052d0: 6d65 292c 2074 6974 6c65 3d27 5065 726d  me), title='Perm
+000052e0: 6973 7369 6f6e 2044 656e 6965 6427 290a  ission Denied').
+000052f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00005300: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005310: 2020 672e 616c 6572 7428 2245 7272 6f72    g.alert("Error
+00005320: 206f 6363 7572 7265 6420 7768 696c 6520   occurred while 
+00005330: 696e 7374 616c 6c69 6e67 207b 7d2e 5c6e  installing {}.\n
+00005340: 5c74 7b7d 222e 666f 726d 6174 2870 6c75  \t{}".format(plu
+00005350: 6769 6e2e 6e61 6d65 2c20 6529 2c20 7469  gin.name, e), ti
+00005360: 746c 653d 2750 6c75 6769 6e20 496e 7374  tle='Plugin Inst
+00005370: 616c 6c20 4661 696c 6564 2729 2020 2020  all Failed')    
+00005380: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+00005390: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000053a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000053b0: 2020 506c 7567 696e 4d61 6e61 6765 722e    PluginManager.
+000053c0: 6775 692e 7374 6174 7573 4261 722e 7368  gui.statusBar.sh
+000053d0: 6f77 4d65 7373 6167 6528 2745 7874 7261  owMessage('Extra
+000053e0: 6374 696e 6720 2025 7327 2025 2070 6c75  cting  %s' % plu
+000053f0: 6769 6e2e 6e61 6d65 290a 2020 2020 2020  gin.name).      
+00005400: 2020 706c 7567 696e 2e76 6572 7369 6f6e    plugin.version
+00005410: 203d 2070 6c75 6769 6e2e 6c61 7465 7374   = plugin.latest
+00005420: 5f76 6572 7369 6f6e 0a20 2020 2020 2020  _version.       
+00005430: 2070 6c75 6769 6e2e 6c69 7374 5769 6467   plugin.listWidg
+00005440: 6574 2e73 6574 4963 6f6e 2851 7447 7569  et.setIcon(QtGui
+00005450: 2e51 4963 6f6e 2869 6d61 6765 5f70 6174  .QIcon(image_pat
+00005460: 6828 2263 6865 636b 2e70 6e67 2229 2929  h("check.png")))
+00005470: 0a20 2020 2020 2020 2023 706c 7567 696e  .        #plugin
+00005480: 2e6d 656e 7520 3d20 6d61 6b65 5f70 6c75  .menu = make_plu
+00005490: 6769 6e5f 6d65 6e75 2870 6c75 6769 6e29  gin_menu(plugin)
+000054a0: 0a20 2020 2020 2020 2070 6c75 6769 6e2e  .        plugin.
+000054b0: 6d65 6e75 203d 2051 7457 6964 6765 7473  menu = QtWidgets
+000054c0: 2e51 4d65 6e75 2870 6c75 6769 6e2e 6e61  .QMenu(plugin.na
+000054d0: 6d65 290a 2020 2020 2020 2020 6275 696c  me).        buil
+000054e0: 645f 7375 626d 656e 7528 706c 7567 696e  d_submenu(plugin
+000054f0: 2e64 6972 6563 746f 7279 2c20 706c 7567  .directory, plug
+00005500: 696e 2e6d 656e 752c 2070 6c75 6769 6e2e  in.menu, plugin.
+00005510: 6d65 6e75 5f6c 6179 6f75 7429 0a20 2020  menu_layout).   
+00005520: 2020 2020 200a 2020 2020 2020 2020 506c       .        Pl
+00005530: 7567 696e 4d61 6e61 6765 722e 6775 692e  uginManager.gui.
+00005540: 7374 6174 7573 4261 722e 7368 6f77 4d65  statusBar.showMe
+00005550: 7373 6167 6528 2753 7563 6365 7373 6675  ssage('Successfu
+00005560: 6c6c 7920 696e 7374 616c 6c65 6420 7b7d  lly installed {}
+00005570: 2061 6e64 2069 745c 2773 2064 6570 656e   and it\'s depen
+00005580: 6465 6e63 6965 7327 2e66 6f72 6d61 7428  dencies'.format(
+00005590: 706c 7567 696e 2e6e 616d 6529 290a 2020  plugin.name)).  
+000055a0: 2020 2020 2020 506c 7567 696e 4d61 6e61        PluginMana
+000055b0: 6765 722e 6775 692e 706c 7567 696e 5365  ger.gui.pluginSe
+000055c0: 6c65 6374 6564 2870 6c75 6769 6e2e 6c69  lected(plugin.li
+000055d0: 7374 5769 6467 6574 290a 2020 2020 2020  stWidget).      
+000055e0: 2020 706c 7567 696e 2e69 6e73 7461 6c6c    plugin.install
+000055f0: 6564 203d 2054 7275 650a 0a0a 636c 6173  ed = True...clas
+00005600: 7320 4c6f 6164 5f4c 6f63 616c 5f50 6c75  s Load_Local_Plu
+00005610: 6769 6e73 5f54 6872 6561 6428 5174 436f  gins_Thread(QtCo
+00005620: 7265 2e51 5468 7265 6164 293a 0a20 2020  re.QThread):.   
+00005630: 2070 6c75 6769 6e73 5f64 6f6e 655f 7369   plugins_done_si
+00005640: 6720 3d20 5174 436f 7265 2e53 6967 6e61  g = QtCore.Signa
+00005650: 6c28 6469 6374 290a 2020 2020 6572 726f  l(dict).    erro
+00005660: 725f 6c6f 6164 696e 6720 3d20 5174 436f  r_loading = QtCo
+00005670: 7265 2e53 6967 6e61 6c28 7374 7229 0a20  re.Signal(str). 
+00005680: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00005690: 7365 6c66 293a 0a20 2020 2020 2020 2051  self):.        Q
+000056a0: 7443 6f72 652e 5154 6872 6561 642e 5f5f  tCore.QThread.__
+000056b0: 696e 6974 5f5f 2873 656c 6629 0a0a 2020  init__(self)..  
+000056c0: 2020 6465 6620 7275 6e28 7365 6c66 293a    def run(self):
+000056d0: 0a20 2020 2020 2020 2023 6c6f 6767 6572  .        #logger
+000056e0: 2e64 6562 7567 2822 5374 6172 7465 6420  .debug("Started 
+000056f0: 2761 7070 2e70 6c75 6769 6e5f 6d61 6e61  'app.plugin_mana
+00005700: 6765 722e 6c6f 6164 5f6c 6f63 616c 5f70  ger.load_local_p
+00005710: 6c75 6769 6e73 2722 290a 2020 2020 2020  lugins'").      
+00005720: 2020 706c 7567 696e 7320 3d20 7b6e 3a20    plugins = {n: 
+00005730: 506c 7567 696e 286e 2920 666f 7220 6e20  Plugin(n) for n 
+00005740: 696e 2070 6c75 6769 6e5f 6c69 7374 7d0a  in plugin_list}.
+00005750: 2020 2020 2020 2020 696e 7374 616c 6c65          installe
+00005760: 645f 706c 7567 696e 7320 3d20 7b7d 0a20  d_plugins = {}. 
+00005770: 2020 2020 2020 2066 6f72 2070 6c75 6769         for plugi
+00005780: 6e50 6174 6820 696e 2050 6c75 6769 6e4d  nPath in PluginM
+00005790: 616e 6167 6572 2e6c 6f63 616c 5f70 6c75  anager.local_plu
+000057a0: 6769 6e5f 7061 7468 7328 293a 0a20 2020  gin_paths():.   
+000057b0: 2020 2020 2020 2020 2070 203d 2050 6c75           p = Plu
+000057c0: 6769 6e28 290a 2020 2020 2020 2020 2020  gin().          
+000057d0: 2020 702e 6672 6f6d 4c6f 6361 6c28 706c    p.fromLocal(pl
+000057e0: 7567 696e 5061 7468 290a 2020 2020 2020  uginPath).      
+000057f0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00005800: 2020 2020 2020 2020 2020 2070 2e62 696e             p.bin
+00005810: 645f 6d65 6e75 5f61 6e64 5f6d 6574 686f  d_menu_and_metho
+00005820: 6473 2829 0a20 2020 2020 2020 2020 2020  ds().           
+00005830: 2020 2020 2069 6620 702e 6e61 6d65 206e       if p.name n
+00005840: 6f74 2069 6e20 706c 7567 696e 732e 6b65  ot in plugins.ke
+00005850: 7973 2829 206f 7220 702e 6e61 6d65 206e  ys() or p.name n
+00005860: 6f74 2069 6e20 696e 7374 616c 6c65 645f  ot in installed_
+00005870: 706c 7567 696e 732e 6b65 7973 2829 3a0a  plugins.keys():.
+00005880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005890: 2020 2020 702e 696e 7374 616c 6c65 6420      p.installed 
+000058a0: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
+000058b0: 2020 2020 2020 2020 2020 2070 6c75 6769             plugi
+000058c0: 6e73 5b70 2e6e 616d 655d 203d 2070 0a20  ns[p.name] = p. 
+000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058e0: 2020 2069 6e73 7461 6c6c 6564 5f70 6c75     installed_plu
+000058f0: 6769 6e73 5b70 2e6e 616d 655d 203d 2070  gins[p.name] = p
+00005900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005910: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00005920: 2020 2020 2020 2020 2020 2067 2e61 6c65             g.ale
+00005930: 7274 2827 436f 756c 6420 6e6f 7420 6c6f  rt('Could not lo
+00005940: 6164 2074 6865 2070 6c75 6769 6e20 7b7d  ad the plugin {}
+00005950: 2e20 5468 6572 6520 6973 2061 6c72 6561  . There is alrea
+00005960: 6479 2061 2070 6c75 6769 6e20 7769 7468  dy a plugin with
+00005970: 2074 6869 7320 7361 6d65 206e 616d 652e   this same name.
+00005980: 2043 6861 6e67 6520 7468 6520 706c 7567   Change the plug
+00005990: 696e 206e 616d 6520 696e 2074 6865 2069  in name in the i
+000059a0: 6e66 6f2e 786d 6c20 6669 6c65 272e 666f  nfo.xml file'.fo
+000059b0: 726d 6174 2870 2e6e 616d 6529 290a 2020  rmat(p.name)).  
+000059c0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+000059d0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+000059e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000059f0: 206d 7367 203d 2022 436f 756c 6420 6e6f   msg = "Could no
+00005a00: 7420 6c6f 6164 2070 6c75 6769 6e20 7b7d  t load plugin {}
+00005a10: 222e 666f 726d 6174 2870 6c75 6769 6e50  ".format(pluginP
+00005a20: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+00005a30: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
+00005a40: 6c6f 6164 696e 672e 656d 6974 286d 7367  loading.emit(msg
+00005a50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00005a60: 2020 2367 2e61 6c65 7274 286d 7367 290a    #g.alert(msg).
+00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a80: 6c6f 6767 6572 2e65 7272 6f72 286d 7367  logger.error(msg
+00005a90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00005aa0: 2020 6578 5f74 7970 652c 2065 782c 2074    ex_type, ex, t
+00005ab0: 6220 3d20 7379 732e 6578 635f 696e 666f  b = sys.exc_info
+00005ac0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00005ad0: 2020 2073 7973 2e65 7863 6570 7468 6f6f     sys.excepthoo
+00005ae0: 6b28 6578 5f74 7970 652c 2065 782c 2074  k(ex_type, ex, t
+00005af0: 6229 0a20 2020 2020 2020 2073 656c 662e  b).        self.
+00005b00: 706c 7567 696e 735f 646f 6e65 5f73 6967  plugins_done_sig
+00005b10: 2e65 6d69 7428 706c 7567 696e 7329 0a20  .emit(plugins). 
+00005b20: 2020 2020 2020 2023 6c6f 6767 6572 2e64         #logger.d
+00005b30: 6562 7567 2822 436f 6d70 6c65 7465 6420  ebug("Completed 
+00005b40: 2761 7070 2e70 6c75 6769 6e5f 6d61 6e61  'app.plugin_mana
+00005b50: 6765 722e 6c6f 6164 5f6c 6f63 616c 5f70  ger.load_local_p
+00005b60: 6c75 6769 6e73 2722 290a 0a23 2066 726f  lugins'")..# fro
+00005b70: 6d20 666c 696b 612e 6170 702e 706c 7567  m flika.app.plug
+00005b80: 696e 5f6d 616e 6167 6572 2069 6d70 6f72  in_manager impor
+00005b90: 7420 2a0a 0a0a 6c6f 6767 6572 2e64 6562  t *...logger.deb
+00005ba0: 7567 2822 436f 6d70 6c65 7465 6420 2772  ug("Completed 'r
+00005bb0: 6561 6469 6e67 2061 7070 2f70 6c75 6769  eading app/plugi
+00005bc0: 6e5f 6d61 6e61 6765 722e 7079 2722 29    n_manager.py'")
```

### Comparing `flika-0.2.9/flika/app/script_namespace.py` & `flika-0.3.0/flika/app/script_namespace.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-# -*- coding: utf-8 -*-
-from inspect import getmembers, ismodule
-import numpy as np
-import scipy
-import pyqtgraph as pg
-from .. import process
-from .. import global_vars as g
-from .. import window
-from ..roi import open_rois
-
-
-def getnamespace():
-    """
-    This function gets the namespace for the script interpreter.  It goes through all the modules in the 'process' package and loads all the objects defined in their '__all__' variables.
-    """
-    
-    d = {}
-    for name, mod in getmembers(process):
-        if ismodule(mod):
-            for func in mod.__all__:
-                d[func] = mod.__dict__[func]
-    d['g'] = g
-    d['np'] = np
-    d['scipy'] = scipy
-    d['pg'] = pg
-    d['plot'] = pg.plot
-    d['Window'] = window.Window
+# -*- coding: utf-8 -*-
+from inspect import getmembers, ismodule
+import numpy as np
+import scipy
+import pyqtgraph as pg
+from .. import process
+from .. import global_vars as g
+from .. import window
+from ..roi import open_rois
+
+
+def getnamespace():
+    """
+    This function gets the namespace for the script interpreter.  It goes through all the modules in the 'process' package and loads all the objects defined in their '__all__' variables.
+    """
+    
+    d = {}
+    for name, mod in getmembers(process):
+        if ismodule(mod):
+            for func in mod.__all__:
+                d[func] = mod.__dict__[func]
+    d['g'] = g
+    d['np'] = np
+    d['scipy'] = scipy
+    d['pg'] = pg
+    d['plot'] = pg.plot
+    d['Window'] = window.Window
+    d['open_rois'] = open_rois
     return d
```

### Comparing `flika-0.2.9/flika/app/syntax.py` & `flika-0.3.0/flika/app/syntax.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-import sys
-from qtpy import QtCore, QtGui
-
-def format(color, style=''):
-    """Return a QtGui.QTextCharFormat with the given attributes.
-    """
-    _color = QtGui.QColor()
-    _color.setNamedColor(color)
-
-    _format = QtGui.QTextCharFormat()
-    _format.setForeground(_color)
-    if 'bold' in style:
-        _format.setFontWeight(QtGui.QFont.Bold)
-    if 'italic' in style:
-        _format.setFontItalic(True)
-    return _format
-
-
-# Syntax styles that can be shared by all languages
-STYLES = {
-    'keyword': format('blue'),
-    'operator': format('red'),
-    'brace': format('black'),
-    'defclass': format('black', 'bold'),
-    'string': format('magenta'),
-    'string2': format('darkMagenta'),
-    'comment': format('darkGreen', 'italic'),
-    'self': format('black', 'italic'),
-    'numbers': format('brown'),
-}
-
-
-class PythonHighlighter (QtGui.QSyntaxHighlighter):
-    """Syntax highlighter for the Python language.
-    """
-    # Python keywords
-    keywords = [
-        'and', 'assert', 'break', 'class', 'continue', 'def',
-        'del', 'elif', 'else', 'except', 'exec', 'finally',
-        'for', 'from', 'global', 'if', 'import', 'in',
-        'is', 'lambda', 'not', 'or', 'pass', 'print',
-        'raise', 'return', 'try', 'while', 'yield',
-        'None', 'True', 'False',
-    ]
-
-    # Python operators
-    operators = [
-        '=',
-        # Comparison
-        '==', '!=', '<', '<=', '>', '>=',
-        # Arithmetic
-        '\+', '-', '\*', '/', '//', '\%', '\*\*',
-        # In-place
-        '\+=', '-=', '\*=', '/=', '\%=',
-        # Bitwise
-        '\^', '\|', '\&', '\~', '>>', '<<',
-    ]
-
-    # Python braces
-    braces = [
-        '\{', '\}', '\(', '\)', '\[', '\]',
-    ]
-    def __init__(self, document):
-        QtGui.QSyntaxHighlighter.__init__(self, document)
-
-        # Multi-line strings (expression, flag, style)
-        # FIXME: The triple-quotes in these two lines will mess up the
-        # syntax highlighting from this point onward
-        self.tri_single = (QtCore.QRegExp("'''"), 1, STYLES['string2'])
-        self.tri_double = (QtCore.QRegExp('"""'), 2, STYLES['string2'])
-
-        rules = []
-
-        # Keyword, operator, and brace rules
-        rules += [(r'\b%s\b' % w, 0, STYLES['keyword'])
-            for w in PythonHighlighter.keywords]
-        rules += [(r'%s' % o, 0, STYLES['operator'])
-            for o in PythonHighlighter.operators]
-        rules += [(r'%s' % b, 0, STYLES['brace'])
-            for b in PythonHighlighter.braces]
-
-        # All other rules
-        rules += [
-            # 'self'
-            (r'\bself\b', 0, STYLES['self']),
-
-            # Double-quoted string, possibly containing escape sequences
-            (r'"[^"\\]*(\\.[^"\\]*)*"', 0, STYLES['string']),
-            # Single-quoted string, possibly containing escape sequences
-            (r"'[^'\\]*(\\.[^'\\]*)*'", 0, STYLES['string']),
-
-            # 'def' followed by an identifier
-            (r'\bdef\b\s*(\w+)', 1, STYLES['defclass']),
-            # 'class' followed by an identifier
-            (r'\bclass\b\s*(\w+)', 1, STYLES['defclass']),
-
-            # From '#' until a newline
-            (r'#[^\n]*', 0, STYLES['comment']),
-
-            # Numeric literals
-            (r'\b[+-]?[0-9]+[lL]?\b', 0, STYLES['numbers']),
-            (r'\b[+-]?0[xX][0-9A-Fa-f]+[lL]?\b', 0, STYLES['numbers']),
-            (r'\b[+-]?[0-9]+(?:\.[0-9]+)?(?:[eE][+-]?[0-9]+)?\b', 0, STYLES['numbers']),
-        ]
-
-        # Build a QtCore.QRegExp for each pattern
-        self.rules = [(QtCore.QRegExp(pat), index, fmt)
-            for (pat, index, fmt) in rules]
-
-
-    def highlightBlock(self, text):
-        """Apply syntax highlighting to the given block of text.
-        """
-        # Do other syntax formatting
-        for expression, nth, format in self.rules:
-            index = expression.indexIn(text, 0)
-
-            while index >= 0:
-                # We actually want the index of the nth match
-                index = expression.pos(nth)
-                length = len(expression.cap(nth))
-                self.setFormat(index, length, format)
-                index = expression.indexIn(text, index + length)
-
-        self.setCurrentBlockState(0)
-
-        # Do multi-line strings
-        in_multiline = self.match_multiline(text, *self.tri_single)
-        if not in_multiline:
-            in_multiline = self.match_multiline(text, *self.tri_double)
-
-
-    def match_multiline(self, text, delimiter, in_state, style):
-        """Do highlighting of multi-line strings. ``delimiter`` should be a
-        ``QtCore.QRegExp`` for triple-single-quotes or triple-double-quotes, and
-        ``in_state`` should be a unique integer to represent the corresponding
-        state changes when inside those strings. Returns True if we're still
-        inside a multi-line string when this function is finished.
-        """
-        # If inside triple-single quotes, start at 0
-        if self.previousBlockState() == in_state:
-            start = 0
-            add = 0
-        # Otherwise, look for the delimiter on this line
-        else:
-            start = delimiter.indexIn(text)
-            # Move past this match
-            add = delimiter.matchedLength()
-
-        # As long as there's a delimiter match on this line...
-        while start >= 0:
-            # Look for the ending delimiter
-            end = delimiter.indexIn(text, start + add)
-            # Ending delimiter on this line?
-            if end >= add:
-                length = end - start + add + delimiter.matchedLength()
-                self.setCurrentBlockState(0)
-            # No; multi-line string
-            else:
-                self.setCurrentBlockState(in_state)
-                length = len(text) - start + add
-            # Apply formatting
-            self.setFormat(start, length, style)
-            # Look for the next match
-            start = delimiter.indexIn(text, start + length)
-
-        # Return True if still inside a multi-line string, False otherwise
-        if self.currentBlockState() == in_state:
-            return True
-        else:
+import sys
+from qtpy import QtCore, QtGui
+
+def format(color, style=''):
+    """Return a QtGui.QTextCharFormat with the given attributes.
+    """
+    _color = QtGui.QColor()
+    _color.setNamedColor(color)
+
+    _format = QtGui.QTextCharFormat()
+    _format.setForeground(_color)
+    if 'bold' in style:
+        _format.setFontWeight(QtGui.QFont.Bold)
+    if 'italic' in style:
+        _format.setFontItalic(True)
+    return _format
+
+
+# Syntax styles that can be shared by all languages
+STYLES = {
+    'keyword': format('blue'),
+    'operator': format('red'),
+    'brace': format('black'),
+    'defclass': format('black', 'bold'),
+    'string': format('magenta'),
+    'string2': format('darkMagenta'),
+    'comment': format('darkGreen', 'italic'),
+    'self': format('black', 'italic'),
+    'numbers': format('brown'),
+}
+
+
+class PythonHighlighter (QtGui.QSyntaxHighlighter):
+    """Syntax highlighter for the Python language.
+    """
+    # Python keywords
+    keywords = [
+        'and', 'assert', 'break', 'class', 'continue', 'def',
+        'del', 'elif', 'else', 'except', 'exec', 'finally',
+        'for', 'from', 'global', 'if', 'import', 'in',
+        'is', 'lambda', 'not', 'or', 'pass', 'print',
+        'raise', 'return', 'try', 'while', 'yield',
+        'None', 'True', 'False',
+    ]
+
+    # Python operators
+    operators = [
+        '=',
+        # Comparison
+        '==', '!=', '<', '<=', '>', '>=',
+        # Arithmetic
+        '\+', '-', '\*', '/', '//', '\%', '\*\*',
+        # In-place
+        '\+=', '-=', '\*=', '/=', '\%=',
+        # Bitwise
+        '\^', '\|', '\&', '\~', '>>', '<<',
+    ]
+
+    # Python braces
+    braces = [
+        '\{', '\}', '\(', '\)', '\[', '\]',
+    ]
+    def __init__(self, document):
+        QtGui.QSyntaxHighlighter.__init__(self, document)
+
+        # Multi-line strings (expression, flag, style)
+        # FIXME: The triple-quotes in these two lines will mess up the
+        # syntax highlighting from this point onward
+        self.tri_single = (QtCore.QRegularExpression("'''"), 1, STYLES['string2'])
+        self.tri_double = (QtCore.QRegularExpression('"""'), 2, STYLES['string2'])
+
+        rules = []
+
+        # Keyword, operator, and brace rules
+        rules += [(r'\b%s\b' % w, 0, STYLES['keyword'])
+            for w in PythonHighlighter.keywords]
+        rules += [(r'%s' % o, 0, STYLES['operator'])
+            for o in PythonHighlighter.operators]
+        rules += [(r'%s' % b, 0, STYLES['brace'])
+            for b in PythonHighlighter.braces]
+
+        # All other rules
+        rules += [
+            # 'self'
+            (r'\bself\b', 0, STYLES['self']),
+
+            # Double-quoted string, possibly containing escape sequences
+            (r'"[^"\\]*(\\.[^"\\]*)*"', 0, STYLES['string']),
+            # Single-quoted string, possibly containing escape sequences
+            (r"'[^'\\]*(\\.[^'\\]*)*'", 0, STYLES['string']),
+
+            # 'def' followed by an identifier
+            (r'\bdef\b\s*(\w+)', 1, STYLES['defclass']),
+            # 'class' followed by an identifier
+            (r'\bclass\b\s*(\w+)', 1, STYLES['defclass']),
+
+            # From '#' until a newline
+            (r'#[^\n]*', 0, STYLES['comment']),
+
+            # Numeric literals
+            (r'\b[+-]?[0-9]+[lL]?\b', 0, STYLES['numbers']),
+            (r'\b[+-]?0[xX][0-9A-Fa-f]+[lL]?\b', 0, STYLES['numbers']),
+            (r'\b[+-]?[0-9]+(?:\.[0-9]+)?(?:[eE][+-]?[0-9]+)?\b', 0, STYLES['numbers']),
+        ]
+
+        # Build a QtCore.QRegularExpression for each pattern
+        self.rules = [(QtCore.QRegularExpression(pat), index, fmt)
+            for (pat, index, fmt) in rules]
+
+
+    def highlightBlock(self, text):
+        """Apply syntax highlighting to the given block of text.
+        """
+        # Do other syntax formatting
+        for expression, nth, format in self.rules:
+            index = expression.indexIn(text, 0)
+
+            while index >= 0:
+                # We actually want the index of the nth match
+                index = expression.pos(nth)
+                length = len(expression.cap(nth))
+                self.setFormat(index, length, format)
+                index = expression.indexIn(text, index + length)
+
+        self.setCurrentBlockState(0)
+
+        # Do multi-line strings
+        in_multiline = self.match_multiline(text, *self.tri_single)
+        if not in_multiline:
+            in_multiline = self.match_multiline(text, *self.tri_double)
+
+
+    def match_multiline(self, text, delimiter, in_state, style):
+        """Do highlighting of multi-line strings. ``delimiter`` should be a
+        ``QtCore.QRegularExpression`` for triple-single-quotes or triple-double-quotes, and
+        ``in_state`` should be a unique integer to represent the corresponding
+        state changes when inside those strings. Returns True if we're still
+        inside a multi-line string when this function is finished.
+        """
+        # If inside triple-single quotes, start at 0
+        if self.previousBlockState() == in_state:
+            start = 0
+            add = 0
+        # Otherwise, look for the delimiter on this line
+        else:
+            start = delimiter.indexIn(text)
+            # Move past this match
+            add = delimiter.matchedLength()
+
+        # As long as there's a delimiter match on this line...
+        while start >= 0:
+            # Look for the ending delimiter
+            end = delimiter.indexIn(text, start + add)
+            # Ending delimiter on this line?
+            if end >= add:
+                length = end - start + add + delimiter.matchedLength()
+                self.setCurrentBlockState(0)
+            # No; multi-line string
+            else:
+                self.setCurrentBlockState(in_state)
+                length = len(text) - start + add
+            # Apply formatting
+            self.setFormat(start, length, style)
+            # Look for the next match
+            start = delimiter.indexIn(text, start + length)
+
+        # Return True if still inside a multi-line string, False otherwise
+        if self.currentBlockState() == in_state:
+            return True
+        else:
             return False
```

### Comparing `flika-0.2.9/flika/docs/_build/html/_static/favicon.ico` & `flika-0.3.0/flika/docs/_static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/docs/_build/html/_static/flika.png` & `flika-0.3.0/flika/images/favicon.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/docs/_build/html/_static/flika_logo.png` & `flika-0.3.0/flika/docs/_static/img/flika_logo.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/docs/_build/html/_static/img/favicon.ico` & `flika-0.3.0/flika/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/check.png` & `flika-0.3.0/flika/images/check.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/exclamation.png` & `flika-0.3.0/flika/images/exclamation.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/freehand.png` & `flika-0.3.0/flika/images/freehand.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/line.png` & `flika-0.3.0/flika/images/line.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/mouse.png` & `flika-0.3.0/flika/images/mouse.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/point.png` & `flika-0.3.0/flika/images/point.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/rect.png` & `flika-0.3.0/flika/images/rect.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/rect_line.png` & `flika-0.3.0/flika/images/rect_line.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/refresh.png` & `flika-0.3.0/flika/images/refresh.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/search.png` & `flika-0.3.0/flika/images/search.png`

 * *Files identical despite different names*

### Comparing `flika-0.2.9/flika/images/__init__.py` & `flika-0.3.0/flika/images/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-# -*- coding: utf-8 -*-
-import os
-import pkg_resources
-
-__all__ = ['image_path']
-
-def image_path(image_name):
-    """
-    Return the absolute path to an image
-
-    Parameters
-    ----------
-    image_name : str
-       Name of image
-
-    Returns
-    -------
-    path : str
-      Full path to image
-    """
-
-
-    try:
-        if pkg_resources.resource_exists('flika.images', image_name):
-            return pkg_resources.resource_filename('flika.images', image_name)
-        else:
-            raise RuntimeError("image does not exist: %s" % image_name)
-    except NotImplementedError:  # workaround for mac app
-        result = os.path.dirname(__file__)
-        return os.path.join(result.replace('site-packages.zip', 'flika'),
+# -*- coding: utf-8 -*-
+import os
+
+__all__ = ['image_path']
+
+def image_path(image_name):
+    """
+    Return the absolute path to an image
+
+    Parameters
+    ----------
+    image_name : str
+       Name of image
+
+    Returns
+    -------
+    path : str
+      Full path to image
+    """
+    import pkg_resources
+    try:
+        if pkg_resources.resource_exists('flika.images', image_name):
+            return pkg_resources.resource_filename('flika.images', image_name)
+        else:
+            raise RuntimeError("image does not exist: %s" % image_name)
+    except NotImplementedError:  # workaround for mac app
+        result = os.path.dirname(__file__)
+        return os.path.join(result.replace('site-packages.zip', 'flika'),
                             image_name)
```

### Comparing `flika-0.2.9/flika/process/BaseProcess.py` & `flika-0.3.0/flika/utils/BaseProcess.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,445 +1,531 @@
-# -*- coding: utf-8 -*-
-import os.path
-import numpy as np
-from qtpy import QtCore, QtGui, QtWidgets
-import pyqtgraph as pg
-import sys
-import inspect
-
-from .. import global_vars as g
-from .. import window
-from ..utils.misc import save_file_gui
-
-__all__ = []
-
-        
-class MissingWindowError(Exception):
-    def __init__(self, value):
-        self.value = value
-        g.m.statusBar().showMessage(value)
-    def __str__(self):
-        return repr(self.value)
-
-
-class WindowSelector(QtWidgets.QWidget):
-    """
-    This widget is a button with a label.  Once you click the button, the widget waits for you to click a Window object.  Once you do, it sets self.window to be the window, and it sets the label to be the widget name.
-    """
-    valueChanged=QtCore.Signal()
-    def __init__(self):
-        QtWidgets.QWidget.__init__(self)
-        self.button = QtWidgets.QPushButton('Select Window')
-        self.button.setCheckable(True)
-        self.label = QtWidgets.QLabel('None')
-        self.window = None
-        self.layout = QtWidgets.QHBoxLayout()
-        self.layout.addWidget(self.button)
-        self.layout.addWidget(self.label)
-        self.setLayout(self.layout)
-        self.button.clicked.connect(self.buttonclicked)
-
-    def buttonclicked(self):
-        if self.button.isChecked() is False:
-            g.m.setCurrentWindowSignal.sig.disconnect(self.setWindow)
-        else:
-            g.m.setCurrentWindowSignal.sig.connect(self.setWindow)
-
-    def setWindow(self, window=None):
-        if window is None:
-            try:
-                g.m.setCurrentWindowSignal.sig.disconnect(self.setWindow)
-            except TypeError:
-                pass
-            self.window = g.currentWindow
-        else:
-            self.window = window
-        self.button.setChecked(False)
-        self.label.setText('...'+os.path.split(self.window.name)[-1][-20:])
-        self.valueChanged.emit()
-    def value(self):
-        return self.window
-    def setValue(self, window):
-        ''' This function is written to satify the requirement that all items have a setValue function to recall from settings the last set value. '''
-        self.setWindow(window)
-
-
-class FileSelector(QtWidgets.QWidget):
-    """
-    This widget is a button with a label.  Once you click the button, the widget waits for you to select a file to save.  Once you do, it sets self.filename and it sets the label.
-    """
-    valueChanged=QtCore.Signal()
-    def __init__(self,filetypes='*.*'):
-        QtWidgets.QWidget.__init__(self)
-        self.button=QtWidgets.QPushButton('Select Filename')
-        self.label=QtWidgets.QLabel('None')
-        self.window=None
-        self.layout=QtWidgets.QHBoxLayout()
-        self.layout.addWidget(self.button)
-        self.layout.addWidget(self.label)
-        self.setLayout(self.layout)
-        self.button.clicked.connect(self.buttonclicked)
-        self.filetypes = filetypes
-        self.filename = ''
-        
-    def buttonclicked(self):
-        prompt = 'testing fileSelector'
-        self.filename = save_file_gui(prompt, filetypes=self.filetypes)
-        self.label.setText('...'+os.path.split(self.filename)[-1][-20:])
-        self.valueChanged.emit()
-
-    def value(self):
-        return self.filename
-
-    def setValue(self, filename):
-        self.filename = str(filename)
-        self.label.setText('...' + os.path.split(self.filename)[-1][-20:])
-
-def color_pixmap(color):
-    pm = QtGui.QPixmap(15, 15)
-    p = QtGui.QPainter(pm)
-    b = QtGui.QBrush(QtGui.QColor(color))
-    p.fillRect(-1, -1, 20, 20, b)
-    return pm
-
-class ColorSelector(QtWidgets.QWidget):
-    """
-    This widget is a button with a label.  Once you click the button, the widget waits for you to select a color.  Once you do, it sets self.color and it sets the label.
-    """
-    valueChanged=QtCore.Signal()
-    def __init__(self):
-        QtWidgets.QWidget.__init__(self)
-        self.button=QtWidgets.QPushButton('Select Color')
-        self.label=QtWidgets.QLabel('None')
-        self.window=None
-        self.layout=QtWidgets.QHBoxLayout()
-        self.layout.addWidget(self.button)
-        self.layout.addWidget(self.label)
-        self.setLayout(self.layout)
-        self.button.clicked.connect(self.buttonclicked)
-        self._color=''
-        self.colorDialog=QtWidgets.QColorDialog()
-        self.colorDialog.colorSelected.connect(self.colorSelected)
-
-    @property
-    def color(self):
-        return self._color
-
-    @color.setter
-    def color(self, color):
-        self._color = color
-        self.button.setIcon(QtGui.QIcon(color_pixmap(color)))
-
-    def buttonclicked(self):
-        self.colorDialog.open()
-
-    def value(self):
-        return self._color
-        
-    def colorSelected(self, color):
-        if color.isValid():
-            self.color=color.name()
-            self.label.setText(color.name())
-            self.valueChanged.emit()
-
-
-class SliderLabel(QtWidgets.QWidget):
-    changeSignal=QtCore.Signal(int)
-    def __init__(self,decimals=0): #decimals specifies the resolution of the slider.  0 means only integers,  1 means the tens place, etc.
-        QtWidgets.QWidget.__init__(self)
-        self.slider=QtWidgets.QSlider(QtCore.Qt.Horizontal)
-        self.decimals=decimals
-        if self.decimals<=0:
-            self.label=QtWidgets.QSpinBox()
-        else:
-            self.label=QtWidgets.QDoubleSpinBox()
-            self.label.setDecimals(self.decimals)
-        self.layout=QtWidgets.QHBoxLayout()
-        self.layout.addWidget(self.slider)
-        self.layout.addWidget(self.label)
-        self.layout.setContentsMargins(0,0,0,0)
-        self.setLayout(self.layout)
-        self.slider.valueChanged.connect(lambda val: self.updateLabel(val/10**self.decimals))
-        self.label.valueChanged.connect(self.updateSlider)
-        self.valueChanged=self.label.valueChanged
-    @QtCore.Slot(float)
-    @QtCore.Slot(int)
-    def updateSlider(self,value):
-        self.slider.setValue(int(value*10**self.decimals))
-    def updateLabel(self,value):
-        self.label.setValue(value)
-    def value(self):
-        return self.label.value()
-    def setRange(self,minn,maxx):
-        self.slider.setRange(minn*10**self.decimals,maxx*10**self.decimals)
-        self.label.setRange(minn,maxx)
-    def setMinimum(self,minn):
-        self.slider.setMinimum(minn*10**self.decimals)
-        self.label.setMinimum(minn)
-    def setMaximum(self,maxx):
-        self.slider.setMaximum(maxx*10**self.decimals)
-        self.label.setMaximum(maxx)
-    def setValue(self,value):
-        self.slider.setValue(value*10**self.decimals)
-        self.label.setValue(value)
-    def setSingleStep(self,value):
-        self.label.setSingleStep(value)
-    def setEnabled(self, en):
-        self.label.setEnabled(en)
-        self.slider.setEnabled(en)
-
-
-class SliderLabelOdd(SliderLabel):
-    '''This is a modified SliderLabel class that forces the user to only choose odd numbers.'''
-    def __init__(self):
-        SliderLabel.__init__(self,decimals=0)
-    @QtCore.Slot(int)
-    def updateSlider(self,value):
-        value=int(value)
-        if value%2==0: #if value is even
-            value+=1
-        self.slider.setValue(value)
-    def updateLabel(self,value):
-        value=int(value)
-        if value%2==0: #if value is even
-            value+=1
-        self.label.setValue(value)
-
-
-class CheckBox(QtWidgets.QCheckBox):
-    ''' I overwrote the QCheckBox class so that every graphical element has the method 'setValue'
-    '''
-    def __init__(self,parent=None):
-        QtWidgets.QCheckBox.__init__(self,parent)
-    def setValue(self,value):
-        self.setChecked(value)
-
-class ComboBox(QtWidgets.QComboBox):
-    ''' I overwrote the QComboBox class so that every graphical element has the method 'setValue'
-    '''
-    def __init__(self, parent=None):
-        QtWidgets.QComboBox.__init__(self, parent)
-    def setValue(self, value):
-        if isinstance(value, str):
-            idx = self.findText(value)
-        else:
-            idx = self.findData(value)
-        if idx != -1:
-            self.setCurrentIndex(idx)
-
-class BaseDialog(QtWidgets.QDialog):
-    changeSignal=QtCore.Signal()
-    closeSignal=QtCore.Signal()
-    def __init__(self, items, title, docstring, parent=None):
-        QtWidgets.QDialog.__init__(self)
-        self.parent = parent
-        self.setWindowTitle(title)
-        self.formlayout = QtWidgets.QFormLayout()
-        self.formlayout.setLabelAlignment(QtCore.Qt.AlignRight)
-        self.items = items
-        self.setupitems()
-        self.connectToChangeSignal()
-        self.bbox = QtWidgets.QDialogButtonBox(QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel)
-        self.bbox.accepted.connect(self.accept)
-        self.bbox.rejected.connect(self.reject)
-        self.docstring = QtWidgets.QLabel(docstring)
-        self.docstring.setWordWrap(True)
-        self.layout = QtWidgets.QVBoxLayout()
-        self.layout.addWidget(self.docstring)
-        self.layout.addLayout(self.formlayout)
-        self.layout.addWidget(self.bbox)
-        self.setLayout(self.layout)
-        self.changeSignal.connect(self.updateValues)
-        self.updateValues()
-
-    def setupitems(self):
-        for item in self.items:
-            self.formlayout.addRow(item['string'], item['object'])
-        # Get the old vals from settings
-        if self.parent is not None:
-            name = self.parent.__name__
-            if g.settings['baseprocesses'] is None:
-                g.settings['baseprocesses'] = dict()
-            if name not in g.settings['baseprocesses']:
-                settings = self.parent.get_init_settings_dict()
-                g.settings['baseprocesses'][name] = settings
-            else:
-                settings = g.settings['baseprocesses'][name]
-            for item in self.items:
-                if item['name'] in settings:
-                    item['object'].setValue(settings[item['name']])
-
-    def connectToChangeSignal(self):
-        for item in self.items:
-            methods=[method for method in dir(item['object']) if callable(getattr(item['object'], method))]
-            if 'valueChanged' in methods:
-                item['object'].valueChanged.connect(self.changeSignal)
-            elif 'stateChanged' in methods:
-                item['object'].stateChanged.connect(self.changeSignal)
-            elif 'currentIndexChanged' in methods:
-                item['object'].currentIndexChanged.connect(self.changeSignal)
-
-    def updateValues(self): # copy values from gui into the 'item' dictionary
-        for item in self.items:
-            methods=[method for method in dir(item['object']) if callable(getattr(item['object'], method))]
-            if 'value' in methods:
-                item['value']=item['object'].value()
-            elif 'currentText' in methods:
-                item['value']=item['object'].currentText()
-            elif 'isChecked' in methods:
-                item['value']=item['object'].isChecked()
-    def closeEvent(self,ev):
-        self.closeSignal.emit()
-
-
-def convert_to_string(item):
-    if isinstance(item, str):
-        return "'{}'".format(item)
-    else:
-        return str(item)
-
-
-class BaseProcess(object):
-    def __init__(self):
-        self.noPriorWindow = False
-        self.__name__=self.__class__.__name__.lower()
-        self.items=[]
-
-    def getValue(self,name):
-        return [i['value'] for i in self.items if i['name']==name][0]
-
-    def get_init_settings_dict(self):
-        return dict() #this function needs to be overwritten by every subclass
-
-    def start(self, keepSourceWindow):
-        frame = inspect.getouterframes(inspect.currentframe())[1][0]
-        args, _, _, values = inspect.getargvalues(frame)
-        funcname = self.__name__
-        self.command = funcname+'('+', '.join([i+'='+convert_to_string(values[i]) for i in args if i!='self'])+')'
-        g.m.statusBar().showMessage('Running function {}...'.format(self.__name__))
-        self.keepSourceWindow = keepSourceWindow
-        self.oldwindow = g.currentWindow
-        if self.oldwindow is None:
-            raise(MissingWindowError("You cannot execute '{}' without selecting a window first.".format(self.__name__)))
-        self.tif = self.oldwindow.image
-        self.oldname = self.oldwindow.name
-
-    def end(self):
-        if not hasattr(self, 'newtif') or self.newtif is None:
-            self.oldwindow.reset()
-            return
-        commands=self.oldwindow.commands[:]
-        commands.append(self.command)
-        newWindow=window.Window(self.newtif,str(self.newname),self.oldwindow.filename,commands,self.oldwindow.metadata)
-        if self.keepSourceWindow is False:
-            self.oldwindow.close()
-        else:
-            self.oldwindow.reset()
-        if np.max(self.newtif)==1 and np.min(self.newtif)==0: #if the array is boolean
-            newWindow.imageview.setLevels(-.1,1.1)
-        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
-        del self.tif
-        del self.newtif
-        return newWindow
-
-    def gui(self):
-        self.ui=BaseDialog(self.items,self.__name__,self.__doc__, self)
-        if hasattr(self, '__url__'):
-            self.ui.bbox.addButton(QtWidgets.QDialogButtonBox.Help)
-            self.ui.bbox.helpRequested.connect(lambda : QtWidgets.QDesktopServices.openUrl(QtCore.QUrl(self.__url__)))
-        self.proxy= pg.SignalProxy(self.ui.changeSignal,rateLimit=60, slot=self.preview)
-        if g.currentWindow is not None:
-            self.ui.rejected.connect(g.currentWindow.reset)
-        self.ui.accepted.connect(self.call_from_gui)
-        self.ui.show()
-        g.dialogs.append(self.ui)
-        return True
-
-    def gui_reset(self):
-        self.items=[]
-
-    def call_from_gui(self):
-        varnames = [i for i in inspect.getargspec(self.__call__)[0] if i != 'self' and i != 'keepSourceWindow']
-        try:
-            args = [self.getValue(name) for name in varnames]
-        except IndexError as err:
-            msg = "IndexError in {}: {}".format(self.__name__, varnames)
-            msg += str(err)
-            g.alert(msg)
-        newsettings = dict()
-        for name in varnames:
-            value = self.getValue(name)
-            if not isinstance(value, window.Window): # cannot save window objects using pickle
-                newsettings[name] = value
-        g.settings['baseprocesses'][self.__name__] = newsettings
-        g.settings.save()
-        try:
-            if self.noPriorWindow:
-                self.__call__(*args)
-            else:
-                self.__call__(*args, keepSourceWindow=True)
-        except MemoryError as err:
-            msg = 'There was a memory error in {}. Close other programs and try again.'.format(self.__name__)
-            msg += str(err)
-            g.alert(msg)
-    def preview(self):
-        pass
-
-
-class BaseProcess_noPriorWindow(BaseProcess):
-
-    def __init__(self):
-        super().__init__()
-        self.noPriorWindow = True
-
-    def start(self):
-        frame = inspect.getouterframes(inspect.currentframe())[1][0]
-        args, _, _, values = inspect.getargvalues(frame)
-        funcname = self.__name__
-        self.command = funcname+'('+', '.join([i+'='+convert_to_string(values[i]) for i in args if i!='self'])+')'
-        g.m.statusBar().showMessage('Performing {}...'.format(self.__name__))
-        
-    def end(self):
-        commands = [self.command]
-        newWindow = window.Window(self.newtif,str(self.newname),commands=commands)
-        if np.max(self.newtif) == 1 and np.min(self.newtif) == 0: #if the array is boolean
-            newWindow.imageview.setLevels(-.1,1.1)
-        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
-        del self.newtif
-        return newWindow
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+# -*- coding: utf-8 -*-
+from ..utils.misc import save_file_gui
+from .. import global_vars as g
+import markdown
+import inspect
+import sys
+from qtpy import QtCore, QtGui, QtWidgets
+import numpy as np
+import os.path
+from ..logger import logger
+logger.debug("Started 'reading process/BaseProcess.py'")
+
+
+__all__ = ['MissingWindowError', 'WindowSelector', 'FileSelector', 'ColorSelector', 'SliderLabel',
+           'SliderLabelOdd', 'CheckBox', 'ComboBox', 'BaseDialog', 'BaseProcess', 'BaseProcess_noPriorWindow']
+
+
+class MissingWindowError(Exception):
+    def __init__(self, value):
+        self.value = value
+        g.m.statusBar().showMessage(value)
+
+    def __str__(self):
+        return repr(self.value)
+
+
+class WindowSelector(QtWidgets.QWidget):
+    """
+    This widget is a button with a label.  Once you click the button, the widget waits for you to click a Window object.  Once you do, it sets self.window to be the window, and it sets the label to be the widget name.
+    """
+    valueChanged = QtCore.Signal()
+
+    def __init__(self):
+        QtWidgets.QWidget.__init__(self)
+        self.button = QtWidgets.QPushButton('Select Window')
+        self.button.setCheckable(True)
+        self.label = QtWidgets.QLabel('None')
+        self.window = None
+        self.layout = QtWidgets.QHBoxLayout()
+        self.layout.addWidget(self.button)
+        self.layout.addWidget(self.label)
+        self.setLayout(self.layout)
+        self.button.clicked.connect(self.buttonclicked)
+
+    def buttonclicked(self):
+        if self.button.isChecked() is False:
+            g.m.setCurrentWindowSignal.sig.disconnect(self.setWindow)
+        else:
+            g.m.setCurrentWindowSignal.sig.connect(self.setWindow)
+
+    def setWindow(self, window=None):
+        if window is None:
+            try:
+                g.m.setCurrentWindowSignal.sig.disconnect(self.setWindow)
+            except TypeError:
+                pass
+            self.window = g.win
+        else:
+            self.window = window
+        self.button.setChecked(False)
+        self.label.setText('...'+os.path.split(self.window.name)[-1][-20:])
+        self.valueChanged.emit()
+        self.parent().raise_()
+
+    def value(self):
+        return self.window
+
+    def setValue(self, window):
+        ''' This function is written to satify the requirement that all items have a setValue function to recall from settings the last set value. '''
+        self.setWindow(window)
+
+
+class FileSelector(QtWidgets.QWidget):
+    """
+    This widget is a button with a label.  Once you click the button, the widget waits for you to select a file to save.  Once you do, it sets self.filename and it sets the label.
+    """
+    valueChanged = QtCore.Signal()
+
+    def __init__(self, filetypes='*.*'):
+        QtWidgets.QWidget.__init__(self)
+        self.button = QtWidgets.QPushButton('Select Filename')
+        self.label = QtWidgets.QLabel('None')
+        self.window = None
+        self.layout = QtWidgets.QHBoxLayout()
+        self.layout.addWidget(self.button)
+        self.layout.addWidget(self.label)
+        self.setLayout(self.layout)
+        self.button.clicked.connect(self.buttonclicked)
+        self.filetypes = filetypes
+        self.filename = ''
+
+    def buttonclicked(self):
+        prompt = 'testing fileSelector'
+        self.filename = save_file_gui(prompt, filetypes=self.filetypes)
+        self.label.setText('...'+os.path.split(self.filename)[-1][-20:])
+        self.valueChanged.emit()
+
+    def value(self):
+        return self.filename
+
+    def setValue(self, filename):
+        self.filename = str(filename)
+        self.label.setText('...' + os.path.split(self.filename)[-1][-20:])
+
+
+def color_pixmap(color):
+    pm = QtGui.QPixmap(15, 15)
+    p = QtGui.QPainter(pm)
+    b = QtGui.QBrush(QtGui.QColor(color))
+    p.fillRect(-1, -1, 20, 20, b)
+    return pm
+
+
+class ColorSelector(QtWidgets.QWidget):
+    """
+    This widget is a button with a label.  Once you click the button, the widget waits for you to select a color.  Once you do, it sets self.color and it sets the label.
+    """
+    valueChanged = QtCore.Signal()
+
+    def __init__(self):
+        QtWidgets.QWidget.__init__(self)
+        self.button = QtWidgets.QPushButton('Select Color')
+        self.label = QtWidgets.QLabel('None')
+        self.window = None
+        self.layout = QtWidgets.QHBoxLayout()
+        self.layout.addWidget(self.button)
+        self.layout.addWidget(self.label)
+        self.setLayout(self.layout)
+        self.button.clicked.connect(self.buttonclicked)
+        self._color = ''
+        self.colorDialog = QtWidgets.QColorDialog()
+        self.colorDialog.colorSelected.connect(self.colorSelected)
+
+    @property
+    def color(self):
+        return self._color
+
+    @color.setter
+    def color(self, color):
+        self._color = color
+        self.button.setIcon(QtGui.QIcon(color_pixmap(color)))
+
+    def buttonclicked(self):
+        self.colorDialog.open()
+
+    def value(self):
+        return self._color
+
+    def colorSelected(self, color):
+        if color.isValid():
+            self.color = color.name()
+            self.label.setText(color.name())
+            self.valueChanged.emit()
+
+
+class SliderLabel(QtWidgets.QWidget):
+    changeSignal = QtCore.Signal(int)
+
+    def __init__(self, decimals: int = 0):
+        """
+        Args:
+          decimals: the resolution of the slider. 0 means only integers,  1 
+          means the tens place, etc.
+        """
+        # decimals specifies the resolution of the slider.
+        QtWidgets.QWidget.__init__(self)
+        self.slider = QtWidgets.QSlider(QtCore.Qt.Horizontal)
+        self.decimals = decimals
+        if self.decimals <= 0:
+            self.label = QtWidgets.QSpinBox()
+        else:
+            self.label = QtWidgets.QDoubleSpinBox()
+            self.label.setDecimals(self.decimals)
+        self.layout = QtWidgets.QHBoxLayout()
+        self.layout.addWidget(self.slider)
+        self.layout.addWidget(self.label)
+        self.layout.setContentsMargins(0, 0, 0, 0)
+        self.setLayout(self.layout)
+        self.slider.valueChanged.connect(
+            lambda slider_value: self.updateLabel(self.slider_2_spinbox(slider_value)))
+        self.label.valueChanged.connect(self.updateSlider)
+        self.valueChanged = self.label.valueChanged
+
+    def spinbox_2_slider(self, spinbox_value: float | int) -> int:
+        """Takes a spinbox value and converts it to a slider value."""
+        return int(spinbox_value * 10**self.decimals)
+    
+    def slider_2_spinbox(self, slider_value: int) -> int | float:
+        """Takes a slider value and converts it to a spinbox value."""
+        spinbox_value = slider_value / 10**self.decimals
+        if isinstance(self.label, QtWidgets.QSpinBox):
+            spinbox_value = int(spinbox_value)
+        return spinbox_value
+
+    @QtCore.Slot(float)
+    @QtCore.Slot(int)
+    def updateSlider(self, value: int | float):
+        slider_value = self.spinbox_2_slider(value)
+        self.slider.setValue(slider_value)
+
+    def updateLabel(self, spinbox_value: int | float):
+        """Sets the spinbox value."""
+        self.label.setValue(spinbox_value)
+
+    def value(self) -> int | float:
+        """Gets the spinbox value."""
+        return self.label.value()
+
+    def setRange(self, new_min: float, new_max: float):
+        new_slider_min = self.spinbox_2_slider(new_min)
+        new_slider_max = self.spinbox_2_slider(new_max)
+        self.slider.setRange(new_slider_min, new_slider_max)
+        self.label.setRange(new_min, new_max)
+
+    def setMinimum(self, new_min: float):
+        new_slider_min = self.spinbox_2_slider(new_min)
+        self.slider.setMinimum(new_slider_min)
+        self.label.setMinimum(new_min)
+
+    def setMaximum(self, new_max: float):
+        new_slider_max = self.spinbox_2_slider(new_max)
+        self.slider.setMaximum(new_slider_max)
+        self.label.setMaximum(new_max)
+
+    def setValue(self, spinbox_value: float):
+        slider_value = self.spinbox_2_slider(spinbox_value)
+        self.slider.setValue(slider_value)
+        self.label.setValue(spinbox_value)
+
+    def setSingleStep(self, spinbox_step_value: int | float):
+        self.label.setSingleStep(spinbox_step_value)
+
+    def setEnabled(self, enabled: bool):
+        self.label.setEnabled(enabled)
+        self.slider.setEnabled(enabled)
+
+
+class SliderLabelOdd(SliderLabel):
+    '''This is a modified SliderLabel class that forces the user to only choose odd numbers.'''
+
+    def __init__(self):
+        SliderLabel.__init__(self, decimals=0)
+
+    @QtCore.Slot(int)
+    def updateSlider(self, value):
+        value = int(value)
+        if value % 2 == 0:  # if value is even
+            value += 1
+        self.slider.setValue(value)
+
+    def updateLabel(self, spinbox_value: int | float):
+        spinbox_value = int(spinbox_value)
+        if spinbox_value % 2 == 0:  # if value is even
+            spinbox_value += 1
+        self.label.setValue(spinbox_value)
+
+
+class CheckBox(QtWidgets.QCheckBox):
+    '''Overwrote the QCheckBox class so that every graphical element has the method 'setValue'
+    '''
+
+    def __init__(self, parent=None):
+        QtWidgets.QCheckBox.__init__(self, parent)
+
+    def setValue(self, value):
+        self.setChecked(value)
+
+
+class ComboBox(QtWidgets.QComboBox):
+    '''Overwrote the QComboBox class so that every graphical element has the method 'setValue'
+    '''
+
+    def __init__(self, parent=None):
+        QtWidgets.QComboBox.__init__(self, parent)
+
+    def setValue(self, value):
+        if isinstance(value, str):
+            idx = self.findText(value)
+        else:
+            idx = self.findData(value)
+        if idx != -1:
+            self.setCurrentIndex(idx)
+
+
+class BaseDialog(QtWidgets.QDialog):
+    changeSignal = QtCore.Signal()
+    closeSignal = QtCore.Signal()
+
+    def __init__(self, items, title, docstring, parent=None):
+        QtWidgets.QDialog.__init__(self)
+        self.parent = parent
+        self.setWindowTitle(title)
+        self.formlayout = QtWidgets.QFormLayout()
+        self.formlayout.setLabelAlignment(QtCore.Qt.AlignRight)
+        self.docstring = None
+        self.items = items
+        self.setupitems()
+        self.connectToChangeSignal()
+        self.bbox = QtWidgets.QDialogButtonBox(
+            QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel)
+        self.bbox.accepted.connect(self.accept)
+        self.bbox.rejected.connect(self.reject)
+        self._init_docstring(docstring)
+        self.layout = QtWidgets.QVBoxLayout()
+        if docstring is not None:
+            self.layout.addWidget(self.docstring)
+        self.layout.addLayout(self.formlayout)
+        self.layout.addWidget(self.bbox)
+        self.setLayout(self.layout)
+        self.changeSignal.connect(self.updateValues)
+        self.updateValues()
+
+    def _init_docstring(self, docstring):
+        if docstring is None:
+            return None
+        self.docstring = QtWidgets.QTextBrowser()
+        self.docstring.setOpenExternalLinks(True)
+        docstring = markdown.markdown(docstring)
+        self.docstring.setHtml(docstring)
+        # css = """ """
+        # self.docstring.setStyleSheet(css)
+        self.docstring.setWordWrapMode(QtGui.QTextOption.NoWrap)
+
+    def setupitems(self):
+        for item in self.items:
+            self.formlayout.addRow(item['string'], item['object'])
+        # Get the old vals from settings
+        if self.parent is not None:
+            name = self.parent.__name__
+            if g.settings['baseprocesses'] is None:
+                g.settings['baseprocesses'] = dict()
+            if name not in g.settings['baseprocesses']:
+                settings = self.parent.get_init_settings_dict()
+                g.settings['baseprocesses'][name] = settings
+            else:
+                settings = g.settings['baseprocesses'][name]
+            for item in self.items:
+                if item['name'] in settings and not isinstance(item['object'], WindowSelector):
+                    item['object'].setValue(settings[item['name']])
+
+    def connectToChangeSignal(self):
+        for item in self.items:
+            methods = [method for method in dir(item['object']) if callable(
+                getattr(item['object'], method))]
+            if 'valueChanged' in methods:
+                item['object'].valueChanged.connect(self.changeSignal)
+            elif 'stateChanged' in methods:
+                item['object'].stateChanged.connect(self.changeSignal)
+            elif 'currentIndexChanged' in methods:
+                item['object'].currentIndexChanged.connect(self.changeSignal)
+
+    def updateValues(self):  # copy values from gui into the 'item' dictionary
+        for item in self.items:
+            methods = [method for method in dir(item['object']) if callable(
+                getattr(item['object'], method))]
+            if 'value' in methods:
+                item['value'] = item['object'].value()
+            elif 'currentText' in methods:
+                item['value'] = item['object'].currentText()
+            elif 'isChecked' in methods:
+                item['value'] = item['object'].isChecked()
+
+    def closeEvent(self, ev):
+        self.closeSignal.emit()
+
+
+def convert_to_string(item):
+    if isinstance(item, str):
+        return "'{}'".format(item)
+    else:
+        return str(item)
+
+
+class BaseProcess(object):
+    """BaseProcess(object)
+    Foundation for all flika processes. Subclass BaseProcess when writing your own process.
+
+    Attributes:
+        items: list of significant values unique to each BaseProcess subclass
+
+
+    """
+
+    def __init__(self):
+        self.noPriorWindow = False
+        self.__name__ = self.__class__.__name__.lower()
+        self.items = []
+
+    def getValue(self, name):
+        '''getValue(self,name)
+
+        Returns:
+            The value of a the name stored in self.items
+
+        '''
+        return [i['value'] for i in self.items if i['name'] == name][0]
+
+    def get_init_settings_dict(self):
+        '''get_init_settings_dict(self)
+        Function for storing the intial settings of any BaseProcess into self.items
+
+        Note:
+            In most cases when writing a BaseProcess subclass, this function must be overloaded
+
+        Returns:
+            A dictionary containing the initial settings and their values
+
+                '''
+        return dict()  # this function needs to be overwritten by every subclass
+
+    def start(self, keepSourceWindow):
+        frame = inspect.getouterframes(inspect.currentframe())[1][0]
+        args, _, _, values = inspect.getargvalues(frame)
+        funcname = self.__name__
+        self.command = funcname + \
+            '('+', '.join([i+'='+convert_to_string(values[i])
+                           for i in args if i != 'self'])+')'
+        g.m.statusBar().showMessage('Running function {}...'.format(self.__name__))
+        self.keepSourceWindow = keepSourceWindow
+        self.oldwindow = g.win
+        if self.oldwindow is None:
+            raise (MissingWindowError(
+                "You cannot execute '{}' without selecting a window first.".format(self.__name__)))
+        self.tif = self.oldwindow.image
+        self.oldname = self.oldwindow.name
+
+    def end(self):
+        from .. import window
+        if not hasattr(self, 'newtif') or self.newtif is None:
+            self.oldwindow.reset()
+            return
+        commands = self.oldwindow.commands[:]
+        if hasattr(self, 'command'):
+            commands.append(self.command)
+        newWindow = window.Window(self.newtif, str(
+            self.newname), self.oldwindow.filename, commands, self.oldwindow.metadata)
+        if self.keepSourceWindow is False:
+            self.oldwindow.close()
+        else:
+            self.oldwindow.reset()
+        if np.max(self.newtif) == 1 and np.min(self.newtif) == 0:  # if the array is boolean
+            newWindow.imageview.setLevels(-.1, 1.1)
+        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
+        del self.tif
+        del self.newtif
+        return newWindow
+
+    def gui(self):
+        from pyqtgraph import SignalProxy
+        self.ui = BaseDialog(self.items, self.__name__, self.__doc__, self)
+        if hasattr(self, '__url__'):
+            self.ui.bbox.addButton(QtWidgets.QDialogButtonBox.Help)
+            self.ui.bbox.helpRequested.connect(
+                lambda: QtWidgets.QDesktopServices.openUrl(QtCore.QUrl(self.__url__)))
+        self.proxy = SignalProxy(self.ui.changeSignal,
+                                 rateLimit=60, slot=self.preview)
+        if g.win is not None:
+            self.ui.rejected.connect(g.win.reset)
+        self.ui.closeSignal.connect(self.ui.rejected.emit)
+        self.ui.accepted.connect(self.call_from_gui)
+        self.ui.resize(750, 450)
+        self.ui.show()
+        g.dialogs.append(self.ui)
+        return True
+
+    def gui_reset(self):
+        self.items = []
+
+    def call_from_gui(self):
+        from .. import window
+        varnames = [i for i in inspect.getfullargspec(
+            self.__call__)[0] if i != 'self' and i != 'keepSourceWindow']
+        try:
+            args = [self.getValue(name) for name in varnames]
+        except IndexError as err:
+            msg = "IndexError in {}: {}".format(self.__name__, varnames)
+            msg += str(err)
+            g.alert(msg)
+        newsettings = dict()
+        for name in varnames:
+            value = self.getValue(name)
+            # cannot save window objects using pickle
+            if not isinstance(value, window.Window):
+                newsettings[name] = value
+        g.settings['baseprocesses'][self.__name__] = newsettings
+        g.settings.save()
+        try:
+            if self.noPriorWindow:
+                self.__call__(*args)
+            else:
+                self.__call__(*args, keepSourceWindow=True)
+        except MemoryError as err:
+            msg = 'There was a memory error in {}. Close other programs and try again.'.format(
+                self.__name__)
+            msg += str(err)
+            g.alert(msg)
+
+    def preview(self):
+        pass
+
+
+class BaseProcess_noPriorWindow(BaseProcess):
+    """A BaseProcess subclass that has no prior window.
+    Some flika objects inherit this class."""
+
+    def __init__(self):
+        super().__init__()
+        self.noPriorWindow = True
+
+    def start(self):
+        frame = inspect.getouterframes(inspect.currentframe())[1][0]
+        args, _, _, values = inspect.getargvalues(frame)
+        funcname = self.__name__
+        self.command = funcname + \
+            '('+', '.join([i+'='+convert_to_string(values[i])
+                           for i in args if i != 'self'])+')'
+        g.m.statusBar().showMessage('Performing {}...'.format(self.__name__))
+
+    def end(self):
+        from .. import window
+        commands = [self.command]
+        newWindow = window.Window(self.newtif, str(
+            self.newname), commands=commands)
+        if np.max(self.newtif) == 1 and np.min(self.newtif) == 0:  # if the array is boolean
+            newWindow.imageview.setLevels(-.1, 1.1)
+        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
+        del self.newtif
+        return newWindow
+
+
+logger.debug("Completed 'reading process/BaseProcess.py'")
```

### Comparing `flika-0.2.9/flika/process/binary.py` & `flika-0.3.0/flika/process/binary.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,554 +1,575 @@
-# -*- coding: utf-8 -*-
-import numpy as np
-import scipy
-import scipy.ndimage    
-from skimage import feature, measure
-from skimage.morphology import remove_small_objects
-from skimage.filters import threshold_adaptive
-from qtpy import QtCore, QtGui, QtWidgets
-from .. import global_vars as g
-from .BaseProcess import BaseProcess, SliderLabel, WindowSelector,  MissingWindowError, CheckBox, ComboBox
-from ..roi import makeROI, ROI_Drawing
-
-
-__all__ = ['threshold','remove_small_blobs','adaptive_threshold','logically_combine','binary_dilation','binary_erosion', 'generate_rois', 'canny_edge_detector']
-     
-     
-def convert2uint8(tif):
-    oldmin = np.min(tif)
-    oldmax = np.max(tif)
-    newmax = 2**8-1
-    tif = ((tif-oldmin)*newmax)/(oldmax-oldmin)
-    tif = tif.astype(np.uint8)
-    return tif
-    
-class Threshold(BaseProcess):
-    """threshold(value, darkBackground=False, keepSourceWindow=False)
-    Creates a boolean matrix by applying a threshold
-    
-    Parameters:
-        | value (float) -- The threshold to be applied
-        | darkBackground (bool) -- If this is True, pixels below the threshold will be True
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        valueSlider=SliderLabel(2)
-        if g.currentWindow is not None:
-            image=g.currentWindow.image
-            valueSlider.setRange(np.min(image),np.max(image))
-            valueSlider.setValue(np.mean(image))
-        preview=CheckBox()
-        preview.setChecked(True)
-        self.items.append({'name':'value','string':'Value','object':valueSlider})
-        self.items.append({'name':'darkBackground','string':'Dark Background','object': CheckBox()})
-        self.items.append({'name':'preview','string':'Preview','object':preview})
-        super().gui()
-    def __call__(self,value,darkBackground=False, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.oldwindow.nDims > 3:
-            g.alert("You cannot run this function on an image of dimension greater than 3. If your window has color, convert to a grayscale image before running this function")
-            return None
-        if darkBackground:
-            newtif=self.tif<value
-        else:
-            newtif=self.tif>value
-        self.newtif=newtif.astype(np.uint8)
-        self.newname=self.oldname+' - Thresholded '+str(value)
-        return self.end()
-    def preview(self):
-        value=self.getValue('value')
-        preview=self.getValue('preview')
-        darkBackground=self.getValue('darkBackground')
-        nDim=len(g.currentWindow.image.shape)
-        if nDim > 3:
-            g.alert("You cannot run this function on an image of dimension greater than 3. If your window has color, convert to a grayscale image before running this function")
-            return None
-        if preview:
-            if nDim==3: # if the image is 3d
-                testimage=np.copy(g.currentWindow.image[g.currentWindow.currentIndex])
-            elif nDim==2:
-                testimage=np.copy(g.currentWindow.image)
-            if darkBackground:
-                testimage=testimage<value
-            else:
-                testimage=testimage>value
-            g.currentWindow.imageview.setImage(testimage,autoLevels=False)
-            g.currentWindow.imageview.setLevels(-.1,1.1)
-        else:
-            g.currentWindow.reset()
-            if nDim==3:
-                image=g.currentWindow.image[g.currentWindow.currentIndex]
-            else:
-                image=g.currentWindow.image
-            g.currentWindow.imageview.setLevels(np.min(image),np.max(image))
-threshold=Threshold()
-
-class BlocksizeSlider(SliderLabel):
-    def __init__(self,demicals=0):
-        SliderLabel.__init__(self,demicals)
-    def updateSlider(self,value):
-        if value%2==0:
-            if value<self.slider.value():
-                value-=1
-            else:
-                value+=1
-            self.label.setValue(value)
-        self.slider.setValue(int(value*10**self.decimals))
-    def updateLabel(self,value):
-        if value%2==0:
-            value-=1
-        self.label.setValue(value)
-    
-class Adaptive_threshold(BaseProcess):
-    """adaptive_threshold(value, block_size, darkBackground=False, keepSourceWindow=False)
-    Creates a boolean matrix by applying an adaptive threshold using the scikit-image threshold_adaptive function
-    
-    Parameters:
-        | value (int) -- The threshold to be applied
-        | block_size (int)  -- size of a pixel neighborhood that is used to calculate a threshold value for the pixel. Must be an odd number greater than 3.
-        | darkBackground (bool) -- If this is True, pixels below the threshold will be True
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        valueSlider=SliderLabel(2)
-        valueSlider.setRange(-20,20)
-        valueSlider.setValue(0)
-        block_size=BlocksizeSlider(0)
-        if g.currentWindow is not None:
-            max_block=int(max([g.currentWindow.image.shape[-1],g.currentWindow.image.shape[-2]])/2)
-        block_size.setRange(3,max_block)
-        preview = CheckBox(); preview.setChecked(True)
-        self.items.append({'name': 'value', 'string': 'Value', 'object': valueSlider})
-        self.items.append({'name': 'block_size', 'string':'Block Size', 'object':block_size})
-        self.items.append({'name': 'darkBackground', 'string': 'Dark Background', 'object': CheckBox()})
-        self.items.append({'name': 'preview', 'string': 'Preview', 'object': preview})
-        super().gui()
-        self.preview()
-
-    def __call__(self, value, block_size, darkBackground=False, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.tif.dtype == np.float16:
-            g.alert("Adaptive Threshold does not support float16 type arrays")
-            return
-        newtif = np.copy(self.tif)
-
-        if self.oldwindow.nDims == 2:
-            newtif = threshold_adaptive(newtif, block_size, offset=value)
-        elif self.oldwindow.nDims == 3:
-            for i in np.arange(len(newtif)):
-                newtif[i] = threshold_adaptive(newtif[i], block_size, offset=value)
-        else:
-            g.alert("You cannot run this function on an image of dimension greater than 3. If your window has color, convert to a grayscale image before running this function")
-            return None
-        if darkBackground:
-            newtif = np.logical_not(newtif)
-        self.newtif = newtif.astype(np.uint8)
-        self.newname = self.oldname + ' - Thresholded ' + str(value)
-        return self.end()
-
-    def preview(self):
-        value = self.getValue('value')
-        block_size = self.getValue('block_size')
-        preview = self.getValue('preview')
-        darkBackground = self.getValue('darkBackground')
-        nDim = len(g.currentWindow.image.shape)
-        if nDim > 3:
-            g.alert("You cannot run this function on an image of dimension greater than 3. If your window has color, convert to a grayscale image before running this function")
-            return None
-        if preview:
-            if nDim == 3: # if the image is 3d
-                testimage=np.copy(g.currentWindow.image[g.currentWindow.currentIndex])
-            elif nDim == 2:
-                testimage=np.copy(g.currentWindow.image)
-            testimage = threshold_adaptive(testimage, block_size, offset=value)
-            if darkBackground:
-                testimage = np.logical_not(testimage)
-            testimage = testimage.astype(np.uint8)
-            g.currentWindow.imageview.setImage(testimage, autoLevels=False)
-            g.currentWindow.imageview.setLevels(-.1, 1.1)
-        else:
-            g.currentWindow.reset()
-            if nDim == 3:
-                image = g.currentWindow.image[g.currentWindow.currentIndex]
-            else:
-                image = g.currentWindow.image
-            g.currentWindow.imageview.setLevels(np.min(image), np.max(image))
-adaptive_threshold=Adaptive_threshold()
-
-
-class Canny_edge_detector(BaseProcess):
-    """canny_edge_detector(sigma, keepSourceWindow=False)
-    
-    Parameters:
-        | sigma (float) -- 
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        sigma=SliderLabel(2)
-        if g.currentWindow is not None:
-            sigma.setRange(0,1000)
-            sigma.setValue(1)
-        preview=CheckBox(); preview.setChecked(True)
-        self.items.append({'name':'sigma','string':'Sigma','object':sigma})
-        self.items.append({'name':'preview','string':'Preview','object':preview})
-        super().gui()
-        self.preview()
-    def __call__(self,sigma, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        nDim=len(self.tif.shape) 
-        newtif=np.copy(self.tif)
-
-        if self.tif.dtype == np.float16:
-            g.alert("Canny Edge Detection does not work on float32 images. Change the data type to use this function.")
-            return None
-
-        if nDim==2:
-            newtif=feature.canny(self.tif,sigma)
-        else:
-            for i in np.arange(len(newtif)):
-                newtif[i] = feature.canny(self.tif[i],sigma)
-        self.newtif=newtif.astype(np.uint8)
-        self.newname=self.oldname+' - Canny '
-        return self.end()
-    def preview(self):
-        sigma=self.getValue('sigma')
-        preview=self.getValue('preview')
-        nDim=len(g.currentWindow.image.shape)
-        if preview:
-            if nDim==3: # if the image is 3d
-                testimage=np.copy(g.currentWindow.image[g.currentWindow.currentIndex])
-            elif nDim==2:
-                testimage=np.copy(g.currentWindow.image)
-            testimage=feature.canny(testimage,sigma)
-            g.currentWindow.imageview.setImage(testimage,autoLevels=False)
-            g.currentWindow.imageview.setLevels(-.1,1.1)
-        else:
-            g.currentWindow.reset()
-            if nDim==3:
-                image=g.currentWindow.image[g.currentWindow.currentIndex]
-            else:
-                image=g.currentWindow.image
-            g.currentWindow.imageview.setLevels(np.min(image),np.max(image))
-canny_edge_detector=Canny_edge_detector()
-
-
-class Logically_combine(BaseProcess):
-    """ logically_combine(window1, window2,operator, keepSourceWindow=False)
-    Combines two windows according to the operator
-    
-    Parameters:
-        | window1 (Window)
-        | window2 (Window)
-        | operator (str)
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        window1=WindowSelector()
-        window2=WindowSelector()
-        operator=ComboBox()
-        operator.addItem('AND')
-        operator.addItem('OR')
-        operator.addItem('XOR')
-        self.items.append({'name':'window1','string':'Window 1','object':window1})
-        self.items.append({'name':'window2','string':'Window 2','object':window2})
-        self.items.append({'name':'operator','string':'Operator','object':operator})
-        super().gui()
-    def __call__(self,window1, window2,operator,keepSourceWindow=False):
-        self.keepSourceWindow=keepSourceWindow
-        g.m.statusBar().showMessage('Performing {}...'.format(self.__name__))
-        if window1 is None or window2 is None:
-            raise(MissingWindowError("You cannot execute '{}' without selecting a window first.".format(self.__name__)))
-        if window1.image.shape!=window2.image.shape:
-            g.m.statusBar().showMessage('The two windows have images of different shapes. They could not be combined')
-            return None
-        if operator=='AND':
-            self.newtif=np.logical_and(window1.image,window2.image)
-        elif operator=='OR':
-            self.newtif=np.logical_or(window1.image,window2.image)
-        elif operator=='XOR':
-            self.newtif=np.logical_xor(window1.image,window2.image)
-            
-        self.oldwindow=window1
-        self.oldname=window1.name
-        self.newname=self.oldname+' - Logical {}'.format(operator)
-        if keepSourceWindow is False:
-            window2.close()
-        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
-        return self.end()
-logically_combine=Logically_combine()
-
-    
-class Remove_small_blobs(BaseProcess):
-    """remove_small_blobs(rank, value, keepSourceWindow=False)
-    Finds all contiguous 'True' pixels in rank dimensions.  Removes regions which have fewer than the specified pixels.
-    
-    Parameters:
-        | rank  (int) -- The number of dimensions.  If rank==2, each frame is treated independently
-        | value (int) -- The size (in pixels) below which each contiguous region must be in order to be discarded.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-
-    def gui(self):
-        self.gui_reset()
-        rank = QtWidgets.QSpinBox()
-        rank.setRange(2,3)
-        value = QtWidgets.QSpinBox()
-        value.setRange(1, 100000)
-        self.items.append({'name': 'rank', 'string': 'Number of Dimensions', 'object': rank})
-        self.items.append({'name': 'value', 'string': 'Value', 'object': value})
-        super().gui()
-
-    def __call__(self, rank, value, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.tif.dtype == np.float16:
-            g.alert("remove_small_blobs() does not support float16 type arrays")
-            return
-        oldshape = self.tif.shape
-        newtif = np.zeros_like(self.tif, dtype='bool')
-        if self.oldwindow.nDims == 2:
-            newtif = remove_small_objects(self.tif.astype('bool'), value, connectivity=2)
-        elif self.oldwindow.nDims == 3:
-            if rank == 2:
-                for i in np.arange(len(self.tif)):
-                    newtif[i] = remove_small_objects(self.tif[i].astype('bool'), value, connectivity=2)
-            elif rank == 3:
-                newtif = remove_small_objects(self.tif.astype('bool'), value, connectivity=2)
-        self.newtif = newtif
-        self.newname = self.oldname + ' - Removed Blobs ' + str(value)
-        return self.end()
-
-    def get_init_settings_dict(self):
-        s = dict()
-        s['rank'] = 2
-        s['value'] = 1
-        return s
-
-remove_small_blobs = Remove_small_blobs()
-
-
-class Binary_Dilation(BaseProcess):
-    """binary_dilation(rank,connectivity,iterations, keepSourceWindow=False)
-    Performs a binary dilation on a binary image.  The 'False' pixels neighboring 'True' pixels become converted to 'True' pixels.
-    
-    Parameters:
-        | rank (int) -- The number of dimensions to dilate. Can be either 2 or 3.  
-        | connectivity (int) -- `connectivity` determines the distance to dilate.
-             `connectivity` may range from 1 (no diagonal elements are neighbors) 
-             to `rank` (all elements are neighbors).
-        | iterations (int) -- How many times to repeat the dilation
-        | keepSourceWindow (bool) -- If this is False, a new Window is created with the result. Otherwise, the currentWindow is used
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        rank=QtWidgets.QSpinBox()
-        rank.setRange(2,3)
-        connectivity=QtWidgets.QSpinBox()
-        connectivity.setRange(1,3)
-        iterations=QtWidgets.QSpinBox()
-        iterations.setRange(1,100)
-        self.items.append({'name':'rank','string':'Number of Dimensions','object':rank})
-        self.items.append({'name':'connectivity','string':'Connectivity','object':connectivity})
-        self.items.append({'name':'iterations','string':'Iterations','object':iterations})
-
-        super().gui()
-    def __call__(self,rank,connectivity,iterations, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.tif.dtype == np.float16:
-            g.alert("Adaptive Threshold does not support float16 type arrays")
-            return
-        if len(self.tif.shape)==3 and rank==2:
-            s=scipy.ndimage.generate_binary_structure(3,connectivity)
-            s[0]=False
-            s[2]=False
-        else:
-            s=scipy.ndimage.generate_binary_structure(rank,connectivity)
-        self.newtif=scipy.ndimage.morphology.binary_dilation(self.tif,s,iterations)
-        self.newtif=self.newtif.astype(np.uint8)
-        self.newname=self.oldname+' - Dilated '
-        return self.end()
-binary_dilation=Binary_Dilation()
-
-
-class Binary_Erosion(BaseProcess):
-    """binary_erosion(rank,connectivity,iterations, keepSourceWindow=False)
-    Performs a binary erosion on a binary image.  The 'True' pixels neighboring 'False' pixels become converted to 'False' pixels.
-    
-    Parameters:
-        | rank (int) -- The number of dimensions to erode. Can be either 2 or 3.  
-        | connectivity (int) -- `connectivity` determines the distance to erode.
-             `connectivity` may range from 1 (no diagonal elements are neighbors) 
-             to `rank` (all elements are neighbors).
-        | iterations (int) -- How many times to repeat the erosion
-        | keepSourceWindow (bool) -- If this is False, a new Window is created with the result. Otherwise, the currentWindow is used
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        rank=QtWidgets.QSpinBox()
-        rank.setRange(2,3)
-        connectivity=QtWidgets.QSpinBox()
-        connectivity.setRange(1,3)
-        iterations=QtWidgets.QSpinBox()
-        iterations.setRange(1,100)
-        self.items.append({'name':'rank','string':'Number of Dimensions','object':rank})
-        self.items.append({'name':'connectivity','string':'Connectivity','object':connectivity})
-        self.items.append({'name':'iterations','string':'Iterations','object':iterations})
-
-        super().gui()
-    def __call__(self,rank,connectivity,iterations, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.tif.dtype == np.float16:
-            g.alert("Binary Erosion does not work on float32 images. Change the data type to use this function.")
-            return None
-        if len(self.tif.shape)==3 and rank==2:
-            s=scipy.ndimage.generate_binary_structure(3,connectivity)
-            s[0]=False
-            s[2]=False
-        else:
-            s=scipy.ndimage.generate_binary_structure(rank,connectivity)
-        self.newtif=scipy.ndimage.morphology.binary_erosion(self.tif,s,iterations)
-        self.newtif=self.newtif.astype(np.uint8)
-        self.newname=self.oldname+' - Dilated '
-        return self.end()
-binary_erosion=Binary_Erosion()
-
-
-class Generate_ROIs(BaseProcess):
-    """generate_rois(level, keepSourceWindow=False)
-    Uses a binary image to create ROIs from positive clusters.
-    
-    Parameters:
-        | level (float) - value in [0, 1] to use when finding contours
-        | keepSourceWindow (bool) -- If this is False, a new Window is created with the result. Otherwise, the currentWindow is used
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-        self.ROIs = []
-    def gui(self):
-        self.gui_reset()
-        self.previewing = False
-        self.toPreview = False
-        level=SliderLabel(2)
-        level.setRange(0,1)
-        level.setValue(.5)
-        minDensity=QtWidgets.QSpinBox()
-        minDensity.setRange(4, 1000)
-        self.items.append({'name':'level','string':'Contour Level','object':level})
-        self.items.append({'name':'minDensity','string':'Minimum Density','object':minDensity})
-        self.ROIs = []
-        super().gui()
-        self.ui.rejected.connect(self.removeROIs)
-
-    def removeROIs(self):
-        for roi in self.ROIs:
-            roi.cancel()
-        self.ROIs = []
-
-    def __call__(self, level, minDensity, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.tif.dtype == np.float16:
-            g.alert("Adaptive Threshold does not support float16 type arrays")
-            return
-        for roi in self.ROIs:
-            roi.cancel()
-        self.ROIs = []
-
-        im = g.currentWindow.image if g.currentWindow.image.ndim == 2 else g.currentWindow.image[g.currentWindow.currentIndex]
-        im = scipy.ndimage.morphology.binary_closing(im)
-        if np.any(im < 0) or np.any(im > 1):
-            raise Exception("The current image is not a binary image. Threshold first")
-
-        thresholded_image = np.squeeze(im)
-        labelled=measure.label(thresholded_image)
-        ROIs = []
-        for i in range(1, np.max(labelled)+1):
-            if np.sum(labelled == i) >= minDensity:
-                im = scipy.ndimage.morphology.binary_dilation(scipy.ndimage.morphology.binary_closing(labelled == i))
-                outline_coords = measure.find_contours(im, level)
-                if len(outline_coords) == 0:
-                    continue
-                outline_coords = outline_coords[0]
-                new_roi = makeROI("freehand", outline_coords)
-                ROIs.append(new_roi)
-
-    def preview(self):
-        if self.previewing:
-            self.toPreview = True
-            return
-        self.previewing = True
-        im = g.currentWindow.image if g.currentWindow.image.ndim == 2 else g.currentWindow.image[g.currentWindow.currentIndex]
-        im = scipy.ndimage.morphology.binary_closing(im)
-        if np.any(im < 0) or np.any(im > 1):
-            raise Exception("The current image is not a binary image. Threshold first")
-
-        level = self.getValue('level')
-        minDensity = self.getValue('minDensity')
-        thresholded_image = np.squeeze(im)
-        labelled=measure.label(thresholded_image)
-        for roi in self.ROIs:
-            roi.cancel()
-        self.ROIs = []
-
-        for i in range(1, np.max(labelled)+1):
-            QtWidgets.qApp.processEvents()
-            if np.sum(labelled == i) >= minDensity:
-                im = scipy.ndimage.morphology.binary_dilation(scipy.ndimage.morphology.binary_closing(labelled == i))
-                outline_coords = measure.find_contours(im, level)
-                if len(outline_coords) == 0:
-                    continue
-                outline_coords = outline_coords[0]
-                self.ROIs.append(ROI_Drawing(g.currentWindow, outline_coords[0][0], outline_coords[0][1], 'freehand'))
-                for p in outline_coords[1:]:
-                    self.ROIs[-1].extend(p[0], p[1])
-                    QtWidgets.qApp.processEvents()
-
-        self.previewing = False
-        if self.toPreview:
-            self.toPreview = False
-            self.preview()
-
-generate_rois = Generate_ROIs()
-
-
-
-
-
-
-
-
-
-
-
-
-
-    
-    
+# -*- coding: utf-8 -*-
+import numpy as np
+import scipy
+import scipy.ndimage
+import skimage
+from skimage import feature, measure
+from skimage.filters import threshold_local
+from skimage.morphology import remove_small_objects
+from qtpy import QtCore, QtGui, QtWidgets
+from .. import global_vars as g
+from ..utils.BaseProcess import BaseProcess, SliderLabel, WindowSelector,  MissingWindowError, CheckBox, ComboBox
+from ..roi import makeROI, ROI_Drawing
+
+__all__ = ['threshold','remove_small_blobs','adaptive_threshold','logically_combine','binary_dilation','binary_erosion', 'generate_rois', 'canny_edge_detector']
+     
+     
+def convert2uint8(tif):
+    oldmin = np.min(tif)
+    oldmax = np.max(tif)
+    newmax = 2**8-1
+    tif = ((tif-oldmin)*newmax)/(oldmax-oldmin)
+    tif = tif.astype(np.uint8)
+    return tif
+    
+class Threshold(BaseProcess):
+    """threshold(value, darkBackground=False, keepSourceWindow=False)
+
+    Creates a boolean matrix by applying a threshold
+    
+    Parameters:
+        value (float): The threshold to be applied
+        darkBackground (bool): If this is True, pixels below the threshold will be True
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        self.gui_reset()
+        valueSlider = SliderLabel(2)
+        if g.win is not None:
+            image=g.win.image
+            valueSlider.setRange(np.min(image),np.max(image))
+            valueSlider.setValue(np.mean(image))
+        preview=CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name': 'value','string': 'Value','object': valueSlider})
+        self.items.append({'name': 'darkBackground', 'string':'Dark Background','object': CheckBox()})
+        self.items.append({'name': 'preview','string': 'Preview','object': preview})
+        super().gui()
+
+    def __call__(self, value, darkBackground=False, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.oldwindow.nDims > 3:
+            g.alert("You cannot run this function on an image of dimension greater than 3. If your window has color, convert to a grayscale image before running this function")
+            return None
+        if darkBackground:
+            newtif = self.tif < value
+        else:
+            newtif = self.tif > value
+        self.newtif = newtif.astype(np.uint8)
+        self.newname = self.oldname+' - Thresholded '+str(value)
+        return self.end()
+
+    def preview(self):
+        if g.win is None or g.win.closed:
+            return
+        win = g.win
+        value = self.getValue('value')
+        preview = self.getValue('preview')
+        darkBackground = self.getValue('darkBackground')
+        if win.nDims > 3:
+            g.alert("You cannot run this function on an image of dimension greater than 3. If your window has color, convert to a grayscale image before running this function")
+            return None
+        if preview:
+            if win.nDims == 3: # if the image is 3d
+                testimage = np.copy(win.image[win.currentIndex])
+            elif win.nDims == 2:
+                testimage = np.copy(win.image)
+            if darkBackground:
+                testimage = testimage<value
+            else:
+                testimage = testimage>value
+            win.imageview.setImage(testimage, autoLevels=False)
+            win.imageview.setLevels(-.1,1.1)
+        else:
+            win.reset()
+            if win.nDims == 3:
+                image = win.image[win.currentIndex]
+            else:
+                image = win.image
+            win.imageview.setLevels(np.min(image), np.max(image))
+threshold = Threshold()
+
+class BlocksizeSlider(SliderLabel):
+    def __init__(self,demicals=0):
+        SliderLabel.__init__(self,demicals)
+    def updateSlider(self,value):
+        if value%2==0:
+            if value<self.slider.value():
+                value-=1
+            else:
+                value+=1
+            self.label.setValue(value)
+        self.slider.setValue(int(value*10**self.decimals))
+    def updateLabel(self,value):
+        if value%2==0:
+            value-=1
+        self.label.setValue(value)
+    
+class Adaptive_threshold(BaseProcess):
+    """adaptive_threshold(value, block_size, darkBackground=False, keepSourceWindow=False)
+
+    Creates a boolean matrix by applying an adaptive threshold using the scikit-image threshold_local function
+    
+    Parameters:
+        value (int): The threshold to be applied
+        block_size (int): size of a pixel neighborhood that is used to calculate a threshold value for the pixel. Must be an odd number greater than 3.
+        darkBackground (bool): If this is True, pixels below the threshold will be True
+
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        valueSlider=SliderLabel(2)
+        valueSlider.setRange(-20,20)
+        valueSlider.setValue(0)
+        block_size=BlocksizeSlider(0)
+        if g.win is not None:
+            max_block = int(max([g.win.image.shape[-1],g.win.image.shape[-2]])/2)
+        else:
+            max_block = 100
+        block_size.setRange(3, max_block)
+        preview = CheckBox(); preview.setChecked(True)
+        self.items.append({'name': 'value', 'string': 'Value', 'object': valueSlider})
+        self.items.append({'name': 'block_size', 'string':'Block Size', 'object':block_size})
+        self.items.append({'name': 'darkBackground', 'string': 'Dark Background', 'object': CheckBox()})
+        self.items.append({'name': 'preview', 'string': 'Preview', 'object': preview})
+        super().gui()
+        self.preview()
+
+    def __call__(self, value, block_size, darkBackground=False, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.tif.dtype == np.float16:
+            g.alert("Local Threshold does not support float16 type arrays")
+            return
+        newtif = np.copy(self.tif)
+
+        if self.oldwindow.nDims == 2:
+            newtif = threshold_local(newtif, block_size, offset=value)
+        elif self.oldwindow.nDims == 3:
+            for i in np.arange(len(newtif)):
+                newtif[i] = threshold_local(newtif[i], block_size, offset=value)
+        else:
+            g.alert("You cannot run this function on an image of dimension greater than 3. If your window has color, convert to a grayscale image before running this function")
+            return None
+        if darkBackground:
+            newtif = np.logical_not(newtif)
+        self.newtif = newtif.astype(np.uint8)
+        self.newname = self.oldname + ' - Thresholded ' + str(value)
+        return self.end()
+
+    def preview(self):
+        if g.win is None or g.win.closed:
+            return
+        win = g.win
+        value = self.getValue('value')
+        block_size = self.getValue('block_size')
+        preview = self.getValue('preview')
+        darkBackground = self.getValue('darkBackground')
+        nDim = len(win.image.shape)
+        if nDim > 3:
+            g.alert("You cannot run this function on an image of dimension greater than 3. If your window has color, convert to a grayscale image before running this function")
+            return None
+        if preview:
+            if nDim == 3: # if the image is 3d
+                testimage=np.copy(win.image[win.currentIndex])
+            elif nDim == 2:
+                testimage=np.copy(win.image)
+            testimage = threshold_local(testimage, block_size, offset=value)
+            if darkBackground:
+                testimage = np.logical_not(testimage)
+            testimage = testimage.astype(np.uint8)
+            win.imageview.setImage(testimage, autoLevels=False)
+            win.imageview.setLevels(-.1, 1.1)
+        else:
+            win.reset()
+            if nDim == 3:
+                image = win.image[win.currentIndex]
+            else:
+                image = win.image
+            win.imageview.setLevels(np.min(image), np.max(image))
+adaptive_threshold=Adaptive_threshold()
+
+
+class Canny_edge_detector(BaseProcess):
+    """canny_edge_detector(sigma, keepSourceWindow=False)
+    
+    Parameters:
+        sigma (float):
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        sigma=SliderLabel(2)
+        if g.win is not None:
+            sigma.setRange(0,1000)
+            sigma.setValue(1)
+        preview=CheckBox(); preview.setChecked(True)
+        self.items.append({'name':'sigma','string':'Sigma','object':sigma})
+        self.items.append({'name':'preview','string':'Preview','object':preview})
+        super().gui()
+        self.preview()
+    def __call__(self,sigma, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        nDim=len(self.tif.shape) 
+        newtif=np.copy(self.tif)
+
+        if self.tif.dtype == np.float16:
+            g.alert("Canny Edge Detection does not work on float32 images. Change the data type to use this function.")
+            return None
+
+        if nDim==2:
+            newtif=feature.canny(self.tif,sigma)
+        else:
+            for i in np.arange(len(newtif)):
+                newtif[i] = feature.canny(self.tif[i],sigma)
+        self.newtif=newtif.astype(np.uint8)
+        self.newname=self.oldname+' - Canny '
+        return self.end()
+
+    def preview(self):
+        if g.win is None or g.win.closed:
+            return
+        win = g.win
+        sigma = self.getValue('sigma')
+        preview = self.getValue('preview')
+        nDim = len(win.image.shape)
+        if preview:
+            if nDim==3: # if the image is 3d
+                testimage=np.copy(win.image[win.currentIndex])
+            elif nDim==2:
+                testimage=np.copy(win.image)
+            testimage=feature.canny(testimage,sigma)
+            win.imageview.setImage(testimage,autoLevels=False)
+            win.imageview.setLevels(-.1,1.1)
+        else:
+            win.reset()
+            if nDim==3:
+                image=win.image[win.currentIndex]
+            else:
+                image=win.image
+            win.imageview.setLevels(np.min(image),np.max(image))
+canny_edge_detector=Canny_edge_detector()
+
+
+class Logically_combine(BaseProcess):
+    """logically_combine(window1, window2,operator, keepSourceWindow=False)
+
+    Combines two windows according to the operator
+    
+    Parameters:
+        window1 (Window)
+        window2 (Window)
+        operator (str)
+
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        window1=WindowSelector()
+        window2=WindowSelector()
+        operator=ComboBox()
+        operator.addItem('AND')
+        operator.addItem('OR')
+        operator.addItem('XOR')
+        self.items.append({'name':'window1','string':'Window 1','object':window1})
+        self.items.append({'name':'window2','string':'Window 2','object':window2})
+        self.items.append({'name':'operator','string':'Operator','object':operator})
+        super().gui()
+    def __call__(self,window1, window2,operator,keepSourceWindow=False):
+        self.keepSourceWindow=keepSourceWindow
+        g.m.statusBar().showMessage('Performing {}...'.format(self.__name__))
+        if window1 is None or window2 is None:
+            raise(MissingWindowError("You cannot execute '{}' without selecting a window first.".format(self.__name__)))
+        if window1.image.shape!=window2.image.shape:
+            g.m.statusBar().showMessage('The two windows have images of different shapes. They could not be combined')
+            return None
+        if operator=='AND':
+            self.newtif=np.logical_and(window1.image,window2.image)
+        elif operator=='OR':
+            self.newtif=np.logical_or(window1.image,window2.image)
+        elif operator=='XOR':
+            self.newtif=np.logical_xor(window1.image,window2.image)
+            
+        self.oldwindow=window1
+        self.oldname=window1.name
+        self.newname=self.oldname+' - Logical {}'.format(operator)
+        if keepSourceWindow is False:
+            window2.close()
+        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
+        return self.end()
+logically_combine=Logically_combine()
+
+    
+class Remove_small_blobs(BaseProcess):
+    """remove_small_blobs(rank, value, keepSourceWindow=False)
+
+    Finds all contiguous 'True' pixels in rank dimensions.  Removes regions which have fewer than the specified pixels.
+    
+    Parameters:
+        rank  (int): The number of dimensions.  If rank==2, each frame is treated independently
+        value (int): The size (in pixels) below which each contiguous region must be in order to be discarded.
+
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        self.gui_reset()
+        rank = QtWidgets.QSpinBox()
+        rank.setRange(2,3)
+        value = QtWidgets.QSpinBox()
+        value.setRange(1, 100000)
+        self.items.append({'name': 'rank', 'string': 'Number of Dimensions', 'object': rank})
+        self.items.append({'name': 'value', 'string': 'Value', 'object': value})
+        super().gui()
+
+    def __call__(self, rank, value, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.tif.dtype == np.float16:
+            g.alert("remove_small_blobs() does not support float16 type arrays")
+            return
+        oldshape = self.tif.shape
+        newtif = np.zeros_like(self.tif, dtype='bool')
+        if self.oldwindow.nDims == 2:
+            newtif = remove_small_objects(self.tif.astype('bool'), value, connectivity=2)
+        elif self.oldwindow.nDims == 3:
+            if rank == 2:
+                for i in np.arange(len(self.tif)):
+                    newtif[i] = remove_small_objects(self.tif[i].astype('bool'), value, connectivity=2)
+            elif rank == 3:
+                newtif = remove_small_objects(self.tif.astype('bool'), value, connectivity=2)
+        self.newtif = newtif
+        self.newname = self.oldname + ' - Removed Blobs ' + str(value)
+        return self.end()
+
+    def get_init_settings_dict(self):
+        s = dict()
+        s['rank'] = 2
+        s['value'] = 1
+        return s
+
+remove_small_blobs = Remove_small_blobs()
+
+
+class Binary_Dilation(BaseProcess):
+    """binary_dilation(rank,connectivity,iterations, keepSourceWindow=False)
+
+    Performs a binary dilation on a binary image.  The 'False' pixels neighboring 'True' pixels become converted to 'True' pixels.
+
+    Parameters:
+        rank (int): The number of dimensions to dilate. Can be either 2 or 3.
+        connectivity (int): `connectivity` determines the distance to dilate.
+             `connectivity` may range from 1 (no diagonal elements are neighbors) 
+             to `rank` (all elements are neighbors).
+        iterations (int): How many times to repeat the dilation
+        keepSourceWindow (bool): If this is False, a new Window is created with the result. Otherwise, the currentWindow is used
+
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        rank=QtWidgets.QSpinBox()
+        rank.setRange(2,3)
+        connectivity=QtWidgets.QSpinBox()
+        connectivity.setRange(1,3)
+        iterations=QtWidgets.QSpinBox()
+        iterations.setRange(1,100)
+        self.items.append({'name':'rank','string':'Number of Dimensions','object':rank})
+        self.items.append({'name':'connectivity','string':'Connectivity','object':connectivity})
+        self.items.append({'name':'iterations','string':'Iterations','object':iterations})
+
+        super().gui()
+    def __call__(self,rank,connectivity,iterations, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.tif.dtype == np.float16:
+            g.alert("binary_dilation does not support float16 type arrays")
+            return
+        if len(self.tif.shape)==3 and rank==2:
+            s=scipy.ndimage.generate_binary_structure(3,connectivity)
+            s[0]=False
+            s[2]=False
+        else:
+            s=scipy.ndimage.generate_binary_structure(rank,connectivity)
+        self.newtif=scipy.ndimage.morphology.binary_dilation(self.tif,s,iterations)
+        self.newtif=self.newtif.astype(np.uint8)
+        self.newname=self.oldname+' - Dilated '
+        return self.end()
+binary_dilation=Binary_Dilation()
+
+
+class Binary_Erosion(BaseProcess):
+    """binary_erosion(rank,connectivity,iterations, keepSourceWindow=False)
+
+    Performs a binary erosion on a binary image.  The 'True' pixels neighboring 'False' pixels become converted to 'False' pixels.
+    
+    Parameters:
+        rank (int): The number of dimensions to erode. Can be either 2 or 3.
+        connectivity (int): `connectivity` determines the distance to erode. `connectivity` may range from 1 (no diagonal elements are neighbors) to `rank` (all elements are neighbors).
+        iterations (int): How many times to repeat the erosion
+        keepSourceWindow (bool): If this is False, a new Window is created with the result. Otherwise, the currentWindow is used
+
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        self.gui_reset()
+        rank=QtWidgets.QSpinBox()
+        rank.setRange(2,3)
+        connectivity=QtWidgets.QSpinBox()
+        connectivity.setRange(1,3)
+        iterations=QtWidgets.QSpinBox()
+        iterations.setRange(1,100)
+        self.items.append({'name':'rank','string':'Number of Dimensions','object':rank})
+        self.items.append({'name':'connectivity','string':'Connectivity','object':connectivity})
+        self.items.append({'name':'iterations','string':'Iterations','object':iterations})
+
+        super().gui()
+    def __call__(self, rank, connectivity, iterations, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.tif.dtype == np.float16:
+            g.alert("Binary Erosion does not work on float32 images. Change the data type to use this function.")
+            return None
+        if len(self.tif.shape)==3 and rank==2:
+            s = scipy.ndimage.generate_binary_structure(3, connectivity)
+            s[0] = False
+            s[2] = False
+        else:
+            s = scipy.ndimage.generate_binary_structure(rank, connectivity)
+        self.newtif = scipy.ndimage.morphology.binary_erosion(self.tif, s, iterations)
+        self.newtif = self.newtif.astype(np.uint8)
+        self.newname = self.oldname+' - Dilated '
+        return self.end()
+binary_erosion=Binary_Erosion()
+
+
+class Generate_ROIs(BaseProcess):
+    """generate_rois(level, keepSourceWindow=False)
+
+    Uses a binary image to create ROIs from positive clusters.
+    
+    Parameters:
+        level (float): value in [0, 1] to use when finding contours
+        keepSourceWindow (bool): If this is False, a new Window is created with the result. Otherwise, the currentWindow is used
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+        self.ROIs = []
+
+    def gui(self):
+        self.gui_reset()
+        level=SliderLabel(2)
+        level.setRange(0,1)
+        level.setValue(.5)
+        minDensity=QtWidgets.QSpinBox()
+        minDensity.setRange(4, 1000)
+        preview=CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name':'level','string':'Contour Level','object':level})
+        self.items.append({'name':'minDensity','string':'Minimum Density','object':minDensity})
+        self.items.append({'name': 'preview','string': 'Preview','object': preview})
+        self.ROIs = []
+        super().gui()
+        self.ui.rejected.connect(self.removeROIs)
+
+    def removeROIs(self):
+        for roi in self.ROIs:
+            roi.cancel()
+        self.ROIs = []
+
+    def __call__(self, level, minDensity, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.tif.dtype == np.float16:
+            g.alert("generate_rois does not support float16 type arrays")
+            return None
+        if not np.all((self.tif == 0) | (self.tif == 1)):
+            g.alert("The current image is not a binary image. Threshold first")
+            return None
+        for roi in self.ROIs:
+            roi.cancel()
+        self.ROIs = []
+
+        im = g.win.image if g.win.image.ndim == 2 else g.win.image[g.win.currentIndex]
+        im = scipy.ndimage.morphology.binary_closing(im)
+        thresholded_image = np.squeeze(im)
+        labelled = measure.label(thresholded_image)
+        ROIs = []
+        for i in range(1, np.max(labelled)+1):
+            if np.sum(labelled == i) >= minDensity:
+                im = scipy.ndimage.morphology.binary_dilation(scipy.ndimage.morphology.binary_closing(labelled == i))
+                outline_coords = measure.find_contours(im, level)
+                if len(outline_coords) == 0:
+                    continue
+                outline_coords = outline_coords[0]
+                new_roi = makeROI("freehand", outline_coords)
+                ROIs.append(new_roi)
+
+    def preview(self):
+        if g.win is None or g.win.closed:
+            return
+        win = g.win
+        im = win.image if win.image.ndim == 2 else win.image[win.currentIndex]
+        if not np.all((im == 0) | (im == 1)):
+            g.alert("The current image is not a binary image. Threshold first")
+            return None
+        im = scipy.ndimage.morphology.binary_closing(im)
+        level = self.getValue('level')
+        minDensity = self.getValue('minDensity')
+        thresholded_image = np.squeeze(im)
+        labelled=measure.label(thresholded_image)
+        for roi in self.ROIs:
+            roi.cancel()
+        self.ROIs = []
+
+        for i in range(1, np.max(labelled)+1):
+            QtWidgets.QApplication.processEvents()
+            if np.sum(labelled == i) >= minDensity:
+                im = scipy.ndimage.morphology.binary_dilation(scipy.ndimage.morphology.binary_closing(labelled == i))
+                outline_coords = measure.find_contours(im, level)
+                if len(outline_coords) == 0:
+                    continue
+                outline_coords = outline_coords[0]
+                self.ROIs.append(ROI_Drawing(win, outline_coords[0][0], outline_coords[0][1], 'freehand'))
+                for p in outline_coords[1:]:
+                    self.ROIs[-1].extend(p[0], p[1])
+                    QtWidgets.QApplication.processEvents()
+
+generate_rois = Generate_ROIs()
+
+
+
+
+
+
+
+
+
+
+
+
+
+    
+
```

### Comparing `flika-0.2.9/flika/process/file_.py` & `flika-0.3.0/flika/process/file_.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,501 +1,649 @@
-# -*- coding: utf-8 -*-
-import pyqtgraph as pg
-import pyqtgraph.exporters
-import time
-import os.path
-import numpy as np
-from qtpy import uic, QtGui, QtCore, QtWidgets
-import codecs
-import shutil, subprocess
-import json
-import re
-import nd2reader
-import datetime
-import json
-import pip
-import re
-
-from .. import global_vars as g
-from ..app.script_editor import ScriptEditor
-from .BaseProcess import BaseDialog
-from ..window import Window
-from ..utils.misc import open_file_gui, save_file_gui
-from ..utils.io import tifffile
-
-__all__ = ['save_file', 'save_points', 'save_movie_gui', 'open_file', 'open_file_from_gui', 'open_points', 'close']
-
-########################################################################################################################
-######################                  SAVING FILES                                         ###########################
-########################################################################################################################
-
-
-
-def save_file(filename=None):
-    """
-    Save the image in the currentWindow to a .tif file.
-
-    Parameters
-    ----------
-    filename : str
-        The image or movie will be saved here.
-
-    """
-    if filename is None or filename is False:
-        filetypes = '*.tif'
-        prompt = 'Save File As Tif'
-        filename = save_file_gui(prompt, filetypes=filetypes)
-        if filename is None:
-            return None
-    if os.path.dirname(filename) == '':  # if the user didn't specify a directory
-        directory = os.path.normpath(os.path.dirname(g.settings['filename']))
-        filename = os.path.join(directory, filename)
-    g.m.statusBar().showMessage('Saving {}'.format(os.path.basename(filename)))
-    A = g.currentWindow.image
-    metadata = g.currentWindow.metadata
-    try:
-        metadata = json.dumps(metadata, default=JSONhandler)
-    except TypeError as e:
-        msg = "Error saving metadata.\n{}\nContinuing to save file".format(e)
-        g.alert(msg)
-    if len(A.shape) == 3:
-        A = np.transpose(A, (0, 2, 1))  # This keeps the x and the y the same as in FIJI
-    elif len(A.shape) == 2:
-        A = np.transpose(A, (1, 0))
-    tifffile.imsave(filename, A,
-                    description=metadata)  # http://stackoverflow.com/questions/20529187/what-is-the-best-way-to-save-image-metadata-alongside-a-tif-with-python
-    g.m.statusBar().showMessage('Successfully saved {}'.format(os.path.basename(filename)))
-    return filename
-
-def save_points(filename=None):
-    if filename is None:
-        filetypes = '*.txt'
-        prompt = 'Save Points'
-        filename = save_file_gui(prompt, filetypes=filetypes)
-        if filename is None:
-            return None
-    g.m.statusBar().showMessage('Saving Points in {}'.format(os.path.basename(filename)))
-    p_out = []
-    p_in = g.currentWindow.scatterPoints
-    for t in np.arange(len(p_in)):
-        for p in p_in[t]:
-            p_out.append(np.array([t, p[0], p[1]]))
-    p_out = np.array(p_out)
-    np.savetxt(filename, p_out)
-    g.m.statusBar().showMessage('Successfully saved {}'.format(os.path.basename(filename)))
-    return filename
-
-
-def save_movie_gui():
-    rateSpin = pg.SpinBox(value=50, bounds=[1, 1000], suffix='fps', int=True, step=1)
-    rateDialog = BaseDialog([{'string': 'Framerate', 'object': rateSpin}], 'Save Movie', 'Set the framerate')
-    rateDialog.accepted.connect(lambda: save_movie(rateSpin.value()))
-    g.dialogs.append(rateDialog)
-    rateDialog.show()
-
-
-def save_movie(rate, filename=None):
-    """save_movie(rate, filename)
-    Saves the currentWindow video as a .mp4 movie by joining .jpg frames together
-
-    Parameters:
-        | rate (int) -- framerate
-        | filename (str) -- Address to save the movie to, with .mp4
-
-    Notes:
-        | Once you've exported all of the frames you wanted, open a command line and run the following:
-        |   ffmpeg -r 100 -i %03d.jpg output.mp4
-        | -r: framerate
-        | -i: input files.
-        | %03d: The files have to be numbered 001.jpg, 002.jpg... etc.
-    """
-
-
-    ## Check if ffmpeg is installed
-    if os.name == 'nt':  # If we are running windows
-        try:
-            subprocess.call(["ffmpeg"])
-        except FileNotFoundError as e:
-            if e.errno == os.errno.ENOENT:
-                # handle file not found error.
-                # I used http://ffmpeg.org/releases/ffmpeg-2.8.4.tar.bz2 originally
-                g.alert("The program FFmpeg is required to export movies. \
-                \n\nFor instructions on how to install, go here: http://www.wikihow.com/Install-FFmpeg-on-Windows")
-                return None
-            else:
-                # Something else went wrong while trying to run `wget`
-                raise
-
-    filetypes = "Movies (*.mp4)"
-    prompt = "Save movie to .mp4 file"
-    filename = save_file_gui(prompt, filetypes=filetypes)
-    if filename is None:
-        return None
-
-    win = g.currentWindow
-    A = win.image
-    if len(A.shape) < 3:
-        g.alert('Movie not the right shape for saving.')
-        return None
-    try:
-        exporter = pg.exporters.ImageExporter(win.imageview.view)
-    except TypeError:
-        exporter = pg.exporters.ImageExporter.ImageExporter(win.imageview.view)
-
-    nFrames = len(A)
-    tmpdir = os.path.join(os.path.dirname(g.settings.config_file), 'tmp')
-    if os.path.isdir(tmpdir):
-        shutil.rmtree(tmpdir)
-    os.mkdir(tmpdir)
-    win.top_left_label.hide()
-    for i in np.arange(0, nFrames):
-        win.setIndex(i)
-        exporter.export(os.path.join(tmpdir, '{:03}.jpg'.format(i)))
-        QtWidgets.qApp.processEvents()
-    win.top_left_label.show()
-    olddir = os.getcwd()
-    os.chdir(tmpdir)
-    subprocess.call(
-        ['ffmpeg', '-r', '%d' % rate, '-i', '%03d.jpg', '-vf', 'scale=trunc(iw/2)*2:trunc(ih/2)*2', 'output.mp4'])
-    os.rename('output.mp4', filename)
-    os.chdir(olddir)
-    g.m.statusBar().showMessage('Successfully saved movie as {}.'.format(os.path.basename(filename)))
-
-
-
-
-
-
-
-
-
-
-########################################################################################################################
-######################                         OPENING FILES                                 ###########################
-########################################################################################################################
-
-
-def open_file_from_gui():
-    open_file(None, True)
-
-
-def open_file(filename=None, from_gui=False):
-    """ open_file(filename=None)
-    Opens an image or movie file (.tif, .stk, .nd2) into a newWindow.
-
-    Parameters:
-        | filename (str) -- Address of file to open. If no filename is provided, the last opened file is used.
-    Returns:
-        newWindow
-    """
-    if filename is None:
-        if from_gui:
-            filetypes = 'Image Files (*.tif *.stk *.tiff *.nd2);;All Files (*.*)'
-            prompt = 'Open File'
-            filename = open_file_gui(prompt, filetypes=filetypes)
-            if filename is None:
-                return None
-        else:
-            filename = g.settings['filename']
-            if filename is None:
-                g.alert('No filename selected')
-                return None
-    append_recent_file(filename)  # make first in recent file menu
-    g.m.statusBar().showMessage('Loading {}'.format(os.path.basename(filename)))
-    t = time.time()
-    metadata = dict()
-    ext = os.path.splitext(filename)[1]
-    if ext in ['.tif', '.stk', '.tiff', '.ome']:
-        try:
-            Tiff = tifffile.TiffFile(filename)
-        except Exception as s:
-            g.alert("Unable to open {}. {}".format(filename, s))
-            return None
-        metadata = get_metadata_tiff(Tiff)
-        A = Tiff.asarray()
-        Tiff.close()
-        axes = [tifffile.AXES_LABELS[ax] for ax in Tiff.pages[0].axes]
-        # print("Original Axes = {}".format(axes)) #sample means RBGA, plane means frame, width means X, height means Y
-        if Tiff.is_rgb:
-            if A.ndim == 3:  # still color image.  [X, Y, RBGA]
-                A = np.transpose(A, (1, 0, 2))
-            elif A.ndim == 4:  # movie in color.  [T, X, Y, RGBA]
-                A = np.transpose(A, (0, 2, 1, 3))
-        else:
-            if A.ndim == 2:  # black and white still image [X,Y]
-                A = np.transpose(A, (1, 0))
-            elif A.ndim == 3:  # black and white movie [T,X,Y]
-                A = np.transpose(A, (0, 2, 1))  # This keeps the x and y the same as in FIJI.
-            elif A.ndim == 4:
-                if axes[3] == 'sample' and A.shape[3] == 1:
-                    A = np.squeeze(A)  # this gets rid of the meaningless 4th dimention in .stk files
-                    A = np.transpose(A, (0, 2, 1))
-    elif ext == '.nd2':
-        nd2 = nd2reader.Nd2(filename)
-        mt, mx, my = len(nd2), nd2.width, nd2.height
-        A = np.zeros((mt, mx, my))
-        percent = 0
-        for frame in range(mt):
-            A[frame] = nd2[frame].T
-            if percent < int(100 * float(frame) / mt):
-                percent = int(100 * float(frame) / mt)
-                g.m.statusBar().showMessage('Loading file {}%'.format(percent))
-                QtWidgets.qApp.processEvents()
-        metadata = get_metadata_nd2(nd2)
-    elif ext == '.py':
-        ScriptEditor.importScript(filename)
-        return
-    elif ext == '.whl':
-        # first, remove trailing (1) or (2)
-        newfilename = re.sub(r' \([^)]*\)', '', filename)
-        try:
-            os.rename(filename, newfilename)
-        except FileExistsError:
-            pass
-        filename = newfilename
-        result = pip.main(['install', filename])
-        if result == 0:
-            g.alert('Successfully installed {}'.format(filename))
-        else:
-            g.alert('Install of {} failed'.format(filename))
-        return
-    else:
-        msg = "Could not open.  Filetype for '{}' not recognized".format(filename)
-        g.alert(msg)
-        if filename in g.settings['recent_files']:
-            g.settings['recent_files'].remove(filename)
-        # make_recent_menu()
-        return
-    g.m.statusBar().showMessage('{} successfully loaded ({} s)'.format(os.path.basename(filename), time.time() - t))
-    g.settings['filename'] = filename
-    commands = ["open_file('{}')".format(filename)]
-    newWindow = Window(A, os.path.basename(filename), filename, commands, metadata)
-    return newWindow
-
-        
-def open_points(filename=None):
-    if g.currentWindow is None:
-        g.alert('Points cannot be loaded if no window is selected. Open a file and click on a window.')
-        return None
-    if filename is None:
-        filetypes = '*.txt'
-        prompt = 'Load Points'
-        filename = open_file_gui(prompt, filetypes=filetypes)
-        if filename is None:
-            return None
-    g.m.statusBar().showMessage('Loading points from {}'.format(os.path.basename(filename)))
-    try:
-        pts = np.loadtxt(filename)
-    except UnicodeDecodeError:
-        g.alert('This points file contains text that cannot be read. No points loaded.')
-        return None
-    if len(pts) == 0:
-        g.alert('This points file is empty. No points loaded.')
-        return None
-    nCols = pts.shape[1]
-    pointSize = g.settings['point_size']
-    pointColor = QtGui.QColor(g.settings['point_color'])
-    if nCols == 3:
-        for pt in pts:
-            t = int(pt[0])
-            if g.currentWindow.mt == 1:
-                t = 0
-            g.currentWindow.scatterPoints[t].append([pt[1],pt[2], pointColor, pointSize])
-        t = g.currentWindow.currentIndex
-        g.currentWindow.scatterPlot.setPoints(pos=g.currentWindow.scatterPoints[t])
-    elif nCols == 2:
-        t = 0
-        for pt in pts:
-            g.currentWindow.scatterPoints[t].append([pt[0], pt[1], pointColor, pointSize])
-        t = g.currentWindow.currentIndex
-        g.currentWindow.scatterPlot.setPoints(pos=g.currentWindow.scatterPoints[t])
-    g.m.statusBar().showMessage('Successfully loaded {}'.format(os.path.basename(filename)))
-
-    
-
-
-    
-########################################################################################################################
-######################                INTERNAL HELPER FUNCTIONS                              ###########################
-########################################################################################################################
-
-
-def append_recent_file(fname):
-    if fname in g.settings['recent_files']:
-        g.settings['recent_files'].remove(fname)
-    if os.path.exists(fname):
-        g.settings['recent_files'].append(fname)
-        if len(g.settings['recent_files']) > 8:
-            g.settings['recent_files'] = g.settings['recent_files'][-8:]
-    return fname
-
-
-def get_metadata_tiff(Tiff):
-    metadata = {}
-    if hasattr(Tiff[0], 'is_micromanager') and Tiff[0].is_micromanager:
-        imagej_tags_unpacked = {}
-        if hasattr(Tiff[0],'imagej_tags'):
-            imagej_tags = Tiff[0].imagej_tags
-            imagej_tags['info']
-            imagej_tags_unpacked = json.loads(imagej_tags['info'])
-        micromanager_metadata = Tiff[0].tags['micromanager_metadata']
-        metadata = {**micromanager_metadata.value, **imagej_tags_unpacked}
-        if 'Frames' in metadata and metadata['Frames'] > 1:
-            timestamps = [c.tags['micromanager_metadata'].value['ElapsedTime-ms'] for c in Tiff]
-            metadata['timestamps'] = timestamps
-            metadata['timestamp_units'] = 'ms'
-        keys_to_remove = ['NextFrame', 'ImageNumber', 'Frame', 'FrameIndex']
-        for key in keys_to_remove:
-            metadata.pop(key)
-    else:
-        try:
-            metadata = Tiff[0].image_description
-            metadata = txt2dict(metadata)
-        except AttributeError:
-            metadata = dict()
-    metadata['is_rgb'] = Tiff[0].is_rgb
-    return metadata
-
-
-def get_metadata_nd2(nd2):
-    metadata = dict()
-    metadata['channels'] = nd2.channels
-    metadata['date'] = nd2.date
-    metadata['fields_of_view'] = nd2.fields_of_view
-    metadata['frames'] = nd2.frames
-    metadata['height'] = nd2.height
-    metadata['width'] = nd2.width
-    metadata['z_levels'] = nd2.z_levels
-    return metadata
-
-
-def txt2dict(metadata):
-    meta = dict()
-    try:
-        metadata = json.loads(metadata.decode('utf-8'))
-        return metadata
-    except ValueError:  # if the metadata isn't in JSON
-        pass
-    for line in metadata.splitlines():
-        line = re.split('[:=]', line.decode())
-        if len(line) == 1:
-            meta[line[0]] = ''
-        else:
-            meta[line[0].lstrip().rstrip()] = line[1].lstrip().rstrip()
-    return meta
-
-
-def JSONhandler(obj):
-    if isinstance(obj,datetime.datetime):
-        return obj.isoformat()
-    else:
-        json.JSONEncoder().default(obj)
-
-
-def close(windows=None):
-    '''
-    Will close a window or a set of windows.
-
-    Values for windows:
-        | 'all' (str) -- closes all windows
-        | windows (list) - closes each window in the list
-        | (Window) - closes individual window
-        | (None) - closes current window
-    '''
-    if isinstance(windows, str):
-        if windows == 'all':
-            windows = [window for window in g.windows]
-            for window in windows:
-                window.close()
-    elif isinstance(windows,list):
-        for window in windows:
-            if isinstance(window,Window):
-                window.close()
-    elif isinstance(windows,Window):
-        windows.close()
-    elif windows is None:
-        if g.currentWindow is not None:
-            g.currentWindow.close()
-
-
-########################################################################################################################
-######################             OLD FUNCTIONS THAT MIGHT BE USEFUL SOMEDAY                ###########################
-########################################################################################################################
-"""
-
-def save_roi_traces(filename):
-    g.m.statusBar().showMessage('Saving traces to {}'.format(os.path.basename(filename)))
-    to_save = [roi.getTrace() for roi in g.currentWindow.rois]
-    np.savetxt(filename, np.transpose(to_save), header='\t'.join(['ROI %d' % i for i in range(len(to_save))]), fmt='%.4f', delimiter='\t', comments='')
-    g.settings['filename'] = filename
-    g.m.statusBar().showMessage('Successfully saved traces to {}'.format(os.path.basename(filename)))
-
-def load_metadata(filename=None):
-    '''This function loads the .txt file corresponding to a file into a dictionary
-    The .txt is a file which includes database connection information'''
-    meta=dict()
-    if filename is None:
-        filename=os.path.splitext(g.settings['filename'])[0]+'.txt'
-    BOM = codecs.BOM_UTF8.decode('utf8')
-    if not os.path.isfile(filename):
-        g.alert("'"+filename+"' is not a file.")
-        return dict()
-    with codecs.open(filename, encoding='utf-8') as f:
-        for line in f:
-            line = line.lstrip(BOM)
-            line=line.split('=')
-            meta[line[0].lstrip().rstrip()]=line[1].lstrip().rstrip()
-    for k in meta.keys():
-        if meta[k].isdigit():
-            meta[k]=int(meta[k])
-        else:
-            try:
-                meta[k]=float(meta[k])
-            except ValueError:
-                pass
-    return meta
-
-def save_metadata(meta):
-    filename=os.path.splitext(g.settings['filename'])[0]+'.txt'
-    f=open(filename, 'w')
-    text=''
-    for item in meta.items():
-        text+="{}={}\n".format(item[0],item[1])
-    f.write(text)
-    f.close()
-
-
-def save_current_frame(filename):
-    "" save_current_frame(filename)
-    Save the current single frame image of the currentWindow to a .tif file.
-
-    Parameters:
-        | filename (str) -- Address to save the frame to.
-    ""
-    if os.path.dirname(filename)=='': #if the user didn't specify a directory
-        directory=os.path.normpath(os.path.dirname(g.settings['filename']))
-        filename=os.path.join(directory,filename)
-    g.m.statusBar().showMessage('Saving {}'.format(os.path.basename(filename)))
-    A=np.average(g.currentWindow.image, 0)#.astype(g.settings['internal_data_type'])
-    metadata=json.dumps(g.currentWindow.metadata)
-    if len(A.shape)==3:
-        A = A[g.currentWindow.currentIndex]
-        A=np.transpose(A,(0,2,1)) # This keeps the x and the y the same as in FIJI
-    elif len(A.shape)==2:
-        A=np.transpose(A,(1,0))
-    tifffile.imsave(filename, A, description=metadata) #http://stackoverflow.com/questions/20529187/what-is-the-best-way-to-save-image-metadata-alongside-a-tif-with-python
-    g.m.statusBar().showMessage('Successfully saved {}'.format(os.path.basename(filename)))
-
-def make_recent_menu():
-    g.m.menuRecent_Files.clear()
-    if len(g.settings['recent_files']) == 0:
-        no_recent = QtWidgets.QAction("No Recent Files", g.m)
-        no_recent.setEnabled(False)
-        g.m.menuRecent_Files.addAction(no_recent)
-        return
-    def openFun(f):
-        return lambda: open_file(append_recent_file(f))
-    for fname in g.settings['recent_files'][:10]:
-        if os.path.exists(fname):
-            g.m.menuRecent_Files.addAction(QtWidgets.QAction(fname, g.m, triggered=openFun(fname)))
-
-"""
+# -*- coding: utf-8 -*-
+from ..logger import logger
+logger.debug("Started 'reading process/file_.py'")
+import pyqtgraph as pg
+import pyqtgraph.exporters
+import time
+import os.path
+import sys
+import numpy as np
+from qtpy import uic, QtGui, QtCore, QtWidgets
+import shutil, subprocess
+import datetime
+import json
+import re
+import pathlib
+
+from .. import global_vars as g
+from ..utils.BaseProcess import BaseDialog
+from ..window import Window
+from ..utils.misc import open_file_gui, save_file_gui
+from ..utils.io import tifffile
+
+__all__ = ['save_file', 'save_points', 'save_rois', 'save_movie_gui', 'open_file', 'open_file_from_gui', 'open_image_sequence_from_gui', 'open_points', 'close']
+
+########################################################################################################################
+######################                  SAVING FILES                                         ###########################
+########################################################################################################################
+
+
+
+def save_file(filename=None):
+    """save_file(filename=None)
+    Save the image in the currentWindow to a .tif file.
+
+    Parameters:
+        filename (str): The image or movie will be saved as  'filename'.tif.
+
+    """
+    if filename is None or filename is False:
+        filetypes = '*.tif'
+        prompt = 'Save File As Tif'
+        filename = save_file_gui(prompt, filetypes=filetypes)
+        if filename is None:
+            return None
+    if os.path.dirname(filename) == '':  # if the user didn't specify a directory
+        directory = os.path.normpath(os.path.dirname(g.settings['filename']))
+        filename = os.path.join(directory, filename)
+    g.m.statusBar().showMessage(f'Saving {os.path.basename(filename)}')
+    A = g.win.image
+    if A.dtype == np.bool:
+        A = A.astype(np.uint8)
+    metadata = g.win.metadata
+    try:
+        metadata = json.dumps(metadata, default=JSONhandler)
+    except TypeError as e:
+        msg = f"Error saving metadata.\n{e}\nContinuing to save file"
+        g.alert(msg)
+    if len(A.shape) == 3:
+        A = np.transpose(A, (0, 2, 1))  # This keeps the x and the y the same as in FIJI
+    elif len(A.shape) == 2:
+        A = np.transpose(A, (1, 0))
+    tifffile.imsave(filename, A,
+                    description=metadata)  # http://stackoverflow.com/questions/20529187/what-is-the-best-way-to-save-image-metadata-alongside-a-tif-with-python
+    g.m.statusBar().showMessage(f'Successfully saved {os.path.basename(filename)}')
+    return filename
+
+def save_points(filename=None):
+    """save_points(filename=None)
+    Saves the points in the current window to a text file
+
+    Parameters:
+        filename (str): Address to save the points to, with .txt
+
+
+    """
+
+    if filename is None:
+        filetypes = '*.txt'
+        prompt = 'Save Points'
+        filename = save_file_gui(prompt, filetypes=filetypes)
+        if filename is None:
+            return None
+    g.m.statusBar().showMessage(f'Saving Points in {os.path.basename(filename)}')
+    p_out = []
+    p_in = g.win.scatterPoints
+    for t in np.arange(len(p_in)):
+        for p in p_in[t]:
+            p_out.append(np.array([t, p[0], p[1]]))
+    p_out = np.array(p_out)
+    np.savetxt(filename, p_out)
+    g.m.statusBar().showMessage(f'Successfully saved {os.path.basename(filename)}')
+    return filename
+
+
+def save_movie_gui():
+    rateSpin = pg.SpinBox(value=50, bounds=[1, 1000], suffix='fps', int=True, step=1)
+    rateDialog = BaseDialog([{'string': 'Framerate', 'object': rateSpin}], 'Save Movie', 'Set the framerate')
+    rateDialog.accepted.connect(lambda: save_movie(rateSpin.value()))
+    g.dialogs.append(rateDialog)
+    rateDialog.show()
+
+def save_rois( filename=None):
+    g.currentWindow.save_rois(filename)
+
+
+def save_movie(rate, filename=None):
+    """save_movie(rate, filename)
+    Saves the currentWindow video as a .mp4 movie by joining .jpg frames together
+
+    Parameters:
+        rate (int): framerate
+        filename (str): Address to save the movie to, with .mp4
+
+    Notes:
+        Once you've exported all of the frames you wanted, open a command line and run the following:
+        ffmpeg -r 100 -i %03d.jpg output.mp4
+        -r: framerate
+        -i: input files.
+        %03d: The files have to be numbered 001.jpg, 002.jpg... etc.
+
+    """
+
+
+    ## Check if ffmpeg is installed
+    if os.name == 'nt':  # If we are running windows
+        try:
+            subprocess.call(["ffmpeg"])
+        except FileNotFoundError as e:
+            if e.errno == os.errno.ENOENT:
+                # handle file not found error.
+                # I used http://ffmpeg.org/releases/ffmpeg-2.8.4.tar.bz2 originally
+                g.alert("The program FFmpeg is required to export movies. \
+                \n\nFor instructions on how to install, go here: http://www.wikihow.com/Install-FFmpeg-on-Windows")
+                return None
+            else:
+                # Something else went wrong while trying to run `wget`
+                raise
+
+    filetypes = "Movies (*.mp4)"
+    prompt = "Save movie to .mp4 file"
+    filename = save_file_gui(prompt, filetypes=filetypes)
+    if filename is None:
+        return None
+
+    win = g.win
+    A = win.image
+    if len(A.shape) < 3:
+        g.alert('Movie not the right shape for saving.')
+        return None
+    try:
+        exporter = pg.exporters.ImageExporter(win.imageview.view)
+    except TypeError:
+        exporter = pg.exporters.ImageExporter.ImageExporter(win.imageview.view)
+
+    nFrames = len(A)
+    tmpdir = os.path.join(os.path.dirname(g.settings.settings_file), 'tmp')
+    if os.path.isdir(tmpdir):
+        shutil.rmtree(tmpdir)
+    os.mkdir(tmpdir)
+    win.top_left_label.hide()
+    for i in np.arange(0, nFrames):
+        win.setIndex(i)
+        exporter.export(os.path.join(tmpdir, f'{i:03}.jpg'))
+        QtWidgets.QApplication.processEvents()
+    win.top_left_label.show()
+    olddir = os.getcwd()
+    os.chdir(tmpdir)
+    subprocess.call(
+        ['ffmpeg', '-r', '%d' % rate, '-i', '%03d.jpg', '-vf', 'scale=trunc(iw/2)*2:trunc(ih/2)*2', 'output.mp4'])
+    os.rename('output.mp4', filename)
+    os.chdir(olddir)
+    g.m.statusBar().showMessage(f'Successfully saved movie as {os.path.basename(filename)}.')
+
+
+
+
+
+
+
+
+
+
+########################################################################################################################
+######################                         OPENING FILES                                 ###########################
+########################################################################################################################
+
+def open_image_sequence_from_gui():
+    open_image_sequence(None, True)
+
+def open_file_from_gui():
+    open_file(None, True)
+
+
+def open_image_sequence(filename=None, from_gui=False):
+    """ open_image_sequencefilename(filename=None)
+    Opens an image sequence (.tif, .png) into a new_window.
+
+    Parameters:
+        filename (str): Address of the first of a series of files that will be stitched together into a movie.
+                            If no filename is provided, the last opened file is used.
+    Returns:
+        new_window
+
+    """
+    if filename is None:
+        if from_gui:
+            filetypes = 'Image Files (*.tif *.tiff *.png);;All Files (*.*)'
+            prompt = 'Open File'
+            filename = open_file_gui(prompt, filetypes=filetypes)
+            if filename is None:
+                return None
+        else:
+            filename = g.settings['filename']
+            if filename is None:
+                g.alert('No filename selected')
+                return None
+    print(f"Filename: {filename}")
+    g.m.statusBar().showMessage(f'Loading {os.path.basename(filename)}')
+    t = time.time()
+    metadata = dict()
+
+    filename = pathlib.Path(filename)
+    assert filename.is_file()
+    directory = filename.parents[0]
+    ext = filename.suffix
+    all_image_filenames = [p for p in directory.iterdir() if p.suffix == ext]
+
+    all_images = []
+    if ext in ['.tif', '.stk', '.tiff', '.ome']:
+        for f in all_image_filenames:
+            results = open_tiff(f, metadata)
+            if results is None:
+                return None
+            else:
+                A, metadata = results
+                all_images.append(A)
+        all_images = np.array(all_images)
+    elif ext in ['.png']:
+        pass
+
+    append_recent_file(str(filename))  # make first in recent file menu
+    msg = f'{filename.parts[-1]} successfully loaded ({time.time() - t} s)'
+    g.m.statusBar().showMessage(msg)
+    g.settings['filename'] = str(filename)
+    commands = [f"open_image_sequence('{str(filename)}')"]
+    new_window = Window(all_images, filename.parts[-1], str(filename), commands, metadata)
+    return new_window
+
+
+def open_file(filename=None, from_gui=False):
+    """ open_file(filename=None)
+    Opens an image or movie file (.tif, .stk, .nd2) into a new_window.
+
+    Parameters:
+        filename (str): Address of file to open. If no filename is provided, the last opened file is used.
+    Returns:
+        new_window
+
+    """
+    if filename is None:
+        if from_gui:
+            filetypes = 'Image Files (*.tif *.stk *.tiff *.nd2);;All Files (*.*)'
+            prompt = 'Open File'
+            filename = open_file_gui(prompt, filetypes=filetypes)
+            if filename is None:
+                return None
+        else:
+            filename = g.settings['filename']
+            if filename is None:
+                g.alert('No filename selected')
+                return None
+    print(f"Filename: {filename}")
+    g.m.statusBar().showMessage(f'Loading {os.path.basename(str(filename))}')
+    t = time.time()
+    metadata = dict()
+    ext = os.path.splitext(str(filename))[1]
+    if ext in ['.tif', '.stk', '.tiff', '.ome']:
+        results = open_tiff(str(filename), metadata)
+        if results is None:
+            return None
+        else:
+            A, metadata = results
+    elif ext == '.nd2':
+        import nd2reader
+        nd2 = nd2reader.ND2Reader(str(filename))
+        axes = nd2.axes
+        mx = nd2.metadata['width']
+        my = nd2.metadata['height']
+        mt = nd2.metadata['total_images_per_channel']
+        A = np.zeros((mt, mx, my))
+        percent = 0
+        for frame in range(mt):
+            A[frame] = nd2[frame].T
+            if percent < int(100 * float(frame) / mt):
+                percent = int(100 * float(frame) / mt)
+                g.m.statusBar().showMessage(f'Loading file {percent}%')
+                QtWidgets.QApplication.processEvents()
+        metadata = nd2.metadata
+    elif ext == '.py':
+        from ..app.script_editor import ScriptEditor
+        ScriptEditor.importScript(filename)
+        return
+    elif ext == '.whl':
+        # first, remove trailing (1) or (2)
+        newfilename = re.sub(r' \([^)]*\)', '', filename)
+        try:
+            os.rename(filename, newfilename)
+        except FileExistsError:
+            pass
+        filename = newfilename
+        result = subprocess.call([sys.executable, '-m', 'pip', 'install', f'{filename}'])
+        if result == 0:
+            g.alert(f'Successfully installed {filename}')
+        else:
+            g.alert(f'Install of {filename} failed')
+        return
+    elif ext == '.jpg' or ext == '.png':
+        import skimage.io
+        A = skimage.io.imread(filename)
+        if len(A.shape) == 3:
+            perm = get_permutation_tuple(['y', 'x', 'c'], ['x', 'y', 'c'])
+            A = np.transpose(A, perm)
+            metadata['is_rgb'] = True
+
+    else:
+        msg = f"Could not open.  Filetype for '{filename}' not recognized"
+        g.alert(msg)
+        if filename in g.settings['recent_files']:
+            g.settings['recent_files'].remove(filename)
+        # make_recent_menu()
+        return
+        
+    append_recent_file(str(filename))  # make first in recent file menu
+    msg = f'{os.path.basename(str(filename))} successfully loaded ({time.time() - t} s)'
+    g.m.statusBar().showMessage(msg)
+    g.settings['filename'] = str(filename)
+    commands = [f"open_file('{filename}')"]
+    new_window = Window(A, os.path.basename(str(filename)), filename, commands, metadata)
+    return new_window
+
+def open_tiff(filename, metadata):
+    try:
+        Tiff = tifffile.TiffFile(str(filename))
+    except Exception as s:
+        g.alert(f"Unable to open {filename}. {s}")
+        return None
+    metadata = get_metadata_tiff(Tiff)
+    A = Tiff.asarray()
+    Tiff.close()
+    axes = [tifffile.AXES_LABELS[ax] for ax in Tiff.series[0].axes]
+    # print("Original Axes = {}".format(Tiff.series[0].axes)) #sample means RBGA, plane means frame, width means X, height means Y
+    try:
+        assert len(axes) == len(A.shape)
+    except AssertionError:
+        msg = 'Tiff could not be loaded because the number of axes in the array does not match the number of axes found by tifffile.py\n'
+        msg += f"Shape of array: {A.shape}\n"
+        msg += f"Axes found by tifffile.py: {axes}\n"
+        g.alert(msg)
+        return None
+    if set(axes) == set(['height', 'width']):  # still image in black and white.
+        target_axes = ['width', 'height']
+    elif set(axes) == set(['height', 'width', 'channel']):  # still image in color.
+        target_axes = ['width', 'height', 'channel']
+        metadata['is_rgb'] = True
+    elif set(axes) == set(['height', 'width', 'sample']):  # still image in color.
+        target_axes = ['width', 'height', 'sample']
+        metadata['is_rgb'] = True
+    elif set(axes) == set(['height', 'width', 'series']):  # movie in black and white
+        target_axes = ['series', 'width', 'height']
+    elif set(axes) == set(['height', 'width', 'time']):  # movie in black and white
+        target_axes = ['time', 'width', 'height']
+    elif set(axes) == set(['height', 'width', 'depth']):  # movie in black and white
+        target_axes = ['depth', 'width', 'height']
+    elif set(axes) == set(['channel', 'time', 'height', 'width']):  # movie in color
+        target_axes = ['time', 'width', 'height', 'channel']
+        metadata['is_rgb'] = True
+    elif set(axes) == set(['sample', 'time', 'height', 'width']):  # movie in color
+        target_axes = ['time', 'width', 'height', 'sample']
+        metadata['is_rgb'] = True
+    elif set(axes) == set(['other', 'height', 'width']):
+        target_axes = ['other', 'height', 'width']
+        metadata['is_rgb'] = False
+
+    perm = get_permutation_tuple(axes, target_axes)
+    A = np.transpose(A, perm)
+    if target_axes[-1] in ['channel', 'sample', 'series'] and A.shape[-1] == 2:
+        B = np.zeros(A.shape[:-1])
+        B = np.expand_dims(B, len(B.shape))
+        A = np.append(A, B, len(A.shape) - 1)  # add a column of zeros to the last dimension.
+        # if A.ndim == 4 and axes[3] == 'sample' and A.shape[3] == 1:
+        #    A = np.squeeze(A)  # this gets rid of the meaningless 4th dimention in .stk files
+    return [A, metadata]
+
+
+def open_points(filename=None):
+    """open_points(filename=None)
+    Opens a specified text file and displays the points from that file into the currentWindow
+
+    Parameters:
+        filename (str): Address of file to open. If no filename is provided, the last opened file is used.
+
+    Note:
+        Any existing points on a currentWindow will persist when another points file is opened and displayed
+
+    """
+    if g.win is None:
+        g.alert('Points cannot be loaded if no window is selected. Open a file and click on a window.')
+        return None
+    if filename is None:
+        filetypes = '*.txt'
+        prompt = 'Load Points'
+        filename = open_file_gui(prompt, filetypes=filetypes)
+        if filename is None:
+            return None
+    msg = f'Loading points from {os.path.basename(filename)}'
+    g.m.statusBar().showMessage(msg)
+    try:
+        pts = np.loadtxt(filename)
+    except UnicodeDecodeError:
+        g.alert('This points file contains text that cannot be read. No points loaded.')
+        return None
+    if len(pts) == 0:
+        g.alert('This points file is empty. No points loaded.')
+        return None
+    nCols = pts.shape[1]
+    pointSize = g.settings['point_size']
+    pointColor = QtGui.QColor(g.settings['point_color'])
+    if nCols == 3:
+        for pt in pts:
+            t = int(pt[0])
+            if g.win.mt == 1:
+                t = 0
+            g.win.scatterPoints[t].append([pt[1],pt[2], pointColor, pointSize])
+        if g.settings['show_all_points']:
+            pts = []
+            for t in np.arange(g.win.mt):
+                pts.extend(g.win.scatterPoints[t])
+            pointSizes = [pt[3] for pt in pts]
+            brushes = [pg.mkBrush(*pt[2].getRgb()) for pt in pts]
+            g.win.scatterPlot.setPoints(pos=pts, size=pointSizes, brush=brushes)
+        else:
+            t = g.win.currentIndex
+            g.win.scatterPlot.setPoints(pos=g.win.scatterPoints[t])
+            g.win.updateindex()
+    elif nCols == 2:
+        t = 0
+        for pt in pts:
+            g.win.scatterPoints[t].append([pt[0], pt[1], pointColor, pointSize])
+        t = g.win.currentIndex
+        g.win.scatterPlot.setPoints(pos=g.win.scatterPoints[t])
+
+    g.m.statusBar().showMessage(f'Successfully loaded {os.path.basename(filename)}')
+
+
+
+
+    
+########################################################################################################################
+######################                INTERNAL HELPER FUNCTIONS                              ###########################
+########################################################################################################################
+def get_permutation_tuple(src, dst):
+    """get_permtation_tuple(src, dst)
+
+    Parameters:
+        src (list): The original ordering of the axes in the tiff.
+        dst (list): The desired ordering of the axes in the tiff.
+
+    Returns:
+        result (tuple): The required permutation so the axes are ordered as desired.
+    """
+    result = []
+    for i in dst:
+        result.append(src.index(i))
+    result = tuple(result)
+    return result
+
+def append_recent_file(fname):
+    fname = os.path.abspath(fname)
+    if fname in g.settings['recent_files']:
+        g.settings['recent_files'].remove(fname)
+    if os.path.exists(fname):
+        g.settings['recent_files'].append(fname)
+        if len(g.settings['recent_files']) > 8:
+            g.settings['recent_files'] = g.settings['recent_files'][-8:]
+    return fname
+
+
+def get_metadata_tiff(Tiff):
+    metadata = {}
+    if hasattr(Tiff[0], 'is_micromanager') and Tiff[0].is_micromanager:
+        imagej_tags_unpacked = {}
+        if hasattr(Tiff[0],'imagej_tags'):
+            imagej_tags = Tiff[0].imagej_tags
+            imagej_tags['info']
+            imagej_tags_unpacked = json.loads(imagej_tags['info'])
+        micromanager_metadata = Tiff[0].tags['micromanager_metadata']
+        metadata = {**micromanager_metadata.value, **imagej_tags_unpacked}
+        if 'Frames' in metadata and metadata['Frames'] > 1:
+            timestamps = [c.tags['micromanager_metadata'].value['ElapsedTime-ms'] for c in Tiff]
+            metadata['timestamps'] = timestamps
+            metadata['timestamp_units'] = 'ms'
+        keys_to_remove = ['NextFrame', 'ImageNumber', 'Frame', 'FrameIndex']
+        for key in keys_to_remove:
+            metadata.pop(key, None)
+    else:
+        try:
+            metadata = Tiff[0].image_description
+            metadata = txt2dict(metadata)
+        except AttributeError:
+            metadata = dict()
+    metadata['is_rgb'] = Tiff[0].is_rgb
+    return metadata
+
+
+
+def txt2dict(metadata):
+    meta = dict()
+    try:
+        metadata = json.loads(metadata.decode('utf-8'))
+        return metadata
+    except ValueError:  # if the metadata isn't in JSON
+        pass
+    for line in metadata.splitlines():
+        line = re.split('[:=]', line.decode())
+        if len(line) == 1:
+            meta[line[0]] = ''
+        else:
+            meta[line[0].lstrip().rstrip()] = line[1].lstrip().rstrip()
+    return meta
+
+
+def JSONhandler(obj):
+    if isinstance(obj, datetime.datetime):
+        return obj.isoformat()
+    else:
+        json.JSONEncoder().default(obj)
+
+
+def close(windows=None):
+    """close(window=None)
+    Will close a window or a set of windows.
+
+    Parameters:
+        'all' (str): closes all windows
+        windows (list): closes each window in the list
+        Window: closes individual window
+        (None): closes current window
+
+    """
+    if isinstance(windows, str):
+        if windows == 'all':
+            windows = [window for window in g.windows]
+            for window in windows:
+                window.close()
+    elif isinstance(windows,list):
+        for window in windows:
+            if isinstance(window,Window):
+                window.close()
+    elif isinstance(windows,Window):
+        windows.close()
+    elif windows is None:
+        if g.win is not None:
+            g.win.close()
+
+
+########################################################################################################################
+######################             OLD FUNCTIONS THAT MIGHT BE USEFUL SOMEDAY                ###########################
+########################################################################################################################
+"""
+
+def save_roi_traces(filename):
+    g.m.statusBar().showMessage('Saving traces to {}'.format(os.path.basename(filename)))
+    to_save = [roi.getTrace() for roi in g.win.rois]
+    np.savetxt(filename, np.transpose(to_save), header='\t'.join(['ROI %d' % i for i in range(len(to_save))]), fmt='%.4f', delimiter='\t', comments='')
+    g.settings['filename'] = filename
+    g.m.statusBar().showMessage('Successfully saved traces to {}'.format(os.path.basename(filename)))
+
+def load_metadata(filename=None):
+    '''This function loads the .txt file corresponding to a file into a dictionary
+    The .txt is a file which includes database connection information'''
+    meta=dict()
+    if filename is None:
+        filename=os.path.splitext(g.settings['filename'])[0]+'.txt'
+    BOM = codecs.BOM_UTF8.decode('utf8')
+    if not os.path.isfile(filename):
+        g.alert("'"+filename+"' is not a file.")
+        return dict()
+    with codecs.open(filename, encoding='utf-8') as f:
+        for line in f:
+            line = line.lstrip(BOM)
+            line=line.split('=')
+            meta[line[0].lstrip().rstrip()]=line[1].lstrip().rstrip()
+    for k in meta.keys():
+        if meta[k].isdigit():
+            meta[k]=int(meta[k])
+        else:
+            try:
+                meta[k]=float(meta[k])
+            except ValueError:
+                pass
+    return meta
+
+def save_metadata(meta):
+    filename=os.path.splitext(g.settings['filename'])[0]+'.txt'
+    f=open(filename, 'w')
+    text=''
+    for item in meta.items():
+        text+="{}={}\n".format(item[0],item[1])
+    f.write(text)
+    f.close()
+
+
+def save_current_frame(filename):
+    "" save_current_frame(filename)
+    Save the current single frame image of the currentWindow to a .tif file.
+
+    Parameters:
+        | filename (str) -- Address to save the frame to.
+    ""
+    if os.path.dirname(filename)=='': #if the user didn't specify a directory
+        directory=os.path.normpath(os.path.dirname(g.settings['filename']))
+        filename=os.path.join(directory,filename)
+    g.m.statusBar().showMessage('Saving {}'.format(os.path.basename(filename)))
+    A=np.average(g.win.image, 0)#.astype(g.settings['internal_data_type'])
+    metadata=json.dumps(g.win.metadata)
+    if len(A.shape)==3:
+        A = A[g.win.currentIndex]
+        A=np.transpose(A,(0,2,1)) # This keeps the x and the y the same as in FIJI
+    elif len(A.shape)==2:
+        A=np.transpose(A,(1,0))
+    tifffile.imsave(filename, A, description=metadata) #http://stackoverflow.com/questions/20529187/what-is-the-best-way-to-save-image-metadata-alongside-a-tif-with-python
+    g.m.statusBar().showMessage('Successfully saved {}'.format(os.path.basename(filename)))
+
+def make_recent_menu():
+    g.m.menuRecent_Files.clear()
+    if len(g.settings['recent_files']) == 0:
+        no_recent = QtWidgets.QAction("No Recent Files", g.m)
+        no_recent.setEnabled(False)
+        g.m.menuRecent_Files.addAction(no_recent)
+        return
+    def openFun(f):
+        return lambda: open_file(append_recent_file(f))
+    for fname in g.settings['recent_files'][:10]:
+        if os.path.exists(fname):
+            g.m.menuRecent_Files.addAction(QtWidgets.QAction(fname, g.m, triggered=openFun(fname)))
+
+"""
+
+logger.debug("Completed 'reading process/file_.py'")
```

### Comparing `flika-0.2.9/flika/process/filters.py` & `flika-0.3.0/flika/process/filters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,865 +1,1032 @@
-# -*- coding: utf-8 -*-
-import numpy as np
-import skimage
-import skimage.filters
-from qtpy import QtWidgets, QtGui, QtCore
-import time
-from .. import global_vars as g
-from .BaseProcess import BaseProcess, SliderLabel, SliderLabelOdd, CheckBox
-from .progress_bar import ProgressBar
-
-__all__ = ['gaussian_blur','mean_filter','median_filter','butterworth_filter','boxcar_differential_filter','wavelet_filter','difference_filter', 'fourier_filter', 'bilateral_filter']
-###############################################################################
-##################   SPATIAL FILTERS       ####################################
-###############################################################################
-class Gaussian_blur(BaseProcess):
-    """ gaussian_blur(sigma, norm_edges=False, keepSourceWindow=False)
-
-    This applies a spatial gaussian_blur to every frame of your stack.  
-    
-    Args:
-        sigma (float): The width of the gaussian
-        norm_edges (bool): If true, this reduces the values of the pixels near the edges so they have the same standard deviation as the rest of the image
-
-    Returns:
-        flika.window.Window
-
-    """
-    def __init__(self):
-        super().__init__()
-        assert 'gaussian' in skimage.filters.__dict__  # Make sure your version of skimage is >= 0.12.3
-    def gui(self):
-        self.gui_reset()
-        sigma=SliderLabel(2)
-        sigma.setRange(0,100)
-        sigma.setValue(1)
-        norm_edges=CheckBox()
-        norm_edges.setChecked(False)
-        preview=CheckBox()
-        preview.setChecked(True)
-        self.items.append({'name': 'sigma', 'string': 'Sigma (pixels)', 'object': sigma})
-        self.items.append({'name': 'norm_edges', 'string': 'Normalize Edges', 'object': norm_edges})
-        self.items.append({'name': 'preview', 'string': 'Preview', 'object': preview})
-        super().gui()
-        self.preview()
-
-    def __call__(self, sigma, norm_edges=False, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if norm_edges == True:
-            mode = 'constant'
-        else:
-            mode = 'nearest'
-        if sigma>0:
-            self.newtif=np.zeros(self.tif.shape)
-            if len(self.tif.shape)==3:
-                for i in np.arange(len(self.newtif)):
-                    self.newtif[i]=skimage.filters.gaussian(self.tif[i].astype(np.float64),sigma, mode=mode)
-            elif len(self.tif.shape)==2:
-                self.newtif=skimage.filters.gaussian(self.tif.astype(np.float64),sigma, mode=mode)
-            self.newtif=self.newtif.astype(g.settings['internal_data_type'])
-        else:
-            self.newtif=self.tif
-        self.newname=self.oldname+' - Gaussian Blur sigma='+str(sigma)
-        return self.end()
-    def preview(self):
-        norm_edges = self.getValue('norm_edges')
-        if norm_edges == True:
-            mode = 'constant'
-        else:
-            mode = 'nearest'
-        sigma=self.getValue('sigma')
-        preview=self.getValue('preview')
-        if preview:
-            if len(g.currentWindow.image.shape)==3:
-                testimage=g.currentWindow.image[g.currentWindow.currentIndex].astype(np.float64)
-            elif len(g.currentWindow.image.shape)==2:
-                testimage=g.currentWindow.image.astype(np.float64)
-            if sigma>0:
-                testimage=skimage.filters.gaussian(testimage,sigma, mode=mode)
-            g.currentWindow.imageview.setImage(testimage,autoLevels=False)            
-        else:
-            g.currentWindow.reset()
-gaussian_blur=Gaussian_blur()
-    
-    
-###############################################################################
-##################   TEMPORAL FILTERS       ###################################
-###############################################################################
-from scipy.signal import butter, filtfilt
-    
-
-class Butterworth_filter(BaseProcess):
-    """ butterworth_filter(filter_order, low, high, keepSourceWindow=False)
-    This filters a stack in time.
-    
-    Parameters:
-        | filter_order (int) -- The order of the butterworth filter (higher->steeper).
-        | low (float) -- The low frequency cutoff.  Must be between 0 and 1 and must be below high.
-        | high (float) -- The high frequency cutoff.  Must be between 0 and 1 and must be above low.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-
-    def gui(self):
-        self.gui_reset()
-        filter_order=QtWidgets.QSpinBox()
-        filter_order.setRange(1,10)
-        low=SliderLabel(5)
-        low.setRange(0,1)
-        low.setValue(0)
-        high=SliderLabel(5)
-        high.setRange(0,1)
-        high.setValue(1)
-        low.valueChanged.connect(lambda low: high.setMinimum(low))
-        high.valueChanged.connect(lambda high: low.setMaximum(high))
-        preview=CheckBox()
-        preview.setChecked(True)
-        self.items.append({'name':'filter_order','string':'Filter Order','object':filter_order})
-        self.items.append({'name':'low','string':'Low Cutoff Frequency','object':low})
-        self.items.append({'name':'high','string':'High Cutoff Frequency','object':high})
-        self.items.append({'name':'preview','string':'Preview','object':preview})        
-        super().gui()
-        self.roi=g.currentWindow.currentROI
-        if self.roi is not None:
-            self.ui.rejected.connect(self.roi.redraw_trace)
-            self.ui.accepted.connect(self.roi.redraw_trace)
-        if self.roi is None or g.currentTrace is None:
-            preview.setChecked(False)
-            preview.setEnabled(False)
-        
-    def __call__(self,filter_order,low,high,keepSourceWindow=False):
-        if low==0 and high==1:
-            return
-        self.start(keepSourceWindow)
-        if self.tif.ndim != 3:
-            g.alert("Butterworth filter only works on 3-dimensional movies.")
-            return
-        if g.settings['multiprocessing']:
-            self.newtif=butterworth_filter_multi(filter_order,low,high,g.currentWindow.image)
-        else:
-            self.newtif=np.zeros(self.tif.shape,dtype=g.settings.d['internal_data_type'])
-            mt,mx,my=self.tif.shape
-            b,a,padlen=self.makeButterFilter(filter_order,low,high)
-            for i in np.arange(mx):
-                for j in np.arange(my):
-                    self.newtif[:, i, j]=filtfilt(b,a, self.tif[:, i, j], padlen=padlen)
-        self.newname=self.oldname+' - Butter Filtered'
-        return self.end()
-        
-    def preview(self):
-        if g.currentTrace is not None:
-            filter_order=self.getValue('filter_order')
-            low=self.getValue('low')
-            high=self.getValue('high')
-            preview=self.getValue('preview')
-            if self.roi is not None:
-                if preview:
-                    if (low==0 and high==1) or (low==0 and high==0):
-                        self.roi.onRegionChangeFinished() #redraw roi without filter
-                    else:
-                        b,a,padlen=self.makeButterFilter(filter_order,low,high)
-                        trace=self.roi.getTrace()
-                        trace=filtfilt(b,a, trace, padlen=padlen)
-                        roi_index=g.currentTrace.get_roi_index(self.roi)
-                        g.currentTrace.update_trace_full(roi_index,trace) #update_trace_partial may speed it up
-                else:
-                    self.roi.redraw_trace()
-    def makeButterFilter(self,filter_order,low,high):
-        padlen=0
-        if high==1: 
-            if low==0: #if there is no temporal filter at all,
-                return None,None,None
-            else: #if only high pass temporal filter
-                [b,a]= butter(filter_order,low,btype='highpass')
-                padlen=3
-        else:
-            if low==0:
-                [b,a]= butter(filter_order,high,btype='lowpass')
-            else:
-                [b,a]=butter(filter_order,[low,high], btype='bandpass')
-            padlen=6
-        return b,a,padlen
-        
-butterworth_filter=Butterworth_filter()
-
-        
-def butterworth_filter_multi(filter_order,low,high,tif):
-    nThreads= g.settings['nCores']
-    mt,mx,my=tif.shape
-    block_ends=np.linspace(0,mx,nThreads+1).astype(np.int)
-    data=[tif[:, block_ends[i]:block_ends[i+1],:] for i in np.arange(nThreads)] #split up data along x axis. each thread will get one.
-    args=(filter_order,low,high)
-    progress = ProgressBar(butterworth_filter_multi_inner, data, args, nThreads, msg='Performing Butterworth Filter')
-    if progress.results is None or any(r is None for r in progress.results):
-        result=None
-    else:
-        result=np.concatenate(progress.results,axis=1).astype(g.settings['internal_data_type'])
-    return result
-    
-
-def butterworth_filter_multi_inner(q_results, q_progress, q_status, child_conn, args):
-    data=child_conn.recv()
-    status=q_status.get(True) #this blocks the process from running until all processes are launched
-    if status=='Stop':
-        q_results.put(None)
-    
-    def makeButterFilter(filter_order,low,high):
-        padlen=0
-        if high==1: 
-            if low==0: #if there is no temporal filter at all,
-                return None,None,None
-            else: #if only high pass temporal filter
-                [b,a]= butter(filter_order,low,btype='highpass')
-                padlen=3
-        else:
-            if low==0:
-                [b,a]= butter(filter_order,high,btype='lowpass')
-            else:
-                [b,a]=butter(filter_order,[low,high], btype='bandpass')
-            padlen=6
-        return b,a,padlen
-        
-    filter_order,low,high = args
-    b,a,padlen=makeButterFilter(filter_order,low,high)
-    mt,mx,my=data.shape
-    result=np.zeros(data.shape,g.settings['internal_data_type'])
-    nPixels=mx*my
-    pixel=0
-    percent=0
-    for x in np.arange(mx):
-        for y in np.arange(my):
-            if not q_status.empty():
-                stop=q_status.get(False)
-                q_results.put(None)
-                return
-            pixel+=1
-            if percent<int(100*pixel/nPixels):
-                percent=int(100*pixel/nPixels)
-                q_progress.put(percent)
-            result[:, x, y]=filtfilt(b,a, data[:, x, y], padlen=padlen)
-    q_results.put(result)
-
-from scipy.ndimage.filters import convolve
-class Mean_filter(BaseProcess):
-    """ mean_filter(nFrames, keepSourceWindow=False)
-    This filters a stack in time.
-    
-    Parameters:
-        | nFrames (int) -- Number of frames to average
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        nFrames=SliderLabel(0)
-        nFrames.setRange(1,100)
-        preview=CheckBox()
-        preview.setChecked(True)
-        self.items.append({'name':'nFrames','string':'nFrames','object':nFrames})
-        self.items.append({'name':'preview','string':'Preview','object':preview})        
-        super().gui()
-        self.roi=g.currentWindow.currentROI
-        if self.roi is not None:
-            self.ui.rejected.connect(self.roi.redraw_trace)
-            self.ui.accepted.connect(self.roi.redraw_trace)
-        else:
-            preview.setChecked(False)
-            preview.setEnabled(False)
-            
-    def __call__(self,nFrames,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.tif.dtype == np.float16:
-            g.alert("Mean Filter does not support float16 type arrays")
-            return
-        if self.tif.ndim != 3:
-            g.alert("Mean Filter only supports 3-dimensional movies.")
-            return
-        self.newtif=convolve(self.tif,weights=np.full((nFrames,1,1),1.0/nFrames))        
-        self.newname=self.oldname+' - Mean Filtered'
-        return self.end()
-    def preview(self):
-        nFrames=self.getValue('nFrames')
-        preview=self.getValue('preview')
-        if self.roi is not None:
-            if preview:
-                if nFrames==1:
-                    self.roi.redraw_trace() #redraw roi without filter
-                else:
-                    trace=self.roi.getTrace()
-                    trace=convolve(trace,weights=np.full((nFrames),1.0/nFrames))        
-                    roi_index=g.currentTrace.get_roi_index(self.roi)
-                    g.currentTrace.update_trace_full(roi_index,trace) #update_trace_partial may speed it up
-            else:
-                self.roi.redraw_trace()
-mean_filter=Mean_filter()
-
-
-from scipy.signal import medfilt
-class Median_filter(BaseProcess):
-    """ median_filter(nFrames, keepSourceWindow=False)
-    This filters a stack in time.
-    
-    Parameters:
-        | nFrames (int) -- Number of frames to average.  This must be an odd number
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        nFrames=SliderLabelOdd()
-        nFrames.setRange(1,100)
-        preview=CheckBox()
-        preview.setChecked(True)
-        self.items.append({'name':'nFrames','string':'nFrames','object':nFrames})
-        self.items.append({'name':'preview','string':'Preview','object':preview})        
-        super().gui()
-        self.roi=g.currentWindow.currentROI
-        if self.roi is not None:
-            self.ui.rejected.connect(self.roi.redraw_trace)
-            self.ui.accepted.connect(self.roi.redraw_trace)
-        else:
-            preview.setChecked(False)
-            preview.setEnabled(False)
-            
-    def __call__(self, nFrames, keepSourceWindow=False):
-        if nFrames%2 == 0: #if value is even:
-            g.alert('median_filter only takes odd numbers.  Operation cancelled')
-            return None
-        self.start(keepSourceWindow)
-        if self.tif.ndim < 3:
-            g.alert("Median filter requires at least 3 dimensions. %d < 3" % self.tif.ndim)
-            return
-        mx=self.tif.shape[2]
-        my=self.tif.shape[1]
-        self.newtif=np.zeros(self.tif.shape)
-        for i in np.arange(my):
-            for j in np.arange(mx):
-                self.newtif[:, i, j]=medfilt(self.tif[:, i, j], kernel_size=nFrames)      
-        self.newname=self.oldname+' - Median Filtered'
-        return self.end()
-    def preview(self):
-        nFrames=self.getValue('nFrames')
-        preview=self.getValue('preview')
-        if self.roi is not None:
-            if preview:
-                print(nFrames)
-                if nFrames==1:
-                    self.roi.redraw_trace() #redraw roi without filter
-                elif nFrames%2==0: #if value is even
-                    return None
-                else:
-                    trace=self.roi.getTrace()
-                    trace=medfilt(trace,kernel_size=nFrames)
-                    roi_index=g.currentTrace.get_roi_index(self.roi)
-                    g.currentTrace.update_trace_full(roi_index,trace) #update_trace_partial may speed it up
-            else:
-                self.roi.redraw_trace()
-                
-median_filter=Median_filter()
-
-
-
-
-from scipy.fftpack import fft, ifft, fftfreq
-class Fourier_filter(BaseProcess):
-    """ fourier_filter(frame_rate, low, high, loglogPreview, keepSourceWindow=False)
-    I'm going to eventually plot the trace in the frequency domain inside this box so you can see where the power is.
-
-    Parameters:
-        | frame_rate (int) -- Frame Rate in Hz
-        | low (float) -- Low cutoff frequency for the fourier filter
-        | high (float) -- High cutoff frequency for fourier filter
-        | loglogPreview (boolean) -- whether or not to plot frequency spectrum on log log axes
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        frame_rate=QtWidgets.QDoubleSpinBox()
-        frame_rate.setRange(.01,1000)
-        frame_rate.setValue(200)
-        low=SliderLabel(5)
-        low.setRange(0,1)
-        low.setValue(0)
-        high=SliderLabel(5)
-        high.setRange(0,1)
-        high.setValue(1)
-        frame_rate.valueChanged.connect(self.frame_rate_changed)
-        low.valueChanged.connect(lambda low: high.setMinimum(low))
-        high.valueChanged.connect(lambda high: low.setMaximum(high))
-        preview=CheckBox()
-        preview.setChecked(True)
-        loglogPreview=CheckBox()
-        self.items.append({'name':'frame_rate','string':'Frame Rate (Hz)','object':frame_rate})
-        self.items.append({'name':'low','string':'Low Cutoff Frequency','object':low})
-        self.items.append({'name':'high','string':'High Cutoff Frequency','object':high})
-        self.items.append({'name':'loglogPreview','string':'Plot frequency spectrum on log log axes','object':loglogPreview})    
-        self.items.append({'name':'preview','string':'Preview','object':preview})        
-        super().gui()
-        self.roi=g.currentWindow.currentROI
-        if self.roi is not None:
-            self.ui.rejected.connect(self.roi.redraw_trace)
-            self.ui.accepted.connect(self.roi.redraw_trace)
-        else:
-            preview.setChecked(False)
-            preview.setEnabled(False)
-            loglogPreview.setEnabled(False) 
-    def __call__(self, frame_rate, low, high, loglogPreview, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.tif.dtype == np.float16:
-            g.alert("Fourier transform does not support float16 movies.")
-            return
-        if self.tif.ndim != 3 or self.tif.shape[2] == 3:
-            g.alert('Fourier transform requires 3 dimensional movies.')
-            return
-        if low==0 and high==frame_rate/2.0:
-            return
-        mt,mx,my=self.tif.shape
-        W = fftfreq(mt, d=1.0/frame_rate)
-        filt=np.ones((mt))
-        filt[(np.abs(W)<low)] = 0
-        filt[(np.abs(W)>high)] = 0
-        self.newtif=np.zeros(self.tif.shape)
-        for i in np.arange(my):
-            for j in np.arange(mx):
-                f_signal = fft(self.tif[:, i, j])
-                f_signal*=filt
-                self.newtif[:, i, j]=np.real(ifft(f_signal))
-        self.newname=self.oldname+' - Fourier Filtered'
-        return self.end()
-    def preview(self):
-        frame_rate=self.getValue('frame_rate')
-        low=self.getValue('low')
-        high=self.getValue('high')
-        loglogPreview=self.getValue('loglogPreview')
-        preview=self.getValue('preview')
-        if self.roi is not None:
-            if preview:
-                if (low==0 and high==frame_rate/2.0) or (low==0 and high==0):
-                    self.roi.redraw_trace() #redraw roi without filter
-                else:
-                    trace=self.roi.getTrace()
-                    W = fftfreq(len(trace), d=1.0/frame_rate)
-                    f_signal = fft(trace)
-                    f_signal[(np.abs(W)<low)] = 0
-                    f_signal[(np.abs(W)>high)] = 0
-                    cut_signal=np.real(ifft(f_signal))
-                    roi_index=g.currentTrace.get_roi_index(self.roi)
-                    g.currentTrace.update_trace_full(roi_index,cut_signal) #update_trace_partial may speed it up
-            else:
-                self.roi.redraw_trace()
-                
-    def frame_rate_changed(self):
-        low=[item for item in self.items if item['name']=='low'][0]['object']
-        high=[item for item in self.items if item['name']=='high'][0]['object']
-        frame_rate=[item for item in self.items if item['name']=='frame_rate'][0]['object']
-        f=frame_rate.value()
-        low.setRange(0.0,f/2.0)
-        high.setRange(0.0,f/2.0)
-        low.setValue(0)
-        high.setValue(f/2.0)
-""" This is demo code for plotting in the frequency domain, something I hoepfully will get around to implementing
-
-from numpy import sin, linspace, pi
-from pylab import plot, show, title, xlabel, ylabel, subplot
-from scipy import fft, arange
-
-def plotSpectrum(y,Fs):
-    n = len(y) # length of the signal
-    k = arange(n)
-    W = fftfreq(len(y), d=1/Fs)
-
-    Y = fft(y) # fft computing and normalization
-    f_signal[(np.abs(W)>10)] = 0
-    plot(abs(f_signal)[0:N/2])
-    cut_signal=np.real(ifft(f_signal))
-    p=plot(trace)
-    p.plot(cut_signal,pen=pg.mkPen('r'))
-    
-    plot(frq,abs(f_signal),'r') # plotting the spectrum
-    xlabel('Freq (Hz)')
-    ylabel('|Y(freq)|')"""
-        
-fourier_filter=Fourier_filter()
-
-
-
-class Difference_filter(BaseProcess):
-    """ difference_filter(keepSourceWindow=False)
-    subtracts each frame from the preceeding frame
-    
-    
-    Parameters:
-        | None
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        if super().gui()==False:
-            return False
-    def __call__(self,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        self.newtif=np.zeros(self.tif.shape)
-        for i in np.arange(1,len(self.newtif)):
-            self.newtif[i]=self.tif[i]-self.tif[i-1]
-        self.newname=self.oldname+' - Difference Filtered'
-        return self.end()
-difference_filter=Difference_filter()
-
-    
-class Boxcar_differential_filter(BaseProcess):
-    """ boxcar_differential_filter(minNframes, maxNframes, keepSourceWindow=False)
-    Applies a Boxcar differential filter by comparing each frameat index I to the frames in range [I+minNframes, I+maxNframes]
-
-    Parameters:
-        | minNframes (int) -- The starting point of your boxcar window.
-        | maxNframes (int) -- The ending point of your boxcar window.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        minNframes=SliderLabel(0)
-        minNframes.setRange(1,100)
-        maxNframes=SliderLabel(0)
-        maxNframes.setRange(2,101)
-        minNframes.valueChanged.connect(lambda minn: maxNframes.setMinimum(minn+1))
-        maxNframes.valueChanged.connect(lambda maxx: minNframes.setMaximum(maxx-1))
-        preview=CheckBox()
-        preview.setChecked(True)
-        self.items.append({'name':'minNframes','string':'Minimum Number of Frames','object':minNframes})
-        self.items.append({'name':'maxNframes','string':'Maximum Number of Frames','object':maxNframes})
-        self.items.append({'name':'preview','string':'Preview','object':preview})  
-        if super().gui()==False:
-            return False
-        self.roi=g.currentWindow.currentROI
-        if self.roi is not None:
-            self.ui.rejected.connect(self.roi.redraw_trace)
-            self.ui.accepted.connect(self.roi.redraw_trace)
-        else:
-            preview.setChecked(False)
-            preview.setEnabled(False)
-    def __call__(self,minNframes,maxNframes,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        self.newtif=np.zeros(self.tif.shape)
-        for i in np.arange(maxNframes,len(self.newtif)):
-            self.newtif[i]=self.tif[i]-np.min(self.tif[i-maxNframes:i-minNframes],0)
-        self.newname=self.oldname+' - Boxcar Differential Filtered'
-        return self.end()
-    def preview(self):
-        minNframes=self.getValue('minNframes')
-        maxNframes=self.getValue('maxNframes')
-        preview=self.getValue('preview')
-        if self.roi is not None:
-            if preview:
-                self.tif=self.roi.window.image
-                (mt,mx,my)=self.tif.shape
-                cnt=np.array([np.array([np.array([p[1],p[0]])]) for p in self.roi.pts ])
-                mask=np.zeros(self.tif[0,:,:].shape,np.uint8)
-                cv2.drawContours(mask,[cnt],0,255,-1)
-                mask=mask.reshape(mx*my).astype(np.bool)
-                tif=self.tif.reshape((mt,mx*my))
-                tif=tif[:,mask]
-                newtrace=np.zeros(mt)
-                for i in np.arange(maxNframes,mt):
-                    newtrace[i]=np.mean(tif[i]-np.min(tif[i-maxNframes:i-minNframes],0))
-                roi_index=g.currentTrace.get_roi_index(self.roi)
-                g.currentTrace.update_trace_full(roi_index,newtrace) #update_trace_partial may speed it up
-            else:
-                self.roi.redraw_trace()
-boxcar_differential_filter=Boxcar_differential_filter()
-    
-    
-from scipy import signal
-class Wavelet_filter(BaseProcess):
-    ''' wavelet_filter(low, high, keepSourceWindow=False)
-    ***Warning!! This function is extremely slow.***
-    
-    Parameters:
-        | low (int) -- The starting point of your boxcar window.
-        | high (int) -- The ending point of your boxcar window.
-    Returns:
-        newWindow
-    '''
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        low=SliderLabel(0)
-        low.setRange(1,50)
-        high=SliderLabel(0)
-        high.setRange(2,50)
-        low.valueChanged.connect(lambda minn: high.setMinimum(minn+1))
-        high.valueChanged.connect(lambda maxx: low.setMaximum(maxx-1))
-        preview=CheckBox()
-        preview.setChecked(True)
-        self.items.append({'name':'low','string':'Low Frequency Threshold','object':low})
-        self.items.append({'name':'high','string':'High Frequency Threshold','object':high})
-        self.items.append({'name':'preview','string':'Preview','object':preview})  
-        super().gui()
-        self.roi=g.currentWindow.currentROI
-        if self.roi is not None:
-            self.ui.rejected.connect(self.roi.redraw_trace)
-            self.ui.accepted.connect(self.roi.redraw_trace)
-        else:
-            preview.setChecked(False)
-            preview.setEnabled(False)
-    def __call__(self,low,high,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.tif.ndim != 3:
-            g.alert("Wavelet filter only works on 3 dimensional movies")
-            return
-        mx=self.tif.shape[2]
-        my=self.tif.shape[1]
-        self.newtif=np.zeros(self.tif.shape)
-        wavelet = signal.ricker
-        widths = np.arange(low, high)
-        for i in np.arange(my):
-            print(i)
-            for j in np.arange(mx):
-                cwtmatr = signal.cwt(self.tif[:, i, j], wavelet, widths)
-                self.newtif[:, i, j]=np.mean(cwtmatr,0)
-        self.newname=self.oldname+' - Wavelet Filtered'
-        return self.end()
-    def preview(self):
-        low=self.getValue('low')
-        high=self.getValue('high')
-        preview=self.getValue('preview')
-        if self.roi is not None:
-            if preview:
-                trace=self.roi.getTrace()
-                wavelet = signal.ricker
-                widths = np.arange(low, high)
-                cwtmatr = signal.cwt(trace, wavelet, widths)
-                newtrace=np.mean(cwtmatr,0)
-                roi_index=g.currentTrace.get_roi_index(self.roi)
-                g.currentTrace.update_trace_full(roi_index,newtrace) #update_trace_partial may speed it up
-            else:
-                self.roi.redraw_trace()
-wavelet_filter=Wavelet_filter()
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-class Bilateral_filter(BaseProcess):
-    ''' bilateral_filter( keepSourceWindow=False)
-    
-    Parameters:
-        | soft (bool)  --     True for guassian, False for hard filter
-        | beta (float) --     beta of kernel
-        | width (float) --    width of kernel
-        | stoptol (float) --  tolerance for convergence
-        | maxiter (int)  --   maximum number of iterations
-    Returns:
-        newWindow
-    '''
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        
-        soft=CheckBox()
-        soft.setChecked(True)
-        beta=SliderLabel(2)
-        beta.setRange(1,500)
-        beta.setValue(200)
-        width=SliderLabel(2)
-        width.setRange(1,50)
-        width.setValue(8)
-        stoptol=SliderLabel(4)
-        stoptol.setRange(0,.02)
-        stoptol.setValue(.001)
-        maxiter=SliderLabel(0)
-        maxiter.setRange(1,100)
-        maxiter.setValue(10)
-        preview=CheckBox()
-        preview.setChecked(True)
-        self.items.append({'name':'soft','string':'soft','object':soft})  
-        self.items.append({'name':'beta','string':'beta','object':beta})  
-        self.items.append({'name':'width','string':'width','object':width})  
-        self.items.append({'name':'stoptol','string':'stop tolerance','object':stoptol})  
-        self.items.append({'name':'maxiter','string':'Maximum Iterations','object':maxiter})  
-        self.items.append({'name':'preview','string':'Preview','object':preview})  
-        super().gui()
-        self.roi=g.currentWindow.currentROI
-        if self.roi is not None:
-            self.ui.rejected.connect(self.roi.redraw_trace)
-            self.ui.accepted.connect(self.roi.redraw_trace)
-        else:
-            preview.setChecked(False)
-            preview.setEnabled(False)
-        
-    def __call__(self,soft, beta, width, stoptol, maxiter, keepSourceWindow=False):
-        
-        self.start(keepSourceWindow)
-        if self.tif.ndim != 3:
-            g.alert("Bilateral filter requires 3-dimensional image.")
-            return
-        if g.settings['multiprocessing']:
-            self.newtif=bilateral_filter_multi(soft,beta,width,stoptol,maxiter,g.currentWindow.image)
-        else:
-            self.newtif=np.zeros(self.tif.shape)
-            mt,mx,my=self.tif.shape
-            for i in np.arange(mx):
-                for j in np.arange(my):
-                    self.newtif[:, i, j]=bilateral_smooth(soft,beta,width,stoptol,maxiter,self.tif[:,i,j])
-        self.newname=self.oldname+' - Bilateral Filtered'
-        return self.end()
-
-    def preview(self):
-        soft=self.getValue('soft')
-        beta=self.getValue('beta')
-        width=self.getValue('width')
-        stoptol=self.getValue('stoptol')
-        maxiter=self.getValue('maxiter')
-        preview=self.getValue('preview')
-        
-        if self.roi is not None:
-            if preview:
-                trace=self.roi.getTrace()
-                trace=bilateral_smooth(soft,beta,width,stoptol,maxiter,trace)
-                roi_index=g.currentTrace.get_roi_index(self.roi)
-                g.currentTrace.update_trace_full(roi_index,trace) #update_trace_partial may speed it up
-            else:
-                self.roi.redraw_trace()
-        
-
-def bilateral_filter_multi(soft,beta,width,stoptol,maxiter,tif):
-    nThreads= g.settings['nCores']
-    mt,mx,my=tif.shape
-    block_ends=np.linspace(0,mx,nThreads+1).astype(np.int)
-    data=[tif[:, block_ends[i]:block_ends[i+1],:] for i in np.arange(nThreads)] #split up data along x axis. each thread will get one.
-    args=(soft,beta,width,stoptol,maxiter)
-    progress = ProgressBar(bilateral_filter_inner, data, args, nThreads, msg='Performing Bilateral Filter')
-    if progress.results is None or any(r is None for r in progress.results):
-        result=None
-    else:
-        result=np.concatenate(progress.results,axis=1)
-    return result
-    
-    
-def bilateral_filter_inner(q_results, q_progress, q_status, child_conn, args):
-    data=child_conn.recv() # unfortunately this step takes a long time
-    percent=0  # This is the variable we send back which displays our progress
-    status=q_status.get(True) #this blocks the process from running until all processes are launched
-    if status=='Stop':
-        q_results.put(None) # if the user presses stop, return None
-    
-    
-    # Here is the meat of the inner_func.
-    soft,beta,width,stoptol,maxiter=args #unpack all the variables inside the args tuple
-    result=np.zeros(data.shape)
-    tt,xx,yy=data.shape
-    for x in np.arange(xx):
-        for y in np.arange(yy):
-            result[:,x,y]=bilateral_smooth(soft,beta,width,stoptol,maxiter,data[:,x,y])
-            if not q_status.empty(): #check if the stop button has been pressed
-                stop=q_status.get(False)
-                q_results.put(None)
-                return
-        if percent<int(100*x/xx):
-            percent=int(100*x/xx)
-            q_progress.put(percent)
-                    
-    # finally, when we've finished with our calculation, we send back the result
-    q_results.put(result)
-    
-def bilateral_smooth(soft,beta,width,stoptol,maxiter,y):
-    display=False       # 1 to report iteration values
-    
-    y=np.array(y[:])
-    N=np.size(y,0)
-    w=np.zeros((N,N))
-    j=np.arange(0,N)
-    
-    #construct initial bilateral kernel
-    for i in np.arange(0,N):
-        w[i,np.arange(0,N)]=(abs(i-j) <= width)
-    
-    #initial guess from input signal
-    xold=np.copy(y)
-    
-    #new matrix for storing distances
-    d=np.zeros((N,N))
-    
-    #fig1 = plt.plot(y)
-    
-    if (display):
-        if (soft):
-            print('Soft kernel')
-        else:
-            print('Hard kernel')
-        print('Kernel parameters beta= %d, W= %d' % (beta,width))
-        print('Iter# Change')
-    
-    #start iteration
-    iterate=1
-    gap=np.inf
-    
-    while (iterate < maxiter):
-    
-        if (display):
-            print('%d %f'% (iterate,gap))
-    
-        # calculate paiwise distances for all points
-        for i in np.arange(0,N):
-            d[:,i] = (0.5 * (xold - xold[i]) ** 2)
-        
-        #create kernel
-        if (soft):
-            W=np.multiply(np.exp(-beta*d),w)
-    
-        else:
-            W=np.multiply((d <= beta ** 2),w)
-        
-        #apply kernel to get weighted mean shift   
-        xnew1=np.sum(np.multiply(np.transpose(W),xold), axis=1)
-        xnew2=np.sum(W, axis=1)
-        xnew=np.divide(xnew1,xnew2)
-       
-        #plt.plot(xnew)   
-        
-        #check for convergence
-        gap=np.sum(np.square(xold-xnew))
-    
-        if (gap < stoptol):
-            if (display):
-                print('Converged in %d iterations' % iterate)
-            break
-    
-        xold=np.copy(xnew)
-        iterate+=1
-    return xold
-    
-bilateral_filter=Bilateral_filter()
-
-
-
-
-
-
-#from scipy import signal
-#data=g.currentTrace.rois[0]['roi'].getTrace()
-#wavelet = signal.ricker
-#widths = np.arange(1, 200)
-#cwtmatr = signal.cwt(data, wavelet, widths)
-#import pyqtgraph as pg
-#i=pg.image(cwtmatr.T)
+import numpy as np
+import skimage
+import skimage.filters
+from qtpy import QtWidgets, QtGui, QtCore
+from ..logger import logger
+from .. import global_vars as g
+from ..utils.BaseProcess import BaseProcess, SliderLabel, SliderLabelOdd, CheckBox
+from .progress_bar import ProgressBar
+
+__all__ = ['gaussian_blur', 'difference_of_gaussians', 'mean_filter', 'variance_filter', 'median_filter', 'butterworth_filter', 'boxcar_differential_filter','wavelet_filter','difference_filter', 'fourier_filter', 'bilateral_filter']
+###############################################################################
+##################   SPATIAL FILTERS       ####################################
+###############################################################################
+
+
+class Gaussian_blur(BaseProcess):
+    """ gaussian_blur(sigma, norm_edges=False, keepSourceWindow=False)
+
+    This applies a spatial gaussian_blur to every frame of your stack.  
+    
+    Args:
+        sigma (float): The width of the gaussian
+        norm_edges (bool): If true, this reduces the values of the pixels near the edges so they have the same standard deviation as the rest of the image
+
+    Returns:
+        flika.window.Window
+
+    """
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        logger.debug("Started 'running process.filters.gaussian_blur.gui()'")
+        self.gui_reset()
+        sigma=SliderLabel(2)
+        sigma.setRange(0,100)
+        sigma.setValue(1)
+        norm_edges=CheckBox()
+        norm_edges.setChecked(False)
+        preview=CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name': 'sigma', 'string': 'Sigma (pixels)', 'object': sigma})
+        self.items.append({'name': 'norm_edges', 'string': 'Normalize Edges', 'object': norm_edges})
+        self.items.append({'name': 'preview', 'string': 'Preview', 'object': preview})
+        super().gui()
+        self.preview()
+        logger.debug("Completed 'running process.filters.gaussian_blur.gui()'")
+
+    def __call__(self, sigma, norm_edges=False, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if norm_edges == True:
+            mode = 'constant'
+        else:
+            mode = 'nearest'
+        if sigma>0:
+            self.newtif=np.zeros(self.tif.shape)
+            if len(self.tif.shape)==3:
+                for i in np.arange(len(self.newtif)):
+                    self.newtif[i]=skimage.filters.gaussian(self.tif[i].astype(np.float64),sigma, mode=mode)
+            elif len(self.tif.shape)==2:
+                self.newtif=skimage.filters.gaussian(self.tif.astype(np.float64),sigma, mode=mode)
+            self.newtif=self.newtif.astype(g.settings['internal_data_type'])
+        else:
+            self.newtif=self.tif
+        self.newname=self.oldname+' - Gaussian Blur sigma='+str(sigma)
+        return self.end()
+    def preview(self):
+        logger.debug("Started 'running process.filters.gaussian_blur.preview()'")
+        norm_edges = self.getValue('norm_edges')
+        if norm_edges:
+            mode = 'constant'
+        else:
+            mode = 'nearest'
+        sigma=self.getValue('sigma')
+        preview=self.getValue('preview')
+        if preview:
+            if len(g.win.image.shape)==3:
+                testimage=g.win.image[g.win.currentIndex].astype(np.float64)
+            elif len(g.win.image.shape)==2:
+                testimage=g.win.image.astype(np.float64)
+            if sigma>0:
+                testimage=skimage.filters.gaussian(testimage,sigma, mode=mode)
+            g.win.imageview.setImage(testimage,autoLevels=False)
+        else:
+            g.win.reset()
+        logger.debug("Completed 'running process.filters.gaussian_blur.preview()'")
+gaussian_blur = Gaussian_blur()
+
+
+class Difference_of_Gaussians(BaseProcess):
+    """gaussian_blur(sigma1, sigma2, keepSourceWindow=False)
+
+    This subtracts one gaussian blurred image from another to spatially bandpass filter.
+
+    Args:
+        sigma1 (float): The width of the first gaussian
+        sigma2 (float): The width of the first gaussian
+
+    Returns:
+        flika.window.Window
+
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        self.gui_reset()
+        sigma1 = SliderLabel(2)
+        sigma1.setRange(0, 100)
+        sigma1.setValue(1)
+        sigma2 = SliderLabel(2)
+        sigma2.setRange(0, 100)
+        sigma2.setValue(2)
+        preview = CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name': 'sigma1', 'string': 'Sigma 1 (pixels)', 'object': sigma1})
+        self.items.append({'name': 'sigma2', 'string': 'Sigma 2 (pixels)', 'object': sigma2})
+        self.items.append({'name': 'preview', 'string': 'Preview', 'object': preview})
+        super().gui()
+        self.preview()
+
+    def __call__(self, sigma1, sigma2, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if sigma1 > 0 and sigma2 > 0:
+            self.newtif = np.zeros(self.tif.shape)
+            if len(self.tif.shape) == 3:
+                for i in np.arange(len(self.newtif)):
+                    self.newtif[i] = skimage.filters.gaussian(self.tif[i].astype(np.float64), sigma1, mode='nearest') -\
+                                     skimage.filters.gaussian(self.tif[i].astype(np.float64), sigma2, mode='nearest')
+            elif len(self.tif.shape) == 2:
+                self.newtif = skimage.filters.gaussian(self.tif.astype(np.float64), sigma1, mode='nearest') - \
+                              skimage.filters.gaussian(self.tif.astype(np.float64), sigma2, mode='nearest')
+            self.newtif = self.newtif.astype(g.settings['internal_data_type'])
+        else:
+            self.newtif = self.tif
+        self.newname = self.oldname + ' - Difference of Gaussians ({} {})'.format(sigma1, sigma2)
+        return self.end()
+
+    def preview(self):
+        sigma1 = self.getValue('sigma1')
+        sigma2 = self.getValue('sigma2')
+        preview = self.getValue('preview')
+        if preview:
+            if len(g.win.image.shape) == 3:
+                testimage = g.win.image[g.win.currentIndex].astype(np.float64)
+            elif len(g.win.image.shape) == 2:
+                testimage = g.win.image.astype(np.float64)
+            if sigma1 > 0 and sigma2 > 0:
+                testimage = skimage.filters.gaussian(testimage, sigma1, mode='nearest') - skimage.filters.gaussian(testimage, sigma2, mode='nearest')
+            g.win.imageview.setImage(testimage, autoLevels=False)
+        else:
+            g.win.reset()
+
+
+difference_of_gaussians = Difference_of_Gaussians()
+###############################################################################
+##################   TEMPORAL FILTERS       ###################################
+###############################################################################
+from scipy.signal import butter, filtfilt
+    
+
+class Butterworth_filter(BaseProcess):
+    """ butterworth_filter(filter_order, low, high, framerate, keepSourceWindow=False)
+
+    This filters a stack in time.
+    
+    Parameters:
+        filter_order (int): The order of the butterworth filter (higher order -> steeper cutoff).
+        low (float): The low frequency cutoff.  Must be between 0 and 1 and must be below high.
+        high (float): The high frequency cutoff.  Must be between 0 and 1 and must be above low.
+        framerate (float): The framerate in Hz. If set to zero, a framerate of 2 Hz will be used, so as to set the Nyquist frequency to 1. Default is 0.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def framerate_adjusted(self, rate):
+        high = self.items[2]
+        assert high['name'] == 'high'
+        if rate == 0:
+            rate = 2
+        high['object'].setMaximum(rate / 2)
+
+
+    def gui(self):
+        self.gui_reset()
+        filter_order=QtWidgets.QSpinBox()
+        filter_order.setRange(1,10)
+        low=SliderLabel(5)
+        low.setRange(0,1)
+        low.setValue(0)
+        high=SliderLabel(5)
+        high.setRange(0,1)
+        high.setValue(1)
+        framerate = SliderLabel(2)
+        framerate.setRange(0, 1000)
+        low.valueChanged.connect(lambda low: high.setMinimum(low))
+        high.valueChanged.connect(lambda high: low.setMaximum(high))
+        framerate.valueChanged.connect(self.framerate_adjusted)
+        preview=CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name':'filter_order','string':'Filter Order','object':filter_order})
+        self.items.append({'name':'low','string':'Low Cutoff Frequency','object':low})
+        self.items.append({'name':'high','string':'High Cutoff Frequency','object':high})
+        self.items.append({'name': 'framerate', 'string': 'Frame rate (Hz)', 'object': framerate})
+        self.items.append({'name':'preview','string':'Preview','object':preview})        
+        super().gui()
+        if g.win is None:
+            self.roi = None
+        else:
+            self.roi=g.win.currentROI
+        if self.roi is not None:
+            self.ui.rejected.connect(self.roi.redraw_trace)
+            self.ui.accepted.connect(self.roi.redraw_trace)
+        if self.roi is None or g.currentTrace is None:
+            preview.setChecked(False)
+            preview.setEnabled(False)
+        
+    def __call__(self, filter_order, low, high, framerate=0, keepSourceWindow=False):
+        if framerate == 0:
+            framerate = 2
+        if low == 0 and high == framerate/2:
+            return
+        self.start(keepSourceWindow)
+        if self.tif.ndim != 3:
+            g.alert("Butterworth filter only works on 3-dimensional movies.")
+            return
+        if g.settings['multiprocessing']:
+            self.newtif = butterworth_filter_multi(filter_order, low/(framerate/2), high/(framerate/2), g.win.image)
+        else:
+            self.newtif = np.zeros(self.tif.shape, dtype=g.settings.d['internal_data_type'])
+            mt, mx, my = self.tif.shape
+            b, a, padlen = self.makeButterFilter(filter_order, low/(framerate/2), high/(framerate/2))
+            for i in np.arange(mx):
+                for j in np.arange(my):
+                    self.newtif[:, i, j] = filtfilt(b, a, self.tif[:, i, j], padlen=padlen)
+        self.newname = self.oldname+' - Butter Filtered'
+        return self.end()
+        
+    def preview(self):
+        if g.currentTrace is not None:
+            framerate = self.getValue('framerate')
+            if framerate == 0:
+                framerate = 2
+            filter_order = self.getValue('filter_order')
+            low = self.getValue('low')
+            high = self.getValue('high')
+            preview = self.getValue('preview')
+            if self.roi is not None:
+                if preview:
+                    if (low == 0 and high == framerate/2) or (low == 0 and high == 0):
+                        self.roi.onRegionChangeFinished() #redraw roi without filter
+                    else:
+                        b, a, padlen = self.makeButterFilter(filter_order, low/(framerate/2), high/(framerate/2))
+                        trace = self.roi.getTrace()
+                        trace = filtfilt(b,a, trace, padlen=padlen)
+                        roi_index = g.currentTrace.get_roi_index(self.roi)
+                        g.currentTrace.update_trace_full(roi_index,trace) #update_trace_partial may speed it up
+                else:
+                    self.roi.redraw_trace()
+    def makeButterFilter(self, filter_order, low, high):
+        padlen = 0
+        if high == 1:
+            if low == 0: #if there is no temporal filter at all,
+                return None,None,None
+            else: #if only high pass temporal filter
+                [b, a] = butter(filter_order, low, btype='highpass')
+                padlen = 3
+        else:
+            if low == 0:
+                [b,a] = butter(filter_order, high, btype='lowpass')
+            else:
+                [b,a] = butter(filter_order, [low, high], btype='bandpass')
+            padlen = 6
+        return b, a, padlen
+        
+butterworth_filter=Butterworth_filter()
+
+        
+def butterworth_filter_multi(filter_order, low, high, tif):
+    nThreads = g.settings['nCores']
+    mt, mx, my = tif.shape
+    block_ends = np.linspace(0, mx, nThreads+1).astype(np.int)
+    data = [tif[:, block_ends[i]:block_ends[i+1], :] for i in np.arange(nThreads)] #split up data along x axis. each thread will get one.
+    args = (filter_order, low, high)
+    progress = ProgressBar(butterworth_filter_multi_inner, data, args, nThreads, msg='Performing Butterworth Filter')
+    if progress.results is None or any(r is None for r in progress.results):
+        result = None
+    else:
+        result = np.concatenate(progress.results,axis=1).astype(g.settings['internal_data_type'])
+    return result
+    
+
+def butterworth_filter_multi_inner(q_results, q_progress, q_status, child_conn, args):
+    data = child_conn.recv()
+    status = q_status.get(True) #this blocks the process from running until all processes are launched
+    if status == 'Stop':
+        q_results.put(None)
+    
+    def makeButterFilter(filter_order, low, high):
+        padlen = 0
+        if high == 1:
+            if low == 0: #if there is no temporal filter at all,
+                return None,None,None
+            else: #if only high pass temporal filter
+                [b,a] = butter(filter_order,low,btype='highpass')
+                padlen = 3
+        else:
+            if low == 0:
+                [b,a]= butter(filter_order, high, btype='lowpass')
+            else:
+                [b,a]=butter(filter_order, [low,high], btype='bandpass')
+            padlen = 6
+        return b, a, padlen
+        
+    filter_order,low,high = args
+    b, a, padlen = makeButterFilter(filter_order,low,high)
+    mt, mx, my = data.shape
+    result = np.zeros(data.shape,g.settings['internal_data_type'])
+    nPixels = mx*my
+    pixel = 0
+    percent = 0
+    for x in np.arange(mx):
+        for y in np.arange(my):
+            if not q_status.empty():
+                stop = q_status.get(False)
+                q_results.put(None)
+                return
+            pixel += 1
+            if percent < int(100*pixel/nPixels):
+                percent = int(100*pixel/nPixels)
+                q_progress.put(percent)
+            result[:, x, y] = filtfilt(b,a, data[:, x, y], padlen=padlen)
+    q_results.put(result)
+
+from scipy.ndimage.filters import convolve
+class Mean_filter(BaseProcess):
+    """ mean_filter(nFrames, keepSourceWindow=False)
+
+    This filters a stack in time.
+    
+    Parameters:
+        nFrames (int): Number of frames to average
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        nFrames=SliderLabel(0)
+        nFrames.setRange(1,100)
+        preview=CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name':'nFrames','string':'nFrames','object':nFrames})
+        self.items.append({'name':'preview','string':'Preview','object':preview})        
+        super().gui()
+        self.roi=g.win.currentROI
+        if self.roi is not None:
+            self.ui.rejected.connect(self.roi.redraw_trace)
+            self.ui.accepted.connect(self.roi.redraw_trace)
+        else:
+            preview.setChecked(False)
+            preview.setEnabled(False)
+            
+    def __call__(self,nFrames,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.tif.dtype == np.float16:
+            g.alert("Mean Filter does not support float16 type arrays")
+            return
+        if self.tif.ndim != 3:
+            g.alert("Mean Filter only supports 3-dimensional movies.")
+            return
+        self.newtif=convolve(self.tif,weights=np.full((nFrames,1,1),1.0/nFrames))        
+        self.newname=self.oldname+' - Mean Filtered'
+        return self.end()
+    def preview(self):
+        nFrames=self.getValue('nFrames')
+        preview=self.getValue('preview')
+        if self.roi is not None:
+            if preview:
+                if nFrames==1:
+                    self.roi.redraw_trace() #redraw roi without filter
+                else:
+                    trace=self.roi.getTrace()
+                    trace=convolve(trace,weights=np.full((nFrames),1.0/nFrames))        
+                    roi_index=g.currentTrace.get_roi_index(self.roi)
+                    g.currentTrace.update_trace_full(roi_index,trace) #update_trace_partial may speed it up
+            else:
+                self.roi.redraw_trace()
+mean_filter=Mean_filter()
+
+def varfilt(trace, nFrames):
+    result = np.zeros_like(trace)
+    mt = len(trace)
+    for i in np.arange(mt):
+        i0 = int(i-nFrames/2)
+        i1 = int(i+nFrames/2)
+        if i0 < 0:
+            i0 = 0
+        if i1 > len(trace):
+            i1 = len(trace)
+        result[i] = np.var(trace[i0:i1])
+    return result
+
+class Variance_filter(BaseProcess):
+    """ variance_filter(nFrames, keepSourceWindow=False)
+
+    This filters a stack in time.
+
+    Parameters:
+        nFrames (int): Number of frames to take teh variance of
+    Returns:
+        newWindow
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        self.gui_reset()
+        nFrames = SliderLabel(0)
+        nFrames.setRange(1, 100)
+        preview = CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name': 'nFrames', 'string': 'nFrames', 'object': nFrames})
+        self.items.append({'name': 'preview', 'string': 'Preview', 'object': preview})
+        super().gui()
+        self.roi = g.win.currentROI
+        if self.roi is not None:
+            self.ui.rejected.connect(self.roi.redraw_trace)
+            self.ui.accepted.connect(self.roi.redraw_trace)
+        else:
+            preview.setChecked(False)
+            preview.setEnabled(False)
+
+    def __call__(self, nFrames, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.tif.dtype == np.float16:
+            g.alert("Variance filter does not support float16 type arrays")
+            return
+        if self.tif.ndim != 3:
+            g.alert("Variance filter only supports 3-dimensional movies.")
+            return
+        self.newtif = np.zeros(self.tif.shape)
+        _, mx, my = self.tif.shape
+        for i in np.arange(my):
+            for j in np.arange(mx):
+                self.newtif[:, i, j] = varfilt(self.tif[:, i, j], nFrames)
+        self.newname = self.oldname + ' - Variance Filtered'
+        return self.end()
+
+    def preview(self):
+        nFrames = self.getValue('nFrames')
+        preview = self.getValue('preview')
+        if self.roi is not None:
+            if preview:
+                if nFrames == 1:
+                    self.roi.redraw_trace()  # redraw roi without filter
+                else:
+                    trace = self.roi.getTrace()
+                    trace = varfilt(trace, nFrames)
+                    roi_index = g.currentTrace.get_roi_index(self.roi)
+                    g.currentTrace.update_trace_full(roi_index, trace)  # update_trace_partial may speed it up
+            else:
+                self.roi.redraw_trace()
+
+
+variance_filter = Variance_filter()
+
+from scipy.signal import medfilt
+class Median_filter(BaseProcess):
+    """ median_filter(nFrames, keepSourceWindow=False)
+
+    This filters a stack in time.
+    
+    Parameters:
+        nFrames (int): Number of frames to average.  This must be an odd number
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        nFrames=SliderLabelOdd()
+        nFrames.setRange(1,100)
+        preview=CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name':'nFrames','string':'nFrames','object':nFrames})
+        self.items.append({'name':'preview','string':'Preview','object':preview})        
+        super().gui()
+        self.roi=g.win.currentROI
+        if self.roi is not None:
+            self.ui.rejected.connect(self.roi.redraw_trace)
+            self.ui.accepted.connect(self.roi.redraw_trace)
+        else:
+            preview.setChecked(False)
+            preview.setEnabled(False)
+            
+    def __call__(self, nFrames, keepSourceWindow=False):
+        if nFrames%2 == 0: #if value is even:
+            g.alert('median_filter only takes odd numbers.  Operation cancelled')
+            return None
+        self.start(keepSourceWindow)
+        if self.tif.ndim < 3:
+            g.alert("Median filter requires at least 3 dimensions. %d < 3" % self.tif.ndim)
+            return
+        mx=self.tif.shape[2]
+        my=self.tif.shape[1]
+        self.newtif = np.zeros(self.tif.shape)
+        for i in np.arange(my):
+            for j in np.arange(mx):
+                self.newtif[:, i, j]=medfilt(self.tif[:, i, j], kernel_size=nFrames)      
+        self.newname=self.oldname+' - Median Filtered'
+        return self.end()
+    def preview(self):
+        nFrames=self.getValue('nFrames')
+        preview=self.getValue('preview')
+        if self.roi is not None:
+            if preview:
+                print(nFrames)
+                if nFrames==1:
+                    self.roi.redraw_trace() #redraw roi without filter
+                elif nFrames%2==0: #if value is even
+                    return None
+                else:
+                    trace=self.roi.getTrace()
+                    trace=medfilt(trace,kernel_size=nFrames)
+                    roi_index=g.currentTrace.get_roi_index(self.roi)
+                    g.currentTrace.update_trace_full(roi_index,trace) #update_trace_partial may speed it up
+            else:
+                self.roi.redraw_trace()
+                
+median_filter=Median_filter()
+
+
+
+
+from scipy.fftpack import fft, ifft, fftfreq
+class Fourier_filter(BaseProcess):
+    """ fourier_filter(frame_rate, low, high, loglogPreview, keepSourceWindow=False)
+
+    I'm going to eventually plot the trace in the frequency domain inside this box so you can see where the power is.
+
+    Parameters:
+        frame_rate (int): Frame Rate in Hz
+        low (float): Low cutoff frequency for the fourier filter
+        high (float): High cutoff frequency for fourier filter
+        loglogPreview (boolean): whether or not to plot frequency spectrum on log log axes
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        frame_rate=QtWidgets.QDoubleSpinBox()
+        frame_rate.setRange(.01,1000)
+        frame_rate.setValue(200)
+        low=SliderLabel(5)
+        low.setRange(0,1)
+        low.setValue(0)
+        high=SliderLabel(5)
+        high.setRange(0,1)
+        high.setValue(1)
+        frame_rate.valueChanged.connect(self.frame_rate_changed)
+        low.valueChanged.connect(lambda low: high.setMinimum(low))
+        high.valueChanged.connect(lambda high: low.setMaximum(high))
+        preview=CheckBox()
+        preview.setChecked(True)
+        loglogPreview=CheckBox()
+        self.items.append({'name':'frame_rate','string':'Frame Rate (Hz)','object':frame_rate})
+        self.items.append({'name':'low','string':'Low Cutoff Frequency','object':low})
+        self.items.append({'name':'high','string':'High Cutoff Frequency','object':high})
+        self.items.append({'name':'loglogPreview','string':'Plot frequency spectrum on log log axes','object':loglogPreview})    
+        self.items.append({'name':'preview','string':'Preview','object':preview})        
+        super().gui()
+        self.roi=g.win.currentROI
+        if self.roi is not None:
+            self.ui.rejected.connect(self.roi.redraw_trace)
+            self.ui.accepted.connect(self.roi.redraw_trace)
+        else:
+            preview.setChecked(False)
+            preview.setEnabled(False)
+            loglogPreview.setEnabled(False)
+
+    def __call__(self, frame_rate, low, high, loglogPreview, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.tif.dtype == np.float16:
+            g.alert("Fourier transform does not support float16 movies.")
+            return
+        if self.tif.ndim != 3 or self.tif.shape[2] == 3:
+            g.alert('Fourier transform requires 3 dimensional movies.')
+            return
+        if low==0 and high==frame_rate/2.0:
+            return
+        mt,mx,my=self.tif.shape
+        W = fftfreq(mt, d=1.0/frame_rate)
+        filt=np.ones((mt))
+        filt[(np.abs(W)<low)] = 0
+        filt[(np.abs(W)>high)] = 0
+        self.newtif=np.zeros(self.tif.shape)
+        for i in np.arange(my):
+            for j in np.arange(mx):
+                f_signal = fft(self.tif[:, i, j])
+                f_signal*=filt
+                self.newtif[:, i, j]=np.real(ifft(f_signal))
+        self.newname=self.oldname+' - Fourier Filtered'
+        return self.end()
+    def preview(self):
+        frame_rate=self.getValue('frame_rate')
+        low=self.getValue('low')
+        high=self.getValue('high')
+        loglogPreview=self.getValue('loglogPreview')
+        preview=self.getValue('preview')
+        if self.roi is not None:
+            if preview:
+                if (low==0 and high==frame_rate/2.0) or (low==0 and high==0):
+                    self.roi.redraw_trace() #redraw roi without filter
+                else:
+                    trace=self.roi.getTrace()
+                    W = fftfreq(len(trace), d=1.0/frame_rate)
+                    f_signal = fft(trace)
+                    f_signal[(np.abs(W)<low)] = 0
+                    f_signal[(np.abs(W)>high)] = 0
+                    cut_signal=np.real(ifft(f_signal))
+                    roi_index=g.currentTrace.get_roi_index(self.roi)
+                    g.currentTrace.update_trace_full(roi_index,cut_signal) #update_trace_partial may speed it up
+            else:
+                self.roi.redraw_trace()
+                
+    def frame_rate_changed(self):
+        low=[item for item in self.items if item['name']=='low'][0]['object']
+        high=[item for item in self.items if item['name']=='high'][0]['object']
+        frame_rate=[item for item in self.items if item['name']=='frame_rate'][0]['object']
+        f=frame_rate.value()
+        low.setRange(0.0,f/2.0)
+        high.setRange(0.0,f/2.0)
+        low.setValue(0)
+        high.setValue(f/2.0)
+""" This is demo code for plotting in the frequency domain, something I hoepfully will get around to implementing
+
+from numpy import sin, linspace, pi
+from pylab import plot, show, title, xlabel, ylabel, subplot
+from scipy import fft, arange
+
+def plotSpectrum(y,Fs):
+    n = len(y) # length of the signal
+    k = arange(n)
+    W = fftfreq(len(y), d=1/Fs)
+
+    Y = fft(y) # fft computing and normalization
+    f_signal[(np.abs(W)>10)] = 0
+    plot(abs(f_signal)[0:N/2])
+    cut_signal=np.real(ifft(f_signal))
+    p=plot(trace)
+    p.plot(cut_signal,pen=pg.mkPen('r'))
+    
+    plot(frq,abs(f_signal),'r') # plotting the spectrum
+    xlabel('Freq (Hz)')
+    ylabel('|Y(freq)|')"""
+        
+fourier_filter=Fourier_filter()
+
+
+
+class Difference_filter(BaseProcess):
+    """ difference_filter(keepSourceWindow=False)
+
+    Subtracts each frame from the preceeding frame
+
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        if super().gui()==False:
+            return False
+    def __call__(self,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        self.newtif=np.zeros(self.tif.shape)
+        for i in np.arange(1,len(self.newtif)):
+            self.newtif[i]=self.tif[i]-self.tif[i-1]
+        self.newname=self.oldname+' - Difference Filtered'
+        return self.end()
+difference_filter=Difference_filter()
+
+    
+class Boxcar_differential_filter(BaseProcess):
+    """ boxcar_differential_filter(minNframes, maxNframes, keepSourceWindow=False)
+
+    Applies a Boxcar differential filter by comparing each frameat index I to the frames in range [I+minNframes, I+maxNframes]
+
+    Parameters:
+        minNframes (int): The starting point of your boxcar window.
+        maxNframes (int): The ending point of your boxcar window.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        minNframes=SliderLabel(0)
+        minNframes.setRange(1,100)
+        maxNframes=SliderLabel(0)
+        maxNframes.setRange(2,101)
+        minNframes.valueChanged.connect(lambda minn: maxNframes.setMinimum(minn+1))
+        maxNframes.valueChanged.connect(lambda maxx: minNframes.setMaximum(maxx-1))
+        preview=CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name':'minNframes','string':'Minimum Number of Frames','object':minNframes})
+        self.items.append({'name':'maxNframes','string':'Maximum Number of Frames','object':maxNframes})
+        self.items.append({'name':'preview','string':'Preview','object':preview})  
+        if super().gui()==False:
+            return False
+        self.roi=g.win.currentROI
+        if self.roi is not None:
+            self.ui.rejected.connect(self.roi.redraw_trace)
+            self.ui.accepted.connect(self.roi.redraw_trace)
+        else:
+            preview.setChecked(False)
+            preview.setEnabled(False)
+    def __call__(self,minNframes,maxNframes,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        self.newtif=np.zeros(self.tif.shape)
+        for i in np.arange(maxNframes,len(self.newtif)):
+            self.newtif[i]=self.tif[i]-np.min(self.tif[i-maxNframes:i-minNframes],0)
+        self.newname=self.oldname+' - Boxcar Differential Filtered'
+        return self.end()
+    def preview(self):
+        minNframes=self.getValue('minNframes')
+        maxNframes=self.getValue('maxNframes')
+        preview=self.getValue('preview')
+        if self.roi is not None:
+            if preview:
+                self.tif=self.roi.window.image
+                (mt,mx,my)=self.tif.shape
+                cnt=np.array([np.array([np.array([p[1],p[0]])]) for p in self.roi.pts ])
+                mask=np.zeros(self.tif[0,:,:].shape,np.uint8)
+                cv2.drawContours(mask,[cnt],0,255,-1)
+                mask=mask.reshape(mx*my).astype(np.bool)
+                tif=self.tif.reshape((mt,mx*my))
+                tif=tif[:,mask]
+                newtrace=np.zeros(mt)
+                for i in np.arange(maxNframes,mt):
+                    newtrace[i]=np.mean(tif[i]-np.min(tif[i-maxNframes:i-minNframes],0))
+                roi_index=g.currentTrace.get_roi_index(self.roi)
+                g.currentTrace.update_trace_full(roi_index,newtrace) #update_trace_partial may speed it up
+            else:
+                self.roi.redraw_trace()
+boxcar_differential_filter=Boxcar_differential_filter()
+    
+    
+from scipy import signal
+class Wavelet_filter(BaseProcess):
+    ''' wavelet_filter(low, high, keepSourceWindow=False)
+
+    ***Warning!! This function is extremely slow.***
+    
+    Parameters:
+        low (int): The starting point of your boxcar window.
+        high (int): The ending point of your boxcar window.
+    Returns:
+        newWindow
+    '''
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        low=SliderLabel(0)
+        low.setRange(1,50)
+        high=SliderLabel(0)
+        high.setRange(2,50)
+        low.valueChanged.connect(lambda minn: high.setMinimum(minn+1))
+        high.valueChanged.connect(lambda maxx: low.setMaximum(maxx-1))
+        preview=CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name':'low','string':'Low Frequency Threshold','object':low})
+        self.items.append({'name':'high','string':'High Frequency Threshold','object':high})
+        self.items.append({'name':'preview','string':'Preview','object':preview})  
+        super().gui()
+        self.roi=g.win.currentROI
+        if self.roi is not None:
+            self.ui.rejected.connect(self.roi.redraw_trace)
+            self.ui.accepted.connect(self.roi.redraw_trace)
+        else:
+            preview.setChecked(False)
+            preview.setEnabled(False)
+    def __call__(self,low,high,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.tif.ndim != 3:
+            g.alert("Wavelet filter only works on 3 dimensional movies")
+            return
+        mx=self.tif.shape[2]
+        my=self.tif.shape[1]
+        self.newtif=np.zeros(self.tif.shape)
+        wavelet = signal.ricker
+        widths = np.arange(low, high)
+        for i in np.arange(my):
+            print(i)
+            for j in np.arange(mx):
+                cwtmatr = signal.cwt(self.tif[:, i, j], wavelet, widths)
+                self.newtif[:, i, j]=np.mean(cwtmatr,0)
+        self.newname=self.oldname+' - Wavelet Filtered'
+        return self.end()
+    def preview(self):
+        low=self.getValue('low')
+        high=self.getValue('high')
+        preview=self.getValue('preview')
+        if self.roi is not None:
+            if preview:
+                trace=self.roi.getTrace()
+                wavelet = signal.ricker
+                widths = np.arange(low, high)
+                cwtmatr = signal.cwt(trace, wavelet, widths)
+                newtrace=np.mean(cwtmatr,0)
+                roi_index=g.currentTrace.get_roi_index(self.roi)
+                g.currentTrace.update_trace_full(roi_index,newtrace) #update_trace_partial may speed it up
+            else:
+                self.roi.redraw_trace()
+wavelet_filter=Wavelet_filter()
+
+
+class Bilateral_filter(BaseProcess):
+    """bilateral_filter( keepSourceWindow=False)
+    
+    Parameters:
+        soft (bool): True for guassian, False for hard filter
+        beta (float): beta of kernel
+        width (float): width of kernel
+        stoptol (float): tolerance for convergence
+        maxiter (int): maximum number of iterations
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        
+        soft=CheckBox()
+        soft.setChecked(True)
+        beta=SliderLabel(2)
+        beta.setRange(1,500)
+        beta.setValue(200)
+        width=SliderLabel(2)
+        width.setRange(1,50)
+        width.setValue(8)
+        stoptol=SliderLabel(4)
+        stoptol.setRange(0,.02)
+        stoptol.setValue(.001)
+        maxiter=SliderLabel(0)
+        maxiter.setRange(1,100)
+        maxiter.setValue(10)
+        preview=CheckBox()
+        preview.setChecked(True)
+        self.items.append({'name':'soft','string':'soft','object':soft})  
+        self.items.append({'name':'beta','string':'beta','object':beta})  
+        self.items.append({'name':'width','string':'width','object':width})  
+        self.items.append({'name':'stoptol','string':'stop tolerance','object':stoptol})  
+        self.items.append({'name':'maxiter','string':'Maximum Iterations','object':maxiter})  
+        self.items.append({'name':'preview','string':'Preview','object':preview})  
+        super().gui()
+        self.roi=g.win.currentROI
+        if self.roi is not None:
+            self.ui.rejected.connect(self.roi.redraw_trace)
+            self.ui.accepted.connect(self.roi.redraw_trace)
+        else:
+            preview.setChecked(False)
+            preview.setEnabled(False)
+        
+    def __call__(self,soft, beta, width, stoptol, maxiter, keepSourceWindow=False):
+        
+        self.start(keepSourceWindow)
+        if self.tif.ndim != 3:
+            g.alert("Bilateral filter requires 3-dimensional image.")
+            return
+        if g.settings['multiprocessing']:
+            self.newtif=bilateral_filter_multi(soft,beta,width,stoptol,maxiter,g.win.image)
+        else:
+            self.newtif=np.zeros(self.tif.shape)
+            mt,mx,my=self.tif.shape
+            for i in np.arange(mx):
+                for j in np.arange(my):
+                    self.newtif[:, i, j]=bilateral_smooth(soft,beta,width,stoptol,maxiter,self.tif[:,i,j])
+        self.newname=self.oldname+' - Bilateral Filtered'
+        return self.end()
+
+    def preview(self):
+        soft=self.getValue('soft')
+        beta=self.getValue('beta')
+        width=self.getValue('width')
+        stoptol=self.getValue('stoptol')
+        maxiter=self.getValue('maxiter')
+        preview=self.getValue('preview')
+        
+        if self.roi is not None:
+            if preview:
+                trace=self.roi.getTrace()
+                trace=bilateral_smooth(soft,beta,width,stoptol,maxiter,trace)
+                roi_index=g.currentTrace.get_roi_index(self.roi)
+                g.currentTrace.update_trace_full(roi_index,trace) #update_trace_partial may speed it up
+            else:
+                self.roi.redraw_trace()
+        
+
+def bilateral_filter_multi(soft,beta,width,stoptol,maxiter,tif):
+    nThreads= g.settings['nCores']
+    mt,mx,my=tif.shape
+    block_ends=np.linspace(0,mx,nThreads+1).astype(np.int)
+    data=[tif[:, block_ends[i]:block_ends[i+1],:] for i in np.arange(nThreads)] #split up data along x axis. each thread will get one.
+    args=(soft,beta,width,stoptol,maxiter)
+    progress = ProgressBar(bilateral_filter_inner, data, args, nThreads, msg='Performing Bilateral Filter')
+    if progress.results is None or any(r is None for r in progress.results):
+        result=None
+    else:
+        result=np.concatenate(progress.results,axis=1)
+    return result
+    
+    
+def bilateral_filter_inner(q_results, q_progress, q_status, child_conn, args):
+    data=child_conn.recv() # unfortunately this step takes a long time
+    percent=0  # This is the variable we send back which displays our progress
+    status=q_status.get(True) #this blocks the process from running until all processes are launched
+    if status=='Stop':
+        q_results.put(None) # if the user presses stop, return None
+    
+    
+    # Here is the meat of the inner_func.
+    soft,beta,width,stoptol,maxiter=args #unpack all the variables inside the args tuple
+    result=np.zeros(data.shape)
+    tt,xx,yy=data.shape
+    for x in np.arange(xx):
+        for y in np.arange(yy):
+            result[:,x,y]=bilateral_smooth(soft,beta,width,stoptol,maxiter,data[:,x,y])
+            if not q_status.empty(): #check if the stop button has been pressed
+                stop=q_status.get(False)
+                q_results.put(None)
+                return
+        if percent<int(100*x/xx):
+            percent=int(100*x/xx)
+            q_progress.put(percent)
+                    
+    # finally, when we've finished with our calculation, we send back the result
+    q_results.put(result)
+    
+def bilateral_smooth(soft,beta,width,stoptol,maxiter,y):
+    display=False       # 1 to report iteration values
+    
+    y=np.array(y[:])
+    N=np.size(y,0)
+    w=np.zeros((N,N))
+    j=np.arange(0,N)
+    
+    #construct initial bilateral kernel
+    for i in np.arange(0,N):
+        w[i,np.arange(0,N)]=(abs(i-j) <= width)
+    
+    #initial guess from input signal
+    xold=np.copy(y)
+    
+    #new matrix for storing distances
+    d=np.zeros((N,N))
+    
+    #fig1 = plt.plot(y)
+    
+    if (display):
+        if (soft):
+            print('Soft kernel')
+        else:
+            print('Hard kernel')
+        print('Kernel parameters beta= %d, W= %d' % (beta,width))
+        print('Iter# Change')
+    
+    #start iteration
+    iterate=1
+    gap=np.inf
+    
+    while (iterate < maxiter):
+    
+        if (display):
+            print('%d %f'% (iterate,gap))
+    
+        # calculate paiwise distances for all points
+        for i in np.arange(0,N):
+            d[:,i] = (0.5 * (xold - xold[i]) ** 2)
+        
+        #create kernel
+        if (soft):
+            W=np.multiply(np.exp(-beta*d),w)
+    
+        else:
+            W=np.multiply((d <= beta ** 2),w)
+        
+        #apply kernel to get weighted mean shift   
+        xnew1=np.sum(np.multiply(np.transpose(W),xold), axis=1)
+        xnew2=np.sum(W, axis=1)
+        xnew=np.divide(xnew1,xnew2)
+       
+        #plt.plot(xnew)   
+        
+        #check for convergence
+        gap=np.sum(np.square(xold-xnew))
+    
+        if (gap < stoptol):
+            if (display):
+                print('Converged in %d iterations' % iterate)
+            break
+    
+        xold=np.copy(xnew)
+        iterate+=1
+    return xold
+    
+bilateral_filter=Bilateral_filter()
+
+
+
+
+
+
+#from scipy import signal
+#data=g.currentTrace.rois[0]['roi'].getTrace()
+#wavelet = signal.ricker
+#widths = np.arange(1, 200)
+#cwtmatr = signal.cwt(data, wavelet, widths)
+#import pyqtgraph as pg
+#i=pg.image(cwtmatr.T)
 #i.view.setAspectLocked(lock=True, ratio=cwtmatr.shape[0]/cwtmatr.shape[1]*20)
```

### Comparing `flika-0.2.9/flika/process/math_.py` & `flika-0.3.0/flika/process/math_.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,283 +1,373 @@
-# -*- coding: utf-8 -*-
-import numpy as np
-from qtpy import QtGui, QtWidgets, QtCore
-from .. import global_vars as g
-from .BaseProcess import BaseProcess, CheckBox, ComboBox
-from ..window import Window
-
-__all__ = ['subtract','multiply','power','ratio','absolute_value','subtract_trace','divide_trace']
-
-
-def upgrade_dtype(dtype):
-    if dtype==np.uint8:
-        return np.uint16
-    elif dtype==np.uint16:
-        return np.uint32
-    elif dtype==np.uint32:
-        return np.uint64
-    elif dtype==np.uint64:
-        return np.int8
-    elif dtype==np.int8:
-        return np.int16
-    elif dtype==np.int16:
-        return np.int32
-    elif dtype==np.int32:
-        return np.int64
-    elif dtype==np.float16:
-        return np.float32
-    elif dtype==np.float32:
-        return np.float64
-
-
-class Subtract(BaseProcess):
-    """ subtract(value, keepSourceWindow=False)
-    This takes a value and subtracts it from the current window's image.
-    
-    Parameters:
-        | value (int) -- The number you are subtracting.
-    Returns:
-        newWindow
-    """
-    __url__ = ""
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        value=QtWidgets.QDoubleSpinBox()
-        if g.currentWindow is not None:
-            value.setRange(-1 * np.max(g.currentWindow.image),np.max(g.currentWindow.image)) # -np.max sometimes returns abnormal large value
-            value.setValue(np.min(g.currentWindow.image))
-        self.items.append({'name':'value','string':'Value','object':value})
-        self.items.append({'name':'preview','string':'Preview','object':CheckBox()})
-        super().gui()
-    def __call__(self,value,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if hasattr(value,'is_integer') and value.is_integer():
-            value = int(value)
-        if np.issubdtype(self.tif.dtype,np.integer):
-            ddtype=np.iinfo(self.tif.dtype)
-            while np.min(self.tif)-value<ddtype.min or np.max(self.tif)-value>ddtype.max: # if we exceed the bounds of the datatype
-                ddtype=np.iinfo(upgrade_dtype(ddtype.dtype))
-            self.newtif=self.tif.astype(ddtype.dtype)-value
-        else:
-            self.newtif=self.tif-value
-        self.newname=self.oldname+' - Subtracted '+str(value)
-        return self.end()
-    def preview(self):
-        value=self.getValue('value')
-        preview=self.getValue('preview')
-        if preview:
-            testimage=np.copy(g.currentWindow.image[g.currentWindow.currentIndex])
-            testimage=testimage-value
-            g.currentWindow.imageview.setImage(testimage,autoLevels=False)
-        else:
-            g.currentWindow.reset()
-subtract=Subtract()
-
-class Subtract_trace(BaseProcess):
-    """ subtract_trace(keepSourceWindow=False)
-    This takes the most recently plotted trace and subtracts it from each corresponding frame.
-    
-    Parameters:
-        | 
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def __call__(self,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        trace=g.currentTrace.rois[-1]['roi'].getTrace()
-        nDims=len(self.tif.shape)
-        if nDims !=3:
-            g.alert('Wrong number of dimensions')
-            return self.end()
-        if self.tif.shape[0]!=len(trace):
-            g.alert('Wrong trace length')
-            return self.end()
-        self.newtif=np.transpose(np.transpose(self.tif)-trace)
-        self.newname=self.oldname+' - subtracted trace'
-        return self.end()
-subtract_trace=Subtract_trace()
-
-class Divide_trace(BaseProcess):
-    """ divide_trace(keepSourceWindow=False)
-    This takes the most recently plotted trace and divides each pixel in the current Window by its value.
-    
-    Parameters:
-        | 
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def __call__(self,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        trace=g.currentTrace.rois[-1]['roi'].getTrace()
-        nDims=len(self.tif.shape)
-        if nDims !=3:
-            g.alert('Wrong number of dimensions')
-            return self.end()
-        if self.tif.shape[0]!=len(trace):
-            g.alert('Wrong trace length')
-            return self.end()
-        self.newtif=np.transpose(np.transpose(self.tif)/trace)
-        self.newname=self.oldname+' - divided trace'
-        return self.end()
-divide_trace=Divide_trace()
-    
-class Multiply(BaseProcess):
-    """ multiply(value, keepSourceWindow=False)
-    This takes a value and multiplies it to the current window's image.
-    
-    Parameters:
-        | value (float) -- The number you are multiplying by.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        value=QtWidgets.QDoubleSpinBox()
-        value.setRange(-2**64,2**64)
-        self.items.append({'name':'value','string':'Value','object':value})
-        self.items.append({'name':'preview','string':'Preview','object':CheckBox()})
-        super().gui()
-    def __call__(self,value,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        self.newtif=self.tif*value
-        self.newname=self.oldname+' - Multiplied '+str(value)
-        return self.end()
-    def preview(self):
-        value=self.getValue('value')
-        preview=self.getValue('preview')
-        if preview:
-            testimage=np.copy(g.currentWindow.image[g.currentWindow.currentIndex])
-            testimage=testimage*value
-            g.currentWindow.imageview.setImage(testimage,autoLevels=False)
-        else:
-            g.currentWindow.reset()
-multiply=Multiply()
-
-class Power(BaseProcess):
-    """ power(value, keepSourceWindow=False)
-    This raises the current window's image to the power of 'value'.
-    
-    Parameters:
-        | value (int) -- The exponent.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        value=QtWidgets.QDoubleSpinBox()
-        if g.currentWindow is not None:
-            value.setRange(-100,100)
-            value.setValue(1)
-        self.items.append({'name':'value','string':'Value','object':value})
-        self.items.append({'name':'preview','string':'Preview','object':CheckBox()})
-        super().gui()
-    def __call__(self,value,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        self.newtif=self.tif**value
-        self.newname=self.oldname+' - Power of '+str(value)
-        return self.end()
-    def preview(self):
-        value=self.getValue('value')
-        preview=self.getValue('preview')
-        if preview:
-            testimage=np.copy(g.currentWindow.image[g.currentWindow.currentIndex])
-            testimage=testimage**value
-            g.currentWindow.imageview.setImage(testimage,autoLevels=False)
-        else:
-            g.currentWindow.reset()
-power=Power()
-    
-class Ratio(BaseProcess):
-    """ ratio(first_frame,nFrames,ratio_type, keepSourceWindow=False)
-    Takes a set of frames, combines them into a 2D array according to ratio_type, and divides the entire 3D array frame-by-frame by this array.
-    
-    Parameters:
-        | first_frame (int) -- The first frame in the set of frames to be combined
-        | nFrames (int) -- The number of frames to be combined.
-        | ratio_type (str) -- The method used to combine the frames.  Either 'standard deviation' or 'average'.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        nFrames=1
-        if g.currentWindow is not None:
-            nFrames=g.currentWindow.image.shape[0]
-        first_frame=QtWidgets.QSpinBox()
-        first_frame.setMaximum(nFrames)
-        self.items.append({'name':'first_frame','string':'First Frame','object':first_frame})
-        nFrames_spinbox=QtWidgets.QSpinBox()
-        nFrames_spinbox.setMaximum(nFrames)
-        nFrames_spinbox.setMinimum(1)
-        self.items.append({'name':'nFrames','string':'Number of Frames','object':nFrames_spinbox})
-        ratio_type=ComboBox()
-        ratio_type.addItem('average')
-        ratio_type.addItem('standard deviation')
-        self.items.append({'name':'ratio_type','string':'Ratio Type','object':ratio_type})
-        super().gui()
-    def __call__(self,first_frame,nFrames,ratio_type,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.oldwindow.volume is None:
-            A = self.tif
-        else:
-            A = self.oldwindow.volume
-        if ratio_type=='average':
-            baseline=A[first_frame:first_frame+nFrames].mean(0)
-            baseline[baseline == 0] = np.min(np.abs(baseline[baseline != 0])) #This isn't mathematically correct.  I do this to avoid dividing by zero
-        elif ratio_type=='standard deviation':
-            baseline=A[first_frame:first_frame+nFrames].std(0)
-            baseline[baseline == 0] = np.min(np.abs(baseline[baseline != 0]))
-        else:
-            g.alert("'{}' is an unknown ratio_type.  Try 'average' or 'standard deviation'".format(ratio_type))
-            return None
-
-        newA = (A/baseline).astype(g.settings['internal_data_type'])
-        if self.oldwindow.volume is None:
-            self.newtif=newA
-            self.newname=self.oldname+' - Ratioed by '+str(ratio_type)
-            return self.end()
-        else:
-            from plugins.light_sheet_analyzer.light_sheet_analyzer import Volume_Viewer
-            self.newtif = np.squeeze(newA[:, 0, :, :])
-            self.newname = self.oldname + ' - Ratioed by ' + str(ratio_type)
-            w = self.end()
-            w.volume = newA
-            Volume_Viewer(w)
-            return w
-ratio=Ratio()
-
-
-class Absolute_value(BaseProcess):
-    """ absolute_value(keepSourceWindow=False)
-    Takes the absolute value of a set of frames
-    
-    Parameters:
-        | None
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        if super().gui()==False:
-            return False
-    def __call__(self,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        self.newtif=np.abs(self.tif)
-        self.newname=self.oldname+' - Absolute Value'
-        return self.end()
-absolute_value=Absolute_value()
-
-
+# -*- coding: utf-8 -*-
+from ..logger import logger
+logger.debug("Started 'reading process/math_.py'")
+import numpy as np
+from qtpy import QtGui, QtWidgets, QtCore
+from .. import global_vars as g
+from ..utils.BaseProcess import BaseProcess, CheckBox, ComboBox
+from ..window import Window
+
+__all__ = ['subtract','multiply','divide','power','ratio','absolute_value','subtract_trace','divide_trace', 'sqrt']
+
+
+def upgrade_dtype(dtype):
+    if dtype==np.uint8:
+        return np.uint16
+    elif dtype==np.uint16:
+        return np.uint32
+    elif dtype==np.uint32:
+        return np.uint64
+    elif dtype==np.uint64:
+        return np.int8
+    elif dtype==np.int8:
+        return np.int16
+    elif dtype==np.int16:
+        return np.int32
+    elif dtype==np.int32:
+        return np.int64
+    elif dtype==np.float16:
+        return np.float32
+    elif dtype==np.float32:
+        return np.float64
+
+
+class Subtract(BaseProcess):
+    """ subtract(value, keepSourceWindow=False)
+
+    This takes a value and subtracts it from the current window's image.
+    
+    Parameters:
+        value (int): The number you are subtracting.
+    Returns:
+        newWindow
+    """
+    __url__ = ""
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        value=QtWidgets.QDoubleSpinBox()
+        if g.win is not None:
+            maxx = np.max(g.win.image) * 100
+            minn = -1 * maxx # -np.max sometimes returns abnormal large value
+            value.setRange(minn, maxx)
+            value.setValue(np.min(g.win.image))
+        self.items.append({'name':'value','string':'Value','object':value})
+        self.items.append({'name':'preview','string':'Preview','object':CheckBox()})
+        super().gui()
+    def __call__(self,value,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if hasattr(value,'is_integer') and value.is_integer():
+            value = int(value)
+        if np.issubdtype(self.tif.dtype,np.integer):
+            ddtype=np.iinfo(self.tif.dtype)
+            while np.min(self.tif)-value<ddtype.min or np.max(self.tif)-value>ddtype.max: # if we exceed the bounds of the datatype
+                ddtype=np.iinfo(upgrade_dtype(ddtype.dtype))
+            self.newtif=self.tif.astype(ddtype.dtype)-value
+        else:
+            self.newtif=self.tif-value
+        self.newname=self.oldname+' - Subtracted '+str(value)
+        return self.end()
+    def preview(self):
+        value=self.getValue('value')
+        preview=self.getValue('preview')
+        if preview:
+            testimage=np.copy(g.win.image[g.win.currentIndex])
+            testimage=testimage-value
+            g.win.imageview.setImage(testimage,autoLevels=False)
+        else:
+            g.win.reset()
+subtract=Subtract()
+
+class Subtract_trace(BaseProcess):
+    """ subtract_trace(keepSourceWindow=False)
+
+    This takes the most recently plotted trace and subtracts it from each corresponding frame.
+
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def __call__(self,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        trace=g.currentTrace.rois[-1]['roi'].getTrace()
+        nDims=len(self.tif.shape)
+        if nDims !=3:
+            g.alert('Wrong number of dimensions')
+            return self.end()
+        if self.tif.shape[0]!=len(trace):
+            g.alert('Wrong trace length')
+            return self.end()
+        self.newtif=np.transpose(np.transpose(self.tif)-trace)
+        self.newname=self.oldname+' - subtracted trace'
+        return self.end()
+subtract_trace=Subtract_trace()
+
+class Divide_trace(BaseProcess):
+    """ divide_trace(keepSourceWindow=False)
+
+    This takes the most recently plotted trace and divides each pixel in the current Window by its value.
+
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def __call__(self,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        trace=g.currentTrace.rois[-1]['roi'].getTrace()
+        nDims=len(self.tif.shape)
+        if nDims !=3:
+            g.alert('Wrong number of dimensions')
+            return self.end()
+        if self.tif.shape[0]!=len(trace):
+            g.alert('Wrong trace length')
+            return self.end()
+        self.newtif=np.transpose(np.transpose(self.tif)/trace)
+        self.newname=self.oldname+' - divided trace'
+        return self.end()
+divide_trace=Divide_trace()
+    
+class Multiply(BaseProcess):
+    """ multiply(value, keepSourceWindow=False)
+
+    This takes a value and multiplies it to the current window's image.
+    
+    Parameters:
+        value (float): The number you are multiplying by.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        value=QtWidgets.QDoubleSpinBox()
+        value.setRange(-2**64,2**64)
+        self.items.append({'name':'value','string':'Value','object':value})
+        self.items.append({'name':'preview','string':'Preview','object':CheckBox()})
+        super().gui()
+    def __call__(self,value,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        self.newtif = self.tif*value
+        self.newname = self.oldname+' - Multiplied by '+str(value)
+        return self.end()
+    def preview(self):
+        value=self.getValue('value')
+        preview=self.getValue('preview')
+        if preview:
+            testimage=np.copy(g.win.image[g.win.currentIndex])
+            testimage=testimage*value
+            g.win.imageview.setImage(testimage,autoLevels=False)
+        else:
+            g.win.reset()
+multiply=Multiply()
+
+
+class Divide(BaseProcess):
+    """ divide(value, keepSourceWindow=False)
+
+    This takes a value and divides it to the current window's image.
+
+    Parameters:
+        value (float): The number you are dividing by.
+    Returns:
+        newWindow
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        self.gui_reset()
+        value = QtWidgets.QDoubleSpinBox()
+        value.setRange(-2 ** 64, 2 ** 64)
+        self.items.append({'name': 'value', 'string': 'Value', 'object': value})
+        self.items.append({'name': 'preview', 'string': 'Preview', 'object': CheckBox()})
+        super().gui()
+
+    def __call__(self, value, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        self.newtif = self.tif / value
+        self.newname = self.oldname + ' - Divided by ' + str(value)
+        return self.end()
+
+    def preview(self):
+        value = self.getValue('value')
+        preview = self.getValue('preview')
+        if preview:
+            testimage = np.copy(g.win.image[g.win.currentIndex])
+            testimage = testimage / value
+            g.win.imageview.setImage(testimage, autoLevels=False)
+        else:
+            g.win.reset()
+
+
+divide = Divide()
+
+class Power(BaseProcess):
+    """ power(value, keepSourceWindow=False)
+
+    This raises the current window's image to the power of 'value'.
+    
+    Parameters:
+        value (int): The exponent.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        value=QtWidgets.QDoubleSpinBox()
+        if g.win is not None:
+            value.setRange(-100,100)
+            value.setValue(1)
+        self.items.append({'name':'value','string':'Value','object':value})
+        self.items.append({'name':'preview','string':'Preview','object':CheckBox()})
+        super().gui()
+    def __call__(self,value,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        self.newtif=self.tif**value
+        self.newname=self.oldname+' - Power of '+str(value)
+        return self.end()
+    def preview(self):
+        value=self.getValue('value')
+        preview=self.getValue('preview')
+        if preview:
+            testimage=np.copy(g.win.image[g.win.currentIndex])
+            testimage=testimage**value
+            g.win.imageview.setImage(testimage,autoLevels=False)
+        else:
+            g.win.reset()
+power=Power()
+
+class Sqrt(BaseProcess):
+    """ sqrt(value, keepSourceWindow=False)
+
+    This takes the square root of the current window's image.
+    In this function, the square root of a negative number is set to 0.
+    
+    Parameters:
+        value (int): The exponent.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        self.items.append({'name':'preview', 'string':'Preview', 'object':CheckBox()})
+        super().gui()
+    def __call__(self, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        A = np.copy(self.tif)
+        A[A<0] = 0
+        self.newtif = np.sqrt(A)
+        self.newname = self.oldname+' - Sqrt '
+        return self.end()
+    def preview(self):
+        preview = self.getValue('preview')
+        if preview:
+            A = np.copy(g.win.image[g.win.currentIndex])
+            A[A<0] = 0
+            A = np.sqrt(A)
+            g.win.imageview.setImage(A, autoLevels=False)
+        else:
+            g.win.reset()
+sqrt = Sqrt()
+    
+class Ratio(BaseProcess):
+    """ ratio(first_frame, nFrames, ratio_type, black_level, keepSourceWindow=False)
+
+    Takes a set of frames, combines them into a 2D array according to ratio_type, and divides the entire 3D array frame-by-frame by this array.
+    
+    Parameters:
+        first_frame (int): The first frame in the set of frames to be combined
+        nFrames (int): The number of frames to be combined.
+        ratio_type (str): The method used to combine the frames.  Either 'standard deviation' or 'average'.
+        black_level (float): The value to subtract from the entire movie prior to the ratio operation.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        self.gui_reset()
+        nFrames = 1
+        if g.win is not None:
+            nFrames = g.win.image.shape[0]
+        first_frame = QtWidgets.QSpinBox()
+        first_frame.setMaximum(nFrames)
+        self.items.append({'name': 'first_frame', 'string': 'First Frame', 'object': first_frame})
+        nFrames_spinbox = QtWidgets.QSpinBox()
+        nFrames_spinbox.setMaximum(nFrames)
+        nFrames_spinbox.setMinimum(1)
+        self.items.append({'name': 'nFrames', 'string': 'Number of Frames', 'object': nFrames_spinbox})
+        ratio_type = ComboBox()
+        ratio_type.addItem('average')
+        ratio_type.addItem('standard deviation')
+        self.items.append({'name': 'ratio_type', 'string': 'Ratio Type', 'object': ratio_type})
+        black_level = QtWidgets.QDoubleSpinBox()
+        black_level.setMinimum(0)
+        black_level.setMaximum(1000)
+        self.items.append({'name': 'black_level', 'string': 'Black Level', 'object': black_level})
+        super().gui()
+
+    def __call__(self, first_frame, nFrames, ratio_type, black_level=0, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.oldwindow.volume is None:
+            A = self.tif - black_level
+        else:
+            A = self.oldwindow.volume - black_level
+        if ratio_type == 'average':
+            baseline = A[first_frame:first_frame+nFrames].mean(0)
+            baseline[baseline == 0] = np.min(np.abs(baseline[baseline != 0])) # This isn't mathematically correct.  I do this to avoid dividing by zero
+        elif ratio_type == 'standard deviation':
+            baseline = A[first_frame:first_frame+nFrames].std(0)
+            baseline[baseline == 0] = np.min(np.abs(baseline[baseline != 0]))
+        else:
+            g.alert("'{}' is an unknown ratio_type.  Try 'average' or 'standard deviation'".format(ratio_type))
+            return None
+
+        newA = (A/baseline).astype(g.settings['internal_data_type'])
+        if self.oldwindow.volume is None:
+            self.newtif=newA
+            self.newname=self.oldname+' - Ratioed by '+str(ratio_type)
+            return self.end()
+        else:
+            from plugins.light_sheet_analyzer.light_sheet_analyzer import Volume_Viewer
+            self.newtif = np.squeeze(newA[:, 0, :, :])
+            self.newname = self.oldname + ' - Ratioed by ' + str(ratio_type)
+            w = self.end()
+            w.volume = newA
+            Volume_Viewer(w)
+            return w
+ratio=Ratio()
+
+
+class Absolute_value(BaseProcess):
+    """ absolute_value(keepSourceWindow=False)
+
+    Takes the absolute value of a set of frames
+
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        if super().gui()==False:
+            return False
+    def __call__(self,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        self.newtif=np.abs(self.tif)
+        self.newname=self.oldname+' - Absolute Value'
+        return self.end()
+absolute_value=Absolute_value()
+
+
+logger.debug("Completed 'reading process/math_.py'")
```

### Comparing `flika-0.2.9/flika/process/measure.py` & `flika-0.3.0/flika/process/measure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,199 +1,204 @@
-# -*- coding: utf-8 -*-
-import os
-import numpy as np
-import pyqtgraph as pg
-from qtpy import QtWidgets, QtCore, QtGui
-from .. import global_vars as g
-from .BaseProcess import BaseProcess
-from ..utils.misc import save_file_gui
-
-__all__ = ['measure']
-
-
-np.set_printoptions(suppress=True)
-np.set_printoptions(precision=3)
-            
-class Measure(BaseProcess):
-    """
-    Click in the graph to select a point.
-    Shift-Click in the graph to select the nearest data point
-    
-    """
-    def __init__(self):
-        self.ON=False
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        self.currentPoint = 0
-        active_point = QtWidgets.QLineEdit() #active_point.setEnabled(False)
-        second_point = QtWidgets.QLineEdit() #second_point.setEnabled(False)
-        difference = QtWidgets.QLineEdit() #difference.setEnabled(False)
-        slope = QtWidgets.QLineEdit() #slope.setEnabled(False)
-        log = QtWidgets.QPushButton('Log Data')
-        log.pressed.connect(self.log)
-        newcol=QtWidgets.QPushButton('New Column')
-        newcol.pressed.connect(self.newcol)
-        self.table = pg.TableWidget()
-        self.items.append({'name':'active_point','string':'Active Point: ','object':active_point})
-        self.items.append({'name':'second_point','string':'Second Point: ','object':second_point})
-        self.items.append({'name':'difference','string':'Difference: ','object':difference})
-        self.items.append({'name':'slope','string':'Slope: ','object':slope})
-        self.items.append({'name':'log','string':'','object':log})
-        self.items.append({'name':'newcol','string':'','object':newcol})
-        super().gui()
-        self.fig = None
-        self.overwrite = False
-        self.ui.accepted.disconnect()
-        self.ui.closeSignal.connect(self.close)
-        self.ui.rejected.connect(self.close)
-        self.ui.accepted.connect(self.close)
-        self.ui.accepted.connect(self.export_gui)
-        self.data = [[]]
-        self.ON = True
-    def log(self):
-        point=[self.firstPoint[0],self.firstPoint[1],self.secondPoint[0],self.secondPoint[1],self.difference[0],self.difference[1],self.slope]
-        self.data[len(self.data)-1].append(point)
-    def newcol(self):
-        self.data.append([])
-
-    def clear(self):
-        self.currentPoint = 0
-        try:
-            self.viewbox.removeItem(self.pathitem)
-        except:
-            pass
-
-    def pointclicked(self,evt, window=None, overwrite=False):
-        if evt.button() != 1:
-            return
-        if self.ON is False:
-            return
-        pos=evt.pos()
-        if self.overwrite:
-            self.overwrite = overwrite
-            return
-        elif window != None:
-            if window != self.fig:
-                self.clear()
-                self.fig = window
-                self.viewbox = self.fig.imageview.view
-                self.pathitem=QtWidgets.QGraphicsPathItem(self.viewbox)
-                self.pathitem.setPen(QtGui.QPen(QtCore.Qt.red))
-                self.viewbox.addItem(self.pathitem,ignoreBounds=True)
-            mousePoint = self.fig.imageview.getImageItem().mapFromScene(pos)
-            pos = np.array([mousePoint.y(),mousePoint.x()])
-        else:
-            if self.fig is not g.currentTrace: #if we created a new tracefig
-                self.clear()
-                self.fig=g.currentTrace
-                self.viewbox=self.fig.vb
-                if not g.currentTrace.p1.plotItem.sceneBoundingRect().contains(pos):
-                    return
-                self.pathitem=QtWidgets.QGraphicsPathItem(self.viewbox)
-                self.pathitem.setPen(QtGui.QPen(QtCore.Qt.red))
-                self.viewbox.addItem(self.pathitem,ignoreBounds=True)
-            mousePoint = self.viewbox.mapSceneToView(pos) if not overwrite else pos
-            pos = np.array([mousePoint.x(),mousePoint.y()])
-
-        self.overwrite = overwrite
-        self.update(pos)
-
-    def update(self, point):
-        
-        modifiers = QtWidgets.QApplication.keyboardModifiers()
-        if modifiers == QtCore.Qt.ShiftModifier:
-            point=self.getNearestPoint(point)
-        if self.currentPoint==0:
-            self.currentPoint=1
-            self.firstPoint=point
-            self.ui.items[0]['object'].setText(str(point))
-            self.ui.items[1]['object'].setText('')
-            self.ui.items[2]['object'].setText('')
-            self.ui.items[3]['object'].setText('')
-            self.secondPoint=None
-            self.draw([self.firstPoint])
-        else:
-            self.currentPoint=0
-            self.secondPoint=point
-            self.ui.items[1]['object'].setText(str(point))
-            self.difference=self.secondPoint-self.firstPoint
-            self.ui.items[2]['object'].setText(str(self.difference))
-            if self.difference[0]==0:
-                self.slope=np.inf
-            else:
-                self.slope=self.difference[1]/self.difference[0]
-            self.ui.items[3]['object'].setText(str(self.slope))
-            self.draw([self.firstPoint,self.secondPoint])
-                    
-    def draw(self,points):
-        if type(self.fig) != type(g.currentTrace):
-            points = [p[::-1] for p in points]
-        path=QtGui.QPainterPath(QtCore.QPointF(*points[0]))
-        for i in np.arange(1,len(points)):
-            path.lineTo(QtCore.QPointF(*points[i]))
-        self.pathitem.setPath(path)
-        
-    def close(self):
-        if hasattr(self, "pathitem") and self.pathitem.parentWidget() != None:
-            self.pathitem.parentWidget().removeItem(self.pathitem) 
-        self.ON=False
-    def getNearestPoint(self,point):
-        if hasattr(self.fig, 'imageview'):
-            return point
-        roi=g.currentTrace.rois[0]
-        d=roi['p2trace'].getData()
-        index=np.abs(d[0]-point[0]).argmin()
-        x=d[0][index]
-        ys=[]
-        for roi in g.currentTrace.rois:
-            d=roi['p2trace'].getData()
-            ys.append(d[1][index])
-        roi_idx=np.argmin(abs(ys - point[1]))
-        y=ys[roi_idx]
-        return np.array([x,y])
-    
-    def export_gui(self):
-        filename = g.settings['filename']
-        directory = os.path.dirname(filename)
-        if filename is not None:
-            filename = getSaveFileName(g.m, 'Save Measurements', directory, '*.txt')
-        else:
-            filename = getSaveFileName(g.m, 'Save Measurements', '*.txt')
-        filename = str(filename)
-        if filename == '':
-            return False
-        else:
-            self.export(filename)
-            
-    def export(self,filename):
-        ''' This function saves out all the traces in the tracefig to a file specified by the argument 'filename'.
-        The output file is a tab seperated ascii file where each column is a trace.  
-        Traces are saved in the order they were added to the plot.
-        
-        '''
-        g.m.statusBar().showMessage('Saving {}'.format(os.path.basename(filename)))
-        d=self.data
-        output=''
-        maxj=np.max([len(j) for j in d])
-        header=['x1' ,'y1','x2','y2','x difference','y difference' , 'slope']
-        for i in np.arange(len(d)):
-            for k in np.arange(7):
-                output+=header[k]+'\t'
-            output+='\t'
-        output+='\n'
-        for j in np.arange(maxj): #this loops through each row of data
-            for i in np.arange(len(d)): #this loops through each mega-column, each of which is composed of 7 mini-columns.
-                for k in np.arange(7): #this loops through each of the seven values
-                    try:
-                        output+=str(d[i][j][k])+'\t'
-                    except IndexError:
-                        output+='\t'
-                output+='\t'
-            output+='\n'
-        f = open(filename, 'w')
-        f.write(output)
-        f.close()
-        g.m.statusBar().showMessage('Successfully saved {}'.format(os.path.basename(filename)))
-    
-measure = Measure()
-
+# -*- coding: utf-8 -*-
+from ..logger import logger
+logger.debug("Started 'reading process/measure.py'")
+import os
+import numpy as np
+import pyqtgraph as pg
+from qtpy import QtWidgets, QtCore, QtGui
+from .. import global_vars as g
+from ..utils.BaseProcess import BaseProcess
+from ..utils.misc import save_file_gui
+
+from ..roi import ROI_Base
+__all__ = ['measure']
+
+
+np.set_printoptions(suppress=True)
+np.set_printoptions(precision=3)
+            
+class Measure(BaseProcess):
+    """Measure(BaseProcess)
+
+    Click in the graph to select a point.
+    Shift-Click in the graph to select the nearest data point
+    
+    """
+    def __init__(self):
+        self.ON=False
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        self.currentPoint = 0
+        active_point = QtWidgets.QLineEdit() #active_point.setEnabled(False)
+        second_point = QtWidgets.QLineEdit() #second_point.setEnabled(False)
+        difference = QtWidgets.QLineEdit() #difference.setEnabled(False)
+        slope = QtWidgets.QLineEdit() #slope.setEnabled(False)
+        log = QtWidgets.QPushButton('Log Data')
+        log.pressed.connect(self.log)
+        newcol=QtWidgets.QPushButton('New Column')
+        newcol.pressed.connect(self.newcol)
+        self.table = pg.TableWidget()
+        self.items.append({'name':'active_point','string':'Active Point: ','object':active_point})
+        self.items.append({'name':'second_point','string':'Second Point: ','object':second_point})
+        self.items.append({'name':'difference','string':'Difference: ','object':difference})
+        self.items.append({'name':'slope','string':'Slope: ','object':slope})
+        self.items.append({'name':'log','string':'','object':log})
+        self.items.append({'name':'newcol','string':'','object':newcol})
+        super().gui()
+        self.fig = None
+        self.ui.accepted.disconnect()
+        self.ui.closeSignal.connect(self.close)
+        self.ui.rejected.connect(self.close)
+        self.ui.accepted.connect(self.close)
+        self.ui.accepted.connect(self.export_gui)
+        self.data = [[]]
+        self.ON = True
+    def log(self):
+        point=[self.firstPoint[0],self.firstPoint[1],self.secondPoint[0],self.secondPoint[1],self.difference[0],self.difference[1],self.slope]
+        self.data[len(self.data)-1].append(point)
+    def newcol(self):
+        self.data.append([])
+
+    def clear(self):
+        self.currentPoint = 0
+        try:
+            self.viewbox.removeItem(self.pathitem)
+        except:
+            pass
+
+    def pointclicked(self,evt, window=None):
+        if evt.button() != 1:
+            return
+        if self.ON is False:
+            return
+        pos = evt.pos()
+        if isinstance(evt.currentItem, (ROI_Base, pg.ROI)):
+            pos = evt.currentItem.mapToScene(pos)
+
+        if window != None:
+            if window != self.fig:
+                self.clear()
+                self.fig = window
+                self.viewbox = self.fig.imageview.view
+                self.pathitem=QtWidgets.QGraphicsPathItem(self.viewbox)
+                self.pathitem.setPen(QtGui.QPen(QtCore.Qt.red, 0))
+                self.viewbox.addItem(self.pathitem,ignoreBounds=True)
+            mousePoint = self.fig.imageview.getImageItem().mapFromScene(pos)
+            pos = np.array([mousePoint.y(),mousePoint.x()])
+        else:
+            if self.fig is not g.currentTrace: #if we created a new tracefig
+                self.clear()
+                self.fig=g.currentTrace
+                self.viewbox=self.fig.vb
+                if not g.currentTrace.p1.plotItem.sceneBoundingRect().contains(pos):
+                    return
+                self.pathitem=QtWidgets.QGraphicsPathItem(self.viewbox)
+                self.pathitem.setPen(QtGui.QPen(QtCore.Qt.red, 0))
+                self.viewbox.addItem(self.pathitem,ignoreBounds=True)
+            mousePoint = self.viewbox.mapSceneToView(pos)
+            pos = np.array([mousePoint.x(),mousePoint.y()])
+        
+        self.update(pos)
+
+    def update(self, point):
+        
+        modifiers = QtWidgets.QApplication.keyboardModifiers()
+        if modifiers == QtCore.Qt.ShiftModifier:
+            point=self.getNearestPoint(point)
+        if self.currentPoint==0:
+            self.currentPoint=1
+            self.firstPoint=point
+            self.ui.items[0]['object'].setText(str(point))
+            self.ui.items[1]['object'].setText('')
+            self.ui.items[2]['object'].setText('')
+            self.ui.items[3]['object'].setText('')
+            self.secondPoint=None
+            self.draw([self.firstPoint])
+        else:
+            self.currentPoint=0
+            self.secondPoint=point
+            self.ui.items[1]['object'].setText(str(point))
+            self.difference=self.secondPoint-self.firstPoint
+            self.ui.items[2]['object'].setText(str(self.difference))
+            if self.difference[0]==0:
+                self.slope=np.inf
+            else:
+                self.slope=self.difference[1]/self.difference[0]
+            self.ui.items[3]['object'].setText(str(self.slope))
+            self.draw([self.firstPoint,self.secondPoint])
+                    
+    def draw(self,points):
+        if type(self.fig) != type(g.currentTrace):
+            points = [p[::-1] for p in points]
+        path=QtGui.QPainterPath(QtCore.QPointF(*points[0]))
+        for i in np.arange(1,len(points)):
+            path.lineTo(QtCore.QPointF(*points[i]))
+        self.pathitem.setPath(path)
+        
+    def close(self):
+        if hasattr(self, "pathitem") and self.pathitem.parentWidget() != None:
+            self.pathitem.parentWidget().removeItem(self.pathitem) 
+        self.ON=False
+    def getNearestPoint(self,point):
+        if hasattr(self.fig, 'imageview'):
+            return point
+        roi=g.currentTrace.rois[0]
+        d=roi['p2trace'].getData()
+        index=np.abs(d[0]-point[0]).argmin()
+        x=d[0][index]
+        ys=[]
+        for roi in g.currentTrace.rois:
+            d=roi['p2trace'].getData()
+            ys.append(d[1][index])
+        roi_idx=np.argmin(abs(ys - point[1]))
+        y=ys[roi_idx]
+        return np.array([x,y])
+    
+    def export_gui(self):
+        filename = g.settings['filename']
+        directory = os.path.dirname(filename)
+        if filename is not None:
+            filename = save_file_gui('Save Measurements', directory, '*.txt')
+        else:
+            filename = save_file_gui('Save Measurements', None, '*.txt')
+        filename = str(filename)
+        if filename == '':
+            return False
+        else:
+            self.export(filename)
+            
+    def export(self,filename):
+        ''' This function saves out all the traces in the tracefig to a file specified by the argument 'filename'.
+        The output file is a tab seperated ascii file where each column is a trace.  
+        Traces are saved in the order they were added to the plot.
+
+        Parameters:
+            filename (str): name of file to save
+        
+        '''
+        g.m.statusBar().showMessage('Saving {}'.format(os.path.basename(filename)))
+        d=self.data
+        output=''
+        maxj=np.max([len(j) for j in d])
+        header=['x1' ,'y1','x2','y2','x difference','y difference' , 'slope']
+        for i in np.arange(len(d)):
+            for k in np.arange(7):
+                output+=header[k]+'\t'
+            output+='\t'
+        output+='\n'
+        for j in np.arange(maxj): #this loops through each row of data
+            for i in np.arange(len(d)): #this loops through each mega-column, each of which is composed of 7 mini-columns.
+                for k in np.arange(7): #this loops through each of the seven values
+                    try:
+                        output+=str(d[i][j][k])+'\t'
+                    except IndexError:
+                        output+='\t'
+                output+='\t'
+            output+='\n'
+        f = open(filename, 'w')
+        f.write(output)
+        f.close()
+        g.m.statusBar().showMessage('Successfully saved {}'.format(os.path.basename(filename)))
+    
+measure = Measure()
+logger.debug("Completed 'reading process/measure.py'")
```

### Comparing `flika-0.2.9/flika/process/overlay.py` & `flika-0.3.0/flika/process/overlay.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,292 +1,296 @@
-# -*- coding: utf-8 -*-
-import numpy as np
-import pyqtgraph as pg
-from qtpy import QtWidgets, QtCore, QtGui
-from .. import global_vars as g
-from .BaseProcess import BaseProcess, SliderLabel, WindowSelector,  MissingWindowError, CheckBox, ComboBox
-
-__all__ = ['time_stamp','background','scale_bar']
-     
-
-
-class Time_Stamp(BaseProcess):
-    """time_stamp(framerate,show=True)
-    Adds a time stamp to a movie
-    
-    Parameters:
-        | framerate (float) -- The number of frames per second
-        | show (bool) -- Turns on or off the time stamp
-    Returns:
-        None
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        framerate=QtWidgets.QDoubleSpinBox()
-        if hasattr(g.currentWindow,'framerate'):
-            framerate.setValue(g.currentWindow.framerate)
-        elif 'framerate' in g.settings.d.keys():
-            framerate.setValue(g.settings['framerate'])
-        framerate.setRange(0,1000000)
-        framerate.setDecimals(10)
-        show=QtWidgets.QCheckBox(); show.setChecked(True)
-        self.items.append({'name':'framerate','string':'Frame Rate (Hz)','object':framerate})
-        self.items.append({'name':'show','string':'Show','object':show})
-        super().gui()
-    def __call__(self,framerate,show=True,keepSourceWindow=None):
-        w=g.currentWindow
-        if show:
-            w.framerate=framerate
-            g.settings['framerate']=framerate
-            if hasattr(w,'timeStampLabel') and w.timeStampLabel is not None:
-                return
-            w.timeStampLabel= pg.TextItem(html="<span style='font-size: 12pt;color:white;background-color:None;'>0 ms</span>")
-            w.imageview.view.addItem(w.timeStampLabel)
-            w.sigTimeChanged.connect(w.updateTimeStampLabel)
-        else:
-            if hasattr(w,'timeStampLabel') and w.timeStampLabel is not None:
-                w.imageview.view.removeItem(w.timeStampLabel)
-                w.timeStampLabel=None
-                w.sigTimeChanged.disconnect(w.updateTimeStampLabel)
-        return None
-    def preview(self):
-        framerate=self.getValue('framerate')
-        show=self.getValue('show')
-        self.__call__(framerate,show)
-
-     
-time_stamp=Time_Stamp()
-
-
-class ShowCheckbox(CheckBox):
-
-    def __init__(self, opacity_slider, parent=None):
-        super().__init__(parent)
-        self.stateChanged.connect(self.changed)
-        self.opacity_slider = opacity_slider
-
-    def changed(self, state):
-        if state == 0:  # unchecked
-            self.opacity_slider.setEnabled(True)
-        if state == 2:  # checked
-            self.opacity_slider.setEnabled(False)
-
-
-class Background(BaseProcess):
-    """ background(background_window, data_window)
-    Overlays the background_window onto the data_window
-    
-    Parameters:
-        | background_window (Window)
-        | data_window (Window)
-    Returns:
-        None
-    """
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        background_window=WindowSelector()
-        data_window=WindowSelector()
-        opacity = SliderLabel(3)
-        opacity.setRange(0,1)
-        opacity.setValue(.5)
-        show = ShowCheckbox(opacity)
-        show.setChecked(True)
-        self.items.append({'name':'background_window','string':'Background window','object':background_window})
-        self.items.append({'name':'data_window','string':'Data window','object':data_window})
-        self.items.append({'name':'opacity','string':'Opacity','object':opacity})
-        self.items.append({'name':'show','string':'Show','object':show})
-        super().gui()
-    def __call__(self, background_window, data_window, opacity,show,keepSourceWindow=False):
-        if background_window is None or data_window is None:
-            return
-        w=data_window
-        if show:
-            if hasattr(w, 'bgItem') and w.bgItem is not None:
-                w.bgItem.hist_luttt.hide()
-                w.imageview.ui.gridLayout.removeWidget(w.bgItem.hist_luttt)
-                w.imageview.view.removeItem(w.bgItem)
-            bgItem = pg.ImageItem(background_window.imageview.imageItem.image)
-            bgItem.setOpacity(opacity)
-            w.imageview.view.addItem(bgItem)
-            bgItem.hist_luttt = pg.HistogramLUTWidget()
-            bgItem.hist_luttt.setMinimumWidth(110)
-            bgItem.hist_luttt.setImageItem(bgItem)
-            w.imageview.ui.gridLayout.addWidget(bgItem.hist_luttt, 0, 4, 1, 4)
-            w.bgItem = bgItem
-        else:
-            if hasattr(w, 'bgItem') and w.bgItem is not None:
-                w.bgItem.hist_luttt.hide()
-                w.imageview.ui.gridLayout.removeWidget(w.bgItem.hist_luttt)
-                w.imageview.view.removeItem(w.bgItem)
-                w.bgItem.hist_luttt = None
-                w.bgItem = None
-            return None
-    def preview(self):
-        background_window=self.getValue('background_window')
-        data_window=self.getValue('data_window')
-        opacity=self.getValue('opacity')
-        show=self.getValue('show')
-        self.__call__(background_window,data_window,opacity,show)
-        
-background=Background()
-
-class Scale_Bar(BaseProcess):
-    ''' scale_bar(width_microns, width_pixels, font_size, color, background, location, show=True)
-
-    Parameters:
-        | width_microns (float)
-        | width_pixels (float)
-        | font_size (int)
-        | color ['Black','White'] (string)
-        | background  ['Black','White', 'None'] (string)
-        | location ['Lower Right','Lower Left','Top Right','Top Left'] (string)
-        | show (bool)
-    '''
-    
-    def __init__(self):
-        super().__init__()
-    def gui(self):
-        self.gui_reset()
-        w=g.currentWindow
-        width_microns=QtWidgets.QDoubleSpinBox()
-        
-        width_pixels=QtWidgets.QSpinBox()
-        width_pixels.setRange(.001,1000000)
-        width_pixels.setRange(1,w.mx)
-        
-        font_size=QtWidgets.QSpinBox()
-        
-        color=ComboBox()
-        color.addItem("White")
-        color.addItem("Black")
-        background=ComboBox()
-        background.addItem('None')
-        background.addItem('Black')
-        background.addItem('White')
-        location=ComboBox()
-        location.addItem('Lower Right')
-        location.addItem('Lower Left')
-        location.addItem('Top Right')
-        location.addItem('Top Left')
-        show=CheckBox()
-        if hasattr(w,'scaleBarLabel') and w.scaleBarLabel is not None: #if the scaleBarLabel already exists
-            props=w.scaleBarLabel.flika_properties
-            width_microns.setValue(props['width_microns'])
-            width_pixels.setValue(props['width_pixels'])
-            font_size.setValue(props['font_size'])
-            color.setCurrentIndex(color.findText(props['color']))
-            background.setCurrentIndex(background.findText(props['background']))
-            location.setCurrentIndex(location.findText(props['location']))
-        else:
-            font_size.setValue(12)
-            width_pixels.setValue(int(w.mx/8))
-            width_microns.setValue(1)
-            
-        show.setChecked(True) 
-        self.items.append({'name':'width_microns','string':'Width of bar in microns','object':width_microns})
-        self.items.append({'name':'width_pixels','string':'Width of bar in pixels','object':width_pixels})
-        self.items.append({'name':'font_size','string':'Font size','object':font_size})
-        self.items.append({'name':'color','string':'Color','object':color})
-        self.items.append({'name':'background','string':'Background','object':background})
-        self.items.append({'name':'location','string':'Location','object':location})
-        self.items.append({'name':'show','string':'Show','object':show})
-        
-        super().gui()
-        self.preview()
-    def __call__(self,width_microns, width_pixels, font_size, color, background,location,show=True,keepSourceWindow=None):
-        w=g.currentWindow
-        if show:
-            if hasattr(w,'scaleBarLabel') and w.scaleBarLabel is not None:
-                w.imageview.view.removeItem(w.scaleBarLabel.bar)
-                w.imageview.view.removeItem(w.scaleBarLabel)
-                w.imageview.view.sigResized.disconnect(self.updateBar)
-            if location=='Top Left':
-                anchor=(0,0)
-                pos=[0,0]
-            elif location=='Top Right':
-                anchor=(0,0)
-                pos=[w.mx,0]
-            elif location=='Lower Right':
-                anchor=(0,0)
-                pos=[w.mx,w.my]
-            elif location=='Lower Left':
-                anchor=(0,0)
-                pos=[0,w.my]
-            w.scaleBarLabel= pg.TextItem(anchor=anchor, html="<span style='font-size: {}pt;color:{};background-color:{};'>{} μm</span>".format(font_size, color, background,width_microns))
-            w.scaleBarLabel.setPos(pos[0],pos[1])
-            w.scaleBarLabel.flika_properties={item['name']:item['value'] for item in self.items}
-            w.imageview.view.addItem(w.scaleBarLabel)
-            if color=='White':
-                color255=[255,255,255,255]
-            elif color=='Black':
-                color255=[0,0,0,255]
-            textRect=w.scaleBarLabel.boundingRect()
-            
-            if location=='Top Left':
-                barPoint=QtCore.QPoint(0, textRect.height())
-            elif location=='Top Right':
-                barPoint=QtCore.QPoint(-width_pixels, textRect.height())
-            elif location=='Lower Right':
-                barPoint=QtCore.QPoint(-width_pixels, -textRect.height())
-            elif location=='Lower Left':
-                barPoint=QtCore.QPoint(0, -textRect.height())
-                
-            bar = QtWidgets.QGraphicsRectItem(QtCore.QRectF(barPoint, QtCore.QSizeF(width_pixels,int(font_size/3))))
-            bar.setPen(pg.mkPen(color255)); bar.setBrush(pg.mkBrush(color255))
-            w.imageview.view.addItem(bar)
-            #bar.setParentItem(w.scaleBarLabel)
-            w.scaleBarLabel.bar=bar
-            w.imageview.view.sigResized.connect(self.updateBar)
-            self.updateBar()
-            
-        else:
-            if hasattr(w,'scaleBarLabel') and w.scaleBarLabel is not None:
-                w.imageview.view.removeItem(w.scaleBarLabel.bar)
-                w.imageview.view.removeItem(w.scaleBarLabel)
-                w.scaleBarLabel=None
-                w.imageview.view.sigResized.disconnect(self.updateBar)
-        return None
-        
-    def updateBar(self):
-        w=g.currentWindow
-        width_pixels=self.getValue('width_pixels')
-        location=self.getValue('location')
-        view = w.imageview.view
-        textRect=w.scaleBarLabel.boundingRect()
-        textWidth=textRect.width()*view.viewPixelSize()[0]
-        textHeight=textRect.height()*view.viewPixelSize()[1]
-        
-        if location=='Top Left':
-            barPoint=QtCore.QPoint(0, 1.3*textHeight)
-            w.scaleBarLabel.setPos(QtCore.QPointF(width_pixels/2-textWidth/2,0))
-        elif location=='Top Right':
-            barPoint=QtCore.QPoint(w.mx-width_pixels, 1.3*textHeight)
-            w.scaleBarLabel.setPos(QtCore.QPointF(w.mx-width_pixels/2-textWidth/2,0))
-        elif location=='Lower Right':
-            barPoint=QtCore.QPoint(w.mx-width_pixels, w.my-1.3*textHeight)
-            w.scaleBarLabel.setPos(QtCore.QPointF(w.mx-width_pixels/2-textWidth/2,w.my-textHeight))
-        elif location=='Lower Left':
-            barPoint=QtCore.QPoint(0, w.my-1.3*textHeight)
-            w.scaleBarLabel.setPos(QtCore.QPointF(QtCore.QPointF(width_pixels/2-textWidth/2,w.my-textHeight)))
-        w.scaleBarLabel.bar.setRect(QtCore.QRectF(barPoint, QtCore.QSizeF(width_pixels,textHeight/4)))
-        
-    def preview(self):
-        width_microns=self.getValue('width_microns')
-        width_pixels=self.getValue('width_pixels')
-        font_size=self.getValue('font_size')
-        color=self.getValue('color')
-        background=self.getValue('background')
-        location=self.getValue('location')
-        show=self.getValue('show')
-        self.__call__(width_microns, width_pixels, font_size, color, background, location, show)
-scale_bar=Scale_Bar()
-
-
-
-
-
-
-
+# -*- coding: utf-8 -*-
+from ..logger import logger
+logger.debug("Started 'reading process/overlay.py'")
+import numpy as np
+import pyqtgraph as pg
+from qtpy import QtWidgets, QtCore, QtGui
+from .. import global_vars as g
+from ..utils.BaseProcess import BaseProcess, SliderLabel, WindowSelector,  MissingWindowError, CheckBox, ComboBox
+
+__all__ = ['time_stamp','background','scale_bar']
+     
+
+
+class Time_Stamp(BaseProcess):
+    """time_stamp(framerate,show=True)
+
+    Adds a time stamp to a movie
+    
+    Parameters:
+        framerate (float): The number of frames per second
+        show (bool): Turns on or off the time stamp
+    Returns:
+        None
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        framerate=QtWidgets.QDoubleSpinBox()
+        if hasattr(g.win,'framerate'):
+            framerate.setValue(g.win.framerate)
+        elif 'framerate' in g.settings.d.keys():
+            framerate.setValue(g.settings['framerate'])
+        framerate.setRange(0,1000000)
+        framerate.setDecimals(10)
+        show = CheckBox(); show.setChecked(True)
+        self.items.append({'name':'framerate','string':'Frame Rate (Hz)','object':framerate})
+        self.items.append({'name':'show','string':'Show','object':show})
+        super().gui()
+    def __call__(self,framerate,show=True,keepSourceWindow=None):
+        w=g.win
+        if show:
+            w.framerate=framerate
+            g.settings['framerate']=framerate
+            if hasattr(w,'timeStampLabel') and w.timeStampLabel is not None:
+                return
+            w.timeStampLabel= pg.TextItem(html="<span style='font-size: 12pt;color:white;background-color:None;'>0 ms</span>")
+            w.imageview.view.addItem(w.timeStampLabel)
+            w.sigTimeChanged.connect(w.updateTimeStampLabel)
+        else:
+            if hasattr(w,'timeStampLabel') and w.timeStampLabel is not None:
+                w.imageview.view.removeItem(w.timeStampLabel)
+                w.timeStampLabel=None
+                w.sigTimeChanged.disconnect(w.updateTimeStampLabel)
+        return None
+    def preview(self):
+        framerate=self.getValue('framerate')
+        show=self.getValue('show')
+        self.__call__(framerate,show)
+
+     
+time_stamp=Time_Stamp()
+
+
+class ShowCheckbox(CheckBox):
+
+    def __init__(self, opacity_slider, parent=None):
+        super().__init__(parent)
+        self.stateChanged.connect(self.changed)
+        self.opacity_slider = opacity_slider
+
+    def changed(self, state):
+        if state == 0:  # unchecked
+            self.opacity_slider.setEnabled(True)
+        if state == 2:  # checked
+            self.opacity_slider.setEnabled(False)
+
+
+class Background(BaseProcess):
+    """ background(background_window, data_window)
+
+    Overlays the background_window onto the data_window
+    
+    Parameters:
+        background_window (Window)
+        data_window (Window)
+    Returns:
+        None
+    """
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        background_window=WindowSelector()
+        data_window=WindowSelector()
+        opacity = SliderLabel(3)
+        opacity.setRange(0,1)
+        opacity.setValue(.5)
+        show = ShowCheckbox(opacity)
+        show.setChecked(True)
+        self.items.append({'name':'background_window','string':'Background window','object':background_window})
+        self.items.append({'name':'data_window','string':'Data window','object':data_window})
+        self.items.append({'name':'opacity','string':'Opacity','object':opacity})
+        self.items.append({'name':'show','string':'Show','object':show})
+        super().gui()
+    def __call__(self, background_window, data_window, opacity,show,keepSourceWindow=False):
+        if background_window is None or data_window is None:
+            return
+        w=data_window
+        if show:
+            if hasattr(w, 'bgItem') and w.bgItem is not None:
+                w.bgItem.hist_luttt.hide()
+                w.imageview.ui.gridLayout.removeWidget(w.bgItem.hist_luttt)
+                w.imageview.view.removeItem(w.bgItem)
+            bgItem = pg.ImageItem(background_window.imageview.imageItem.image)
+            bgItem.setOpacity(opacity)
+            w.imageview.view.addItem(bgItem)
+            bgItem.hist_luttt = pg.HistogramLUTWidget()
+            bgItem.hist_luttt.setMinimumWidth(110)
+            bgItem.hist_luttt.setImageItem(bgItem)
+            w.imageview.ui.gridLayout.addWidget(bgItem.hist_luttt, 0, 4, 1, 4)
+            w.bgItem = bgItem
+        else:
+            if hasattr(w, 'bgItem') and w.bgItem is not None:
+                w.bgItem.hist_luttt.hide()
+                w.imageview.ui.gridLayout.removeWidget(w.bgItem.hist_luttt)
+                w.imageview.view.removeItem(w.bgItem)
+                w.bgItem.hist_luttt = None
+                w.bgItem = None
+            return None
+    def preview(self):
+        background_window=self.getValue('background_window')
+        data_window=self.getValue('data_window')
+        opacity=self.getValue('opacity')
+        show=self.getValue('show')
+        self.__call__(background_window,data_window,opacity,show)
+        
+background=Background()
+
+class Scale_Bar(BaseProcess):
+    ''' scale_bar(width_microns, width_pixels, font_size, color, background, location, show=True)
+
+    Parameters:
+        width_microns (float): width in microns
+        width_pixels (float): width in pixels
+        font_size (int): size of the font
+        color (string): ['Black', White']
+        background (string): ['Black','White', 'None']
+        location (string): ['Lower Right','Lower Left','Top Right','Top Left']
+        show (bool): controls whether the Scale_bar is displayed or not
+    '''
+    
+    def __init__(self):
+        super().__init__()
+    def gui(self):
+        self.gui_reset()
+        w=g.win
+        width_microns=QtWidgets.QDoubleSpinBox()
+        
+        width_pixels=QtWidgets.QSpinBox()
+        width_pixels.setRange(.001,1000000)
+        width_pixels.setRange(1,w.mx)
+        
+        font_size=QtWidgets.QSpinBox()
+        
+        color=ComboBox()
+        color.addItem("White")
+        color.addItem("Black")
+        background=ComboBox()
+        background.addItem('None')
+        background.addItem('Black')
+        background.addItem('White')
+        location=ComboBox()
+        location.addItem('Lower Right')
+        location.addItem('Lower Left')
+        location.addItem('Top Right')
+        location.addItem('Top Left')
+        show=CheckBox()
+        if hasattr(w,'scaleBarLabel') and w.scaleBarLabel is not None: #if the scaleBarLabel already exists
+            props=w.scaleBarLabel.flika_properties
+            width_microns.setValue(props['width_microns'])
+            width_pixels.setValue(props['width_pixels'])
+            font_size.setValue(props['font_size'])
+            color.setCurrentIndex(color.findText(props['color']))
+            background.setCurrentIndex(background.findText(props['background']))
+            location.setCurrentIndex(location.findText(props['location']))
+        else:
+            font_size.setValue(12)
+            width_pixels.setValue(int(w.mx/8))
+            width_microns.setValue(1)
+            
+        show.setChecked(True) 
+        self.items.append({'name':'width_microns','string':'Width of bar in microns','object':width_microns})
+        self.items.append({'name':'width_pixels','string':'Width of bar in pixels','object':width_pixels})
+        self.items.append({'name':'font_size','string':'Font size','object':font_size})
+        self.items.append({'name':'color','string':'Color','object':color})
+        self.items.append({'name':'background','string':'Background','object':background})
+        self.items.append({'name':'location','string':'Location','object':location})
+        self.items.append({'name':'show','string':'Show','object':show})
+        
+        super().gui()
+        self.preview()
+    def __call__(self,width_microns, width_pixels, font_size, color, background,location,show=True,keepSourceWindow=None):
+        w=g.win
+        if show:
+            if hasattr(w,'scaleBarLabel') and w.scaleBarLabel is not None:
+                w.imageview.view.removeItem(w.scaleBarLabel.bar)
+                w.imageview.view.removeItem(w.scaleBarLabel)
+                w.imageview.view.sigResized.disconnect(self.updateBar)
+            if location=='Top Left':
+                anchor=(0,0)
+                pos=[0,0]
+            elif location=='Top Right':
+                anchor=(0,0)
+                pos=[w.mx,0]
+            elif location=='Lower Right':
+                anchor=(0,0)
+                pos=[w.mx,w.my]
+            elif location=='Lower Left':
+                anchor=(0,0)
+                pos=[0,w.my]
+            w.scaleBarLabel= pg.TextItem(anchor=anchor, html="<span style='font-size: {}pt;color:{};background-color:{};'>{} μm</span>".format(font_size, color, background,width_microns))
+            w.scaleBarLabel.setPos(pos[0],pos[1])
+            w.scaleBarLabel.flika_properties={item['name']:item['value'] for item in self.items}
+            w.imageview.view.addItem(w.scaleBarLabel)
+            if color=='White':
+                color255=[255,255,255,255]
+            elif color=='Black':
+                color255=[0,0,0,255]
+            textRect=w.scaleBarLabel.boundingRect()
+            
+            if location=='Top Left':
+                barPoint=QtCore.QPoint(0, textRect.height())
+            elif location=='Top Right':
+                barPoint=QtCore.QPoint(-width_pixels, textRect.height())
+            elif location=='Lower Right':
+                barPoint=QtCore.QPoint(-width_pixels, -textRect.height())
+            elif location=='Lower Left':
+                barPoint=QtCore.QPoint(0, -textRect.height())
+                
+            bar = QtWidgets.QGraphicsRectItem(QtCore.QRectF(barPoint, QtCore.QSizeF(width_pixels,int(font_size/3))))
+            bar.setPen(pg.mkPen(color255)); bar.setBrush(pg.mkBrush(color255))
+            w.imageview.view.addItem(bar)
+            #bar.setParentItem(w.scaleBarLabel)
+            w.scaleBarLabel.bar=bar
+            w.imageview.view.sigResized.connect(self.updateBar)
+            self.updateBar()
+            
+        else:
+            if hasattr(w,'scaleBarLabel') and w.scaleBarLabel is not None:
+                w.imageview.view.removeItem(w.scaleBarLabel.bar)
+                w.imageview.view.removeItem(w.scaleBarLabel)
+                w.scaleBarLabel=None
+                w.imageview.view.sigResized.disconnect(self.updateBar)
+        return None
+        
+    def updateBar(self):
+        w=g.win
+        width_pixels=self.getValue('width_pixels')
+        location=self.getValue('location')
+        view = w.imageview.view
+        textRect=w.scaleBarLabel.boundingRect()
+        textWidth=textRect.width()*view.viewPixelSize()[0]
+        textHeight=textRect.height()*view.viewPixelSize()[1]
+        
+        if location=='Top Left':
+            barPoint=QtCore.QPoint(0, 1.3*textHeight)
+            w.scaleBarLabel.setPos(QtCore.QPointF(width_pixels/2-textWidth/2,0))
+        elif location=='Top Right':
+            barPoint=QtCore.QPoint(w.mx-width_pixels, 1.3*textHeight)
+            w.scaleBarLabel.setPos(QtCore.QPointF(w.mx-width_pixels/2-textWidth/2,0))
+        elif location=='Lower Right':
+            barPoint=QtCore.QPoint(w.mx-width_pixels, w.my-1.3*textHeight)
+            w.scaleBarLabel.setPos(QtCore.QPointF(w.mx-width_pixels/2-textWidth/2,w.my-textHeight))
+        elif location=='Lower Left':
+            barPoint=QtCore.QPoint(0, w.my-1.3*textHeight)
+            w.scaleBarLabel.setPos(QtCore.QPointF(QtCore.QPointF(width_pixels/2-textWidth/2,w.my-textHeight)))
+        w.scaleBarLabel.bar.setRect(QtCore.QRectF(barPoint, QtCore.QSizeF(width_pixels,textHeight/4)))
+        
+    def preview(self):
+        width_microns=self.getValue('width_microns')
+        width_pixels=self.getValue('width_pixels')
+        font_size=self.getValue('font_size')
+        color=self.getValue('color')
+        background=self.getValue('background')
+        location=self.getValue('location')
+        show=self.getValue('show')
+        self.__call__(width_microns, width_pixels, font_size, color, background, location, show)
+scale_bar=Scale_Bar()
+
+
+
+logger.debug("Completed 'reading process/overlay.py'")
+
+
+
```

### Comparing `flika-0.2.9/flika/process/progress_bar.py` & `flika-0.3.0/flika/process/progress_bar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,270 +1,271 @@
-# -*- coding: utf-8 -*-
-import sys, time
-from qtpy import QtCore, QtGui, QtWidgets
-from multiprocessing import Process, Queue, cpu_count, Pipe
-import os
-import numpy as np
-
-__all__ = []
-
-tic=time.time()
-
-class ProcessLauncher(QtCore.QThread):
-    status_update=QtCore.Signal(str)
-    def __init__(self,parent):
-        QtCore.QThread.__init__(self)
-        self.parent=parent
-        self.nCores=parent.nCores
-    def __del__(self):
-        self.wait()
-    def run(self):
-        p=self.parent
-        nCores=self.nCores
-
-        for i in range(nCores):
-            self.status_update.emit('Creating process {}/{}'.format(i+1,nCores))
-            q_result=Queue()
-            q_progress=Queue()
-            q_status=Queue()
-            parent_conn, child_conn=Pipe()
-            p.q_results.append(q_result)
-            p.q_progress.append(q_progress)
-            p.q_status.append(q_status)
-            p.pipes.append(parent_conn)
-            p.processes.append(Process(target=p.outerfunc, args=(q_result, q_progress, q_status, child_conn, p.args )))
-
-        started=[False for i in range(nCores)]
-        for i in range(nCores):
-            if p.stopPressed:
-                break
-            self.status_update.emit('Initializing process {}/{}'.format(i+1,nCores))
-            p.processes[i].start()
-            started[i]=True
-        for i in range(nCores):
-            if started[i]:
-                if not p.stopPressed:
-                    self.status_update.emit('Sending data to process {}/{}'.format(i+1,nCores))
-                    tic=time.time()
-                    p.pipes[i].send(p.data[i])
-                    #print('Time it took to send data: {}'.format(time.time()-tic))
-        for i in range(nCores):
-            if started[i]:
-                if not p.stopPressed:
-                    self.status_update.emit('Starting process {}/{}'.format(i+1,nCores))
-                    p.q_status[i].put('Start')
-                else:
-                    p.q_status[i].put('Stop')
-            else: #if the the process was never started
-                p.process_finished[i]=True
-        self.status_update.emit(p.msg)
-        
-        
-
-        
-    
-class ProgressBar(QtWidgets.QWidget):
-    finished_sig=QtCore.Signal()
-    def __init__(self, outerfunc, data, args, nCores, msg='Performing Operations', parent=None ):
-        super(ProgressBar, self).__init__(parent)
-        self.outerfunc=outerfunc
-        self.data=data
-        self.args=args
-        self.nCores=nCores
-        self.msg=msg
-        
-        # GUI
-        self.label=QtWidgets.QLabel(msg)
-        #self.setAttribute(QtCore.Qt.WA_DeleteOnClose)
-        self.progress_bars=[]
-        self.button = QtWidgets.QPushButton('Stop')
-        self.button.clicked.connect(self.handleButton)
-        main_layout = QtWidgets.QGridLayout()
-        main_layout.addWidget(self.label,0,0)
-        main_layout.addWidget(self.button, 0, 1)
-        for i in range(nCores):
-            bar=QtWidgets.QProgressBar()
-            bar.setMinimum(1)
-            bar.setMaximum(100)
-            main_layout.addWidget(bar, 1+i, 0)
-            self.progress_bars.append(bar)
-        self.setLayout(main_layout)
-        self.setWindowTitle(msg)
-        self.stopPressed = False
-        self.show()
-        QtWidgets.qApp.processEvents()
-        
-        self.results=[None for i in range(nCores)]
-        self.process_finished=[False for i in range(nCores)]
-        self.q_results=[]
-        self.q_progress=[]
-        self.q_status=[]
-        self.pipes=[]
-        self.processes=[]
-        self.processLauncher=ProcessLauncher(self)
-        self.processLauncher.status_update.connect(self.status_updated)
-        self.processLauncher.start()
-        
-        self.timer=QtCore.QTimer()
-        self.timer.timeout.connect(self.check_if_finished)
-        self.timer.start(50)
-        
-        self.loop = QtCore.QEventLoop()
-        self.finished=False
-        self.finished_sig.connect(self.loop.quit)
-        self.finished_sig.connect(self.update_finished_status)
-        self.loop.exec_() # This blocks until the "finished" signal is emitted
-        
-        while self.finished is False: #the exec_() loop doesn't wait for loop.quit when running in spyder for some reason.  This is the workaround
-            time.sleep(.01)
-            QtWidgets.qApp.processEvents()
-        self.close()
-        
-    def check_if_finished(self):
-        for i in range(len(self.q_progress)):
-            if not self.q_progress[i].empty():
-                while not self.q_progress[i].empty():
-                    percent=self.q_progress[i].get()
-                self.progress_bars[i].setValue(percent)
-            if not self.q_results[i].empty():
-                self.progress_bars[i].setValue(100)
-                self.results[i]=self.q_results[i].get()
-                self.process_finished[i]=True
-                self.processes[i].join(1)
-        QtWidgets.qApp.processEvents()
-        if all(self.process_finished):
-            if any(r is None for r in self.results):
-                self.results=None
-            self.timer.timeout.disconnect()
-            self.finished_sig.emit()
-        if self.stopPressed:
-            #print('STOPPPPP')
-            for i in range(self.nCores):
-                self.q_status[i].put('Stop')
-
-    def handleButton(self):
-        self.stopPressed=True
-    
-    def status_updated(self,msg):
-        self.label.setText(msg)
-    def update_finished_status(self):
-        self.finished=True
-
-    def clear_memory(self):
-        for child in self.children():
-            child.deleteLater()
-        for attr in dir(self):
-            try:
-                delattr(self, attr)
-            except Exception:
-                pass
-        
-    def clear_memory(self):
-        for child in self.children():
-            child.deleteLater()
-        for attr in dir(self):
-            try:
-                delattr(self, attr)
-            except Exception:
-                pass
-        
-#    def closeEvent(self, event):
-#        for child in self.findChildren(QtGui.QDialog):
-#            if child is not widget:
-#                child.deleteLater()
-#                    
-#        if self.closed:
-#            print('This window was already closed')
-#            event.accept()
-#        else:
-#            self.closeSignal.emit()
-#            if hasattr(self,'image'):
-#                del self.image
-#            self.imageview.setImage(np.zeros((2,2))) #clear the memory
-#            self.imageview.close()
-#            del self.imageview
-#            g.m.setWindowTitle("flika")
-#            if g.currentWindow==self:
-#                g.currentWindow=None
-#            if self in g.windows:
-#                g.windows.remove(self)
-#            self.closed=True
-#            event.accept() # let the window close
-        
-        
-        
-'''
-When using the Progress Bar, you need to write two functions:
-    1) An outer function that takes an object like a numpy array, breaks it into blocks, and creates the ProgressBar object.
-    2) An inner function that receives the chunks, performs the processing, and returns the results.
-
-The first function should look something like this:  
-'''
-def outer_func():
-    # get original data and arguments that the inner function will receive
-    original_data=np.random.random((1000,200,200))
-    args=(1,)
-    
-    #break data into blocks
-    nCores = cpu_count()
-    
-    block_ends = np.linspace(0,len(original_data),nCores+1).astype(np.int)
-    data_blocks=[original_data[block_ends[i]:block_ends[i+1]] for  i in np.arange(nCores)] # each thread will get one element of this list.
-    
-    # create the ProgressBar object
-    progress = ProgressBar(inner_func, data_blocks, args, nCores, msg='Performing my cool inner function')
-    
-    # Once the ProgressBar object finishes running, the results of all the 
-    # inner function's computations will be stored in progress.results in a 
-    # list.  You will have to merge the list. If the user presses the Stop
-    # button, the progress.results will be set to None
-    if progress.results is None or any(r is None for r in progress.results):
-        result=None
-    else:
-        result=np.concatenate(progress.results,axis=0)
-    return result
-'''
-The inner function will actually do the heavy lifting.  
-Each process will be running the inner function.  Each inner function must 
-take the same 5 arguments.  
-'''
-def inner_func(q_results, q_progress, q_status, child_conn, args):
-    data=child_conn.recv() # unfortunately this step takes a long time
-    percent=0  # This is the variable we send back which displays our progress
-    status=q_status.get(True) #this blocks the process from running until all processes are launched
-    if status=='Stop':
-        q_results.put(None) # if the user presses stop, return None
-    
-    
-    # Here is the meat of the inner_func.
-    val,=args #unpack all the variables inside the args tuple
-    result=np.zeros(data.shape)
-    ii,jj,kk=data.shape
-    for i in np.arange(ii):
-        for j in np.arange(jj):
-            for k in np.arange(kk):
-                result[i,j,k]=data[i,j,k]+val
-            
-        if not q_status.empty(): #check if the stop button has been pressed
-            stop=q_status.get(False)
-            q_results.put(None)
-            return
-        if percent<int(100*i/ii):
-            percent=int(100*i/ii)
-            q_progress.put(percent)
-                    
-    # finally, when we've finished with our calculation, we send back the result
-    q_results.put(result)
-    
-    
-    
-
-        
-if __name__ == '__main__':
-    app = QtWidgets.QApplication(sys.argv)
-    result=outer_func()
-    print(result)
-
-
-
-
-
+# -*- coding: utf-8 -*-
+import sys, time
+from qtpy import QtCore, QtGui, QtWidgets
+from multiprocessing import Process, Queue, cpu_count, Pipe
+import os
+import numpy as np
+
+__all__ = []
+
+tic=time.time()
+
+class ProcessLauncher(QtCore.QThread):
+    status_update=QtCore.Signal(str)
+    def __init__(self,parent):
+        QtCore.QThread.__init__(self)
+        self.parent=parent
+        self.nCores=parent.nCores
+    def __del__(self):
+        self.wait()
+    def run(self):
+        p=self.parent
+        nCores=self.nCores
+
+        for i in range(nCores):
+            self.status_update.emit('Creating process {}/{}'.format(i+1,nCores))
+            q_result=Queue()
+            q_progress=Queue()
+            q_status=Queue()
+            parent_conn, child_conn=Pipe()
+            p.q_results.append(q_result)
+            p.q_progress.append(q_progress)
+            p.q_status.append(q_status)
+            p.pipes.append(parent_conn)
+            p.processes.append(Process(target=p.outerfunc, args=(q_result, q_progress, q_status, child_conn, p.args )))
+
+        started=[False for i in range(nCores)]
+        for i in range(nCores):
+            if p.stopPressed:
+                break
+            self.status_update.emit('Initializing process {}/{}'.format(i+1,nCores))
+            p.processes[i].start()
+            started[i]=True
+        for i in range(nCores):
+            if started[i]:
+                if not p.stopPressed:
+                    self.status_update.emit('Sending data to process {}/{}'.format(i+1,nCores))
+                    tic=time.time()
+                    p.pipes[i].send(p.data[i])
+                    #print('Time it took to send data: {}'.format(time.time()-tic))
+        for i in range(nCores):
+            if started[i]:
+                if not p.stopPressed:
+                    self.status_update.emit('Starting process {}/{}'.format(i+1,nCores))
+                    p.q_status[i].put('Start')
+                else:
+                    p.q_status[i].put('Stop')
+            else: #if the the process was never started
+                p.process_finished[i]=True
+        self.status_update.emit(p.msg)
+        
+        
+
+        
+    
+class ProgressBar(QtWidgets.QWidget):
+    finished_sig=QtCore.Signal()
+    def __init__(self, outerfunc, data, args, nCores, msg='Performing Operations', parent=None ):
+        super(ProgressBar, self).__init__(parent)
+        self.outerfunc=outerfunc
+        self.data=data
+        self.args=args
+        self.nCores=nCores
+        self.msg=msg
+        
+        # GUI
+        self.label=QtWidgets.QLabel(msg)
+        #self.setAttribute(QtCore.Qt.WA_DeleteOnClose)
+        self.progress_bars=[]
+        self.button = QtWidgets.QPushButton('Stop')
+        self.button.clicked.connect(self.handleButton)
+        main_layout = QtWidgets.QGridLayout()
+        main_layout.addWidget(self.label,0,0)
+        main_layout.addWidget(self.button, 0, 1)
+        for i in range(nCores):
+            bar=QtWidgets.QProgressBar()
+            bar.setMinimum(1)
+            bar.setMaximum(100)
+            main_layout.addWidget(bar, 1+i, 0)
+            self.progress_bars.append(bar)
+        self.setLayout(main_layout)
+        self.setWindowTitle(msg)
+        self.stopPressed = False
+        self.show()
+        QtWidgets.QApplication.processEvents()
+        
+        self.results=[None for i in range(nCores)]
+        self.process_finished=[False for i in range(nCores)]
+        self.q_results=[]
+        self.q_progress=[]
+        self.q_status=[]
+        self.pipes=[]
+        self.processes=[]
+        self.processLauncher=ProcessLauncher(self)
+        self.processLauncher.status_update.connect(self.status_updated)
+        self.processLauncher.start()
+        
+        self.timer=QtCore.QTimer()
+        self.timer.timeout.connect(self.check_if_finished)
+        self.timer.start(50)
+        
+        self.loop = QtCore.QEventLoop()
+        self.finished=False
+        self.finished_sig.connect(self.loop.quit)
+        self.finished_sig.connect(self.update_finished_status)
+        self.loop.exec_() # This blocks until the "finished" signal is emitted
+        
+        while self.finished is False: #the exec_() loop doesn't wait for loop.quit when running in spyder for some reason.  This is the workaround
+            time.sleep(.01)
+            QtWidgets.QApplication.processEvents()
+        self.close()
+        
+    def check_if_finished(self):
+        for i in range(len(self.q_progress)):
+            if not self.q_progress[i].empty():
+                while not self.q_progress[i].empty():
+                    percent=self.q_progress[i].get()
+                self.progress_bars[i].setValue(percent)
+            if not self.q_results[i].empty():
+                self.progress_bars[i].setValue(100)
+                self.results[i]=self.q_results[i].get()
+                self.process_finished[i]=True
+                self.processes[i].join(1)
+        QtWidgets.QApplication.processEvents()
+        if all(self.process_finished):
+            if any(r is None for r in self.results):
+                self.results=None
+            self.timer.timeout.disconnect()
+            self.finished_sig.emit()
+        if self.stopPressed:
+            #print('STOPPPPP')
+            for i in range(self.nCores):
+                self.q_status[i].put('Stop')
+
+    def handleButton(self):
+        self.stopPressed=True
+    
+    def status_updated(self,msg):
+        self.label.setText(msg)
+    def update_finished_status(self):
+        self.finished=True
+
+    def clear_memory(self):
+        for child in self.children():
+            child.deleteLater()
+        for attr in dir(self):
+            try:
+                delattr(self, attr)
+            except Exception:
+                pass
+        
+    def clear_memory(self):
+        for child in self.children():
+            child.deleteLater()
+        for attr in dir(self):
+            try:
+                delattr(self, attr)
+            except Exception:
+                pass
+        
+#    def closeEvent(self, event):
+#        for child in self.findChildren(QtGui.QDialog):
+#            if child is not widget:
+#                child.deleteLater()
+#                    
+#        if self.closed:
+#            print('This window was already closed')
+#            event.accept()
+#        else:
+#            self.closeSignal.emit()
+#            if hasattr(self,'image'):
+#                del self.image
+#            self.imageview.setImage(np.zeros((2,2))) #clear the memory
+#            self.imageview.close()
+#            del self.imageview
+#            g.m.setWindowTitle("flika")
+#            if g.win==self:
+#                g.win=None
+#            if self in g.windows:
+#                g.windows.remove(self)
+#            self.closed=True
+#            event.accept() # let the window close
+        
+        
+        
+'''
+When using the Progress Bar, you need to write two functions:
+    1) An outer function that takes an object like a numpy array, breaks it into blocks, and creates the ProgressBar object.
+    2) An inner function that receives the chunks, performs the processing, and returns the results.
+
+If you are using a progress bar in a plugin, make sure to write it in its own python file, or the threads may crash. 
+The first function should look something like this:  
+'''
+def outer_func():
+    # get original data and arguments that the inner function will receive
+    original_data=np.random.random((1000,200,200))
+    args=(1,)
+    
+    #break data into blocks
+    nCores = cpu_count()
+    
+    block_ends = np.linspace(0,len(original_data),nCores+1).astype(np.int)
+    data_blocks=[original_data[block_ends[i]:block_ends[i+1]] for  i in np.arange(nCores)] # each thread will get one element of this list.
+    
+    # create the ProgressBar object
+    progress = ProgressBar(inner_func, data_blocks, args, nCores, msg='Performing my cool inner function')
+    
+    # Once the ProgressBar object finishes running, the results of all the 
+    # inner function's computations will be stored in progress.results in a 
+    # list.  You will have to merge the list. If the user presses the Stop
+    # button, the progress.results will be set to None
+    if progress.results is None or any(r is None for r in progress.results):
+        result=None
+    else:
+        result=np.concatenate(progress.results,axis=0)
+    return result
+'''
+The inner function will actually do the heavy lifting.  
+Each process will be running the inner function.  Each inner function must 
+take the same 5 arguments.  
+'''
+def inner_func(q_results, q_progress, q_status, child_conn, args):
+    data=child_conn.recv() # unfortunately this step takes a long time
+    percent=0  # This is the variable we send back which displays our progress
+    status=q_status.get(True) #this blocks the process from running until all processes are launched
+    if status=='Stop':
+        q_results.put(None) # if the user presses stop, return None
+    
+    
+    # Here is the meat of the inner_func.
+    val,=args #unpack all the variables inside the args tuple
+    result=np.zeros(data.shape)
+    ii,jj,kk=data.shape
+    for i in np.arange(ii):
+        for j in np.arange(jj):
+            for k in np.arange(kk):
+                result[i,j,k]=data[i,j,k]+val
+            
+        if not q_status.empty(): #check if the stop button has been pressed
+            stop=q_status.get(False)
+            q_results.put(None)
+            return
+        if percent<int(100*i/ii):
+            percent=int(100*i/ii)
+            q_progress.put(percent)
+                    
+    # finally, when we've finished with our calculation, we send back the result
+    q_results.put(result)
+    
+    
+    
+
+        
+if __name__ == '__main__':
+    app = QtWidgets.QApplication(sys.argv)
+    result=outer_func()
+    print(result)
+
+
+
+
+
```

### Comparing `flika-0.2.9/flika/process/stacks.py` & `flika-0.3.0/flika/process/stacks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,523 +1,544 @@
-# -*- coding: utf-8 -*-
-import numpy as np
-from qtpy import QtWidgets
-from ..window import Window
-from .. import global_vars as g
-from .BaseProcess import BaseProcess, BaseProcess_noPriorWindow, WindowSelector, MissingWindowError, CheckBox, SliderLabel, ComboBox
-from ..tracefig import TraceFig
-
-
-__all__ = ['deinterleave','trim','zproject','image_calculator', 'pixel_binning', 'frame_binning', 'resize', 'concatenate_stacks', 'duplicate', 'generate_random_image', 'change_datatype']
-
-def duplicate():
-    old = g.currentWindow
-    if old is None:
-        g.alert('Select a window before trying to duplicate it.')
-    else:
-        return Window(old.image, old.name, old.filename, old.commands, old.metadata)
-
-class Generate_Random_Image(BaseProcess_noPriorWindow):
-    def __init__(self):
-        super().__init__()
-        self.puffs=None
-
-    def get_init_settings_dict(self):
-        s = dict()
-        s['nFrames'] = 1000
-        s['width'] = 128
-        return s
-
-    def gui(self):
-        self.gui_reset()
-        nFrames = SliderLabel(0)
-        nFrames.setRange(0,10000)
-        width = SliderLabel(0)
-        width.setRange(2,1024)
-        self.items.append({'name':'nFrames','string':'Movie Duration (frames)','object':nFrames})
-        self.items.append({'name':'width','string':'Width of image (pixels)','object':width})
-        super().gui()
-
-    def __call__(self, nFrames=10000, width=128):
-        self.start()
-        self.newtif = np.random.randn(nFrames, width, width)
-        self.newname=' Random Noise '
-        return self.end()
-generate_random_image = Generate_Random_Image()
-
-class Deinterleave(BaseProcess):
-    """ deinterleave(nChannels, keepSourceWindow=False)
-    This deinterleaves a stack into nChannels
-    
-    Parameters:
-        | nChannels (int) -- The number of channels to deinterleave.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-
-    def get_init_settings_dict(self):
-        return {'nChannels': 3}
-
-    def gui(self):
-        self.gui_reset()
-        nChannels=QtWidgets.QSpinBox()
-        nChannels.setMinimum(2)
-        self.items.append({'name':'nChannels','string':'How many Channels?','object':nChannels})
-        super().gui()
-    def __call__(self,nChannels,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-
-        newWindows=[]
-        for i in np.arange(nChannels):
-            newtif=self.tif[i::nChannels]
-            name=self.oldname+' - Channel '+str(i)
-            newWindow=Window(newtif,name,self.oldwindow.filename)
-            newWindows.append(newWindow)
-        
-        if keepSourceWindow is False:
-            self.oldwindow.close()  
-        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
-        return newWindows
-deinterleave=Deinterleave()
-
-class Pixel_binning(BaseProcess):
-    """ pixel_binning(nPixels, keepSourceWindow=False)
-    This bins the pixels to reduce the file size
-    
-    Parameters:
-        | nPixels (int) -- The number of pixels to bin.  Example: a value of 2 will reduce file size from 256x256->128x128.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-
-    def get_init_settings_dict(self):
-        s = dict()
-        s['nPixels'] = 2
-        return s
-
-    def gui(self):
-        self.gui_reset()
-        nPixels=QtWidgets.QSpinBox()
-        nPixels.setMinimum(2)
-        nPixels.setMaximum(2)
-        self.items.append({'name': 'nPixels', 'string': 'How many adjacent pixels to bin?', 'object': nPixels})
-        super().gui()
-    def __call__(self,nPixels,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        tif=self.tif
-        nDim=len(tif.shape)
-        if nPixels==2:
-            if nDim==4:
-                image1=tif[:,0::2,0::2,:]
-                image2=tif[:,1::2,0::2,:]
-                image3=tif[:,0::2,1::2,:]
-                image4=tif[:,1::2,1::2,:]
-                self.newtif=(image1+image2+image3+image4)/4
-                self.newname=self.oldname+' - Binned'
-                return self.end()
-            elif nDim==3:
-                mt,mx,my=tif.shape
-                if mx%2==1:
-                    tif=tif[:,:-1,:]
-                if my%2==1:
-                    tif=tif[:,:,:-1]
-                image1=tif[:,0::2,0::2]
-                image2=tif[:,1::2,0::2]
-                image3=tif[:,0::2,1::2]
-                image4=tif[:,1::2,1::2]
-                self.newtif=(image1+image2+image3+image4)/4
-                self.newname=self.oldname+' - Binned'
-                return self.end()
-            elif nDim==2:
-                image1=tif[0::2,0::2]
-                image2=tif[1::2,0::2]
-                image3=tif[0::2,1::2]
-                image4=tif[1::2,1::2]
-                self.newtif=(image1+image2+image3+image4)/4
-                self.newname=self.oldname+' - Binned'
-                return self.end()
-        else:
-            g.alert("2 is the only supported value for binning at the moment")
-pixel_binning=Pixel_binning()
-
-class Frame_binning(BaseProcess):
-    """ frame_binning(nFrames, keepSourceWindow=False)
-    This bins the pixels to reduce the file size
-    
-    Parameters:
-        | nFrames (int) -- The number of frames to bin.  Example: a value of 2 will reduce number of frames from 1000 to 500.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-
-    def get_init_settings_dict(self):
-        return {'nFrames': 2}
-
-    def gui(self):
-        self.gui_reset()
-        nFrames=QtWidgets.QSpinBox()
-        nFrames.setMinimum(2)
-        nFrames.setMaximum(10000)
-        self.items.append({'name':'nFrames','string':'How many frames to bin?','object':nFrames})
-        super().gui()
-    def __call__(self,nFrames,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        tif=self.tif
-        nDim=len(tif.shape)
-        self.newtif=np.array([np.mean(tif[i:i+nFrames],0) for i in np.arange(0,len(tif),nFrames)])
-        self.newname=self.oldname+' - Binned {} frames'.format(nFrames)
-        return self.end()
-frame_binning=Frame_binning()
-
-
-import skimage.transform
-class Resize(BaseProcess):
-    """ resize(factor, keepSourceWindow=False)
-    Performs interpolation to up-size images
-    
-    Parameters:
-        | factor (int) -- The factor to scale the images by.  Example: a value of 2 will double the number of pixels wide the images are.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-
-    def get_init_settings_dict(self):
-        return {'factor': 2}
-
-    def gui(self):
-        self.gui_reset()
-        factor=QtWidgets.QSpinBox()
-        factor.setMinimum(2)
-        factor.setMaximum(100)
-        self.items.append({'name':'factor','string':'By what factor to resize the image?','object':factor})
-        super().gui()
-
-    def __call__(self,factor,keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.tif.dtype in (np.uint64, np.int64):
-            g.alert("Resize fails on int64 and uint64 movie types, change the image type to resize.")
-            return
-        A = self.tif
-        nDim = len(A.shape)
-        is_rgb = self.oldwindow.metadata['is_rgb'] or (nDim == 3 and A.shape[2] == 3) or nDim == 4
-        B = None
-        if not is_rgb:
-            if nDim == 3:
-                mt,mx,my = A.shape
-                B = np.zeros((mt, mx*factor, my*factor))
-                for t in np.arange(mt):
-                    B[t]=skimage.transform.resize(A[t], (mx*factor,my*factor))
-            elif nDim == 2:
-                mx, my = A.shape
-                B = skimage.transform.resize(A,(mx*factor, my*factor))
-        self.newtif = B
-        self.newname = self.oldname+' - resized {}x '.format(factor)
-        return self.end()
-resize = Resize()
-
-
-class Trim(BaseProcess):
-    """ trim(firstFrame, lastFrame, increment=1, delete=False, keepSourceWindow=False)
-    This creates a new stack from the frames between the firstFrame and the lastFrame
-    
-    Parameters:
-        | firstFrame (int) -- The index of the first frame in the stack to be kept.
-        | lastFrame (int) -- The index of the last frame in the stack to be kept.
-        | increment (int) -- if increment equals i, then every ith frame is kept.
-        | delete (bool) -- if False, then the specified frames will be kept.  If True, they will be deleted.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-
-    def get_init_settings_dict(self):
-        s = dict()
-        s['firstFrame'] = 0
-        s['lastFrame'] = g.currentWindow.image.shape[0]
-        s['increment'] = 1
-        s['delete'] = False
-        return s
-
-    def gui(self):
-        self.gui_reset()
-        nFrames=1
-        if g.currentWindow is not None:
-            nFrames=g.currentWindow.image.shape[0]
-        firstFrame=QtWidgets.QSpinBox()
-        firstFrame.setMaximum(nFrames-1)
-        lastFrame=QtWidgets.QSpinBox()
-        lastFrame.setRange(0,nFrames-1)
-        increment=QtWidgets.QSpinBox()
-        increment.setMaximum(nFrames)
-        increment.setMinimum(1)
-        delete = CheckBox()
-
-        self.items.append({'name': 'firstFrame', 'string': 'First Frame', 'object': firstFrame})
-        self.items.append({'name': 'lastFrame',  'string': 'Last Frame',  'object': lastFrame })
-        self.items.append({'name': 'increment',  'string': 'Increment',   'object': increment })
-        self.items.append({'name': 'delete',     'string': 'Delete',      'object': delete    })
-        super().gui()
-
-    def __call__(self, firstFrame, lastFrame, increment=1, delete = False, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if not delete:
-            self.newtif=self.tif[firstFrame:lastFrame+1:increment]
-        if delete:
-            idxs_not=np.arange(firstFrame, lastFrame+1, increment)
-            idxs = np.ones(len(self.tif),dtype=np.bool)
-            idxs[idxs_not] = False
-            self.newtif = self.tif[idxs]
-        self.newname=self.oldname+' - Kept Stack'
-        return self.end()
-trim=Trim()
-
-
-class ZProject(BaseProcess):
-    """ zproject(firstFrame,lastFrame,projection_type,keepSourceWindow=False)
-    This creates a new stack from the frames between the firstFrame and the lastFrame
-    
-    Parameters:
-        | firstFrame (int) -- The index of the first frame in the stack to be kept.
-        | lastFrame (int) -- The index of the last frame in the stack to be kept.
-        | projection_type (str) -- Method used to combine the frames.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-
-    def get_init_settings_dict(self):
-        return {'firstFrame': 0, 'lastFrame': 0, 'projection_type': 'Average'}
-
-    def gui(self):
-        self.gui_reset()
-        nFrames=1
-        if g.currentWindow and len(g.currentWindow.image.shape) != 3:
-            g.alert('zproject only works on 3 dimensional windows')
-            return False
-        if g.currentWindow is not None:
-            nFrames=g.currentWindow.image.shape[0]
-        firstFrame=QtWidgets.QSpinBox()
-        firstFrame.setMaximum(nFrames)
-        self.items.append({'name':'firstFrame','string':'First Frame','object':firstFrame})
-        lastFrame=QtWidgets.QSpinBox()
-        lastFrame.setRange(1,nFrames-1)
-        self.items.append({'name':'lastFrame','string':'Last Frame','object':lastFrame})
-        projection_type=ComboBox()
-        projection_type.addItem('Average')
-        projection_type.addItem('Max Intensity')
-        projection_type.addItem('Min Intensity')
-        projection_type.addItem('Sum Slices')
-        projection_type.addItem('Standard Deviation')
-        projection_type.addItem('Median')
-        self.items.append({'name':'projection_type','string':'Projection Type','object':projection_type})
-        super().gui()
-        lastFrame.setValue(nFrames - 1)
-
-    def __call__(self, firstFrame, lastFrame, projection_type, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        if self.tif.ndim != 3 or self.tif.shape[2] == 3:
-            g.m.statusBar().showMessage('zproject only works on 3 dimensional, non-color windows')
-            return False
-        self.newtif=self.tif[firstFrame:lastFrame+1]
-        p=projection_type
-        if p=='Average':
-            self.newtif=np.mean(self.newtif,0)
-        elif p=='Max Intensity':
-            self.newtif=np.max(self.newtif,0)
-        elif p=='Min Intensity':
-            self.newtif=np.min(self.newtif,0)
-        elif p=='Sum Slices':
-            self.newtif=np.sum(self.newtif,0)
-        elif p=='Standard Deviation':
-            self.newtif=np.std(self.newtif,0)
-        elif p=='Median':
-            self.newtif=np.median(self.newtif,0)
-        self.newname=self.oldname+' {} Projection'.format(projection_type)
-        return self.end()
-zproject=ZProject()
-
-class Image_calculator(BaseProcess):
-    """ image_calculator(window1,window2,operation,keepSourceWindow=False)
-    This creates a new stack by combining two windows in an operation
-    
-    Parameters:
-        | window1 (Window) -- The first window 
-        | window2 (Window) -- The second window
-        | operation (str)  -- Method used to combine the frames.
-    Returns:
-        newWindow
-    """
-    def __init__(self):
-        super().__init__()
-
-    def gui(self):
-        self.gui_reset()
-        window1=WindowSelector()
-        window2=WindowSelector()      
-        operation=ComboBox()
-        operation.addItems(['Add','Subtract','Multiply','Divide','AND','OR','XOR','Min','Max','Average'])
-        self.items.append({'name':'window1','string':'Window 1','object':window1})
-        self.items.append({'name':'window2','string':'Window 2','object':window2})
-        self.items.append({'name':'operation','string':'Operation','object':operation})
-        super().gui()
-    def __call__(self,window1, window2, operation, keepSourceWindow=False):
-        self.keepSourceWindow=keepSourceWindow
-        g.m.statusBar().showMessage('Performing {}...'.format(self.__name__))
-        if window1 is None or window2 is None:
-            g.alert("You cannot execute '{}' without selecting a window first.".format(self.__name__))
-            return None
-        A = window1.image
-        B = window2.image
-        nDim1 = len(A.shape)
-        nDim2 = len(B.shape)
-        xyshape1 = A.shape
-        xyshape2 = B.shape
-        if nDim1 == 3:
-            xyshape1 = xyshape1[1:]
-        if nDim2 == 3:
-            xyshape2 = xyshape2[1:]
-        if xyshape1 != xyshape2:
-            g.alert('The two windows have images of different shapes. They could not be combined')
-            return None
-        if nDim1 == 3 and nDim2 == 3:
-            n1=A.shape[0]; n2=B.shape[0]
-            if n1 != n2: #if the two movies have different # frames
-                n = np.min([n1,n2])
-                A = A[:n] #shrink them so they have the same length
-                B = B[:n]
-                
-        
-        if operation=='Add':
-            self.newtif=np.add(A,B)
-        elif operation=='Subtract':
-            self.newtif=np.subtract(A,B)
-        elif operation=='Multiply':
-            self.newtif=np.multiply(A,B)
-        elif operation=='Divide':
-            self.newtif=np.divide(A,B)
-            self.newtif[np.isnan(self.newtif)]=0
-            self.newtif[np.isinf(self.newtif)]=0
-        if operation=='AND':
-            self.newtif=np.logical_and(window1.image,window2.image).astype(np.uint8)
-        elif operation=='OR':
-            self.newtif=np.logical_or(window1.image,window2.image).astype(np.uint8)
-        elif operation=='XOR':
-            self.newtif=np.logical_xor(window1.image,window2.image).astype(np.uint8)
-        elif operation=='Min':
-            self.newtif=np.minimum(A,B)
-        elif operation=='Max':
-            self.newtif=np.maximum(A,B)
-        elif operation=='Average':
-            if nDim1==3 and nDim2==3:
-                C=np.concatenate((np.expand_dims(A,4),np.expand_dims(B,4)),3)
-                self.newtif=np.mean(C,3)
-            elif nDim1==2 and nDim2==2:
-                C=np.concatenate((np.expand_dims(A,3),np.expand_dims(B,3)),2)
-                self.newtif=np.mean(C,2)
-            else:
-                if nDim1==3:
-                    B=np.repeat(np.expand_dims(B,0),len(A),0)
-                elif nDim2==3:
-                    A=np.repeat(np.expand_dims(A,0),len(B),0)
-                C=np.concatenate((np.expand_dims(A,4),np.expand_dims(B,4)),3)
-                self.newtif=np.mean(C,3)
-#            
-        self.oldwindow=window1
-        self.oldname=window1.name
-        self.newname=self.oldname+' - {}'.format(operation)
-        if keepSourceWindow is False:
-            print('closing both windows')
-            window1.close()
-            window2.close()
-        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
-        newWindow=Window(self.newtif,str(self.newname),self.oldwindow.filename)
-        del self.newtif
-        return newWindow
-        
-image_calculator=Image_calculator()
-
-
-class Concatenate_stacks(BaseProcess):
-    """ concatenate_stacks(window1,window2,keepSourceWindow=False)
-    This creates a new stack by concatenating two stacks
-
-    Parameters:
-        | window1 (Window) -- The first window
-        | window2 (Window) -- The second window
-    Returns:
-        newWindow
-    """
-
-    def __init__(self):
-        super().__init__()
-
-    def gui(self):
-        self.gui_reset()
-        window1 = WindowSelector()
-        window2 = WindowSelector()
-        self.items.append({'name': 'window1', 'string': 'Window 1', 'object': window1})
-        self.items.append({'name': 'window2', 'string': 'Window 2', 'object': window2})
-        super().gui()
-
-    def __call__(self, window1, window2, keepSourceWindow=False):
-        self.keepSourceWindow = keepSourceWindow
-        g.m.statusBar().showMessage('Performing {}...'.format(self.__name__))
-        if window1 is None or window2 is None:
-            raise (
-            MissingWindowError("You cannot execute '{}' without selecting a window first.".format(self.__name__)))
-        A = window1.image
-        B = window2.image
-        self.newtif = np.concatenate((A,B),0)
-
-        self.oldwindow = window1
-        self.oldname = window1.name
-        self.newname = self.oldname + ' - {}'.format('concatenated')
-        if keepSourceWindow is False:
-            print('closing both windows')
-            window1.close()
-            window2.close()
-        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
-        newWindow = Window(self.newtif, str(self.newname), self.oldwindow.filename)
-        del self.newtif
-        return newWindow
-
-
-concatenate_stacks = Concatenate_stacks()
-
-class Change_datatype(BaseProcess):
-    """ change_datatype(datatype, keepSourceWindow=False)
-    This bins the pixels to reduce the file size
-
-    Parameters:
-        | datatype (string)
-    Returns:
-        newWindow
-    """
-
-    def __init__(self):
-        super().__init__()
-
-    def gui(self):
-        self.gui_reset()
-        dtype = ComboBox()
-        dtype_strs = ['uint8', 'uint16', 'uint32', 'uint64', 'int8','int16', 'int32', 'int64', 'float16', 'float32', 'float64']
-        for d in dtype_strs:
-            dtype.addItem(d)
-        self.items.append({'name': 'datatype', 'string': 'Convert image to which datatype?', 'object': dtype})
-        super().gui()
-    def __call__(self, datatype, keepSourceWindow=False):
-        self.start(keepSourceWindow)
-        self.newtif = self.tif.astype(np.dtype(datatype))
-        self.newname = self.oldname
-        return self.end()
-
-change_datatype = Change_datatype()
+# -*- coding: utf-8 -*-
+from ..logger import logger
+logger.debug("Started 'reading process/stacks.py'")
+
+
+import numpy as np
+from qtpy import QtWidgets
+from ..window import Window
+from .. import global_vars as g
+from ..utils.BaseProcess import BaseProcess, BaseProcess_noPriorWindow, WindowSelector, MissingWindowError, CheckBox, SliderLabel, ComboBox
+
+
+
+__all__ = ['deinterleave','trim','zproject','image_calculator', 'pixel_binning', 'frame_binning', 'resize', 'concatenate_stacks', 'duplicate', 'generate_random_image', 'change_datatype']
+
+def duplicate():
+    old = g.win
+    if old is None:
+        g.alert('Select a window before trying to duplicate it.')
+    else:
+        return Window(old.image, old.name, old.filename, old.commands, old.metadata)
+
+class Generate_Random_Image(BaseProcess_noPriorWindow):
+    def __init__(self):
+        super().__init__()
+        self.puffs=None
+
+    def get_init_settings_dict(self):
+        s = dict()
+        s['nFrames'] = 1000
+        s['width'] = 128
+        return s
+
+    def gui(self):
+        self.gui_reset()
+        nFrames = SliderLabel(0)
+        nFrames.setRange(0,10000)
+        width = SliderLabel(0)
+        width.setRange(2,1024)
+        self.items.append({'name':'nFrames','string':'Movie Duration (frames)','object':nFrames})
+        self.items.append({'name':'width','string':'Width of image (pixels)','object':width})
+        super().gui()
+
+    def __call__(self, nFrames=10000, width=128):
+        self.start()
+        self.newtif = np.random.randn(nFrames, width, width)
+        self.newname=' Random Noise '
+        return self.end()
+generate_random_image = Generate_Random_Image()
+
+class Deinterleave(BaseProcess):
+    """deinterleave(nChannels, keepSourceWindow=False)
+
+    This deinterleaves a stack into nChannels
+    
+    Parameters:
+        nChannels (int): The number of channels to deinterleave.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def get_init_settings_dict(self):
+        return {'nChannels': 3}
+
+    def gui(self):
+        self.gui_reset()
+        nChannels=QtWidgets.QSpinBox()
+        nChannels.setMinimum(2)
+        self.items.append({'name':'nChannels','string':'How many Channels?','object':nChannels})
+        super().gui()
+    def __call__(self,nChannels,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+
+        newWindows=[]
+        for i in np.arange(nChannels):
+            newtif=self.tif[i::nChannels]
+            name=self.oldname+' - Channel '+str(i)
+            newWindow=Window(newtif,name,self.oldwindow.filename)
+            newWindows.append(newWindow)
+        
+        if keepSourceWindow is False:
+            self.oldwindow.close()  
+        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
+        return newWindows
+deinterleave=Deinterleave()
+
+class Pixel_binning(BaseProcess):
+    """pixel_binning(nPixels, keepSourceWindow=False)
+
+    This bins the pixels to reduce the file size
+    
+    Parameters:
+        nPixels (int): The number of pixels to bin.  Example: a value of 2 will reduce file size from 256x256->128x128.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def get_init_settings_dict(self):
+        s = dict()
+        s['nPixels'] = 2
+        return s
+
+    def gui(self):
+        self.gui_reset()
+        nPixels=QtWidgets.QSpinBox()
+        nPixels.setMinimum(2)
+        nPixels.setMaximum(2)
+        self.items.append({'name': 'nPixels', 'string': 'How many adjacent pixels to bin?', 'object': nPixels})
+        super().gui()
+    def __call__(self,nPixels,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        tif=self.tif
+        nDim=len(tif.shape)
+        if nPixels==2:
+            if nDim==4:
+                image1=tif[:,0::2,0::2,:]
+                image2=tif[:,1::2,0::2,:]
+                image3=tif[:,0::2,1::2,:]
+                image4=tif[:,1::2,1::2,:]
+                self.newtif=(image1+image2+image3+image4)/4
+                self.newname=self.oldname+' - Binned'
+                return self.end()
+            elif nDim==3:
+                mt,mx,my=tif.shape
+                if mx%2==1:
+                    tif=tif[:,:-1,:]
+                if my%2==1:
+                    tif=tif[:,:,:-1]
+                image1=tif[:,0::2,0::2]
+                image2=tif[:,1::2,0::2]
+                image3=tif[:,0::2,1::2]
+                image4=tif[:,1::2,1::2]
+                self.newtif=(image1+image2+image3+image4)/4
+                self.newname=self.oldname+' - Binned'
+                return self.end()
+            elif nDim==2:
+                image1=tif[0::2,0::2]
+                image2=tif[1::2,0::2]
+                image3=tif[0::2,1::2]
+                image4=tif[1::2,1::2]
+                self.newtif=(image1+image2+image3+image4)/4
+                self.newname=self.oldname+' - Binned'
+                return self.end()
+        else:
+            g.alert("2 is the only supported value for binning at the moment")
+pixel_binning=Pixel_binning()
+
+class Frame_binning(BaseProcess):
+    """frame_binning(nFrames, keepSourceWindow=False)
+
+    This bins the pixels to reduce the file size
+    
+    Parameters:
+        nFrames (int): The number of frames to bin.  Example: a value of 2 will reduce number of frames from 1000 to 500.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def get_init_settings_dict(self):
+        return {'nFrames': 2}
+
+    def gui(self):
+        self.gui_reset()
+        nFrames=QtWidgets.QSpinBox()
+        nFrames.setMinimum(2)
+        nFrames.setMaximum(10000)
+        self.items.append({'name':'nFrames','string':'How many frames to bin?','object':nFrames})
+        super().gui()
+    def __call__(self,nFrames,keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        tif=self.tif
+        nDim=len(tif.shape)
+        self.newtif=np.array([np.mean(tif[i:i+nFrames],0) for i in np.arange(0,len(tif),nFrames)])
+        self.newname=self.oldname+' - Binned {} frames'.format(nFrames)
+        return self.end()
+frame_binning=Frame_binning()
+
+
+
+class Resize(BaseProcess):
+    """resize(factor, keepSourceWindow=False)
+
+    Performs interpolation to up-size images
+    
+    Parameters:
+        factor (int): The factor to scale the images by.  Example: a value of 2 will double the number of pixels wide the images are.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def get_init_settings_dict(self):
+        return {'factor': 2}
+
+    def gui(self):
+        self.gui_reset()
+        factor=QtWidgets.QSpinBox()
+        factor.setMinimum(2)
+        factor.setMaximum(100)
+        self.items.append({'name':'factor','string':'By what factor to resize the image?','object':factor})
+        super().gui()
+
+    def __call__(self,factor,keepSourceWindow=False):
+        import skimage.transform
+        self.start(keepSourceWindow)
+        if self.tif.dtype in (np.uint64, np.int64):
+            g.alert("Resize fails on int64 and uint64 movie types, change the image type to resize.")
+            return
+        A = self.tif
+        nDim = len(A.shape)
+        is_rgb = self.oldwindow.metadata['is_rgb'] or (nDim == 3 and A.shape[2] == 3) or nDim == 4
+        B = None
+        if not is_rgb:
+            if nDim == 3:
+                mt,mx,my = A.shape
+                B = np.zeros((mt, mx*factor, my*factor))
+                for t in np.arange(mt):
+                    B[t]=skimage.transform.resize(A[t], (mx*factor,my*factor))
+            elif nDim == 2:
+                mx, my = A.shape
+                B = skimage.transform.resize(A,(mx*factor, my*factor))
+        self.newtif = B
+        self.newname = self.oldname+' - resized {}x '.format(factor)
+        return self.end()
+resize = Resize()
+
+
+class Trim(BaseProcess):
+    """trim(firstFrame, lastFrame, increment=1, delete=False, keepSourceWindow=False)
+
+    This creates a new stack from the frames between the firstFrame and the lastFrame
+    
+    Parameters:
+        firstFrame (int): The index of the first frame in the stack to be kept.
+        lastFrame (int): The index of the last frame in the stack to be kept.
+        increment (int): if increment equals i, then every ith frame is kept.
+        delete (bool): if False, then the specified frames will be kept.  If True, they will be deleted.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def get_init_settings_dict(self):
+        s = dict()
+        s['firstFrame'] = 0
+        s['lastFrame'] = g.win.image.shape[0]
+        s['increment'] = 1
+        s['delete'] = False
+        return s
+
+    def gui(self):
+        self.gui_reset()
+        nFrames=1
+        if g.win is not None:
+            nFrames=g.win.image.shape[0]
+        firstFrame=QtWidgets.QSpinBox()
+        firstFrame.setMaximum(nFrames-1)
+        lastFrame=QtWidgets.QSpinBox()
+        lastFrame.setRange(0,nFrames-1)
+        increment=QtWidgets.QSpinBox()
+        increment.setMaximum(nFrames)
+        increment.setMinimum(1)
+        delete = CheckBox()
+
+        self.items.append({'name': 'firstFrame', 'string': 'First Frame', 'object': firstFrame})
+        self.items.append({'name': 'lastFrame',  'string': 'Last Frame',  'object': lastFrame })
+        self.items.append({'name': 'increment',  'string': 'Increment',   'object': increment })
+        self.items.append({'name': 'delete',     'string': 'Delete',      'object': delete    })
+        super().gui()
+
+    def __call__(self, firstFrame, lastFrame, increment=1, delete = False, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if not delete:
+            self.newtif=self.tif[firstFrame:lastFrame+1:increment]
+        if delete:
+            idxs_not=np.arange(firstFrame, lastFrame+1, increment)
+            idxs = np.ones(len(self.tif),dtype=np.bool)
+            idxs[idxs_not] = False
+            self.newtif = self.tif[idxs]
+        self.newname=self.oldname+' - Kept Stack'
+        return self.end()
+trim=Trim()
+
+
+class ZProject(BaseProcess):
+    """zproject(firstFrame, lastFrame, projection_type, keepSourceWindow=False)
+
+    This creates a new stack from the frames between the firstFrame and the lastFrame
+    
+    Parameters:
+        firstFrame (int): The index of the first frame in the stack to be kept.
+        lastFrame (int): The index of the last frame in the stack to be kept.
+        projection_type (str): Method used to combine the frames.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def get_init_settings_dict(self):
+        return {'firstFrame': 0, 'lastFrame': 0, 'projection_type': 'Average'}
+
+    def gui(self):
+        self.gui_reset()
+        nFrames=1
+        if g.win and len(g.win.image.shape) != 3:
+            g.alert('zproject only works on 3 dimensional windows')
+            return False
+        if g.win is not None:
+            nFrames=g.win.image.shape[0]
+        firstFrame=QtWidgets.QSpinBox()
+        firstFrame.setMaximum(nFrames)
+        self.items.append({'name':'firstFrame','string':'First Frame','object':firstFrame})
+        lastFrame=QtWidgets.QSpinBox()
+        lastFrame.setRange(1,nFrames-1)
+        self.items.append({'name':'lastFrame','string':'Last Frame','object':lastFrame})
+        projection_type=ComboBox()
+        projection_type.addItem('Average')
+        projection_type.addItem('Max Intensity')
+        projection_type.addItem('Min Intensity')
+        projection_type.addItem('Sum Slices')
+        projection_type.addItem('Standard Deviation')
+        projection_type.addItem('Median')
+        self.items.append({'name':'projection_type','string':'Projection Type','object':projection_type})
+        super().gui()
+        lastFrame.setValue(nFrames - 1)
+
+    def __call__(self, firstFrame, lastFrame, projection_type, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        if self.tif.ndim != 3 or self.tif.shape[2] == 3:
+            g.m.statusBar().showMessage('zproject only works on 3 dimensional, non-color windows')
+            return False
+        self.newtif=self.tif[firstFrame:lastFrame+1]
+        p=projection_type
+        if p=='Average':
+            self.newtif=np.mean(self.newtif,0)
+        elif p=='Max Intensity':
+            self.newtif=np.max(self.newtif,0)
+        elif p=='Min Intensity':
+            self.newtif=np.min(self.newtif,0)
+        elif p=='Sum Slices':
+            self.newtif=np.sum(self.newtif,0)
+        elif p=='Standard Deviation':
+            self.newtif=np.std(self.newtif,0)
+        elif p=='Median':
+            self.newtif=np.median(self.newtif,0)
+        self.newname=self.oldname+' {} Projection'.format(projection_type)
+        return self.end()
+zproject=ZProject()
+
+class Image_calculator(BaseProcess):
+    """###image_calculator(window1,window2,operation,keepSourceWindow=False)
+
+    This creates a new stack by combining two windows in an operation
+    
+    Parameters:
+        window1 (Window): The first window
+        window2 (Window): The second window
+        operation (str): Method used to combine the frames.
+    Returns:
+        newWindow
+    """
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        self.gui_reset()
+        window1=WindowSelector()
+        window2=WindowSelector()      
+        operation=ComboBox()
+        operation.addItems(['Add','Subtract','Multiply','Divide','AND','OR','XOR','Min','Max','Average'])
+        self.items.append({'name':'window1','string':'Window 1','object':window1})
+        self.items.append({'name':'window2','string':'Window 2','object':window2})
+        self.items.append({'name':'operation','string':'Operation','object':operation})
+        super().gui()
+    def __call__(self,window1, window2, operation, keepSourceWindow=False):
+        self.keepSourceWindow=keepSourceWindow
+        g.m.statusBar().showMessage('Performing {}...'.format(self.__name__))
+        if window1 is None or window2 is None:
+            g.alert("You cannot execute '{}' without selecting a window first.".format(self.__name__))
+            return None
+        A = window1.image
+        B = window2.image
+        nDim1 = len(A.shape)
+        nDim2 = len(B.shape)
+        xyshape1 = A.shape
+        xyshape2 = B.shape
+        if nDim1 == 3:
+            xyshape1 = xyshape1[1:]
+        if nDim2 == 3:
+            xyshape2 = xyshape2[1:]
+        if xyshape1 != xyshape2:
+            g.alert('The two windows have images of different shapes. They could not be combined')
+            return None
+        if nDim1 == 3 and nDim2 == 3:
+            n1=A.shape[0]; n2=B.shape[0]
+            if n1 != n2: #if the two movies have different # frames
+                n = np.min([n1,n2])
+                A = A[:n] #shrink them so they have the same length
+                B = B[:n]
+                
+        
+        if operation=='Add':
+            self.newtif=np.add(A,B)
+        elif operation=='Subtract':
+            self.newtif=np.subtract(A,B)
+        elif operation=='Multiply':
+            self.newtif=np.multiply(A,B)
+        elif operation=='Divide':
+            self.newtif=np.divide(A,B)
+            self.newtif[np.isnan(self.newtif)]=0
+            self.newtif[np.isinf(self.newtif)]=0
+        if operation=='AND':
+            self.newtif=np.logical_and(window1.image,window2.image).astype(np.uint8)
+        elif operation=='OR':
+            self.newtif=np.logical_or(window1.image,window2.image).astype(np.uint8)
+        elif operation=='XOR':
+            self.newtif=np.logical_xor(window1.image,window2.image).astype(np.uint8)
+        elif operation=='Min':
+            self.newtif=np.minimum(A,B)
+        elif operation=='Max':
+            self.newtif=np.maximum(A,B)
+        elif operation=='Average':
+            if nDim1==3 and nDim2==3:
+                C=np.concatenate((np.expand_dims(A,4),np.expand_dims(B,4)),3)
+                self.newtif=np.mean(C,3)
+            elif nDim1==2 and nDim2==2:
+                C=np.concatenate((np.expand_dims(A,3),np.expand_dims(B,3)),2)
+                self.newtif=np.mean(C,2)
+            else:
+                if nDim1==3:
+                    B=np.repeat(np.expand_dims(B,0),len(A),0)
+                elif nDim2==3:
+                    A=np.repeat(np.expand_dims(A,0),len(B),0)
+                C=np.concatenate((np.expand_dims(A,4),np.expand_dims(B,4)),3)
+                self.newtif=np.mean(C,3)
+#            
+        self.oldwindow=window1
+        self.oldname=window1.name
+        self.newname=self.oldname+' - {}'.format(operation)
+        if keepSourceWindow is False:
+            print('closing both windows')
+            window1.close()
+            window2.close()
+        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
+        newWindow=Window(self.newtif,str(self.newname),self.oldwindow.filename)
+        del self.newtif
+        return newWindow
+        
+image_calculator=Image_calculator()
+
+
+class Concatenate_stacks(BaseProcess):
+    """concatenate_stacks(window1,window2,keepSourceWindow=False)
+
+    This creates a new stack by concatenating two stacks
+
+    Parameters:
+        window1 (Window): The first window
+        window2 (Window): The second window
+    Returns:
+        newWindow
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        self.gui_reset()
+        window1 = WindowSelector()
+        window2 = WindowSelector()
+        self.items.append({'name': 'window1', 'string': 'Window 1', 'object': window1})
+        self.items.append({'name': 'window2', 'string': 'Window 2', 'object': window2})
+        super().gui()
+
+    def __call__(self, window1, window2, keepSourceWindow=False):
+        self.keepSourceWindow = keepSourceWindow
+        g.m.statusBar().showMessage('Performing {}...'.format(self.__name__))
+        if window1 is None or window2 is None:
+            raise (
+            MissingWindowError("You cannot execute '{}' without selecting a window first.".format(self.__name__)))
+        A = window1.image
+        B = window2.image
+        try:
+            self.newtif = np.concatenate((A, B), 0)
+        except ValueError:
+            if len(A.shape) == 2 and len(B.shape) == 3:
+                self.newtif = np.concatenate((np.expand_dims(A, 0), B), 0)
+            elif len(A.shape) == 3 and len(B.shape) == 2:
+                self.newtif = np.concatenate((A, np.expand_dims(B, 0)), 0)
+        self.oldwindow = window1
+        self.oldname = window1.name
+        self.newname = self.oldname + ' - {}'.format('concatenated')
+        if keepSourceWindow is False:
+            print('closing both windows')
+            window1.close()
+            window2.close()
+        g.m.statusBar().showMessage('Finished with {}.'.format(self.__name__))
+        newWindow = Window(self.newtif, str(self.newname), self.oldwindow.filename)
+        del self.newtif
+        return newWindow
+
+
+concatenate_stacks = Concatenate_stacks()
+
+class Change_datatype(BaseProcess):
+    """change_datatype(datatype, keepSourceWindow=False)
+
+    This bins the pixels to reduce the file size
+
+    Parameters:
+        datatype (string)
+    Returns:
+        newWindow
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def gui(self):
+        self.gui_reset()
+        dtype = ComboBox()
+        dtype_strs = ['uint8', 'uint16', 'uint32', 'uint64', 'int8','int16', 'int32', 'int64', 'float16', 'float32', 'float64']
+        for d in dtype_strs:
+            dtype.addItem(d)
+        self.items.append({'name': 'datatype', 'string': 'Convert image to which datatype?', 'object': dtype})
+        super().gui()
+    def __call__(self, datatype, keepSourceWindow=False):
+        self.start(keepSourceWindow)
+        self.newtif = self.tif.astype(np.dtype(datatype))
+        self.newname = self.oldname
+        return self.end()
+
+change_datatype = Change_datatype()
+
+logger.debug("Completed 'reading process/stacks.py'")
```

### Comparing `flika-0.2.9/flika/process/__init__.py` & `flika-0.3.0/flika/process/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,93 @@
-# -*- coding: utf-8 -*-
-from .stacks import *
-from .math_ import *
-from .filters import *
-from .binary import *
-from .roi import *
-from .measure import *
-from .color import *
-from .overlay import *
-from .file_ import *
-
-def setup_menus():
-    from .. import global_vars as g
-    if len(g.menus) > 0:
-        print("flika menubar already initialized.")
-        return
-    from qtpy import QtGui, QtWidgets
-    imageMenu = QtWidgets.QMenu("Image")
-    processMenu = QtWidgets.QMenu("Process")
-
-    def addAction(menu, name, trigger):
-        menu.addAction(QtWidgets.QAction(name, menu, triggered=trigger))
-
-    stacksMenu = imageMenu.addMenu("Stacks")
-
-    addAction(stacksMenu, "Duplicate", duplicate)
-    addAction(stacksMenu, "Generate Random Image", generate_random_image.gui)
-    addAction(stacksMenu, "Trim Frames", trim.gui)
-    addAction(stacksMenu, "Deinterlace", deinterleave.gui)
-    addAction(stacksMenu, "Z Project", zproject.gui)
-    addAction(stacksMenu, "Pixel Binning", pixel_binning.gui)
-    addAction(stacksMenu, "Frame Binning", frame_binning.gui)
-    addAction(stacksMenu, "Resize", resize.gui)
-    addAction(stacksMenu, "Concatenate Stacks", concatenate_stacks.gui)
-    addAction(stacksMenu, "Change Data Type", change_datatype.gui)
-
-    colorMenu = imageMenu.addMenu("Color")
-    addAction(colorMenu, "Split Channels", split_channels.gui)
-
-    addAction(imageMenu, "Measure", measure.gui)
-    addAction(imageMenu, "Set Value", set_value.gui)
-    overlayMenu = imageMenu.addMenu("Overlay")
-    addAction(overlayMenu, "Background", background.gui)
-    addAction(overlayMenu, "Timestamp", time_stamp.gui)
-    addAction(overlayMenu, "Scale Bar", scale_bar.gui)
-
-    binaryMenu = processMenu.addMenu("Binary")
-    mathMenu = processMenu.addMenu("Math")
-    filtersMenu = processMenu.addMenu("Filters")
-    processMenu.addAction(QtWidgets.QAction("Image Calculator", processMenu, triggered=image_calculator.gui))
-
-    addAction(binaryMenu, "Threshold", threshold.gui)
-    addAction(binaryMenu, "Adaptive Threshold", adaptive_threshold.gui)
-    addAction(binaryMenu, "Canny Edge Detector", canny_edge_detector.gui)
-    binaryMenu.addSeparator()
-    addAction(binaryMenu, "Logically Combine", logically_combine.gui)
-    addAction(binaryMenu, "Remove Small Blobs", remove_small_blobs.gui)
-    addAction(binaryMenu, "Binary Erosion", binary_erosion.gui)
-    addAction(binaryMenu, "Binary Dilation", binary_dilation.gui)
-    addAction(binaryMenu, "Generate ROIs", generate_rois.gui)
-
-    addAction(mathMenu, "Multiply", multiply.gui)
-    addAction(mathMenu, "Subtract", subtract.gui)
-    addAction(mathMenu, "Power", power.gui)
-    addAction(mathMenu, "Ratio By Baseline", ratio.gui)
-    addAction(mathMenu, "Absolute Value", absolute_value.gui)
-    addAction(mathMenu, "Subtract Trace", subtract_trace.gui)
-    addAction(mathMenu, "Divide Trace", divide_trace.gui)
-
-    addAction(filtersMenu, "Gaussian Blur", gaussian_blur.gui)
-    filtersMenu.addSeparator()
-    addAction(filtersMenu, "Butterworth Filter", butterworth_filter.gui)
-    addAction(filtersMenu, "Mean Filter", mean_filter.gui)
-    addAction(filtersMenu, "Median Filter", median_filter.gui)
-    addAction(filtersMenu, "Fourier Filter", fourier_filter.gui)
-    addAction(filtersMenu, "Difference Filter", difference_filter.gui)
-    addAction(filtersMenu, "Boxcar Differential", boxcar_differential_filter.gui)
-    addAction(filtersMenu, "Wavelet Filter", wavelet_filter.gui)
-    addAction(filtersMenu, "Bilateral Filter", bilateral_filter.gui)
-
-    g.menus.append(imageMenu)
-    g.menus.append(processMenu)
+# -*- coding: utf-8 -*-
+from ..logger import logger
+logger.debug("Started 'reading process/__init__.py'")
+
+from .stacks import *
+from .math_ import *
+from .filters import *
+from .binary import *
+from .roi import *
+from .measure import *
+from .color import *
+from .overlay import *
+from .file_ import *
+
+def setup_menus():
+    logger.debug("Started 'process.__init__.setup_menus()'")
+    from .. import global_vars as g
+    if len(g.menus) > 0:
+        print("flika menubar already initialized.")
+        return
+    from qtpy import QtGui, QtWidgets
+    imageMenu = QtWidgets.QMenu("Image")
+    processMenu = QtWidgets.QMenu("Process")
+
+    def addAction(menu, name, trigger):
+        menu.addAction(QtWidgets.QAction(name, menu, triggered=trigger))
+
+    stacksMenu = imageMenu.addMenu("Stacks")
+
+    addAction(stacksMenu, "Duplicate", duplicate)
+    addAction(stacksMenu, "Generate Random Image", generate_random_image.gui)
+    addAction(stacksMenu, "Trim Frames", trim.gui)
+    addAction(stacksMenu, "Deinterlace", deinterleave.gui)
+    addAction(stacksMenu, "Z Project", zproject.gui)
+    addAction(stacksMenu, "Pixel Binning", pixel_binning.gui)
+    addAction(stacksMenu, "Frame Binning", frame_binning.gui)
+    addAction(stacksMenu, "Resize", resize.gui)
+    addAction(stacksMenu, "Concatenate Stacks", concatenate_stacks.gui)
+    addAction(stacksMenu, "Change Data Type", change_datatype.gui)
+
+    colorMenu = imageMenu.addMenu("Color")
+    addAction(colorMenu, "Split Channels", split_channels.gui)
+
+    addAction(imageMenu, "Measure", measure.gui)
+    addAction(imageMenu, "Set Value", set_value.gui)
+    overlayMenu = imageMenu.addMenu("Overlay")
+    addAction(overlayMenu, "Background", background.gui)
+    addAction(overlayMenu, "Timestamp", time_stamp.gui)
+    addAction(overlayMenu, "Scale Bar", scale_bar.gui)
+
+    binaryMenu = processMenu.addMenu("Binary")
+    mathMenu = processMenu.addMenu("Math")
+    filtersMenu = processMenu.addMenu("Filters")
+    processMenu.addAction(QtWidgets.QAction("Image Calculator", processMenu, triggered=image_calculator.gui))
+
+    addAction(binaryMenu, "Threshold", threshold.gui)
+    addAction(binaryMenu, "Adaptive Threshold", adaptive_threshold.gui)
+    addAction(binaryMenu, "Canny Edge Detector", canny_edge_detector.gui)
+    binaryMenu.addSeparator()
+    addAction(binaryMenu, "Logically Combine", logically_combine.gui)
+    addAction(binaryMenu, "Remove Small Blobs", remove_small_blobs.gui)
+    addAction(binaryMenu, "Binary Erosion", binary_erosion.gui)
+    addAction(binaryMenu, "Binary Dilation", binary_dilation.gui)
+    addAction(binaryMenu, "Generate ROIs", generate_rois.gui)
+
+    addAction(mathMenu, "Multiply", multiply.gui)
+    addAction(mathMenu, "Divide", divide.gui)
+    addAction(mathMenu, "Subtract", subtract.gui)
+    addAction(mathMenu, "Power", power.gui)
+    addAction(mathMenu, "Square Root", sqrt.gui)
+    addAction(mathMenu, "Ratio By Baseline", ratio.gui)
+    addAction(mathMenu, "Absolute Value", absolute_value.gui)
+    addAction(mathMenu, "Subtract Trace", subtract_trace.gui)
+    addAction(mathMenu, "Divide Trace", divide_trace.gui)
+
+    addAction(filtersMenu, "Gaussian Blur", gaussian_blur.gui)
+    addAction(filtersMenu, "Difference of Gaussians", difference_of_gaussians.gui)
+    filtersMenu.addSeparator()
+    addAction(filtersMenu, "Butterworth Filter", butterworth_filter.gui)
+    addAction(filtersMenu, "Mean Filter", mean_filter.gui)
+    addAction(filtersMenu, "Variance Filter", variance_filter.gui)
+    addAction(filtersMenu, "Median Filter", median_filter.gui)
+    addAction(filtersMenu, "Fourier Filter", fourier_filter.gui)
+    addAction(filtersMenu, "Difference Filter", difference_filter.gui)
+    addAction(filtersMenu, "Boxcar Differential", boxcar_differential_filter.gui)
+    addAction(filtersMenu, "Wavelet Filter", wavelet_filter.gui)
+    addAction(filtersMenu, "Bilateral Filter", bilateral_filter.gui)
+
+    g.menus.append(imageMenu)
+    g.menus.append(processMenu)
+    logger.debug("Completed 'process.__init__.setup_menus()'")
+
+logger.debug("Completed 'reading process/__init__.py'")
```

### Comparing `flika-0.2.9/flika/roi.py` & `flika-0.3.0/flika/roi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1058 +1,1145 @@
-# -*- coding: utf-8 -*-
-from qtpy import QtGui, QtCore, QtWidgets
-import pyqtgraph as pg
-from pyqtgraph.graphicsItems.ROI import Handle
-from skimage.draw import polygon, line
-import numpy as np
-import os
-from scipy.ndimage.interpolation import rotate
-from . import global_vars as g
-from .utils.misc import random_color, open_file_gui
-from .tracefig import roiPlot
-
-
-class ROI_Drawing(pg.GraphicsObject):
-    """
-    This class is used by the g.currentWindow when an roi is being created. Once the creation is finished, drawFinished()
-    is called and this class returns an ROI object.
-    """
-    def __init__(self, window, x, y, kind):
-        pg.GraphicsObject.__init__(self)
-        window.imageview.addItem(self)
-        self.window = window
-        self.pts = [pg.Point(round(x), round(y))]
-        if self.extendRectLine():
-            window.imageview.removeItem(self)
-            return
-        self.kind = kind
-        self.state = {'pos': pg.Point(x, y), 'size': pg.Point(0, 0)}
-        self.color = QtGui.QColor(g.settings['roi_color']) if g.settings['roi_color'] != 'random' else random_color()
-
-    def cancel(self):
-        g.currentWindow.imageview.removeItem(self)
-        g.currentWindow.currentROI = None
-
-    def extendRectLine(self):
-        for roi in self.window.rois:
-            if isinstance(roi, ROI_rect_line):
-                a = roi.getNearestHandle(self.pts[0])
-                if a:
-                    roi.extendHandle = a
-                    self.extend = roi.extend
-                    self.drawFinished = roi.extendFinished
-                    #self.__dict__.update(roi.__dict__)
-                    self.boundingRect = roi.boundingRect
-                    return True
-        return False
-
-    def extend(self, x, y):
-        new_pt = pg.Point(round(x), round(y))
-        if self.kind == 'freehand':
-            if self.pts[-1] != new_pt:
-                self.pts.append(new_pt)
-        elif self.kind in ('line', 'rectangle', 'rect_line'):
-            if len(self.pts) == 1:
-                self.pts.append(new_pt)
-            else:
-                self.pts[1] = new_pt
-
-            #self.pts = sorted(self.pts, key=lambda a: a.x()/a.y())
-
-        self.state['pos'] = pg.Point(*np.min(self.pts, 0))
-        self.state['size'] = pg.Point(*np.ptp(self.pts, 0))
-
-        self.prepareGeometryChange()
-        self.update()
-
-    def paint(self, p, *args):
-        pen = QtGui.QPen(self.color)
-        pen.setWidth(0)
-        p.setPen(pen)
-        if self.kind == 'freehand':
-            p.drawPolyline(*self.pts)
-        elif self.kind == 'rectangle':
-            p.drawRect(self.boundingRect())
-        elif self.kind in ('rect_line', 'line'):
-            p.drawLine(*self.pts)
-
-    def drawFinished(self):
-        self.window.imageview.removeItem(self)
-        if self.kind == 'rectangle':
-            pts = [self.state['pos'], self.state['size']]
-        else:
-            pts = self.pts
-        return makeROI(self.kind, pts, self.window)
-
-
-    def contains(self, *args):
-        if len(args) == 2:
-            args = [pg.Point(*args)]
-        return pg.GraphicsObject.contains(self, *args)
-
-    def boundingRect(self):
-        return QtCore.QRectF(self.state['pos'].x(), self.state['pos'].y(), self.state['size'].x(), self.state['size'].y())
-
-
-class ROI_Base():
-    """ ROI_Base interface for all ROI types, template class for duplicate functions and functions to override.
-        connect window.closeEvent to ROI delete
-        set the window.currentROI to self
-
-    Attributes:
-        colorDialog: dialog for selecting the color of the ROI and its trace
-        traceWindow: the tracewindow that this ROI is plotted to, or None
-        mask: array of XY values that are contained within the ROI
-        pts: array of XY values used to copy the ROI
-        linkedROIs: set of rois that act as one ROI
-
-    Not Implemented Functions:
-        getMask()
-        getPoints()
-
-    Functions:
-        plot():
-            run the roiPlot function and link this window to the traceWindow
-            Returns the traceWindow
-        unplot():
-            Remove the roi from its traceWindow
-        link(roi):
-            add an roi to the linkedROIs set, so they translate together
-        colorSelected(QColor):
-            set the color of the roi
-        copy():
-            store the roi in the clipboard
-        paste():
-            Create an roi from the clipboard ROI using roi.getPoints()
-        delete():
-            unplot the ROI, remove the ROI from the window, clear it from the clipboard if it was copied, disconnect all signals
-        drawFinished():
-            add the ROI to the window, called by ROI_Drawing
-        str():
-            return kind and self.pts for recreating the ROI
-    """
-    INITIAL_ARGS = {'translateSnap': True, 'removable': True, 'snapSize': 1, 'scaleSnap': True}
-
-    def __init__(self, window, pts):
-        self.window = window
-        self.colorDialog=QtWidgets.QColorDialog()
-        self.colorDialog.colorSelected.connect(self.colorSelected)
-        self.window.closeSignal.connect(self.delete)
-        self.window.currentROI = self
-        self.traceWindow = None  # To test if roi is plotted, check if traceWindow is None
-        self.pts = np.array(pts)
-        self.linkedROIs = set()
-        self.resetSignals()
-        self.makeMenu()
-        self.mouseHovering = False
-        self.pen = None  # This is the permanent pen for the ROI.
-        self.currentPen = None  # This is the current, temporary pen.
-        self.set_ROI_pen()
-        self.drawFinished()
-
-    def set_ROI_pen(self, pen=None):
-        """ This should be called when permanently setting the pen. This doesn't need to be overwritten when the ROI has
-        components that need to be set individually. """
-        if pen is None:
-            color = QtGui.QColor(g.settings['roi_color']) if g.settings['roi_color'] != 'random' else random_color()
-            pen = QtGui.QPen(color)
-            pen.setWidth(0)
-        self.pen = pen
-        self.set_currentPen(pen)
-
-    def set_currentPen(self, pen):
-        """ This should be called when temporarily setting the pen. This needs to be overwritten when the ROI has
-        components that need to be set individually. """
-        self.currentPen = pen
-        self.setPen(self.currentPen)
-        self.update()
-
-    def paint(self, p, *args):
-        """ This is overwritten by most classes"""
-        pass
-
-    def setPen(self, pen):
-        """ This is overwritten by most classes"""
-        pass
-
-    def resetSignals(self):
-        try:
-            self.sigRegionChanged.disconnect()
-        except:
-            pass
-        try:
-            self.sigRegionChangeFinished.disconnect()
-        except:
-            pass
-        self.sigRegionChanged.connect(self.onRegionChange)
-        self.sigRegionChangeFinished.connect(self.onRegionChangeFinished)
-
-    def updateLinkedROIs(self, finish=False):
-        for roi in self.linkedROIs:
-            roi.blockSignals(True)
-            roi.draw_from_points(self.pts, finish=False)
-            if roi.traceWindow is not None:
-                if not finish:
-                    roi.traceWindow.translated(roi)
-                else:
-                    roi.traceWindow.translateFinished(roi)
-            roi.blockSignals(False)
-
-    def redraw_trace(self):
-        if self.traceWindow is not None:
-            self.traceWindow.translateFinished(self)
-
-    def getSnapPosition(self, *args, **kargs):
-        shift = pg.Point(.5, .5) if isinstance(self, (ROI_rect_line, )) else pg.Point(0, 0)
-        return pg.ROI.getSnapPosition(self, *args, **kargs) + shift
-
-    def onRegionChange(self):
-        self.pts = self.getPoints()
-        self.updateLinkedROIs(finish=False)
-        
-    def onRegionChangeFinished(self):
-        self.pts = self.getPoints()
-        self.updateLinkedROIs(finish=True)
-
-    def link(self,roi):
-        '''This function links this roi to another, so a translation of one will cause a translation of the other'''
-        if not isinstance(roi, type(self)):
-            return
-        join = self.linkedROIs | roi.linkedROIs | {self, roi}
-        self.linkedROIs = join - {self}
-        roi.linkedROIs = join - {roi}
-
-    def getMask(self):
-        '''
-        Returns the list of integer points contained within the ROI
-        '''
-        raise NotImplementedError()
-
-    def getTrace(self, bounds=None):
-        '''
-        Compute the average of the pixels within this ROI for the window of this ROI, return an array of average values, cropped by bounds
-        '''
-        trace = None
-        if self.window.image.ndim == 4 or self.window.metadata['is_rgb']:
-            g.alert("Plotting trace of RGB movies is not supported. Try splitting the channels.")
-            return None
-        s1, s2 = self.getMask()
-        if np.size(s1) == 0 or np.size(s2) == 0:
-            trace = np.zeros(self.window.mt)
-
-        elif self.window.image.ndim == 3:
-            trace = self.window.image[:, s1, s2]
-            while trace.ndim > 1:
-                trace = np.average(trace, 1)
-        elif self.window.image.ndim == 2:
-            trace = self.window.image[s1, s2]
-            trace = [np.average(trace)]
-
-        if bounds:
-            trace = trace[bounds[0]:bounds[1]]
-        return trace
-
-    def getPoints(self):
-        '''
-        return the points that represent this ROI. Used for exporting
-        '''
-        raise NotImplementedError()
-
-    def draw_from_points(self, pts, finish=True):
-        '''
-        Redraw the ROI from the given points, used on linked ROIs
-        '''
-        raise NotImplementedError()
-
-    def setMouseHover(self, hover):
-        """
-        Inform the ROI that the mouse is or is not hovering over it.
-
-        Args:
-            hover (bool)
-
-        """
-        if self.mouseHovering is hover:
-            return
-        self.mouseHovering = hover
-        if hover:
-            self.set_currentPen(QtGui.QPen(QtGui.QColor(255, 0, 0)))
-        else:
-            self.set_currentPen(self.pen)
-
-    def plot(self):
-        self.traceWindow = roiPlot(self)
-        if self.traceWindow == None:
-            return
-        self.traceWindow.indexChanged.connect(self.window.setIndex)
-        self.plotSignal.emit()
-        return self.traceWindow
-
-    def changeColor(self):
-        self.colorDialog.open()
-        
-    def colorSelected(self, color):
-        if color.isValid():
-            self.set_ROI_pen(QtGui.QPen(QtGui.QColor(color.name())))
-            self.sigRegionChangeFinished.emit(self)
-
-    def unplot(self):
-        try:
-            self.traceWindow.indexChanged.disconnect(self.window.setIndex)
-        except:
-            # sometimes errors, says signals not connected
-            pass
-        if self.traceWindow != None:
-            self.traceWindow.removeROI(self)
-            self.traceWindow = None
-
-    def copy(self):
-        g.clipboard=self
-
-    def raiseContextMenu(self, ev):
-        pos = ev.screenPos()
-        self.menu.addSeparator()
-        self.menu.addActions(self.window.menu.actions())
-        self.menu.popup(QtCore.QPoint(pos.x(), pos.y()))
-    
-    def makeMenu(self):
-        def plotPressed():
-            if plotAct.text() == "&Plot":
-                self.plot()
-            else:
-                self.unplot()
-
-        plotAct = QtWidgets.QAction("&Plot", self, triggered=plotPressed)
-        colorAct = QtWidgets.QAction("&Change Color",self,triggered=self.changeColor)
-        copyAct = QtWidgets.QAction("&Copy", self, triggered=self.copy)
-        remAct = QtWidgets.QAction("&Delete", self, triggered=self.delete)
-        self.menu = QtWidgets.QMenu("ROI Menu")
-
-        def updateMenu():
-            #plotAct.setEnabled(self.window.image.ndim > 2)
-            plotAct.setText("&Plot" if self.traceWindow == None else "&Unplot")
-            self.window.menu.aboutToShow.emit()
-
-        self.menu.addAction(plotAct)
-        self.menu.addAction(colorAct)
-        self.menu.addAction(copyAct)
-        self.menu.addAction(remAct)
-        self.menu.aboutToShow.connect(updateMenu)
-
-    def delete(self):
-        self.unplot()
-        for roi in self.linkedROIs:
-            if self in roi.linkedROIs:
-                roi.linkedROIs.remove(self)
-        if self in self.window.rois:
-            self.window.rois.remove(self)
-        self.window.currentROI=None
-        self.window.imageview.removeItem(self)
-        self.window.closeSignal.disconnect(self.delete)
-        if g.clipboard == self:
-            g.clipboard = None
-
-    def drawFinished(self):
-        self.window.imageview.addItem(self)
-        self.window.rois.append(self)
-        self.window.currentROI = self
-
-    def str(self):
-        s = self.kind + '\n'
-        for x, y in self.pts:
-            s += '{} {}\n'.format(x, y)
-        return s
-
-    def showMask(self):
-        from .window import Window
-        im = np.zeros_like(self.window.imageview.getImageItem().image)
-        s1, s2 = self.getMask()
-        im[s1, s2] = 1
-        return Window(im)
-
-
-class ROI_line(ROI_Base, pg.LineSegmentROI):
-    '''
-    ROI Line class for selecting a straight line of pixels between two points
-        Extends from the ROI_Base class and pyqtgraph ROI.LineSegmentROI
-    '''
-    kind = 'line'
-    plotSignal = QtCore.Signal()
-    
-    def __init__(self, window, positions, **kargs):
-        roiArgs = self.INITIAL_ARGS.copy()
-        roiArgs.update(kargs)
-        pg.LineSegmentROI.__init__(self, positions=positions, **roiArgs)
-        self.kymograph = None
-        self.kymographAct = QtWidgets.QAction("&Kymograph", self, triggered=self.update_kymograph)
-        ROI_Base.__init__(self, window, positions)
-
-    def paint(self, p, *args):
-        p.setRenderHint(QtGui.QPainter.Antialiasing)
-        p.setPen(self.currentPen)
-        h1 = self.handles[0]['item'].pos()
-        h2 = self.handles[1]['item'].pos()
-        p.drawLine(h1, h2)
-
-    def resetSignals(self):
-        ROI_Base.resetSignals(self)
-        self.sigRegionChanged.connect(self.snapPoints)
-
-    def snapPoints(self):
-        fix = False
-        self.blockSignals(True)
-        for handle in self.handles:
-            pos = handle['pos']
-            pos_snap = self.getSnapPosition(pg.Point(pos))# + pg.Point(.5, .5)
-            if not (pos == pos_snap):
-                handle['item'].setPos(pos_snap)
-                handle['pos'] = pos_snap
-                fix = True
-
-        self.blockSignals(False)
-        #if fix:
-        #    self.sigRegionChanged.emit(self)
-
-    def draw_from_points(self, pts, finish=True):
-        self.blockSignals(True)
-        self.movePoint(self.handles[0]['item'], pts[0], finish=False)
-        self.movePoint(self.handles[1]['item'], pts[1], finish=False)
-        self.pts = pts
-        self.blockSignals(False)
-        if finish:
-            self.sigRegionChangeFinished.emit(self)
-
-    def delete(self):
-        ROI_Base.delete(self)
-        if self.kymograph:
-            self.deleteKymograph()
-
-    def getMask(self):
-        x=np.array([p[0] for p in self.pts], dtype=int)
-        y=np.array([p[1] for p in self.pts], dtype=int)
-        xx, yy = line(x[0],y[0],x[1],y[1])
-        idx_to_keep = np.logical_not( (xx>=self.window.mx) | (xx<0) | (yy>=self.window.my) | (yy<0))
-        xx = xx[idx_to_keep]
-        yy = yy[idx_to_keep]
-        return xx, yy
-
-    def getPoints(self):
-        return np.array([handle['pos'] + self.state['pos'] for handle in self.handles])
-
-    def makeMenu(self):
-        ROI_Base.makeMenu(self)
-        self.menu.addAction(self.kymographAct)
-        self.kymographAct.setEnabled(self.window.image.ndim == 3 and not self.window.metadata['is_rgb'])
-
-    def update_kymograph(self):
-        tif=self.window.image
-        if tif.ndim != 3:
-            g.alert("Can only kymograph a 3d movie")
-            return
-
-        xx, yy = self.getMask()
-        mt = len(tif)
-        if len(xx) == 0:
-            return
-        xx = np.array(xx)
-        yy = np.array(yy)
-        
-        if len(xx) == 0:
-            return
-        mn=np.zeros((mt,len(xx)))
-        for t in np.arange(mt):
-            mn[t]=tif[t,xx,yy]
-        mn=mn.T
-        if self.kymograph is None:
-            self.createKymograph(mn)
-        else:
-            self.kymograph.imageview.setImage(mn,autoLevels=False,autoRange=False)
-            #self.kymograph.imageview.view.setAspectLocked(lock=True,ratio=mn.shape[1]/mn.shape[0])
-    
-    def createKymograph(self,mn):
-        from .window import Window
-        oldwindow=g.currentWindow
-        name=oldwindow.name+' - Kymograph'
-        self.kymograph=Window(mn,name,metadata=self.window.metadata)
-        self.sigRegionChanged.connect(self.update_kymograph)
-        self.kymograph.closeSignal.connect(self.deleteKymograph)
-        self.sigRemoveRequested.connect(self.deleteKymograph)
-
-    def deleteKymograph(self):
-        self.kymograph.closeSignal.disconnect(self.deleteKymograph)
-        self.kymograph=None
-
-
-class ROI_rectangle(ROI_Base, pg.ROI):
-    '''
-    ROI rectangle class for selecting a set width and height group of pixels on an image
-        Extends from pyqtgraph ROI and ROI_Base
-
-    Parameters:
-        window: parent window to draw the ROI in
-        pos: XY coordinate of the upper left corner of the rectangle
-        size: (width, height) tuple of the ROI
-        resizable: scale handles will be drawn on each corner if this is True
-        See pg.ROI for other parameters
-
-    Functions:
-        crop():
-            create a new window with the original image cropped within this ROI
-    '''
-    kind = 'rectangle'
-    plotSignal = QtCore.Signal()
-
-    def __init__(self, window, pos, size, resizable=True, **kargs):
-        roiArgs = self.INITIAL_ARGS.copy()
-        roiArgs.update(kargs)
-        pos = np.array(pos, dtype=int)
-        size = np.array(size, dtype=int)
-
-        pg.ROI.__init__(self, pos, size, **roiArgs)
-        if resizable:
-            self.addScaleHandle([0, 1], [1, 0])
-            self.addScaleHandle([1, 0], [0, 1])
-            self.addScaleHandle([0, 0], [1, 1])
-            self.addScaleHandle([1, 1], [0, 0])
-        self.cropAction = QtWidgets.QAction('&Crop', self, triggered=self.crop)
-        ROI_Base.__init__(self, window, [pos, size])
-
-    def center_around(self, x, y):
-        old_pts = self.getPoints()
-        old_center = old_pts[0] + .5 * old_pts[1]
-        new_center = np.array([x, y])
-        diff = new_center - old_center
-        new_pts = np.array([old_pts[0]+diff, old_pts[1]])
-        self.draw_from_points(new_pts)
-
-    def getPoints(self):
-        return np.array([self.state['pos'], self.state['size']], dtype=int)
-
-    def contains_pts(self, x, y):
-        target = np.array([x, y])
-        return np.all(self.pts[0] < target) and np.all(target < self.pts[0]+self.pts[1])
-
-    def getMask(self):
-        x, y = self.state['pos']
-        w, h = self.state['size']
-
-        xmin = max(x, 0)
-        ymin = max(y, 0)
-        xmax = min(x+w, self.window.mx)
-        ymax = min(y+h, self.window.my)
-
-        xx, yy = np.meshgrid(np.arange(xmin, xmax, dtype=int), np.arange(ymin, ymax, dtype=int))
-
-        return xx.flatten(), yy.flatten()
-
-    def paint(self, p, *args):
-        pg.ROI.paint(self, p, *args)
-
-    def draw_from_points(self, pts, finish=True):
-        self.setPos(pts[0], finish=False)
-        self.setSize(pts[1], finish=False)
-        self.pts = np.array(pts)
-        if finish:
-            self.sigRegionChangeFinished.emit(self)
-
-    def makeMenu(self):
-        ROI_Base.makeMenu(self)
-        self.menu.addAction(self.cropAction)
-
-    def crop(self):
-        from .window import Window
-        r = self.boundingRect()
-        p1 = r.topLeft() + self.state['pos']
-        p2 = r.bottomRight() + self.state['pos']
-        x1, y1 = int(p1.x()), int(p1.y())
-        x2, y2 = int(p2.x()), int(p2.y())
-
-        tif=self.window.image
-        if tif.ndim==3:
-            mt,mx,my=tif.shape
-            if x1<0: x1=0
-            if y1<0: y1=0
-            if x2>=mx: x2=mx-1
-            if y2>=my: y2=my-1
-            newtif=tif[:,x1:x2,y1:y2]
-        elif tif.ndim==2:
-            mx,my=tif.shape
-            if x1<0: x1=0
-            if y1<0: y1=0
-            if x2>=mx: x2=mx-1
-            if y2>=my: y2=my-1
-            mx,my=tif.shape
-            newtif=tif[x1:x2,y1:y2]
-        elif tif.ndim==4:
-            mt,mx,my,mc=tif.shape
-            if x1<0: x1=0
-            if y1<0: y1=0
-            if x2>=mx: x2=mx-1
-            if y2>=my: y2=my-1
-            newtif=tif[:,x1:x2,y1:y2]
-        else:
-            g.alert("Image dimensions not understood")
-            return None
-        return Window(newtif,self.window.name+' Cropped',metadata=self.window.metadata)
-
-
-class ROI_freehand(ROI_Base, pg.PolyLineROI):
-    kind = 'freehand'
-    plotSignal = QtCore.Signal()
-    def __init__(self, window, pts, **kargs):
-        roiArgs = self.INITIAL_ARGS.copy()
-        roiArgs.update(kargs)
-        roiArgs['closed'] = True
-        self.pen = None
-        pg.PolyLineROI.__init__(self, pts, **roiArgs)
-        ROI_Base.__init__(self, window, pts)
-        self._untranslated_mask = None
-
-    def draw_from_points(self, pts, finish=False):
-        return
-        self.blockSignals(True)
-        self.setPoints([pg.Point(p) for p in pts], closed=True)
-        self.blockSignals(False)
-
-    def set_currentPen(self, pen):
-        super(ROI_freehand, self).set_currentPen(pen)
-        for seg in self.segments:
-            seg.setPen(self.currentPen)
-
-    def translate(self, pos, y=None, *args, **kargs):
-        if y is None:
-            pos = pg.Point(pos)
-        else:
-            # avoid ambiguity where update is provided as a positional argument
-            if isinstance(y, bool):
-                raise TypeError("Positional arguments to setPos() must be numerical.")
-            pos = pg.Point(pos, y)
-
-
-        pos = self.getSnapPosition(pos) 
-        pg.PolyLineROI.translate(self, pos, *args, **kargs)
-        for roi in self.linkedROIs:
-            roi.blockSignals(True)
-            roi.setPos(roi.state['pos'] + pos)
-            roi.pts = roi.getPoints()
-            roi.blockSignals(False)
-
-    def getPoints(self):
-        return np.array([h.pos() + self.state['pos'] for h in self.getHandles()], dtype=int)
-
-    def removeSegment(self, seg):
-        for handle in seg.handles[:]:
-            seg.removeHandle(handle['item'])
-        self.segments.remove(seg)
-        self.scene().removeItem(seg)
-
-    def addSegment(self, h1, h2, index=None):
-        seg = pg.LineSegmentROI(handles=(h1, h2), pen=self.pen, parent=self, movable=False)
-        if index is None:
-            self.segments.append(seg)
-        else:
-            self.segments.insert(index, seg)
-        seg.setAcceptedMouseButtons(QtCore.Qt.LeftButton)
-        seg.setZValue(self.zValue()+1)
-        seg.setMouseHover = self.setMouseHover
-        for h in seg.handles:
-            h['item'].setAcceptedMouseButtons(h['item'].acceptedMouseButtons() | QtCore.Qt.LeftButton) ## have these handles take left clicks too, so that handles cannot be added on top of other handles
-            h['item'].setOpacity(0)
-
-    def getMask(self):
-        if self._untranslated_mask is not None:
-            xx = self._untranslated_mask[0] + int(self.state['pos'][0])
-            yy = self._untranslated_mask[1] + int(self.state['pos'][1])
-        else:
-            x, y = np.transpose(self.pts)
-            mask=np.zeros(self.window.imageDimensions())
-            xx,yy=polygon(x,y,shape=mask.shape)
-            self._untranslated_mask = xx, yy
-
-        idx_to_keep = np.logical_not( (xx>=self.window.mx) | (xx<0) | (yy>=self.window.my) | (yy<0))
-        xx = xx[idx_to_keep]
-        yy = yy[idx_to_keep]
-        return xx, yy
-
-
-class ROI_rect_line(ROI_Base, QtWidgets.QGraphicsObject):
-    """
-    This ROI is a line with an adjustable width that can be composed of multiple straight line segments.
-    """
-    kind = 'rect_line'
-    plotSignal = QtCore.Signal()
-    sigRegionChanged = QtCore.Signal(object)
-    sigRegionChangeFinished = QtCore.Signal(object)
-
-    def __init__(self, window, pts, width=1, **kargs):
-        self.roiArgs = self.INITIAL_ARGS.copy()
-        self.roiArgs.update(kargs)
-        self.roiArgs['scaleSnap'] = False
-        self.width = width
-        self.currentLine = None
-        self.kymograph = None
-        QtWidgets.QGraphicsObject.__init__(self)
-        self.kymographAct = QtWidgets.QAction("&Kymograph", self, triggered=self.update_kymograph)
-        self.removeLinkAction = QtWidgets.QAction('Remove Last Link', self, triggered=self.removeSegment)
-        self.setWidthAction = QtWidgets.QAction("Set Width", self, triggered=lambda: self.setWidth())
-        self.lines = []
-        ROI_Base.__init__(self, window, pts)
-        self.getPoints = self.getHandlePositions
-        self.pen = QtGui.QPen(QtGui.QColor(255, 255, 0))
-        self.pen.setWidth(0)
-        if len(pts) < 2:
-            raise Exception("Must start with at least 2 points")
-        print('ROI_rect_line self.pts at drawFinished: {}'.format(pts))
-        self.addSegment(pts[1], connectTo=pts[0])
-        for p in pts[2:]:
-            self.addSegment(p)
-        self.extending = False
-
-    def delete(self):
-        ROI_Base.delete(self)
-        if self.kymograph:
-            self.deleteKymograph()
-
-    def draw_from_points(self, pts, finish=False):
-        while len(self.lines) > 1:
-            self.removeSegment(self.lines[-1])
-
-        self.lines[0].movePoint(0, pts[0])
-        self.lines[0].movePoint(1, pts[1])
-        for p in pts[2:]:
-            self.addSegment(p)
-
-        if finish:
-            self.sigRegionChangeFinished.emit(self)
-        self.pts = pts
-
-    def getTrace(self, bounds=None):
-        if self.window.image.ndim > 3 or self.window.metadata['is_rgb']:
-            g.alert("Plotting trace of RGB movies is not supported. Try splitting the channels.")
-            return None
-        if self.window.image.ndim == 3:
-            region = self.getArrayRegion(self.window.imageview.image, self.window.imageview.getImageItem(), (1, 2))
-            while region.ndim > 1:
-                region = np.average(region, 1)
-        elif self.window.image.ndim == 2:
-            region = self.getArrayRegion(self.window.imageview.image, self.window.imageview.getImageItem(), (0, 1))
-            region = np.average(region)
-
-        if bounds:
-            region = region[bounds[0]:bounds[1]]
-        return region
-
-    def preview(self):
-        im = self.getArrayRegion(self.window.imageview.getImageItem().image, self.window.imageview.getImageItem(), (0, 1))
-        if not hasattr(self, 'prev'):
-            from .window import Window
-            self.prev = Window(im)
-            self.sigRegionChanged.connect(lambda a: self.preview())
-        else:
-            self.prev.imageview.setImage(im)
-
-    def lineRegionChange(self, line):
-        print('lineRegionChange')
-        line.blockSignals(True)
-        for i in range(2):
-            p = self.mapFromScene(line.getHandles()[i].scenePos())
-            p = line.getSnapPosition([p.x(), p.y()])
-            if line.getHandles()[i].isMoving:
-                line.movePoint(i, p)
-        line.blockSignals(False)
-        self.pts = self.getPoints()
-        self.sigRegionChanged.emit(self)
-
-    def getHandlePositions(self):
-        """Return the positions of all handles in local coordinates."""
-        print("getHandlePositions")
-        return None
-        p = self.mapFromScene(self.lines[0].getHandles()[0].scenePos())
-        p = self.lines[0].getSnapPosition([p.x(), p.y()])
-        pos = [p]
-        for l in self.lines:
-            p = self.mapFromScene(l.getHandles()[1].scenePos())
-            p = l.getSnapPosition([p.x(), p.y()])
-            pos.append(p)
-        self.pts = pos
-        return self.pts
-        
-    def getArrayRegion(self, arr, img=None, axes=(0,1), **kwds):
-        rgns = []
-        for l in self.lines:
-            rgn = l.getArrayRegion(arr, img, axes=axes, **kwds)
-            if rgn is None:
-                continue
-                #return None
-            rgns.append(rgn)
-            #print l.state['size']
-            
-        ## make sure orthogonal axis is the same size
-        ## (sometimes fp errors cause differences)
-        if img.axisOrder == 'row-major':
-            axes = axes[::-1]
-        ms = min([r.shape[axes[1]] for r in rgns])
-        sl = [slice(None)] * rgns[0].ndim
-        sl[axes[1]] = slice(0,ms)
-        rgns = [r[sl] for r in rgns]
-        #print [r.shape for r in rgns], axes
-        
-        return np.concatenate(rgns, axis=axes[0])
-        
-    def addSegment(self, pos=(0, 0), connectTo=None):
-        """
-        Add a new segment to the ROI connecting from the previous endpoint to *pos*.
-        (pos is specified in the parent coordinate system of the MultiRectROI)
-        """
-        ## by default, connect to the previous endpoint
-        if connectTo is None:
-            connectTo = self.lines[-1].getHandles()[1]
-            
-        ## create new ROI
-        newRoi = pg.ROI((0,0), [1, self.width], parent=self, pen=self.pen, **self.roiArgs)
-        self.lines.append(newRoi)
-        
-        ## Add first SR handle
-        if isinstance(connectTo, Handle):
-            h = self.lines[-1].addScaleRotateHandle([0, 0.5], [1, 0.5], item=connectTo)
-            newRoi.movePoint(connectTo, connectTo.scenePos(), coords='scene')
-        else:
-            h = self.lines[-1].addScaleRotateHandle([0, 0.5], [1, 0.5])
-            newRoi.movePoint(h, connectTo, coords='scene')
-            
-        ## add second SR handle
-        h = self.lines[-1].addScaleRotateHandle([1, 0.5], [0, 0.5]) 
-        newRoi.movePoint(h, pos)
-            
-        newRoi.translatable = False
-        newRoi.hoverEvent = lambda e: self.hoverEvent(newRoi, e)
-        newRoi.sigRegionChanged.connect(self.lineRegionChange)
-        newRoi.raiseContextMenu = self.raiseContextMenu
-        #newRoi.sigRegionChangeStarted.connect(self.roiChangeStartedEvent) 
-        newRoi.sigRegionChangeFinished.connect( lambda a: self.sigRegionChangeFinished.emit(self))
-        self.sigRegionChanged.emit(self)
-
-    def getNearestHandle(self, pos, max_distance=None):
-        h = None
-        d = max_distance
-        for l in self.lines:
-            for i in range(2):
-                p = self.window.imageview.getImageItem().mapFromScene(l.getSceneHandlePositions(i)[1])
-                d = pg.Point(p - pos).manhattanLength()
-                if max_distance == None:
-                    if h == None or d < dist:
-                        h = l.handles[i]['item']
-                        dist = d
-                else:
-                    if d <= dist:
-                        h = l.handles[i]['item']
-                        dist = d
-        return h
-
-    def removeSegment(self, segment=None): 
-        """Remove a segment from the ROI."""
-        if isinstance(segment, int):
-            segment = self.lines[segment]
-
-        if not isinstance(segment, pg.ROI):
-            segment = self.currentLine
-        
-        for h in segment.getHandles():
-            if len(h.rois) == 2 and h.parentItem() == segment:
-                otherROI = [line for line in h.rois if line != segment][0]
-                h.setParentItem(otherROI)
-                h.setPos(0, .5)
-            h.disconnectROI(segment)
-        if segment in self.lines:
-            self.lines.remove(segment)
-
-        self.scene().removeItem(segment)
-        segment.sigRegionChanged.disconnect() 
-        segment.sigRegionChangeFinished.disconnect()
-        if len(self.lines) == 0:
-            self.delete()
-        else:
-            self.sigRegionChanged.emit(self)
-
-    def extend(self, x, y, finish=True):
-        point = self.lines[0].getSnapPosition([x, y])
-        if not self.extending:
-            h = self.getNearestHandle(pg.Point(x, y))
-            if h is not None and len(h.rois) > 1:
-                return
-            self.extending = True
-            self.addSegment(point, connectTo=h)
-        else:
-            self.lines[-1].handles[-1]['item'].movePoint(self.window.imageview.getImageItem().mapToScene(point))
-        self.sigRegionChanged.emit(self)
-        if finish:
-            self.sigRegionChangeFinished.emit(self)
-
-    def extendFinished(self):
-        self.extending = False
-        self.extendHandle = None
-        self.sigRegionChangeFinished.emit(self)
-        if self.lines[0].getHandles()[0] in self.lines[-1].getHandles():
-            self.lines.insert(0, self.lines[-1])
-            self.lines = self.lines[:-1]
-            self.lines[0].handles = self.lines[0].handles[::-1]
-
-    def hoverEvent(self, l, ev):
-        self.currentLine = l
-        if ev.enter:
-            pen = QtGui.QPen(QtGui.QColor(255, 0, 0))
-            pen.setWidth(0)
-            self.set_currentPen(pen)
-        elif ev.exit:
-            self.set_currentPen(self.pen)
-
-    def getMask(self):
-        print('getMask')
-        xxs = []
-        yys = []
-        for i in range(len(self.pts)-1):
-            p1, p2 = self.pts[i], self.pts[i+1]
-            xx, yy = line(int(p1[0]), int(p1[1]), int(p2[0]), int(p2[1]))
-            idx_to_keep = np.logical_not( (xx>=self.window.mx) | (xx<0) | (yy>=self.window.my) | (yy<0))
-            xx = xx[idx_to_keep]
-            yy = yy[idx_to_keep]
-            xxs.extend(xx)
-            yys.extend(yy)
-
-        return np.array(xxs, dtype=int), np.array(yys, dtype=int)
-
-    def makeMenu(self):
-        ROI_Base.makeMenu(self)
-        self.menu.addAction(self.removeLinkAction)
-        self.menu.addAction(self.setWidthAction)
-        self.menu.addAction(self.kymographAct)
-        self.kymographAct.setEnabled(self.window.image.ndim > 2)
-
-    def raiseContextMenu(self, ev):
-        if np.any([len(i.rois)<2 for i in self.currentLine.getHandles()]):
-            self.removeLinkAction.setText("Remove Link")
-            self.removeLinkAction.setVisible(True)
-        else:
-            self.removeLinkAction.setVisible(False)
-        
-        ROI_Base.raiseContextMenu(self, ev)
-
-    def boundingRect(self):
-        return QtCore.QRectF()
-
-    def set_currentPen(self, pen):
-        super(ROI_rect_line, self).set_currentPen(pen)
-        for line in self.lines:
-            line.setPen(pen)
-
-    def update_kymograph(self):
-        tif=self.window.image
-        if tif.ndim != 3:
-            g.alert("Can only kymograph on 3D movies")
-            return
-        
-        if self.width == 1:
-            w, h = self.window.imageDimensions()
-            r = QtCore.QRect(0, 0, w, h)
-            xx, yy = self.getMask()
-            mn = tif[:, xx, yy].T
-        else:
-            region = self.getArrayRegion(self.window.imageview.image, self.window.imageview.getImageItem(), (1, 2))
-            mn = np.average(region, 2).T
-
-
-        if self.kymograph is None:
-            self.createKymograph(mn)
-        else:
-            if mn.size > 0:
-                self.kymograph.imageview.setImage(mn,autoLevels=False,autoRange=False)
-            #self.kymograph.imageview.view.setAspectLocked(lock=True,ratio=mn.shape[1]/mn.shape[0])
-
-    def setWidth(self, newWidth=None):
-        s = True
-        if newWidth == None:
-            newWidth, s = QtWidgets.QInputDialog.getInt(None, "Enter a width value", 'Float Value', value = self.width)
-        if not s or s == 0:
-            return
-        for l in self.lines:
-            l.scale([1.0, newWidth/self.width], center=[0.5,0.5])
-        self.width = newWidth
-        self.sigRegionChangeFinished.emit(self)
-
-    def createKymograph(self,mn):
-        from .window import Window
-        oldwindow=g.currentWindow
-        name=oldwindow.name+' - Kymograph'
-        self.kymograph=Window(mn,name,metadata=self.window.metadata)
-        self.kymographproxy = pg.SignalProxy(self.sigRegionChanged, rateLimit=1, slot=self.update_kymograph) #This will only update 3 Hz
-        self.sigRegionChanged.connect(self.update_kymograph)
-        self.kymograph.closeSignal.connect(self.deleteKymograph)
-
-    def deleteKymograph(self):
-        self.kymographproxy.disconnect()
-        self.kymograph.closeSignal.disconnect(self.deleteKymograph)
-        self.kymograph=None
-
-
-def makeROI(kind, pts, window=None, **kargs):
-    if window is None:
-        window = g.currentWindow
-        if window is None:
-            g.alert('ERROR: In order to make and ROI a window needs to be selected')
-            return None
-    if kind == 'freehand':
-        if len(pts) < 4:
-            return None
-        roi = ROI_freehand(window, pts, **kargs)
-    elif kind == 'rectangle':
-        if len(pts) > 2:
-            size = np.ptp(pts,0)
-            top_left = np.min(pts,0)
-        else:
-            size = pts[1]
-            top_left = pts[0]
-        roi=ROI_rectangle(window, top_left, size, **kargs)
-    elif kind == 'line':
-        roi = ROI_line(window, (pts), **kargs)
-    elif kind == 'rect_line':
-        roi = ROI_rect_line(window, pts, **kargs)
-    else:
-        g.alert("ERROR: THIS KIND OF ROI COULD NOT BE FOUND: {}".format(kind))
-        return None
-    return roi
-
-
-def open_rois(filename=None):
-    """
-    Open an roi.txt file, creates ROI objects and places them in the current Window.
-    
-    Args:
-        filename (str): The filename (including full path) of the roi.txt file.
-
-    Returns:
-        list of rois
-
-
-    """
-    if filename is None:
-        filetypes = '*.txt'
-        prompt = 'Load ROIs from file'
-        filename = open_file_gui(prompt, filetypes=filetypes)
-        if filename is None:
-            return None
-    text = open(filename, 'r').read()
-    rois = []
-    kind = None
-    pts = None
-    for text_line in text.split('\n'):
-        if kind is None:
-            kind = text_line
-            pts = []
-        elif text_line == '':
-            roi = makeROI(kind,pts)
-            rois.append(roi)
-            kind = None
-            pts = None
-        else:
-            pts.append(tuple(int(float(i)) for i in text_line.split()))
-
-    return rois
+# -*- coding: utf-8 -*-
+"""This module declares Region Of Interest (ROI) types as extensions of pyqtgraph.ROI objects.
+
+Current ROI types are:
+    * line
+    * rectangle
+    * freehand
+    * rect_line
+
+Example:
+    >>> roi = makeROI('line', [[10, 10], [20, 15]])
+    >>> roi.plot()
+    >>> roi.copy()
+    >>> win2 = open_file()
+    >>> roi2 = win2.paste()
+
+Todo:
+    * Correct ROI line handles to be at center of pixel
+"""
+from .logger import logger
+logger.debug("Started 'reading roi.py'")
+import os
+from qtpy import QtGui, QtCore, QtWidgets
+import pyqtgraph as pg
+import numpy as np
+from pyqtgraph.graphicsItems.ROI import Handle
+from . import global_vars as g
+from .utils.misc import random_color, open_file_gui, nonpartial
+
+
+class ROI_Drawing(pg.GraphicsObject):
+    """Graphics Object for ROIs while initially being drawn. Extends pyqtrgaph.GraphicsObject
+
+    Only used on initial mouse drag, the drawFinished method returns the
+    resulting ROI object which can then be modified
+
+    Attributes:
+        window (window.Window): Window object to draw the ROI in
+        x (int): x coordinate of mouse press
+        y (int): y coordinate of mouse press
+        kind (str): one of ['rectangle', 'line', 'freehand', 'rect_line']
+        color (QtGui.QColor): pen color to draw ROI with
+    """
+    def __init__(self, window, x, y, kind):
+        pg.GraphicsObject.__init__(self)
+        window.imageview.addItem(self)
+        self.window = window
+        self.pts = [pg.Point(round(x), round(y))]
+        self.kind = kind
+        self.state = {'pos': pg.Point(x, y), 'size': pg.Point(0, 0)}
+        self.color = QtGui.QColor(g.settings['roi_color']) if g.settings['roi_color'] != 'random' else random_color()
+
+    def cancel(self):
+        g.win.imageview.removeItem(self)
+        g.win.currentROI = None
+        self.deleteLater()
+
+    def extend(self, x, y):
+        new_pt = pg.Point(round(x), round(y))
+        if self.kind == 'freehand':
+            if self.pts[-1] != new_pt:
+                self.pts.append(new_pt)
+        elif self.kind in ('line', 'rectangle', 'rect_line'):
+            if len(self.pts) == 1:
+                self.pts.append(new_pt)
+            else:
+                self.pts[1] = new_pt
+
+            #self.pts = sorted(self.pts, key=lambda a: a.x()/a.y())
+
+        self.state['pos'] = pg.Point(*np.min(self.pts, 0))
+        self.state['size'] = pg.Point(*np.ptp(self.pts, 0))
+
+        self.prepareGeometryChange()
+        self.update()
+
+    def paint(self, p, *args):
+        pen = QtGui.QPen(self.color)
+        pen.setWidth(0)
+        p.setPen(pen)
+        if self.kind == 'freehand':
+            p.drawPolyline(*self.pts)
+        elif self.kind == 'rectangle':
+            p.drawRect(self.boundingRect())
+        elif self.kind in ('rect_line', 'line'):
+            p.drawLine(*self.pts)
+
+    def drawFinished(self):
+        self.window.imageview.removeItem(self)
+        if self.kind == 'rectangle':
+            pts = [self.state['pos'], self.state['size']]
+        else:
+            pts = self.pts
+        return makeROI(self.kind, pts, self.window, color=self.color)
+
+
+    def contains(self, *args):
+        if len(args) == 2:
+            args = [pg.Point(*args)]
+        return pg.GraphicsObject.contains(self, *args)
+
+    def boundingRect(self):
+        return QtCore.QRectF(self.state['pos'].x(), self.state['pos'].y(), self.state['size'].x(), self.state['size'].y())
+
+class ROI_Base():
+    """ROI_Base interface for all ROI types
+
+    Template class for common and abstract functions, connects window.closeEvent to pyqtgraph.ROI.delete, set the window.currentROI to self
+
+    Attributes:
+        colorDialog: dialog for selecting the color of the ROI and its trace
+        traceWindow: the :class:`TraceFig <flika.tracefig.TraceFig>` that this ROI is plotted to, or None
+        pts: array of XY values used to copy the ROI
+        linkedROIs: set of rois that act as one ROI
+
+    Note:
+        All ROI objects implement the following methods:
+            getMask():
+                returns the [2, N] array of mask coordinates
+            getPoints():
+                returns the [N, 2] points that make up the ROI   
+            draw_from_points(pts, finish=True):
+                updates the point locations that make the ROI, used in linked ROIs
+
+    """
+    INITIAL_ARGS = {'translateSnap': True, 'removable': True, 'snapSize': 1, 'scaleSnap': True}
+
+    def __init__(self, window, pts):
+        self.window = window #: window.Window: Parent window that this ROI belongs to
+        self.colorDialog=QtWidgets.QColorDialog()
+        self.colorDialog.colorSelected.connect(self.colorSelected)
+        self.window.closeSignal.connect(self.delete)
+        self.window.currentROI = self
+        self.traceWindow = None  #: tracefig.TraceFig: the Trace window that this ROI is plotted in. To test if roi is plotted, check 'roi.traceWindow is None'
+        self.pts = np.array(pts) #: list: Array of points that make up the boundary of the ROI
+        self.linkedROIs = set()
+        self.resetSignals()
+        self.makeMenu()
+
+    def mouseClickEvent(self, ev):
+        self.window.currentROI = self
+        super().mouseClickEvent(ev)
+
+    def resetSignals(self):
+        try:
+            self.sigRegionChanged.disconnect()
+        except:
+            pass
+        try:
+            self.sigRegionChangeFinished.disconnect()
+        except:
+            pass
+        self.sigRegionChanged.connect(self.onRegionChange)
+        self.sigRegionChangeFinished.connect(self.onRegionChangeFinished)
+
+    def updateLinkedROIs(self, finish=False):
+        for roi in self.linkedROIs:
+            roi.blockSignals(True)
+            roi.draw_from_points(self.pts, finish=False)
+            if roi.traceWindow is not None:
+                if not finish:
+                    roi.traceWindow.translated(roi)
+                else:
+                    roi.traceWindow.translateFinished(roi)
+            roi.blockSignals(False)
+
+    def redraw_trace(self):
+        """Emit the translateFinished signal which redraws the ROI trace
+        """
+        if self.traceWindow is not None:
+            self.traceWindow.translateFinished(self)
+
+    def onRegionChange(self):
+        self.pts = self.getPoints()
+        self.updateLinkedROIs(finish=False)
+        
+    def onRegionChangeFinished(self):
+        self.pts = self.getPoints()
+        self.updateLinkedROIs(finish=True)
+
+    def link(self,roi):
+        '''Link this roi to another, so a translation of one will cause a translation of the other'''
+        if not isinstance(roi, type(self)):
+            return
+        join = self.linkedROIs | roi.linkedROIs | {self, roi}
+        self.linkedROIs = join - {self}
+        roi.linkedROIs = join - {roi}
+
+    def getMask(self):
+        '''Returns the list of integer points contained within the ROI, differs by ROI type
+        '''
+        raise NotImplementedError()
+
+    def getTrace(self, bounds=None):
+        '''Compute the average of the pixels within this ROI in its window
+
+        Returns:
+            Average value within ROI mask, as an array. Cropped to bounds if specified
+        '''
+        trace = None
+        if self.window.image.ndim == 4 or self.window.metadata['is_rgb']:
+            g.alert("Plotting trace of RGB movies is not supported. Try splitting the channels.")
+            return None
+        s1, s2 = self.getMask()
+        if np.size(s1) == 0 or np.size(s2) == 0:
+            trace = np.zeros(self.window.mt)
+
+        elif self.window.image.ndim == 3:
+            trace = self.window.image[:, s1, s2]
+            while trace.ndim > 1:
+                trace = np.average(trace, 1)
+        elif self.window.image.ndim == 2:
+            trace = self.window.image[s1, s2]
+            trace = [np.average(trace)]
+
+        if bounds:
+            trace = trace[bounds[0]:bounds[1]]
+        return trace
+
+    def getPoints(self):
+        '''Get points that represent this ROI, used for exporting
+        '''
+        raise NotImplementedError()
+
+    def draw_from_points(self, pts, finish=True):
+        '''Redraw the ROI from the given points, used on linked ROIs
+
+        Args:
+            pts: points used to represent ROI, often handle positions
+            finish: whether or not to emit the onRegionChangeFinished signal
+        '''
+        raise NotImplementedError()
+
+    def setMouseHover(self, hover):
+        """
+        Inform the ROI that the mouse is or is not hovering over it.
+
+        Args:
+            hover (bool)
+
+        """
+        if self.mouseHovering is hover:
+            return
+        self.mouseHovering = hover
+        if hover:
+            self.currentPen = pg.mkPen(QtGui.QColor(255, 0, 0))
+        else:
+            self.currentPen = self.pen
+
+        self.update()
+
+    def plot(self):
+        """Plot the ROI trace in a :class:`TraceFig <flika.tracefig.TraceFig>`
+
+        Returns:
+            tracefig.TraceFig: the trace window that the ROI was plotted to
+        """
+        from .tracefig import roiPlot
+        self.traceWindow = roiPlot(self)
+        if self.traceWindow == None:
+            return
+        self.traceWindow.indexChanged.connect(self.window.setIndex)
+        self.plotSignal.emit()
+        return self.traceWindow
+
+    def changeColor(self):
+        self.colorDialog.open()
+        
+    def colorSelected(self, color):
+        """Set the pen color of the ROI
+
+        Args:
+            color (QtGui.QColor): new color for the ROI
+        """
+        if color.isValid():
+            self.setPen(QtGui.QColor(color.name()))
+            self.sigRegionChangeFinished.emit(self)
+
+    def unplot(self):
+        """Remove the ROI from its :class:`TraceFig <flika.tracefig.TraceFig>`
+        """
+        try:
+            self.traceWindow.indexChanged.disconnect(self.window.setIndex)
+        except:
+            # sometimes errors, says signals not connected
+            pass
+        if self.traceWindow != None:
+            self.traceWindow.removeROI(self)
+        
+        self.traceWindow = None
+
+    def copy(self):
+        """Store this ROI in the clipboard
+        """
+        g.clipboard=self
+
+    def raiseContextMenu(self, ev):
+        pos = ev.screenPos()
+        x = int(pos.x())
+        y = int(pos.y())
+        self.menu.addSeparator()
+        self.menu.addActions(self.window.menu.actions())
+        self.menu.popup(QtCore.QPoint(x, y))
+    
+    def makeMenu(self):
+        def plotPressed():
+            if plotAct.text() == "&Plot":
+                self.plot()
+            else:
+                self.unplot()
+
+        plotAct = QtWidgets.QAction("&Plot", self, triggered=plotPressed)
+        colorAct = QtWidgets.QAction("&Change Color",self,triggered=self.changeColor)
+        copyAct = QtWidgets.QAction("&Copy", self, triggered=self.copy)
+        remAct = QtWidgets.QAction("&Delete", self, triggered=self.delete)
+        self.menu = QtWidgets.QMenu("ROI Menu")
+
+        def updateMenu():
+            #plotAct.setEnabled(self.window.image.ndim > 2)
+            plotAct.setText("&Plot" if self.traceWindow == None else "&Unplot")
+            self.window.menu.aboutToShow.emit()
+
+        self.menu.addAction(plotAct)
+        self.menu.addAction(colorAct)
+        self.menu.addAction(copyAct)
+        self.menu.addAction(remAct)
+        self.menu.aboutToShow.connect(updateMenu)
+
+    def delete(self):
+        """Remove the ROI from its window, unlink all ROIs and delete the object"""
+        self.unplot()
+        for roi in self.linkedROIs:
+            if self in roi.linkedROIs:
+                roi.linkedROIs.remove(self)
+        if self in self.window.rois:
+            self.window.rois.remove(self)
+        self.window.currentROI=None
+        self.window.imageview.removeItem(self)
+        self.window.closeSignal.disconnect(self.delete)
+        if g.clipboard == self:
+            g.clipboard = None
+
+    def drawFinished(self):
+        self.window.imageview.addItem(self)
+        self.window.rois.append(self)
+        self.window.currentROI = self
+
+    def _str(self):
+        """Return ROI kind and points for easy export and import
+    
+        Returns:
+            str: ROI string representation
+        """
+        s = self.kind + '\n'
+        for x, y in self.pts:
+            s += '{} {}\n'.format(x, y)
+        return s
+
+    def showMask(self):
+        """Create a new binary window that visualizes the ROI mask
+
+        Returns:
+            window.Window: created mask window
+        """
+        from .window import Window
+        self.copy()
+        im = np.zeros_like(self.window.imageview.getImageItem().image)
+        s1, s2 = self.getMask()
+        im[s1, s2] = 1
+        w = Window(im)
+        w.paste()
+        return w
+
+
+class ROI_line(ROI_Base, pg.LineSegmentROI):
+    '''ROI Line class for selecting a straight line of pixels between two points.
+
+    Extends from :class:`ROI_Base <flika.roi.ROI_Base>` and pyqtgraph pyqtgraph.LineSegmentROI
+
+    Attributes:
+        kymograph (Window): :class:`Window <flika.window.Window>` showing 2d kymograph.
+    '''
+    kind = 'line'
+    plotSignal = QtCore.Signal()
+    
+    def __init__(self, window, positions, **kargs):
+        roiArgs = self.INITIAL_ARGS.copy()
+        roiArgs.update(kargs)
+        pg.LineSegmentROI.__init__(self, positions=positions, **roiArgs)
+        self.kymograph = None
+        self.kymographAct = QtWidgets.QAction("&Kymograph", self, triggered=self.update_kymograph)
+        ROI_Base.__init__(self, window, positions)
+        #self.snapPoints()
+
+    def paint(self, p, *args):
+        p.setRenderHint(QtGui.QPainter.Antialiasing)
+        p.setPen(self.currentPen)
+        h1 = self.handles[0]['item'].pos()
+        h2 = self.handles[1]['item'].pos()
+        p.drawLine(h1, h2)
+
+    def resetSignals(self):
+        ROI_Base.resetSignals(self)
+        self.sigRegionChanged.connect(self.snapPoints)
+
+    def snapPoints(self):
+        """Correct ROI points to be at the center of pixels, for clarity
+        """
+        fix = False
+        self.blockSignals(True)
+        for handle in self.handles:
+            pos = handle['pos']
+            pos_snap = self.getSnapPosition(pg.Point(pos))# + pg.Point(.5, .5)
+            if not (pos == pos_snap):
+                handle['item'].setPos(pos_snap)
+                handle['pos'] = pos_snap
+                fix = True
+
+        self.blockSignals(False)
+        #if fix:
+        #    self.sigRegionChanged.emit(self)
+
+    def draw_from_points(self, pts, finish=True):
+        self.blockSignals(True)
+        self.movePoint(self.handles[0]['item'], pts[0], finish=False)
+        self.movePoint(self.handles[1]['item'], pts[1], finish=False)
+        self.pts = pts
+        self.blockSignals(False)
+        if finish:
+            self.sigRegionChangeFinished.emit(self)
+
+    def delete(self):
+        ROI_Base.delete(self)
+        if self.kymograph:
+            self.deleteKymograph()
+
+    def getMask(self):
+        from skimage.draw import line
+        x=np.array([p[0] for p in self.pts], dtype=int)
+        y=np.array([p[1] for p in self.pts], dtype=int)
+        xx, yy = line(x[0],y[0],x[1],y[1])
+        idx_to_keep = np.logical_not( (xx>=self.window.mx) | (xx<0) | (yy>=self.window.my) | (yy<0))
+        xx = xx[idx_to_keep]
+        yy = yy[idx_to_keep]
+        return xx, yy
+
+    def getPoints(self):
+        return np.array([handle['pos'] + self.state['pos'] for handle in self.handles])
+
+    def makeMenu(self):
+        ROI_Base.makeMenu(self)
+        self.menu.addAction(self.kymographAct)
+        self.kymographAct.setEnabled(self.window.image.ndim == 3 and not self.window.metadata['is_rgb'])
+
+    def update_kymograph(self):
+        tif=self.window.image
+        if tif.ndim != 3:
+            g.alert("Can only kymograph a 3d movie")
+            return
+
+        xx, yy = self.getMask()
+        mt = len(tif)
+        if len(xx) == 0:
+            return
+        xx = np.array(xx)
+        yy = np.array(yy)
+        
+        if len(xx) == 0:
+            return
+        mn=np.zeros((mt,len(xx)))
+        for t in np.arange(mt):
+            mn[t]=tif[t,xx,yy]
+        mn=mn.T
+        if self.kymograph is None:
+            self.createKymograph(mn)
+        else:
+            self.kymograph.imageview.setImage(mn,autoLevels=False,autoRange=False)
+            #self.kymograph.imageview.view.setAspectLocked(lock=True,ratio=mn.shape[1]/mn.shape[0])
+    
+    def createKymograph(self,mn):
+        from .window import Window
+        oldwindow = g.win
+        name=oldwindow.name+' - Kymograph'
+        self.kymograph=Window(mn,name,metadata=self.window.metadata)
+        self.sigRegionChanged.connect(self.update_kymograph)
+        self.kymograph.closeSignal.connect(self.deleteKymograph)
+        self.sigRemoveRequested.connect(self.deleteKymograph)
+
+    def deleteKymograph(self):
+        self.kymograph.closeSignal.disconnect(self.deleteKymograph)
+        self.sigRegionChanged.disconnect(self.update_kymograph)
+        self.kymograph=None
+
+class ROI_rectangle(ROI_Base, pg.ROI):
+    '''ROI rectangle class for selecting a set width and height group of pixels on an image.
+
+    Extends from :class:`ROI_Base <flika.roi.ROI_Base>` and pyqtgraph.ROI
+    '''
+    kind = 'rectangle'
+    plotSignal = QtCore.Signal()
+
+    def __init__(self, window, pos, size, resizable=True, **kargs):
+        """__init__ of ROI_rectangle class
+
+        Args:
+            pos (2-tuple): position of top left corner
+            size: (2-tuple): width and height of the rectangle
+            resizable (bool): add resize handles to ROI, this cannot be changed after creation
+        """
+        roiArgs = self.INITIAL_ARGS.copy()
+        roiArgs.update(kargs)
+        pos = np.array(pos, dtype=int)
+        size = np.array(size, dtype=int)
+
+        pg.ROI.__init__(self, pos, size, **roiArgs)
+        if resizable:
+            self.addScaleHandle([0, 1], [1, 0])
+            self.addScaleHandle([1, 0], [0, 1])
+            self.addScaleHandle([0, 0], [1, 1])
+            self.addScaleHandle([1, 1], [0, 0])
+        self.cropAction = QtWidgets.QAction('&Crop', self, triggered=self.crop)
+        ROI_Base.__init__(self, window, [pos, size])
+
+    def center_around(self, x, y):
+        """Relocate ROI so center lies at Point (x, y). size is not changed
+
+        Args:
+            x (int): new center for rectangle on X axis
+            y (int): new center for rectangle on Y axis
+        """
+        old_pts = self.getPoints()
+        old_center = old_pts[0] + .5 * old_pts[1]
+        new_center = np.array([x, y])
+        diff = new_center - old_center
+        new_pts = np.array([old_pts[0]+diff, old_pts[1]])
+        self.draw_from_points(new_pts)
+
+    def getPoints(self):
+        return np.array([self.state['pos'], self.state['size']], dtype=int)
+
+    def contains_pts(self, x, y):
+        target = np.array([x, y])
+        return np.all(self.pts[0] < target) and np.all(target < self.pts[0]+self.pts[1])
+
+    def getMask(self):
+        x, y = self.state['pos']
+        ww, hh = self.state['size']
+
+        xmin = max(x, 0)
+        ymin = max(y, 0)
+        xmax = min(x+ww, self.window.mx)
+        ymax = min(y+hh, self.window.my)
+
+        xx, yy = np.meshgrid(np.arange(xmin, xmax, dtype=int), np.arange(ymin, ymax, dtype=int))
+
+        return xx.flatten(), yy.flatten()
+
+    def draw_from_points(self, pts, finish=True):
+        self.setPos(pts[0], finish=False)
+        self.setSize(pts[1], finish=False)
+        self.pts = np.array(pts)
+        self.sigRegionChanged.emit(self)
+        if finish:
+            self.sigRegionChangeFinished.emit(self)
+
+    def makeMenu(self):
+        ROI_Base.makeMenu(self)
+        self.menu.addAction(self.cropAction)
+
+    def crop(self):
+        """Create a new window of the image cropped to this ROI
+
+        Returns:
+            window.Window: cropped image Window
+        """
+        from .window import Window
+        r = self.boundingRect()
+        p1 = r.topLeft() + self.state['pos']
+        p2 = r.bottomRight() + self.state['pos']
+        x1, y1 = int(p1.x()), int(p1.y())
+        x2, y2 = int(p2.x()), int(p2.y())
+
+        if x1<0: x1=0
+        if y1<0: y1=0
+
+        tif=self.window.image
+        #if self.window.imageview.hasTimeAxis():
+        if self.window.mt > 1:
+            mt, mx, my = tif.shape[:3]
+            if x2>=mx: x2=mx-1
+            if y2>=my: y2=my-1
+            newtif=tif[:,x1:x2,y1:y2]
+        else:
+            mx, my = tif.shape[:2]
+            if x2>=mx: x2=mx-1
+            if y2>=my: y2=my-1
+            newtif=tif[x1:x2,y1:y2]
+
+        w =  Window(newtif, self.window.name+' Cropped', metadata=self.window.metadata)
+        w.imageview.setImage(newtif, axes=self.window.imageview.axes)
+        w.image = newtif
+        return w
+
+class ROI_freehand(ROI_Base, pg.ROI):
+    """ROI freehand class for selecting a polygon from the original image.
+
+    Extends from :class:`ROI_Base <flika.roi.ROI_Base>` and pyqtgraph.ROI.
+    """
+    kind = 'freehand'
+    plotSignal = QtCore.Signal()
+    def __init__(self, window, pts, **kargs):
+        roiArgs = self.INITIAL_ARGS.copy()
+        roiArgs.update(kargs)
+        roiArgs['closed'] = True
+        pg.ROI.__init__(self, np.min(pts, 0), np.ptp(np.array(pts), 0), translateSnap=(1, 1), **kargs)
+        ROI_Base.__init__(self, window, pts)
+        self._untranslated_pts = np.subtract(self.pts, self.pos())
+        self._untranslated_mask = None
+        self.getMask()
+
+    def shape(self):
+        p = QtGui.QPainterPath()
+        p.moveTo(*self._untranslated_pts[0])
+        for i in range(len(self._untranslated_pts)):
+            p.lineTo(*self._untranslated_pts[i])
+        p.lineTo(*self._untranslated_pts[0])
+        return p
+
+    def paint(self, painter, *args):
+        painter.setPen(self.currentPen)
+        painter.drawPolygon(*[pg.Point(a, b) for a, b in self._untranslated_pts])
+
+    def draw_from_points(self, pts, finish=False):
+        self.blockSignals(True)
+        self.setPos(*np.min(pts, 0), False)
+        self.setSize(np.ptp(pts, 0), False)
+        self._untranslated_pts = np.subtract(pts, self.pos())
+        self.pts = pts
+        
+        self.sigRegionChanged.emit(self)
+        if finish:
+            self.sigRegionChangeFinished.emit(self)
+        self.blockSignals(False)
+
+    def contextMenuEnabled(self):
+        return True
+
+    def getPoints(self):
+        x, y = self.state['pos']
+        return np.add(self._untranslated_pts, [x, y])
+
+    def contains_pt(self, x, y):
+        pt = QtCore.QPointF(x, y) - self.pos()
+        qPainterPath = self.shape()
+        return qPainterPath.contains(pt)
+
+    def contains_pts(self, x, y):
+        ''' not yet implemented'''
+        pass
+
+    def getMask(self):
+        from skimage.draw import polygon
+        if self._untranslated_mask is not None:
+            xx = self._untranslated_mask[0] + int(self.state['pos'][0])
+            yy = self._untranslated_mask[1] + int(self.state['pos'][1])
+        else:
+            x, y = np.transpose(self._untranslated_pts)
+            mask=np.zeros(self.window.imageDimensions())
+            xx, yy = polygon(x,y,shape=mask.shape)
+            self._untranslated_mask = xx, yy
+
+        idx_to_keep = np.logical_not( (xx>=self.window.mx) | (xx<0) | (yy>=self.window.my) | (yy<0))
+        xx = xx[idx_to_keep]
+        yy = yy[idx_to_keep]
+        return xx, yy
+
+class ROI_rect_line(ROI_Base, QtWidgets.QGraphicsObject):
+    """Collection of linked line segments with adjustable width.
+
+    Extends from :class:`ROI_Base <flika.roi.ROI_Base>` and QtWidgets.QGraphicsObject
+
+    Attributes:
+        kymograph (Window): :class:`Window <flika.window.Window>` showing 2d kymograph.
+    """
+    kind = 'rect_line'
+    plotSignal = QtCore.Signal()
+    sigRegionChanged = QtCore.Signal(object)
+    sigRegionChangeFinished = QtCore.Signal(object)
+
+    def __init__(self, window, pts, width=1, **kargs):
+        self.roiArgs = self.INITIAL_ARGS.copy()
+        self.roiArgs.update(kargs)
+        self.roiArgs['scaleSnap'] = False
+        self.width = width
+        self.kymograph = None
+        QtWidgets.QGraphicsObject.__init__(self)
+        self.kymographAct = QtWidgets.QAction("&Kymograph", self, triggered=self.update_kymograph)
+        self.removeLinkAction = QtWidgets.QAction('Remove Last Link', self, triggered=nonpartial(self.removeSegment))
+        self.setWidthAction = QtWidgets.QAction("Set Width", self, triggered=nonpartial(self.setWidth))
+        ROI_Base.__init__(self, window, pts)
+        self.getPoints = self.getHandlePositions
+        self.pen = QtGui.QPen(QtGui.QColor(255, 255, 0))
+        self.pen.setWidth(0)
+        self.lines = []
+        if len(pts) < 2:
+            raise Exception("Must start with at least 2 points")
+        self.extendHandle = None
+            
+        self.addSegment(pts[1], connectTo=pts[0])
+        for p in pts[2:]:
+            self.addSegment(p)
+
+    def getHandles(self):
+        handles = []
+        for line in self.lines:
+            handles.append(line.getHandles()[0])
+        handles.append(self.lines[-1].getHandles()[1])
+        return handles
+
+    def movePoint(self, handle, *args, **kargs):
+        if isinstance(handle, int):
+            handle = self.getHandles()[handle]
+        kargs['finish'] = False
+        self.blockSignals(True)
+        for line in handle.rois:
+            line.movePoint(handle, *args, **kargs)
+        self.blockSignals(False)
+        self.sigRegionChanged.emit(self)
+        self.sigRegionChangeFinished.emit(self)
+
+    def delete(self):
+        ROI_Base.delete(self)
+        if self.kymograph:
+            self.deleteKymograph()
+
+    def draw_from_points(self, pts, finish=False):
+        while len(self.lines) > 1:
+            self.removeSegment(self.lines[-1])
+
+        self.lines[0].movePoint(0, pts[0])
+        self.lines[0].movePoint(1, pts[1])
+        for p in pts[2:]:
+            self.addSegment(p)
+
+        if finish:
+            self.sigRegionChangeFinished.emit(self)
+        self.pts = pts
+
+    def getTrace(self, bounds=None):
+        if self.window.image.ndim > 3 or self.window.metadata['is_rgb']:
+            g.alert("Plotting trace of RGB movies is not supported. Try splitting the channels.")
+            return None
+        if self.window.image.ndim == 3:
+            region = self.getArrayRegion(self.window.imageview.image, self.window.imageview.getImageItem(), (1, 2))
+            while region.ndim > 1:
+                region = np.average(region, 1)
+        elif self.window.image.ndim == 2:
+            region = self.getArrayRegion(self.window.imageview.image, self.window.imageview.getImageItem(), (0, 1))
+            region = [np.average(region)]
+
+        if bounds:
+            region = region[bounds[0]:bounds[1]]
+        return region
+
+    def preview(self):
+        im = self.getArrayRegion(self.window.imageview.getImageItem().image, self.window.imageview.getImageItem(), (0, 1))
+        if not hasattr(self, 'prev'):
+            from .window import Window
+            self.prev = Window(im)
+            self.sigRegionChanged.connect(lambda a: self.preview())
+        else:
+            self.prev.imageview.setImage(im)
+
+    def getHandlePositions(self):
+        """Return the positions of all handles in local coordinates."""
+        p = self.mapFromScene(self.lines[0].getHandles()[0].scenePos())
+        p = self.lines[0].getSnapPosition([p.x(), p.y()])
+        pos = [p]
+        for line in self.lines:
+            p = self.mapFromScene(line.getHandles()[1].scenePos())
+            p = line.getSnapPosition([p.x(), p.y()])
+            pos.append(p)
+        self.pts = pos
+        return self.pts
+
+    def getArrayRegion(self, data: np.ndarray,
+                       image_item: QtWidgets.QGraphicsItem=None,
+                       axes: tuple[int, int]=(0, 1),
+                       **kwds) -> np.ndarray:
+        rgns = []
+        for line in self.lines:
+            rgn = line.getArrayRegion(data, image_item, axes=axes, **kwds)
+            if rgn is None:
+                continue
+                #return None
+            rgns.append(rgn)
+            #print line.state['size']
+            
+        ## make sure orthogonal axis is the same size
+        ## (sometimes fp errors cause differences)
+        if image_item.axisOrder == 'row-major':
+            axes = axes[::-1]
+        ms = min([rgn.shape[axes[1]] for rgn in rgns])
+        slices = [slice(None)] * rgns[0].ndim
+        slices[axes[1]] = slice(0, ms)
+        rgns = [rgn[*slices] for rgn in rgns]
+        #print [r.shape for r in rgns], axes
+        
+        return np.concatenate(rgns, axis=axes[0])
+        
+    def addSegment(self, pos=(0, 0), connectTo=None):
+        """
+        Add a new segment to the ROI connecting from the previous endpoint to *pos*.
+        (pos is specified in the parent coordinate system of the MultiRectROI)
+        """
+        ## by default, connect to the previous endpoint
+        if len(self.lines) == 0 or connectTo == self.lines[0].getHandles()[0]:
+            ind = 0
+        else:
+            ind = len(self.lines)
+
+        def dragEvent(handle, ev):
+            pos = self.window.imageview.view.mapToView(ev.scenePos())
+            if ev.button() == QtCore.Qt.RightButton:
+                edgeHandles = self.getHandles()
+                edgeHandles = edgeHandles[0], edgeHandles[-1]
+                if self.extendHandle is None and handle not in edgeHandles:
+                    return
+
+                if len(handle.rois) == 1 and ev.isStart():
+                    _, self.extendHandle = self.addSegment(pos, connectTo=handle)
+                elif ev.isFinish():
+                    self.extendFinished()
+                else:
+                    self.extend(round(pos.x()), round(pos.y()), finish=False)
+            else:
+                for roi in handle.rois:
+                    roi.movePoint(handle, [round(pos.x()), round(pos.y())])
+                return
+            Handle.mouseDragEvent(handle, ev)
+            ev.accept()
+
+        if connectTo is None:
+            connectTo = self.lines[-1].getHandles()[1]
+
+        ## create new ROI
+        if len(self.lines) > 0:
+            newRoi = pg.ROI((0,0), [1, self.width], parent=self, pen=self.pen, **self.roiArgs)
+        else:
+            newRoi = pg.ROI((0,0), [1, self.width], pen=self.pen, **self.roiArgs)
+            newRoi.setParentItem(self)
+
+        if len(self.lines) == 0 or ind > 0: # add handles in order
+            ## Add first SR handle
+            if isinstance(connectTo, Handle):
+                h = newRoi.addScaleRotateHandle([0, 0.5], [1, 0.5], item=connectTo)
+                newRoi.movePoint(connectTo, connectTo.scenePos(), coords='scene')
+            else:
+                h = newRoi.addScaleRotateHandle([0, 0.5], [1, 0.5])
+                newRoi.movePoint(h, connectTo, coords='scene')
+            h.mouseDragEvent = lambda ev: dragEvent(h, ev)
+
+            ## add second SR handle
+            h2 = newRoi.addScaleRotateHandle([1, 0.5], [0, 0.5])
+            h2.mouseDragEvent = lambda ev: dragEvent(h2, ev)
+            newRoi.movePoint(h2, pos)
+        else:
+            h2 = newRoi.addScaleRotateHandle([1, 0.5], [0, 0.5])
+            h2.mouseDragEvent = lambda ev: dragEvent(h2, ev)
+            newRoi.movePoint(h2, pos)
+
+            if isinstance(connectTo, Handle):
+                h = newRoi.addScaleRotateHandle([0, 0.5], [1, 0.5], item=connectTo)
+                newRoi.movePoint(connectTo, connectTo.scenePos(), coords='scene')
+            else:
+                h = newRoi.addScaleRotateHandle([0, 0.5], [1, 0.5])
+                newRoi.movePoint(h, connectTo, coords='scene')
+            h.mouseDragEvent = lambda ev: dragEvent(h, ev)
+
+
+        self.lines.insert(ind, newRoi)
+        self.lines[0]._updateView()
+            
+        newRoi.translatable = False
+        newRoi.hoverEvent = lambda e: self.hoverEvent(newRoi, e)
+        newRoi.raiseContextMenu = self.raiseContextMenu
+        #newRoi.sigRegionChangeStarted.connect(self.roiChangeStartedEvent) 
+        newRoi.sigRegionChanged.connect(lambda a: self.sigRegionChanged.emit(self))
+        newRoi.sigRegionChangeFinished.connect( lambda a: self.sigRegionChangeFinished.emit(self))
+        self.sigRegionChanged.emit(self)
+        return newRoi, h2
+
+    def removeSegment(self, segment=None, finish=True): 
+        """Remove a segment from the ROI"""
+        if segment is None:
+            segment = self.removeLinkAction.data()
+            if segment is None:
+                return
+        elif isinstance(segment, int):
+            segment = self.lines[segment]
+        
+        segment.sigRegionChangeFinished.disconnect()
+        segment.sigRegionChanged.disconnect()
+
+        for h in segment.getHandles():
+            if len(h.rois) == 2 and h.parentItem() == segment:
+                otherROI = [line for line in h.rois if line != segment][0]
+                h.setParentItem(otherROI)
+                h.setPos(0, .5)
+            h.disconnectROI(segment)
+        if segment in self.lines:
+            self.lines.remove(segment)
+
+        segment.scene().removeItem(segment)
+        if len(self.lines) == 0:
+            self.delete()
+        
+    def extend(self, x, y, finish=True):
+        self.blockSignals(True)
+        point = pg.Point(x, y)
+
+        if self.extendHandle is not None:
+            for roi in self.lines:
+                if self.extendHandle in roi.getHandles():
+                    roi.movePoint(self.extendHandle, point, finish=False)
+            #self.extendHandle.movePoint(self.window.imageview.getImageItem().mapToScene(point), finish=False)
+        else:
+            self.addSegment((x, y))
+        self.blockSignals(False)
+
+        self.sigRegionChanged.emit(self)
+        if finish:
+            self.sigRegionChangeFinished.emit(self)
+
+    def drawFinished(self):
+        ROI_Base.drawFinished(self)
+        for l in self.lines:
+            l._updateView()
+
+    def extendFinished(self):
+        self.extendHandle = None
+        for l in self.lines: # fix resizing handles. First link Viewbox was set to something different
+            l._updateView()
+        self.sigRegionChangeFinished.emit(self)
+
+    def hoverEvent(self, l, ev):
+        if ev.enter:
+            pen = QtGui.QPen(QtGui.QColor(255, 0, 0))
+            pen.setWidth(0)
+            l.setPen(pen)
+            l.mouseHovering = True
+            #self.setCurrentPen(pen)
+        elif ev.exit:
+            l.setPen(self.pen)
+            self.setCurrentPen(self.pen)
+            l.mouseHovering = False
+
+    def getMask(self):
+
+        xxs = []
+        yys = []
+        for i in range(len(self.pts)-1):
+            p1, p2 = self.pts[i], self.pts[i+1]
+            xx, yy = line(int(p1[0]), int(p1[1]), int(p2[0]), int(p2[1]))
+            idx_to_keep = np.logical_not( (xx>=self.window.mx) | (xx<0) | (yy>=self.window.my) | (yy<0))
+            xx = xx[idx_to_keep]
+            yy = yy[idx_to_keep]
+            xxs.extend(xx)
+            yys.extend(yy)
+
+        return np.array(xxs, dtype=int), np.array(yys, dtype=int)
+
+    def makeMenu(self):
+        ROI_Base.makeMenu(self)
+        self.menu.addAction(self.removeLinkAction)
+        self.menu.addAction(self.setWidthAction)
+        self.menu.addAction(self.kymographAct)
+        self.kymographAct.setEnabled(self.window.image.ndim > 2)
+
+    def raiseContextMenu(self, ev):
+        currentLines = [line for line in self.lines if line.mouseHovering]
+        if len(currentLines) > 0 and np.any([len(i.rois)==1 for i in currentLines[0].getHandles()]):
+            self.removeLinkAction.setText("Remove Link")
+            self.removeLinkAction.setVisible(True)
+            self.removeLinkAction.setData(currentLines[0])
+        else:
+            self.removeLinkAction.setVisible(False)
+        
+        ROI_Base.raiseContextMenu(self, ev)
+
+    def boundingRect(self):
+        return QtCore.QRectF()
+
+    def paint(self, p, *args):
+        pass
+
+    def setPen(self, pen):
+        pen = QtGui.QPen(pen)
+        pen.setWidth(0)
+        self.pen = pen
+        self.setCurrentPen(pen)
+
+    def setCurrentPen(self, pen):
+        pen = QtGui.QPen(pen)
+        pen.setWidth(0)
+        for l in self.lines:
+            l.currentPen = pen
+            l.update()
+
+    def update_kymograph(self):
+        tif=self.window.image
+        if tif.ndim != 3:
+            g.alert("Can only kymograph on 3D movies")
+            return
+        
+        if self.width == 1:
+            w, h = self.window.imageDimensions()
+            r = QtCore.QRect(0, 0, w, h)
+            xx, yy = self.getMask()
+            mn = tif[:, xx, yy].T
+        else:
+            region = self.getArrayRegion(self.window.imageview.image, self.window.imageview.getImageItem(), (1, 2))
+            mn = np.average(region, 2).T
+
+
+        if self.kymograph is None:
+            self.createKymograph(mn)
+        else:
+            if mn.size > 0:
+                self.kymograph.imageview.setImage(mn,autoLevels=False,autoRange=False)
+            #self.kymograph.imageview.view.setAspectLocked(lock=True,ratio=mn.shape[1]/mn.shape[0])
+
+    def setWidth(self, newWidth=None):
+        """Set the width of each segment in the ROI
+
+        Args:
+            newWidth (int): new width of all segments
+        """
+        s = True
+        if newWidth is None:
+            newWidth, s = QtWidgets.QInputDialog.getInt(None, "Enter a width value", 'Float Value', value=self.width)
+        if not s or s == 0:
+            return
+        for l in self.lines:
+            l.scale([1.0, newWidth/self.width], center=[0.5,0.5])
+        self.width = newWidth
+        self.sigRegionChangeFinished.emit(self)
+
+    def createKymograph(self,mn):
+        from .window import Window
+        oldwindow=g.win
+        name=oldwindow.name+' - Kymograph'
+        self.kymograph=Window(mn,name,metadata=self.window.metadata)
+        self.kymographproxy = pg.SignalProxy(self.sigRegionChanged, rateLimit=1, slot=self.update_kymograph) #This will only update 3 Hz
+        self.sigRegionChanged.connect(self.update_kymograph)
+        self.kymograph.closeSignal.connect(self.deleteKymograph)
+
+    def deleteKymograph(self):
+        self.kymographproxy.disconnect()
+        self.sigRegionChanged.disconnect(self.update_kymograph)
+        self.kymograph.closeSignal.disconnect(self.deleteKymograph)
+        self.kymograph=None
+
+def makeROI(kind, pts, window=None, color=None, **kargs):
+    """Create an ROI object in window with the given points
+
+    Args:
+        kind (str): one of ['line', 'rectangle', 'freehand', 'rect_line']
+        pts ([N, 2] list of coords): points used to draw the ROI, differs by kind
+        window (window.Window): window to draw the ROI in, or currentWindow if not specified
+        color (QtGui.QColor): pen color of the new ROI
+        **kargs: additional arguments to pass to the ROI __init__ function
+
+    Returns:
+        ROI Object extending ROI_Base
+    """
+    if window is None:
+        window = g.win
+        if window is None:
+            g.alert('ERROR: In order to make and ROI a window needs to be selected')
+            return None
+
+    if kind == 'freehand':
+        roi = ROI_freehand(window, pts, **kargs)
+    elif kind == 'rectangle':
+        if len(pts) > 2:
+            size = np.ptp(pts,0)
+            top_left = np.min(pts,0)
+        else:
+            size = pts[1]
+            top_left = pts[0]
+        roi = ROI_rectangle(window, top_left, size, **kargs)
+    elif kind == 'line':
+        roi = ROI_line(window, (pts), **kargs)
+    elif kind == 'rect_line':
+        roi = ROI_rect_line(window, pts, **kargs)
+    else:
+        g.alert("ERROR: THIS KIND OF ROI COULD NOT BE FOUND: {}".format(kind))
+        return None
+
+    if color is None or not isinstance(color, QtGui.QColor):
+        pen = QtGui.QPen(QtGui.QColor(g.settings['roi_color']) if g.settings['roi_color'] != 'random' else random_color())
+    else:
+        pen = QtGui.QPen(color)
+    pen.setWidth(0)
+
+    roi.drawFinished()
+    roi.setPen(pen)
+    return roi
+
+def open_rois(filename=None):
+    """
+    Open an roi.txt file, creates ROI objects and places them in the current Window.
+    
+    Args:
+        filename (str): The filename (including full path) of the roi.txt file.
+
+    Returns:
+        list of rois
+
+    """
+    if filename is None:
+        filetypes = '*.txt'
+        prompt = 'Load ROIs from file'
+        filename = open_file_gui(prompt, filetypes=filetypes)
+        if filename is None:
+            return None
+    text = open(filename, 'r').read()
+    rois = []
+    kind = None
+    pts = None
+    for text_line in text.split('\n'):
+        if kind is None:
+            kind = text_line
+            pts = []
+        elif text_line == '':
+            roi = makeROI(kind,pts)
+            rois.append(roi)
+            kind = None
+            pts = None
+        else:
+            pts.append(tuple(int(float(i)) for i in text_line.split()))
+
+    return rois
+logger.debug("Completed 'reading roi.py'")
```

### Comparing `flika-0.2.9/flika/tests/test_macros.py` & `flika-0.3.0/flika/tests/test_macros.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from ..app.plugin_manager import PluginManager, load_local_plugins, plugin_list
-from ..app.script_editor import ScriptEditor
-from ..window import Window
-import numpy as np
-
-class TestPluginManager():
-	def setup_method(self, method):
-		PluginManager.show()
-		load_local_plugins()
-		
-	def teardown_method(self, method):
-		PluginManager.close()
-
-	def test_local_plugins(self):
-		local = set(plugin_list.keys())
-		plugins = set(PluginManager.plugins.keys())
-
-		assert (local & plugins) == plugins, "Local plugin list not loaded correctly"
-
-	def test_install_plugin(self):
-		load_local_plugins()
-		plugin_name = 'Detect Puffs'
-		if PluginManager.plugins[plugin_name].installed:
-			return
-		PluginManager.refresh_online_plugins()
-		i = 0
-		while PluginManager.plugins[plugin_name].url == None:
-			i += 1
-			if i == 1000:
-				return
-			continue
-		PluginManager.downloadPlugin(plugin_name)
-		assert PluginManager.plugins[plugin_name].menu is not None and PluginManager.plugins[plugin_name].installed, "Plugin install"
-		PluginManager.removePlugin(plugin_name)
-		assert PluginManager.plugins[plugin_name].menu is None and not PluginManager.plugins[plugin_name].installed, "Plugin uninstall"
-
-
-class TestScriptEditor():
-	def setup_method(self, method):
-		ScriptEditor.show()
-
-	def teardown_method(self, method):
-		ScriptEditor.close()
-
-	def test_from_window(self):
-		w1 = Window(np.random.random([10, 20, 20]))
-		from ..process import threshold
-		w2 = threshold(.5)
-		ScriptEditor.gui.actionFrom_Window.trigger()
-		text = str(ScriptEditor.gui.currentTab().toPlainText())
+from ..app.plugin_manager import PluginManager, plugin_list
+from ..app.script_editor import ScriptEditor
+from ..window import Window
+from .. import flika
+import numpy as np
+
+class TestPluginManager():
+	def setup_method(self, method):
+		flika.start_flika()
+		PluginManager.show()
+		
+	def teardown_method(self, method):
+		PluginManager.close()
+
+	def test_local_plugins(self):
+		local = set(plugin_list.keys())
+		plugins = set(PluginManager.plugins.keys())
+
+		assert (local & plugins) == local, "Local plugin list not loaded correctly"
+
+	def test_install_plugin(self):
+		plugin_name = 'Detect Puffs'
+		if PluginManager.plugins[plugin_name].installed:
+			return
+		PluginManager.refresh_online_plugins()
+		i = 0
+		while PluginManager.plugins[plugin_name].url == None:
+			i += 1
+			if i == 1000:
+				return
+			continue
+		PluginManager.downloadPlugin(plugin_name)
+		assert PluginManager.plugins[plugin_name].menu is not None and PluginManager.plugins[plugin_name].installed, "Plugin install"
+		PluginManager.removePlugin(plugin_name)
+		assert PluginManager.plugins[plugin_name].menu is None and not PluginManager.plugins[plugin_name].installed, "Plugin uninstall"
+
+
+class TestScriptEditor():
+	def setup_method(self, method):
+		ScriptEditor.show()
+
+	def teardown_method(self, method):
+		ScriptEditor.close()
+
+	def test_from_window(self):
+		w1 = Window(np.random.random([10, 20, 20]))
+		from ..process import threshold
+		w2 = threshold(.5)
+		ScriptEditor.gui.actionFrom_Window.trigger()
+		text = str(ScriptEditor.gui.currentTab().toPlainText())
 		assert text == "threshold(value=0.5, darkBackground=False, keepSourceWindow=False)", "From window command not expected"
```

### Comparing `flika-0.2.9/flika/tests/test_settings.py` & `flika-0.3.0/flika/tests/test_settings.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from .. import global_vars as g
-from ..window import Window
-import numpy as np
-from ..roi import makeROI
-
-class TestSettings():
-
-	def test_random_roi_color(self):
-		initial = g.settings['roi_color']
-		g.settings['roi_color'] = 'random'
-		w1 = Window(np.random.random([10, 10, 10]))
-		roi1 = makeROI('rectangle', [[1, 1], [3, 3]])
-		roi2 = makeROI('rectangle', [[2, 2], [3, 3]])
-		assert roi1.pen.color().name() != roi2.pen.color().name(), 'Random ROI color is the same. This could be a random chance. Run repeatedly.'
-		
-		g.settings['roi_color'] = '#00ff00'
-		roi3 = makeROI('rectangle', [[3, 3], [3, 3]])
-		assert roi3.pen.color().name() == "#00ff00", 'ROI color set. all rois are same color'
-
-		g.settings['roi_color'] = initial
-
-	def test_multitrace(self):
-		initial = g.settings['multipleTraceWindows']
-		g.settings['multipleTraceWindows'] = False
-
-		w1 = Window(np.random.random([10, 10, 10]))
-		roi1 = makeROI('rectangle', [[1, 1], [3, 3]])
-		roi1.plot()
-		roi2 = makeROI('rectangle', [[2, 2], [3, 3]])
-		roi2.plot()
-		assert roi1.traceWindow == roi2.traceWindow, 'Traces not plotted together.'
-		
-		g.settings['multipleTraceWindows'] = True
-		roi3 = makeROI('rectangle', [[3, 3], [3, 3]])
-		roi3.plot()
-		assert roi3.traceWindow != roi1.traceWindow, 'Multiple trace windows'
-
-		g.settings['multipleTraceWindows'] = initial
+from .. import global_vars as g
+from ..window import Window
+import numpy as np
+from ..roi import makeROI
+
+class TestSettings():
+
+	def test_random_roi_color(self):
+		initial = g.settings['roi_color']
+		g.settings['roi_color'] = 'random'
+		w1 = Window(np.random.random([10, 10, 10]))
+		roi1 = makeROI('rectangle', [[1, 1], [3, 3]])
+		roi2 = makeROI('rectangle', [[2, 2], [3, 3]])
+		assert roi1.pen.color().name() != roi2.pen.color().name(), 'Random ROI color is the same. This could be a random chance. Run repeatedly.'
+		
+		g.settings['roi_color'] = '#00ff00'
+		roi3 = makeROI('rectangle', [[3, 3], [3, 3]])
+		assert roi3.pen.color().name() == "#00ff00", 'ROI color set. all rois are same color'
+
+		g.settings['roi_color'] = initial
+
+	def test_multitrace(self):
+		initial = g.settings['multipleTraceWindows']
+		g.settings['multipleTraceWindows'] = False
+
+		w1 = Window(np.random.random([10, 10, 10]))
+		roi1 = makeROI('rectangle', [[1, 1], [3, 3]])
+		roi1.plot()
+		roi2 = makeROI('rectangle', [[2, 2], [3, 3]])
+		roi2.plot()
+		assert roi1.traceWindow == roi2.traceWindow, 'Traces not plotted together.'
+		
+		g.settings['multipleTraceWindows'] = True
+		roi3 = makeROI('rectangle', [[3, 3], [3, 3]])
+		roi3.plot()
+		assert roi3.traceWindow != roi1.traceWindow, 'Multiple trace windows'
+
+		g.settings['multipleTraceWindows'] = initial
```

### Comparing `flika-0.2.9/flika/window.py` & `flika-0.3.0/flika/window.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,544 +1,788 @@
-# -*- coding: utf-8 -*-
-from qtpy import QtCore, QtGui, QtWidgets
-import pyqtgraph as pg
-import os, time
-import numpy as np
-from skimage import measure
-from .tracefig import TraceFig
-from . import global_vars as g
-from .roi import *
-from .utils.misc import save_file_gui
-pg.setConfigOptions(useWeave=False)
-
-
-class Window(QtWidgets.QWidget):
-    """
-    Window objects are the central objects in flika. Almost all functions in the 
-    :mod:`process <flika.process>` module are performed on Window objects and 
-    output Window objects. 
-
-    """
-    closeSignal = QtCore.Signal()
-    keyPressSignal = QtCore.Signal(QtCore.QEvent)
-    sigTimeChanged = QtCore.Signal(int)
-    gainedFocusSignal = QtCore.Signal()
-    lostFocusSignal = QtCore.Signal()
-
-    def __init__(self, tif, name='flika', filename='', commands=[], metadata=dict()):
-        QtWidgets.QWidget.__init__(self)
-        self.commands = commands  # commands is a list of the commands used to create this window, starting with loading the file.
-        self.metadata = metadata
-        if 'is_rgb' not in metadata.keys():
-            metadata['is_rgb'] = tif.ndim == 4
-        if g.currentWindow is None:
-            if 'window_settings' not in g.settings:
-                g.settings['window_settings'] = dict()
-            if 'coords' in g.settings['window_settings']:
-                geometry = QtCore.QRect(*g.settings['window_settings']['coords'])
-            else:
-                width = 684
-                height = 585
-                nwindows = len(g.windows)
-                x = 10 + 10 * nwindows
-                y = 300 + 10 * nwindows
-                geometry = QtCore.QRect(x, y, width, height)
-                g.settings['window_settings']['coords'] = geometry.getRect()
-        else:
-            geometry = g.currentWindow.geometry()
-            geometry.setX(geometry.x()+10)
-            geometry.setY(geometry.y() + 10)
-
-        self.resizeEvent = self.onResize
-        self.moveEvent = self.onMove
-        self.name = name
-        self.filename = filename
-        self.setAsCurrentWindow()
-        self.setWindowTitle(name)
-        self.imageview = pg.ImageView(self)
-        self.imageview.setMouseTracking(True)
-        self.imageview.installEventFilter(self)
-        self.imageview.ui.menuBtn.setParent(None)
-        self.imageview.ui.roiBtn.setParent(None) # gets rid of 'roi' button that comes with ImageView
-        self.imageview.ui.normLUTbtn = QtWidgets.QPushButton(self.imageview.ui.layoutWidget)
-        self.imageview.ui.normLUTbtn.setObjectName("LUT norm")
-        self.imageview.ui.normLUTbtn.setText("LUT norm")
-        self.imageview.ui.gridLayout.addWidget(self.imageview.ui.normLUTbtn, 1, 1, 1, 1)
-        self.imageview.ui.normLUTbtn.pressed.connect(self.normLUT)
-        rp = self.imageview.ui.roiPlot.getPlotItem()
-        self.linkMenu = QtWidgets.QMenu("Link frame")
-        rp.ctrlMenu = self.linkMenu
-        self.linkMenu.aboutToShow.connect(self.make_link_menu)
-
-        if np.any(np.isinf(tif)):
-            tif[np.isinf(tif)] = 0
-            g.alert('Some array values were inf. Setting those values to 0')
-
-        self.imageview.setImage(tif)
-        self.image = tif
-        self.volume = None  # When attaching a 4D array to this Window object, where self.image is a 3D slice of this volume, attach it here. This will remain None for all 3D Windows
-        self.nDims = len(np.shape(self.image))
-        dimensions_txt = ""
-        mx = 0
-        my = 0
-        mt = 0
-        if self.nDims == 3:
-            if metadata['is_rgb']:
-                mx, my, mc = tif.shape
-                mt = 1
-                dimensions_txt = "{}x{} pixels; {} colors; ".format(mx,my,mc)
-            else:
-                mt, mx, my = tif.shape
-                dimensions_txt = "{} frames; {}x{} pixels; ".format(mt, mx, my)
-        elif self.nDims == 4:
-            mt, mx ,my, mc = tif.shape
-            dimensions_txt = "{} frames; {}x{} pixels; {} colors; ".format(mt, mx, my, mc)
-        elif self.nDims == 2:
-            mt = 1
-            mx, my = tif.shape
-            dimensions_txt = "{}x{} pixels; ".format(mx, my)
-        self.mx = mx
-        self.my = my
-        self.mt = mt
-        dtype = self.image.dtype
-        dimensions_txt += 'dtype=' + str(dtype)
-        if 'timestamps' in self.metadata:
-            ts = self.metadata['timestamps']
-            self.framerate = (ts[-1] - ts[0]) / len(ts)
-            dimensions_txt += '; {:.4f} {}/frame'.format(self.framerate, self.metadata['timestamp_units'])
-        self.top_left_label = pg.LabelItem(dimensions_txt, justify='right')
-        self.imageview.ui.graphicsView.addItem(self.top_left_label)
-        self.imageview.timeLine.sigPositionChanged.connect(self.updateindex)
-        self.currentIndex = self.imageview.currentIndex
-        self.normLUT()
-        self.layout = QtWidgets.QVBoxLayout(self)
-        self.layout.addWidget(self.imageview)
-        self.layout.setContentsMargins(0, 0, 0, 0)
-        self.setGeometry(geometry)
-        self.imageview.scene.sigMouseMoved.connect(self.mouseMoved)
-        self.imageview.view.mouseDragEvent = self.mouseDragEvent
-        self.imageview.view.mouseClickEvent = self.mouseClickEvent
-        self.rois = []
-        self.currentROI = None
-        self.creatingROI = False
-        pointSize = g.settings['point_size']
-        pointColor = QtGui.QColor(g.settings['point_color'])
-        self.scatterPlot = pg.ScatterPlotItem(size=pointSize, pen=pg.mkPen([0, 0, 0, 255]), brush=pg.mkBrush(*pointColor.getRgb()))  #this is the plot that all the red points will be drawn on
-        self.scatterPoints = [[] for _ in np.arange(mt)]
-        self.scatterPlot.sigClicked.connect(self.clickedScatter)
-        self.imageview.addItem(self.scatterPlot)
-        self.pasteAct = QtWidgets.QAction("&Paste", self, triggered=self.paste)
-        if g.settings['show_windows']:
-            self.show()
-            QtWidgets.qApp.processEvents()
-        self.sigTimeChanged.connect(self.showFrame)
-        if self not in g.windows:
-            g.windows.append(self)
-        self.closed=False
-
-        from .process.measure import measure
-        self.measure = measure
-        def clicked(evt):
-            self.measure.pointclicked(evt, window=self)
-        self.imageview.scene.sigMouseClicked.connect(clicked)
-        self.linkedWindows = set()
-        self.makeMenu()
-
-    def onResize(self, event):
-        g.settings['window_settings']['coords'] = self.geometry().getRect()
-
-    def onMove(self, event):
-        g.settings['window_settings']['coords'] = self.geometry().getRect()
-
-    def save(self, filename):
-        from .process.file_ import save_file
-        old_curr_win = g.currentWindow
-        self.setAsCurrentWindow()
-        save_file(filename)
-        old_curr_win.setAsCurrentWindow()
-
-    def normLUT(self):
-        if self.nDims ==2:
-            # if the image is binary (either all 0s or 0s and 1s)
-            if np.min(self.image) == 0 and (np.max(self.image) == 0 or np.max(self.image) == 1):
-                self.imageview.setLevels(-.01, 1.01)  # set levels from slightly below 0 to 1
-        if self.nDims == 3 and not self.metadata['is_rgb']:
-            if np.all(self.image[self.currentIndex] == 0):  # if the current frame is all zeros
-                r = (np.min(self.image), np.max(self.image))  # set the levels to be just above and below the min and max of the entire tif
-                r = (r[0] - (r[1] - r[0]) / 100, r[1] + (r[1] - r[0]) / 100)
-                self.imageview.setLevels(r[0], r[1])
-            else:
-                r = (np.min(self.image[self.currentIndex]),
-                     np.max(self.image[self.currentIndex]))  # set the levels to be just above and below the min and max of the first frame
-                r = (r[0] - (r[1] - r[0]) / 100, r[1] + (r[1] - r[0]) / 100)
-                self.imageview.setLevels(r[0], r[1])
-        elif self.nDims == 4 and not self.metadata['is_rgb']:
-            if np.min(self.image) == 0 and (np.max(self.image) == 0 or np.max(self.image) == 1):  # if the image is binary (either all 0s or 0s and 1s)
-                self.imageview.setLevels(-.01, 1.01)  # set levels from slightly below 0 to 1
-    
-    def link(self, win):
-        if win not in self.linkedWindows:
-            self.sigTimeChanged.connect(win.imageview.setCurrentIndex)
-            self.linkedWindows.add(win)
-            win.link(self)
-
-    def unlink(self, win):
-        if win in self.linkedWindows:
-            self.linkedWindows.remove(win)
-            self.sigTimeChanged.disconnect(win.imageview.setCurrentIndex)
-            win.unlink(self)
-
-    def link_toggled(self, win):
-        return lambda b: self.link(win) if b else self.unlink(win)
-
-    def make_link_menu(self):
-        self.linkMenu.clear()
-        for win in g.windows:
-            if win == self or not win.isVisible():
-                continue
-            win_action = QtWidgets.QAction("%s" % win.name, self.linkMenu, checkable=True)
-            win_action.setChecked(win in self.linkedWindows)
-            win_action.toggled.connect(self.link_toggled(win))
-            self.linkMenu.addAction(win_action)
-        
-    def updateindex(self):
-        if self.mt == 1:
-            t = 0
-        else:
-            (idx, t) = self.imageview.timeIndex(self.imageview.timeLine)
-            t = int(np.floor(t))
-        if 0 <= t < self.mt:
-            self.currentIndex = t
-            if not g.settings['show_all_points']:
-                pointSizes = [pt[3] for pt in self.scatterPoints[t]]
-                brushes = [pg.mkBrush(*pt[2].getRgb()) for pt in self.scatterPoints[t]]
-                self.scatterPlot.setPoints(pos=self.scatterPoints[t], size=pointSizes, brush=brushes)
-            self.sigTimeChanged.emit(t)
-
-    def setIndex(self,index):
-        if hasattr(self, 'image') and self.image.ndim > 2 and 0 <= index < len(self.image):
-            self.imageview.setCurrentIndex(index)
-
-    def showFrame(self,index):
-        if index>=0 and index<self.mt:
-            msg = 'frame {}'.format(index)
-            if 'timestamps' in self.metadata and self.metadata['timestamp_units']=='ms':
-                ttime = self.metadata['timestamps'][index]
-                if ttime < 1*1000:
-                    msg += '; {:.4f} ms'.format(ttime)
-                elif ttime < 60*1000:
-                    seconds = ttime / 1000
-                    msg += '; {:.4f} s'.format(seconds)
-                elif ttime < 3600*1000:
-                    minutes = int(np.floor(ttime / (60*1000)))
-                    seconds = (ttime/1000) % 60
-                    msg += '; {} m {:.4f} s'.format(minutes, seconds)
-                else:
-                    seconds = ttime/1000
-                    hours = int(np.floor(seconds / 3600))
-                    mminutes = seconds - hours * 3600
-                    minutes = int(np.floor(mminutes / 60))
-                    seconds = mminutes - minutes * 60
-                    '; {} h {} m {:.4f} s'.format(hours, minutes, seconds)
-            g.m.statusBar().showMessage(msg)
-
-    def setName(self,name):
-        name = str(name)
-        self.name = name
-        self.setWindowTitle(name)
-        
-    def reset(self):
-        if not self.closed:
-            currentIndex = int(self.currentIndex)
-            self.imageview.setImage(self.image, autoLevels=True) #I had autoLevels=False before.  I changed it to adjust after boolean previews.
-            if self.imageview.axes['t'] is not None:
-                self.imageview.setCurrentIndex(currentIndex)
-            g.m.statusBar().showMessage('')
-
-    def closeEvent(self, event):
-        if self.closed:
-            print('Attempt to close window {} that was already closed'.format(self))
-            event.accept()
-        else:
-            self.closeSignal.emit()
-            for win in list(self.linkedWindows):
-                self.unlink(win)
-            if hasattr(self,'image'):
-                del self.image
-            self.imageview.setImage(np.zeros((2,2))) #clear the memory
-            self.imageview.close()
-            del self.imageview
-            if g.currentWindow==self:
-                g.currentWindow=None
-            if self in g.windows:
-                g.windows.remove(self)
-            self.closed=True
-            event.accept() # let the window close
-
-    def imageArray(self):
-        """
-        returns image as a 3d array, correcting for color or 2d image
-        """
-        tif = self.image
-        nDims = len(tif.shape)
-        if nDims == 4:  # If this is an RGB image stack  #[t, x, y, colors]
-            tif = np.mean(tif,3)
-            mx, my = tif[0,:,:].shape
-        elif nDims == 3:
-            if self.metadata['is_rgb']:  # [x, y, colors]
-                tif = np.mean(tif,2)
-                mx, my = tif.shape
-                tif = tif[np.newaxis]
-            else: 
-                mx, my = tif[0,:,:].shape
-        elif nDims == 2:
-            mx, my = tif.shape
-            tif = tif[np.newaxis]
-        return tif
-
-    def imageDimensions(self):
-        nDims = self.image.shape
-        if len(nDims) == 4: #if this is an RGB image stack
-            return nDims[1:3]
-        elif len(nDims) == 3:
-            if self.metadata['is_rgb']:  # [x, y, colors]
-                return nDims[:2]
-            else:                               # [t, x, y]
-                return nDims[1:]
-        if len(nDims) == 2:  # If this is a static image
-            return nDims
-        return nDims
-
-    def resizeEvent(self, event):
-        event.accept()
-        self.imageview.resize(self.size())
-
-    def paste(self):
-        """ This function pastes an ROI from one window into another.
-        The ROIs will be linked so that when you translate one of them, the other one also moves.
-        """
-        def pasteROI(roi):
-            if roi in self.rois:
-                return None
-            self.currentROI=makeROI(roi.kind,roi.pts,self)
-            if roi in roi.window.rois:
-                self.currentROI.link(roi)
-            return self.currentROI
-
-        if type(g.clipboard) == list:
-            rois = []
-            for roi in g.clipboard:
-                rois.append(pasteROI(roi))
-            return rois
-        else:
-            return pasteROI(g.clipboard)
-        
-    def mousePressEvent(self,ev):
-        ev.accept()
-        self.setAsCurrentWindow()
-
-    def setAsCurrentWindow(self):
-        if g.currentWindow is not None:
-            g.currentWindow.setStyleSheet("border:1px solid rgb(0, 0, 0); ")
-            g.currentWindow.lostFocusSignal.emit()
-        g.currentWindow=self
-        g.m.currentWindow = g.currentWindow
-        g.m.setWindowTitle("flika - {}".format(self.name))
-        self.setStyleSheet("border:1px solid rgb(0, 255, 0); ")
-        g.m.setCurrentWindowSignal.sig.emit()
-        self.gainedFocusSignal.emit()
-    
-    def clickedScatter(self, plot, points):
-        p = points[0]
-        x, y = p.pos()
-
-        if g.settings['show_all_points']:
-            pts = []
-            for t in np.arange(self.mt):
-                self.scatterPoints[t] = [p for p in self.scatterPoints[t] if not (x == p[0] and y == p[1])]
-                pts.extend(self.scatterPoints[t])
-            pointSizes = [pt[3] for pt in pts]
-            brushes = [pg.mkBrush(*pt[2].getRgb()) for pt in pts]
-            self.scatterPlot.setPoints(pos=pts, size=pointSizes, brush=brushes)
-        else:
-            t = self.currentIndex
-            self.scatterPoints[t] = [p for p in self.scatterPoints[t] if not (x == p[0] and y == p[1])]
-            pointSizes = [pt[3] for pt in self.scatterPoints[t]]
-            brushes = [pg.mkBrush(*pt[2].getRgb()) for pt in self.scatterPoints[t]]
-            self.scatterPlot.setPoints(pos=self.scatterPoints[t], size=pointSizes, brush=brushes)
-
-    def getScatterPts(self):
-        p_out=[]
-        p_in=self.scatterPoints
-        for t in np.arange(len(p_in)):
-            for p in p_in[t]:
-                p_out.append(np.array([t,p[0],p[1]]))
-        p_out=np.array(p_out)
-        return p_out
-        
-    def makeMenu(self):
-        self.menu = QtWidgets.QMenu(self)
-
-        def updateMenu():
-            from .roi import ROI_Base
-            pasteAct.setEnabled(isinstance(g.clipboard, (list, ROI_Base)))
-
-        pasteAct = QtWidgets.QAction("&Paste", self, triggered=self.paste)
-        plotAllAct = QtWidgets.QAction('&Plot All ROIs', self.menu, triggered=self.plotAllROIs )
-        copyAll = QtWidgets.QAction("Copy All ROIs", self.menu, triggered = lambda a: setattr(g, 'clipboard', self.rois))
-        removeAll = QtWidgets.QAction("Remove All ROIs", self.menu, triggered = self.removeAllROIs)
-        saveAll = QtWidgets.QAction("&Save All ROIs",self, triggered=self.exportROIs)
-
-        self.menu.addAction(pasteAct)
-        self.menu.addAction(plotAllAct)
-        self.menu.addAction(copyAll)
-        self.menu.addAction(saveAll)
-        self.menu.addAction(removeAll)
-        self.menu.aboutToShow.connect(updateMenu)
-
-    def plotAllROIs(self):
-        for roi in self.rois:
-            if roi.traceWindow == None:
-                roi.plot()
-
-    def removeAllROIs(self):
-        for roi in self.rois[:]:
-            roi.delete()
-
-    def addPoint(self, p=None):
-        if p is None:
-            p = [self.currentIndex, self.x, self.y]
-        elif len(p) != 3:
-            raise Exception("addPoint takes a 3-tuple (t, x, y) as argument")
-
-        t, x, y = p
-
-        pointSize=g.m.settings['point_size']
-        pointColor = QtGui.QColor(g.settings['point_color'])
-        position=[x, y, pointColor, pointSize]
-        self.scatterPoints[t].append(position)
-        self.scatterPlot.addPoints(pos=[[x, y]], size=pointSize, brush=pg.mkBrush(*pointColor.getRgb()))
-
-    def mouseClickEvent(self,ev):
-        self.EEEE = ev
-        if self.x is not None and self.y is not None and ev.button() == 2 and not self.creatingROI:
-            mm = g.settings['mousemode']
-            if mm == 'point':
-                self.addPoint()
-            elif mm == 'rectangle' and g.settings['default_roi_on_click']:
-                    self.currentROI = ROI_Drawing(self, self.x - g.settings['rect_width']/2, self.y - g.settings['rect_height']/2, mm)
-                    self.currentROI.extend(self.x + g.settings['rect_width']/2, self.y + g.settings['rect_height']/2)
-                    self.currentROI.drawFinished()
-            elif mm == 'freehand' and g.settings['default_roi_on_click']:
-                # Before using this script to get the outlines of cells from a raw movie of fluorescence, you need to do some processing.
-                # Get a good image of cells by averaging the movie using the zproject() function inside flika.
-                # Then threshold the image and use a combination of binary dilation and binary erosion to clean it up (all functions inside flika)
-                if not (np.all(self.image >= 0) and np.all(self.image <= 1)):
-                    return
-
-
-                thresholded_image = np.squeeze(self.image[self.currentIndex] if self.image.ndim == 3 else self.image)
-                labelled=measure.label(thresholded_image)
-
-                outline_coords = measure.find_contours(labelled == labelled[int(self.x)][int(self.y)], 0.5)
-                outline_coords = sorted(outline_coords, key=lambda a: -len(a))[0]
-                new_roi = makeROI("freehand", outline_coords)
-            else:
-                self.menu.exec_(ev.screenPos().toQPoint())
-        elif self.creatingROI:
-            self.currentROI.cancel()
-            self.creatingROI = None
-
-    def exportROIs(self, filename=None):
-        if not isinstance(filename, str):
-            if filename is not None and os.path.isfile(filename):
-                filename = os.path.splitext(g.settings['filename'])[0]
-                filename = save_file_gui('Save ROI', filename, '*.txt')
-            else:
-                filename = save_file_gui('Save ROI', '', '*.txt')
-
-        if filename != '' and isinstance(filename, str):
-            reprs = [roi.str() for roi in self.rois]
-            reprs = '\n'.join(reprs)
-            open(filename, 'w').write(reprs)
-        else:
-            g.m.statusBar().showMessage('No File Selected')
-    
-    def keyPressEvent(self, ev):
-        if ev.key() == QtCore.Qt.Key_Delete:
-            i = 0
-            while i < len(self.rois):
-                if self.rois[i].mouseHovering:
-                    self.rois[i].delete()
-                else:
-                    i += 1
-        self.keyPressSignal.emit(ev)
-        
-    def mouseMoved(self,point):
-        point=self.imageview.getImageItem().mapFromScene(point)
-        self.point = point
-        self.x = point.x()
-        self.y = point.y()
-        image=self.imageview.getImageItem().image
-        if self.x < 0 or self.y < 0 or self.x >= image.shape[0] or self.y>=image.shape[1]:
-            pass# if we are outside the image
-        else:
-            z=self.imageview.currentIndex
-            value=image[int(self.x),int(self.y)]
-            g.m.statusBar().showMessage('x={}, y={}, z={}, value={}'.format(int(self.x),int(self.y),z,value))
-        
-
-    def mouseDragEvent(self, ev):
-        modifiers = QtWidgets.QApplication.keyboardModifiers()
-        if modifiers == QtCore.Qt.ShiftModifier:
-            pass #This is how I detect that the shift key is held down.
-        if ev.button() == QtCore.Qt.LeftButton:
-            ev.accept()
-            difference=self.imageview.getImageItem().mapFromScene(ev.lastScenePos())-self.imageview.getImageItem().mapFromScene(ev.scenePos())
-            self.imageview.view.translateBy(difference)
-        if ev.button() == QtCore.Qt.RightButton:
-            ev.accept()
-            mm = g.settings['mousemode']
-            if mm in ('freehand', 'line', 'rectangle', 'rect_line'):
-                if ev.isStart():
-                    self.ev = ev
-                    pt = self.imageview.getImageItem().mapFromScene(ev.buttonDownScenePos())
-                    self.x = pt.x()  # This sets x and y to the button down position, not the current position.
-                    self.y = pt.y()
-                    self.creatingROI = True
-                    self.currentROI = ROI_Drawing(self, self.x, self.y, mm)
-                if ev.isFinish():
-                    if self.creatingROI:   
-                        if ev._buttons | QtCore.Qt.RightButton != ev._buttons:
-                            self.currentROI = self.currentROI.drawFinished()
-                            self.creatingROI = False
-                        else:
-                            self.currentROI.cancel()
-                            self.creatingROI = False
-                    else:
-                        for r in self.currentROIs:
-                            r.finish_translate()
-                else:  # If we are in the middle of the drag between starting and finishing.
-                    if self.creatingROI:
-                        self.currentROI.extend(self.x, self.y)
-
-    def updateTimeStampLabel(self,frame):
-        label = self.timeStampLabel
-        if self.framerate == 0:
-            label.setHtml("<span style='font-size: 12pt;color:white;background-color:None;'>Frame rate is 0 Hz</span>" )
-            return False
-        ttime = frame/self.framerate  # Time elapsed since the first frame until the current frame, in seconds.
-        if ttime < 1:
-            ttime = ttime * 1000
-            label.setHtml("<span style='font-size: 12pt;color:white;background-color:None;'>{:.0f} ms</span>".format(ttime))
-        elif ttime < 60:
-            label.setHtml("<span style='font-size: 12pt;color:white;background-color:None;'>{:.3f} s</span>".format(ttime))
-        elif ttime < 3600:
-            minutes = int(np.floor(ttime/60))
-            seconds = ttime % 60
-            label.setHtml("<span style='font-size: 12pt;color:white;background-color:None;'>{}m {:.3f} s</span>".format(minutes,seconds))
-        else:
-            hours = int(np.floor(ttime/3600))
-            mminutes = ttime-hours*3600
-            minutes = int(np.floor(mminutes/60))
-            seconds = mminutes-minutes*60
-            label.setHtml("<span style='font-size: 12pt;color:white;background-color:None;'>{}h {}m {:.3f} s</span>".format(hours,minutes,seconds))
+# -*- coding: utf-8 -*-
+from .logger import logger
+logger.debug("Started 'reading window.py'")
+from qtpy import QtCore, QtGui, QtWidgets
+import pyqtgraph as pg
+import os, time
+import numpy as np
+from . import global_vars as g
+from .roi import *
+from .utils.misc import save_file_gui
+from .utils.BaseProcess import WindowSelector, SliderLabel
+
+pg.setConfigOptions()
+
+
+class Bg_im_dialog(QtWidgets.QDialog):
+    def __init__(self, parent=None):
+        QtWidgets.QDialog.__init__(self)
+        self.parent = parent
+        self.setWindowTitle("Select background image")
+        self.window_selector = WindowSelector()
+        self.window_selector.valueChanged.connect(self.bg_win_changed)
+        self.alpha_slider = SliderLabel(3)
+        self.alpha_slider.setRange(0,1)
+        self.alpha_slider.setValue(.5)
+        self.alpha_slider.valueChanged.connect(self.alpha_changed)
+        self.formlayout = QtWidgets.QFormLayout()
+        self.formlayout.setLabelAlignment(QtCore.Qt.AlignRight)
+        self.formlayout.addRow("Select window with background image", self.window_selector)
+        self.formlayout.addRow("Set background opacity", self.alpha_slider)
+        self.layout = QtWidgets.QVBoxLayout()
+        self.layout.addLayout(self.formlayout)
+        self.setLayout(self.layout)
+
+    def alpha_changed(self, value):
+        if self.parent.bg_im is not None:
+            self.parent.bg_im.setOpacity(value)
+
+    def bg_win_changed(self):
+        if self.parent.bg_im is not None:
+            self.parent.imageview.view.removeItem(self.parent.bg_im)
+            self.bg_im = None
+        self.parent.bg_im = pg.ImageItem(self.window_selector.window.imageview.imageItem.image)
+        self.parent.bg_im.setOpacity(self.alpha_slider.value())
+        self.parent.imageview.view.addItem(self.parent.bg_im)
+
+
+    def closeEvent(self,ev):
+        if self.parent.bg_im is not None:
+            self.parent.imageview.view.removeItem(self.parent.bg_im)
+            self.bg_im = None
+
+
+class ImageView(pg.ImageView):
+    def __init__(self, *args, **kargs):
+        pg.ImageView.__init__(self, *args, **kargs)
+        self.view.unregister()
+        self.view.removeItem(self.roi)
+        self.view.removeItem(self.normRoi)
+        self.roi.setParent(None)
+        self.normRoi.setParent(None)
+        self.ui.menuBtn.setParent(None)
+        self.ui.roiBtn.setParent(None) # gets rid of 'roi' button that comes with ImageView
+        self.ui.normLUTbtn = QtWidgets.QPushButton(self.ui.layoutWidget)
+        self.ui.normLUTbtn.setObjectName("LUT norm")
+        self.ui.normLUTbtn.setText("LUT norm")
+        self.ui.gridLayout.addWidget(self.ui.normLUTbtn, 1, 1, 1, 1)
+
+        self.ui.bg_imbtn = QtWidgets.QPushButton(self.ui.layoutWidget)
+        self.ui.bg_imbtn.setObjectName("bg im")
+        self.ui.bg_imbtn.setText("bg im")
+        self.ui.gridLayout.addWidget(self.ui.bg_imbtn, 1, 2, 1, 1)
+
+        self.ui.roiPlot.setMaximumHeight(40)
+        self.ui.roiPlot.getPlotItem().getViewBox().setMouseEnabled(False)
+        self.ui.roiPlot.getPlotItem().hideButtons()
+
+    def hasTimeAxis(self):
+        return 't' in self.axes and not (self.axes['t'] is None or self.image.shape[self.axes['t']] == 1)
+
+    def roiClicked(self):
+        showRoiPlot = False
+        if self.hasTimeAxis():
+            showRoiPlot = True
+            mn = self.tVals.min()
+            mx = self.tVals.max() + .01
+            self.ui.roiPlot.setXRange(mn, mx, padding=0.01)
+            self.timeLine.show()
+            self.timeLine.setBounds([mn, mx])
+            self.ui.roiPlot.show()
+            if not self.ui.roiBtn.isChecked():
+                self.ui.splitter.setSizes([self.height()-35, 35])
+        else:
+            self.timeLine.hide()
+            #self.ui.roiPlot.hide()
+            
+        self.ui.roiPlot.setVisible(showRoiPlot)
+
+
+class Window(QtWidgets.QWidget):
+    """
+    Window objects are the central objects in flika. Almost all functions in the 
+    :mod:`process <flika.process>` module are performed on Window objects and 
+    output Window objects. 
+
+    Args:
+        tif (numpy.array): The image the window will store and display
+        name (str): The name of the window.
+        filename (str): The filename (including full path) of file this window's image orinated from.
+        commands (list of str): a list of the commands used to create this window, starting with loading the file.
+        metadata (dict): dict: a dictionary containing the original file's metadata.
+
+
+    """
+    closeSignal = QtCore.Signal()
+    keyPressSignal = QtCore.Signal(QtCore.QEvent)
+    sigTimeChanged = QtCore.Signal(int)
+    gainedFocusSignal = QtCore.Signal()
+    lostFocusSignal = QtCore.Signal()
+
+    def __init__(self, tif, name='flika', filename='', commands=[], metadata=dict()):
+        from .process.measure import measure
+        QtWidgets.QWidget.__init__(self)
+        self.name = name  #: str: The name of the window.
+        self.filename = filename  #: str: The filename (including full path) of file this window's image orinated from.
+        self.commands = commands  #: list of str: a list of the commands used to create this window, starting with loading the file.
+        self.metadata = metadata  #: dict: a dictionary containing the original file's metadata.
+        self.volume = None  # When attaching a 4D array to this Window object, where self.image is a 3D slice of this volume, attach it here. This will remain None for all 3D Windows
+        self.scatterPlot = None
+        self.closed = False  #: bool: True if the window has been closed, False otherwise.
+        self.mx = 0  #: int: The number of pixels wide the image is in the x (left to right) dimension.
+        self.my = 0  #: int: The number of pixels heigh the image is in the y (up to down) dimension.
+        self.mt = 0  #: int: The number of frames in the image stack.
+        self.framerate = None  #: float: The number of frames per second (Hz).
+        self.image = tif
+        self.dtype = tif.dtype  #: dtype: The datatype of the stored image, e.g. ``uint8``.
+        self.top_left_label = None
+        self.rois = []  #: list of ROIs: a list of all the :class:`ROIs <flika.roi.ROI_Base>` inside this window.
+        self.currentROI = None  #: :class:`ROI <flika.roi.ROI_Base>`: When an ROI is clicked, it becomes the currentROI of that window and can be accessed via this variable.
+        self.creatingROI = False
+        self.imageview = None
+        self.bg_im = None
+        self.currentIndex = 0
+        self.linkedWindows = set()
+        self.measure = measure
+        self.resizeEvent = self.onResize
+        self.moveEvent = self.onMove
+        self.pasteAct = QtWidgets.QAction("&Paste", self, triggered=self.paste)
+        self.sigTimeChanged.connect(self.showFrame)
+        self._check_for_infinities(tif)
+        self._init_dimensions(tif)
+        self._init_imageview(tif)
+        self.setWindowTitle(name)
+        self.normLUT(tif)
+        self._init_scatterplot()
+        self._init_menu()
+        self._init_geometry()
+        self.setAsCurrentWindow()
+
+    def _init_geometry(self):
+        assert g.win != self  # self.setAsCurrentWindow() must be called after this function
+        if g.win is None:
+            if 'window_settings' not in g.settings:
+                g.settings['window_settings'] = dict()
+            if 'coords' in g.settings['window_settings']:
+                geometry = QtCore.QRect(*g.settings['window_settings']['coords'])
+            else:
+                width = 684
+                height = 585
+                nwindows = len(g.windows)
+                x = 10 + 10 * nwindows
+                y = 300 + 10 * nwindows
+                geometry = QtCore.QRect(x, y, width, height)
+                g.settings['window_settings']['coords'] = geometry.getRect()
+        else:
+            geometry = g.win.geometry()
+
+        desktopGeom = QtGui.QGuiApplication.primaryScreen().availableGeometry()
+        maxX = (desktopGeom.width() - geometry.width()) or 1
+        maxY = (desktopGeom.height() - geometry.height()) or 1
+        newX = (geometry.x() + 10) % maxX
+        newY = ((geometry.y() + 10) % maxY) or 30
+        
+        geometry = QtCore.QRect(newX, newY, geometry.width(), geometry.height())
+        self.setGeometry(geometry)
+        self.layout = QtWidgets.QVBoxLayout(self)
+        self.layout.addWidget(self.imageview)
+        self.layout.setContentsMargins(0, 0, 0, 0)
+        if g.settings['show_windows']:
+            self.show()
+            self.raise_()
+            QtWidgets.QApplication.processEvents()
+
+    def _check_for_infinities(self, tif):
+        try:
+            if np.any(np.isinf(tif)):
+                tif[np.isinf(tif)] = 0
+                g.alert('Some array values were inf. Setting those values to 0')
+        except MemoryError:
+            pass
+
+    def _init_imageview(self, tif):
+        self.imageview = ImageView(self)
+        self.imageview.setMouseTracking(True)
+        self.imageview.installEventFilter(self)
+        self.imageview.ui.normLUTbtn.pressed.connect(lambda: self.normLUT(self.image))
+        self.imageview.ui.bg_imbtn.pressed.connect(self.set_bg_im)
+        rp = self.imageview.ui.roiPlot.getPlotItem()
+        self.linkMenu = QtWidgets.QMenu("Link frame")
+        rp.ctrlMenu = self.linkMenu
+        self.linkMenu.aboutToShow.connect(self.make_link_menu)
+        self.imageview.setImage(tif)
+        def clicked(evt):
+            self.measure.pointclicked(evt, window=self)
+        self.imageview.scene.sigMouseClicked.connect(clicked)
+        self.imageview.timeLine.sigPositionChanged.connect(self.updateindex)
+        self.currentIndex = self.imageview.currentIndex
+        self.imageview.scene.sigMouseMoved.connect(self.mouseMoved)
+        self.imageview.view.mouseDragEvent = self.mouseDragEvent
+        self.imageview.view.mouseClickEvent = self.mouseClickEvent
+        assert self.top_left_label is not None
+        self.imageview.ui.graphicsView.addItem(self.top_left_label)
+
+    def _init_dimensions(self, tif):
+        if 'is_rgb' not in self.metadata.keys():
+            self.metadata['is_rgb'] = tif.ndim == 4
+        self.nDims = len(np.shape(tif))  #: int: The number of dimensions of the stored image.
+        dimensions_txt = ""
+        if self.nDims == 3:
+            if self.metadata['is_rgb']:
+                self.mx, self.my, mc = tif.shape
+                self.mt = 1
+                dimensions_txt = f"{self.mx}x{self.my} pixels; {mc} colors; "
+            else:
+                self.mt, self.mx, self.my = tif.shape
+                dimensions_txt = f"{self.mt} frames; {self.mx}x{self.my} pixels; "
+        elif self.nDims == 4:
+            self.mt, self.mx ,self.my, mc = tif.shape
+            dimensions_txt = f"{self.mt} frames; {self.mx}x{self.my} pixels; {mc} colors; "
+        elif self.nDims == 2:
+            self.mt = 1
+            self.mx, self.my = tif.shape
+            dimensions_txt = f"{self.mx}x{self.my} pixels; "
+        dimensions_txt += 'dtype=' + str(self.dtype)
+        if self.framerate is None:
+            if 'timestamps' in self.metadata:
+                ts = self.metadata['timestamps']
+                self.framerate = (ts[-1] - ts[0]) / len(ts)
+        if self.framerate is not None:
+            tu = self.metadata['timestamp_units']
+            dimensions_txt += f'; {self.framerate:.4f} {tu}/frame'
+
+        if self.top_left_label is not None and self.imageview is not None and self.top_left_label in self.imageview.ui.graphicsView.items():
+            self.imageview.ui.graphicsView.removeItem(self.top_left_label)
+        self.top_left_label = pg.LabelItem(dimensions_txt, justify='right')
+
+    def _init_scatterplot(self):
+        if self.scatterPlot in self.imageview.ui.graphicsView.items():
+            self.imageview.ui.graphicsView.removeItem(self.scatterPlot)
+        pointSize = g.settings['point_size']
+        pointColor = QtGui.QColor(g.settings['point_color'])
+        self.scatterPlot = pg.ScatterPlotItem(size=pointSize, pen=pg.mkPen([0, 0, 0, 255]), brush=pg.mkBrush(*pointColor.getRgb()))  #this is the plot that all the red points will be drawn on
+        self.scatterPoints = [[] for _ in np.arange(self.mt)]
+        self.scatterPlot.sigClicked.connect(self.clickedScatter)
+        self.imageview.addItem(self.scatterPlot)
+
+    def _init_menu(self):
+        self.menu = QtWidgets.QMenu(self)
+
+        def updateMenu():
+            from .roi import ROI_Base
+            pasteAct.setEnabled(isinstance(g.clipboard, (list, ROI_Base)))
+
+        pasteAct = QtWidgets.QAction("&Paste", self, triggered=self.paste)
+        plotAllAct = QtWidgets.QAction('&Plot All ROIs', self.menu, triggered=self.plotAllROIs )
+        copyAll = QtWidgets.QAction("Copy All ROIs", self.menu, triggered = lambda a: setattr(g, 'clipboard', self.rois))
+        removeAll = QtWidgets.QAction("Remove All ROIs", self.menu, triggered = self.removeAllROIs)
+        self.menu.addAction(pasteAct)
+        self.menu.addAction(plotAllAct)
+        self.menu.addAction(copyAll)
+        self.menu.addAction(removeAll)
+        self.menu.aboutToShow.connect(updateMenu)
+
+    def onResize(self, event):
+        g.settings['window_settings']['coords'] = self.geometry().getRect()
+
+    def onMove(self, event):
+        g.settings['window_settings']['coords'] = self.geometry().getRect()
+
+    def save(self, filename):
+        """save(self, filename)
+        Saves the current window to a specificed directory as a (.tif) file
+
+        Args:
+            filename (str): The filename, including the full path, where this (.tif) file will be saved.
+
+        """
+        from .process.file_ import save_file
+        old_curr_win = g.win
+        self.setAsCurrentWindow()
+        save_file(filename)
+        old_curr_win.setAsCurrentWindow()
+
+    def normLUT(self, tif):
+        if self.nDims == 2:
+            # if the image is binary (either all 0s or 0s and 1s)
+            if np.min(tif) == 0 and (np.max(tif) == 0 or np.max(tif) == 1):
+                self.imageview.setLevels(-.01, 1.01)  # set levels from slightly below 0 to 1
+            else:
+                r = (np.min(tif), np.max(tif))  # set the levels to be just above and below the min and max of the image
+                r = (r[0] - (r[1] - r[0]) / 100, r[1] + (r[1] - r[0]) / 100)
+                self.imageview.setLevels(r[0], r[1])
+        if self.nDims == 3 and not self.metadata['is_rgb']:
+            if np.all(tif[self.currentIndex] == 0):  # if the current frame is all zeros
+                r = (np.min(tif), np.max(tif))  # set the levels to be just above and below the min and max of the entire tif
+                r = (r[0] - (r[1] - r[0]) / 100, r[1] + (r[1] - r[0]) / 100)
+                self.imageview.setLevels(r[0], r[1])
+            else:
+                r = (np.min(tif[self.currentIndex]),
+                     np.max(tif[self.currentIndex]))  # set the levels to be just above and below the min and max of the first frame
+                r = (r[0] - (r[1] - r[0]) / 100, r[1] + (r[1] - r[0]) / 100)
+                self.imageview.setLevels(r[0], r[1])
+        elif self.nDims == 4 and not self.metadata['is_rgb']:
+            if np.min(tif) == 0 and (np.max(tif) == 0 or np.max(tif) == 1):  # if the image is binary (either all 0s or 0s and 1s)
+                self.imageview.setLevels(-.01, 1.01)  # set levels from slightly below 0 to 1
+
+    def set_bg_im(self):
+        self.bg_im_dialog = Bg_im_dialog(self)
+        self.bg_im_dialog.show()
+
+    def link(self, win):
+        """link(self, win)
+        Linking a window to another means when the current index of one changes, the index of the other will automatically change.
+
+        Args:
+            win (flika.window.Window): The window that will be linked with this one
+        """
+        if win not in self.linkedWindows:
+            self.sigTimeChanged.connect(win.imageview.setCurrentIndex)
+            self.linkedWindows.add(win)
+            win.link(self)
+
+    def unlink(self, win):
+        """unlink(self, win)
+        This unlinks a window from this one.
+
+        Args:
+            win (flika.window.Window): The window that will be unlinked from this one
+        """
+        if win in self.linkedWindows:
+            self.linkedWindows.remove(win)
+            self.sigTimeChanged.disconnect(win.imageview.setCurrentIndex)
+            win.unlink(self)
+
+    def link_toggled(self, win):
+        return lambda b: self.link(win) if b else self.unlink(win)
+
+    def make_link_menu(self):
+        self.linkMenu.clear()
+        for win in g.windows:
+            if win == self or not win.isVisible():
+                continue
+            win_action = QtWidgets.QAction("%s" % win.name, self.linkMenu, checkable=True)
+            win_action.setChecked(win in self.linkedWindows)
+            win_action.toggled.connect(self.link_toggled(win))
+            self.linkMenu.addAction(win_action)
+        
+    def updateindex(self):
+        if self.mt == 1:
+            t = 0
+        else:
+            (idx, t) = self.imageview.timeIndex(self.imageview.timeLine)
+            t = int(np.floor(t))
+        if 0 <= t < self.mt:
+            self.currentIndex = t
+            if not g.settings['show_all_points']:
+                pointSizes = [pt[3] for pt in self.scatterPoints[t]]
+                brushes = [pg.mkBrush(*pt[2].getRgb()) for pt in self.scatterPoints[t]]
+                self.scatterPlot.setData(pos=self.scatterPoints[t], size=pointSizes, brush=brushes)
+            self.sigTimeChanged.emit(t)
+
+    def setIndex(self, index):
+        """setIndex(self, index)
+        This sets the index (frame) of this window. 
+
+        Args:
+            index (int): The index of the image this window will display
+        """
+        if hasattr(self, 'image') and self.image.ndim > 2 and 0 <= index < len(self.image):
+            self.imageview.setCurrentIndex(index)
+
+    def showFrame(self, index):
+        if index>=0 and index<self.mt:
+            msg = 'frame {}'.format(index)
+            if 'timestamps' in self.metadata and self.metadata['timestamp_units']=='ms':
+                ttime = self.metadata['timestamps'][index]
+                if ttime < 1*1000:
+                    msg += '; {:.4f} ms'.format(ttime)
+                elif ttime < 60*1000:
+                    seconds = ttime / 1000
+                    msg += '; {:.4f} s'.format(seconds)
+                elif ttime < 3600*1000:
+                    minutes = int(np.floor(ttime / (60*1000)))
+                    seconds = (ttime/1000) % 60
+                    msg += '; {} m {:.4f} s'.format(minutes, seconds)
+                else:
+                    seconds = ttime/1000
+                    hours = int(np.floor(seconds / 3600))
+                    mminutes = seconds - hours * 3600
+                    minutes = int(np.floor(mminutes / 60))
+                    seconds = mminutes - minutes * 60
+                    msg += '; {} h {} m {:.4f} s'.format(hours, minutes, seconds)
+            g.m.statusBar().showMessage(msg)
+
+    def setName(self,name):
+        """setName(self,name)
+        Set the name of this window.
+
+        Args:
+            name (str): the name for window to be set to
+        """
+        name = str(name)
+        self.name = name
+        self.setWindowTitle(name)
+        
+    def reset(self):
+        if not self.closed:
+            currentIndex = int(self.currentIndex)
+            self.imageview.setImage(self.image, autoLevels=True) #I had autoLevels=False before.  I changed it to adjust after boolean previews.
+            if self.imageview.axes['t'] is not None:
+                self.imageview.setCurrentIndex(currentIndex)
+            g.m.statusBar().showMessage('')
+
+    def closeEvent(self, event):
+        if self.closed:
+            print('Attempt to close window {} that was already closed'.format(self))
+            event.accept()
+        else:
+            self.closeSignal.emit()
+            for win in list(self.linkedWindows):
+                self.unlink(win)
+            if hasattr(self,'image'):
+                del self.image
+            self.imageview.setImage(np.zeros((2,2))) #clear the memory
+            self.imageview.close()
+            del self.imageview
+            if g.win==self:
+                g.win=None
+            if self in g.windows:
+                g.windows.remove(self)
+            self.closed=True
+            event.accept() # let the window close
+
+    def imageArray(self):
+        """imageArray(self)
+
+        Returns:
+             Image as a 3d array, correcting for color or 2d image
+        """
+        tif = self.image
+        nDims = len(tif.shape)
+        if nDims == 4:  # If this is an RGB image stack  #[t, x, y, colors]
+            tif = np.mean(tif,3)
+            mx, my = tif[0, :, :].shape
+        elif nDims == 3:
+            if self.metadata['is_rgb']:  # [x, y, colors]
+                tif = np.mean(tif,2)
+                mx, my = tif.shape
+                tif = tif[np.newaxis]
+            else: 
+                mx, my = tif[0,:,:].shape
+        elif nDims == 2:
+            mx, my = tif.shape
+            tif = tif[np.newaxis]
+        return tif
+
+    def imageDimensions(self):
+        nDims = self.image.shape
+        if len(nDims) == 4: #if this is an RGB image stack
+            return nDims[1:3]
+        elif len(nDims) == 3:
+            if self.metadata['is_rgb']:  # [x, y, colors]
+                return nDims[:2]
+            else:                               # [t, x, y]
+                return nDims[1:]
+        if len(nDims) == 2:  # If this is a static image
+            return nDims
+        return nDims
+
+    def resizeEvent(self, event):
+        event.accept()
+        self.imageview.resize(self.size())
+
+    def paste(self):
+        """ paste(self)
+        This function pastes a ROI from one window into another.
+        The ROIs will be automatically linked using the link() fucntion so that when you alter one of them, the other will be altered in the same way.
+        """
+        def pasteROI(roi):
+            if roi in self.rois:
+                return None
+            if roi.kind == 'rect_line':
+                self.currentROI = makeROI(roi.kind, roi.pts, self, width=roi.width)
+            else:
+                self.currentROI = makeROI(roi.kind, roi.pts, self)
+            if roi in roi.window.rois:
+                self.currentROI.link(roi)
+            return self.currentROI
+
+        if type(g.clipboard) == list:
+            rois = []
+            for roi in g.clipboard:
+                rois.append(pasteROI(roi))
+            return rois
+        else:
+            return pasteROI(g.clipboard)
+        
+    def mousePressEvent(self,ev):
+        ev.accept()
+        self.setAsCurrentWindow()
+
+    def setAsCurrentWindow(self):
+        """setAsCurrentWindow(self)
+        This function sets this window as the current window. There is only one current window. All operations are performed on the
+        current window. The current window can be accessed from the variable ``g.win``. 
+        """
+
+        if g.win is not None:
+            g.win.setStyleSheet("border:1px solid rgb(0, 0, 0); ")
+            g.win.lostFocusSignal.emit()
+        g.win = self
+        g.m.currentWindow = g.win
+        g.currentWindow = g.win
+        if self not in g.windows:
+            g.windows.append(self)
+        g.m.setWindowTitle("flika - {}".format(self.name))
+        self.setStyleSheet("border:1px solid rgb(0, 255, 0); ")
+        g.m.setCurrentWindowSignal.sig.emit()
+        self.gainedFocusSignal.emit()
+    
+    def clickedScatter(self, plot, points):
+        p = points[0]
+        x, y = p.pos()
+        if g.settings['show_all_points']:
+            pts = []
+            for t in np.arange(self.mt):
+                self.scatterPoints[t] = [p for p in self.scatterPoints[t] if not (x == p[0] and y == p[1])]
+                pts.extend(self.scatterPoints[t])
+            pointSizes = [pt[3] for pt in pts]
+            brushes = [pg.mkBrush(*pt[2].getRgb()) for pt in pts]
+            self.scatterPlot.setPoints(pos=pts, size=pointSizes, brush=brushes)
+        else:
+            t = self.currentIndex
+            self.scatterPoints[t] = [p for p in self.scatterPoints[t] if not (x == p[0] and y == p[1])]
+            pointSizes = [pt[3] for pt in self.scatterPoints[t]]
+            brushes = [pg.mkBrush(*pt[2].getRgb()) for pt in self.scatterPoints[t]]
+            self.scatterPlot.setPoints(pos=self.scatterPoints[t], size=pointSizes, brush=brushes)
+
+    def getScatterPts(self):
+        """getScatterPts(self)
+
+        Returns:
+            numpy array: an Nx3 array of scatter points, where N is the number of points. Col0 is frame, Col1 is x, Col2 is y. 
+        """
+        p_out=[]
+        p_in=self.scatterPoints
+        for t in np.arange(len(p_in)):
+            for p in p_in[t]:
+                p_out.append(np.array([t,p[0],p[1]]))
+        p_out=np.array(p_out)
+        return p_out
+
+    def plotAllROIs(self):
+        for roi in self.rois:
+            if roi.traceWindow == None:
+                roi.plot()
+
+    def removeAllROIs(self):
+        for roi in self.rois[:]:
+            roi.delete()
+
+    def addPoint(self, p=None):
+        if p is None:
+            p = [self.currentIndex, self.x, self.y]
+        elif len(p) != 3:
+            raise Exception("addPoint takes a 3-tuple (t, x, y) as argument")
+
+        t, x, y = p
+
+        pointSize=g.m.settings['point_size']
+        pointColor = QtGui.QColor(g.settings['point_color'])
+        position=[x, y, pointColor, pointSize]
+        self.scatterPoints[t].append(position)
+        self.scatterPlot.addPoints(pos=[[x, y]], size=pointSize, brush=pg.mkBrush(*pointColor.getRgb()))
+
+    def mouseClickEvent(self, ev):
+        ''''mouseClickevent(self, ev)
+        Event handler for when the mouse is pressed in a flika window.
+        '''
+        self.EEEE = ev
+        if self.x is not None and self.y is not None and ev.button() == QtCore.Qt.RightButton and not self.creatingROI:
+            mm = g.settings['mousemode']
+            if mm == 'point':
+                self.addPoint()
+            elif mm == 'rectangle' and g.settings['default_roi_on_click']:
+                pts = [pg.Point(self.x - g.settings['rect_width']/2, self.y - g.settings['rect_height']/2), pg.Point(g.settings['rect_width'], g.settings['rect_height'])]
+                self.currentROI = makeROI("rectangle", pts)
+            else:
+                self.menu.exec_(ev.screenPos().toQPoint())
+        elif self.creatingROI:
+            self.currentROI.cancel()
+            self.creatingROI = None
+
+    def save_rois(self, filename=None):
+        """save_rois(self, filename=None)
+
+        Args:
+            filename (str): The filename, including the full path, where the ROI file will be saved.
+
+        """
+        if not isinstance(filename, str):
+            if filename is not None and os.path.isfile(filename):
+                filename = os.path.splitext(g.settings['filename'])[0]
+                filename = save_file_gui('Save ROI', filename, '*.txt')
+            else:
+                filename = save_file_gui('Save ROI', '', '*.txt')
+
+        if filename != '' and isinstance(filename, str):
+            reprs = [roi._str() for roi in self.rois]
+            reprs = '\n'.join(reprs)
+            open(filename, 'w').write(reprs)
+        else:
+            g.m.statusBar().showMessage('No File Selected')
+
+    
+    def keyPressEvent(self, ev):
+        if ev.key() == QtCore.Qt.Key_Delete:
+            i = 0
+            while i < len(self.rois):
+                if self.rois[i].mouseHovering:
+                    self.rois[i].delete()
+                else:
+                    i += 1
+        self.keyPressSignal.emit(ev)
+        
+    def mouseMoved(self,point):
+        '''mouseMoved(self,point)
+        Event handler function for mouse movement.
+        '''
+        point=self.imageview.getImageItem().mapFromScene(point)
+        self.point = point
+        self.x = point.x()
+        self.y = point.y()
+        image=self.imageview.getImageItem().image
+        if self.x < 0 or self.y < 0 or self.x >= image.shape[0] or self.y >= image.shape[1]:
+            pass# if we are outside the image
+        else:
+            z=self.imageview.currentIndex
+            value=image[int(self.x),int(self.y)]
+            g.m.statusBar().showMessage('x={}, y={}, z={}, value={}'.format(int(self.x),int(self.y),z,value))
+
+    def mouseDragEvent(self, ev):
+        modifiers = QtWidgets.QApplication.keyboardModifiers()
+        if modifiers == QtCore.Qt.ShiftModifier:
+            pass #This is how I detect that the shift key is held down.
+        if ev.button() == QtCore.Qt.LeftButton:
+            ev.accept()
+            if g.settings['mousemode'] == 'pencil':
+                if ev.isStart():
+                    self.last_x = None
+                    self.last_y = None
+                else:
+                    if self.x < 0 or self.y < 0 or self.x >= self.mx or self.y >= self.my:
+                        self.last_x = None  # if we are outside the image
+                        self.last_y = None
+                    else:
+                        x = int(self.x)
+                        y = int(self.y)
+                        if self.last_x == x and self.last_y == y:
+                            pass
+                        z = self.imageview.currentIndex
+                        image = self.imageview.getImageItem().image
+                        v = g.settings['pencil_value']
+                        if self.last_x is None:
+                            image[x, y] = v
+                        else:
+                            xs, ys = get_line(x, y, self.last_x, self.last_y).T
+                            image[xs, ys] = v
+                        self.imageview.imageItem.updateImage(image)
+                        self.last_x = x
+                        self.last_y = y
+                        self.ev = ev
+            else:
+                difference=self.imageview.getImageItem().mapFromScene(ev.lastScenePos())-self.imageview.getImageItem().mapFromScene(ev.scenePos())
+                self.imageview.view.translateBy(difference)
+        if ev.button() == QtCore.Qt.RightButton:
+            ev.accept()
+            mm = g.settings['mousemode']
+            if mm in ('freehand', 'line', 'rectangle', 'rect_line'):
+                if ev.isStart():
+                    self.ev = ev
+                    pt = self.imageview.getImageItem().mapFromScene(ev.buttonDownScenePos())
+                    self.x = pt.x()  # This sets x and y to the button down position, not the current position.
+                    self.y = pt.y()
+                    self.creatingROI = True
+                    self.currentROI = ROI_Drawing(self, self.x, self.y, mm)
+                if ev.isFinish():
+                    if self.creatingROI:   
+                        if ev._buttons | QtCore.Qt.RightButton != ev._buttons:
+                            self.currentROI = self.currentROI.drawFinished()
+                            self.creatingROI = False
+                        else:
+                            self.currentROI.cancel()
+                            self.creatingROI = False
+                else:  # If we are in the middle of the drag between starting and finishing.
+                    if self.creatingROI:
+                        self.currentROI.extend(self.x, self.y)
+
+    def updateTimeStampLabel(self,frame):
+        label = self.timeStampLabel
+        if self.framerate == 0:
+            label.setHtml("<span style='font-size: 12pt;color:white;background-color:None;'>Frame rate is 0 Hz</span>" )
+            return False
+        ttime = frame/self.framerate  # Time elapsed since the first frame until the current frame, in seconds.
+        if ttime < 1:
+            ttime = ttime * 1000
+            label.setHtml("<span style='font-size: 12pt;color:white;background-color:None;'>{:.0f} ms</span>".format(ttime))
+        elif ttime < 60:
+            label.setHtml("<span style='font-size: 12pt;color:white;background-color:None;'>{:.3f} s</span>".format(ttime))
+        elif ttime < 3600:
+            minutes = int(np.floor(ttime/60))
+            seconds = ttime % 60
+            label.setHtml("<span style='font-size: 12pt;color:white;background-color:None;'>{}m {:.3f} s</span>".format(minutes,seconds))
+        else:
+            hours = int(np.floor(ttime/3600))
+            mminutes = ttime-hours*3600
+            minutes = int(np.floor(mminutes/60))
+            seconds = mminutes-minutes*60
+            label.setHtml("<span style='font-size: 12pt;color:white;background-color:None;'>{}h {}m {:.3f} s</span>".format(hours,minutes,seconds))
+
+
+def get_line(x1, y1, x2, y2):
+    """Bresenham's Line Algorithm
+    Produces a list of tuples """
+    # Setup initial conditions
+    dx = x2 - x1
+    dy = y2 - y1
+
+    # Determine how steep the line is
+    is_steep = abs(dy) > abs(dx)
+
+    # Rotate line
+    if is_steep:
+        x1, y1 = y1, x1
+        x2, y2 = y2, x2
+
+    # Swap start and end points if necessary and store swap state
+    swapped = False
+    if x1 > x2:
+        x1, x2 = x2, x1
+        y1, y2 = y2, y1
+        swapped = True
+
+    # Recalculate differentials
+    dx = x2 - x1
+    dy = y2 - y1
+
+    # Calculate error
+    error = int(dx / 2.0)
+    ystep = 1 if y1 < y2 else -1
+
+    # Iterate over bounding box generating points between start and end
+    y = y1
+    points = []
+    for x in range(x1, x2 + 1):
+        coord = [y, x] if is_steep else [x, y]
+        points.append(coord)
+        error -= abs(dy)
+        if error < 0:
+            y += ystep
+            error += dx
+
+    # Reverse the list if the coordinates were swapped
+    if swapped:
+        points.reverse()
+    return np.array(points)
+
+logger.debug("Completed 'reading window.py'")
```

### Comparing `flika-0.2.9/setup.py` & `flika-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,108 +1,109 @@
-#!/usr/bin/env python
-"""
-Commands to upload to pypi:
-
-python setup.py sdist bdist_wheel
-twine upload dist/*
-"""
-from setuptools import setup, find_packages
-from distutils.core import Command
-from setuptools.command.install import install
-import platform
-import os
-import sys
-
-with open('flika/version.py') as infile:
-    __version__ = '0.0.0'
-    exec(infile.read())  # This sets the __version__ variable.
-
-with open('README.rst') as readme:
-    LONG_DESCRIPTION = readme.read()
-    LONG_DESCRIPTION = LONG_DESCRIPTION.replace('.. image:: flika/docs/_static/img/flika_screencapture.gif', '')
-
-cmdclass = {}
-
-
-class PyTest(Command):
-
-    user_options = [('pytest-args=', 'a', "Arguments to pass to py.test")]
-
-    def initialize_options(self):
-        self.pytest_args = ""
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        # import here, cause outside the eggs aren't loaded
-        import pytest
-        errno = pytest.main(self.pytest_args + ' flika')
-        sys.exit(errno)
-
-
-cmdclass['test'] = PyTest
-
-entry_points = """
-[console_scripts]
-flika = flika.flika:exec_
-flika_post_install = flika.flika:post_install
-"""
-
-setup_requires = ['numpy', 'scipy']
-
-# must have numpy and scipy installed already
-install_requires = [
-      'pandas>=0.14',
-      'matplotlib>=1.4',
-      'pyqtgraph>=0.9',
-      'qtpy>=1.1',
-      'setuptools>=1.0',
-      'scikit-image',
-      'scikit-learn',
-      'ipython>=1.0',
-      'ipykernel',
-      'qtconsole',
-      'pyopengl',
-      'nd2reader']
-
-if sys.platform == 'win32':
-    install_requires += ['winshell', 'pypiwin32']
-
-
-
-setup(name='flika',
-      version=__version__,
-      cmdclass=cmdclass,
-      description='An interactive image processing program for biologists written in Python.',
-      long_description=LONG_DESCRIPTION,
-      author='Kyle Ellefsen, Brett Settle',
-      author_email='kyleellefsen@gmail.com',
-      url='http://flika-org.github.io',
-      setup_requires=setup_requires,
-      install_requires=install_requires,
-      license='MIT',
-      classifiers=[
-          'Intended Audience :: Science/Research',
-          'Operating System :: OS Independent',
-          'Programming Language :: Python',
-          'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.3',
-          'Programming Language :: Python :: 3.4',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
-          'Topic :: Scientific/Engineering :: Visualization',
-          ],
-      packages=find_packages(),
-      entry_points=entry_points,
-      include_package_data=True,
-      package_data={'gui': ['*.ui'],
-                    'images': ['*.ico', '*.png', '*.txt', '*.tif']})
-
-
-
-
-
-
-
-
-
+#!/usr/bin/env python
+"""
+Commands to upload to pypi:
+
+python setup.py sdist bdist_wheel
+twine upload dist/*
+"""
+from setuptools import setup, find_packages
+from distutils.core import Command
+from setuptools.command.install import install
+import platform
+import os
+import sys
+
+with open('flika/version.py') as version_file:
+    __version__ = '0.0.0'
+    exec(version_file.read())  # This sets the __version__ variable.
+
+with open('README.rst') as readme:
+    LONG_DESCRIPTION = readme.read()
+    LONG_DESCRIPTION = LONG_DESCRIPTION.replace('.. image:: flika/docs/_static/img/flika_screencapture.gif', '')
+
+cmdclass = {}
+
+
+class PyTest(Command):
+
+    user_options = [('pytest-args=', 'a', "Arguments to pass to py.test")]
+
+    def initialize_options(self):
+        self.pytest_args = ""
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        # import here, cause outside the eggs aren't loaded
+        import pytest
+        errno = pytest.main(self.pytest_args + ' flika')
+        sys.exit(errno)
+
+
+cmdclass['test'] = PyTest
+
+entry_points = """
+[console_scripts]
+flika = flika.flika:exec_
+flika_post_install = flika.flika:post_install
+"""
+
+setup_requires = ['numpy', 'scipy']
+
+# must have numpy and scipy installed already
+install_requires = [
+      'pandas>=0.14',
+      'matplotlib>=1.4',
+      'pyqtgraph>=0.9',
+      'PyQt6',
+      'qtpy>=1.1',
+      'pyqt6-tools',
+      'setuptools>=1.0',
+      'scikit-image>0.13.0',
+      'scikit-learn',
+      'ipython>=1.0',
+      'ipykernel',
+      'qtconsole',
+      'pyopengl',
+      'requests',
+      'nd2reader',
+      'markdown']
+
+extras_require = {
+    ':sys_platform == "win32"': ['winshell', 'pypiwin32']
+}
+
+setup(name='flika',
+      version=__version__,
+      cmdclass=cmdclass,
+      description='An interactive image processing program for biologists written in Python.',
+      long_description=LONG_DESCRIPTION,
+      author='Kyle Ellefsen, Brett Settle',
+      author_email='kyleellefsen@gmail.com',
+      url='http://flika-org.github.io',
+      setup_requires=setup_requires,
+      install_requires=install_requires,
+      extras_require=extras_require,
+      license='MIT',
+      classifiers=[
+          'Intended Audience :: Science/Research',
+          'Operating System :: OS Independent',
+          'Programming Language :: Python',
+          'Programming Language :: Python :: 3',
+          'Programming Language :: Python :: 3.11',
+          'Topic :: Scientific/Engineering :: Visualization',
+          ],
+      packages=find_packages(),
+      entry_points=entry_points,
+      include_package_data=True,
+      package_data={'gui': ['*.ui'],
+                    'images': ['*.ico', '*.png', '*.txt', '*.tif']})
+
+
+
+
+
+
+
+
+
```

