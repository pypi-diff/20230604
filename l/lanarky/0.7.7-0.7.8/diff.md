# Comparing `tmp/lanarky-0.7.7.tar.gz` & `tmp/lanarky-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.7.7.tar", max compression
+gzip compressed data, was "lanarky-0.7.8.tar", max compression
```

## Comparing `lanarky-0.7.7.tar` & `lanarky-0.7.8.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1073 2023-06-04 07:36:57.046769 lanarky-0.7.7/LICENSE
--rw-r--r--   0        0        0     4575 2023-06-04 07:36:57.046769 lanarky-0.7.7/README.md
--rw-r--r--   0        0        0       68 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0     3023 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/callbacks/agents.py
--rw-r--r--   0        0        0     2200 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1685 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     3461 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0      422 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/register/__init__.py
--rw-r--r--   0        0        0     1171 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/register/base.py
--rw-r--r--   0        0        0     1074 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/register/callbacks.py
--rw-r--r--   0        0        0       74 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     4956 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/responses/streaming.py
--rw-r--r--   0        0        0      150 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/routing/__init__.py
--rw-r--r--   0        0        0     5266 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/routing/langchain.py
--rw-r--r--   0        0        0     4185 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/routing/utils.py
--rw-r--r--   0        0        0      715 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3845 2023-06-04 07:36:57.246771 lanarky-0.7.7/lanarky/websockets/base.py
--rw-r--r--   0        0        0     1399 2023-06-04 07:36:57.246771 lanarky-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     5709 1970-01-01 00:00:00.000000 lanarky-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-04 20:29:47.738920 lanarky-0.7.8/LICENSE
+-rw-r--r--   0        0        0     4746 2023-06-04 20:29:47.738920 lanarky-0.7.8/README.md
+-rw-r--r--   0        0        0      130 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/__init__.py
+-rw-r--r--   0        0        0     2874 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     3082 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     2204 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1685 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     3515 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0      422 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/register/__init__.py
+-rw-r--r--   0        0        0     1171 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/register/base.py
+-rw-r--r--   0        0        0     1074 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/register/callbacks.py
+-rw-r--r--   0        0        0       74 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     5980 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0      150 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/routing/__init__.py
+-rw-r--r--   0        0        0     5591 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/routing/langchain.py
+-rw-r--r--   0        0        0     7467 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/routing/utils.py
+-rw-r--r--   0        0        0      316 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/schemas/__init__.py
+-rw-r--r--   0        0        0      335 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/schemas/callbacks.py
+-rw-r--r--   0        0        0      707 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/schemas/websockets.py
+-rw-r--r--   0        0        0       69 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     4793 2023-06-04 20:29:47.918933 lanarky-0.7.8/lanarky/websockets/base.py
+-rw-r--r--   0        0        0     1419 2023-06-04 20:29:47.918933 lanarky-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     5884 1970-01-01 00:00:00.000000 lanarky-0.7.8/PKG-INFO
```

### Comparing `lanarky-0.7.7/LICENSE` & `lanarky-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.7/README.md` & `lanarky-0.7.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 </div>
 
 Lanarky is an open-source framework to deploy LLM applications in production. It is built on top of [FastAPI](https://github.com/tiangolo/fastapi)
 and comes with batteries included.
 
 ## 🚀 Features
 
-- supports [LangChain](https://github.com/hwchase17/langchain)
-- simple gradio chatbot UI for fast prototyping
+- 🌐 multi-mode token streaming
+- 💬 simple gradio chatbot UI for fast prototyping
+- 🔗 supports [LangChain](https://github.com/hwchase17/langchain) applications
+- 🗄️ multiple LLM caching strategies
 
 See [Roadmap](#-roadmap) for upcoming features.
 
 ## ❓ Why?
 
 There are great low-code/no-code solutions in the open source to deploy your LLM projects. However,
 most of them are opinionated in terms of cloud or deployment code. This project aims to provide users
@@ -76,14 +78,15 @@
 
 ## 📍 Roadmap
 
 - [x] Add support for [LangChain](https://github.com/hwchase17/langchain)
 - [x] Add [Gradio](https://github.com/gradio-app/gradio) UI for fast prototyping
 - [x] Add support for in-memory, Redis and [GPTCache](https://github.com/zilliztech/GPTCache) LLM caching
 - [ ] Add support for [LlamaIndex](https://github.com/jerryjliu/llama_index)
+- [ ] Add support for [Guidance](https://github.com/microsoft/guidance)
 - [ ] Add SQL database integration
 - [ ] Add support for [Rebuff](https://github.com/woop/rebuff)
 
 ## 🤩 Stargazers
 
 Leave a ⭐ if you find this project useful.
```

### Comparing `lanarky-0.7.7/lanarky/callbacks/__init__.py` & `lanarky-0.7.8/lanarky/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.7/lanarky/callbacks/agents.py` & `lanarky-0.7.8/lanarky/callbacks/agents.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         self, serialized: dict[str, Any], prompts: list[str], **kwargs: Any
     ) -> None:
         """Run when LLM starts running."""
         self.last_tokens = [""] * len(self.answer_prefix_tokens)
         self.answer_reached = False
 
     def _check_if_answer_reached(self, token: str):
+        """Checks if the final answer has been reached."""
         self.last_tokens.append(token)
         if len(self.last_tokens) > len(self.answer_prefix_tokens):
             self.last_tokens.pop(0)
 
         if self.last_tokens == self.answer_prefix_tokens:
             self.answer_reached = True
             return
```

### Comparing `lanarky-0.7.7/lanarky/callbacks/base.py` & `lanarky-0.7.8/lanarky/callbacks/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,50 +19,50 @@
         return True
 
     class Config:
         arbitrary_types_allowed = True
 
     @abstractmethod
     def _construct_message(self, content: Any) -> Any:  # pragma: no cover
-        """Construct a Message from a string."""
+        """Constructs a Message from a string."""
         pass
 
 
 class AsyncStreamingResponseCallback(AsyncLanarkyCallback):
     """Async Callback handler for StreamingResponse."""
 
     send: Send = Field(...)
 
     def _construct_message(self, content: str) -> Message:
-        """Construct a Message from a string."""
+        """Constructs a Message from a string."""
         return {
             "type": "http.response.body",
             "body": content.encode("utf-8"),
             "more_body": True,
         }
 
 
 class AsyncWebsocketCallback(AsyncLanarkyCallback):
     """Async Callback handler for WebsocketConnection."""
 
     websocket: WebSocket = Field(...)
     response: WebsocketResponse = Field(...)
 
     def _construct_message(self, content: str) -> dict:
-        """Construct a WebsocketResponse from a string."""
+        """Constructs a WebsocketResponse from a string."""
         return {**self.response.dict(), **{"message": content}}
 
 
 class AsyncStreamingJSONResponseCallback(AsyncStreamingResponseCallback):
     """Async Callback handler for StreamingJSONResponse."""
 
     send: Send = Field(...)
 
     def _construct_message(self, content: StreamingJSONResponse) -> Message:
-        """Construct a Message from a dictionary."""
+        """Constructs a Message from a dictionary."""
         return {
             "type": "http.response.body",
             "body": json.dumps(
                 content.dict(),
                 ensure_ascii=False,
                 allow_nan=False,
                 indent=None,
```

### Comparing `lanarky-0.7.7/lanarky/callbacks/llm.py` & `lanarky-0.7.8/lanarky/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.7/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.7.8/lanarky/callbacks/retrieval_qa.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,28 +22,29 @@
     "RetrievalQAWithSourcesChain",
     "ConversationalRetrievalChain",
 ]
 SOURCE_DOCUMENT_TEMPLATE = """
 page content: {page_content}
 {document_metadata}
 """
+SOURCE_DOCUMENTS_KEY = "source_documents"
 
 
 @register_streaming_callback(SUPPORTED_CHAINS)
 class AsyncBaseRetrievalQAStreamingCallback(AsyncLLMChainStreamingCallback):
     """AsyncStreamingResponseCallback handler for BaseRetrievalQA."""
 
     source_document_template: str = SOURCE_DOCUMENT_TEMPLATE
 
     async def on_chain_end(self, outputs: dict[str, Any], **kwargs: Any) -> None:
         """Run when chain ends running."""
-        if "source_documents" in outputs:
+        if SOURCE_DOCUMENTS_KEY in outputs:
             message = self._construct_message("\n\nSOURCE DOCUMENTS:\n")
             await self.send(message)
-            for document in outputs["source_documents"]:
+            for document in outputs[SOURCE_DOCUMENTS_KEY]:
                 document_metadata = "\n".join(
                     [f"{k}: {v}" for k, v in document.metadata.items()]
                 )
                 message = self._construct_message(
                     self.source_document_template.format(
                         page_content=document.page_content,
                         document_metadata=document_metadata,
@@ -56,18 +57,18 @@
 class AsyncBaseRetrievalQAWebsocketCallback(AsyncLLMChainWebsocketCallback):
     """AsyncWebsocketCallback handler for BaseRetrievalQA."""
 
     source_document_template: str = SOURCE_DOCUMENT_TEMPLATE
 
     async def on_chain_end(self, outputs: dict[str, Any], **kwargs: Any) -> None:
         """Run when chain ends running."""
-        if "source_documents" in outputs:
+        if SOURCE_DOCUMENTS_KEY in outputs:
             message = self._construct_message("\n\nSOURCE DOCUMENTS:\n")
             await self.websocket.send_json(message)
-            for document in outputs["source_documents"]:
+            for document in outputs[SOURCE_DOCUMENTS_KEY]:
                 document_metadata = "\n".join(
                     [f"{k}: {v}" for k, v in document.metadata.items()]
                 )
                 message = self._construct_message(
                     self.source_document_template.format(
                         page_content=document.page_content,
                         document_metadata=document_metadata,
@@ -78,15 +79,15 @@
 
 @register_streaming_json_callback(SUPPORTED_CHAINS)
 class AsyncBaseRetrievalQAStreamingJSONCallback(AsyncLLMChainStreamingJSONCallback):
     """AsyncStreamingJSONResponseCallback handler for BaseRetrievalQA."""
 
     async def on_chain_end(self, outputs: dict[str, Any], **kwargs: Any) -> None:
         """Run when chain ends running."""
-        if "source_documents" in outputs:
+        if SOURCE_DOCUMENTS_KEY in outputs:
             source_documents = [
-                document.dict() for document in outputs["source_documents"]
+                document.dict() for document in outputs[SOURCE_DOCUMENTS_KEY]
             ]
             message = self._construct_message(
                 BaseRetrievalQAStreamingJSONResponse(source_documents=source_documents)
             )
             await self.send(message)
```

### Comparing `lanarky-0.7.7/lanarky/register/base.py` & `lanarky-0.7.8/lanarky/register/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.7/lanarky/register/callbacks.py` & `lanarky-0.7.8/lanarky/register/callbacks.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.7/lanarky/responses/streaming.py` & `lanarky-0.7.8/lanarky/responses/streaming.py`

 * *Files 24% similar despite different names*

```diff
@@ -50,26 +50,34 @@
 
     def __init__(
         self,
         chain_executor: Callable[[Send], Awaitable[Any]],
         background: Optional[BackgroundTask] = None,
         **kwargs: Any,
     ) -> None:
+        """Constructor method.
+
+        Args:
+            chain_executor: function to execute ``chain.acall()``.
+            background: A ``BackgroundTask`` object to run in the background.
+        """
         super().__init__(content=iter(()), background=background, **kwargs)
 
         self.chain_executor = chain_executor
 
     async def listen_for_disconnect(self, receive: Receive) -> None:
+        """Listen for client disconnect."""
         while True:
             message = await receive()
             if message["type"] == "http.disconnect":
                 logger.debug("Client disconnected")
                 break
 
     async def stream_response(self, send: Send) -> None:
+        """Streams the response."""
         await send(
             {
                 "type": "http.response.start",
                 "status": self.status_code,
                 "headers": self.raw_headers,
             }
         )
@@ -119,14 +127,22 @@
     @staticmethod
     def _create_chain_executor(
         chain: Chain,
         inputs: Union[dict[str, Any], Any],
         as_json: bool = False,
         **callback_kwargs,
     ) -> Callable[[Send], Awaitable[Any]]:
+        """Creates a function to execute ``chain.acall()``.
+
+        Args:
+            chain: A ``Chain`` object.
+            inputs: Inputs to pass to ``chain.acall()``.
+            as_json: Whether to return the outputs as JSON.
+            callback_kwargs: Keyword arguments to pass to the callback function.
+        """
         get_callback_fn = (
             get_streaming_json_callback if as_json else get_streaming_callback
         )
 
         async def wrapper(send: Send):
             return await chain.acall(
                 inputs=inputs,
@@ -141,14 +157,23 @@
         chain: Chain,
         inputs: Union[dict[str, Any], Any],
         as_json: bool = False,
         background: Optional[BackgroundTask] = None,
         callback_kwargs: dict[str, Any] = {},
         **kwargs: Any,
     ) -> "StreamingResponse":
+        """Creates a ``StreamingResponse`` object from a ``Chain`` object.
+
+        Args:
+            chain: A ``Chain`` object.
+            inputs: Inputs to pass to ``chain.acall()``.
+            as_json: Whether to return the outputs as JSON.
+            background: A ``BackgroundTask`` object to run in the background.
+            callback_kwargs: Keyword arguments to pass to the callback function.
+        """
         chain_executor = cls._create_chain_executor(
             chain, inputs, as_json, **callback_kwargs
         )
 
         return cls(
             chain_executor=chain_executor,
             background=background,
```

### Comparing `lanarky-0.7.7/lanarky/routing/langchain.py` & `lanarky-0.7.8/lanarky/routing/langchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import random
-import string
 from typing import Any, Optional, Type
 
 from fastapi.routing import APIRouter
 from fastapi.websockets import WebSocket
 from langchain.chains.base import Chain
 
 from .utils import (
@@ -108,20 +106,24 @@
         self,
         url: str,
         langchain_object: Chain,
         streaming_mode: StreamingMode,
         methods: list[str] = ["POST"],
         **kwargs,
     ):
-        """Adds a Langchain API route to the router."""
-        langchain_dependency = create_langchain_dependency(langchain_object)
+        """Adds a Langchain API route to the router.
 
-        name_prefix = "".join(
-            random.choice(string.ascii_letters) for _ in range(5)
-        ).title()
+        Args:
+            url: The URL of the route.
+            langchain_object: The Langchain object to use for the route.
+            streaming_mode: The streaming mode to use for the route.
+            methods: The HTTP methods to use for the route.
+        """
+        name_prefix = url.replace("/", "").title().replace("_", "")
+        langchain_dependency = create_langchain_dependency(langchain_object)
         endpoint_request = create_request_from_langchain_dependency(
             langchain_dependency, name_prefix
         )
         response_model = (
             create_response_model_from_langchain_dependency(
                 langchain_dependency, name_prefix
             )
@@ -143,15 +145,20 @@
             methods=methods,
             **kwargs,
         )
 
         self.langchain_dependencies.append(langchain_dependency)
 
     def add_langchain_api_websocket_route(self, url: str, langchain_object: Chain):
-        """Adds a Langchain API websocket route to the router."""
+        """Adds a Langchain API websocket route to the router.
+
+        Args:
+            url: The URL of the route.
+            langchain_object: The Langchain object to use for the route.
+        """
         langchain_dependency = create_langchain_dependency(langchain_object)
         endpoint = create_langchain_websocket_endpoint(
             WebSocket,
             langchain_dependency,
         )
 
         self.add_api_websocket_route(url, endpoint)
```

### Comparing `lanarky-0.7.7/lanarky/testing/gradio.py` & `lanarky-0.7.8/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.7/lanarky/websockets/base.py` & `lanarky-0.7.8/lanarky/websockets/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,21 +14,24 @@
 from lanarky.callbacks import get_websocket_callback
 from lanarky.schemas import Message, MessageType, Sender, WebsocketResponse
 
 logger = logging.getLogger(__name__)
 
 
 class BaseWebsocketConnection(BaseModel):
+    """Base class for websocket connections."""
+
     websocket: WebSocket = Field(...)
     chain_executor: Callable[[str], Awaitable[Any]] = Field(...)
 
     class Config:
         arbitrary_types_allowed = True
 
     async def connect(self):
+        """Connect to websocket."""
         await self.websocket.accept()
         while True:
             try:
                 user_message = await self.websocket.receive_text()
                 await self.websocket.send_json(
                     WebsocketResponse(
                         sender=Sender.HUMAN,
@@ -67,23 +70,38 @@
     @staticmethod
     def _create_chain_executor(
         chain: Chain,
         websocket: WebSocket,
         response: WebsocketResponse,
         **callback_kwargs,
     ) -> Callable[[str], Awaitable[Any]]:
+        """Creates a function to execute ``chain.acall()``.
+
+        Args:
+            chain: langchain chain instance.
+            websocket: websocket instance.
+            response: WebsocketResponse instance.
+            callback_kwargs: keyword arguments for callback function.
+        """
         raise NotImplementedError
 
     @classmethod
     def from_chain(
         cls,
         chain: Chain,
         websocket: WebSocket,
         callback_kwargs: dict[str, Any] = {},
     ) -> "BaseWebsocketConnection":
+        """Creates a BaseWebsocketConnection instance from a langchain chain instance.
+
+        Args:
+            chain: langchain chain instance.
+            websocket: websocket instance.
+            callback_kwargs: keyword arguments for callback function.
+        """
         chain_executor = cls._create_chain_executor(
             chain,
             websocket,
             WebsocketResponse(
                 sender=Sender.BOT, message=Message.NULL, message_type=MessageType.STREAM
             ),
             **callback_kwargs,
@@ -101,14 +119,23 @@
     @staticmethod
     def _create_chain_executor(
         chain: Chain,
         websocket: WebSocket,
         response: WebsocketResponse,
         **callback_kwargs,
     ) -> Callable[[str], Awaitable[Any]]:
+        """Creates a function to execute ``chain.acall()``.
+
+        Args:
+            chain: langchain chain instance.
+            websocket: websocket instance.
+            response: WebsocketResponse instance.
+            callback_kwargs: keyword arguments for callback function.
+        """
+
         async def wrapper(user_message: str):
             return await chain.acall(
                 inputs=user_message,
                 callbacks=[
                     get_websocket_callback(
                         chain=chain,
                         websocket=websocket,
```

### Comparing `lanarky-0.7.7/pyproject.toml` & `lanarky-0.7.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.7.7"
+version = "0.7.8"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-fastapi = ">=0.95.2"
-langchain = ">=0.0.183"
+fastapi = ">=0.96.0"
+langchain = ">=0.0.189"
 urllib3 = "<=1.26.15"  # added due to poetry errors
 python-dotenv = "^1.0.0"
 typing-extensions = "4.5.0"  # added due to https://github.com/hwchase17/langchain/issues/5113
 redis = {version = "^4.5.5", optional = true}
-gptcache = {version = "^0.1.28", optional = true}
+gptcache = {version = "^0.1.29.1", optional = true}
 openai = {version = "^0.27.7", optional = true}
 tiktoken = {version = "^0.4.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.3.1"
+pre-commit = "^3.3.2"
 
 
 [tool.poetry.group.docs.dependencies]
-furo = "^2023.3.27"
+furo = "^2023.5.20"
 sphinx-autobuild = "^2021.3.14"
 myst-parser = "^1.0.0"
 sphinx-copybutton = "^0.5.2"
 autodoc-pydantic = "^1.8.0"
 toml = "^0.10.2"
 
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.21.0"
 coveralls = "^3.3.1"
+httpx = "^0.24.1"
 
 [tool.poetry.extras]
 openai = ["openai", "tiktoken"]
 redis = ["redis"]
 gptcache = ["gptcache"]
 
 [build-system]
```

### Comparing `lanarky-0.7.7/PKG-INFO` & `lanarky-0.7.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.7.7
+Version: 0.7.8
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gptcache
 Provides-Extra: openai
 Provides-Extra: redis
-Requires-Dist: fastapi (>=0.95.2)
-Requires-Dist: gptcache (>=0.1.28,<0.2.0) ; extra == "gptcache"
-Requires-Dist: langchain (>=0.0.183)
+Requires-Dist: fastapi (>=0.96.0)
+Requires-Dist: gptcache (>=0.1.29.1,<0.2.0.0) ; extra == "gptcache"
+Requires-Dist: langchain (>=0.0.189)
 Requires-Dist: openai (>=0.27.7,<0.28.0) ; extra == "openai"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: redis (>=4.5.5,<5.0.0) ; extra == "redis"
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0) ; extra == "openai"
 Requires-Dist: typing-extensions (==4.5.0)
 Requires-Dist: urllib3 (<=1.26.15)
 Project-URL: Repository, https://github.com/ajndkr/lanarky
@@ -46,16 +46,18 @@
 </div>
 
 Lanarky is an open-source framework to deploy LLM applications in production. It is built on top of [FastAPI](https://github.com/tiangolo/fastapi)
 and comes with batteries included.
 
 ## 🚀 Features
 
-- supports [LangChain](https://github.com/hwchase17/langchain)
-- simple gradio chatbot UI for fast prototyping
+- 🌐 multi-mode token streaming
+- 💬 simple gradio chatbot UI for fast prototyping
+- 🔗 supports [LangChain](https://github.com/hwchase17/langchain) applications
+- 🗄️ multiple LLM caching strategies
 
 See [Roadmap](#-roadmap) for upcoming features.
 
 ## ❓ Why?
 
 There are great low-code/no-code solutions in the open source to deploy your LLM projects. However,
 most of them are opinionated in terms of cloud or deployment code. This project aims to provide users
@@ -105,14 +107,15 @@
 
 ## 📍 Roadmap
 
 - [x] Add support for [LangChain](https://github.com/hwchase17/langchain)
 - [x] Add [Gradio](https://github.com/gradio-app/gradio) UI for fast prototyping
 - [x] Add support for in-memory, Redis and [GPTCache](https://github.com/zilliztech/GPTCache) LLM caching
 - [ ] Add support for [LlamaIndex](https://github.com/jerryjliu/llama_index)
+- [ ] Add support for [Guidance](https://github.com/microsoft/guidance)
 - [ ] Add SQL database integration
 - [ ] Add support for [Rebuff](https://github.com/woop/rebuff)
 
 ## 🤩 Stargazers
 
 Leave a ⭐ if you find this project useful.
```

