# Comparing `tmp/lanarky-0.7.6.tar.gz` & `tmp/lanarky-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.7.6.tar", max compression
+gzip compressed data, was "lanarky-0.7.7.tar", max compression
```

## Comparing `lanarky-0.7.6.tar` & `lanarky-0.7.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2023-06-01 22:26:50.860827 lanarky-0.7.6/LICENSE
--rw-r--r--   0        0        0     4575 2023-06-01 22:26:50.860827 lanarky-0.7.6/README.md
--rw-r--r--   0        0        0       68 2023-06-01 22:26:51.036829 lanarky-0.7.6/lanarky/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0     3023 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/callbacks/agents.py
--rw-r--r--   0        0        0     2200 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1685 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     3461 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0      422 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/register/__init__.py
--rw-r--r--   0        0        0     1171 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/register/base.py
--rw-r--r--   0        0        0     1074 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/register/callbacks.py
--rw-r--r--   0        0        0       74 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     4956 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/responses/streaming.py
--rw-r--r--   0        0        0      150 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/routing/__init__.py
--rw-r--r--   0        0        0     5266 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/routing/langchain.py
--rw-r--r--   0        0        0     4185 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/routing/utils.py
--rw-r--r--   0        0        0      715 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3844 2023-06-01 22:26:51.040829 lanarky-0.7.6/lanarky/websockets/base.py
--rw-r--r--   0        0        0     1399 2023-06-01 22:26:51.040829 lanarky-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     5709 1970-01-01 00:00:00.000000 lanarky-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-04 07:36:57.046769 lanarky-0.7.7/LICENSE
+-rw-r--r--   0        0        0     4575 2023-06-04 07:36:57.046769 lanarky-0.7.7/README.md
+-rw-r--r--   0        0        0       68 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     3023 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     2200 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1685 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     3461 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0      422 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/register/__init__.py
+-rw-r--r--   0        0        0     1171 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/register/base.py
+-rw-r--r--   0        0        0     1074 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/register/callbacks.py
+-rw-r--r--   0        0        0       74 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     4956 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0      150 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/routing/__init__.py
+-rw-r--r--   0        0        0     5266 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/routing/langchain.py
+-rw-r--r--   0        0        0     4185 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/routing/utils.py
+-rw-r--r--   0        0        0      715 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/schemas.py
+-rw-r--r--   0        0        0       69 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     3845 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/websockets/base.py
+-rw-r--r--   0        0        0     1399 2023-06-04 07:36:57.246771 lanarky-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     5709 1970-01-01 00:00:00.000000 lanarky-0.7.7/PKG-INFO
```

### Comparing `lanarky-0.7.6/LICENSE` & `lanarky-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/README.md` & `lanarky-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/callbacks/__init__.py` & `lanarky-0.7.7/lanarky/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/callbacks/agents.py` & `lanarky-0.7.7/lanarky/callbacks/agents.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/callbacks/base.py` & `lanarky-0.7.7/lanarky/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/callbacks/llm.py` & `lanarky-0.7.7/lanarky/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.7.7/lanarky/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/register/base.py` & `lanarky-0.7.7/lanarky/register/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/register/callbacks.py` & `lanarky-0.7.7/lanarky/register/callbacks.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/responses/streaming.py` & `lanarky-0.7.7/lanarky/responses/streaming.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/routing/langchain.py` & `lanarky-0.7.7/lanarky/routing/langchain.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/routing/utils.py` & `lanarky-0.7.7/lanarky/routing/utils.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/schemas.py` & `lanarky-0.7.7/lanarky/schemas.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/testing/gradio.py` & `lanarky-0.7.7/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.6/lanarky/websockets/base.py` & `lanarky-0.7.7/lanarky/websockets/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                     WebsocketResponse(
                         sender=Sender.BOT,
                         message=Message.NULL,
                         message_type=MessageType.END,
                     ).dict()
                 )
             except WebSocketDisconnect:
-                logger.info("client disconnected.")
+                logger.debug("client disconnected.")
                 break
             except Exception as e:
                 logger.error(e)
                 await self.websocket.send_json(
                     WebsocketResponse(
                         sender=Sender.BOT,
                         message=Message.ERROR,
```

### Comparing `lanarky-0.7.6/pyproject.toml` & `lanarky-0.7.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.7.6"
+version = "0.7.7"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
```

### Comparing `lanarky-0.7.6/PKG-INFO` & `lanarky-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.7.6
+Version: 0.7.7
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

