# Comparing `tmp/chatstream-0.1.5.tar.gz` & `tmp/chatstream-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatstream-0.1.5.tar", last modified: Wed May 31 09:18:07 2023, max compression
+gzip compressed data, was "chatstream-0.2.0.tar", last modified: Sun Jun  4 04:36:33 2023, max compression
```

## Comparing `chatstream-0.1.5.tar` & `chatstream-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 09:18:07.086113 chatstream-0.1.5/
-drwxrwxrwx   0        0        0        0 2023-05-31 09:18:07.065408 chatstream-0.1.5/ChatStream.egg-info/
--rw-rw-rw-   0        0        0     8598 2023-05-31 09:18:07.000000 chatstream-0.1.5/ChatStream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-05-31 09:18:07.000000 chatstream-0.1.5/ChatStream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 09:18:07.000000 chatstream-0.1.5/ChatStream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-31 09:18:07.000000 chatstream-0.1.5/ChatStream.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 09:18:07.000000 chatstream-0.1.5/ChatStream.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11356 2023-05-21 23:57:09.000000 chatstream-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     8598 2023-05-31 09:18:07.085108 chatstream-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     7703 2023-05-31 09:10:35.000000 chatstream-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 09:18:07.080605 chatstream-0.1.5/chatstream/
--rw-rw-rw-   0        0        0      472 2023-05-31 07:50:57.000000 chatstream-0.1.5/chatstream/__init__.py
--rw-rw-rw-   0        0        0     8430 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/chat_core.py
--rw-rw-rw-   0        0        0     9316 2023-05-30 07:48:10.000000 chatstream-0.1.5/chatstream/chat_process.py
--rw-rw-rw-   0        0        0     4447 2023-05-27 07:38:12.000000 chatstream-0.1.5/chatstream/chat_process_mock.py
--rw-rw-rw-   0        0        0     8831 2023-05-30 07:38:04.000000 chatstream-0.1.5/chatstream/chat_prompt.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:18:07.082605 chatstream-0.1.5/chatstream/chat_prompt_presets/
--rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/chat_prompt_presets/__init__.py
--rw-rw-rw-   0        0        0     2296 2023-05-31 00:36:00.000000 chatstream-0.1.5/chatstream/chat_prompt_presets/chat_prompt_redpajama_incite.py
--rw-rw-rw-   0        0        0     1452 2023-05-31 00:10:08.000000 chatstream-0.1.5/chatstream/chat_prompt_presets/chat_prompt_rinna.py
--rw-rw-rw-   0        0        0    21392 2023-05-31 07:35:08.000000 chatstream-0.1.5/chatstream/chat_stream.py
--rw-rw-rw-   0        0        0     3146 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/mock_response_example_text.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:18:07.085108 chatstream-0.1.5/chatstream/request_handler/
--rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/request_handler/__init__.py
--rw-rw-rw-   0        0        0     4428 2023-05-31 07:34:47.000000 chatstream-0.1.5/chatstream/request_handler/request_handler.py
--rw-rw-rw-   0        0        0    10863 2023-05-31 07:35:08.000000 chatstream-0.1.5/chatstream/request_handler/simple_session_request_handler.py
--rw-rw-rw-   0        0        0     3356 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/sampling_utils.py
--rw-rw-rw-   0        0        0      803 2023-05-21 23:57:09.000000 chatstream-0.1.5/chatstream/util_request_id.py
--rw-rw-rw-   0        0        0       42 2023-05-31 09:18:07.086113 chatstream-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-05-31 09:10:49.000000 chatstream-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:36:33.219724 chatstream-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-06-04 04:36:33.146085 chatstream-0.2.0/ChatStream.egg-info/
+-rw-rw-rw-   0        0        0     5080 2023-06-04 04:36:33.000000 chatstream-0.2.0/ChatStream.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1028 2023-06-04 04:36:33.000000 chatstream-0.2.0/ChatStream.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 04:36:33.000000 chatstream-0.2.0/ChatStream.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-04 04:36:33.000000 chatstream-0.2.0/ChatStream.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-04 04:36:33.000000 chatstream-0.2.0/ChatStream.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11356 2023-05-21 23:57:09.000000 chatstream-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5080 2023-06-04 04:36:33.218724 chatstream-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4312 2023-06-04 04:29:00.000000 chatstream-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 04:36:33.184010 chatstream-0.2.0/chatstream/
+-rw-rw-rw-   0        0        0      510 2023-06-01 14:46:05.000000 chatstream-0.2.0/chatstream/__init__.py
+-rw-rw-rw-   0        0        0     8557 2023-06-02 16:05:38.000000 chatstream-0.2.0/chatstream/chat_core.py
+-rw-rw-rw-   0        0        0     9316 2023-05-30 07:48:10.000000 chatstream-0.2.0/chatstream/chat_process.py
+-rw-rw-rw-   0        0        0     4447 2023-05-27 07:38:12.000000 chatstream-0.2.0/chatstream/chat_process_mock.py
+-rw-rw-rw-   0        0        0     8831 2023-05-30 07:38:04.000000 chatstream-0.2.0/chatstream/chat_prompt.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:36:33.196013 chatstream-0.2.0/chatstream/chat_prompt_presets/
+-rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.2.0/chatstream/chat_prompt_presets/__init__.py
+-rw-rw-rw-   0        0        0     2296 2023-05-31 00:36:00.000000 chatstream-0.2.0/chatstream/chat_prompt_presets/chat_prompt_redpajama_incite.py
+-rw-rw-rw-   0        0        0     1452 2023-06-02 16:06:54.000000 chatstream-0.2.0/chatstream/chat_prompt_presets/chat_prompt_rinna.py
+-rw-rw-rw-   0        0        0    24061 2023-06-02 16:02:12.000000 chatstream-0.2.0/chatstream/chat_stream.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:36:33.197013 chatstream-0.2.0/chatstream/data/
+-rw-rw-rw-   0        0        0        0 2023-06-02 14:56:24.000000 chatstream-0.2.0/chatstream/data/__init__.py
+-rw-rw-rw-   0        0        0     3146 2023-05-21 23:57:09.000000 chatstream-0.2.0/chatstream/mock_response_example_text.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:36:33.209521 chatstream-0.2.0/chatstream/request_handler/
+-rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.2.0/chatstream/request_handler/__init__.py
+-rw-rw-rw-   0        0        0     4428 2023-05-31 07:34:47.000000 chatstream-0.2.0/chatstream/request_handler/request_handler.py
+-rw-rw-rw-   0        0        0    10863 2023-05-31 07:35:08.000000 chatstream-0.2.0/chatstream/request_handler/simple_session_request_handler.py
+-rw-rw-rw-   0        0        0     4228 2023-06-02 10:37:29.000000 chatstream-0.2.0/chatstream/sampling_utils.py
+-rw-rw-rw-   0        0        0      803 2023-05-21 23:57:09.000000 chatstream-0.2.0/chatstream/util_request_id.py
+-rw-rw-rw-   0        0        0       42 2023-06-04 04:36:33.219724 chatstream-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-06-02 16:02:12.000000 chatstream-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:36:33.218724 chatstream-0.2.0/tests/
+-rw-rw-rw-   0        0        0     3507 2023-05-31 00:34:34.000000 chatstream-0.2.0/tests/test_chat_prompt_of_redpajama.py
+-rw-rw-rw-   0        0        0    13117 2023-05-31 00:32:45.000000 chatstream-0.2.0/tests/test_chat_prompt_of_rinna.py
```

### Comparing `chatstream-0.1.5/ChatStream.egg-info/SOURCES.txt` & `chatstream-0.2.0/ChatStream.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,10 +19,13 @@
 chatstream.egg-info/SOURCES.txt
 chatstream.egg-info/dependency_links.txt
 chatstream.egg-info/requires.txt
 chatstream.egg-info/top_level.txt
 chatstream/chat_prompt_presets/__init__.py
 chatstream/chat_prompt_presets/chat_prompt_redpajama_incite.py
 chatstream/chat_prompt_presets/chat_prompt_rinna.py
+chatstream/data/__init__.py
 chatstream/request_handler/__init__.py
 chatstream/request_handler/request_handler.py
-chatstream/request_handler/simple_session_request_handler.py
+chatstream/request_handler/simple_session_request_handler.py
+tests/test_chat_prompt_of_redpajama.py
+tests/test_chat_prompt_of_rinna.py
```

### Comparing `chatstream-0.1.5/LICENSE` & `chatstream-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.5/chatstream/chat_core.py` & `chatstream-0.2.0/chatstream/chat_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
     top_k_value = params.get("top_k_value", 50)
 
     use_top_p_sampling = params.get("use_top_p_sampling", True)
     top_p_value = params.get("top_p_value", 1.0)
 
     use_repetition_penalty = params.get("use_repetition_penalty", False)
 
-    repetition_penalty = params.get("repetition_penalty", 1),
+    repetition_penalty = params.get("repetition_penalty", 1)
+
     repetition_penalty_method = params.get("repetition_penalty_method", "multiplicative")
     use_bos_for_input = params.get("use_bos_for_input", False)
 
     if force_set_bos_token_id:
         # patch for open_llama_7b_preview_300bt
         tokenizer.bos_token_id = force_set_bos_token_id
 
@@ -130,37 +131,42 @@
 
             if device == "mps":
                 last_token_logits = last_token_logits.float().to("cpu")
 
             if temperature < 1e-4:
                 token_id = int(torch.argmax(last_token_logits))
             else:
-                token_id = sampling(logits=last_token_logits,
-                                    k=top_k_value if use_top_k_sampling else None,
-                                    p=top_p_value if use_top_p_sampling else None,
-                                    temperature=temperature,
-                                    past_tokens=output_token_ids,
-                                    penalty=repetition_penalty if use_repetition_penalty else None,
-                                    penalty_method=repetition_penalty_method)
+                if not use_repetition_penalty:
+                    repetition_penalty = None
+
+                token_id = sampling(
+                    logits=last_token_logits,
+                    k=top_k_value if use_top_k_sampling else None,
+                    p=top_p_value if use_top_p_sampling else None,
+                    temperature=temperature,
+                    past_tokens=output_token_ids,
+                    penalty=repetition_penalty,
+                    penalty_method=repetition_penalty_method
+                )
 
             output_token_ids.append(token_id)
 
             if token_id in stop_token_ids:
                 stopped = True
             else:
                 stopped = False
 
             if idx % stream_interval == 0 or idx == max_new_tokens - 1 or stopped:
                 output = tokenizer.decode(output_token_ids, skip_special_tokens=True)
 
                 if stop_strs:
                     for stop_str in stop_strs:
                         if stop_str:
-
                             pos = output.rfind(stop_str, len_prompt)
+                            # print(f"output:'{output}' prompt:{prompt} len_prompt:{len_prompt} stop_str:{stop_str} pos:{pos}")
                             is_stop_str_found = (pos != -1)
                             if is_stop_str_found:
                                 output = output[:pos]
                                 stopped = True
 
                 yield output
```

### Comparing `chatstream-0.1.5/chatstream/chat_process.py` & `chatstream-0.2.0/chatstream/chat_process.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.5/chatstream/chat_process_mock.py` & `chatstream-0.2.0/chatstream/chat_process_mock.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.5/chatstream/chat_prompt.py` & `chatstream-0.2.0/chatstream/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.5/chatstream/chat_prompt_presets/chat_prompt_redpajama_incite.py` & `chatstream-0.2.0/chatstream/chat_prompt_presets/chat_prompt_redpajama_incite.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.5/chatstream/chat_prompt_presets/chat_prompt_rinna.py` & `chatstream-0.2.0/chatstream/chat_prompt_presets/chat_prompt_rinna.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.5/chatstream/chat_stream.py` & `chatstream-0.2.0/chatstream/chat_stream.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import asyncio
 import logging
 import os
 import signal
 import traceback
+import json
+import sys
 from typing import Generator
 
-from fastapi import Request
+from fastapi import Request, Response
 from starlette.requests import ClientDisconnect
 from starlette.responses import JSONResponse
 
 from .chat_process import ChatGenerator
 from .chat_process_mock import ChatGeneratorMock
 from .request_handler.simple_session_request_handler import SimpleSessionRequestHandler
 from .util_request_id import set_req_id, req_id
+import importlib.resources as pkg_resources
 
 
 class ChatStream:
     def __init__(self,
                  model=None,  # Pre-trained language model in HuggingFace style
                  tokenizer=None,  # HuggingFace style tokenizer
                  device=None,  # Run on "cpu" / "cuda" / "mps"
@@ -65,15 +68,15 @@
             "max_new_tokens": max_new_tokens,  # 新たに生成する最大トークンサイズ（何トークン分か。)
             "context_len": context_len,  ## コンテクストのサイズ（何トークン分か。)
             "use_top_k_sampling": top_k is not None,  # True: top K サンプリングを有効にする
             "top_k_value": top_k,  # top K サンプリングの値。
             "use_top_p_sampling": top_p is not None,  # True: top P サンプリングを有効にする
             "top_p_value": top_p,  # top P サンプリングの値
             "use_repetition_penalty": repetition_penalty is not None,  # True:繰り返し同じトークンを生成したときのペナルティを有効する
-            "repetition_penalty": repetition_penalty is not None,  # ペナルティの値
+            "repetition_penalty": repetition_penalty,  # ペナルティの値
             "repetition_penalty_method": repetition_penalty_method,  # ペナルティの計算方法
             "add_special_tokens": add_special_tokens,  # トークナイザーの add_special_tokens 設定
         }
 
         self.too_many_request_as_http_error = too_many_request_as_http_error
 
         self.chat_prompt_clazz = chat_prompt_clazz
@@ -174,14 +177,46 @@
 
         # この request がリクエスト処理キューで処理されるのをまつ
         await this_request_semaphore.acquire()  # 処理待ち用カウントセマフォが releaseされるのを待つ / Wait for the waiting count semaphore to be released
 
         self.logger.debug(f"{req_id(request)} このリクエスト用セマフォは解放された")
         return await future_result
 
+    async def handle_clear_context_request(self, request: Request, request_body=None, callback=None):
+        """
+        コンテクストをクリアする
+        (TODO セッションハンドラーが前提となっているため、 simple_session_request_handler.py に委譲すること)
+        :param request:
+        :param request_body:
+        :param callback:
+        :return:
+        """
+        try:
+            session_mgr = getattr(request.state, "session", None)
+            if session_mgr:
+                # セッションオブジェクト（辞書オブジェクト）を取得する
+                session = session_mgr.get_session()
+                chat_prompt = session.get("chat_prompt")
+                if chat_prompt:
+                    session.pop("chat_prompt", None)  # 削除する
+
+                # session_mgr.clear_session()
+                self.logger.debug(f"sid:{session_mgr.get_session_id()} コンテクストがクリアされました")
+
+                return {"success": True, "message": "context successfully cleared"}
+            else:
+                self.logger.debug(f"コンテクストをクリアしようとしましたが、セッションは存在しませんでした")
+                return {"success": False, "message": "no context."}
+
+        except Exception as e:
+            tb = traceback.format_exc()
+            sys.stderr.write(tb)
+            self.logger.debug(f"コンテクストをクリアしようとしたところ予期せぬエラーが発生しました")
+            return {"success": False, "message": "error occurred"}
+
     async def handle_console_input(self, user_input: str) -> Generator:
         """
         コンソールチャット向けのクライアントからの入力を処理し、対応するレスポンスを生成する
         本メソッドはモデル入出力と挙動のカジュアルな確認用に用いることができる
         
         :param user_input: ユーザーからの入力。この入力に基づいて事前学習済モデルがレスポンスを生成する
         :rtype: Generator
@@ -322,7 +357,34 @@
         Starts the queue worker and registers the force termination and shutdown handlers.
         """
 
         self.queue_worker_task = asyncio.create_task(self.queue_worker())  # キューワーカーを開始
 
         # 強制終了のシャットダウンハンドラを登録
         signal.signal(signal.SIGINT, lambda s, f: os._exit(0))
+
+    def _send_resource(self, file_name, response: Response, replacer=None):
+
+        data = pkg_resources.read_text(f"{__package__}.data", file_name)
+        if replacer:
+            data = replacer(data)
+
+        response.body = data.encode('utf-8')  # You need to encode string to bytes
+        response.media_type = "text/html"
+        response.status_code = 200  # Add this line
+
+        return response
+
+    def index(self, response: Response, opts={}):
+
+        ui_init_params = opts.get("ui_init_params", None)
+
+        if ui_init_params:
+            def replacer(text):
+                return text.replace('const opts = {}', f'const opts = {json.dumps(ui_init_params)}')
+
+            return self._send_resource(file_name="index.html", replacer=replacer, response=response)
+        else:
+            return self._send_resource(file_name="index.html", response=response)
+
+    def js(self, response: Response):
+        return self._send_resource(file_name="chatstream.js", response=response)
```

### Comparing `chatstream-0.1.5/chatstream/mock_response_example_text.py` & `chatstream-0.2.0/chatstream/mock_response_example_text.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.5/chatstream/request_handler/request_handler.py` & `chatstream-0.2.0/chatstream/request_handler/request_handler.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.5/chatstream/request_handler/simple_session_request_handler.py` & `chatstream-0.2.0/chatstream/request_handler/simple_session_request_handler.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.5/chatstream/util_request_id.py` & `chatstream-0.2.0/chatstream/util_request_id.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.5/setup.py` & `chatstream-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chatstream",
-    version="0.1.5",
+    version="0.2.0",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="A streaming chat toolkit for pre-trained large language models(LLM)",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/ChatStream",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples","doc","doc.*"]),
@@ -19,10 +19,11 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.8",
     install_requires=[
         "fastapi",
         "fastsession",
-        "tokflow"
+        "tokflow",
+        "loadtime"
     ]
 )
```

