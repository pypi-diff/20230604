# Comparing `tmp/text2phonemesequence-0.1.1.tar.gz` & `tmp/text2phonemesequence-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/text2phonemesequence-0.1.1.tar", last modified: Sun Jun  4 02:53:55 2023, max compression
+gzip compressed data, was "dist/text2phonemesequence-0.1.2.tar", last modified: Sun Jun  4 03:13:00 2023, max compression
```

## Comparing `text2phonemesequence-0.1.1.tar` & `text2phonemesequence-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2752 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1889 2023-06-03 08:29:56.000000 text2phonemesequence-0.1.1/README.md
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/setup.cfg
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.1.1/setup.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/text2phonemesequence/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-06-04 02:49:40.000000 text2phonemesequence-0.1.1/text2phonemesequence/__init__.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     7857 2023-06-04 02:53:33.000000 text2phonemesequence-0.1.1/text2phonemesequence/text2phonemesequence.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2752 2023-06-04 02:53:54.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/SOURCES.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-06-04 02:53:54.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/dependency_links.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/requires.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/top_level.txt
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2837 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1974 2023-06-04 03:02:25.000000 text2phonemesequence-0.1.2/README.md
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/setup.cfg
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.1.2/setup.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-06-04 03:06:17.000000 text2phonemesequence-0.1.2/text2phonemesequence/__init__.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     8123 2023-06-04 03:12:35.000000 text2phonemesequence-0.1.2/text2phonemesequence/text2phonemesequence.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2837 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/requires.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-06-04 03:13:00.000000 text2phonemesequence-0.1.2/text2phonemesequence.egg-info/top_level.txt
```

### Comparing `text2phonemesequence-0.1.1/PKG-INFO` & `text2phonemesequence-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
@@ -26,15 +26,15 @@
         from text2phonemesequence import Text2PhonemeSequence
         
         # Load Text2PhonemeSequence
         model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
         
         
         # Convert a raw corpus
-        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
+        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file", batch_size=64) # batch_size is the number of words fed into the CharsiuG2P toolkit  
         
         # Convert a raw sentence
         model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
         ##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
         ```
         
 Platform: UNKNOWN
```

### Comparing `text2phonemesequence-0.1.1/README.md` & `text2phonemesequence-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 from text2phonemesequence import Text2PhonemeSequence
 
 # Load Text2PhonemeSequence
 model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
 
 
 # Convert a raw corpus
-model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
+model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file", batch_size=64) # batch_size is the number of words fed into the CharsiuG2P toolkit  
 
 # Convert a raw sentence
 model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
 ##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
 ```
```

### Comparing `text2phonemesequence-0.1.1/setup.py` & `text2phonemesequence-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.1.1/text2phonemesequence/text2phonemesequence.py` & `text2phonemesequence-0.1.2/text2phonemesequence/text2phonemesequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,38 +39,44 @@
             words = line.strip().split("|")[-1].split(" ")
             for w in words:
                 w = w.replace(seperate_syllabel_token, " ").lower()
                 if w not in self.phone_dict.keys():
                     list_words.append(w)
         list_words_p = ['<' + self.language + '>: ' + i for i in list_words]
         list_words_p_batch = []
+        list_words_batch = []
         temp_list = []
-        for w in list_words_p:
-            temp_list.append(w)
+        temp_list_raw = []
+        for m in range(len(list_words_p)):
+            temp_list.append(list_words_p[m])
+            temp_list_raw.append(list_words[m])
             if len(temp_list) == batch_size:
                 list_words_p_batch.append(temp_list)
                 temp_list = []
+                list_words_batch.append(temp_list_raw)
+                temp_list_raw = []
         if len(temp_list) != 0:
             list_words_p_batch.append(temp_list)
+            list_words_batch.append(temp_list_raw)
 
         for j in range(len(list_words_p_batch)):
             out = self.tokenizer(list_words_p_batch[j], padding=True, add_special_tokens=False, return_tensors='pt')
             if self.is_cuda:
                 out['input_ids'] = out['input_ids'].cuda()
                 out['attention_mask'] = out['attention_mask'].cuda()
             if self.language + '.tsv' not in self.phoneme_length.keys():
                 self.phoneme_length[self.language + '.tsv'] = 50
             preds = self.model.generate(**out, num_beams=1, max_length=self.phoneme_length[self.language + '.tsv'])
             phones = self.tokenizer.batch_decode(preds.tolist(),skip_special_tokens=True)
             assert len(phones) == len(list_words_p_batch[j])
 
             for i in range(len(phones)):
-                if list_words_p_batch[j][i] in self.punctuation:
-                    phones[i] = list_words_p_batch[j][i]
-                self.phone_dict[list_words_p_batch[j][i]] = [phones[i]]
+                if list_words_batch[j][i] in self.punctuation:
+                    phones[i] = list_words_batch[j][i]
+                self.phone_dict[list_words_batch[j][i]] = [phones[i]]
         for w in self.phone_dict.keys():
             try:
                 segmented_phone = self.segment_tool(self.phone_dict[w][0], ipa=True)
             except:
                 segmented_phone = self.segment_tool(self.phone_dict[w][0])
             self.phone_dict[w].append(segmented_phone)
```

### Comparing `text2phonemesequence-0.1.1/text2phonemesequence.egg-info/PKG-INFO` & `text2phonemesequence-0.1.2/text2phonemesequence.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
@@ -26,15 +26,15 @@
         from text2phonemesequence import Text2PhonemeSequence
         
         # Load Text2PhonemeSequence
         model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
         
         
         # Convert a raw corpus
-        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
+        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file", batch_size=64) # batch_size is the number of words fed into the CharsiuG2P toolkit  
         
         # Convert a raw sentence
         model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
         ##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
         ```
         
 Platform: UNKNOWN
```

