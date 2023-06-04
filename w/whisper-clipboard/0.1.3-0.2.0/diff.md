# Comparing `tmp/whisper-clipboard-0.1.3.tar.gz` & `tmp/whisper-clipboard-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-clipboard-0.1.3.tar", last modified: Thu Jun  1 23:20:32 2023, max compression
+gzip compressed data, was "whisper-clipboard-0.2.0.tar", last modified: Sun Jun  4 20:50:54 2023, max compression
```

## Comparing `whisper-clipboard-0.1.3.tar` & `whisper-clipboard-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:32.234173 whisper-clipboard-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 23:20:24.000000 whisper-clipboard-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 23:20:32.234173 whisper-clipboard-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-01 23:20:24.000000 whisper-clipboard-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:20:32.234173 whisper-clipboard-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 23:20:24.000000 whisper-clipboard-0.1.3/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2954 2023-06-01 23:20:24.000000 whisper-clipboard-0.1.3/transcribe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:32.234173 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:50:54.077587 whisper-clipboard-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-04 20:50:43.000000 whisper-clipboard-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-04 20:50:54.077587 whisper-clipboard-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-04 20:50:43.000000 whisper-clipboard-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:50:54.077587 whisper-clipboard-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-04 20:50:43.000000 whisper-clipboard-0.2.0/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6486 2023-06-04 20:50:43.000000 whisper-clipboard-0.2.0/transcribe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:50:54.077587 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/top_level.txt
```

### Comparing `whisper-clipboard-0.1.3/LICENSE` & `whisper-clipboard-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-clipboard-0.1.3/PKG-INFO` & `whisper-clipboard-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-clipboard
-Version: 0.1.3
+Version: 0.2.0
 Summary: A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.
 Home-page: http://github.com/data-stepper/whisper-clipboard
 Author: Bent Mueller
 Author-email: bentmuller.ai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `whisper-clipboard-0.1.3/README.md` & `whisper-clipboard-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `whisper-clipboard-0.1.3/setup.py` & `whisper-clipboard-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from os import path
+from pathlib import Path
 
 from setuptools import setup
 
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
+this_directory = Path(__file__).resolve().parent
+
+with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
-with open("requirements.txt") as f:
+with open(this_directory / "requirements.txt") as f:
     requirements = f.read().splitlines()
 
+# Rest of your setup.py code...
+
+
 setup(
     name="whisper-clipboard",
-    version="0.1.3",
+    version="0.2.0",
     description="A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Bent Mueller",
     author_email="bentmuller.ai@gmail.com",
     url="http://github.com/data-stepper/whisper-clipboard",
     py_modules=["transcribe"],
```

### Comparing `whisper-clipboard-0.1.3/whisper_clipboard.egg-info/PKG-INFO` & `whisper-clipboard-0.2.0/whisper_clipboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-clipboard
-Version: 0.1.3
+Version: 0.2.0
 Summary: A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.
 Home-page: http://github.com/data-stepper/whisper-clipboard
 Author: Bent Mueller
 Author-email: bentmuller.ai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

