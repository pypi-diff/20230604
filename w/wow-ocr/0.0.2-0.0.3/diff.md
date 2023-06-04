# Comparing `tmp/wow-ocr-0.0.2.tar.gz` & `tmp/wow-ocr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow-ocr-0.0.2.tar", last modified: Thu Jun  1 17:03:20 2023, max compression
+gzip compressed data, was "wow-ocr-0.0.3.tar", last modified: Sun Jun  4 15:06:23 2023, max compression
```

## Comparing `wow-ocr-0.0.2.tar` & `wow-ocr-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-01 17:03:20.920844 wow-ocr-0.0.2/
--rw-rw-r--   0 user      (1000) user      (1000)     1022 2023-05-31 15:58:44.000000 wow-ocr-0.0.2/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     2653 2023-06-01 17:03:20.920844 wow-ocr-0.0.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      996 2023-06-01 17:01:47.000000 wow-ocr-0.0.2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      925 2023-06-01 17:02:44.000000 wow-ocr-0.0.2/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)      102 2023-06-01 17:03:20.920844 wow-ocr-0.0.2/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-01 17:03:20.916844 wow-ocr-0.0.2/wow_ocr/
--rw-rw-r--   0 user      (1000) user      (1000)       75 2023-06-01 11:11:48.000000 wow-ocr-0.0.2/wow_ocr/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    31392 2023-06-01 16:06:19.000000 wow-ocr-0.0.2/wow_ocr/detector.py
--rw-rw-r--   0 user      (1000) user      (1000)     2779 2023-06-01 11:20:11.000000 wow-ocr-0.0.2/wow_ocr/pipeline.py
--rw-rw-r--   0 user      (1000) user      (1000)    19802 2023-06-01 16:10:07.000000 wow-ocr-0.0.2/wow_ocr/recognizer.py
--rw-rw-r--   0 user      (1000) user      (1000)    12944 2023-06-01 16:57:08.000000 wow-ocr-0.0.2/wow_ocr/tools.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-01 17:03:20.920844 wow-ocr-0.0.2/wow_ocr.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2653 2023-06-01 17:03:20.000000 wow-ocr-0.0.2/wow_ocr.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      295 2023-06-01 17:03:20.000000 wow-ocr-0.0.2/wow_ocr.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-01 17:03:20.000000 wow-ocr-0.0.2/wow_ocr.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      174 2023-06-01 17:03:20.000000 wow-ocr-0.0.2/wow_ocr.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-01 17:03:20.000000 wow-ocr-0.0.2/wow_ocr.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-04 15:06:23.965862 wow-ocr-0.0.3/
+-rw-rw-r--   0 user      (1000) user      (1000)     1022 2023-05-31 15:58:44.000000 wow-ocr-0.0.3/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     2631 2023-06-04 15:06:23.965862 wow-ocr-0.0.3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      974 2023-06-01 17:28:42.000000 wow-ocr-0.0.3/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      925 2023-06-04 15:05:53.000000 wow-ocr-0.0.3/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      102 2023-06-04 15:06:23.965862 wow-ocr-0.0.3/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-04 15:06:23.961862 wow-ocr-0.0.3/wow_ocr/
+-rw-rw-r--   0 user      (1000) user      (1000)       75 2023-06-01 11:11:48.000000 wow-ocr-0.0.3/wow_ocr/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    31392 2023-06-01 16:06:19.000000 wow-ocr-0.0.3/wow_ocr/detector.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2779 2023-06-01 11:20:11.000000 wow-ocr-0.0.3/wow_ocr/pipeline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19802 2023-06-04 15:03:35.000000 wow-ocr-0.0.3/wow_ocr/recognizer.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12944 2023-06-01 17:07:16.000000 wow-ocr-0.0.3/wow_ocr/tools.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-04 15:06:23.965862 wow-ocr-0.0.3/wow_ocr.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2631 2023-06-04 15:06:23.000000 wow-ocr-0.0.3/wow_ocr.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      295 2023-06-04 15:06:23.000000 wow-ocr-0.0.3/wow_ocr.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-04 15:06:23.000000 wow-ocr-0.0.3/wow_ocr.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      174 2023-06-04 15:06:23.000000 wow-ocr-0.0.3/wow_ocr.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-04 15:06:23.000000 wow-ocr-0.0.3/wow_ocr.egg-info/top_level.txt
```

### Comparing `wow-ocr-0.0.2/LICENSE` & `wow-ocr-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wow-ocr-0.0.2/PKG-INFO` & `wow-ocr-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ocr
-Version: 0.0.2
+Version: 0.0.3
 Summary: A packaged OCR model to read texts into WoW screenshots
 Author-email: Geo <geoffrey.menon38@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
@@ -29,15 +29,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 WoW Screenshot OCR
 ==============
 
-Deep learning OCR models to read text from WoW screenshots. Based on a detector that spots text frames from screenshots, and a recognizer that reads text from detected frames.
+Deep learning OCR models to read text from WoW screenshots. Based on a detector that spots text frames, and a recognizer that reads text from detected frames.
 
 - Chat
 - Combat log
 - Nameplates
 - UI frames
 - Map
 
@@ -46,15 +46,15 @@
 
 ### ```pip install wow-ocr```
 
 
 Usage
 ----
 
-Models will use pre trained weights, you don't have to train anything. [Try it on Colab](https://colab.research.google.com/drive/1w4YIS--7qSzdSrwKPcQfqO988PlrxuCM?usp=sharing)
+Models use pre trained weights, you don't have to train anything. [Try it on Colab](https://colab.research.google.com/drive/1w4YIS--7qSzdSrwKPcQfqO988PlrxuCM?usp=sharing)
 
 ```
 import wow_ocr
 
 # Init pipeline, detector and recognizer models with pre trained weights
 pipeline = wow_ocr.pipeline.Pipeline()
```

### Comparing `wow-ocr-0.0.2/README.md` & `wow-ocr-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 WoW Screenshot OCR
 ==============
 
-Deep learning OCR models to read text from WoW screenshots. Based on a detector that spots text frames from screenshots, and a recognizer that reads text from detected frames.
+Deep learning OCR models to read text from WoW screenshots. Based on a detector that spots text frames, and a recognizer that reads text from detected frames.
 
 - Chat
 - Combat log
 - Nameplates
 - UI frames
 - Map
 
@@ -14,15 +14,15 @@
 
 ### ```pip install wow-ocr```
 
 
 Usage
 ----
 
-Models will use pre trained weights, you don't have to train anything. [Try it on Colab](https://colab.research.google.com/drive/1w4YIS--7qSzdSrwKPcQfqO988PlrxuCM?usp=sharing)
+Models use pre trained weights, you don't have to train anything. [Try it on Colab](https://colab.research.google.com/drive/1w4YIS--7qSzdSrwKPcQfqO988PlrxuCM?usp=sharing)
 
 ```
 import wow_ocr
 
 # Init pipeline, detector and recognizer models with pre trained weights
 pipeline = wow_ocr.pipeline.Pipeline()
```

### Comparing `wow-ocr-0.0.2/pyproject.toml` & `wow-ocr-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wow-ocr"
-version = "0.0.2"
+version = "0.0.3"
 description = "A packaged OCR model to read texts into WoW screenshots"
 readme = "README.md"
 authors = [{ name = "Geo", email = "geoffrey.menon38@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `wow-ocr-0.0.2/wow_ocr/detector.py` & `wow-ocr-0.0.3/wow_ocr/detector.py`

 * *Files identical despite different names*

### Comparing `wow-ocr-0.0.2/wow_ocr/pipeline.py` & `wow-ocr-0.0.3/wow_ocr/pipeline.py`

 * *Files identical despite different names*

### Comparing `wow-ocr-0.0.2/wow_ocr/recognizer.py` & `wow-ocr-0.0.3/wow_ocr/recognizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 PRETRAINED_WEIGHTS: typing.Dict[str, typing.Any] = {
     "wow_ocr": {
         "alphabet": DEFAULT_ALPHABET,
         "build_params": DEFAULT_BUILD_PARAMS,
         "weights": {
             "url": "https://github.com/geo-tp/wow-ocr/releases/download/v0.0.1/recognizer_wow_ocr.h5",
             "filename": "recognizer_wow_ocr.h5",
-            "sha256": "0f1af6f1d40abdc551fa46ab478a768dd2a00096fdaa2fa2a124b5ac13d6d0fd",
+            "sha256": "8240eede88bfedbd6bd3b9f42d6305d2e61cc16375183cd789cef6ebe88a4743",
         },
     },
 }
 
 
 def _repeat(x, num_repeats):
     ones = tf.ones((1, num_repeats), dtype="int32")
```

### Comparing `wow-ocr-0.0.2/wow_ocr/tools.py` & `wow-ocr-0.0.3/wow_ocr/tools.py`

 * *Files identical despite different names*

### Comparing `wow-ocr-0.0.2/wow_ocr.egg-info/PKG-INFO` & `wow-ocr-0.0.3/wow_ocr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ocr
-Version: 0.0.2
+Version: 0.0.3
 Summary: A packaged OCR model to read texts into WoW screenshots
 Author-email: Geo <geoffrey.menon38@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
@@ -29,15 +29,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 WoW Screenshot OCR
 ==============
 
-Deep learning OCR models to read text from WoW screenshots. Based on a detector that spots text frames from screenshots, and a recognizer that reads text from detected frames.
+Deep learning OCR models to read text from WoW screenshots. Based on a detector that spots text frames, and a recognizer that reads text from detected frames.
 
 - Chat
 - Combat log
 - Nameplates
 - UI frames
 - Map
 
@@ -46,15 +46,15 @@
 
 ### ```pip install wow-ocr```
 
 
 Usage
 ----
 
-Models will use pre trained weights, you don't have to train anything. [Try it on Colab](https://colab.research.google.com/drive/1w4YIS--7qSzdSrwKPcQfqO988PlrxuCM?usp=sharing)
+Models use pre trained weights, you don't have to train anything. [Try it on Colab](https://colab.research.google.com/drive/1w4YIS--7qSzdSrwKPcQfqO988PlrxuCM?usp=sharing)
 
 ```
 import wow_ocr
 
 # Init pipeline, detector and recognizer models with pre trained weights
 pipeline = wow_ocr.pipeline.Pipeline()
```

