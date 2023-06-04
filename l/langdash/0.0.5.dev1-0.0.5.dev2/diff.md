# Comparing `tmp/langdash-0.0.5.dev1.tar.gz` & `tmp/langdash-0.0.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-0.0.5.dev1.tar", last modified: Fri Jun  2 02:00:55 2023, max compression
+gzip compressed data, was "langdash-0.0.5.dev2.tar", last modified: Sat Jun  3 07:01:52 2023, max compression
```

## Comparing `langdash-0.0.5.dev1.tar` & `langdash-0.0.5.dev2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.5.dev1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-0.0.5.dev1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3600 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2690 2023-05-31 21:54:27.000000 langdash-0.0.5.dev1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       66 2023-06-02 01:58:48.000000 langdash-0.0.5.dev1/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    18804 2023-06-02 01:08:06.000000 langdash-0.0.5.dev1/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.262499 langdash-0.0.5.dev1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.5.dev1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.5.dev1/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     4314 2023-06-01 22:52:48.000000 langdash-0.0.5.dev1/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      690 2023-05-31 17:39:51.000000 langdash-0.0.5.dev1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1223 2023-05-31 17:04:37.000000 langdash-0.0.5.dev1/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7535 2023-06-02 01:14:27.000000 langdash-0.0.5.dev1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.5.dev1/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4698 2023-06-01 18:29:41.000000 langdash-0.0.5.dev1/langdash/models/llamacpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      682 2023-05-31 21:23:49.000000 langdash-0.0.5.dev1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     7462 2023-06-02 01:18:48.000000 langdash-0.0.5.dev1/langdash/models/rwkvcpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      958 2023-05-31 20:11:54.000000 langdash-0.0.5.dev1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6250 2023-06-02 01:19:21.000000 langdash-0.0.5.dev1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      835 2023-05-31 17:40:54.000000 langdash-0.0.5.dev1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2598 2023-06-02 00:56:32.000000 langdash-0.0.5.dev1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.5.dev1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.5.dev1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.5.dev1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.5.dev1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3600 2023-06-02 02:00:55.000000 langdash-0.0.5.dev1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1242 2023-06-02 02:00:55.000000 langdash-0.0.5.dev1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-02 02:00:55.000000 langdash-0.0.5.dev1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      161 2023-06-02 02:00:55.000000 langdash-0.0.5.dev1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-02 02:00:55.000000 langdash-0.0.5.dev1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1522 2023-06-01 18:02:29.000000 langdash-0.0.5.dev1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 07:01:52.758509 langdash-0.0.5.dev2/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.5.dev2/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-0.0.5.dev2/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3600 2023-06-03 07:01:52.758509 langdash-0.0.5.dev2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2690 2023-05-31 21:54:27.000000 langdash-0.0.5.dev2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 07:01:52.754509 langdash-0.0.5.dev2/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       66 2023-06-02 03:48:05.000000 langdash-0.0.5.dev2/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18813 2023-06-02 03:35:57.000000 langdash-0.0.5.dev2/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 07:01:52.750509 langdash-0.0.5.dev2/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.5.dev2/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.5.dev2/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4310 2023-06-02 03:11:36.000000 langdash-0.0.5.dev2/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      716 2023-06-02 04:03:21.000000 langdash-0.0.5.dev2/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1223 2023-05-31 17:04:37.000000 langdash-0.0.5.dev2/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6872 2023-06-02 02:57:30.000000 langdash-0.0.5.dev2/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 07:01:52.758509 langdash-0.0.5.dev2/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.5.dev2/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4698 2023-06-01 18:29:41.000000 langdash-0.0.5.dev2/langdash/models/llamacpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      682 2023-05-31 21:23:49.000000 langdash-0.0.5.dev2/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8039 2023-06-02 06:01:58.000000 langdash-0.0.5.dev2/langdash/models/rwkvcpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      958 2023-05-31 20:11:54.000000 langdash-0.0.5.dev2/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6830 2023-06-02 16:20:58.000000 langdash-0.0.5.dev2/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      835 2023-05-31 17:40:54.000000 langdash-0.0.5.dev2/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2591 2023-06-02 03:34:57.000000 langdash-0.0.5.dev2/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 07:01:52.754509 langdash-0.0.5.dev2/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.5.dev2/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.5.dev2/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.5.dev2/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.5.dev2/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-03 07:01:52.758509 langdash-0.0.5.dev2/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3600 2023-06-03 07:01:52.000000 langdash-0.0.5.dev2/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1242 2023-06-03 07:01:52.000000 langdash-0.0.5.dev2/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-03 07:01:52.000000 langdash-0.0.5.dev2/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      161 2023-06-03 07:01:52.000000 langdash-0.0.5.dev2/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-03 07:01:52.000000 langdash-0.0.5.dev2/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-03 07:01:52.758509 langdash-0.0.5.dev2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1522 2023-06-01 18:02:29.000000 langdash-0.0.5.dev2/setup.py
```

### Comparing `langdash-0.0.5.dev1/LICENSE.txt` & `langdash-0.0.5.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/PKG-INFO` & `langdash-0.0.5.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.5.dev1
+Version: 0.0.5.dev2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-0.0.5.dev1/README.md` & `langdash-0.0.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/langdash/chains.py` & `langdash-0.0.5.dev2/langdash/chains.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 from collections import OrderedDict
 from typing import Generator, Dict, Any, List, Union, Optional, Type, Tuple, FrozenSet, TYPE_CHECKING
 import re
 import random
 import copy
+import warnings
 
 from langdash.response import Response, RespInfer, RespInject, RespReturns
 from langdash.infer import InferArgs
 
 if TYPE_CHECKING:
   from langdash._langdash import Langdash
   from langdash.llm_session import LLMGenerationSession, LLMState
@@ -260,15 +261,15 @@
     
     Args:
       cache_store (LDChainCacheStore): The cache store.
     """
     if self._model != cache_store._model:
       raise ValueError("model mismatch for LDChainCacheStore")
     if self._model_kwargs != cache_store._model_kwargs:
-      raise UserWarning("model kwargs does not match LDChainCacheStore, unexpected behavior might occur")
+      warnings.warn("model kwargs does not match LDChainCacheStore, unexpected behavior might occur", UserWarning)
     self._state_cache = cache_store._dict
   
   def save_cache_store(self) -> LDChainCacheStore:
     """ Saves the cache store into an object. """
     return LDChainCacheStore(
       _dict=copy.deepcopy(self._state_cache),
       _model=self._model,
@@ -492,26 +493,26 @@
 class LDReturns(LDNode):
   """ Return node """
   
   def __init__(self, ld: "Langdash",
                returns: str,
                end: Optional[Union[str, int]],
                padleft: str = "",
-               inference_args: Optional[InferArgs] = None):
+               infer_args: Optional[InferArgs] = None):
     super().__init__(ld)
     self._returns = returns
     self._end = end
     self._padleft = padleft
-    self._inference_args = inference_args
+    self._infer_args = infer_args
   
   def __repr__(self):
     return f"<Returns arg={self._returns}>"
   
   def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
-    for i, respinfer in enumerate(session.infer(end=self._end, args=self._inference_args)):
+    for i, respinfer in enumerate(session.infer(end=self._end, args=self._infer_args)):
       if i == 0:
         if self._padleft and respinfer.tokstr.startswith(self._padleft):
           respinfer.tokstr = respinfer.tokstr[len(self._padleft):]
       yield respinfer
       
 class LDChoice(LDNode):
   """ Choice node """
```

### Comparing `langdash-0.0.5.dev1/langdash/classify/token_qa.py` & `langdash-0.0.5.dev2/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/langdash/core.py` & `langdash-0.0.5.dev2/langdash/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
       returns (str): The name of the return value.
       end (str):
         Where to stop the inference. Either a string, or a token id.
         If None is passed, the inference will continue forever (for streaming).
       padleft (str):
         The left padding value for the return. If the generated string starts with
         *padleft* then it will be stripped.
-      inference_args (Optional[InferArgs]):
+      infer_args (Optional[InferArgs]):
         Optional inference arguments for generation.
 
     Returns:
       The return node.
     """
     return LDReturns(self, *args, **kwargs)
```

### Comparing `langdash-0.0.5.dev1/langdash/infer.py` & `langdash-0.0.5.dev2/langdash/infer.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,13 +9,14 @@
     max_new_tokens: Maximum number of new tokens to generate
     temperature: Temperature
     top_p: Top-P. If typical sampling isn't used, generation defaults to top-p sampling
     typical_mass: Mass parameter. If set, generation will use typical sampling
     max_rep_ctx: Maximum number of tokens to look back for repetition penalty
     rep_penalty: Repetition penalty, applied to logits for every token
   """
+  min_new_tokens: int = 0
   max_new_tokens: int = 512
-  temperature: float = 0.0
+  temperature: float = 1.0
   top_p: float = 0.0
   typical_mass: float = 0.0
   max_rep_ctx: int = 64
   rep_penalty: float = 1.0
```

### Comparing `langdash-0.0.5.dev1/langdash/llm.py` & `langdash-0.0.5.dev2/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/langdash/llm_session.py` & `langdash-0.0.5.dev2/langdash/llm_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,37 +181,21 @@
       tokens = [text]
     if not tokens:
       return 0
     
     num_toks = 0
       
     if self.token_healing:
-      init_offset = 0
       if self._next_token is not None:
-        tokid, tokstr = self._next_token
-        healed_str = self.decode([tokid, tokens[0]])
-        healed_tokens = self.tokenize(healed_str, add_special_tokens=add_special_tokens)
-        
-        if len(tokens) == 1:
-          if len(healed_tokens) == 1:
-            self._next_token = (healed_tokens[0], healed_str)
-            return 1
-          else:
-            # handle rare case where 1 input token maps to 2 or more "healed" tokens
-            self._logits = self._eval_mult(healed_tokens[:-1])
-            self._next_token = (healed_tokens[-1], self.decode(healed_tokens[-1:]))
-            return len(healed_tokens) - 1
-        else:
-          self._logits = self._eval_mult(healed_tokens)
-          init_offset = 1
-      
-      if len(tokens) - init_offset - 1 != 0:
-        self._logits = self._eval_mult(tokens[init_offset:-1])
-        num_toks += len(tokens) - init_offset - 1
-      self._next_token = (tokens[-1], self.decode(tokens[-1:]))
+        tokid, _ = self._next_token
+        tokens = self.tokenize(self.decode([tokid, *tokens]), add_special_tokens=add_special_tokens)
+      if len(tokens) > 1:
+        self._logits = self._eval_mult(tokens[:-1])
+        num_toks += len(tokens) - 1
+      self._next_token = (tokens[-1], self.decode([tokens[-1]]))
     else:
       if self._next_token is not None:
         tokid, tokstr = self._next_token
         self._eval(tokid)
         num_toks += 1
       self._logits = self._eval_mult(tokens)
       num_toks += len(tokens)
```

### Comparing `langdash-0.0.5.dev1/langdash/models/llamacpp.py` & `langdash-0.0.5.dev2/langdash/models/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/langdash/models/mock.py` & `langdash-0.0.5.dev2/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/langdash/models/rwkvcpp.py` & `langdash-0.0.5.dev2/langdash/models/rwkvcpp.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         rwkv_cpp_shared_library.RWKVSharedLibrary(_rwkv_lib),
         llm._model_path
       )
       tokenizer = tokenizers.Tokenizer.from_file(llm._tokenizer_path)
       return model, tokenizer
       
     self._rwkv, self._tokenizer = self._ld.get_model_internal(self.llm, load_model)
-    
+    self._space_token = "\u0120"
     self._logits, self._state = None, None
     self._next_token = None
   
   def _eval(self, tokid: int) -> torch.Tensor:
     self._logits, self._state = self._rwkv.eval(tokid, self._state)
     return self._logits
   
@@ -147,63 +147,75 @@
   def _infer(
     self,
     end: Optional[Union[str, int]],
     args: InferArgs) -> Generator[RespInfer, None, None]:
     generated = ""
     ctx: List[int] = []
     buffered_tokens: List[int] = []
-    stops_at_eot = (
-      (isinstance(end, str) and len(end) == 0) or
-      (isinstance(end, int) and end == 0)
-    )
+    
+    assert args.min_new_tokens >= 0, "min_new_tokens must be at least 0"
+    
+    if isinstance(end, str):
+      if len(end) == 0:
+        end = 0
+      elif args.min_new_tokens > 0:
+        endtoks = self.tokenize(end)
+        assert len(endtoks) == 1
+        end = endtoks[0]
     
     if self._logits is None:
       raise ValueError("no prompt provided for RWKVCppModel")
     
     for i in range(args.max_new_tokens):
-      strip_left = 0
+      strip_left = None
       
       if i == 0 and self._next_token is not None:
         tokid, tokstr = self._next_token
-        
-        for logits_tokstr, logits_tokid in self._tokenizer.get_vocab().items():
-          if not logits_tokstr.startswith(tokstr):
-            self._logits[logits_tokid] = -inf
+
+        if tokstr == " ":
+          for logits_tokstr, logits_tokid in self._tokenizer.get_vocab().items():
+            #https://github.com/openai/gpt-2/issues/80
+            #starts with 0x120
+            if not logits_tokstr.startswith(self._space_token):
+              self._logits[logits_tokid] = -inf
+        else:
+          for logits_tokstr, logits_tokid in self._tokenizer.get_vocab().items():
+            if not logits_tokstr.startswith(tokstr):
+              self._logits[logits_tokid] = -inf
             
         if self._logits.isinf().all():
           # we don't need to heal tokens because no token that begins with _next_token
           self._logits, self._state = self._rwkv.eval(tokid, self._state)
         else:
-          strip_left = len(tokstr)
+          strip_left = tokstr
         
-      if not stops_at_eot: # no early endoftext
+      if end != 0: # no early endoftext
         self._logits[0] = -inf
+      elif args.min_new_tokens > 0 and i < args.min_new_tokens:
+        self._logits[end] = -inf
       
       tokid = sampling.sample(self._logits, args, ctx)
       ctx.append(tokid)
       
       if tokid == end: # implies end is int
         break
       
-      if stops_at_eot and tokid == 0:
-        break
-      
       tokstr = self._tokenizer.decode([tokid])
       
       if "\ufffd" in tokstr:
         buffered_tokens.append(tokid)
         self._next_token = (tokid, "")
       else:
         if buffered_tokens:
           tokstr = self._tokenizer.decode(buffered_tokens)
           tokstr += self._tokenizer.decode([tokid])
           buffered_tokens.clear()
         else:
-          if strip_left:
-            tokstr = tokstr[strip_left:]
+          if strip_left and tokstr.startswith(strip_left):
+            tokstr = tokstr[len(strip_left):]
       
         self._next_token = (tokid, tokstr)
         
         generated += tokstr
         if isinstance(end, str) and end and generated.endswith(end):
           generated = generated[:-len(end)]
           break
```

### Comparing `langdash-0.0.5.dev1/langdash/models/sentence_transformers.py` & `langdash-0.0.5.dev2/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/langdash/models/transformers.py` & `langdash-0.0.5.dev2/langdash/models/transformers.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,18 +8,26 @@
 from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
 from langdash.infer import InferArgs
 import langdash.sampling as sampling
 
 import transformers
 import torch
 
+try:
+  from transformers import RwkvForCausalLM as t_RwkvForCausalLM
+  def model_is_rwkv(model):
+    return isinstance(model, t_RwkvForCausalLM)
+except ImportError:
+  def model_is_rwkv(model):
+    return False
+
 @dataclass
 class TransformersState(LLMState):
   _logits: Optional[torch.Tensor] = None
-  _past_key_values: Any = None
+  _state: Any = None
   _next_token: Optional[Tuple[int, str]] = None
 
 class TransformersSession(LLMGenerationSessionForRawText["TransformersModel", TransformersState, torch.Tensor]):
   """
   Session for transformers model.
   """
   
@@ -47,98 +55,113 @@
         v for k, v in self._tokenizer.get_vocab().items() if "\u0122" in k
       )
     else:
       self._space_token = " "
       self._buffered_token_head = set()
 
     self._logits = None
-    self._past_key_values = None
+    self._state = None
     self._next_token = None
   
   def _heal_token(self, tok_a: int, tok_b: int) -> str:
     return self._tokenizer.decode([tok_a, tok_b])
   
   def set_state(self, state: Optional[TransformersState]):
     if state is None:
       self._logits = None
-      self._past_key_values = None
+      self._state = None
       self._next_token = None
     else:
       self._logits = copy.deepcopy(state._logits)
-      self._past_key_values = copy.deepcopy(state._past_key_values)
+      self._state = copy.deepcopy(state._state)
       self._next_token = state._next_token
     
   def clone_state(self) -> TransformersState:
     return TransformersState(
       _logits = copy.deepcopy(self._logits),
-      _past_key_values = copy.deepcopy(self._past_key_values),
+      _state = copy.deepcopy(self._state),
       _next_token = self._next_token,
     )
   
   def _eval(self, tokid: int):
-    outputs = self._model.forward(
-      torch.IntTensor([tokid]),
-      past_key_values=self._past_key_values,
-      use_cache=True
-    )
-    self._past_key_values = outputs.past_key_values
+    if model_is_rwkv(self._model):
+      outputs = self._model.forward(
+        torch.IntTensor([tokid]),
+        state=self._state,
+        use_cache=True
+      )
+      self._state = outputs.state
+    else:
+      outputs = self._model.forward(
+        torch.IntTensor([tokid]),
+        past_key_values=self._state,
+        use_cache=True
+      )
+      self._state = outputs.past_key_values
     return outputs.logits[-1]
   
   def decode(self, tokids: List[int]) -> str:
     return self._tokenizer.decode(tokids)
   
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
     return self._tokenizer.encode(text, add_special_tokens=add_special_tokens).tolist()
   
   def _next_token_probs(self) -> torch.Tensor:
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
-      logits = self._model.forward(
-        torch.IntTensor([self._next_token[0]]),
-        past_key_values=self._past_key_values,
-        use_cache=True
-      )._logits[-1]
+      if model_is_rwkv(self._model):
+        logits = self._model.forward(
+          torch.IntTensor([self._next_token[0]]),
+          state=self._state,
+          use_cache=True
+        )._logits[-1]
+      else:
+        logits = self._model.forward(
+          torch.IntTensor([self._next_token[0]]),
+          past_key_values=self._state,
+          use_cache=True
+        )._logits[-1]
     return sampling.logits_to_probs(logits)
   
   def _infer(self,
             end: Optional[Union[str, int]],
             args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
     generated = ""
     ctx: List[int] = []
     buffered_tokens: List[int] = []
     stops_at_eot = (
       (isinstance(end, str) and len(end) == 0) or
       (isinstance(end, int) and end == self._tokenizer.eos_token_id)
     )
     
     for i in range(args.max_new_tokens):
-      strip_left = 0
+      strip_left = None
       
       if i == 0 and self._next_token is not None:
         tokid, tokstr = self._next_token
         
         if tokstr == " ":
           for logits_tokstr, logits_tokid in self._tokenizer.get_vocab().items():
             #https://github.com/openai/gpt-2/issues/80
             #starts with 0x120
-            if logits_tokstr.startswith(self._space_token):
+            if not logits_tokstr.startswith(self._space_token):
               self._logits[logits_tokid] = -inf
-          strip_left = 1
         else:
           for logits_tokstr, logits_tokid in self._tokenizer.get_vocab().items():
             if not logits_tokstr.startswith(tokstr):
               self._logits[logits_tokid] = -inf
-          strip_left = len(tokstr)
           
         if self._logits.isinf().all():
           # we don't need to heal tokens because no token that begins with _next_token
           self._logits = self._eval(tokid)
+        else:
+          strip_left = tokstr
       
       if not stops_at_eot: # no early endoftext
         self._logits[0] = -inf
       
       tokid = sampling.sample(self._logits, args, ctx)
       ctx.append(tokid)
       
@@ -149,16 +172,16 @@
       else:
         if buffered_tokens:
           tokstr = self._tokenizer.decode(buffered_tokens + [tokid])
           buffered_tokens = []
         else:
           tokstr = self._tokenizer.decode([tokid])
         
-        if strip_left:
-          tokstr = tokstr[strip_left:]
+        if strip_left and tokstr.startswith(tokstr):
+          tokstr = tokstr[len(strip_left):]
         
         self._next_token = (tokid, tokstr)
         
         generated += tokstr
         if isinstance(end, str) and end and generated.endswith(end):
           generated = generated[:-len(end)]
           break
```

### Comparing `langdash-0.0.5.dev1/langdash/response.py` & `langdash-0.0.5.dev2/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/langdash/sampling.py` & `langdash-0.0.5.dev2/langdash/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
   logits: torch.FloatTensor,
   args: InferArgs,
   ctx: List[int]
 ) -> torch.Tensor:
   # apply repetition penalty
   if args.rep_penalty != 1.0:
     rep_penalty = args.rep_penalty
-    assert 0.0 <= rep_penalty <= 1.0, "rep_penalty must be in [0.0, 1.0]"
+    assert 0.0 <= rep_penalty, "rep_penalty must be in [0.0, inf]"
     for _, tok in zip(range(args.max_rep_ctx), reversed(ctx)):
       if logits[tok] < 0.0:
         logits[tok] *= rep_penalty
       else:
         logits[tok] /= rep_penalty
   
   # probabilities
@@ -52,15 +52,15 @@
     # typical
     probs = _sample_typical(logits, args.typical_mass)
   else:
     # top-p
     probs = _sample_top_p(logits, args.top_p)
   
   # apply temperature
-  if args.temperature != 0.0:
+  if args.temperature != 1.0:
     probs = probs.pow(1.0 / args.temperature)
     
   return probs
 
 def sample(*args, **kwargs) -> int:
   """
   Sample from a distribution of tokens specified by *logits*.
```

### Comparing `langdash-0.0.5.dev1/langdash/search/embedding_search.py` & `langdash-0.0.5.dev2/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/langdash/search/multichoice_search.py` & `langdash-0.0.5.dev2/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/langdash.egg-info/PKG-INFO` & `langdash-0.0.5.dev2/langdash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.5.dev1
+Version: 0.0.5.dev2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-0.0.5.dev1/langdash.egg-info/SOURCES.txt` & `langdash-0.0.5.dev2/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.5.dev1/setup.py` & `langdash-0.0.5.dev2/setup.py`

 * *Files identical despite different names*

