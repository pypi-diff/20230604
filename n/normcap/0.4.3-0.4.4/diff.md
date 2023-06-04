# Comparing `tmp/normcap-0.4.3.tar.gz` & `tmp/normcap-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normcap-0.4.3.tar", max compression
+gzip compressed data, was "normcap-0.4.4.tar", max compression
```

## Comparing `normcap-0.4.3.tar` & `normcap-0.4.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0    14292 2023-06-03 18:44:49.584327 normcap-0.4.3/CHANGELOG
--rw-r--r--   0        0        0      724 2023-06-03 18:44:49.584327 normcap-0.4.3/LICENSE
--rw-r--r--   0        0        0     6999 2023-06-03 18:44:49.584327 normcap-0.4.3/README.md
--rw-r--r--   0        0        0       46 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/__init__.py
--rw-r--r--   0        0        0      113 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/__main__.py
--rw-r--r--   0        0        0     1673 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/app.py
--rw-r--r--   0        0        0      450 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/clipboard/__init__.py
--rw-r--r--   0        0        0     1440 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/clipboard/linux.py
--rw-r--r--   0        0        0      588 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/clipboard/macos.py
--rw-r--r--   0        0        0      284 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/clipboard/qt.py
--rw-r--r--   0        0        0     5885 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/clipboard/windows.py
--rw-r--r--   0        0        0        0 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/gui/__init__.py
--rw-r--r--   0        0        0     8491 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/gui/constants.py
--rw-r--r--   0        0        0     2356 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/gui/downloader.py
--rw-r--r--   0        0        0     8359 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/gui/language_manager.py
--rw-r--r--   0        0        0     2753 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/loading_indicator.py
--rw-r--r--   0        0        0    10108 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/menu_button.py
--rw-r--r--   0        0        0     3481 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/models.py
--rw-r--r--   0        0        0     3949 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/notifier.py
--rw-r--r--   0        0        0   217598 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/resources.py
--rw-r--r--   0        0        0     3552 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/settings.py
--rw-r--r--   0        0        0     6205 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/system_info.py
--rw-r--r--   0        0        0    20934 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/tray.py
--rw-r--r--   0        0        0     4568 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/update_check.py
--rw-r--r--   0        0        0      758 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/utils.py
--rw-r--r--   0        0        0    11944 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/window.py
--rw-r--r--   0        0        0       93 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/__init__.py
--rw-r--r--   0        0        0     3603 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/enhance.py
--rw-r--r--   0        0        0       46 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/__init__.py
--rw-r--r--   0        0        0      870 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/base_magic.py
--rw-r--r--   0        0        0     1807 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/email_magic.py
--rw-r--r--   0        0        0     2463 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/magic.py
--rw-r--r--   0        0        0     1048 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/multi_line_magic.py
--rw-r--r--   0        0        0     1546 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/paragraph_magic.py
--rw-r--r--   0        0        0      964 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/single_line_magic.py
--rw-r--r--   0        0        0     2699 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/url_magic.py
--rw-r--r--   0        0        0     5121 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/models.py
--rw-r--r--   0        0        0     1535 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/recognize.py
--rw-r--r--   0        0        0     3321 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/__init__.py
--rw-r--r--   0        0        0    13773 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/normcap.png
--rw-r--r--   0        0        0    24936 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/normcap.svg
--rw-r--r--   0        0        0     9267 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/notification.png
--rw-r--r--   0        0        0    16576 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/notification.svg
--rw-r--r--   0        0        0     9267 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/parse.png
--rw-r--r--   0        0        0    16576 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/parse.svg
--rw-r--r--   0        0        0     2982 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/raw.png
--rw-r--r--   0        0        0    14953 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/raw.svg
--rw-r--r--   0        0        0      528 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/resources.qrc
--rw-r--r--   0        0        0    17968 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/settings.png
--rw-r--r--   0        0        0    13793 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/settings.svg
--rw-r--r--   0        0        0    17311 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/tray.png
--rw-r--r--   0        0        0    16523 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/tray.svg
--rw-r--r--   0        0        0       79 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/tessdata/.keep
--rw-r--r--   0        0        0    11358 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/tessdata/LICENSE.txt
--rw-r--r--   0        0        0     1081 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/tessdata/README.txt
--rw-r--r--   0        0        0     1242 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/screengrab/__init__.py
--rw-r--r--   0        0        0     7298 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/screengrab/dbus_portal.py
--rw-r--r--   0        0        0     1816 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/screengrab/dbus_shell.py
--rw-r--r--   0        0        0      461 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/screengrab/qt.py
--rw-r--r--   0        0        0     5512 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/screengrab/utils.py
--rw-r--r--   0        0        0     7611 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/utils.py
--rw-r--r--   0        0        0     6967 2023-06-03 18:44:49.912332 normcap-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     8440 1970-01-01 00:00:00.000000 normcap-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    14442 2023-06-04 10:34:41.478260 normcap-0.4.4/CHANGELOG
+-rw-r--r--   0        0        0      724 2023-06-04 10:34:41.478260 normcap-0.4.4/LICENSE
+-rw-r--r--   0        0        0     6999 2023-06-04 10:34:41.478260 normcap-0.4.4/README.md
+-rw-r--r--   0        0        0       46 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/__init__.py
+-rw-r--r--   0        0        0      113 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/__main__.py
+-rw-r--r--   0        0        0     1673 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/app.py
+-rw-r--r--   0        0        0      450 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/clipboard/__init__.py
+-rw-r--r--   0        0        0     1440 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/clipboard/linux.py
+-rw-r--r--   0        0        0      588 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/clipboard/macos.py
+-rw-r--r--   0        0        0      284 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/clipboard/qt.py
+-rw-r--r--   0        0        0     5885 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/clipboard/windows.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/__init__.py
+-rw-r--r--   0        0        0     8491 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/constants.py
+-rw-r--r--   0        0        0     2356 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/downloader.py
+-rw-r--r--   0        0        0     8359 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/language_manager.py
+-rw-r--r--   0        0        0     2753 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/loading_indicator.py
+-rw-r--r--   0        0        0    10108 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/menu_button.py
+-rw-r--r--   0        0        0     3481 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/models.py
+-rw-r--r--   0        0        0     3949 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/notifier.py
+-rw-r--r--   0        0        0   217598 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/resources.py
+-rw-r--r--   0        0        0     3552 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/settings.py
+-rw-r--r--   0        0        0     6205 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/system_info.py
+-rw-r--r--   0        0        0    21173 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/tray.py
+-rw-r--r--   0        0        0     4568 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/update_check.py
+-rw-r--r--   0        0        0      758 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/utils.py
+-rw-r--r--   0        0        0    11944 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/gui/window.py
+-rw-r--r--   0        0        0       93 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/ocr/__init__.py
+-rw-r--r--   0        0        0     3603 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/ocr/enhance.py
+-rw-r--r--   0        0        0       46 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/ocr/magics/__init__.py
+-rw-r--r--   0        0        0      870 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/ocr/magics/base_magic.py
+-rw-r--r--   0        0        0     1807 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/ocr/magics/email_magic.py
+-rw-r--r--   0        0        0     2463 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/ocr/magics/magic.py
+-rw-r--r--   0        0        0     1048 2023-06-04 10:34:41.842254 normcap-0.4.4/normcap/ocr/magics/multi_line_magic.py
+-rw-r--r--   0        0        0     1546 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/ocr/magics/paragraph_magic.py
+-rw-r--r--   0        0        0      964 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/ocr/magics/single_line_magic.py
+-rw-r--r--   0        0        0     2699 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/ocr/magics/url_magic.py
+-rw-r--r--   0        0        0     5121 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/ocr/models.py
+-rw-r--r--   0        0        0     1535 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/ocr/recognize.py
+-rw-r--r--   0        0        0     3321 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/__init__.py
+-rw-r--r--   0        0        0    13773 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/normcap.png
+-rw-r--r--   0        0        0    24936 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/normcap.svg
+-rw-r--r--   0        0        0     9267 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/notification.png
+-rw-r--r--   0        0        0    16576 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/notification.svg
+-rw-r--r--   0        0        0     9267 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/parse.png
+-rw-r--r--   0        0        0    16576 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/parse.svg
+-rw-r--r--   0        0        0     2982 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/raw.png
+-rw-r--r--   0        0        0    14953 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/raw.svg
+-rw-r--r--   0        0        0      528 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/resources.qrc
+-rw-r--r--   0        0        0    17968 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/settings.png
+-rw-r--r--   0        0        0    13793 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/settings.svg
+-rw-r--r--   0        0        0    17311 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/tray.png
+-rw-r--r--   0        0        0    16523 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/icons/tray.svg
+-rw-r--r--   0        0        0       79 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/tessdata/.keep
+-rw-r--r--   0        0        0    11358 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/tessdata/LICENSE.txt
+-rw-r--r--   0        0        0     1081 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/resources/tessdata/README.txt
+-rw-r--r--   0        0        0     1242 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/screengrab/__init__.py
+-rw-r--r--   0        0        0     7298 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/screengrab/dbus_portal.py
+-rw-r--r--   0        0        0     1816 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/screengrab/dbus_shell.py
+-rw-r--r--   0        0        0      461 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/screengrab/qt.py
+-rw-r--r--   0        0        0     5512 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/screengrab/utils.py
+-rw-r--r--   0        0        0     7628 2023-06-04 10:34:41.846253 normcap-0.4.4/normcap/utils.py
+-rw-r--r--   0        0        0     6967 2023-06-04 10:34:41.850253 normcap-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     8440 1970-01-01 00:00:00.000000 normcap-0.4.4/PKG-INFO
```

### Comparing `normcap-0.4.3/CHANGELOG` & `normcap-0.4.4/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## v0.4.4 (2023-06-04)
+
+- All: Fix regression causing exit through system tray not working.
+  ([#458](https://github.com/dynobo/normcap/issues/458))
+
 ## v0.4.3 (2023-06-03)
 
 - All: Add command line flag `--background-mode` to start normcap minimized
   ([#439](https://github.com/dynobo/normcap/issues/439))
 - macOS: Improve dialog that is shown in case screenshot permissions are missing.
 - Windows: Fix upgrading with `msi`-installer might lead to error on startup.
   ([#452](https://github.com/dynobo/normcap/issues/452))
```

### Comparing `normcap-0.4.3/LICENSE` & `normcap-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/README.md` & `normcap-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 [![Screencast](https://user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/assets/normcap.gif)
 
 ## Quickstart
 
 Install a prebuilt release:
 
 - **Windows**:
-  [NormCap-0.4.3-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64-Windows.msi)
+  [NormCap-0.4.4-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-0.4.4-x86_64-Windows.msi)
 - **Linux**:
-  [NormCap-0.4.3-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64.AppImage)
+  [NormCap-0.4.4-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-0.4.4-x86_64.AppImage)
 - **macOS** (x86) ¹:
-  [NormCap-0.4.3-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64-macOS.dmg)
+  [NormCap-0.4.4-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-0.4.4-x86_64-macOS.dmg)
 - **macOS** (M1) ¹·²:
-  [NormCap-0.4.3-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-arm64-macOS.dmg)
+  [NormCap-0.4.4-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-0.4.4-arm64-macOS.dmg)
   \
   <sub>1: On macOS, allow the unsigned application on first start: "System
   Preferences" → "Security & Privacy" → "General" → "Open anyway". You might also need
   to allow NormCap to take screenshots.
   [#135](https://github.com/dynobo/normcap/issues/135)<br> 2: Might be available a bit
   delayed, as it is currently build manually. (Thx,
   [@Takrin](https://github.com/Takrin)!)</sub>
```

#### html2text {}

```diff
@@ -19,22 +19,22 @@
 (https://github.com/dynobo/normcap) | [Documentation](https://dynobo.github.io/
 normcap/) | [FAQs](https://dynobo.github.io/normcap/#faqs) | [Releases](https:/
 /github.com/dynobo/normcap/releases) | [Changelog](https://github.com/dynobo/
 normcap/blob/main/CHANGELOG) [![Screencast](https://user-
 images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
 assets/normcap.gif) ## Quickstart Install a prebuilt release: - **Windows**:
-[NormCap-0.4.3-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
-download/v0.4.3/NormCap-0.4.3-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.3-
-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.3/
-NormCap-0.4.3-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.3-x86_64-
-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-
-0.4.3-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.3-arm64-
-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-
-0.4.3-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
+[NormCap-0.4.4-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
+download/v0.4.4/NormCap-0.4.4-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.4-
+x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.4/
+NormCap-0.4.4-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.4-x86_64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-
+0.4.4-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.4-arm64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-
+0.4.4-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
 start: "System Preferences" â "Security & Privacy" â "General" â "Open
 anyway". You might also need to allow NormCap to take screenshots. [#135]
 (https://github.com/dynobo/normcap/issues/135)
 2: Might be available a bit delayed, as it is currently build manually. (Thx,
 [@Takrin](https://github.com/Takrin)!) Install from repositories: -
 **Windows**: Install from [Microsoft Store](https://apps.microsoft.com/store/
 detail/normcap/XPDLJNB4B6C2ZR). - **Arch / Manjaro**: Install the [`normcap`]
```

### Comparing `normcap-0.4.3/normcap/app.py` & `normcap-0.4.4/normcap/app.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/clipboard/linux.py` & `normcap-0.4.4/normcap/clipboard/linux.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/clipboard/macos.py` & `normcap-0.4.4/normcap/clipboard/macos.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/clipboard/windows.py` & `normcap-0.4.4/normcap/clipboard/windows.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/constants.py` & `normcap-0.4.4/normcap/gui/constants.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/downloader.py` & `normcap-0.4.4/normcap/gui/downloader.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/language_manager.py` & `normcap-0.4.4/normcap/gui/language_manager.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/loading_indicator.py` & `normcap-0.4.4/normcap/gui/loading_indicator.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/menu_button.py` & `normcap-0.4.4/normcap/gui/menu_button.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/models.py` & `normcap-0.4.4/normcap/gui/models.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/notifier.py` & `normcap-0.4.4/normcap/gui/notifier.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/resources.py` & `normcap-0.4.4/normcap/gui/resources.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/settings.py` & `normcap-0.4.4/normcap/gui/settings.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/system_info.py` & `normcap-0.4.4/normcap/gui/system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/tray.py` & `normcap-0.4.4/normcap/gui/tray.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,15 +443,18 @@
         if bool(self.settings.value("tray", False, type=bool)):
             action = QtGui.QAction("Capture", menu)
             action.setObjectName("capture")
             action.triggered.connect(self.com.on_tray_menu_capture_clicked.emit)
             menu.addAction(action)
 
         action = QtGui.QAction("Exit", menu)
-        action.triggered.connect(self.com.on_quit.emit)
+        # Better would be: action_exit.triggered.connect(self.com.on_quit.emit)
+        # but that strangly doesn't work anymore since PySide 6.5.1 and will tigger
+        # the capture acture instead...?!
+        action.triggered.connect(lambda: self._exit_application("clicked exit in tray"))
         menu.addAction(action)
 
     def _create_next_window(self) -> None:
         """Open child window only for next display."""
         if len(system_info.screens()) > len(self.windows):
             index = len(self.windows.keys())
             self._create_window(index)
```

### Comparing `normcap-0.4.3/normcap/gui/update_check.py` & `normcap-0.4.4/normcap/gui/update_check.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/utils.py` & `normcap-0.4.4/normcap/gui/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/gui/window.py` & `normcap-0.4.4/normcap/gui/window.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/enhance.py` & `normcap-0.4.4/normcap/ocr/enhance.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/magics/base_magic.py` & `normcap-0.4.4/normcap/ocr/magics/base_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/magics/email_magic.py` & `normcap-0.4.4/normcap/ocr/magics/email_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/magics/magic.py` & `normcap-0.4.4/normcap/ocr/magics/magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/magics/multi_line_magic.py` & `normcap-0.4.4/normcap/ocr/magics/multi_line_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/magics/paragraph_magic.py` & `normcap-0.4.4/normcap/ocr/magics/paragraph_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/magics/single_line_magic.py` & `normcap-0.4.4/normcap/ocr/magics/single_line_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/magics/url_magic.py` & `normcap-0.4.4/normcap/ocr/magics/url_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/models.py` & `normcap-0.4.4/normcap/ocr/models.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/recognize.py` & `normcap-0.4.4/normcap/ocr/recognize.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/ocr/tesseract.py` & `normcap-0.4.4/normcap/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/normcap.png` & `normcap-0.4.4/normcap/resources/icons/normcap.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/normcap.svg` & `normcap-0.4.4/normcap/resources/icons/normcap.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/notification.png` & `normcap-0.4.4/normcap/resources/icons/notification.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/notification.svg` & `normcap-0.4.4/normcap/resources/icons/notification.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/parse.png` & `normcap-0.4.4/normcap/resources/icons/parse.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/parse.svg` & `normcap-0.4.4/normcap/resources/icons/parse.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/raw.png` & `normcap-0.4.4/normcap/resources/icons/raw.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/raw.svg` & `normcap-0.4.4/normcap/resources/icons/raw.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/resources.qrc` & `normcap-0.4.4/normcap/resources/icons/resources.qrc`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/settings.png` & `normcap-0.4.4/normcap/resources/icons/settings.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/settings.svg` & `normcap-0.4.4/normcap/resources/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/tray.png` & `normcap-0.4.4/normcap/resources/icons/tray.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/icons/tray.svg` & `normcap-0.4.4/normcap/resources/icons/tray.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/tessdata/LICENSE.txt` & `normcap-0.4.4/normcap/resources/tessdata/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/resources/tessdata/README.txt` & `normcap-0.4.4/normcap/resources/tessdata/README.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/screengrab/__init__.py` & `normcap-0.4.4/normcap/screengrab/__init__.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/screengrab/dbus_portal.py` & `normcap-0.4.4/normcap/screengrab/dbus_portal.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/screengrab/dbus_shell.py` & `normcap-0.4.4/normcap/screengrab/dbus_shell.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/screengrab/utils.py` & `normcap-0.4.4/normcap/screengrab/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.3/normcap/utils.py` & `normcap-0.4.4/normcap/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,15 @@
 from normcap.gui import system_info
 from normcap.gui.settings import DEFAULT_SETTINGS
 
 logger = logging.getLogger("normcap")
 
 
 _ISSUES_URLS = "https://github.com/dynobo/normcap/issues"
-_XCB_ERROR_URL = (
-    "https://github.com/dynobo/normcap/blob/main/FAQ.md"
-    "#linux-could-not-load-the-qt-platform-plugin-xcb",
-)
+_XCB_ERROR_URL = "https://dynobo.github.io/normcap/#faqs-couldnt-load-platform-plugin"
 
 
 def create_argparser() -> argparse.ArgumentParser:
     """Parse command line arguments."""
     parser = argparse.ArgumentParser(
         prog="normcap",
         description=(
@@ -212,16 +209,19 @@
 
     if (level == "qtfatalmsg") or ("could not load the qt platform" in msg):
         logger.error("[QT] %s - %s", level, msg)
     else:
         logger.debug("[QT] %s - %s", level, msg)
 
     if ("xcb" in msg) and ("it was found" in msg):
-        logger.error("Try solving the problem as described here: %s", _XCB_ERROR_URL)
-        logger.error("If that doesn't help, please open an issue: %s", _ISSUES_URLS)
+        logger.error(
+            "Please check if installing additional dependencies might help, see: %s",
+            _XCB_ERROR_URL,
+        )
+        logger.error("If that doesn't solve it, please open an issue: %s", _ISSUES_URLS)
 
 
 def copy_traineddata_files(target_path: Optional[os.PathLike]) -> None:
     if not target_path:
         return
 
     target_path = Path(target_path)
```

### Comparing `normcap-0.4.3/pyproject.toml` & `normcap-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "normcap"
-version = "0.4.3"
+version = "0.4.4"
 description = "OCR-powered screen-capture tool to capture information instead of images."
 keywords = ["screenshot", "ocr", "capture", "clipboard"]
 license = "GPLv3"
 authors = ["dynobo <dynobo@mailbox.org>"]
 readme = "README.md"
 homepage = "https://dynobo.github.io/normcap/"
 repository = "https://github.com/dynobo/normcap"
@@ -156,15 +156,15 @@
 cluster = true
 max_cluster_size = 1
 no_show = true
 
 [tool.briefcase]
 project_name = "NormCap"
 bundle = "eu.dynobo"
-version = "0.4.3"
+version = "0.4.4"
 url = "https://github.com/dynobo/normcap"
 license = "GPLv3"
 author = 'dynobo'
 author_email = "dynobo@mailbox.org"
 
 [tool.briefcase.app.normcap]
 formal_name = "NormCap"
@@ -249,15 +249,15 @@
 template_branch = "main"
 
 [tool.briefcase.app.normcap.windows]
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "0.4.3"
+current = "0.4.4"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   ((?P<extra>.+))?
```

### Comparing `normcap-0.4.3/PKG-INFO` & `normcap-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normcap
-Version: 0.4.3
+Version: 0.4.4
 Summary: OCR-powered screen-capture tool to capture information instead of images.
 Home-page: https://dynobo.github.io/normcap/
 License: GPLv3
 Keywords: screenshot,ocr,capture,clipboard
 Author: dynobo
 Author-email: dynobo@mailbox.org
 Requires-Python: >=3.9,<3.12
@@ -58,21 +58,21 @@
 [![Screencast](https://user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/assets/normcap.gif)
 
 ## Quickstart
 
 Install a prebuilt release:
 
 - **Windows**:
-  [NormCap-0.4.3-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64-Windows.msi)
+  [NormCap-0.4.4-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-0.4.4-x86_64-Windows.msi)
 - **Linux**:
-  [NormCap-0.4.3-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64.AppImage)
+  [NormCap-0.4.4-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-0.4.4-x86_64.AppImage)
 - **macOS** (x86) ¹:
-  [NormCap-0.4.3-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64-macOS.dmg)
+  [NormCap-0.4.4-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-0.4.4-x86_64-macOS.dmg)
 - **macOS** (M1) ¹·²:
-  [NormCap-0.4.3-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-arm64-macOS.dmg)
+  [NormCap-0.4.4-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-0.4.4-arm64-macOS.dmg)
   \
   <sub>1: On macOS, allow the unsigned application on first start: "System
   Preferences" → "Security & Privacy" → "General" → "Open anyway". You might also need
   to allow NormCap to take screenshots.
   [#135](https://github.com/dynobo/normcap/issues/135)<br> 2: Might be available a bit
   delayed, as it is currently build manually. (Thx,
   [@Takrin](https://github.com/Takrin)!)</sub>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: normcap Version: 0.4.3 Summary: OCR-powered screen-
+Metadata-Version: 2.1 Name: normcap Version: 0.4.4 Summary: OCR-powered screen-
 capture tool to capture information instead of images. Home-page: https://
 dynobo.github.io/normcap/ License: GPLv3 Keywords:
 screenshot,ocr,capture,clipboard Author: dynobo Author-email:
 dynobo@mailbox.org Requires-Python: >=3.9,<3.12 Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: End Users/Desktop Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 License :: Other/Proprietary License Classifier: Operating System :: MacOS
@@ -38,22 +38,22 @@
 (https://github.com/dynobo/normcap) | [Documentation](https://dynobo.github.io/
 normcap/) | [FAQs](https://dynobo.github.io/normcap/#faqs) | [Releases](https:/
 /github.com/dynobo/normcap/releases) | [Changelog](https://github.com/dynobo/
 normcap/blob/main/CHANGELOG) [![Screencast](https://user-
 images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
 assets/normcap.gif) ## Quickstart Install a prebuilt release: - **Windows**:
-[NormCap-0.4.3-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
-download/v0.4.3/NormCap-0.4.3-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.3-
-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.3/
-NormCap-0.4.3-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.3-x86_64-
-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-
-0.4.3-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.3-arm64-
-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-
-0.4.3-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
+[NormCap-0.4.4-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
+download/v0.4.4/NormCap-0.4.4-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.4-
+x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.4/
+NormCap-0.4.4-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.4-x86_64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-
+0.4.4-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.4-arm64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.4/NormCap-
+0.4.4-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
 start: "System Preferences" â "Security & Privacy" â "General" â "Open
 anyway". You might also need to allow NormCap to take screenshots. [#135]
 (https://github.com/dynobo/normcap/issues/135)
 2: Might be available a bit delayed, as it is currently build manually. (Thx,
 [@Takrin](https://github.com/Takrin)!) Install from repositories: -
 **Windows**: Install from [Microsoft Store](https://apps.microsoft.com/store/
 detail/normcap/XPDLJNB4B6C2ZR). - **Arch / Manjaro**: Install the [`normcap`]
```

