# Comparing `tmp/line_async_webhook-0.1.0.tar.gz` & `tmp/line_async_webhook-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line_async_webhook-0.1.0.tar", max compression
+gzip compressed data, was "line_async_webhook-0.2.0.tar", max compression
```

## Comparing `line_async_webhook-0.1.0.tar` & `line_async_webhook-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-06-04 14:30:20.889200 line_async_webhook-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-04 14:30:50.170739 line_async_webhook-0.1.0/README.md
--rw-r--r--   0        0        0     2215 2023-06-04 14:56:06.568045 line_async_webhook-0.1.0/line_async_webhook/__init__.py
--rw-r--r--   0        0        0      376 2023-06-04 14:36:57.434492 line_async_webhook-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 line_async_webhook-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-04 14:30:20.889200 line_async_webhook-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-04 14:30:50.170739 line_async_webhook-0.2.0/README.md
+-rw-r--r--   0        0        0     2189 2023-06-04 14:57:04.780473 line_async_webhook-0.2.0/line_async_webhook/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 14:59:34.886600 line_async_webhook-0.2.0/line_async_webhook/py.typed
+-rw-r--r--   0        0        0      421 2023-06-04 15:02:05.112825 line_async_webhook-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 line_async_webhook-0.2.0/PKG-INFO
```

### Comparing `line_async_webhook-0.1.0/LICENSE` & `line_async_webhook-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `line_async_webhook-0.1.0/line_async_webhook/__init__.py` & `line_async_webhook-0.2.0/line_async_webhook/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import asyncer
 from linebot import WebhookHandler
 from linebot.models.events import MessageEvent
-from linebot.utils import LOGGER, PY3, safe_compare_digest
+from linebot.utils import LOGGER
 
 
 class AsyncWebhookHandler(WebhookHandler):
     """Webhook Handler for asynchronous compatible
 
     Please read https://github.com/line/line-bot-sdk-python#webhookhandler
     """
```

