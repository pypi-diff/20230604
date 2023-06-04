# Comparing `tmp/pytorch_partial_tagger-0.1.5.tar.gz` & `tmp/pytorch_partial_tagger-0.1.6.tar.gz`

## Comparing `pytorch_partial_tagger-0.1.5.tar` & `pytorch_partial_tagger-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/notebooks/basic.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/__about__.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/embedders.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/matchers.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/recognizer.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/tagger.py
--rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/training.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/utils.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/crf/__init__.py
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/crf/functional.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/crf/nn.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/__init__.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/core.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/batch/__init__.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/batch/core.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/batch/tag.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/batch/text.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/decoders/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/decoders/viterbi.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/encoders/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/encoders/base.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/encoders/linear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/crf/__init__.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/crf/test_functional.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/crf/test_nn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/data/__init__.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/data/test_batch.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/data/test_core.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/LICENSE
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/README.md
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/notebooks/basic.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/__about__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/matchers.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/recognizer.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/tagger.py
+-rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/training.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/utils.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/crf/__init__.py
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/crf/functional.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/crf/nn.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/data/__init__.py
+-rw-r--r--   0        0        0     7700 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/data/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/data/batch/__init__.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/data/batch/tag.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/data/batch/text.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/decoders/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/decoders/viterbi.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/encoders/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/encoders/base.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/src/partial_tagger/encoders/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/helpers.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/test_matchers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/crf/__init__.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/crf/test_functional.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/crf/test_nn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/data/__init__.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/data/test_core.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/tests/data/batch/test_tag.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/README.md
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.6/PKG-INFO
```

### Comparing `pytorch_partial_tagger-0.1.5/.github/workflows/ci.yml` & `pytorch_partial_tagger-0.1.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/.github/workflows/pypi-publish.yml` & `pytorch_partial_tagger-0.1.6/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/notebooks/basic.ipynb` & `pytorch_partial_tagger-0.1.6/notebooks/basic.ipynb`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/matchers.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/matchers.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
         self.__nlp = nlp
 
     def __call__(self, text: str) -> CharBasedTags:
         doc = self.__nlp(text)
         tags = []
         for ent in doc.ents:
             tags.append(Tag(Span(ent.start_char, len(ent.text)), ent.label_))
-        return CharBasedTags(tags, text)
+        return CharBasedTags(tuple(tags), text)
```

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/recognizer.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/recognizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 from typing import cast
 
 import torch
 from torch.utils.data import DataLoader
 
-from .data.batch import Batch, BatchFactory
-from .data.batch.tag import CharBasedTagsCollection
-from .data.batch.text import Texts
+from .data import LabelSet
+from .data.batch.tag import CharBasedTagsBatch, TagFactory
+from .data.batch.text import BaseTokenizer, TextBatch, Texts
 from .tagger import SequenceTagger
 
 
 class Recognizer:
     def __init__(
         self,
         tagger: SequenceTagger,
-        batch_factory: BatchFactory,
+        tokenizer: BaseTokenizer,
+        label_set: LabelSet,
         padding_index: int,
     ):
         self.__tagger = tagger
-        self.__batch_factory = batch_factory
+        self.__tokenizer = tokenizer
+        self.__label_set = label_set
         self.__padding_index = padding_index
 
     def __call__(
         self, texts: Texts, batch_size: int, device: torch.device
-    ) -> CharBasedTagsCollection:
+    ) -> CharBasedTagsBatch:
         dataloader = DataLoader(
             texts,  # type: ignore
-            collate_fn=self.__batch_factory.create,  # type:ignore
+            collate_fn=self.__tokenizer,
             batch_size=batch_size,
             shuffle=False,
         )
 
         tagger = self.__tagger.eval()
 
         predictions = []
-        for batch in dataloader:
-            batch = cast(Batch, batch)
+        for text_batch in dataloader:
+            text_batch = cast(TextBatch, text_batch)
 
             tag_indices = tagger.predict(
-                batch.get_tagger_inputs(device), batch.get_mask(device)
+                text_batch.get_tagger_inputs(device),
+                text_batch.get_mask(device),
             )
 
+            tag_factory = TagFactory(text_batch.tokenized_texts, self.__label_set)
             predictions.extend(
-                batch.create_char_based_tags(tag_indices, self.__padding_index)
+                tag_factory.create_char_based_tags(tag_indices, self.__padding_index)
             )
 
         return tuple(predictions)
```

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/tagger.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/tagger.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,33 +2,28 @@
 
 import torch
 from torch.nn import Module
 
 from .crf.nn import CRF
 from .data.batch.text import TaggerInputs
 from .decoders import ViterbiDecoder
-from .embedders import BaseEmbedder
 from .encoders import BaseEncoder
 
 
 class SequenceTagger(Module):
     """Sequence tagger.
 
     Args:
-        embedder: An embedder.
         encoder: An encoder.
         decoder: A decoder.
     """
 
-    def __init__(
-        self, embedder: BaseEmbedder, encoder: BaseEncoder, decoder: ViterbiDecoder
-    ):
+    def __init__(self, encoder: BaseEncoder, decoder: ViterbiDecoder):
         super(SequenceTagger, self).__init__()
 
-        self.embedder = embedder
         self.encoder = encoder
         self.crf = CRF(encoder.get_hidden_size())
         self.decoder = decoder
 
     def forward(
         self, inputs: TaggerInputs, mask: torch.Tensor
     ) -> tuple[torch.Tensor, torch.Tensor]:
@@ -40,14 +35,13 @@
 
         Returns:
             A pair of a [batch_size, sequence_length, num_tags, num_tags] float tensor
             and a [batch_size, sequence_length] integer tensor.
             The float tensor representing log potentials and
             the integer tensor representing tag sequence.
         """
-        embeddings = self.embedder(inputs)
-        log_potentials = self.crf(self.encoder(embeddings, mask), mask)
+        log_potentials = self.crf(self.encoder(inputs), mask)
         tag_indices = self.decoder(log_potentials, mask)
         return log_potentials, tag_indices
 
     def predict(self, inputs: TaggerInputs, mask: torch.Tensor) -> torch.Tensor:
         return self(inputs, mask)[1]
```

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/training.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/training.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from logging import Logger
 from typing import cast
 
 import torch
 from torch.utils.data import DataLoader
 
 from .crf import functional as F
-from .data import LabelSet
-from .data.batch import Batch, Dataset
-from .data.batch.tag import CharBasedTagsCollection
+from .data import Dataset, LabelSet
+from .data.batch.tag import CharBasedTagsBatch, TagFactory
+from .data.batch.text import TextBatch
+from .encoders.transformer import EncoderType
 from .recognizer import Recognizer
-from .utils import Metric, create_collator, create_tagger
+from .utils import Collator, Metric, create_tagger, create_tokenizer
 
 
 class SlantedTriangular:
     def __init__(self, max_steps: int, cut_frac: float = 0.1, ratio: int = 16):
         self.__cut_frac = cut_frac
         self.__cut = int(max_steps * cut_frac)
         self.__ratio = ratio
@@ -71,23 +72,25 @@
         batch_size: int = 15,
         num_epochs: int = 20,
         learning_rate: float = 2e-5,
         gradient_clip_value: float = 5.0,
         padding_index: int = -1,
         unknown_index: int = -100,
         tokenizer_args: dict | None = None,
+        encoder_type: EncoderType = "default",
     ):
         self.__model_name = model_name
         self.__batch_size = batch_size
         self.__num_epochs = num_epochs
         self.__learning_rate = learning_rate
         self.__gradient_clip_value = gradient_clip_value
         self.__padding_index = padding_index
         self.__unknown_index = unknown_index
         self.__tokenizer_args = tokenizer_args
+        self.__encoder_type = encoder_type
 
     def __call__(
         self,
         train_dataset: Dataset,
         validation_dataset: Dataset,
         device: torch.device,
         logger: Logger | None = None,
@@ -102,19 +105,22 @@
         for _, tags in train_dataset:
             for tag in tags:
                 if tag.label not in labels:
                     labels.add(tag.label)
         label_set = LabelSet(labels)
 
         # Create a tagger
-        tagger = create_tagger(self.__model_name, label_set, self.__padding_index)
+        tagger = create_tagger(
+            self.__model_name, label_set, self.__padding_index, self.__encoder_type
+        )
         tagger.to(device)
 
         # Create a collator
-        collator = create_collator(self.__model_name, label_set, self.__tokenizer_args)
+        tokenizer = create_tokenizer(self.__model_name, self.__tokenizer_args)
+        collator = Collator(tokenizer)
 
         train_dataloader = DataLoader(
             train_dataset,  # type:ignore
             collate_fn=collator,
             batch_size=self.__batch_size,
         )
         validation_dataloader = DataLoader(
@@ -127,67 +133,69 @@
         optimizer = torch.optim.Adam(
             tagger.parameters(), lr=self.__learning_rate, weight_decay=0.0
         )
         schedular = torch.optim.lr_scheduler.LambdaLR(
             optimizer,
             SlantedTriangular(len(train_dataloader) * self.__num_epochs),
         )
-        best_f1_score = 0.0
+        best_f1_score = float("-inf")
         best_tagger_state = io.BytesIO()
 
         for epoch in range(1, self.__num_epochs + 1):
             epoch_loss = 0.0
             tagger.train()
 
-            for batch, ground_truths in train_dataloader:
-                batch = cast(Batch, batch)
-                ground_truths = cast(CharBasedTagsCollection, ground_truths)
+            for text_batch, tags_batch in train_dataloader:
+                text_batch = cast(TextBatch, text_batch)
+                tags_batch = cast(CharBasedTagsBatch, tags_batch)
 
                 optimizer.zero_grad()
 
-                log_potentials, _ = tagger(
-                    batch.get_tagger_inputs(device), batch.get_mask(device)
-                )
+                mask = text_batch.get_mask(device)
+                log_potentials, _ = tagger(text_batch.get_tagger_inputs(device), mask)
 
-                tags_bitmap = batch.create_tag_bitmap(
-                    ground_truths, device, self.__padding_index, self.__unknown_index
+                tag_factory = TagFactory(text_batch.tokenized_texts, label_set)
+                tags_bitmap = tag_factory.create_tag_bitmap(
+                    tags_batch, device, self.__padding_index, self.__unknown_index
                 )
 
                 loss = expected_entity_ratio_loss(
                     log_potentials,
                     tags_bitmap,
-                    batch.get_mask(device),
+                    mask,
                     label_set.get_outside_index(),
                 )
                 loss.backward()
 
                 torch.nn.utils.clip_grad_value_(
                     tagger.parameters(), clip_value=self.__gradient_clip_value
                 )
 
                 optimizer.step()
                 schedular.step()
 
-                epoch_loss += loss.item() * batch.size
+                epoch_loss += loss.item() * text_batch.size
 
             tagger.eval()
             metric = Metric()
-            for batch, ground_truths in validation_dataloader:
-                batch = cast(Batch, batch)
-                ground_truths = cast(CharBasedTagsCollection, ground_truths)
+            for text_batch, tags_batch in validation_dataloader:
+                text_batch = cast(TextBatch, text_batch)
+                tags_batch = cast(CharBasedTagsBatch, tags_batch)
 
                 tag_indices = tagger.predict(
-                    batch.get_tagger_inputs(device), batch.get_mask(device)
+                    text_batch.get_tagger_inputs(device),
+                    text_batch.get_mask(device),
                 )
 
-                predictions = batch.create_char_based_tags(
+                tag_factory = TagFactory(text_batch.tokenized_texts, label_set)
+                predictions = tag_factory.create_char_based_tags(
                     tag_indices, self.__padding_index
                 )
 
-                metric(predictions, ground_truths)
+                metric(predictions, tags_batch)
 
             scores = metric.get_scores()
 
             if best_f1_score < scores["f1_score"]:
                 best_f1_score = scores["f1_score"]
                 best_tagger_state.truncate(0)
                 best_tagger_state.seek(0)
@@ -200,8 +208,8 @@
                     **{f"validation_{key}": value for key, value in scores.items()},
                 }
             )
 
         best_tagger_state.seek(0)
         tagger.load_state_dict(torch.load(best_tagger_state))
 
-        return Recognizer(tagger, collator.batch_factory, self.__padding_index)
+        return Recognizer(tagger, tokenizer, label_set, self.__padding_index)
```

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/crf/functional.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/crf/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/crf/nn.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/crf/nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/data/core.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/data/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         return Span(
             char_span_start.start,
             char_span_end.start + char_span_end.length - char_span_start.start,
         )
 
 
 @dataclass(frozen=True)
-class SubwordBasedTags:
+class TokenBasedTags:
     tags: tuple[Tag, ...]
     tokenized_text: TokenizedText
 
     def __iter__(self) -> Iterator[Tag]:
         yield from self.tags
 
     def __repr__(self) -> str:
```

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/data/batch/tag.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/data/batch/tag.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 from itertools import groupby
 from typing import Tuple
 
 import torch
 
 from ...crf.functional import to_tag_bitmap
-from .. import CharBasedTags, LabelSet, Span, SubwordBasedTags, Tag, TokenizedText
+from .. import CharBasedTags, LabelSet, Span, Tag, TokenBasedTags, TokenizedText
 
 # https://bugs.python.org/issue45117
 # type alias for tuple, dict, list is no longer supported in py38.
-CharBasedTagsCollection = Tuple[CharBasedTags, ...]
-SubwordBasedTagsCollection = Tuple[SubwordBasedTags, ...]
+CharBasedTagsBatch = Tuple[CharBasedTags, ...]
+TokenBasedTagsBatch = Tuple[TokenBasedTags, ...]
 
 
 def pad(batch: list[list[int]], fill_value: int) -> torch.Tensor:
     max_length = max(map(len, batch))
     return torch.tensor([x + [fill_value] * (max_length - len(x)) for x in batch])
 
 
@@ -26,23 +26,23 @@
 class TagFactory:
     def __init__(self, tokenized_texts: tuple[TokenizedText, ...], label_set: LabelSet):
         self.__tokenized_texts = tokenized_texts
         self.__label_set = label_set
 
     def create_char_based_tags(
         self, tag_indices: torch.Tensor, padding_index: int = -1
-    ) -> CharBasedTagsCollection:
+    ) -> CharBasedTagsBatch:
         return tuple(
             tags.get_char_based_tags()
-            for tags in self.create_subword_based_tags(tag_indices, padding_index)
+            for tags in self.create_token_based_tags(tag_indices, padding_index)
         )
 
-    def create_subword_based_tags(
+    def create_token_based_tags(
         self, tag_indices: torch.Tensor, padding_index: int = -1
-    ) -> SubwordBasedTagsCollection:
+    ) -> TokenBasedTagsBatch:
         label_set = self.__label_set
 
         batched_tags = []
 
         for text, indices in zip(
             self.__tokenized_texts, unpad(tag_indices, padding_index)
         ):
@@ -54,29 +54,29 @@
                 length = len(list(group))
 
                 if label is not None:
                     tags.append(Tag(Span(now, length), label))
 
                 now += length
 
-            batched_tags.append(SubwordBasedTags(tuple(tags), text))
+            batched_tags.append(TokenBasedTags(tuple(tags), text))
 
         return tuple(batched_tags)
 
     def create_tag_indices(
         self,
-        tags_collection: CharBasedTagsCollection,
+        tags_batch: CharBasedTagsBatch,
         device: torch.device,
         padding_index: int = -1,
         unknown_index: int = -100,
     ) -> torch.Tensor:
         tag_indices = []
         label_set = self.__label_set
 
-        for text, tags in zip(self.__tokenized_texts, tags_collection):
+        for text, tags in zip(self.__tokenized_texts, tags_batch):
             indices = [unknown_index] * text.num_tokens
 
             for token_index in range(text.num_tokens):
                 span = text.get_char_span(token_index)
                 if span is None:
                     indices[token_index] = label_set.get_outside_index()
 
@@ -94,18 +94,18 @@
 
             tag_indices.append(indices)
 
         return pad(tag_indices, padding_index).to(device)
 
     def create_tag_bitmap(
         self,
-        tags_collection: CharBasedTagsCollection,
+        tags_batch: CharBasedTagsBatch,
         device: torch.device,
         padding_index: int = -1,
         unknown_index: int = -100,
     ) -> torch.Tensor:
         tag_indices = self.create_tag_indices(
-            tags_collection, device, padding_index, unknown_index
+            tags_batch, device, padding_index, unknown_index
         )
         return to_tag_bitmap(
             tag_indices, self.__label_set.get_tag_size(), unknown_index
         )
```

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/data/batch/text.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/data/batch/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ..core import Span, TokenizedText
 
 Texts = Tuple[str, ...]
 TaggerInputs = Dict[str, torch.Tensor]
 
 
-class TokenizedTexts:
+class TextBatch:
     def __init__(
         self,
         tokenized_texts: tuple[TokenizedText, ...],
         tagger_inputs: TaggerInputs,
         mask: torch.Tensor,
     ):
         self.tokenized_texts = tokenized_texts
@@ -32,15 +32,15 @@
 
     def get_mask(self, device: torch.device) -> torch.Tensor:
         return self.__mask.to(device)
 
 
 class BaseTokenizer(metaclass=ABCMeta):
     @abstractmethod
-    def __call__(self, texts: Texts) -> TokenizedTexts:
+    def __call__(self, texts: Texts) -> TextBatch:
         raise NotImplementedError
 
 
 class TransformerTokenizer(BaseTokenizer):
     def __init__(
         self,
         tokenizer: PreTrainedTokenizer,
@@ -53,15 +53,15 @@
 
         self.__tokenizer_args = tokenizer_args or {
             "padding": True,
             "return_tensors": "pt",
         }
         self.__tokenizer_args["return_offsets_mapping"] = True
 
-    def __call__(self, texts: Texts) -> TokenizedTexts:
+    def __call__(self, texts: Texts) -> TextBatch:
         batch_encoding = self.__tokenizer(texts, **self.__tokenizer_args)
 
         mappings = batch_encoding.pop("offset_mapping").tolist()
         pad_token_id = self.__tokenizer.pad_token_id
         tokenized_text_lengths = (batch_encoding.input_ids != pad_token_id).sum(dim=1)
 
         tokenized_texts = []
@@ -85,8 +85,8 @@
             )
 
         lengths = [text.num_tokens for text in tokenized_texts]
         max_length = max(lengths)
         mask = torch.tensor(
             [[True] * length + [False] * (max_length - length) for length in lengths]
         )
-        return TokenizedTexts(tuple(tokenized_texts), batch_encoding, mask)
+        return TextBatch(tuple(tokenized_texts), batch_encoding, mask)
```

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/decoders/viterbi.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/decoders/viterbi.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/src/partial_tagger/encoders/base.py` & `pytorch_partial_tagger-0.1.6/src/partial_tagger/encoders/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from abc import ABCMeta, abstractmethod
 
 import torch
 from torch.nn import Module
 
+from ..data.batch.text import TaggerInputs
+
 
 class BaseEncoder(Module, metaclass=ABCMeta):
     """Base class of all encoders."""
 
     @abstractmethod
-    def forward(self, embeddings: torch.Tensor, mask: torch.Tensor) -> torch.Tensor:
-        """Encode the given embeddings to a tensor.
+    def forward(self, inputs: TaggerInputs) -> torch.Tensor:
+        """Encode the given inputs to a tensor.
 
         Args:
-            embeddings: A [batch_size, sequence_length, embedding_size] float tensor.
-            mask: A [batch_size, sequence_length] boolean tensor.
+            inputs: A dictionary that maps a string key to a tensor value.
 
         Returns:
             A [batch_size, sequence_length, hidden_size] float tensor.
         """
         raise NotImplementedError
 
     @abstractmethod
```

### Comparing `pytorch_partial_tagger-0.1.5/tests/conftest.py` & `pytorch_partial_tagger-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/tests/helpers.py` & `pytorch_partial_tagger-0.1.6/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/tests/crf/test_functional.py` & `pytorch_partial_tagger-0.1.6/tests/crf/test_functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/tests/crf/test_nn.py` & `pytorch_partial_tagger-0.1.6/tests/crf/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/tests/data/test_core.py` & `pytorch_partial_tagger-0.1.6/tests/data/test_core.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/.gitignore` & `pytorch_partial_tagger-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/LICENSE` & `pytorch_partial_tagger-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/README.md` & `pytorch_partial_tagger-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.5/pyproject.toml` & `pytorch_partial_tagger-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 description = "Sequence Tagger for Partially Annotated Dataset in PyTorch"
 authors = [
     {name = "Yasufumi Taniguchi", email = "yasufumi.taniguchi@gmail.com"},
 ]
 dependencies = [
     "transformers>=4.29.2",
     "torch>=2.0.1",
+    "spacy>=3.5.3",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {text = "MIT"}
 dynamic = ["version"]
 classifiers = [
     "Programming Language :: Python",
```

### Comparing `pytorch_partial_tagger-0.1.5/PKG-INFO` & `pytorch_partial_tagger-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pytorch-partial-tagger
-Version: 0.1.5
+Version: 0.1.6
 Summary: Sequence Tagger for Partially Annotated Dataset in PyTorch
 Project-URL: Homepage, https://github.com/yasufumy/pytorch-partial-tagger
 Author-email: Yasufumi Taniguchi <yasufumi.taniguchi@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: spacy>=3.5.3
 Requires-Dist: torch>=2.0.1
 Requires-Dist: transformers>=4.29.2
 Provides-Extra: dev
 Requires-Dist: black>=23.3.0; extra == 'dev'
 Requires-Dist: mypy>=1.3.0; extra == 'dev'
 Requires-Dist: pytest-cov>=4.1.0; extra == 'dev'
 Requires-Dist: pytest>=7.3.1; extra == 'dev'
```

