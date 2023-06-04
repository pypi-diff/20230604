# Comparing `tmp/tulyp-0.0.3.tar.gz` & `tmp/tulyp-0.0.4.tar.gz`

## Comparing `tulyp-0.0.3.tar` & `tulyp-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tulyp-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    98978 2020-02-02 00:00:00.000000 tulyp-0.0.3/images/screenshot.png
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/exceptions/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/exceptions/lyrics_not_found.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/lyrics_sources/__init__.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/lyrics_sources/azlyrics.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/lyrics_sources/genius.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/lyrics_sources/google.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/screen/__init__.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/screen/ui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/utils/__init__.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 tulyp-0.0.3/src/tulyp/utils/misc.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tulyp-0.0.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tulyp-0.0.3/LICENSE
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 tulyp-0.0.3/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 tulyp-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 tulyp-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tulyp-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    98978 2020-02-02 00:00:00.000000 tulyp-0.0.4/images/screenshot.png
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/exceptions/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/exceptions/lyrics_not_found.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/lyrics_sources/__init__.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/lyrics_sources/azlyrics.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/lyrics_sources/genius.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/lyrics_sources/google.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/screen/__init__.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/screen/ui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/utils/__init__.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 tulyp-0.0.4/src/tulyp/utils/misc.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tulyp-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 tulyp-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tulyp-0.0.4/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 tulyp-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 tulyp-0.0.4/PKG-INFO
```

### Comparing `tulyp-0.0.3/.github/workflows/python-publish.yml` & `tulyp-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tulyp-0.0.3/images/screenshot.png` & `tulyp-0.0.4/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `tulyp-0.0.3/src/tulyp/__init__.py` & `tulyp-0.0.4/src/tulyp/__init__.py`

 * *Files identical despite different names*

### Comparing `tulyp-0.0.3/src/tulyp/lyrics_sources/azlyrics.py` & `tulyp-0.0.4/src/tulyp/lyrics_sources/azlyrics.py`

 * *Files identical despite different names*

### Comparing `tulyp-0.0.3/src/tulyp/lyrics_sources/genius.py` & `tulyp-0.0.4/src/tulyp/lyrics_sources/genius.py`

 * *Files identical despite different names*

### Comparing `tulyp-0.0.3/src/tulyp/lyrics_sources/google.py` & `tulyp-0.0.4/src/tulyp/lyrics_sources/google.py`

 * *Files identical despite different names*

### Comparing `tulyp-0.0.3/src/tulyp/screen/ui.py` & `tulyp-0.0.4/src/tulyp/screen/ui.py`

 * *Files identical despite different names*

### Comparing `tulyp-0.0.3/src/tulyp/utils/misc.py` & `tulyp-0.0.4/src/tulyp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tulyp-0.0.3/LICENSE` & `tulyp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tulyp-0.0.3/README.md` & `tulyp-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # tulyp
 
-![screenshot](images/screenshot.png)
+![screenshot](https://raw.githubusercontent.com/laszloszurok/tulyp/main/images/screenshot.png)
 
 `tulyp` displays the lyrics of the currently playing song in the terminal.
 It checks for lyrics from 3 sources (stops at the first successful result):
 
 * genius.com
 * google.com
 * azlyrics.com
@@ -30,15 +30,28 @@
 * `lyricsgenius` provides API to get lyrics from genius.com
 * `dbus-python` to get the currently playing song through dbus
 * `requests` to search for lyrincs on google
 * `beautifulsoup4` to extract lyrics from html
 
 ## Install
 
-`pip install tulyp`
+### From PyPi
+
+```shell
+pip install --user tulyp
+```
+
+### From source
+
+```shell
+git clone https://github.com/laszloszurok/tulyp.git
+cd tulyp
+python -m build
+pip install --user dist/tulyp-0.0.3-py3-none-any.whl
+```
 
 ## Naming
 
 * we got a terminal user interface -> tu
 * we are dealing with lyrics       -> ly
 * the program is written in python -> p
```

### Comparing `tulyp-0.0.3/pyproject.toml` & `tulyp-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tulyp"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="pulzar", email="pulzar@envs.net" },
 ]
 description = "Display lyrics of the currently playing song in a terminal."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `tulyp-0.0.3/PKG-INFO` & `tulyp-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulyp
-Version: 0.0.3
+Version: 0.0.4
 Summary: Display lyrics of the currently playing song in a terminal.
 Project-URL: Homepage, https://github.com/laszloszurok/tulyp
 Project-URL: Bug Tracker, https://github.com/laszloszurok/tulyp/issues
 Author-email: pulzar <pulzar@envs.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: dbus-python
 Requires-Dist: lyricsgenius
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # tulyp
 
-![screenshot](images/screenshot.png)
+![screenshot](https://raw.githubusercontent.com/laszloszurok/tulyp/main/images/screenshot.png)
 
 `tulyp` displays the lyrics of the currently playing song in the terminal.
 It checks for lyrics from 3 sources (stops at the first successful result):
 
 * genius.com
 * google.com
 * azlyrics.com
@@ -48,15 +48,28 @@
 * `lyricsgenius` provides API to get lyrics from genius.com
 * `dbus-python` to get the currently playing song through dbus
 * `requests` to search for lyrincs on google
 * `beautifulsoup4` to extract lyrics from html
 
 ## Install
 
-`pip install tulyp`
+### From PyPi
+
+```shell
+pip install --user tulyp
+```
+
+### From source
+
+```shell
+git clone https://github.com/laszloszurok/tulyp.git
+cd tulyp
+python -m build
+pip install --user dist/tulyp-0.0.3-py3-none-any.whl
+```
 
 ## Naming
 
 * we got a terminal user interface -> tu
 * we are dealing with lyrics       -> ly
 * the program is written in python -> p
```

