# Comparing `tmp/tokflow-1.0.2.tar.gz` & `tmp/tokflow-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokflow-1.0.2.tar", last modified: Mon May 22 02:52:46 2023, max compression
+gzip compressed data, was "tokflow-1.1.0.tar", last modified: Sun Jun  4 09:55:50 2023, max compression
```

## Comparing `tokflow-1.0.2.tar` & `tokflow-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 02:52:46.328494 tokflow-1.0.2/
--rw-rw-rw-   0        0        0    11364 2023-05-19 04:51:42.000000 tokflow-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4054 2023-05-22 02:52:46.328494 tokflow-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3332 2023-05-19 05:20:51.000000 tokflow-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 02:52:46.312326 tokflow-1.0.2/TokFlow.egg-info/
--rw-rw-rw-   0        0        0     4054 2023-05-22 02:52:46.000000 tokflow-1.0.2/TokFlow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-05-22 02:52:46.000000 tokflow-1.0.2/TokFlow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 02:52:46.000000 tokflow-1.0.2/TokFlow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 02:52:46.000000 tokflow-1.0.2/TokFlow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 02:52:46.328494 tokflow-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      888 2023-05-22 02:51:38.000000 tokflow-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 02:52:46.327494 tokflow-1.0.2/tokflow/
--rw-rw-rw-   0        0        0       72 2023-05-19 05:04:54.000000 tokflow-1.0.2/tokflow/__init__.py
--rw-rw-rw-   0        0        0     9784 2023-05-19 04:51:42.000000 tokflow-1.0.2/tokflow/tok_flow.py
--rw-rw-rw-   0        0        0     9059 2023-05-19 04:51:42.000000 tokflow-1.0.2/tokflow/tok_flow_worker.py
+drwxrwxrwx   0        0        0        0 2023-06-04 09:55:50.148610 tokflow-1.1.0/
+-rw-rw-rw-   0        0        0    11364 2023-05-19 04:51:42.000000 tokflow-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6114 2023-06-04 09:55:50.148610 tokflow-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5349 2023-06-04 09:53:45.000000 tokflow-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 09:55:50.111327 tokflow-1.1.0/TokFlow.egg-info/
+-rw-rw-rw-   0        0        0     6114 2023-06-04 09:55:50.000000 tokflow-1.1.0/TokFlow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2023-06-04 09:55:50.000000 tokflow-1.1.0/TokFlow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 09:55:50.000000 tokflow-1.1.0/TokFlow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-04 09:55:50.000000 tokflow-1.1.0/TokFlow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 09:55:50.148610 tokflow-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      888 2023-06-04 09:54:55.000000 tokflow-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 09:55:50.128874 tokflow-1.1.0/tests/
+-rw-rw-rw-   0        0        0     8777 2023-05-19 04:51:42.000000 tokflow-1.1.0/tests/test_refit_flow_worker.py
+-rw-rw-rw-   0        0        0    12117 2023-05-19 04:51:42.000000 tokflow-1.1.0/tests/test_tokflow_01_IN_spot_OUT_spot.py
+-rw-rw-rw-   0        0        0     1394 2023-06-04 07:54:15.000000 tokflow-1.1.0/tests/test_tokflow_02_IN_full_OUT_spot.py
+-rw-rw-rw-   0        0        0    32891 2023-06-04 06:56:56.000000 tokflow-1.1.0/tests/test_tokflow_02_data.py
+-rw-rw-rw-   0        0        0     1649 2023-06-04 09:37:08.000000 tokflow-1.1.0/tests/test_tokflow_03_IN_spot_OUT_full.py
+-rw-rw-rw-   0        0        0     1229 2023-06-04 09:38:29.000000 tokflow-1.1.0/tests/test_tokflow_04_IN_full_OUT_full.py
+drwxrwxrwx   0        0        0        0 2023-06-04 09:55:50.146611 tokflow-1.1.0/tokflow/
+-rw-rw-rw-   0        0        0       72 2023-05-19 05:04:54.000000 tokflow-1.1.0/tokflow/__init__.py
+-rw-rw-rw-   0        0        0    11997 2023-06-04 09:35:11.000000 tokflow-1.1.0/tokflow/tok_flow.py
+-rw-rw-rw-   0        0        0     9059 2023-05-19 04:51:42.000000 tokflow-1.1.0/tokflow/tok_flow_worker.py
```

### Comparing `tokflow-1.0.2/LICENSE` & `tokflow-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tokflow-1.0.2/PKG-INFO` & `tokflow-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokflow
-Version: 1.0.2
+Version: 1.1.0
 Summary: LLM utility of streaming token realtime replacement processing
 Home-page: https://github.com/riversun/TokFlow
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -80,15 +80,58 @@
 print(f"{tokf.flush()}", end="", flush=True)
 
 ```
 
 
 ![tokflow](https://github.com/riversun/TokFlow/assets/11747460/85f497bd-cf51-41d9-aaf5-ad5420f42b6a)
 
+# Generation Options
 
+The `put` method can take an optional parameter `opts` like `put(text,opts)`.
+
+`opts` can specify the format of the input and output, like `{"in_type":"spot","out_type:"spot" }`.
+
+It behaves as follows:
+
+| in_type  | out_type | Description                                    |
+| :------- | :------- | :---------------------------------------------- |
+| spot     | spot     | A mode that incrementally sends tokens to the `put` method, and outputs generated segments each time. |
+| spot     | full     | A mode that incrementally sends tokens to the `put` method, but outputs the full sentence. |
+| full     | spot     | A mode that sends the full sentence to the `put` method at once, but outputs generated segments each time. |
+| full     | full     | A mode that sends the full sentence to the `put` method at once, and outputs the full sentence. |
+
+Notes:
+- All text strings need to be sent to the `put` method before calling the `flush` method. Especially in `full` mode, all input strings are sent at once.
+- If the output type (`out_type`) is `full`, the `flush` method must be called to obtain the final result.
+- It's important to appropriately combine the call pattern of the `put` method and the use of the `flush` method to maintain consistency in each mode.
+
+**Code Example**
+
+Specify rules like `condition = {"in_type": "full", "out_type": "full"}`, and use `condition` as an argument for `put` and `flush`.
+
+```python
+    tokf = TokFlow([("<NL>", "\n")])
+
+    condition = {"in_type": "full", "out_type": "full"}
+    prev_len = 0
+    for input_token_base in get_example_texts():
+        output_sentence = tokf.put(input_token_base, condition)
+
+        print(f"output_sentence:{output_sentence}")
+
+        if prev_len > len(output_sentence):
+            raise ValueError("Length error")
+
+        if "<NL>" in output_sentence:
+            raise Exception("Failure Must be converted str found.")
+
+        prev_len = len(output_sentence)
+
+    output_sentence = tokf.flush(condition)
+```
 
 # Processing
 
 ## About Internal processing
 
 Tokens are sequentially read in real time.
 The token read is combined with the tokens read so far, referred to as the "token buffer".
```

### Comparing `tokflow-1.0.2/TokFlow.egg-info/PKG-INFO` & `tokflow-1.1.0/TokFlow.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokflow
-Version: 1.0.2
+Version: 1.1.0
 Summary: LLM utility of streaming token realtime replacement processing
 Home-page: https://github.com/riversun/TokFlow
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -80,15 +80,58 @@
 print(f"{tokf.flush()}", end="", flush=True)
 
 ```
 
 
 ![tokflow](https://github.com/riversun/TokFlow/assets/11747460/85f497bd-cf51-41d9-aaf5-ad5420f42b6a)
 
+# Generation Options
 
+The `put` method can take an optional parameter `opts` like `put(text,opts)`.
+
+`opts` can specify the format of the input and output, like `{"in_type":"spot","out_type:"spot" }`.
+
+It behaves as follows:
+
+| in_type  | out_type | Description                                    |
+| :------- | :------- | :---------------------------------------------- |
+| spot     | spot     | A mode that incrementally sends tokens to the `put` method, and outputs generated segments each time. |
+| spot     | full     | A mode that incrementally sends tokens to the `put` method, but outputs the full sentence. |
+| full     | spot     | A mode that sends the full sentence to the `put` method at once, but outputs generated segments each time. |
+| full     | full     | A mode that sends the full sentence to the `put` method at once, and outputs the full sentence. |
+
+Notes:
+- All text strings need to be sent to the `put` method before calling the `flush` method. Especially in `full` mode, all input strings are sent at once.
+- If the output type (`out_type`) is `full`, the `flush` method must be called to obtain the final result.
+- It's important to appropriately combine the call pattern of the `put` method and the use of the `flush` method to maintain consistency in each mode.
+
+**Code Example**
+
+Specify rules like `condition = {"in_type": "full", "out_type": "full"}`, and use `condition` as an argument for `put` and `flush`.
+
+```python
+    tokf = TokFlow([("<NL>", "\n")])
+
+    condition = {"in_type": "full", "out_type": "full"}
+    prev_len = 0
+    for input_token_base in get_example_texts():
+        output_sentence = tokf.put(input_token_base, condition)
+
+        print(f"output_sentence:{output_sentence}")
+
+        if prev_len > len(output_sentence):
+            raise ValueError("Length error")
+
+        if "<NL>" in output_sentence:
+            raise Exception("Failure Must be converted str found.")
+
+        prev_len = len(output_sentence)
+
+    output_sentence = tokf.flush(condition)
+```
 
 # Processing
 
 ## About Internal processing
 
 Tokens are sequentially read in real time.
 The token read is combined with the tokens read so far, referred to as the "token buffer".
```

### Comparing `tokflow-1.0.2/setup.py` & `tokflow-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tokflow",
-    version="1.0.2",
+    version="1.1.0",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="LLM utility of streaming token realtime replacement processing",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/TokFlow",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
```

### Comparing `tokflow-1.0.2/tokflow/tok_flow.py` & `tokflow-1.1.0/tokflow/tok_flow.py`

 * *Files 27% similar despite different names*

```diff
@@ -35,18 +35,50 @@
     逐次トークンのほとんどはそのまま逐次表示させ、置換が必要な場合には表示を遅らせる、というストリーム処理することができる。
     """
 
     def __init__(self, replacer_list):
         self.replacer_list = replacer_list
         self.workers = []
         self.not_consumed_str = ""
+        self.prev_input_full_sentence = ""
+        self.prev_output_full_sentence = ""
         for from_token, to_token in replacer_list:
             self.workers.append(TokFlowWorker(from_token, to_token))
 
-    def put(self, token_str):
+    def put(self, str, opts={}):
+        in_type = opts.get("in_type", "spot")
+        out_type = opts.get("out_type", "spot")
+
+        if in_type == "spot":
+            if out_type == "spot":
+                return self.put_spot(str)
+            elif out_type == "full":
+                self.prev_output_full_sentence += self.put_spot(str)
+                return self.prev_output_full_sentence
+            else:
+                raise ValueError(f'unknown out_type:"{out_type}"')
+        elif in_type == "full":
+            if out_type == "spot":
+                return self.put_sentence(str)
+            elif out_type == "full":
+                self.prev_output_full_sentence+=self.put_sentence(str)
+                return self.prev_output_full_sentence
+            else:
+                raise ValueError(f'unknown out_type:"{out_type}"')
+
+        else:
+            raise ValueError(f'unknown in_type:"{in_type}"')
+
+    def put_sentence(self, sentence_str):
+        input_token = sentence_str[len(self.prev_input_full_sentence):]
+        ret = self.put(input_token)
+        self.prev_input_full_sentence = sentence_str
+        return ret
+
+    def put_spot(self, token_str):
         """
         本メソッドにトークンを順次インプットしていくと、検索対象文字列が置換された状態の戻り値を返す。
 
         逐次処理をしていくため、あらかじめすべての完成した文字列を入力する必要はない。断片（トークン）を
         put していくだけで自動的に必要な置換を行う
 
         検索対象文字列の一部がputされると、今後供給されるトークンによっては検索文字列が出現する可能性がある。
@@ -126,17 +158,46 @@
             # ワーカーの1つから、マッチしなかった文字列を戻り値とする
             # 度のワーカーでも同じ unmatched_str を保持しているため、便宜的に0番目を返している
             ret_val = self.workers[0].unmatched_str
             pass
 
         return ret_val
 
-    def flush(self):
+    def flush(self,opts={}):
         """
         put処理が終了したあと、未消費のトークンバッファが残っている場合があるため、
         すべてのput処理が終了したあと、本メソッドを呼出し未消費のトークンバッファを取得する
         未消費のトークンバッファが存在すればそれも出力対象とする
         """
-        return self.not_consumed_str
+
+        in_type = opts.get("in_type", "spot")
+        out_type = opts.get("out_type", "spot")
+
+        if in_type == "spot":
+            if out_type == "spot":
+                final_str = self.not_consumed_str
+                pass
+            elif out_type == "full":
+                final_str = self.prev_output_full_sentence+self.not_consumed_str
+                pass
+            else:
+                raise ValueError(f'unknown out_type:"{out_type}"')
+        elif in_type == "full":
+            if out_type == "spot":
+                final_str = self.not_consumed_str
+                pass
+            elif out_type == "full":
+                final_str = self.prev_output_full_sentence + self.not_consumed_str
+                pass
+            else:
+                raise ValueError(f'unknown out_type:"{out_type}"')
+        else:
+            raise ValueError(f'unknown in_type:"{in_type}"')
+
+        self.prev_output_full_sentence = ""
+        self.prev_input_full_sentence = ""
+
+
+        return final_str
 
     def get_workers(self):
         return self.workers
```

### Comparing `tokflow-1.0.2/tokflow/tok_flow_worker.py` & `tokflow-1.1.0/tokflow/tok_flow_worker.py`

 * *Files identical despite different names*

