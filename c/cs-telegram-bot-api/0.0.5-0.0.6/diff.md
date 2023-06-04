# Comparing `tmp/cs-telegram-bot-api-0.0.5.tar.gz` & `tmp/cs-telegram-bot-api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-telegram-bot-api-0.0.5.tar", last modified: Mon May 29 19:13:12 2023, max compression
+gzip compressed data, was "cs-telegram-bot-api-0.0.6.tar", last modified: Sun Jun  4 20:34:06 2023, max compression
```

## Comparing `cs-telegram-bot-api-0.0.5.tar` & `cs-telegram-bot-api-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:13:12.281933 cs-telegram-bot-api-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 19:13:12.281933 cs-telegram-bot-api-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-29 19:13:00.000000 cs-telegram-bot-api-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:13:12.281933 cs-telegram-bot-api-0.0.5/cs_telegram_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-29 19:13:00.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-29 19:13:00.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:13:12.281933 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 19:13:12.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-29 19:13:12.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:13:12.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 19:13:12.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 19:13:12.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:13:12.281933 cs-telegram-bot-api-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-29 19:13:00.000000 cs-telegram-bot-api-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:06.949681 cs-telegram-bot-api-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-04 20:34:06.949681 cs-telegram-bot-api-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-04 20:33:57.000000 cs-telegram-bot-api-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:06.945680 cs-telegram-bot-api-0.0.6/cs_telegram_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-04 20:33:57.000000 cs-telegram-bot-api-0.0.6/cs_telegram_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-04 20:33:57.000000 cs-telegram-bot-api-0.0.6/cs_telegram_bot/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:06.949681 cs-telegram-bot-api-0.0.6/cs_telegram_bot_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-04 20:34:06.000000 cs-telegram-bot-api-0.0.6/cs_telegram_bot_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-04 20:34:06.000000 cs-telegram-bot-api-0.0.6/cs_telegram_bot_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:34:06.000000 cs-telegram-bot-api-0.0.6/cs_telegram_bot_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 20:34:06.000000 cs-telegram-bot-api-0.0.6/cs_telegram_bot_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 20:34:06.000000 cs-telegram-bot-api-0.0.6/cs_telegram_bot_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:34:06.949681 cs-telegram-bot-api-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-04 20:33:57.000000 cs-telegram-bot-api-0.0.6/setup.py
```

### Comparing `cs-telegram-bot-api-0.0.5/README.md` & `cs-telegram-bot-api-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cs-telegram-bot-api-0.0.5/cs_telegram_bot/api.py` & `cs-telegram-bot-api-0.0.6/cs_telegram_bot/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 A Python module for interacting with the Telegram Bot API.
 """
 import requests
 import os
+import logging
+from secrets_loader import load_secret
 
 
 class TelegramClient:
     """
     A client for the Telegram Bot API.
     """
 
     def __init__(self, bot_token=None):
         """
         Create a new TelegramClient.
         """
-        self.bot_token = bot_token or os.getenv("TELEGRAM_TOKEN")
+        self.bot_token = bot_token or load_secret("TELEGRAM_TOKEN")
         self.offset = 0
 
     def get_new_messages(self):
         """
         Get new messages from the API.
         """
         try:
@@ -62,10 +64,10 @@
             response.raise_for_status()
         except requests.exceptions.RequestException as e:
             raise SystemExit(e)
 
         # If the API call was successful, the response will contain
         # the sent message in the "result" field
         result = response.json()["result"]
-        print(message)
+        logging.info(message)
         return result
```

### Comparing `cs-telegram-bot-api-0.0.5/setup.py` & `cs-telegram-bot-api-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Telegram Bot API Wrapper'
 LONG_DESCRIPTION = 'A Python module for interacting with the Telegram Bot API.'
 
 # Setting up
 setup(
     name="cs-telegram-bot-api",
     version=VERSION,
```

