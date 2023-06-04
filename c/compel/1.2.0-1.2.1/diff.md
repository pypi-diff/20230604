# Comparing `tmp/compel-1.2.0.tar.gz` & `tmp/compel-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-t4pc895k/compel-1.2.0.tar", last modified: Sat Jun  3 18:39:27 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-sibov8rl/compel-1.2.1.tar", last modified: Sun Jun  4 13:28:28 2023, max compression
```

## Comparing `compel-1.2.0.tar` & `compel-1.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 18:39:27.000000 compel-1.2.0/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.2.0/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)    10987 2023-06-03 18:39:27.000000 compel-1.2.0/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)    10409 2023-06-03 18:38:59.000000 compel-1.2.0/README.md
--rw-r--r--   0 damian     (501) staff       (20)      761 2023-06-03 18:15:52.000000 compel-1.2.0/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-06-03 18:39:27.000000 compel-1.2.0/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 18:39:27.000000 compel-1.2.0/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-1.2.0/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    14940 2023-06-03 18:09:49.000000 compel-1.2.0/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.2.0/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.2.0/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-1.2.0/src/compel/diffusers_textual_inversion_manager.py
--rw-r--r--   0 damian     (501) staff       (20)    25187 2023-06-03 06:15:11.000000 compel-1.2.0/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    29912 2023-06-03 06:55:13.000000 compel-1.2.0/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)    10987 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      512 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 18:39:27.000000 compel-1.2.0/test/
--rw-r--r--   0 damian     (501) staff       (20)    15682 2023-06-03 18:14:58.000000 compel-1.2.0/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-1.2.0/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-1.2.0/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-04 13:28:28.000000 compel-1.2.1/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.2.1/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)    11033 2023-06-04 13:28:28.000000 compel-1.2.1/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)    10455 2023-06-04 12:40:31.000000 compel-1.2.1/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      761 2023-06-04 12:40:07.000000 compel-1.2.1/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-06-04 13:28:28.000000 compel-1.2.1/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-04 13:28:28.000000 compel-1.2.1/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-1.2.1/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    15856 2023-06-04 13:25:19.000000 compel-1.2.1/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.2.1/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.2.1/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-1.2.1/src/compel/diffusers_textual_inversion_manager.py
+-rw-r--r--   0 damian     (501) staff       (20)    25187 2023-06-03 06:15:11.000000 compel-1.2.1/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    29912 2023-06-03 06:55:13.000000 compel-1.2.1/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)    11033 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      512 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-06-04 13:28:28.000000 compel-1.2.1/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-04 13:28:28.000000 compel-1.2.1/test/
+-rw-r--r--   0 damian     (501) staff       (20)    15682 2023-06-03 18:14:58.000000 compel-1.2.1/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-1.2.1/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-1.2.1/test/test_prompt_parser.py
```

### Comparing `compel-1.2.0/LICENSE` & `compel-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-1.2.0/PKG-INFO` & `compel-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.2.0
+Version: 1.2.1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -89,14 +89,16 @@
 If you are using Compel heavily and repeatedly, you may run into PyTorch memory issues. To alleviate this, according to @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+#### 1.2.1 - actually apply `.and()` weights
+
 ### 1.2.0 - Concatenate embeddings using `.and()`
 
 For Stable Diffusion 2.1 I've been experimenting with a new feature: concatenated embeddings. What I noticed, for example, is that for more complex prompts image generation quality becomes wildly better when the prompt is broken into multiple parts and fed to OpenCLIP separately.
 
 TL;DR: you can now experiment with breaking up your prompts into segments, which for SD2.1 appears to improve the generated image. The syntax is `("prompt part 1", "prompt part 2").and()`. You can have more than one part, and you can also weight them, eg `("a man eating an apple", "sitting on the roof of a car", "high quality, trending on artstation, 8K UHD").and(1, 0.5, 0.5)` which will assign weight `1` to `man eating an apple` and `0.5` to `sitting on the roof of a car` and `high quality, trending on artstation, 8K UHD`. 
 
 Here's a nonsense example from the InvokeAI discord #garbage-bin channel, created by gogurt enjoyer's incredible [nightmare prompt generator](https://huggingface.co/cactusfriend/nightmare-invokeai-prompts):
```

### Comparing `compel-1.2.0/README.md` & `compel-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 If you are using Compel heavily and repeatedly, you may run into PyTorch memory issues. To alleviate this, according to @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+#### 1.2.1 - actually apply `.and()` weights
+
 ### 1.2.0 - Concatenate embeddings using `.and()`
 
 For Stable Diffusion 2.1 I've been experimenting with a new feature: concatenated embeddings. What I noticed, for example, is that for more complex prompts image generation quality becomes wildly better when the prompt is broken into multiple parts and fed to OpenCLIP separately.
 
 TL;DR: you can now experiment with breaking up your prompts into segments, which for SD2.1 appears to improve the generated image. The syntax is `("prompt part 1", "prompt part 2").and()`. You can have more than one part, and you can also weight them, eg `("a man eating an apple", "sitting on the roof of a car", "high quality, trending on artstation, 8K UHD").and(1, 0.5, 0.5)` which will assign weight `1` to `man eating an apple` and `0.5` to `sitting on the roof of a car` and `high quality, trending on artstation, 8K UHD`. 
 
 Here's a nonsense example from the InvokeAI discord #garbage-bin channel, created by gogurt enjoyer's incredible [nightmare prompt generator](https://huggingface.co/cactusfriend/nightmare-invokeai-prompts):
```

### Comparing `compel-1.2.0/pyproject.toml` & `compel-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-1.2.0/src/compel/compel.py` & `compel-1.2.1/src/compel/compel.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,23 +72,16 @@
             [positive_conditioning, negative_conditioning]
         )
         return StaticConditioningScheduler(positive_conditioning=positive_conditioning,
                                            negative_conditioning=negative_conditioning)
 
     def build_conditioning_tensor(self, text: str) -> torch.Tensor:
         conjunction = self.parse_prompt_string(text)
-        if len(conjunction.prompts) > 1 and conjunction.type != 'AND':
-            raise ValueError("Only AND conjunctions are supported by build_conditioning_tensor()")
-        # concatenate each prompt in the conjunction (typically there will only be 1)
-        to_concat = []
-        for p in conjunction.prompts:
-            conditioning, _ = self.build_conditioning_tensor_for_prompt_object(p)
-            to_concat.append(conditioning)
-        return torch.concat(to_concat, dim=1)
-
+        conditioning, _ = self.build_conditioning_tensor_for_conjunction(conjunction)
+        return conditioning
 
     @torch.no_grad()
     def __call__(self, text: Union[str, List[str]]) -> torch.FloatTensor:
         if not isinstance(text, list):
             text = [text]
 
         cond_tensor = []
@@ -129,14 +122,34 @@
                 cac_args = self._get_conditioning_for_cross_attention_control(prompt)
                 return cac_args.original_conditioning, { 'cross_attention_control': cac_args }
             else:
                 return self._get_conditioning_for_flattened_prompt(prompt), {}
 
         raise ValueError(f"unsupported prompt type: {type(prompt).__name__}")
 
+    def build_conditioning_tensor_for_conjunction(self, conjunction: Conjunction) -> Tuple[torch.Tensor, dict]:
+        if len(conjunction.prompts) > 1 and conjunction.type != 'AND':
+            raise ValueError("Only AND conjunctions are supported by build_conditioning_tensor()")
+        # concatenate each prompt in the conjunction (typically there will only be 1)
+        to_concat = []
+        options = {}
+        empty_conditioning = None
+        for i, p in enumerate(conjunction.prompts):
+            this_conditioning, this_options = self.build_conditioning_tensor_for_prompt_object(p)
+            options.update(this_options)  # this is not a smart way to do this but 🤷‍
+            weight = conjunction.weights[i]
+            if weight != 1:
+                # apply weight if we need to
+                empty_conditioning = self.build_conditioning_tensor('') if empty_conditioning is None else empty_conditioning
+                [padded_empty_conditioning, _] = self.pad_conditioning_tensors_to_same_length([empty_conditioning, this_conditioning])
+                this_conditioning = padded_empty_conditioning + (this_conditioning - padded_empty_conditioning) * weight
+            to_concat.append(this_conditioning)
+        return torch.concat(to_concat, dim=1), options
+
+
     def pad_conditioning_tensors_to_same_length(self, conditionings: List[torch.Tensor],
                                                 ) -> List[torch.Tensor]:
         """
         If `truncate_long_prompts` was set to False on initialization, conditioning tensors do not have a fixed length.
         This is a problem when using a negative and a positive prompt to condition the diffusion process. This function
         pads either c0 or c1 if necessary to ensure they both have the same length, returning the padded c0 and c1.
         """
```

### Comparing `compel-1.2.0/src/compel/conditioning_scheduler.py` & `compel-1.2.1/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.0/src/compel/cross_attention_control.py` & `compel-1.2.1/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.0/src/compel/diffusers_textual_inversion_manager.py` & `compel-1.2.1/src/compel/diffusers_textual_inversion_manager.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.0/src/compel/embeddings_provider.py` & `compel-1.2.1/src/compel/embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.0/src/compel/prompt_parser.py` & `compel-1.2.1/src/compel/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.0/src/compel.egg-info/PKG-INFO` & `compel-1.2.1/src/compel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.2.0
+Version: 1.2.1
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -89,14 +89,16 @@
 If you are using Compel heavily and repeatedly, you may run into PyTorch memory issues. To alleviate this, according to @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+#### 1.2.1 - actually apply `.and()` weights
+
 ### 1.2.0 - Concatenate embeddings using `.and()`
 
 For Stable Diffusion 2.1 I've been experimenting with a new feature: concatenated embeddings. What I noticed, for example, is that for more complex prompts image generation quality becomes wildly better when the prompt is broken into multiple parts and fed to OpenCLIP separately.
 
 TL;DR: you can now experiment with breaking up your prompts into segments, which for SD2.1 appears to improve the generated image. The syntax is `("prompt part 1", "prompt part 2").and()`. You can have more than one part, and you can also weight them, eg `("a man eating an apple", "sitting on the roof of a car", "high quality, trending on artstation, 8K UHD").and(1, 0.5, 0.5)` which will assign weight `1` to `man eating an apple` and `0.5` to `sitting on the roof of a car` and `high quality, trending on artstation, 8K UHD`. 
 
 Here's a nonsense example from the InvokeAI discord #garbage-bin channel, created by gogurt enjoyer's incredible [nightmare prompt generator](https://huggingface.co/cactusfriend/nightmare-invokeai-prompts):
```

### Comparing `compel-1.2.0/src/compel.egg-info/SOURCES.txt` & `compel-1.2.1/src/compel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compel-1.2.0/test/test_compel.py` & `compel-1.2.1/test/test_compel.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.0/test/test_embeddings_provider.py` & `compel-1.2.1/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.2.0/test/test_prompt_parser.py` & `compel-1.2.1/test/test_prompt_parser.py`

 * *Files identical despite different names*

