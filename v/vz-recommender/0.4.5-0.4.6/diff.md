# Comparing `tmp/vz-recommender-0.4.5.tar.gz` & `tmp/vz-recommender-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vz-recommender-0.4.5.tar", last modified: Wed May 10 01:58:12 2023, max compression
+gzip compressed data, was "vz-recommender-0.4.6.tar", last modified: Sun Jun  4 05:30:18 2023, max compression
```

## Comparing `vz-recommender-0.4.5.tar` & `vz-recommender-0.4.6.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.095938 vz-recommender-0.4.5/
--rw-r--r--   0 tangca     (502) staff       (20)      567 2022-11-30 18:56:25.000000 vz-recommender-0.4.5/LICENSE
--rw-r--r--   0 tangca     (502) staff       (20)     2535 2023-05-10 01:58:12.096211 vz-recommender-0.4.5/PKG-INFO
--rw-r--r--   0 tangca     (502) staff       (20)     2151 2023-01-24 15:48:11.000000 vz-recommender-0.4.5/README.md
--rw-r--r--   0 tangca     (502) staff       (20)      103 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/pyproject.toml
--rw-r--r--   0 tangca     (502) staff       (20)      508 2023-05-10 01:58:12.097148 vz-recommender-0.4.5/setup.cfg
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.053831 vz-recommender-0.4.5/src/
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.075709 vz-recommender-0.4.5/src/vz_recommender/
--rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/src/vz_recommender/__init__.py
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.091503 vz-recommender-0.4.5/src/vz_recommender/models/
--rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/src/vz_recommender/models/__init__.py
--rw-r--r--   0 tangca     (502) staff       (20)     4744 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/src/vz_recommender/models/ae.py
--rw-r--r--   0 tangca     (502) staff       (20)    48448 2023-05-09 17:30:48.000000 vz-recommender-0.4.5/src/vz_recommender/models/bst.py
--rw-r--r--   0 tangca     (502) staff       (20)    11865 2023-01-17 15:09:38.000000 vz-recommender-0.4.5/src/vz_recommender/models/context.py
--rw-r--r--   0 tangca     (502) staff       (20)     4418 2023-01-24 17:20:36.000000 vz-recommender-0.4.5/src/vz_recommender/models/mmoe.py
--rw-r--r--   0 tangca     (502) staff       (20)    42778 2023-05-04 20:55:32.000000 vz-recommender-0.4.5/src/vz_recommender/models/moe.py
--rw-r--r--   0 tangca     (502) staff       (20)    13003 2023-01-10 16:37:33.000000 vz-recommender-0.4.5/src/vz_recommender/models/multitask.py
--rw-r--r--   0 tangca     (502) staff       (20)    34073 2023-05-09 17:30:35.000000 vz-recommender-0.4.5/src/vz_recommender/models/pars.py
--rw-r--r--   0 tangca     (502) staff       (20)    39847 2023-05-09 17:30:35.000000 vz-recommender-0.4.5/src/vz_recommender/models/transformer.py
--rw-r--r--   0 tangca     (502) staff       (20)     3988 2023-01-17 15:09:38.000000 vz-recommender-0.4.5/src/vz_recommender/models/txt.py
--rw-r--r--   0 tangca     (502) staff       (20)    10192 2023-03-24 14:13:49.000000 vz-recommender-0.4.5/src/vz_recommender/models/utils.py
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.095262 vz-recommender-0.4.5/src/vz_recommender/utils/
--rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/src/vz_recommender/utils/__init__.py
--rw-r--r--   0 tangca     (502) staff       (20)    10835 2023-03-24 14:13:49.000000 vz-recommender-0.4.5/src/vz_recommender/utils/callbacks_base.py
--rw-r--r--   0 tangca     (502) staff       (20)     4517 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/src/vz_recommender/utils/loggers_base.py
--rw-r--r--   0 tangca     (502) staff       (20)     5763 2023-03-24 14:13:49.000000 vz-recommender-0.4.5/src/vz_recommender/utils/utils.py
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.078982 vz-recommender-0.4.5/src/vz_recommender.egg-info/
--rw-r--r--   0 tangca     (502) staff       (20)     2535 2023-05-10 01:58:12.000000 vz-recommender-0.4.5/src/vz_recommender.egg-info/PKG-INFO
--rw-r--r--   0 tangca     (502) staff       (20)      785 2023-05-10 01:58:12.000000 vz-recommender-0.4.5/src/vz_recommender.egg-info/SOURCES.txt
--rw-r--r--   0 tangca     (502) staff       (20)        1 2023-05-10 01:58:12.000000 vz-recommender-0.4.5/src/vz_recommender.egg-info/dependency_links.txt
--rw-r--r--   0 tangca     (502) staff       (20)       15 2023-05-10 01:58:12.000000 vz-recommender-0.4.5/src/vz_recommender.egg-info/top_level.txt
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-06-04 05:30:18.413997 vz-recommender-0.4.6/
+-rw-r--r--   0 tangca     (502) staff       (20)      567 2022-11-30 18:56:25.000000 vz-recommender-0.4.6/LICENSE
+-rw-r--r--   0 tangca     (502) staff       (20)     2535 2023-06-04 05:30:18.414209 vz-recommender-0.4.6/PKG-INFO
+-rw-r--r--   0 tangca     (502) staff       (20)     2151 2023-01-24 15:48:11.000000 vz-recommender-0.4.6/README.md
+-rw-r--r--   0 tangca     (502) staff       (20)      103 2022-11-30 18:56:26.000000 vz-recommender-0.4.6/pyproject.toml
+-rw-r--r--   0 tangca     (502) staff       (20)      508 2023-06-04 05:30:18.431588 vz-recommender-0.4.6/setup.cfg
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-06-04 05:30:18.390399 vz-recommender-0.4.6/src/
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-06-04 05:30:18.396047 vz-recommender-0.4.6/src/vz_recommender/
+-rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.6/src/vz_recommender/__init__.py
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-06-04 05:30:18.409601 vz-recommender-0.4.6/src/vz_recommender/models/
+-rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.6/src/vz_recommender/models/__init__.py
+-rw-r--r--   0 tangca     (502) staff       (20)     4744 2022-11-30 18:56:26.000000 vz-recommender-0.4.6/src/vz_recommender/models/ae.py
+-rw-r--r--   0 tangca     (502) staff       (20)    48461 2023-05-31 17:48:35.000000 vz-recommender-0.4.6/src/vz_recommender/models/bst.py
+-rw-r--r--   0 tangca     (502) staff       (20)    11865 2023-01-17 15:09:38.000000 vz-recommender-0.4.6/src/vz_recommender/models/context.py
+-rw-r--r--   0 tangca     (502) staff       (20)     1580 2023-05-26 15:34:08.000000 vz-recommender-0.4.6/src/vz_recommender/models/encoders.py
+-rw-r--r--   0 tangca     (502) staff       (20)    41146 2023-06-04 05:28:21.000000 vz-recommender-0.4.6/src/vz_recommender/models/grec.py
+-rw-r--r--   0 tangca     (502) staff       (20)     4418 2023-01-24 17:20:36.000000 vz-recommender-0.4.6/src/vz_recommender/models/mmoe.py
+-rw-r--r--   0 tangca     (502) staff       (20)    43383 2023-06-01 17:56:16.000000 vz-recommender-0.4.6/src/vz_recommender/models/moe.py
+-rw-r--r--   0 tangca     (502) staff       (20)    13003 2023-01-10 16:37:33.000000 vz-recommender-0.4.6/src/vz_recommender/models/multitask.py
+-rw-r--r--   0 tangca     (502) staff       (20)    28597 2023-06-01 17:56:16.000000 vz-recommender-0.4.6/src/vz_recommender/models/transformer.py
+-rw-r--r--   0 tangca     (502) staff       (20)     3988 2023-01-17 15:09:38.000000 vz-recommender-0.4.6/src/vz_recommender/models/txt.py
+-rw-r--r--   0 tangca     (502) staff       (20)    10192 2023-03-24 14:13:49.000000 vz-recommender-0.4.6/src/vz_recommender/models/utils.py
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-06-04 05:30:18.413289 vz-recommender-0.4.6/src/vz_recommender/utils/
+-rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.6/src/vz_recommender/utils/__init__.py
+-rw-r--r--   0 tangca     (502) staff       (20)    10835 2023-03-24 14:13:49.000000 vz-recommender-0.4.6/src/vz_recommender/utils/callbacks_base.py
+-rw-r--r--   0 tangca     (502) staff       (20)     4517 2022-11-30 18:56:26.000000 vz-recommender-0.4.6/src/vz_recommender/utils/loggers_base.py
+-rw-r--r--   0 tangca     (502) staff       (20)     5799 2023-05-31 17:48:35.000000 vz-recommender-0.4.6/src/vz_recommender/utils/utils.py
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-06-04 05:30:18.398825 vz-recommender-0.4.6/src/vz_recommender.egg-info/
+-rw-r--r--   0 tangca     (502) staff       (20)     2535 2023-06-04 05:30:18.000000 vz-recommender-0.4.6/src/vz_recommender.egg-info/PKG-INFO
+-rw-r--r--   0 tangca     (502) staff       (20)      823 2023-06-04 05:30:18.000000 vz-recommender-0.4.6/src/vz_recommender.egg-info/SOURCES.txt
+-rw-r--r--   0 tangca     (502) staff       (20)        1 2023-06-04 05:30:18.000000 vz-recommender-0.4.6/src/vz_recommender.egg-info/dependency_links.txt
+-rw-r--r--   0 tangca     (502) staff       (20)       15 2023-06-04 05:30:18.000000 vz-recommender-0.4.6/src/vz_recommender.egg-info/top_level.txt
```

### Comparing `vz-recommender-0.4.5/LICENSE` & `vz-recommender-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.5/PKG-INFO` & `vz-recommender-0.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vz-recommender
-Version: 0.4.5
+Version: 0.4.6
 Summary: vz recommender package
 Author: lu
 Author-email: luyang.wang@verizon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `vz-recommender-0.4.5/README.md` & `vz-recommender-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.5/src/vz_recommender/models/ae.py` & `vz-recommender-0.4.6/src/vz_recommender/models/ae.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.5/src/vz_recommender/models/bst.py` & `vz-recommender-0.4.6/src/vz_recommender/models/bst.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import *
 import torch
 import abc
 from torch import nn
 from transformers import AutoModel, DistilBertModel
 from .context import ContextHead, ContextTransformerAndWide
-from .transformer import TransformerAEP, ParallelTransformerBlock, ParallelTransformerAEP, TransformerAEPCat
+from .transformer import TransformerAEP, ParallelTransformerBlock, ParallelTransformerAEP, ParallelTransformerAEP2S
 from .mmoe import MMoE
 from .moe import MoE
 from transformers import DistilBertConfig, DistilBertModel
 from .utils import MeanMaxPooling
 from .mmoe import MMoE
 from .moe import ExpertLayer, MoEFFLayer
 
@@ -91,15 +91,15 @@
         self.svc_embedding = nn.Embedding(svc_dim, svc_embed_dim)
         self.new_svc_embedding = nn.Embedding(new_svc_dim, new_svc_embed_dim)
         self.svc_desc_dly_embedding = nn.Embedding(svc_desc_dly_dim, svc_desc_dly_embed_dim)
         self.mm_pooling = MeanMaxPooling()
 
         self.page_embedding = nn.Embedding(page_dim, seq_embed_dim)
         self.item_embedding = nn.Embedding(item_dim, seq_embed_dim)
-        self.sequence_transformer = ParallelTransformerAEP(
+        self.sequence_transformer = ParallelTransformerAEP2S(
             page_embedding=self.page_embedding,
             item_embedding=self.item_embedding,
             dim=seq_embed_dim,
             dim_head=seq_embed_dim,
             heads=sequence_transformer_kwargs.get("seq_num_heads"),
             num_layers=sequence_transformer_kwargs.get("seq_num_layers"),
         )
@@ -217,24 +217,24 @@
         self.svc_embedding = nn.Embedding(svc_dim, svc_embed_dim)
         self.new_svc_embedding = nn.Embedding(new_svc_dim, new_svc_embed_dim)
         self.svc_desc_dly_embedding = nn.Embedding(svc_desc_dly_dim, svc_desc_dly_embed_dim)
         self.mm_pooling = MeanMaxPooling()
 
         self.page_embedding = nn.Embedding(page_dim, seq_embed_dim)
         self.item_embedding = nn.Embedding(item_dim, seq_embed_dim)
-        self.sequence_transformer = ParallelTransformerAEP(
+        self.sequence_transformer = ParallelTransformerAEP2S(
             page_embedding=self.page_embedding,
             item_embedding=self.item_embedding,
             dim=seq_embed_dim,
             dim_head=seq_embed_dim,
             heads=sequence_transformer_kwargs.get("seq_num_heads"),
             num_layers=sequence_transformer_kwargs.get("seq_num_layers"),
         )
 
-        self.nlp_encoder = DistilBertModel.from_pretrained(nlp_encoder_path)
+        self.nlp_encoder = AutoModel.from_pretrained(nlp_encoder_path)
         self.nlp_dense_0 = torch.nn.Linear(
             in_features=nlp_dim,
             out_features=seq_embed_dim
         )
         self.nlp_act = nn.LeakyReLU(0.2)
 
         if user_num_wide:
@@ -302,15 +302,15 @@
         new_svc_out = self.new_svc_embedding(new_svc_in.long())
         new_svc_out = self.mm_pooling(new_svc_out)
         svc_desc_dly_out = self.svc_desc_dly_embedding(svc_desc_dly_in.long())
         svc_desc_dly_out = self.mm_pooling(svc_desc_dly_out)
 
         aep_seq_out = self.sequence_transformer(page_in=page_in, item_in=item_in, vl_in=vl_in)
 
-        nlp_out = self.nlp_encoder(**nlp_in).last_hidden_state[:, 0, :].to(dtype=torch.float32)
+        nlp_out = self.nlp_encoder(**nlp_in).pooler_output.to(dtype=torch.float32)
         nlp_out = self.nlp_dense_0(nlp_out)
         nlp_out = self.nlp_act(nlp_out)
 
         user_ctx_out = self.user_context_head(deep_in=user_deep_in, wide_in=user_wide_in)
         user_out = torch.stack([nlp_out, aep_seq_out, user_ctx_out, svc_out, new_svc_out, svc_desc_dly_out], dim=1)
         user_out = self.user_att_pooling(user_out)
         user_out = torch.concat(user_out.unbind(1), dim=1)
@@ -347,21 +347,21 @@
         # user layers
         self.svc_embedding = nn.Embedding(svc_dim, svc_embed_dim)
         self.new_svc_embedding = nn.Embedding(new_svc_dim, new_svc_embed_dim)
         self.mm_pooling = MeanMaxPooling()
 
         self.page_embedding = nn.Embedding(page_dim, page_embed_dim)
         self.item_embedding = nn.Embedding(item_dim, item_embed_dim)
-        self.sequence_transformer = TransformerAEPCat(
-            page_embedding=self.page_embedding,
-            item_embedding=self.item_embedding,
-            seq_embed_dim=seq_embed_dim,
-            seq_hidden_size=seq_hidden_size,
-            **sequence_transformer_kwargs,
-        )
+#         self.sequence_transformer = ParallelTransformerAEP2S(
+#             page_embedding=self.page_embedding,
+#             item_embedding=self.item_embedding,
+#             seq_embed_dim=seq_embed_dim,
+#             seq_hidden_size=seq_hidden_size,
+#             **sequence_transformer_kwargs,
+#         )
 
         self.nlp_encoder = DistilBertModel.from_pretrained(nlp_encoder_path)
         self.search_nlp_dense_0 = torch.nn.Linear(
             in_features=nlp_dim,
             out_features=seq_embed_dim * 2
         )
         self.search_nlp_dense_1 = torch.nn.Linear(
```

### Comparing `vz-recommender-0.4.5/src/vz_recommender/models/context.py` & `vz-recommender-0.4.6/src/vz_recommender/models/context.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.5/src/vz_recommender/models/mmoe.py` & `vz-recommender-0.4.6/src/vz_recommender/models/mmoe.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.5/src/vz_recommender/models/moe.py` & `vz-recommender-0.4.6/src/vz_recommender/models/moe.py`

 * *Files 4% similar despite different names*

```diff
@@ -638,30 +638,36 @@
         r"""
         `bitsandbytes` `Linear8bitLt` layers does not support manual casting Therefore we need to check if they are an
         instance of the `Linear8bitLt` class by checking special attributes.
         """
         if not (hasattr(self.classifier, "SCB") or hasattr(self.classifier, "CB")):
             self.classifier = self.classifier.to(self.dtype)
 
-    def forward(self, hidden_states: torch.Tensor) -> Tuple:
+    def forward(self, hidden_states, task_state=None) -> Tuple:
         r"""
         Generic forward function for every Router class. Each Router expects to have the same input hidden states
         (`hidden_states`) corresponding to the hidden states for each token, the `expert_capacity` corresponding to the
         number of tokens the Router will send to each expert, some Routers can send up to few tokens to each expert.
         Each Router works as the following: it expects the hidden states for each token, gets the `router_probs` and
         `router_logits` from the `router_weights`. This will assign for each token, the raw probability to be assigned
         to an expert. Then each Router class will have to define its own `_compute_routing_instructions`.
         Args:
             hidden_states (`torch.Tensor`) :
                 [num_groups, tokens_per_group, hidden_dim] inputs to send to experts.
         Returns:
             Tuple[`torch.Tensor`, `torch.Tensor`, `torch.Tensor`] Tuple containing the expert index, the router probs
             and the router logits. The router probabilities and logits are required to compute the loss.
         """
-        router_probs, router_logits = self._compute_router_probabilities(hidden_states)
+        if task_state is None:
+            router_probs, router_logits = self._compute_router_probabilities(hidden_states)
+        else:
+            router_probs, router_logits = self._compute_router_probabilities(task_state)
+            num_token = hidden_states.shape[1]
+            router_probs = torch.cat([router_probs]*num_token, dim=1)
+            router_logits = torch.cat([router_logits]*num_token, dim=1)
 
         expert_index = torch.argmax(router_probs, dim=-1)
         expert_index = torch.nn.functional.one_hot(expert_index, num_classes=self.num_experts)
 
         # Mask tokens outside expert capacity. Sum over each sequence
         token_priority = torch.cumsum(expert_index, dim=-2)
         # mask if the token routed to to the expert will overflow
@@ -722,19 +728,20 @@
 
     def __init__(self, dim, num_experts, expert_capacity, hidden_size, expert_class, router_bias=True,
                  router_jitter_noise=0.1,
                  router_ignore_padding_tokens=False, router_dtype="float32", num_K=1):
         super().__init__()
         # Step 1: Get the correct router according to its class
         self.num_K = num_K
+        self.num_experts = num_experts
         self.router = TopKRouter(num_experts, expert_capacity, hidden_size, router_bias, router_jitter_noise,
                                  router_ignore_padding_tokens, router_dtype, num_K)
         # Step 2: Get the top K experts
         self.experts = nn.ModuleList([
-            expert_class(dim, hidden_size) for _ in range(4)
+            expert_class(dim, hidden_size) for _ in range(self.num_experts)
         ])
 
     def forward(self, hidden_states, task_state=None):
         r"""
         Hold on, this will be slightly tricky to understand In the correct order, a MoE layer does the following:
         1- Gets the `router_mask` from the router. The shape of the mask is `(batch_size, sequence_length, num_expert)`. 
         The probabilities are needed in the computation of the hidden states : they are broadcasted to the hidden states 
@@ -748,15 +755,15 @@
 
         # The routers introduced might not always map all the tokens, to a router, which means that some hidden states
         # can be unchanged from one layer to another. That is why the hidden states are cloned before updating only the seleced ones.
 
         next_states = [hidden_states.clone() for _ in range(self.num_K)]
 
         for k in range(self.num_K):
-            token_indices_k = torch.nn.functional.one_hot(expert_index_list[:, :, k], num_classes=4).bool()
+            token_indices_k = torch.nn.functional.one_hot(expert_index_list[:, :, k], num_classes=self.num_experts).bool()
             token_indices_k = token_indices_k * expert_capacity_mask
             for idx, expert in enumerate(self.experts):
                 token_indices = token_indices_k[:, :, idx]
                 p = router_probs_top_k[:, :, k][token_indices].unsqueeze(1)
                 next_states[k][token_indices] = expert(hidden_states[token_indices]) * p
 
         hidden_states = torch.stack(next_states, dim=0).sum(dim=0)
@@ -776,24 +783,21 @@
         # Step 2: Get the experts
         self.experts = nn.ModuleDict()
         for idx in range(num_experts):
             self.experts[f"expert_{idx}"] = expert_class(dim, hidden_size)
 
     def forward(self, hidden_states, task_state=None):
         r"""
-        Hold on, this will be slightly tricky to understand In the correct order, a MoE layer does the following:
-        1- Gets the `router_mask` from the router. The shape of the mask is `(batch_size, sequence_length, num_expert)`
-        and corresponds to the argmax of the `router_probs`. The probabilities are needed in the computation of the
-        hidden states : they are broadcasted to the hidden states values (can be interpreted as a scaling factor).
-        2- Dispatch the tokens to its associated experts. We do a classic for loop over the experts and assign for each
-        expert the corresponding hidden states.
+        1 - It retrieves the 'router_mask' from the router, which has a shape of (batch_size, sequence_length, num_experts). This mask represents the index of the highest probability assignment for each token in the input sequence, according to the 'router_probs'. These probabilities are used as weights to compute the hidden states for each expert.
+        2 -It dispatches the input tokens to their respective experts by iterating through the list of experts and assigning each one its corresponding hidden state. Each expert processes the tokens assigned to it independently.
+        3 - After all experts have processed the tokens, the outputs from each expert are combined to produce the final output for the layer. This combination can be done either by taking a weighted sum.
         """
         # Step 1: Get the router_mask from the router as wel as the probabilities
-        router_state = hidden_states if task_state is None else task_state
-        router_mask, router_probs, router_logits = self.router(router_state)
+#         router_state = hidden_states if task_state is None else task_state
+        router_mask, router_probs, router_logits = self.router(hidden_states, task_state)
         expert_index = torch.argmax(router_mask, dim=-1)
 
         # The routers introduced might not always map all the tokens, to a router, which means that some hidden states
         # can be unchanged from one layer to another. That is why the hidden states are cloned before updating only the seleced ones.
 
         next_states = hidden_states.clone()
         for idx, expert in enumerate(self.experts.values()):
@@ -814,19 +818,20 @@
             configuration. Check out the [`~PreTrainedModel.from_pretrained`] method to load the model weights.
         is_sparse (`bool`):
             Whether the MLP layer is a `Sparse` layer (contains a Mixture of Experts) or not
     """
 
     def __init__(self, dim, num_experts, expert_capacity, hidden_size, expert_class, dropout_rate=0, 
                  router_bias=True, router_jitter_noise=0.1, router_ignore_padding_tokens=False, 
-                 router_z_loss_coef=0.001, router_aux_loss_coef=0.001, router_dtype="float32", num_K=1):
+                 router_dtype="float32", num_K=1):
         super().__init__()
         self.mlp = SparseMoELayerTopK(dim, num_experts, expert_capacity, hidden_size, expert_class,
-                                  router_bias=True, router_jitter_noise=0.1, 
-                                  router_ignore_padding_tokens=False, router_dtype="float32", num_K=num_K)
+                                      router_bias=router_bias, router_jitter_noise=router_jitter_noise,
+                                      router_ignore_padding_tokens=router_ignore_padding_tokens,
+                                      router_dtype=router_dtype, num_K=num_K)
         self.layer_norm = MoELayerNorm(hidden_size)
         self.dropout = nn.Dropout(dropout_rate)
 
     def forward(self, hidden_states, task_state=None, output_router_logits=True):
         forwarded_states = self.layer_norm(hidden_states)
         forwarded_states = self.mlp(forwarded_states, task_state)
```

### Comparing `vz-recommender-0.4.5/src/vz_recommender/models/multitask.py` & `vz-recommender-0.4.6/src/vz_recommender/models/multitask.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.5/src/vz_recommender/models/pars.py` & `vz-recommender-0.4.6/src/vz_recommender/models/grec.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 
 import torch
 from torch import nn
 from transformers import AutoModel, DistilBertConfig, DistilBertModel
 
 from .context import ContextHead, ContextTransformerAndWide
 from .moe import MOELayer, Top2Gate, ExpertLayer, MoEFFLayer, MoEFFLayerTopK
-from .transformer import (ParallelTransformerAEP, ParallelTransformerAEP2, ParallelTransformerAEP3, ParallelTransformerBlock, TransformerAEP,
+from .transformer import (ParallelTransformerAEP, ParallelTransformerBlock, TransformerAEP, ParallelTransformerAEP2S,
                           TransformerHistory)
 from .utils import MeanMaxPooling, LayerNorm, AutomaticWeightedLoss
 
     
-class PaRS(nn.Module):
-    def __init__(self, deep_dims, page_dim, seq_dim, item_meta_dim, page_embed_dim, seq_embed_dim, item_embed_dim, item_meta_embed_dim, item_pre_embed_dim, deep_embed_dims, wad_embed_dim, nlp_embed_dim, seq_hidden_size, nlp_encoder_path, task_type_dim, task_type_embed_dim, task_out_dims,
-                 num_wide=0, num_shared=0, nlp_dim=0, item_freeze=None, item_pre_freeze=None, nlp_freeze=None, context_head_kwargs=None, sequence_transformer_kwargs=None,
+class GRec(nn.Module):
+    def __init__(self, deep_dims, page_dim, seq_dim, item_meta_dim, page_embed_dim, seq_embed_dim, item_embed_dim, item_meta_embed_dim, item_pre_embed_dim, deep_embed_dims, wad_embed_dim, nlp_embed_dim, seq_hidden_size, nlp_encoder_path, task_type_dims, task_type_embed_dim, task_out_dims, num_task,
+                 num_wide=0, num_meta_wide=0, num_shared=0, nlp_dim=0, item_freeze=None, item_pre_freeze=None, nlp_freeze=None, context_head_kwargs=None, sequence_transformer_kwargs=None,
                  page_embedding_weight=None, item_embedding_weight=None, item_meta_embedding_weight=None, item_pre_embedding_weight=None, shared_embeddings_weight=None, moe_kwargs=None):
         super().__init__()
-        self.nlp_encoder = DistilBertModel.from_pretrained(nlp_encoder_path)
+        #self.nlp_encoder = DistilBertModel.from_pretrained(nlp_encoder_path)
+        self.nlp_encoder = AutoModel.from_pretrained(nlp_encoder_path)
         context_head_kwargs = context_head_kwargs if context_head_kwargs else {}
         sequence_transformer_kwargs = sequence_transformer_kwargs if sequence_transformer_kwargs else {}
         
         if page_embedding_weight is None:
             print("not use pretrained embedding")
             self.page_embedding = nn.Embedding(page_dim, page_embed_dim)
         else:
@@ -51,35 +52,41 @@
         if item_pre_freeze:
             self.item_pre_embedding.weight.requires_grad = False
             
         if nlp_freeze:
             for param in self.nlp_encoder.parameters():
                 param.requires_grad = False
          
-#         self.combined_dim = nlp_embed_dim + wad_embed_dim + seq_embed_dim + item_embed_dim
+#         self.combined_dim = nlp_embed_dim + wad_embed_dim + seq_embed_dim + seq_embed_dim
         self.combined_dim = nlp_embed_dim + wad_embed_dim + seq_embed_dim + seq_embed_dim + seq_embed_dim
-        self.task_embedding = nn.Embedding(task_type_dim, seq_embed_dim)
+#         self.mm_pooling = MeanMaxPooling()
+        self.task_embedding = nn.ModuleList([
+            nn.Embedding(task_type_dim, task_type_embed_dim)
+            for task_type_dim in task_type_dims
+        ])
+#         print(task_type_dims)
+#         print(self.task_embedding)
+#         self.task_embedding = nn.Embedding(task_type_dims, seq_embed_dim)
         self.context_head = ContextHead(
             deep_dims=deep_dims,
             num_wide=num_wide,
             item_embedding=self.item_embedding,
             shared_embeddings_weight=shared_embeddings_weight,
             wad_embed_dim=wad_embed_dim,
             deep_embed_dims=deep_embed_dims
         )
-        self.sequence_transformer = ParallelTransformerAEP2(
+        self.sequence_transformer = ParallelTransformerAEP(
             page_embedding=self.page_embedding,
             item_embedding=self.item_embedding,
             item_meta_embedding=self.item_meta_embedding,
             item_pre_embedding=self.item_pre_embedding,
             dim=seq_embed_dim,
             dim_head=seq_embed_dim,
-            heads=sequence_transformer_kwargs.get("seq_num_heads"),
-            num_layers=sequence_transformer_kwargs.get("seq_num_layers"),
-            moe_kwargs=moe_kwargs
+            moe_kwargs=moe_kwargs,
+            **sequence_transformer_kwargs
         )
         self.att_pooling = ParallelTransformerBlock(
             dim=256, dim_head=256, heads=1
         )
         self.seq_dense = torch.nn.Linear(
             in_features=seq_embed_dim,
             out_features=seq_embed_dim
@@ -112,15 +119,15 @@
         )
         self.tasks_dense2 = nn.Linear(
             self.combined_dim // 2, 
             task_out_dims[0]
         )
         self.tasks_act1 = self.tasks_act2 = nn.LeakyReLU(0.2)
         self.seq_dim = seq_dim
-        self.task_type_dim = task_type_dim
+        self.task_type_dim = num_task
 #         self.awl = AutomaticWeightedLoss(task_type_dim)
 
 #     def split_task(self, task_type_dim, task_in, combined_out):
 #         task_indices = []
 #         task_outs = []
 #         task_user_outs = []
 #         for i in range(task_type_dim):
@@ -147,51 +154,58 @@
             task_user_out = self.tasks_act1(task_out)
             task_out = self.tasks_dense2(task_user_out)
             task_indices.append(task_indice)
             task_user_outs.append(task_user_out)
             task_outs.append(task_out)
         return task_indices, task_outs, task_user_outs
         
-    def forward(self, deep_in, page_in, item_in, item_meta_in, vl_in, task_in, current_in, current_meta_in, wide_in=None, input_ids=None, attention_mask=None, shared_in=None):
+    def forward(self, deep_in, page_in, item_in, vl_in, tasks_in, current_in, current_meta_in, item_meta_in=None, page_meta_in=None, item_meta_wide_in=None, page_meta_wide_in=None, wide_in=None, input_ids=None, attention_mask=None, shared_in=None):
         """
         Args:
             deep_in: list, a list of Tensor of shape [batch_size, deep_dims].
             seq_in: Tensor, shape [batch_size, seq_len].
             vl_in: Tensor, shape [batch_size].
             wide_in: list, a list of Tensor of shape [batch_size, num_wide].
             shared_in: list, a list of Tensor of shape [batch_size, num_shared] (default=None).
             search_ids: tensor, Tensor of shape [batch_size, sentence_length] (default=None).
             att_mask: tensor, Tensor of shape [batch_size, sentence_length] (default=None).
 
         Return:
             out: Tensor, shape [batch_size, seq_dim].
             user_out: Tensor, shape [batch_size, seq_embed_dim].
         """
-        search_out = self.nlp_encoder(input_ids=input_ids, attention_mask=attention_mask).last_hidden_state[:,0,:].to(dtype=torch.float32)
+        search_out = self.nlp_encoder(input_ids=input_ids, attention_mask=attention_mask).pooler_output.to(dtype=torch.float32)
+#         search_out = self.nlp_encoder(input_ids=input_ids, attention_mask=attention_mask).last_hidden_state[:,0,:].to(dtype=torch.float32)
         search_out = self.nlp_dense(search_out)
         ctx_out = self.context_head(deep_in=deep_in, wide_in=wide_in, shared_in=shared_in)
-        seq_out = self.sequence_transformer(page_in=page_in, item_in=item_in, item_meta_in=item_meta_in, vl_in=vl_in)
+        seq_out = self.sequence_transformer(page_in=page_in, item_in=item_in, item_meta_in=item_meta_in, page_meta_in=page_meta_in, item_meta_wide_in=item_meta_wide_in, page_meta_wide_in=page_meta_wide_in, vl_in=vl_in)
         seq_out = self.seq_dense(seq_out)
         current_item_out = self.item_embedding(current_in)
         current_meta_out = self.item_meta_embedding(current_meta_in)
         current_pre_out = self.item_pre_embedding(current_in)
         current_out = torch.cat((current_item_out, current_meta_out, current_pre_out), 1)
-#         task_out = self.task_embedding(task_in)[:, None, :]
+
+#         tasks_out_list = [self.task_embedding[i](task_in).unsqueeze(1)
+#                            for i, task_in in enumerate(tasks_in)]
+#         task_out = torch.cat(tasks_out_list, dim=2)
 #         outs = torch.cat((seq_out[:, None, :], ctx_out[:, None, :], search_out[:, None, :], current_out[:, None, :]), dim=1)
 #         outs = self.att_pooling(outs)
-#         task_out = torch.cat([task_out] * 4, dim=1)
 #         outs, aux_loss = self.moe(outs, task_out)
         
-        task_out = self.task_embedding(task_in)
+        
+        tasks_out_list = [self.task_embedding[i](task_in).unsqueeze(1)
+                           for i, task_in in enumerate(tasks_in)]
+        task_out = torch.cat(tasks_out_list, dim=2).squeeze(1)
+#         task_out = self.mm_pooling(tasks_out)
         outs = torch.cat((seq_out[:, None, :], ctx_out[:, None, :], search_out[:, None, :], current_out[:, None, :], task_out[:, None, :]), dim=1)
         outs = self.att_pooling(outs)
         outs, aux_loss = self.moe(outs)
         
         outs = outs.reshape(-1, self.combined_dim)
-        task_indices, task_outs, task_user_outs = self.split_task(self.task_type_dim, task_in, outs)
+        task_indices, task_outs, task_user_outs = self.split_task(self.task_type_dim, tasks_in[0], outs)
         return (tuple(task_indices), tuple(task_outs), aux_loss)
 
 
 class PaRSAudienceTT(nn.Module):
     def __init__(self, user_deep_dims, user_deep_embed_dims, user_num_wide, user_wad_embed_dim,
                  offer_deep_dims, offer_deep_embed_dims, offer_num_wide, offer_wad_embed_dim,
                  svc_dim, svc_embed_dim, new_svc_dim, new_svc_embed_dim, page_dim, item_dim,
@@ -396,24 +410,25 @@
         # user layers
         self.svc_embedding = nn.Embedding(svc_dim, svc_embed_dim)
         self.new_svc_embedding = nn.Embedding(new_svc_dim, new_svc_embed_dim)
         self.mm_pooling = MeanMaxPooling()
 
         self.page_embedding = nn.Embedding(page_dim, seq_embed_dim)
         self.item_embedding = nn.Embedding(item_dim, seq_embed_dim)
-        self.sequence_transformer = ParallelTransformerAEP(
+        self.sequence_transformer = ParallelTransformerAEP2S(
             page_embedding=self.page_embedding,
             item_embedding=self.item_embedding,
             dim=seq_embed_dim,
             dim_head=seq_embed_dim,
             heads=sequence_transformer_kwargs.get("seq_num_heads"),
             num_layers=sequence_transformer_kwargs.get("seq_num_layers"),
         )
 
-        self.nlp_encoder = DistilBertModel.from_pretrained(nlp_encoder_path)
+        #self.nlp_encoder = DistilBertModel.from_pretrained(nlp_encoder_path)
+        self.nlp_encoder = AutoModel.from_pretrained(nlp_encoder_path)
         self.search_nlp_dense_0 = torch.nn.Linear(
             in_features=nlp_dim,
             out_features=seq_embed_dim * 2
         )
         self.search_nlp_dense_1 = torch.nn.Linear(
             in_features=seq_embed_dim * 2,
             out_features=seq_embed_dim
@@ -479,15 +494,16 @@
         svc_out = self.svc_embedding(svc_in.long())
         svc_out = self.mm_pooling(svc_out)
         new_svc_out = self.new_svc_embedding(new_svc_in.long())
         new_svc_out = self.mm_pooling(new_svc_out)
 
         aep_seq_out = self.sequence_transformer(page_in=page_in, item_in=item_in, vl_in=vl_in)
 
-        search_out = self.nlp_encoder(**search_in).last_hidden_state[:, 0, :].to(dtype=torch.float32)
+#        search_out = self.nlp_encoder(**search_in).last_hidden_state[:, 0, :].to(dtype=torch.float32)
+        search_out = self.nlp_encoder(**search_in).pooler_output.to(dtype=torch.float32)
         search_out = self.search_nlp_dense_0(search_out)
         search_out = self.nlp_act(search_out)
         search_out = self.search_nlp_dense_1(search_out)
         search_out = self.nlp_act(search_out)
 
         user_ctx_out = self.user_context_head(deep_in=user_deep_in, wide_in=user_wide_in)
         user_out = torch.stack([search_out, aep_seq_out, svc_out, new_svc_out, user_ctx_out], dim=1)
@@ -511,19 +527,121 @@
         out = torch.mul(user_out, offer_out)
         out = torch.sum(out, dim=1)
         out = self.out_act(out)
 
         return out, user_out, offer_out, user_aux_loss
 
 
+class GRecUPG(nn.Module):
+    def __init__(self, user_deep_dims, user_deep_embed_dims, user_num_wide, user_wad_embed_dim,
+                 svc_dim, svc_embed_dim, new_svc_dim, new_svc_embed_dim, page_dim, item_dim,
+                 seq_embed_dim, nlp_encoder_path, nlp_dim, sequence_transformer_kwargs,
+                 user_moe_kwargs):
+        super().__init__()
+        self.seq_embed_dim = seq_embed_dim
+
+        # user layers
+        self.svc_embedding = nn.Embedding(svc_dim, svc_embed_dim)
+        self.new_svc_embedding = nn.Embedding(new_svc_dim, new_svc_embed_dim)
+        self.mm_pooling = MeanMaxPooling()
+
+        self.page_embedding = nn.Embedding(page_dim, seq_embed_dim)
+        self.item_embedding = nn.Embedding(item_dim, seq_embed_dim)
+        self.sequence_transformer = ParallelTransformerAEP2S(
+            page_embedding=self.page_embedding,
+            item_embedding=self.item_embedding,
+            dim=seq_embed_dim,
+            dim_head=seq_embed_dim,
+            heads=sequence_transformer_kwargs.get("seq_num_heads"),
+            num_layers=sequence_transformer_kwargs.get("seq_num_layers"),
+        )
+
+        self.nlp_encoder = AutoModel.from_pretrained(nlp_encoder_path)
+        self.search_nlp_dense_0 = torch.nn.Linear(
+            in_features=nlp_dim,
+            out_features=seq_embed_dim * 2
+        )
+        self.search_nlp_dense_1 = torch.nn.Linear(
+            in_features=seq_embed_dim * 2,
+            out_features=seq_embed_dim
+        )
+        self.nlp_act = nn.LeakyReLU(0.2)
+
+        self.user_context_head = ContextTransformerAndWide(
+            deep_dims=user_deep_dims,
+            num_wide=user_num_wide,
+            deep_embed_dims=user_deep_embed_dims,
+            wad_embed_dim=user_wad_embed_dim,
+        )
+        self.user_att_pooling = ParallelTransformerBlock(
+            dim=seq_embed_dim, dim_head=seq_embed_dim, heads=1
+        )
+        # nlp_out + aep_seq_out + svc_out + new_svc_out + user_ctx_out
+        self.user_concat_dim = seq_embed_dim + seq_embed_dim + seq_embed_dim \
+                               + seq_embed_dim + seq_embed_dim
+        self.user_moe = MoEFFLayerTopK(
+            dim=seq_embed_dim,
+            num_experts=user_moe_kwargs.get("num_experts"),
+            expert_capacity=user_moe_kwargs.get("expert_capacity"),
+            hidden_size=seq_embed_dim,
+            expert_class=ExpertLayer,
+            num_K=user_moe_kwargs.get("num_K"),
+        )
+
+        self.user_act = nn.LeakyReLU(0.2)
+        self.user_dropout = nn.Dropout(p=0.1)
+        self.user_dense_0 = nn.Linear(
+            in_features=self.user_concat_dim,
+            out_features=seq_embed_dim * 3
+        )
+        self.user_dense_1 = nn.Linear(
+            in_features=seq_embed_dim * 3,
+            out_features=seq_embed_dim
+        )
+
+        self.out_dense = nn.Linear(
+            in_features=seq_embed_dim,
+            out_features=1
+        )
+        self.out_act = nn.Sigmoid()
+
+    def forward(self, user_deep_in, svc_in, new_svc_in, page_in, item_in, vl_in,
+                user_wide_in, search_in):
+        svc_out = self.svc_embedding(svc_in.long())
+        svc_out = self.mm_pooling(svc_out)
+        new_svc_out = self.new_svc_embedding(new_svc_in.long())
+        new_svc_out = self.mm_pooling(new_svc_out)
+
+        aep_seq_out = self.sequence_transformer(page_in=page_in, item_in=item_in, vl_in=vl_in)
+
+        search_out = self.nlp_encoder(**search_in).pooler_output.to(dtype=torch.float32)
+        search_out = self.search_nlp_dense_0(search_out)
+        search_out = self.nlp_act(search_out)
+        search_out = self.search_nlp_dense_1(search_out)
+        search_out = self.nlp_act(search_out)
 
+        user_ctx_out = self.user_context_head(deep_in=user_deep_in, wide_in=user_wide_in)
+        user_out = torch.stack([search_out, aep_seq_out, svc_out, new_svc_out, user_ctx_out], dim=1)
+        user_out = self.user_att_pooling(user_out)
+        user_out, user_aux_loss = self.user_moe(user_out)
+        user_out = user_out.reshape(-1, self.user_concat_dim)
+        user_out = self.user_dense_0(user_out)
+        user_out = self.user_act(user_out)
+        user_out = self.user_dropout(user_out)
+        user_out = self.user_dense_1(user_out)
+        user_out = self.user_act(user_out)
+
+        out = self.out_dense(user_out)
+        out = self.out_act(out)
+
+        return out, user_aux_loss
+
+    
 class PaRS2(nn.Module):
-    def __init__(self, deep_dims, page_dim, seq_dim, item_meta_dim, page_embed_dim, seq_embed_dim, item_embed_dim, item_meta_embed_dim, item_pre_embed_dim, deep_embed_dims, wad_embed_dim, nlp_embed_dim, seq_hidden_size, nlp_encoder_path, task_type_dim, task_type_embed_dim, task_out_dims,
-                 num_wide=0, num_shared=0, nlp_dim=0, num_meta_wide=0, item_meta_wide_embed_dim=0, item_freeze=None, item_pre_freeze=None, nlp_freeze=None, context_head_kwargs=None, sequence_transformer_kwargs=None,
-                 page_embedding_weight=None, item_embedding_weight=None, item_meta_embedding_weight=None, item_pre_embedding_weight=None, shared_embeddings_weight=None, moe_kwargs=None):
+    def __init__(self, deep_dims, page_dim, seq_dim, page_embed_dim, seq_embed_dim, item_embed_dim, item_meta_dim, item_meta_embed_dim, item_pre_embed_dim, deep_embed_dims, wad_embed_dim, nlp_embed_dim, seq_hidden_size, nlp_encoder_path, task_type_dim, task_type_embed_dim, task_out_dims, num_wide=0, num_shared=0, nlp_dim=0, page_meta_dim=0, page_meta_embed_dim=0, num_page_meta_wide=0, page_meta_wide_embed_dim=0, num_item_meta_wide=0, item_meta_wide_embed_dim=0, page_freeze=None, item_freeze=None, item_pre_freeze=None, nlp_freeze=None, context_head_kwargs=None, sequence_transformer_kwargs=None, page_embedding_weight=None, page_meta_embedding_weight=None, item_embedding_weight=None, item_meta_embedding_weight=None, item_pre_embedding_weight=None, shared_embeddings_weight=None, moe_kwargs=None):
         super().__init__()
         self.nlp_encoder = DistilBertModel.from_pretrained(nlp_encoder_path)
         context_head_kwargs = context_head_kwargs if context_head_kwargs else {}
         sequence_transformer_kwargs = sequence_transformer_kwargs if sequence_transformer_kwargs else {}
         
         if page_embedding_weight is None:
             print("not use pretrained embedding")
@@ -533,26 +651,34 @@
             self.page_embedding = nn.Embedding.from_pretrained(page_embedding_weight, freeze=False)
         if item_embedding_weight is None:
             print("not use pretrained embedding")
             self.item_embedding = nn.Embedding(seq_dim, item_embed_dim)
         else:
             print("use pretrained item embedding")
             self.item_embedding = nn.Embedding.from_pretrained(item_embedding_weight, freeze=False)
+        if page_meta_embedding_weight is None:
+            print("not use pretrained embedding")
+            self.page_meta_embedding = nn.Embedding(page_meta_dim, page_meta_embed_dim)
+        else:
+            print("use pretrained item embedding")
+            self.page_meta_embedding = nn.Embedding.from_pretrained(page_meta_embedding_weight, freeze=False)
         if item_meta_embedding_weight is None:
             print("not use pretrained embedding")
             self.item_meta_embedding = nn.Embedding(item_meta_dim, item_meta_embed_dim)
         else:
             print("use pretrained item embedding")
             self.item_meta_embedding = nn.Embedding.from_pretrained(item_meta_embedding_weight, freeze=False)
         if item_pre_embedding_weight is None:
             print("not use pretrained embedding")
             self.item_pre_embedding = nn.Embedding(seq_dim, item_pre_embed_dim)
         else:
             print("use pretrained item pre embedding")
             self.item_pre_embedding = nn.Embedding.from_pretrained(item_pre_embedding_weight, freeze=False)
+        if page_freeze:
+            self.page_embedding.weight.requires_grad = False
         if item_freeze:
             self.item_embedding.weight.requires_grad = False
         if item_pre_freeze:
             self.item_pre_embedding.weight.requires_grad = False
 
         if nlp_freeze:
             for param in self.nlp_encoder.parameters():
@@ -573,19 +699,22 @@
             item_embedding=self.item_embedding,
             item_meta_embedding=self.item_meta_embedding,
             item_pre_embedding=self.item_pre_embedding,
             dim=seq_embed_dim,
             dim_head=seq_embed_dim,
             heads=sequence_transformer_kwargs.get("seq_num_heads"),
             num_layers=sequence_transformer_kwargs.get("seq_num_layers"),
-            num_meta_wide = num_meta_wide,
-            item_meta_wide_embed_dim = item_meta_wide_embed_dim,
+            num_page_meta_wide=num_page_meta_wide,
+            num_item_meta_wide=num_item_meta_wide,
+            page_meta_embedding=self.page_meta_embedding,
+            page_meta_wide_embed_dim=page_meta_wide_embed_dim,
+            item_meta_wide_embed_dim=item_meta_wide_embed_dim,
             moe_kwargs=moe_kwargs
         )
-       
+    
         self.att_pooling = ParallelTransformerBlock(
             dim=256, dim_head=256, heads=1
         )
         self.seq_dense = torch.nn.Linear(
             in_features=seq_embed_dim,
             out_features=seq_embed_dim
         )
@@ -603,18 +732,18 @@
             self.combined_dim // 2, 
             task_out_dims[0]
         )
         self.tasks_act1 = self.tasks_act2 = nn.LeakyReLU(0.2)
         self.seq_dim = seq_dim
         self.task_type_dim = task_type_dim
 
-        if num_meta_wide>0:
-            self.wide_meta_batch_norm = nn.BatchNorm1d(num_meta_wide)
-            if item_meta_wide_embed_dim>0:
-                self.wide_meta_dense = nn.Linear(num_meta_wide, item_meta_wide_embed_dim)
+        if num_item_meta_wide > 0:
+            self.wide_meta_batch_norm = nn.BatchNorm1d(num_item_meta_wide)
+            if item_meta_wide_embed_dim > 0:
+                self.wide_meta_dense = nn.Linear(num_item_meta_wide, item_meta_wide_embed_dim)
             else: 
                 print("There are wide meta features but item_meta_wide_embed_dim is not given!")
             self.wide_meta_act = nn.LeakyReLU(0.2)
 
     def split_task(self, task_type_dim, task_in, combined_out):
         task_indices = []
         task_outs = []
@@ -627,42 +756,51 @@
             task_user_out = self.tasks_act1(task_out)
             task_out = self.tasks_dense2(task_user_out)
             task_indices.append(task_indice)
             task_user_outs.append(task_user_out)
             task_outs.append(task_out)
         return task_indices, task_outs, task_user_outs
         
-    def forward(self, deep_in, page_in, item_in, item_meta_in, vl_in, task_in, current_in, current_meta_in, wide_in=None, input_ids=None, attention_mask=None, current_meta_wide_in=None, item_meta_wide_in=None, shared_in=None):
+    def forward(self, deep_in, page_in, item_in, item_meta_in, vl_in, task_in, current_in, current_meta_in, wide_in=None, input_ids=None, attention_mask=None, page_meta_in=None, page_meta_wide_in=None, current_meta_wide_in=None, item_meta_wide_in=None, shared_in=None):
         """
         Args:
-            deep_in: list, a list of Tensor of shape [batch_size, deep_dims].
-            seq_in: Tensor, shape [batch_size, seq_len].
-            vl_in: Tensor, shape [batch_size].
-            wide_in: list, a list of Tensor of shape [batch_size, num_wide].
-            shared_in: list, a list of Tensor of shape [batch_size, num_shared] (default=None).
-            search_ids: tensor, Tensor of shape [batch_size, sentence_length] (default=None).
-            att_mask: tensor, Tensor of shape [batch_size, sentence_length] (default=None).
+            deep_in: list, a list of tensor of shape [batch_size, deep_dims]
+            page_in: tensor, page input sequence [batch_size, seq_len]
+            item_in: tensor, item input sequence [batch_size, seq_len]
+            item_meta_in: tensor, item deep meta data input sequence [batch_size, seq_len]
+            vl_in: tensor, valid length of input data [batch_size]
+            taks_in: tensor, task type index [batch_size]
+            current_in: tensor, current item input [batch_size]
+            current_meta_in: tensor, current item deep meta data input [batch_size]
+            wide_in: list, a list of tensor of shape [batch_size, num_wide]
+            inputs_id: list, a list of tensor of shape [batch_size, num_shared] (default=None)
+            att_mask: tensor, tensor of shape [batch_size, sentence_length] (default=None)
+            page_meta_in: tensor, page deep meta data input sequence [batch_size, seq_len]
+            page_meta_wide_in: tensor, page wide meta data input sequence [batch_size, num_page_meta_wide, seq_len]
+            current_meta_wide_in: list, a list of tensor of shape [batch_size, num_item_meta_wide]
+            item_meta_wide_in: tensor, item wide meta data input sequence [batch_size, num_item_meta_wide, seq_len]
+            search_ids: tensor, Tensor of shape [batch_size, sentence_length] (default=None)
 
         Return:
-            out: Tensor, shape [batch_size, seq_dim].
-            user_out: Tensor, shape [batch_size, seq_embed_dim].
+            out: tensor, shape [batch_size, seq_dim].
+            user_out: tensor, shape [batch_size, seq_embed_dim].
         """
         search_out = self.nlp_encoder(input_ids=input_ids, attention_mask=attention_mask).last_hidden_state[:,0,:].to(dtype=torch.float32)
         search_out = self.nlp_dense(search_out)
         ctx_out = self.context_head(deep_in=deep_in, wide_in=wide_in, shared_in=shared_in)
-        seq_out = self.sequence_transformer(page_in=page_in, item_in=item_in, item_meta_in=item_meta_in, vl_in=vl_in, item_meta_wide_in=item_meta_wide_in)
+        seq_out = self.sequence_transformer(page_in=page_in, item_in=item_in, item_meta_in=item_meta_in, vl_in=vl_in, page_meta_in=page_meta_in, page_meta_wide_in=page_meta_wide_in, item_meta_wide_in=item_meta_wide_in)
         seq_out = self.seq_dense(seq_out)
         current_item_out = self.item_embedding(current_in)
         current_meta_out = self.item_meta_embedding(current_meta_in)
         current_pre_out = self.item_pre_embedding(current_in)	        
         if current_meta_wide_in is not None:
-            current_meta_wide_in_list =[wide_i.float() for wide_i in current_meta_wide_in]
+            current_meta_wide_in_list = [wide_i.float() for wide_i in current_meta_wide_in]
             current_meta_wide_cat = torch.stack(current_meta_wide_in_list, dim=0)
             current_meta_wide_out = torch.transpose(current_meta_wide_cat, dim1=1, dim0=0)
-            if len(current_meta_wide_in)>1:
+            if len(current_meta_wide_in) > 1:
                 current_meta_wide_out_norm = self.wide_meta_batch_norm(current_meta_wide_out)
             else:
                 current_meta_wide_out_norm = current_meta_wide_out
             current_meta_wide_out_norm = self.wide_meta_dense(current_meta_wide_out_norm)
             current_meta_wide_out_norm = self.wide_meta_act(current_meta_wide_out_norm)
             current_out = torch.cat((current_item_out, current_meta_out, current_pre_out, current_meta_wide_out_norm), 1)
         else:
```

### Comparing `vz-recommender-0.4.5/src/vz_recommender/models/transformer.py` & `vz-recommender-0.4.6/src/vz_recommender/models/transformer.py`

 * *Files 25% similar despite different names*

```diff
@@ -231,114 +231,14 @@
         mask = self.create_key_padding_mask(seq_in=page_in, valid_length=vl_in)
         seq_out = self.seq_encoder(seq_out, src_key_padding_mask=mask)
         if mask[:, 0].any():
             seq_out = seq_out.nan_to_num(nan=0.0)
         seq_out = self.seq_pooling_dp(seq_out)
         seq_out = self.seq_dense(seq_out)
         return seq_out
-    
-class TransformerAEP2(TransformerHistory):
-    """
-    Transformer Adobe Experience Platform (AEP): Instantiate Positional Encoder, Transformer Encoder 
-    and Mean Max Pooling (refer utils)
-    Concatenate item meta-feature embeddings and item-id embeddings as item full embeddings.
-    Sequences of page embeddings and item full embeddings are multiplied and passeed through the transformer encoder.
-
-    Args :
-        page_embedding : the page field embeddings
-        item_embedding : the item embeddings
-        item_meta_embedding: the item meta data embedding module
-        seq_embed_dim : the number of expected features in the encoder/decoder inputs (default=200)
-        seq_max_length : the max sequence length, (default=8)
-        seq_num_heads : the number of heads in the multiheadattention models (default=4)
-        seq_hidden_size : the hidden layer size of the feedforward network model (default=512).
-        seq_transformer_dropout : the dropout value (default=0.0)
-        seq_num_layers : the number of sub-encoder-layers in the encoder (default=2).
-        seq_pooling_dropout : the pooling dropout value (default=0.0).
-        seq_pe : If "True" then positional encoding is applied (default=True)
-    
-    Examples::
-        >>> import torch 
-        >>> from torch import nn
-        >>> from vz_recommender.models.transformer import TransformerHistory, TransformerAEP2
-        >>> page_embedding = nn.Embedding(4, 32)
-        >>> item_embedding = nn.Embedding(6, 24)
-        >>> item_meta_embedding = nn.Embedding(6, 8)
-        >>> transformer_model = TransformerAEP2(page_embedding=page_embedding, item_embedding=item_embedding, item_meta_embedding=item_meta_embedding, seq_embed_dim=32, seq_max_length=5,seq_num_heads=2, seq_hidden_size=4, seq_transformer_dropout=0.0, seq_num_layers=2,
-    seq_pooling_dropout=0.0, seq_pe=True)
-        >>> page_in = torch.randint(4, (3,5))
-        >>> item_in = torch.randint(6, (3,5))
-        >>> item_meta_in = torch.randint(6, (3,5))
-        >>> vl_in = torch.randint(1, 4, (3,))
-        >>> out = transformer_model(page_in, item_in, item_meta_in, vl_in)
-    """
-    def __init__(self, page_embedding, item_embedding, item_meta_embedding, seq_embed_dim, seq_max_length=8,
-                 seq_num_heads=4, seq_hidden_size=512, seq_transformer_dropout=0.0, seq_num_layers=2,
-                 seq_pooling_dropout=0.0, seq_pe=True):
-        super().__init__(seq_embed_dim, seq_max_length=8, seq_num_heads=4, seq_hidden_size=512,
-                         seq_transformer_dropout=0.0, seq_num_layers=2, seq_pooling_dropout=0.0,
-                         seq_pe=True)
-        self.page_embedding = page_embedding
-        self.item_embedding = item_embedding
-        self.item_meta_embedding = item_meta_embedding
-        self.seq_pos = seq_pe
-        self.seq_embed_dim = seq_embed_dim
-        if seq_pe:
-            self.pos_encoder = PositionalEncoding(d_model=seq_embed_dim,
-                                                  dropout=seq_transformer_dropout,
-                                                  max_len=seq_max_length)
-        encoder_layers = TransformerEncoderLayer(d_model=seq_embed_dim,
-                                                 nhead=seq_num_heads,
-                                                 dropout=seq_transformer_dropout,
-                                                 dim_feedforward=seq_hidden_size,
-                                                 activation='relu',
-                                                 batch_first=True)
-        self.seq_encoder = TransformerEncoder(encoder_layers, num_layers=seq_num_layers)
-        self.seq_pooling_dp = MeanMaxPooling(dropout=seq_pooling_dropout)
-        self.seq_dense = torch.nn.Linear(2 * seq_embed_dim, seq_embed_dim)
-
-    def forward(self, page_in, item_in, item_meta_in, vl_in, seq_history=None):
-        """
-        Creates a composition of page embedding and combined seq of item and meta embeding. Applies 
-        Positional Encoding, Masks padded values and Mean Max Pooling (refer utils)
-        
-        Args :
-            page_in: page input values
-            item_in : item input values
-            vl_in: valid length to be used
-            seq_history: Tensor
-
-        Return :
-            Sequential output after applying transformer 
-
-        Shape :
-            page_in: [batch_size, seq_len]
-            item_in: [batch_size, seq_len]b
-            vl_in: [batch_size]
-            seq_history: [batch_size, history_len]
-
-            out : [batch_size, 2*seq_embed_dim]
-        """
-        page_embed_out = self.page_embedding(page_in.long())
-        item_embed_out = self.item_embedding(item_in.long())
-        item_meta_embed_out = self.item_meta_embedding(item_meta_in.long())
-        item_full_out = torch.cat((item_embed_out, item_meta_embed_out), 2)
-#         seq_embed_out = torch.cat((page_embed_out, item_embed_out), 2)
-        seq_embed_out = torch.mul(page_embed_out, item_full_out)
-        seq_out = seq_embed_out
-        if self.seq_pos:
-            seq_out = seq_out * math.sqrt(self.seq_embed_dim)
-            seq_out = self.pos_encoder(seq_out)
-        mask = self.create_key_padding_mask(seq_in=page_in, valid_length=vl_in)
-        seq_out = self.seq_encoder(seq_out, src_key_padding_mask=mask)
-        if mask[:, 0].any():
-            seq_out = seq_out.nan_to_num(nan=0.0)
-        seq_out = self.seq_pooling_dp(seq_out)
-        seq_out = self.seq_dense(seq_out)
-        return seq_out
 
 
 class ParallelTransformerBlock(nn.Module):
     """
     Parallel Transformer Block : Instantiates Rotary Embedding ( RoPE https://arxiv.org/abs/2104.09864), Linear and SwiGLU Activation Layer
     (a variant of GLU https://arxiv.org/pdf/2002.05202.pdf)
     The architecture is based on the paper "PaLM: Scaling Language Modeling with Pathways" (https://arxiv.org/abs/2204.02311)
@@ -484,375 +384,246 @@
 
         out = rearrange(out, "b h n d -> b n (h d)")
 #         out, aux_loss = self.fused_attn_moe_proj(out)
 
         out = self.attn_out(out) + self.ff_out(ff)
         return out
     
-    
-class TransformerAEPCat(TransformerHistory):
-    """
-    Transformer Adobe Experience Platform (AEP) : Instantiates Positonal Encoding, Transformer Encoder layer, 
-    Mean Max Pooling (refer utils)
-    Sequences of page embeddings and item embeddings are concatenated and passed through the transformer encoder.
-
-    Args :
-        page_embedding : the page field embeddings
-        item_embedding : the item embeddings
-        seq_embed_dim : the number of expected features in the encoder/decoder inputs (default=200)
-        seq_max_length : the max sequence length, (default=8)
-        seq_num_heads : the number of heads in the multiheadattention models (default=4)
-        seq_hidden_size : the hidden layer size of the feedforward network model (default=512).
-        seq_transformer_dropout : the dropout value (default=0.0)
-        seq_num_layers : the number of sub-encoder-layers in the encoder (default=2).
-        seq_pooling_dropout : the pooling dropout value (default=0.0).
-        seq_pe : If "True" then positional encoding is applied (default=True)
-    
-    Examples::
-        >>> import torch 
-        >>> from torch import nn
-        >>> from vz_recommender.models.transformer import TransformerHistory, TransformerAEPCat
-        >>> page_embedding = nn.Embedding(4, 32)
-        >>> item_embedding = nn.Embedding(6, 32)
-        >>> transformer_model = TransformerAEPCat(page_embedding=page_embedding, item_embedding=item_embedding, seq_embed_dim=64, seq_max_length=5,seq_num_heads=2, seq_hidden_size=4, seq_transformer_dropout=0.0, seq_num_layers=2, 
-seq_pooling_dropout=0.0, seq_pe=True)
-        >>> page_in = torch.randint(4, (3,5))
-        >>> item_in = torch.randint(6, (3,5))
-        >>> vl_in = torch.randint(1, 4, (3,))
-        >>> out = transformer_model(page_in, item_in, vl_in)
-    """
-    def __init__(self, page_embedding, item_embedding, seq_embed_dim, seq_max_length=8,
-                 seq_num_heads=4, seq_hidden_size=512, seq_transformer_dropout=0.0, seq_num_layers=2,
-                 seq_pooling_dropout=0.0, seq_pe=True):
-        super().__init__(seq_embed_dim, seq_max_length=8, seq_num_heads=4, seq_hidden_size=512,
-                         seq_transformer_dropout=0.0, seq_num_layers=2, seq_pooling_dropout=0.0,
-                         seq_pe=True)
-        self.page_embedding = page_embedding
-        self.item_embedding = item_embedding
-        self.seq_pos = seq_pe
-        self.seq_embed_dim = seq_embed_dim
-        if seq_pe:
-            self.pos_encoder = PositionalEncoding(d_model=seq_embed_dim,
-                                                  dropout=seq_transformer_dropout,
-                                                  max_len=seq_max_length)
-        encoder_layers = TransformerEncoderLayer(d_model=seq_embed_dim,
-                                                 nhead=seq_num_heads,
-                                                 dropout=seq_transformer_dropout,
-                                                 dim_feedforward=seq_hidden_size,
-                                                 activation='relu',
-                                                 batch_first=True)
-        self.seq_encoder = TransformerEncoder(encoder_layers, num_layers=seq_num_layers)
-        self.seq_pooling_dp = MeanMaxPooling(dropout=seq_pooling_dropout)
-        self.seq_dense = torch.nn.Linear(2 * seq_embed_dim, seq_embed_dim)
-
-    def forward(self, page_in, item_in, vl_in, seq_history=None):
-        """
-         Standard Attention tranformer takes in input and gives output
-
-        Args :
-            page_in: page input values
-            item_in : item input values
-            vl_in: valid length to be used
-            seq_history: Tensor
-
-        Return :
-            Sequential output after applying transformer 
-
-        Shape :
-            page_in: [batch_size, seq_len]
-            item_in: [batch_size, seq_len]
-            vl_in: [batch_size]
-            seq_history: [batch_size, history_len]
-
-            out : [batch_size, 2*seq_embed_dim]
-        """
-        page_embed_out = self.page_embedding(page_in.long())
-        item_embed_out = self.item_embedding(item_in.long())
-        seq_embed_out = torch.cat((page_embed_out, item_embed_out), 2)
-        seq_out = seq_embed_out
-        if self.seq_pos:
-            seq_out = seq_out * math.sqrt(self.seq_embed_dim)
-            seq_out = self.pos_encoder(seq_out)
-        mask = self.create_key_padding_mask(seq_in=page_in, valid_length=vl_in)
-        seq_out = self.seq_encoder(seq_out, src_key_padding_mask=mask)
-        if mask[:, 0].any():
-            seq_out = seq_out.nan_to_num(nan=0.0)
-        seq_out = self.seq_pooling_dp(seq_out)
-        seq_out = self.seq_dense(seq_out)
-        return seq_out
-
 
 class ParallelTransformerAEP(nn.Module):
     """
-    Parallel Transformer Adobe Enterprise Product: Instantiates Mean Max Pooling, Linear Transformation layer
-    and Parallel Transformer Block
-    Sequence of page embeddings and item embeddings are multiplied and passed through the parallel transformer encoder layers.
-
-    Args :
-        page_embedding : the page field embeddings
-        item_embedding : the item embeddings
-        dim : the dimension size
-        dim_head : dimensions of multihead attention network
-        heads : no of multi-head attention required
-        num_layers : number of hidden layers needed
-        ff_mult : feedforward multi
-        seq_pooling_dropout :  the pooling dropout value (default=0.0).
-
-    Examples::
-        >>> import torch 
-        >>> from torch import nn
-        >>> from vz_recommender.models.transformer import ParallelTransformerAEP
-        >>> page_embedding = nn.Embedding(4, 32)
-        >>> item_embedding = nn.Embedding(6, 32)
-        >>> transformer_model = ParallelTransformerAEP(page_embedding=page_embedding, item_embedding=item_embedding, dim=32, dim_head=32, heads=2, num_layers=2, ff_mult=4, seq_pooling_dropout=0.0)
-        >>> page_in = torch.randint(4, (3,5))
-        >>> item_in = torch.randint(6, (3,5))
-        >>> vl_in = torch.randint(1, 4, (3,))
-        >>> out = transformer_model(page_in, item_in, vl_in)
-    """
-    def __init__(self, page_embedding, item_embedding, dim, dim_head, heads, num_layers, ff_mult=4, seq_pooling_dropout=0.0, moe_kwargs=None):
-        super().__init__()
-        self.page_embedding = page_embedding
-        self.item_embedding = item_embedding
-        self.seq_pooling_dp = MeanMaxPooling(dropout=seq_pooling_dropout)
-        self.seq_dense = torch.nn.Linear(2 * dim, dim)  
-        self.num_layers = num_layers
-#         self.ptransformer = nn.ModuleList([
-#             ParallelTransformerBlock(dim=dim, dim_head=dim_head, heads=heads, ff_mult=ff_mult, moe_kwargs=moe_kwargs)
-#             for _ in range(self.num_layers)
-#         ])
-        
-        self.ptransformer = nn.ModuleList([
-            Residual(ParallelTransformerBlock(dim=dim, dim_head=dim_head, heads=heads, ff_mult=ff_mult, moe_kwargs=moe_kwargs))
-            for _ in range(self.num_layers)
-        ])
-        
-    def forward(self, page_in, item_in, vl_in):
-        """
-        Takes in item and page embedding and applies Parallel transformer 
-
-        Args :
-            page_in: input sequence
-            item_in: input sequence
-            vl_in: valid length of input data
-
-        Return :
-            Parallel transformer output
-
-        Shape: page_in: [batch_size, seq_len]
-               item_in: [batch_size, seq_len]
-               vl_in: [batch_size]
-
-               out: [batch_size, seq_embed_dim]
-        """
-        page_embed_out = self.page_embedding(page_in.long())
-        item_embed_out = self.item_embedding(item_in.long())
-#         aux_loss = 0
-        x = torch.mul(page_embed_out, item_embed_out)
-#         x = torch.cat((page_embed_out, item_embed_out), 2)
-        for i in range(self.num_layers):
-            x = self.ptransformer[i](x, vl_in)
-#             x, aux_loss = self.ptransformer[i](x, vl_in)
-#             aux_loss += aux_loss
-
-        out = self.seq_pooling_dp(x)
-        out = self.seq_dense(out)        
-        return out
-
-    
-class ParallelTransformerAEP2(nn.Module):
-    """
     Parallel Transformer Adobe Enterprise Product : Instantiates Parallel Transformer Block
-    Concatenate item meta-feature embeddings, pred-trained visual embeddings, item-id embeddings as item full embeddings.
+    Concatenate item meta-feature embeddings, pred-trained visual embeddings, item-id embeddings, and item meta wide features as item full embeddings.
     Sequence of page embeddings and item full embeddings are multiplied and passed through the parallel transformer encoder layers.
 
     Args :
-        page_embedding : the page field embeddings
+        page_embedding : the page field embeddings 
         item_embedding : the item embeddings
-        item_meta_embedding : item meta data embedding module
-        item_pre_embedding: item pretrained embedding module
         dim : the dimension size
         dim_head : dimensions of multihead attention network
         heads : no of multi-head attention required
         num_layers : number of hidden layers needed
+        num_page_meta_wide: number of page meta wide features
+        page_meta_wide_embed_dim: dimensions of page meta wide feature output 
+        num_item_meta_wide: number of item meta wide features
+        item_meta_wide_embed_dim: dimensions of item meta wide feature output 
         ff_mult : feedforward multi
-        seq_pooling_dropout :  the pooling dropout value (default=0.0).
-    
+        seq_pooling_dropout :  the pooling dropout value (default=0.0)
+        page_meta_embedding : page meta data embeddings
+        item_meta_embedding : item meta data embeddings
+        item_pre_embedding : item pretrained data embeddings
+        
     Examples::
         >>> import torch 
         >>> from torch import nn
-        >>> from vz_recommender.models.transformer import ParallelTransformerAEP2
-        >>> page_embedding = nn.Embedding(4, 32)
-        >>> item_embedding = nn.Embedding(6, 24)
+        >>> from vz_recommender.models.transformer import ParallelTransformerAEP3
+        >>> page_embedding = nn.Embedding(4, 20)
+        >>> page_meta_embedding = nn.Embedding(4, 8)
+        >>> num_page_meta_wide = 2
+        >>> page_meta_wide_embed_dim = 4
+        >>> item_embedding = nn.Embedding(6, 20)
         >>> item_meta_embedding = nn.Embedding(8, 4)
         >>> item_pre_embedding =  nn.Embedding(6, 4)
-        >>> transformer_model = ParallelTransformerAEP2(page_embedding=page_embedding, item_embedding=item_embedding, item_meta_embedding=item_meta_embedding, item_pre_embedding=item_pre_embedding, dim=32, dim_head=32, heads=2, num_layers=2, ff_mult=4, seq_pooling_dropout=0.0)
+        >>> num_item_meta_wide = 2
+        >>> item_meta_wide_embed_dim = 4
+        >>> transformer_model = ParallelTransformerAEP3(page_embedding=page_embedding, page_meta_embedding=page_meta_embedding, num_page_meta_wide=num_page_meta_wide, page_meta_wide_embed_dim=page_meta_wide_embed_dim, item_embedding=item_embedding, item_meta_embedding=item_meta_embedding, item_pre_embedding=item_pre_embedding, num_item_meta_wide = num_item_meta_wide, item_meta_wide_embed_dim=item_meta_wide_embed_dim, dim=32, dim_head=32, heads=2, num_layers=2, ff_mult=4, seq_pooling_dropout=0.0)
         >>> page_in = torch.randint(4, (3,5))
+        >>> page_meta_in = torch.randint(4, (3,5))
+        >>> page_meta_wide_in = torch.rand(3,2,5)
         >>> item_in = torch.randint(6, (3,5))
         >>> item_meta_in = torch.randint(8, (3,5))
+        >>> item_meta_wide_in = torch.rand(3,2,5)
         >>> vl_in = torch.randint(1, 4, (3,))
-        >>> out = transformer_model(page_in, item_in, item_meta_in, vl_in)
+        >>> out = transformer_model(page_in, item_in, item_meta_in, vl_in, page_meta_in, page_meta_wide_in, item_meta_wide_in)
     """
-    def __init__(self, page_embedding, item_embedding, item_meta_embedding, item_pre_embedding, dim, dim_head, heads, num_layers, ff_mult=4, seq_pooling_dropout=0.0, moe_kwargs=None):
+    def __init__(self, page_embedding, item_embedding, dim, dim_head, heads, num_layers, num_page_meta_wide=0, page_meta_wide_embed_dim=0, num_item_meta_wide=0, item_meta_wide_embed_dim=0, ff_mult=4, seq_pooling_dropout=0.0, page_meta_embedding=None, item_meta_embedding=None, item_pre_embedding=None, moe_kwargs=None):
         super().__init__()
         self.page_embedding = page_embedding
+        self.page_meta_embedding = page_meta_embedding
+        if num_page_meta_wide > 0:
+            self.num_page_meta_wide = num_page_meta_wide
+            self.page_meta_wide_dense = nn.Linear(num_page_meta_wide, page_meta_wide_embed_dim)
+            self.page_meta_wide_act = nn.LeakyReLU(0.2)
+        if num_page_meta_wide > 1:
+            self.page_meta_wide_batch_norm = nn.BatchNorm1d(num_page_meta_wide)
         self.item_embedding = item_embedding
         self.item_meta_embedding = item_meta_embedding
         self.item_pre_embedding = item_pre_embedding
+        if num_item_meta_wide > 0:
+            self.num_item_meta_wide = num_item_meta_wide
+            self.item_meta_wide_dense = nn.Linear(num_item_meta_wide, item_meta_wide_embed_dim)
+            self.item_meta_wide_act = nn.LeakyReLU(0.2)
+        if num_item_meta_wide > 1:
+            self.item_meta_wide_batch_norm = nn.BatchNorm1d(num_item_meta_wide)
         self.seq_pooling_dp = MeanMaxPooling(dropout=seq_pooling_dropout)
         self.seq_dense = torch.nn.Linear(2 * dim, dim)  
         self.num_layers = num_layers
-#         self.ptransformer = nn.ModuleList([
-#             ParallelTransformerBlock(dim=dim, dim_head=dim_head, heads=heads, ff_mult=ff_mult, moe_kwargs=moe_kwargs)
-#             for _ in range(self.num_layers)
-#         ])
         
         self.ptransformer = nn.ModuleList([
             Residual(ParallelTransformerBlock(dim=dim, dim_head=dim_head, heads=heads, ff_mult=ff_mult, moe_kwargs=moe_kwargs))
             for _ in range(self.num_layers)
         ])
         
-    def forward(self, page_in, item_in, item_meta_in, vl_in):
+    def forward(self, page_in, item_in, item_meta_in, vl_in, page_meta_in=None, page_meta_wide_in=None, item_meta_wide_in=None):
         """
         Applies Parallel transformer on the page embedding and concatenated value of item embedding and item meta embedding 
 
         Args :
-            page_in: input sequence
-            item_in: input sequence
+            page_in: page input sequence
+            item_in: item input sequence
+            item_meta_in: item deep meta data input sequence
             vl_in: valid length of input data
+            page_meta_in: page deep meta data input sequence
+            page_meta_wide_in: page wide meta data input sequence
+            item_meta_wide_in: item wide meta data input sequence
 
         Return :
             Parallel transformer output
 
         Shape :
             page_in: [batch_size, seq_len]
+            page_meta_in: [batch_size, seq_len]
+            page_meta_wide_in: [batch_size, num_page_meta_wide, seq_len]
             item_in: [batch_size, seq_len]
             item_meta_in: [batch_size, seq_len]
+            item_meta_wide_in: [batch_size, num_item_meta_wide, seq_len]
             vl_in: [batch_size]
 
             out: [batch_size, seq_embed_dim]
         """
         page_embed_out = self.page_embedding(page_in.long())
         item_embed_out = self.item_embedding(item_in.long())
-        item_pre_embed_out = self.item_pre_embedding(item_in.long())
-        item_meta_embed_out = self.item_meta_embedding(item_meta_in.long())
-        item_full_out = torch.cat((item_embed_out, item_meta_embed_out, item_pre_embed_out), 2)
-#         aux_loss = 0
-        x = torch.mul(page_embed_out, item_full_out)
-#         x = torch.cat((page_embed_out, item_embed_out), 2)
+        
+        if page_meta_in is not None:
+            page_meta_embed_out = self.page_meta_embedding(page_meta_in.long()) 
+        if item_meta_in is not None:
+            item_meta_embed_out = self.item_meta_embedding(item_meta_in.long()) 
+            item_pre_embed_out = self.item_pre_embedding(item_in.long())
+        
+        if page_meta_wide_in is not None:
+            page_meta_wide_in_list = [wide_i.float() for wide_i in page_meta_wide_in]
+            page_meta_wide_cat = torch.stack(page_meta_wide_in_list, dim=0)
+            if self.num_page_meta_wide > 1:
+                page_meta_wide_out_norm = self.page_meta_wide_batch_norm(page_meta_wide_cat) 
+            else:
+                page_meta_wide_out_norm = page_meta_wide_cat
+            page_meta_wide_out_norm = torch.permute(page_meta_wide_out_norm, (0,2,1))
+            page_meta_wide_out_norm = self.page_meta_wide_dense(page_meta_wide_out_norm)
+            page_meta_wide_out_norm = self.page_meta_wide_act(page_meta_wide_out_norm)
+            if page_meta_in is not None:
+                page_full_out = torch.cat((page_embed_out, page_meta_embed_out, page_meta_wide_out_norm), 2)
+            else:
+                page_full_out = torch.cat((page_embed_out, page_meta_wide_out_norm), 2)
+        else:
+            if page_meta_in is not None:
+                page_full_out = torch.cat((page_embed_out, page_meta_embed_out), 2)
+            else:
+                page_full_out = page_embed_out
+            
+        if item_meta_wide_in is not None:
+            item_meta_wide_in_list = [wide_i.float() for wide_i in item_meta_wide_in]
+            item_meta_wide_cat = torch.stack(item_meta_wide_in_list, dim=0)
+            if self.num_item_meta_wide > 1:
+                item_meta_wide_out_norm = self.item_meta_wide_batch_norm(item_meta_wide_cat) 
+            else:
+                item_meta_wide_out_norm = item_meta_wide_cat
+            item_meta_wide_out_norm = torch.permute(item_meta_wide_out_norm, (0,2,1))
+            item_meta_wide_out_norm = self.item_meta_wide_dense(item_meta_wide_out_norm)
+            item_meta_wide_out_norm = self.item_meta_wide_act(item_meta_wide_out_norm)
+            if item_meta_in is not None:
+                item_full_out = torch.cat((item_embed_out, item_meta_embed_out, item_pre_embed_out, item_meta_wide_out_norm), 2)
+            else:
+                item_full_out = torch.cat((item_embed_out, item_meta_wide_out_norm), 2)
+        else:
+            if item_meta_in is not None:
+                item_full_out = torch.cat((item_embed_out, item_meta_embed_out, item_pre_embed_out), 2)
+            else: 
+                item_full_out = item_embed_out
+          
+        x = torch.mul(page_full_out, item_full_out)
         for i in range(self.num_layers):
             x = self.ptransformer[i](x, vl_in)
-#             x, aux_loss = self.ptransformer[i](x, vl_in)
-#             aux_loss += aux_loss
 
         out = self.seq_pooling_dp(x)
         out = self.seq_dense(out)        
         return out
 
-class ParallelTransformerAEP3(nn.Module):
+
+class ParallelTransformerAEP2S(nn.Module):
     """
-    Parallel Transformer Adobe Enterprise Product : Instantiates Parallel Transformer Block
-    Concatenate item meta-feature embeddings, pred-trained visual embeddings, item-id embeddings, and item meta wide features as item full embeddings.
-    Sequence of page embeddings and item full embeddings are multiplied and passed through the parallel transformer encoder layers.
+    Parallel Transformer Adobe Enterprise Product: Instantiates Mean Max Pooling, Linear Transformation layer
+    and Parallel Transformer Block
+    Sequence of page embeddings and item embeddings are multiplied and passed through the parallel transformer encoder layers.
 
     Args :
-        page_embedding : the page field embeddings 
+        page_embedding : the page field embeddings
         item_embedding : the item embeddings
-        item_meta_embedding : item meta data embeddings
-        item_meta_wide_in: item meta wide data 
         dim : the dimension size
         dim_head : dimensions of multihead attention network
         heads : no of multi-head attention required
         num_layers : number of hidden layers needed
         ff_mult : feedforward multi
         seq_pooling_dropout :  the pooling dropout value (default=0.0).
-        
+
     Examples::
-        >>> import torch 
+        >>> import torch
         >>> from torch import nn
-        >>> from vz_recommender.models.transformer import ParallelTransformerAEP3
+        >>> from vz_recommender.models.transformer import ParallelTransformerAEP2S
         >>> page_embedding = nn.Embedding(4, 32)
-        >>> item_embedding = nn.Embedding(6, 20)
-        >>> item_meta_embedding = nn.Embedding(8, 4)
-        >>> item_pre_embedding =  nn.Embedding(6, 4)
-        >>> num_meta_wide = 2
-        >>> item_meta_wide_embed_dim = 4
-        >>> transformer_model = ParallelTransformerAEP3(page_embedding=page_embedding, item_embedding=item_embedding, item_meta_embedding=item_meta_embedding, item_pre_embedding=item_pre_embedding, num_meta_wide = num_meta_wide, item_meta_wide_embed_dim = item_meta_wide_embed_dim, dim=32, dim_head=32, heads=2, num_layers=2, ff_mult=4, seq_pooling_dropout=0.0)
+        >>> item_embedding = nn.Embedding(6, 32)
+        >>> transformer_model = ParallelTransformerAEP2S(page_embedding=page_embedding, item_embedding=item_embedding, dim=32, dim_head=32, heads=2, num_layers=2, ff_mult=4, seq_pooling_dropout=0.0)
         >>> page_in = torch.randint(4, (3,5))
         >>> item_in = torch.randint(6, (3,5))
-        >>> item_meta_in = torch.randint(8, (3,5))
-        >>> item_meta_wide_in =torch.rand(3,2,5)
         >>> vl_in = torch.randint(1, 4, (3,))
-        >>> out = transformer_model(page_in, item_in, item_meta_in, vl_in, item_meta_wide_in)
+        >>> out = transformer_model(page_in, item_in, vl_in)
     """
-    def __init__(self, page_embedding, item_embedding, item_meta_embedding, item_pre_embedding, dim, dim_head, heads, num_layers, num_meta_wide=0, item_meta_wide_embed_dim=0, ff_mult=4, seq_pooling_dropout=0.0, moe_kwargs=None):
+
+    def __init__(self, page_embedding, item_embedding, dim, dim_head, heads, num_layers, ff_mult=4,
+                 seq_pooling_dropout=0.0, moe_kwargs=None):
         super().__init__()
         self.page_embedding = page_embedding
         self.item_embedding = item_embedding
-        self.item_meta_embedding = item_meta_embedding
-        self.item_pre_embedding = item_pre_embedding
-        if num_meta_wide>0:
-            self.wide_meta_batch_norm = nn.BatchNorm1d(num_meta_wide)
-            if item_meta_wide_embed_dim>0:
-                self.wide_meta_dense = nn.Linear(num_meta_wide, item_meta_wide_embed_dim)
-            else:
-                print("There are wide meta features but item_meta_wide_embed_dim is not given!")
-            self.wide_meta_act = nn.LeakyReLU(0.2)
         self.seq_pooling_dp = MeanMaxPooling(dropout=seq_pooling_dropout)
-        self.seq_dense = torch.nn.Linear(2 * dim, dim)  
+        self.seq_dense = torch.nn.Linear(2 * dim, dim)
         self.num_layers = num_layers
-        
+        #         self.ptransformer = nn.ModuleList([
+        #             ParallelTransformerBlock(dim=dim, dim_head=dim_head, heads=heads, ff_mult=ff_mult, moe_kwargs=moe_kwargs)
+        #             for _ in range(self.num_layers)
+        #         ])
+
         self.ptransformer = nn.ModuleList([
-            Residual(ParallelTransformerBlock(dim=dim, dim_head=dim_head, heads=heads, ff_mult=ff_mult, moe_kwargs=moe_kwargs))
+            Residual(ParallelTransformerBlock(dim=dim, dim_head=dim_head, heads=heads, ff_mult=ff_mult,
+                                              moe_kwargs=moe_kwargs))
             for _ in range(self.num_layers)
         ])
-        
-    def forward(self, page_in, item_in, item_meta_in, vl_in, item_meta_wide_in = None):
+
+    def forward(self, page_in, item_in, vl_in):
         """
-        Applies Parallel transformer on the page embedding and concatenated value of item embedding and item meta embedding 
+        Takes in item and page embedding and applies Parallel transformer
 
         Args :
             page_in: input sequence
             item_in: input sequence
-            item_meta_in: input sequence
-            item_meta_wide_in: input sequence
             vl_in: valid length of input data
 
         Return :
             Parallel transformer output
 
-        Shape :
-            page_in: [batch_size, seq_len]
-            item_in: [batch_size, seq_len]
-            item_meta_in: [batch_size, seq_len]
-            item_meta_wide_in: [batch_size, num_meta_wide, seq_len]
-            vl_in: [batch_size]
+        Shape: page_in: [batch_size, seq_len]
+               item_in: [batch_size, seq_len]
+               vl_in: [batch_size]
 
-            out: [batch_size, seq_embed_dim]
+               out: [batch_size, seq_embed_dim]
         """
         page_embed_out = self.page_embedding(page_in.long())
         item_embed_out = self.item_embedding(item_in.long())
-        item_pre_embed_out = self.item_pre_embedding(item_in.long())
-        item_meta_embed_out = self.item_meta_embedding(item_meta_in.long())     
-        if item_meta_wide_in is not None:
-            item_meta_wide_in_list =[wide_i.float() for wide_i in item_meta_wide_in]
-            item_meta_wide_cat = torch.stack(item_meta_wide_in_list, dim=0)
-            if item_meta_wide_in.shape[1] > 1:
-                item_meta_wide_out_norm = self.wide_meta_batch_norm(item_meta_wide_cat) 
-            else:
-                item_meta_wide_out_norm = item_meta_wide_cat
-            item_meta_wide_out_norm=torch.permute(item_meta_wide_out_norm, (0,2,1))
-            item_meta_wide_out_norm = self.wide_meta_dense(item_meta_wide_out_norm)
-            item_meta_wide_out_norm = self.wide_meta_act(item_meta_wide_out_norm)
-            item_full_out = torch.cat((item_embed_out, item_meta_embed_out, item_pre_embed_out, item_meta_wide_out_norm), 2)
-        else:
-            item_full_out = torch.cat((item_embed_out, item_meta_embed_out, item_pre_embed_out), 2)
-          
-        x = torch.mul(page_embed_out, item_full_out)
+        #         aux_loss = 0
+        x = torch.mul(page_embed_out, item_embed_out)
+        #         x = torch.cat((page_embed_out, item_embed_out), 2)
         for i in range(self.num_layers):
             x = self.ptransformer[i](x, vl_in)
+        #             x, aux_loss = self.ptransformer[i](x, vl_in)
+        #             aux_loss += aux_loss
 
         out = self.seq_pooling_dp(x)
-        out = self.seq_dense(out)        
+        out = self.seq_dense(out)
         return out
-
-
```

### Comparing `vz-recommender-0.4.5/src/vz_recommender/models/txt.py` & `vz-recommender-0.4.6/src/vz_recommender/models/txt.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.5/src/vz_recommender/models/utils.py` & `vz-recommender-0.4.6/src/vz_recommender/models/utils.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.5/src/vz_recommender/utils/callbacks_base.py` & `vz-recommender-0.4.6/src/vz_recommender/utils/callbacks_base.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.5/src/vz_recommender/utils/loggers_base.py` & `vz-recommender-0.4.6/src/vz_recommender/utils/loggers_base.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.5/src/vz_recommender/utils/utils.py` & `vz-recommender-0.4.6/src/vz_recommender/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import json
 import logging
 from datetime import datetime
 import pandas as pd
 import boto3
-import mlflow
+# import mlflow
 import csv
 import torch
 from typing import Optional
 from ..models.utils import FocalLoss
 
 
 def load_params(params_path):
@@ -65,32 +65,32 @@
     r"""Function that computes Focal loss.
 
     See :class:`~torchgeometry.losses.FocalLoss` for details.
     """
     return FocalLoss(alpha, gamma, reduction)(input, target)
 
 
-def model_logging_setup(new_log_path, run_name, model_name, params_flatten):
-    # WandB
-    global wandb_run
-    logger = logging.getLogger()
-    logger.setLevel(logging.DEBUG)
-    logging.basicConfig(
-        filename=new_log_path,
-        level=logging.INFO
-    )
-
-    # MLflow
-    experiment_paths = [e.name for e in mlflow.list_experiments()]
-    experiment_path = f"/MLflow/{model_name}"
-    if experiment_path in experiment_paths:
-        experiment_id = mlflow.get_experiment_by_name(name=experiment_path).experiment_id
-    else:
-        experiment_id = mlflow.create_experiment(name=experiment_path)
-    return logger, experiment_id
+# def model_logging_setup(new_log_path, run_name, model_name, params_flatten):
+#     # WandB
+#     global wandb_run
+#     logger = logging.getLogger()
+#     logger.setLevel(logging.DEBUG)
+#     logging.basicConfig(
+#         filename=new_log_path,
+#         level=logging.INFO
+#     )
+
+#     # MLflow
+#     experiment_paths = [e.name for e in mlflow.list_experiments()]
+#     experiment_path = f"/MLflow/{model_name}"
+#     if experiment_path in experiment_paths:
+#         experiment_id = mlflow.get_experiment_by_name(name=experiment_path).experiment_id
+#     else:
+#         experiment_id = mlflow.create_experiment(name=experiment_path)
+#     return logger, experiment_id
 
 
 class DownloadS3(object):
     def __init__(self, bucket, access_key, access_secret):
         logging.basicConfig(
             format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
             level=logging.INFO,
```

### Comparing `vz-recommender-0.4.5/src/vz_recommender.egg-info/PKG-INFO` & `vz-recommender-0.4.6/src/vz_recommender.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vz-recommender
-Version: 0.4.5
+Version: 0.4.6
 Summary: vz recommender package
 Author: lu
 Author-email: luyang.wang@verizon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `vz-recommender-0.4.5/src/vz_recommender.egg-info/SOURCES.txt` & `vz-recommender-0.4.6/src/vz_recommender.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 src/vz_recommender.egg-info/SOURCES.txt
 src/vz_recommender.egg-info/dependency_links.txt
 src/vz_recommender.egg-info/top_level.txt
 src/vz_recommender/models/__init__.py
 src/vz_recommender/models/ae.py
 src/vz_recommender/models/bst.py
 src/vz_recommender/models/context.py
+src/vz_recommender/models/encoders.py
+src/vz_recommender/models/grec.py
 src/vz_recommender/models/mmoe.py
 src/vz_recommender/models/moe.py
 src/vz_recommender/models/multitask.py
-src/vz_recommender/models/pars.py
 src/vz_recommender/models/transformer.py
 src/vz_recommender/models/txt.py
 src/vz_recommender/models/utils.py
 src/vz_recommender/utils/__init__.py
 src/vz_recommender/utils/callbacks_base.py
 src/vz_recommender/utils/loggers_base.py
 src/vz_recommender/utils/utils.py
```

