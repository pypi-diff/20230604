# Comparing `tmp/text2phonemesequence-0.1.2.tar.gz` & `tmp/text2phonemesequence-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/text2phonemesequence-0.1.2.tar", last modified: Sun Jun  4 03:13:00 2023, max compression
+gzip compressed data, was "dist/text2phonemesequence-0.1.3.tar", last modified: Sun Jun  4 06:34:35 2023, max compression
```

## Comparing `text2phonemesequence-0.1.2.tar` & `text2phonemesequence-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2837 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1974 2023-06-04 03:02:25.000000 text2phonemesequence-0.1.2/README.md
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/setup.cfg
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.1.2/setup.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-06-04 03:06:17.000000 text2phonemesequence-0.1.2/text2phonemesequence/__init__.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     8123 2023-06-04 03:12:35.000000 text2phonemesequence-0.1.2/text2phonemesequence/text2phonemesequence.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2837 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/SOURCES.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/dependency_links.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/requires.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/top_level.txt
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2838 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1975 2023-06-04 05:13:39.000000 text2phonemesequence-0.1.3/README.md
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/setup.cfg
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.1.3/setup.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-06-04 06:34:11.000000 text2phonemesequence-0.1.3/text2phonemesequence/__init__.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     8114 2023-06-04 05:13:39.000000 text2phonemesequence-0.1.3/text2phonemesequence/text2phonemesequence.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2838 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/requires.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-06-04 06:34:35.000000 text2phonemesequence-0.1.3/text2phonemesequence.egg-info/top_level.txt
```

### Comparing `text2phonemesequence-0.1.2/PKG-INFO` & `text2phonemesequence-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
@@ -22,19 +22,19 @@
         ## Usage example <a name="example"></a>
         The library uses [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) and [segments](https://pypi.org/project/segments/) toolkits to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
         
         ```python
         from text2phonemesequence import Text2PhonemeSequence
         
         # Load Text2PhonemeSequence
-        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
+        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_small_100', language='eng-us', is_cuda=False)
         
         
         # Convert a raw corpus
-        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file", batch_size=64) # batch_size is the number of words fed into the CharsiuG2P toolkit  
+        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file", batch_size=64) # batch_size is the number of words fed into the CharsiuG2P toolkit per times. 
         
         # Convert a raw sentence
         model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
         ##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
         ```
         
 Platform: UNKNOWN
```

### Comparing `text2phonemesequence-0.1.2/README.md` & `text2phonemesequence-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 ## Usage example <a name="example"></a>
 The library uses [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) and [segments](https://pypi.org/project/segments/) toolkits to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
 
 ```python
 from text2phonemesequence import Text2PhonemeSequence
 
 # Load Text2PhonemeSequence
-model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
+model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_small_100', language='eng-us', is_cuda=False)
 
 
 # Convert a raw corpus
-model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file", batch_size=64) # batch_size is the number of words fed into the CharsiuG2P toolkit  
+model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file", batch_size=64) # batch_size is the number of words fed into the CharsiuG2P toolkit per times. 
 
 # Convert a raw sentence
 model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
 ##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
 ```
```

### Comparing `text2phonemesequence-0.1.2/setup.py` & `text2phonemesequence-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.1.2/text2phonemesequence/text2phonemesequence.py` & `text2phonemesequence-0.1.3/text2phonemesequence/text2phonemesequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from transformers import T5ForConditionalGeneration, AutoTokenizer
 from segments import Tokenizer
 import os
 from tqdm import tqdm
 
 class Text2PhonemeSequence:
-    def __init__(self, pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', tokenizer= 'google/byt5-small', language='vie-c', is_cuda=True):
+    def __init__(self, pretrained_g2p_model='charsiu/g2p_multilingual_byT5_small_100', tokenizer= 'google/byt5-small', language='vie-c', is_cuda=True):
         self.tokenizer = AutoTokenizer.from_pretrained(tokenizer)
         self.model = T5ForConditionalGeneration.from_pretrained(pretrained_g2p_model)
         self.is_cuda = is_cuda
         if self.is_cuda:
             self.model = self.model.cuda()
         self.punctuation = list('.?!,:;-()[]{}<>"') + list("'/‘”“/&#~@^|") + ['...', '*']
         self.segment_tool = Tokenizer()
```

### Comparing `text2phonemesequence-0.1.2/text2phonemesequence.egg-info/PKG-INFO` & `text2phonemesequence-0.1.3/text2phonemesequence.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
@@ -22,19 +22,19 @@
         ## Usage example <a name="example"></a>
         The library uses [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) and [segments](https://pypi.org/project/segments/) toolkits to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
         
         ```python
         from text2phonemesequence import Text2PhonemeSequence
         
         # Load Text2PhonemeSequence
-        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
+        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_small_100', language='eng-us', is_cuda=False)
         
         
         # Convert a raw corpus
-        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file", batch_size=64) # batch_size is the number of words fed into the CharsiuG2P toolkit  
+        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file", batch_size=64) # batch_size is the number of words fed into the CharsiuG2P toolkit per times. 
         
         # Convert a raw sentence
         model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
         ##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
         ```
         
 Platform: UNKNOWN
```

