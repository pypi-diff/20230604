# Comparing `tmp/lycoris_lora-0.1.6.tar.gz` & `tmp/lycoris_lora-0.1.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-0.1.6.tar", last modified: Sun Jun  4 13:39:16 2023, max compression
+gzip compressed data, was "lycoris_lora-0.1.6.dev1.tar", last modified: Sun Apr 16 15:51:22 2023, max compression
```

## Comparing `lycoris_lora-0.1.6.tar` & `lycoris_lora-0.1.6.dev1.tar`

### file list

```diff
@@ -1,24 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 13:39:16.877785 lycoris_lora-0.1.6/
--rw-rw-rw-   0        0        0    11545 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/LICENSE.md
--rw-rw-rw-   0        0        0      348 2023-06-04 13:39:16.876787 lycoris_lora-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     7396 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 13:39:16.855977 lycoris_lora-0.1.6/lycoris/
--rw-rw-rw-   0        0        0      113 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/lycoris/__init__.py
--rw-rw-rw-   0        0        0     6222 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/lycoris/dylora.py
--rw-rw-rw-   0        0        0     2103 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/lycoris/ia3.py
--rw-rw-rw-   0        0        0    21720 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/lycoris/kohya.py
--rw-rw-rw-   0        0        0    48868 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/lycoris/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/lycoris/kohya_utils.py
--rw-rw-rw-   0        0        0     3178 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/lycoris/locon.py
--rw-rw-rw-   0        0        0     7657 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/lycoris/loha.py
--rw-rw-rw-   0        0        0     8974 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/lycoris/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-04 13:36:43.000000 lycoris_lora-0.1.6/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:39:16.875779 lycoris_lora-0.1.6/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      348 2023-06-04 13:39:16.000000 lycoris_lora-0.1.6/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-06-04 13:39:16.000000 lycoris_lora-0.1.6/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:39:16.000000 lycoris_lora-0.1.6/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-04 13:39:16.000000 lycoris_lora-0.1.6/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-06-04 13:39:16.000000 lycoris_lora-0.1.6/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-04 13:39:16.000000 lycoris_lora-0.1.6/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 13:39:16.877785 lycoris_lora-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      542 2023-06-04 13:38:57.000000 lycoris_lora-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.484260 lycoris_lora-0.1.6.dev1/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.6.dev1/Algo.md
+-rw-rw-rw-   0        0        0      552 2023-03-29 07:12:55.000000 lycoris_lora-0.1.6.dev1/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.6.dev1/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-04-16 15:51:22.484260 lycoris_lora-0.1.6.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     6498 2023-04-10 10:28:19.000000 lycoris_lora-0.1.6.dev1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.470741 lycoris_lora-0.1.6.dev1/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.6.dev1/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.6.dev1/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.6.dev1/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.6.dev1/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.6.dev1/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.6.dev1/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.6.dev1/experiments/time_test.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.475241 lycoris_lora-0.1.6.dev1/lycoris/
+-rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2514 2023-04-11 15:07:08.000000 lycoris_lora-0.1.6.dev1/lycoris/config.py
+-rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.6.dev1/lycoris/dylora.py
+-rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.6.dev1/lycoris/ia3.py
+-rw-rw-rw-   0        0        0    21664 2023-04-16 14:10:06.000000 lycoris_lora-0.1.6.dev1/lycoris/kohya.py
+-rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.6.dev1/lycoris/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/lycoris/kohya_utils.py
+-rw-rw-rw-   0        0        0     3178 2023-04-07 16:38:33.000000 lycoris_lora-0.1.6.dev1/lycoris/locon.py
+-rw-rw-rw-   0        0        0     7657 2023-04-07 16:38:27.000000 lycoris_lora-0.1.6.dev1/lycoris/loha.py
+-rw-rw-rw-   0        0        0     8974 2023-04-08 05:53:19.000000 lycoris_lora-0.1.6.dev1/lycoris/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-04-10 16:04:23.000000 lycoris_lora-0.1.6.dev1/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.483260 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 15:51:22.484260 lycoris_lora-0.1.6.dev1/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-04-16 15:51:09.000000 lycoris_lora-0.1.6.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.483760 lycoris_lora-0.1.6.dev1/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.6.dev1/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-04-10 15:31:09.000000 lycoris_lora-0.1.6.dev1/tools/merge.py
```

### Comparing `lycoris_lora-0.1.6/LICENSE.md` & `lycoris_lora-0.1.6.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.6/README.md` & `lycoris_lora-0.1.6.dev1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -42,24 +42,14 @@
 ### LoKR
 * Basically same idea of LoHA, but use kronecker product
 * This algo is quite sensitive and you may need to tune the lr
 * This algo can learn both character and style, but since it is small (auto factor, full rank, 2.5MB), it is also hard to transfer.
 * This algo produce relatively small file(auto factor: 900~2500KB)
 * Use smaller factor will produce bigger file, you can tune it if you think 2.5MB full rank is not good enough.
 
-### DyLoRA
-* Ref [DyLoRA: Parameter Efficient Tuning of Pre-trained Models using Dynamic Search-Free Low Rank Adaptation](https://arxiv.org/pdf/2210.07558.pdf)
-* Basically a training trick of lora.
-* Every step, only update one row/col of LoRA weight.
-* When we want to update k row/col, we only use 0~k row/col to rebuild the weight (0<=k<=dim)
-* You can easily resize DyLoRA to target and get similar or even better result than LoRA trained at target dim. (And you don't need to train lot loras with different dim to check which is better)
-* You should use large dim with alpha=dim/4~dim (1 or dim is not very recommended)
-    * Example: dim=128, alpha=64
-* Since we only update 1 row/col each step, you will need more step to get reasonable result. If you want to train it with few steps, you may need to set block_size (update multiple row/col every step) to higer value (default=0)
-
 ---
 
 ## usage
 
 You can just use these training scripts.
 * [derrian-distro/LoRA_Easy_Training_Scripts](https://github.com/derrian-distro/LoRA_Easy_Training_Scripts)
 * [Linaqruf/kohya-trainer](https://github.com/Linaqruf/kohya-trainer)
```

### Comparing `lycoris_lora-0.1.6/lycoris/dylora.py` & `lycoris_lora-0.1.6.dev1/lycoris/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.6/lycoris/ia3.py` & `lycoris_lora-0.1.6.dev1/lycoris/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.6/lycoris/kohya.py` & `lycoris_lora-0.1.6.dev1/lycoris/kohya.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 from .lokr import LokrModule
 from .dylora import DyLoraModule
 
 
 def create_network(multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs):
     if network_dim is None:
         network_dim = 4                     # default
-    conv_dim = int(kwargs.get('conv_dim', network_dim) or network_dim)
-    conv_alpha = float(kwargs.get('conv_alpha', network_alpha) or network_alpha)
-    dropout = float(kwargs.get('dropout', 0.) or 0.)
-    algo = (kwargs.get('algo', 'lora') or 'lora').lower()
-    use_cp = (not kwargs.get('disable_conv_cp', True)
+    conv_dim = int(kwargs.get('conv_dim', network_dim))
+    conv_alpha = float(kwargs.get('conv_alpha', network_alpha))
+    dropout = float(kwargs.get('dropout', 0.))
+    algo = kwargs.get('algo', 'lora').lower()
+    use_cp = (not kwargs.get('disable_conv_cp', True) 
               or kwargs.get('use_conv_cp', False))
-    block_size = int(kwargs.get('block_size', 4) or 4)
+    block_size = int(kwargs.get('block_size', 4))
     network_module = {
         'lora': LoConModule,
         'locon': LoConModule,
         'loha': LohaModule,
         'ia3':  IA3Module,
         'lokr': LokrModule,
         'dylora': DyLoraModule,
@@ -535,8 +535,8 @@
                 metadata = {}
             model_hash, legacy_hash = precalculate_safetensors_hashes(state_dict, metadata)
             metadata["sshs_model_hash"] = model_hash
             metadata["sshs_legacy_hash"] = legacy_hash
 
             save_file(state_dict, file, metadata)
         else:
-            torch.save(state_dict, file)
+            torch.save(state_dict, file)
```

### Comparing `lycoris_lora-0.1.6/lycoris/kohya_model_utils.py` & `lycoris_lora-0.1.6.dev1/lycoris/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.6/lycoris/kohya_utils.py` & `lycoris_lora-0.1.6.dev1/lycoris/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.6/lycoris/locon.py` & `lycoris_lora-0.1.6.dev1/lycoris/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.6/lycoris/loha.py` & `lycoris_lora-0.1.6.dev1/lycoris/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.6/lycoris/lokr.py` & `lycoris_lora-0.1.6.dev1/lycoris/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.6/lycoris/utils.py` & `lycoris_lora-0.1.6.dev1/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.6/setup.py` & `lycoris_lora-0.1.6.dev1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='0.1.6',
+    version='0.1.6.dev1',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

