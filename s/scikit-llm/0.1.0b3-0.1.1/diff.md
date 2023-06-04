# Comparing `tmp/scikit-llm-0.1.0b3.tar.gz` & `tmp/scikit-llm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-llm-0.1.0b3.tar", last modified: Wed May 24 20:41:20 2023, max compression
+gzip compressed data, was "scikit-llm-0.1.1.tar", last modified: Sun Jun  4 11:56:33 2023, max compression
```

## Comparing `scikit-llm-0.1.0b3.tar` & `scikit-llm-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,44 @@
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.193965 scikit-llm-0.1.0b3/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1077 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b3/LICENSE
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     7102 2023-05-24 20:41:20.193643 scikit-llm-0.1.0b3/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     6569 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/README.md
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      780 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/pyproject.toml
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.185584 scikit-llm-0.1.0b3/scikit_llm.egg-info/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     7102 2023-05-24 20:41:20.000000 scikit-llm-0.1.0b3/scikit_llm.egg-info/PKG-INFO
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      661 2023-05-24 20:41:20.000000 scikit-llm-0.1.0b3/scikit_llm.egg-info/SOURCES.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        1 2023-05-24 20:41:20.000000 scikit-llm-0.1.0b3/scikit_llm.egg-info/dependency_links.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       62 2023-05-24 20:41:20.000000 scikit-llm-0.1.0b3/scikit_llm.egg-info/requires.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)        6 2023-05-24 20:41:20.000000 scikit-llm-0.1.0b3/scikit_llm.egg-info/top_level.txt
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       38 2023-05-24 20:41:20.194186 scikit-llm-0.1.0b3/setup.cfg
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.186932 scikit-llm-0.1.0b3/skllm/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)       97 2023-05-12 18:41:11.000000 scikit-llm-0.1.0b3/skllm/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-05-13 17:42:03.000000 scikit-llm-0.1.0b3/skllm/config.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.188471 scikit-llm-0.1.0b3/skllm/datasets/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      209 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/datasets/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5870 2023-05-13 15:02:46.000000 scikit-llm-0.1.0b3/skllm/datasets/multi_class.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1438 2023-05-13 15:03:34.000000 scikit-llm-0.1.0b3/skllm/datasets/multi_label.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     2729 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/datasets/summarization.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.188818 scikit-llm-0.1.0b3/skllm/models/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     5070 2023-05-19 19:12:30.000000 scikit-llm-0.1.0b3/skllm/models/gpt_zero_shot_clf.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.191778 scikit-llm-0.1.0b3/skllm/openai/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1822 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/openai/base_gpt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1151 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/openai/chatgpt.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      111 2023-05-19 18:59:36.000000 scikit-llm-0.1.0b3/skllm/openai/credentials.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      894 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/openai/embeddings.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      730 2023-05-19 19:11:38.000000 scikit-llm-0.1.0b3/skllm/openai/mixin.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     2554 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/openai/prompts.py
-drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-05-24 20:41:20.192870 scikit-llm-0.1.0b3/skllm/preprocessing/
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      121 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/preprocessing/__init__.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      694 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/preprocessing/gpt_summarizer.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)     1394 2023-05-19 19:23:03.000000 scikit-llm-0.1.0b3/skllm/preprocessing/gpt_vectorizer.py
--rw-r--r--   0 kostrominoleg   (501) staff       (20)      296 2023-05-24 20:40:54.000000 scikit-llm-0.1.0b3/skllm/utils.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.546259 scikit-llm-0.1.1/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1077 2023-05-12 18:41:11.000000 scikit-llm-0.1.1/LICENSE
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)    10249 2023-06-04 11:56:33.545508 scikit-llm-0.1.1/PKG-INFO
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     9695 2023-06-03 20:09:48.000000 scikit-llm-0.1.1/README.md
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1885 2023-06-04 11:56:13.000000 scikit-llm-0.1.1/pyproject.toml
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.531133 scikit-llm-0.1.1/scikit_llm.egg-info/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)    10249 2023-06-04 11:56:33.000000 scikit-llm-0.1.1/scikit_llm.egg-info/PKG-INFO
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      890 2023-06-04 11:56:33.000000 scikit-llm-0.1.1/scikit_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)        1 2023-06-04 11:56:33.000000 scikit-llm-0.1.1/scikit_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       88 2023-06-04 11:56:33.000000 scikit-llm-0.1.1/scikit_llm.egg-info/requires.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)        6 2023-06-04 11:56:33.000000 scikit-llm-0.1.1/scikit_llm.egg-info/top_level.txt
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)       38 2023-06-04 11:56:33.546462 scikit-llm-0.1.1/setup.cfg
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.533531 scikit-llm-0.1.1/skllm/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      174 2023-05-29 19:35:15.000000 scikit-llm-0.1.1/skllm/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      502 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/completions.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      592 2023-05-13 17:42:03.000000 scikit-llm-0.1.1/skllm/config.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.536260 scikit-llm-0.1.1/skllm/datasets/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      273 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/datasets/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     5870 2023-05-13 15:02:46.000000 scikit-llm-0.1.1/skllm/datasets/multi_class.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1438 2023-05-13 15:03:34.000000 scikit-llm-0.1.1/skllm/datasets/multi_label.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     2729 2023-05-24 20:40:54.000000 scikit-llm-0.1.1/skllm/datasets/summarization.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      818 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/datasets/translation.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      612 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/gpt4all_client.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.537345 scikit-llm-0.1.1/skllm/models/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1918 2023-05-29 19:35:15.000000 scikit-llm-0.1.1/skllm/models/gpt_few_shot_clf.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     5477 2023-06-04 11:52:37.000000 scikit-llm-0.1.1/skllm/models/gpt_zero_shot_clf.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.540144 scikit-llm-0.1.1/skllm/openai/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1822 2023-05-24 20:40:54.000000 scikit-llm-0.1.1/skllm/openai/base_gpt.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1495 2023-06-04 11:52:37.000000 scikit-llm-0.1.1/skllm/openai/chatgpt.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      111 2023-05-19 18:59:36.000000 scikit-llm-0.1.1/skllm/openai/credentials.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      894 2023-05-24 20:40:54.000000 scikit-llm-0.1.1/skllm/openai/embeddings.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      730 2023-05-19 19:11:38.000000 scikit-llm-0.1.1/skllm/openai/mixin.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.542394 scikit-llm-0.1.1/skllm/preprocessing/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      183 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/preprocessing/__init__.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      698 2023-05-29 11:02:42.000000 scikit-llm-0.1.1/skllm/preprocessing/gpt_summarizer.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1003 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/preprocessing/gpt_translator.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1394 2023-05-28 18:52:20.000000 scikit-llm-0.1.1/skllm/preprocessing/gpt_vectorizer.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.543612 scikit-llm-0.1.1/skllm/prompts/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     3381 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/prompts/builders.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     3608 2023-06-04 11:52:37.000000 scikit-llm-0.1.1/skllm/prompts/templates.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)      525 2023-05-30 12:28:04.000000 scikit-llm-0.1.1/skllm/utils.py
+drwxr-xr-x   0 kostrominoleg   (501) staff       (20)        0 2023-06-04 11:56:33.544754 scikit-llm-0.1.1/tests/
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1689 2023-05-28 18:51:57.000000 scikit-llm-0.1.1/tests/test_chatgpt.py
+-rw-r--r--   0 kostrominoleg   (501) staff       (20)     1923 2023-05-28 19:26:40.000000 scikit-llm-0.1.1/tests/test_gpt_zero_shot_clf.py
```

### Comparing `scikit-llm-0.1.0b3/LICENSE` & `scikit-llm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b3/scikit_llm.egg-info/SOURCES.txt` & `scikit-llm-0.1.1/scikit_llm.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -3,23 +3,31 @@
 pyproject.toml
 scikit_llm.egg-info/PKG-INFO
 scikit_llm.egg-info/SOURCES.txt
 scikit_llm.egg-info/dependency_links.txt
 scikit_llm.egg-info/requires.txt
 scikit_llm.egg-info/top_level.txt
 skllm/__init__.py
+skllm/completions.py
 skllm/config.py
+skllm/gpt4all_client.py
 skllm/utils.py
 skllm/datasets/__init__.py
 skllm/datasets/multi_class.py
 skllm/datasets/multi_label.py
 skllm/datasets/summarization.py
+skllm/datasets/translation.py
+skllm/models/gpt_few_shot_clf.py
 skllm/models/gpt_zero_shot_clf.py
 skllm/openai/base_gpt.py
 skllm/openai/chatgpt.py
 skllm/openai/credentials.py
 skllm/openai/embeddings.py
 skllm/openai/mixin.py
-skllm/openai/prompts.py
 skllm/preprocessing/__init__.py
 skllm/preprocessing/gpt_summarizer.py
-skllm/preprocessing/gpt_vectorizer.py
+skllm/preprocessing/gpt_translator.py
+skllm/preprocessing/gpt_vectorizer.py
+skllm/prompts/builders.py
+skllm/prompts/templates.py
+tests/test_chatgpt.py
+tests/test_gpt_zero_shot_clf.py
```

### Comparing `scikit-llm-0.1.0b3/skllm/config.py` & `scikit-llm-0.1.1/skllm/config.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b3/skllm/datasets/multi_class.py` & `scikit-llm-0.1.1/skllm/datasets/multi_class.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b3/skllm/datasets/multi_label.py` & `scikit-llm-0.1.1/skllm/datasets/multi_label.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b3/skllm/datasets/summarization.py` & `scikit-llm-0.1.1/skllm/datasets/summarization.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b3/skllm/models/gpt_zero_shot_clf.py` & `scikit-llm-0.1.1/skllm/models/gpt_zero_shot_clf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from typing import Optional, Union, List, Any
-import numpy as np
-import pandas as pd
-from collections import Counter
 import random
-from tqdm import tqdm
 from abc import ABC, abstractmethod
+from collections import Counter
+from typing import Any, List, Optional, Union
+
+import numpy as np
+import pandas as pd
 from sklearn.base import BaseEstimator, ClassifierMixin
-from skllm.openai.prompts import get_zero_shot_prompt_slc, get_zero_shot_prompt_mlc
-from skllm.openai.chatgpt import (
-    construct_message,
-    get_chat_completion,
-    extract_json_key,
+from tqdm import tqdm
+
+from skllm.completions import get_chat_completion
+from skllm.openai.chatgpt import construct_message, extract_json_key
+from skllm.openai.mixin import OpenAIMixin as _OAIMixin
+from skllm.prompts.builders import (
+    build_zero_shot_prompt_mlc,
+    build_zero_shot_prompt_slc,
 )
-from skllm.config import SKLLMConfig as _Config
 from skllm.utils import to_numpy as _to_numpy
-from skllm.openai.mixin import OpenAIMixin as _OAIMixin
+
 
 class _BaseZeroShotGPTClassifier(ABC, BaseEstimator, ClassifierMixin, _OAIMixin):
     def __init__(
         self,
         openai_key: Optional[str] = None,
         openai_org: Optional[str] = None,
         openai_model: str = "gpt-3.5-turbo",
@@ -30,15 +32,15 @@
         return _to_numpy(X)
 
     def fit(
         self,
         X: Optional[Union[np.ndarray, pd.Series, List[str]]],
         y: Union[np.ndarray, pd.Series, List[str], List[List[str]]],
     ):
-        X = self._to_np(X)        
+        X = self._to_np(X)
         self.classes_, self.probabilities_ = self._get_unique_targets(y)
         return self
 
     def predict(self, X: Union[np.ndarray, pd.Series, List[str]]):
         X = self._to_np(X)
         predictions = []
         for i in tqdm(range(len(X))):
@@ -87,27 +89,33 @@
         if isinstance(y, (pd.Series, np.ndarray)):
             labels = y.tolist()
         else:
             labels = y
         return labels
 
     def _get_prompt(self, x) -> str:
-        return get_zero_shot_prompt_slc(x, self.classes_)
+        return build_zero_shot_prompt_slc(x, repr(self.classes_))
 
     def _predict_single(self, x):
         completion = self._get_chat_completion(x)
         try:
             label = str(
-                extract_json_key(completion.choices[0].message["content"], "label")
+                extract_json_key(
+                    completion["choices"][0]["message"]["content"], "label"
+                )
             )
         except Exception as e:
+            print(completion)
+            print(f"Could not extract the label from the completion: {str(e)}")
             label = ""
 
         if label not in self.classes_:
-            label = random.choices(self.classes_, self.probabilities_)[0]
+            label = label.replace("'", "").replace('"', "")
+            if label not in self.classes_:  # try again
+                label = random.choices(self.classes_, self.probabilities_)[0]
         return label
 
     def fit(
         self,
         X: Optional[Union[np.ndarray, pd.Series, List[str]]],
         y: Union[np.ndarray, pd.Series, List[str]],
     ):
@@ -133,23 +141,26 @@
         for l in y:
             for j in l:
                 labels.append(j)
 
         return labels
 
     def _get_prompt(self, x) -> str:
-        return get_zero_shot_prompt_mlc(x, self.classes_, self.max_labels)
+        return build_zero_shot_prompt_mlc(x, repr(self.classes_), self.max_labels)
 
     def _predict_single(self, x):
         completion = self._get_chat_completion(x)
         try:
-            labels = extract_json_key(completion.choices[0].message["content"], "label")
+            labels = extract_json_key(completion["choices"][0]["message"]["content"], "label")
             if not isinstance(labels, list):
-                raise RuntimeError("Invalid labels type, expected list")
+                labels = labels.split(",")
+                labels = [l.strip() for l in labels]
         except Exception as e:
+            print(completion)
+            print(f"Could not extract the label from the completion: {str(e)}")
             labels = []
 
         labels = list(filter(lambda l: l in self.classes_, labels))
 
         if len(labels) > self.max_labels:
             labels = labels[: self.max_labels - 1]
         elif len(labels) < 1:
```

### Comparing `scikit-llm-0.1.0b3/skllm/openai/base_gpt.py` & `scikit-llm-0.1.1/skllm/openai/base_gpt.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b3/skllm/openai/chatgpt.py` & `scikit-llm-0.1.1/skllm/openai/chatgpt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,51 @@
-import openai
-from time import sleep
 import json
+from time import sleep
+
+import openai
+
 from skllm.openai.credentials import set_credentials
+from skllm.utils import find_json_in_string
+
 
 def construct_message(role, content):
     if role not in ("system", "user", "assistant"):
         raise ValueError("Invalid role")
     return {"role": role, "content": content}
 
-def get_chat_completion(messages, key, org, model="gpt-3.5-turbo", max_retries = 3):
+
+def get_chat_completion(messages, key, org, model="gpt-3.5-turbo", max_retries=3):
     set_credentials(key, org)
     error_msg = None
     error_type = None
     for _ in range(max_retries):
         try:
             completion = openai.ChatCompletion.create(
-                model=model, temperature=0., messages=messages
+                model=model, temperature=0.0, messages=messages
             )
             return completion
         except Exception as e:
             error_msg = str(e)
-            error_type =  type(e).__name__
+            error_type = type(e).__name__
             sleep(3)
-    print(f"Could not obtain the completion after {max_retries} retries: `{error_type} :: {error_msg}`")
+    print(
+        f"Could not obtain the completion after {max_retries} retries: `{error_type} ::"
+        f" {error_msg}`"
+    )
+
 
 def extract_json_key(json_, key):
-    try: 
-        as_json = json.loads(json_.replace('\n', '')) 
-        if key not in as_json.keys():
-            raise KeyError("The required key was not found")
-        return as_json[key]
-    except Exception as e:
-        return None
+    original_json = json_
+    for i in range(2):
+        try:
+            json_ = original_json.replace("\n", "")
+            if i == 1:
+                json_ = json_.replace("'", "\"")
+            json_ = find_json_in_string(json_)
+            as_json = json.loads(json_)
+            if key not in as_json.keys():
+                raise KeyError("The required key was not found")
+            return as_json[key]
+        except Exception:
+            if i == 0:
+                continue
+            return None
```

### Comparing `scikit-llm-0.1.0b3/skllm/openai/embeddings.py` & `scikit-llm-0.1.1/skllm/openai/embeddings.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b3/skllm/openai/mixin.py` & `scikit-llm-0.1.1/skllm/openai/mixin.py`

 * *Files identical despite different names*

### Comparing `scikit-llm-0.1.0b3/skllm/preprocessing/gpt_vectorizer.py` & `scikit-llm-0.1.1/skllm/preprocessing/gpt_vectorizer.py`

 * *Files identical despite different names*

