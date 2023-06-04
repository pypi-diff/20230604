# Comparing `tmp/EdgeGPT-0.8.0.tar.gz` & `tmp/EdgeGPT-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.8.0.tar", last modified: Sat Jun  3 13:20:13 2023, max compression
+gzip compressed data, was "EdgeGPT-0.8.1.tar", last modified: Sun Jun  4 13:13:14 2023, max compression
```

## Comparing `EdgeGPT-0.8.0.tar` & `EdgeGPT-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:20:13.531043 EdgeGPT-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-03 13:19:42.000000 EdgeGPT-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-06-03 13:20:13.531043 EdgeGPT-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 13:20:13.531043 EdgeGPT-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-03 13:19:42.000000 EdgeGPT-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:20:13.531043 EdgeGPT-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:20:13.531043 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34543 2023-06-03 13:19:42.000000 EdgeGPT-0.8.0/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-03 13:19:42.000000 EdgeGPT-0.8.0/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:13:14.024337 EdgeGPT-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-04 13:12:41.000000 EdgeGPT-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-06-04 13:13:14.024337 EdgeGPT-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-04 13:13:13.000000 EdgeGPT-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-04 13:13:14.024337 EdgeGPT-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-04 13:12:41.000000 EdgeGPT-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:13:14.020337 EdgeGPT-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:13:14.024337 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 13:13:14.000000 EdgeGPT-0.8.1/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34686 2023-06-04 13:12:41.000000 EdgeGPT-0.8.1/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-04 13:12:41.000000 EdgeGPT-0.8.1/src/ImageGen.py
```

### Comparing `EdgeGPT-0.8.0/LICENSE` & `EdgeGPT-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.8.0/PKG-INFO` & `EdgeGPT-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.8.0
+Version: 0.8.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.0 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.1 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.8.0/README.md` & `EdgeGPT-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.8.0/setup.py` & `EdgeGPT-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.8.0",
+    version="0.8.1",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.8.0/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.8.1/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.8.0
+Version: 0.8.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.0 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.1 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.8.0/src/EdgeGPT.py` & `EdgeGPT-0.8.1/src/EdgeGPT.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import asyncio
 import json
 import os
 import random
 import re
 import ssl
 import sys
-import time
+import locale as loc_util
 import uuid
 from enum import Enum
 from pathlib import Path
 from typing import Generator
 from typing import Union
 
 import aiofiles
@@ -191,14 +191,21 @@
     if locale == "en-ie":
         hint = LocationHint.EU.value
     else:
         hint = LocationHint.USA.value
     return hint.get("LocationHint")
 
 
+def guess_locale() -> str:
+    locale, _ = loc_util.getlocale()
+    if not locale:
+        locale = "en-US"
+    return locale.replace("_", "-")
+
+
 class ConversationStyle(Enum):
     creative = [
         "nlu_direct_response_filter",
         "deepleo",
         "disable_emoji_spoken_text",
         "responsible_ai_policy_235",
         "enablemm",
@@ -282,15 +289,15 @@
     def update(
         self,
         prompt: str,
         conversation_style: CONVERSATION_STYLE_TYPE,
         options: list | None = None,
         webpage_context: str | None = None,
         search_result: bool = False,
-        locale: str = "en-US",
+        locale: str = guess_locale(),
     ) -> None:
         if options is None:
             options = [
                 "deepleo",
                 "enable_debug_commands",
                 "disable_emoji_spoken_text",
                 "enablemm",
@@ -524,15 +531,15 @@
         prompt: str,
         wss_link: str,
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
         webpage_context: str | None = None,
         search_result: bool = False,
-        locale: str = "en-US",
+        locale: str = guess_locale(),
     ) -> Generator[str, None, None]:
         timeout = aiohttp.ClientTimeout(total=900)
         self.session = aiohttp.ClientSession(timeout=timeout)
 
         if self.wss and not self.wss.closed:
             await self.wss.close()
         # Check if websocket is closed
@@ -716,33 +723,33 @@
         )
         return self
 
     async def save_conversation(self, filename: str) -> None:
         """
         Save the conversation to a file
         """
-        async with aiofiles.Path.open(filename, "w") as f:
+        with open(filename, "w") as f:
             f.write(json.dumps(self.chat_hub.struct))
 
     async def load_conversation(self, filename: str) -> None:
         """
         Load the conversation from a file
         """
-        async with aiofiles.Path.open(filename, "r") as f:
-            self.chat_hub.struct = json.loads(await f.read())
+        with open(filename, "r") as f:
+            self.chat_hub.struct = json.loads(f.read())
 
     async def ask(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         options: dict = None,
         webpage_context: str | None = None,
         search_result: bool = False,
-        locale: str = "en-US",
+        locale: str = guess_locale(),
     ) -> dict:
         """
         Ask a question to the bot
         """
         async for final, response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
@@ -762,15 +769,15 @@
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
         webpage_context: str | None = None,
         search_result: bool = False,
-        locale: str = "en-US",
+        locale: str = guess_locale(),
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
@@ -1021,9 +1028,10 @@
         default="en-US",
         required=False,
         help="your locale",
     )
     args = parser.parse_args()
     asyncio.run(async_main(args))
 
+
 if __name__ == "__main__":
     main()
```

