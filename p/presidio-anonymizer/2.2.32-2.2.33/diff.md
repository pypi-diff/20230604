# Comparing `tmp/presidio_anonymizer-2.2.32-py3-none-any.whl.zip` & `tmp/presidio_anonymizer-2.2.33-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,35 +1,38 @@
-Zip file size: 26237 bytes, number of entries: 33
--rw-r--r--  2.0 unx      319 b- defN 23-Jan-31 19:53 presidio_anonymizer/__init__.py
--rw-r--r--  2.0 unx     6538 b- defN 23-Jan-31 19:53 presidio_anonymizer/anonymizer_engine.py
--rw-r--r--  2.0 unx     1374 b- defN 23-Jan-31 19:53 presidio_anonymizer/deanonymize_engine.py
--rw-r--r--  2.0 unx      172 b- defN 23-Jan-31 19:53 presidio_anonymizer/core/__init__.py
--rw-r--r--  2.0 unx     4197 b- defN 23-Jan-31 19:53 presidio_anonymizer/core/engine_base.py
--rw-r--r--  2.0 unx     2263 b- defN 23-Jan-31 19:53 presidio_anonymizer/core/text_replace_builder.py
--rw-r--r--  2.0 unx      529 b- defN 23-Jan-31 19:53 presidio_anonymizer/entities/__init__.py
--rw-r--r--  2.0 unx      332 b- defN 23-Jan-31 19:53 presidio_anonymizer/entities/invalid_exception.py
--rw-r--r--  2.0 unx      220 b- defN 23-Jan-31 19:53 presidio_anonymizer/entities/engine/__init__.py
--rw-r--r--  2.0 unx     1717 b- defN 23-Jan-31 19:53 presidio_anonymizer/entities/engine/operator_config.py
--rw-r--r--  2.0 unx     1916 b- defN 23-Jan-31 19:53 presidio_anonymizer/entities/engine/pii_entity.py
--rw-r--r--  2.0 unx     4170 b- defN 23-Jan-31 19:53 presidio_anonymizer/entities/engine/recognizer_result.py
--rw-r--r--  2.0 unx      200 b- defN 23-Jan-31 19:53 presidio_anonymizer/entities/engine/result/__init__.py
--rw-r--r--  2.0 unx     1857 b- defN 23-Jan-31 19:53 presidio_anonymizer/entities/engine/result/engine_result.py
--rw-r--r--  2.0 unx     2025 b- defN 23-Jan-31 19:53 presidio_anonymizer/entities/engine/result/operator_result.py
--rw-r--r--  2.0 unx      552 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/__init__.py
--rw-r--r--  2.0 unx     1701 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/aes_cipher.py
--rw-r--r--  2.0 unx     1273 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/custom.py
--rw-r--r--  2.0 unx     1752 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/decrypt.py
--rw-r--r--  2.0 unx     1740 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/encrypt.py
--rw-r--r--  2.0 unx     1564 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/hash.py
--rw-r--r--  2.0 unx     2700 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/mask.py
--rw-r--r--  2.0 unx      972 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/operator.py
--rw-r--r--  2.0 unx     2822 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/operators_factory.py
--rw-r--r--  2.0 unx      704 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/redact.py
--rw-r--r--  2.0 unx      981 b- defN 23-Jan-31 19:53 presidio_anonymizer/operators/replace.py
--rw-r--r--  2.0 unx       21 b- defN 23-Jan-31 19:53 presidio_anonymizer/services/__init__.py
--rw-r--r--  2.0 unx     2225 b- defN 23-Jan-31 19:53 presidio_anonymizer/services/app_entities_convertor.py
--rw-r--r--  2.0 unx     3273 b- defN 23-Jan-31 19:53 presidio_anonymizer/services/validators.py
--rw-r--r--  2.0 unx     7992 b- defN 23-Jan-31 19:53 presidio_anonymizer-2.2.32.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-31 19:53 presidio_anonymizer-2.2.32.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jan-31 19:53 presidio_anonymizer-2.2.32.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3278 b- defN 23-Jan-31 19:53 presidio_anonymizer-2.2.32.dist-info/RECORD
-33 files, 61491 bytes uncompressed, 20773 bytes compressed:  66.2%
+Zip file size: 28554 bytes, number of entries: 36
+-rw-r--r--  2.0 unx      403 b- defN 23-Jun-04 10:03 presidio_anonymizer/__init__.py
+-rw-r--r--  2.0 unx     6562 b- defN 23-Jun-04 10:03 presidio_anonymizer/anonymizer_engine.py
+-rw-r--r--  2.0 unx     3318 b- defN 23-Jun-04 10:03 presidio_anonymizer/batch_anonymizer_engine.py
+-rw-r--r--  2.0 unx     1374 b- defN 23-Jun-04 10:03 presidio_anonymizer/deanonymize_engine.py
+-rw-r--r--  2.0 unx      172 b- defN 23-Jun-04 10:03 presidio_anonymizer/core/__init__.py
+-rw-r--r--  2.0 unx     4197 b- defN 23-Jun-04 10:03 presidio_anonymizer/core/engine_base.py
+-rw-r--r--  2.0 unx     2263 b- defN 23-Jun-04 10:03 presidio_anonymizer/core/text_replace_builder.py
+-rw-r--r--  2.0 unx      621 b- defN 23-Jun-04 10:03 presidio_anonymizer/entities/__init__.py
+-rw-r--r--  2.0 unx      332 b- defN 23-Jun-04 10:03 presidio_anonymizer/entities/invalid_exception.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-04 10:03 presidio_anonymizer/entities/engine/__init__.py
+-rw-r--r--  2.0 unx     1044 b- defN 23-Jun-04 10:03 presidio_anonymizer/entities/engine/dict_recognizer_result.py
+-rw-r--r--  2.0 unx     1717 b- defN 23-Jun-04 10:03 presidio_anonymizer/entities/engine/operator_config.py
+-rw-r--r--  2.0 unx     1916 b- defN 23-Jun-04 10:03 presidio_anonymizer/entities/engine/pii_entity.py
+-rw-r--r--  2.0 unx     4170 b- defN 23-Jun-04 10:03 presidio_anonymizer/entities/engine/recognizer_result.py
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-04 10:03 presidio_anonymizer/entities/engine/result/__init__.py
+-rw-r--r--  2.0 unx     1857 b- defN 23-Jun-04 10:03 presidio_anonymizer/entities/engine/result/engine_result.py
+-rw-r--r--  2.0 unx     2025 b- defN 23-Jun-04 10:03 presidio_anonymizer/entities/engine/result/operator_result.py
+-rw-r--r--  2.0 unx      587 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/__init__.py
+-rw-r--r--  2.0 unx     1701 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/aes_cipher.py
+-rw-r--r--  2.0 unx     1273 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/custom.py
+-rw-r--r--  2.0 unx     1752 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/decrypt.py
+-rw-r--r--  2.0 unx     1740 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/encrypt.py
+-rw-r--r--  2.0 unx     1564 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/hash.py
+-rw-r--r--  2.0 unx      834 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/keep.py
+-rw-r--r--  2.0 unx     2700 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/mask.py
+-rw-r--r--  2.0 unx      972 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/operator.py
+-rw-r--r--  2.0 unx     2822 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/operators_factory.py
+-rw-r--r--  2.0 unx      704 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/redact.py
+-rw-r--r--  2.0 unx      981 b- defN 23-Jun-04 10:03 presidio_anonymizer/operators/replace.py
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-04 10:03 presidio_anonymizer/services/__init__.py
+-rw-r--r--  2.0 unx     2225 b- defN 23-Jun-04 10:03 presidio_anonymizer/services/app_entities_convertor.py
+-rw-r--r--  2.0 unx     3273 b- defN 23-Jun-04 10:03 presidio_anonymizer/services/validators.py
+-rw-r--r--  2.0 unx     8043 b- defN 23-Jun-04 10:03 presidio_anonymizer-2.2.33.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 10:03 presidio_anonymizer-2.2.33.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-04 10:03 presidio_anonymizer-2.2.33.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3592 b- defN 23-Jun-04 10:03 presidio_anonymizer-2.2.33.dist-info/RECORD
+36 files, 67287 bytes uncompressed, 22574 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: presidio_anonymizer/__init__.py
 Comment: 
 
 Filename: presidio_anonymizer/anonymizer_engine.py
 Comment: 
 
+Filename: presidio_anonymizer/batch_anonymizer_engine.py
+Comment: 
+
 Filename: presidio_anonymizer/deanonymize_engine.py
 Comment: 
 
 Filename: presidio_anonymizer/core/__init__.py
 Comment: 
 
 Filename: presidio_anonymizer/core/engine_base.py
@@ -21,14 +24,17 @@
 
 Filename: presidio_anonymizer/entities/invalid_exception.py
 Comment: 
 
 Filename: presidio_anonymizer/entities/engine/__init__.py
 Comment: 
 
+Filename: presidio_anonymizer/entities/engine/dict_recognizer_result.py
+Comment: 
+
 Filename: presidio_anonymizer/entities/engine/operator_config.py
 Comment: 
 
 Filename: presidio_anonymizer/entities/engine/pii_entity.py
 Comment: 
 
 Filename: presidio_anonymizer/entities/engine/recognizer_result.py
@@ -57,14 +63,17 @@
 
 Filename: presidio_anonymizer/operators/encrypt.py
 Comment: 
 
 Filename: presidio_anonymizer/operators/hash.py
 Comment: 
 
+Filename: presidio_anonymizer/operators/keep.py
+Comment: 
+
 Filename: presidio_anonymizer/operators/mask.py
 Comment: 
 
 Filename: presidio_anonymizer/operators/operator.py
 Comment: 
 
 Filename: presidio_anonymizer/operators/operators_factory.py
@@ -81,20 +90,20 @@
 
 Filename: presidio_anonymizer/services/app_entities_convertor.py
 Comment: 
 
 Filename: presidio_anonymizer/services/validators.py
 Comment: 
 
-Filename: presidio_anonymizer-2.2.32.dist-info/METADATA
+Filename: presidio_anonymizer-2.2.33.dist-info/METADATA
 Comment: 
 
-Filename: presidio_anonymizer-2.2.32.dist-info/WHEEL
+Filename: presidio_anonymizer-2.2.33.dist-info/WHEEL
 Comment: 
 
-Filename: presidio_anonymizer-2.2.32.dist-info/top_level.txt
+Filename: presidio_anonymizer-2.2.33.dist-info/top_level.txt
 Comment: 
 
-Filename: presidio_anonymizer-2.2.32.dist-info/RECORD
+Filename: presidio_anonymizer-2.2.33.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## presidio_anonymizer/__init__.py

```diff
@@ -1,12 +1,13 @@
 """Anonymizer root module."""
 import logging
 
 from .anonymizer_engine import AnonymizerEngine
 from .deanonymize_engine import DeanonymizeEngine
+from .batch_anonymizer_engine import BatchAnonymizerEngine
 
 # Set up default logging (with NullHandler)
 
 
 logging.getLogger("presidio-anonymizer").addHandler(logging.NullHandler())
 
-__all__ = ["AnonymizerEngine", "DeanonymizeEngine"]
+__all__ = ["AnonymizerEngine", "DeanonymizeEngine", "BatchAnonymizerEngine"]
```

## presidio_anonymizer/anonymizer_engine.py

```diff
@@ -1,13 +1,13 @@
 """Handles the entire logic of the Presidio-anonymizer and text anonymizing."""
 import logging
 from typing import List, Dict, Optional
 
-from presidio_anonymizer.entities import OperatorConfig, RecognizerResult, EngineResult
 from presidio_anonymizer.core import EngineBase
+from presidio_anonymizer.entities import OperatorConfig, RecognizerResult, EngineResult
 from presidio_anonymizer.operators import OperatorType
 
 DEFAULT = "replace"
 
 
 class AnonymizerEngine(EngineBase):
     """
@@ -19,18 +19,18 @@
 
     logger = logging.getLogger("presidio-anonymizer")
 
     def __init__(self):
         EngineBase.__init__(self)
 
     def anonymize(
-        self,
-        text: str,
-        analyzer_results: List[RecognizerResult],
-        operators: Optional[Dict[str, OperatorConfig]] = None,
+            self,
+            text: str,
+            analyzer_results: List[RecognizerResult],
+            operators: Optional[Dict[str, OperatorConfig]] = None,
     ) -> EngineResult:
         """Anonymize method to anonymize the given text.
 
         :param text: the text we are anonymizing
         :param analyzer_results: A list of RecognizerResult class -> The results we
         received from the analyzer
         :param operators: The configuration of the anonymizers we would like
@@ -79,15 +79,15 @@
         )
 
         operators = self.__check_or_add_default_operator(operators)
 
         return self._operate(text, analyzer_results, operators, OperatorType.Anonymize)
 
     def _remove_conflicts_and_get_text_manipulation_data(
-        self, analyzer_results: List[RecognizerResult]
+            self, analyzer_results: List[RecognizerResult]
     ) -> List[RecognizerResult]:
         """
         Iterate the list and create a sorted unique results list from it.
 
         Only insert results which are:
         1. Indices are not contained in other result.
         2. Have the same indices as other results but with larger score.
@@ -148,15 +148,15 @@
     def __is_result_conflicted_with_other_elements(other_elements, result):
         return any(
             [result.has_conflict(other_element) for other_element in other_elements]
         )
 
     @staticmethod
     def __check_or_add_default_operator(
-        operators: Dict[str, OperatorConfig]
+            operators: Dict[str, OperatorConfig]
     ) -> Dict[str, OperatorConfig]:
         default_operator = OperatorConfig(DEFAULT)
         if not operators:
             return {"DEFAULT": default_operator}
         if not operators.get("DEFAULT"):
             operators["DEFAULT"] = default_operator
         return operators
```

## presidio_anonymizer/entities/__init__.py

```diff
@@ -1,16 +1,18 @@
 """Handles all the entities objects (structs) of the anonymizer."""
 from .invalid_exception import InvalidParamException
 from .engine.pii_entity import PIIEntity
 from .engine.operator_config import OperatorConfig
 from .engine.recognizer_result import RecognizerResult
 from .engine.result.engine_result import EngineResult
 from .engine.result.operator_result import OperatorResult
+from .engine.dict_recognizer_result import DictRecognizerResult
 
 __all__ = [
     "InvalidParamException",
     "PIIEntity",
     "OperatorConfig",
     "OperatorResult",
     "RecognizerResult",
     "EngineResult",
+    "DictRecognizerResult",
 ]
```

## presidio_anonymizer/operators/__init__.py

```diff
@@ -1,25 +1,27 @@
 """Initializing all the existing anonymizers."""
 from .operator import OperatorType, Operator
 from .hash import Hash
 from .mask import Mask
 from .redact import Redact
 from .replace import Replace
 from .custom import Custom
+from .keep import Keep
 from .encrypt import Encrypt
 from .decrypt import Decrypt
 from .aes_cipher import AESCipher
 from .operators_factory import OperatorsFactory
 
 __all__ = [
     "OperatorType",
     "Operator",
     "Hash",
     "Mask",
     "Redact",
+    "Keep",
     "Replace",
     "Custom",
     "Encrypt",
     "Decrypt",
     "AESCipher",
     "OperatorsFactory",
 ]
```

## Comparing `presidio_anonymizer-2.2.32.dist-info/METADATA` & `presidio_anonymizer-2.2.33.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: presidio-anonymizer
-Version: 2.2.32
+Version: 2.2.33
 Summary: Persidio Anonymizer package - replaces analyzed text with desired values.
 Home-page: https://github.com/microsoft/presidio
 License: MIT license
 Keywords: presidio_anonymizer
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Requires-Dist: pycryptodome (>=3.10.1)
 
 # Presidio anonymizer
 
 ## Description
```

## Comparing `presidio_anonymizer-2.2.32.dist-info/RECORD` & `presidio_anonymizer-2.2.33.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-presidio_anonymizer/__init__.py,sha256=zczimX5sfpQw3deQHCza02qYmGSt0swrZKGd1cknTWo,319
-presidio_anonymizer/anonymizer_engine.py,sha256=BkmCqfcD8qKwsmZM2pB0Yw-MDHBYNOBmoQ5k1lQo6pI,6538
+presidio_anonymizer/__init__.py,sha256=JIdbYfomE4hGEWPu_xzvKdXqV9OfPqqa1XLt-hKbE-I,403
+presidio_anonymizer/anonymizer_engine.py,sha256=3OYmz4lmUsn0m5nsKHc7ji6tyXe68OUe57X03E33I1k,6562
+presidio_anonymizer/batch_anonymizer_engine.py,sha256=jSVyMzc8KZxu6SBbWSqtIcwizWem6FSKMhFDcpz_Cso,3318
 presidio_anonymizer/deanonymize_engine.py,sha256=_Q1CyAT1aYHkkuZA5yOv9h1G7DMJcc7CELzCp9hg18c,1374
 presidio_anonymizer/core/__init__.py,sha256=YMFhRmhAE_I0Ak0zoEnv7brsukbjmYlXQwCbK4uR_aA,172
 presidio_anonymizer/core/engine_base.py,sha256=5FpJIcrROIvqFerjLIRY8P6u2ZCYlwqmsfT2B7ZvmqA,4197
 presidio_anonymizer/core/text_replace_builder.py,sha256=ggyzIwZWQJS3eGc7g9TDCWleJzkWi9-FkLWzpA6ZubA,2263
-presidio_anonymizer/entities/__init__.py,sha256=WnDySnQWIjhGfdAw7Qm6kGmAqxSfoc3_0XpV39g8w6s,529
+presidio_anonymizer/entities/__init__.py,sha256=8wbWUCGOSvznrKzYW-65z3mQGSO62rVPRBGf2l2pjN0,621
 presidio_anonymizer/entities/invalid_exception.py,sha256=O7eHDKmeO2TTwa0crmbRHV97pTm9MYIdrq6wHu73iVw,332
 presidio_anonymizer/entities/engine/__init__.py,sha256=51yXaLe1bnxR8nq8-NodxoTxSN-0mdm8uzLCehHZqZ0,220
+presidio_anonymizer/entities/engine/dict_recognizer_result.py,sha256=XTFeg0c7vmYnDHOteJ2CVKSsVycwh5fNJNlqhpXu5wo,1044
 presidio_anonymizer/entities/engine/operator_config.py,sha256=P8cew7OV7WJ2LfcQbkUn_2Gga4Ou9Ks5-y6nJABlnQk,1717
 presidio_anonymizer/entities/engine/pii_entity.py,sha256=IyeNNltAtfmMnsn7Zfn37ENNb_Nw25lxxU3fBsnP6SY,1916
 presidio_anonymizer/entities/engine/recognizer_result.py,sha256=qynP3_BR1tBSuj-A-hxolf5kEvMI86jnWkh6eAZolAE,4170
 presidio_anonymizer/entities/engine/result/__init__.py,sha256=MZ5t99wQK4za5EDPiivapbgehgzXJG-41Ua3Zo-2wpo,200
 presidio_anonymizer/entities/engine/result/engine_result.py,sha256=6qBwCKvuNkKKFXUCvJ_xFxVDSka1XZafKBn_4ywWD5w,1857
 presidio_anonymizer/entities/engine/result/operator_result.py,sha256=q-AytfQPv-ThPwcKBaPgqii1CnUAxwF3QG5sIOcETMs,2025
-presidio_anonymizer/operators/__init__.py,sha256=Zb4cVNY4nKCAe9ylIoEZQGWoPeyxkfTKQRoRl0m1alU,552
+presidio_anonymizer/operators/__init__.py,sha256=BzgyE5IIqzQ1xnSAhSyk25MrBAhk-417-ZMszuqy_yc,587
 presidio_anonymizer/operators/aes_cipher.py,sha256=ojCiP-XcBwOkWOsw6ZnMR0jTr995FU5vXvE_MC1xdg0,1701
 presidio_anonymizer/operators/custom.py,sha256=_uRqPYvuL3WbR2LYk0TIs0efYSEqG-VPmlz1u7Nj358,1273
 presidio_anonymizer/operators/decrypt.py,sha256=1QyDrEO3-BNOSA7ijNUw25w7PdLH90-PQwAgPzm9EBw,1752
 presidio_anonymizer/operators/encrypt.py,sha256=b1MiNx08XdMkOD3cAK2VkPzaRgeEzDz0UYYe1pK2i1c,1740
 presidio_anonymizer/operators/hash.py,sha256=J7Y-U6flVB2uLeMnzlP4A97pkkkdaTqL3c6xUy-qMug,1564
+presidio_anonymizer/operators/keep.py,sha256=edDRAWOvklxaOHlWEytHvcDeiwFxtF9uOlQIblzkf5Q,834
 presidio_anonymizer/operators/mask.py,sha256=q_E0Fl0gMe9wPVB0n-SND9yK4ziwiHn5pA4gQdAfKgU,2700
 presidio_anonymizer/operators/operator.py,sha256=fbk4gbcV5R4r-ZlNVmbXSVvEEJNWlu1UjVSFZQ3gM08,972
 presidio_anonymizer/operators/operators_factory.py,sha256=bpLSIrNq0n2NovIE1HRrPNqCohe4-VCGozmYldbT03k,2822
 presidio_anonymizer/operators/redact.py,sha256=D20P4bcfAOoPKpQ_YhKKCFU2tAaZmbj3zsaUkpuFn-c,704
 presidio_anonymizer/operators/replace.py,sha256=R6qxC1rKCfakTZ_6MU-hfGfkjoGUk6F2wwds--35Ub4,981
 presidio_anonymizer/services/__init__.py,sha256=ne-KPeMBMTqhQqcqMsL93KUyWpSIJqPAi8KCQoca0rY,21
 presidio_anonymizer/services/app_entities_convertor.py,sha256=ouGaEOB_rhz4AIa3BgSD-xf_3k5qn-nNw8SutV3WlFk,2225
 presidio_anonymizer/services/validators.py,sha256=l-mKjVV6sSlLMgAMCX4ebFw9htWXTA-qjkNVL6gBPuM,3273
-presidio_anonymizer-2.2.32.dist-info/METADATA,sha256=f9Dbg2Zuwqj8TzKu6Z8f0kP8YmlATo6sI0l5c5IBboc,7992
-presidio_anonymizer-2.2.32.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-presidio_anonymizer-2.2.32.dist-info/top_level.txt,sha256=FvDK0W7EbNEph1tKgYJdecF9WsL5AZ1mhHV_cdSKy6E,20
-presidio_anonymizer-2.2.32.dist-info/RECORD,,
+presidio_anonymizer-2.2.33.dist-info/METADATA,sha256=DqFPuitejCXbY1s5EcPzkCp-DNMzfFP61HletnDKFHo,8043
+presidio_anonymizer-2.2.33.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+presidio_anonymizer-2.2.33.dist-info/top_level.txt,sha256=FvDK0W7EbNEph1tKgYJdecF9WsL5AZ1mhHV_cdSKy6E,20
+presidio_anonymizer-2.2.33.dist-info/RECORD,,
```

