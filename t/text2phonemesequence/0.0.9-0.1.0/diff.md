# Comparing `tmp/text2phonemesequence-0.0.9.tar.gz` & `tmp/text2phonemesequence-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/text2phonemesequence-0.0.9.tar", last modified: Sun Jun  4 02:42:47 2023, max compression
+gzip compressed data, was "dist/text2phonemesequence-0.1.0.tar", last modified: Sun Jun  4 02:47:23 2023, max compression
```

## Comparing `text2phonemesequence-0.0.9.tar` & `text2phonemesequence-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:42:47.000000 text2phonemesequence-0.0.9/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2752 2023-06-04 02:42:47.000000 text2phonemesequence-0.0.9/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1889 2023-06-03 08:29:56.000000 text2phonemesequence-0.0.9/README.md
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-06-04 02:42:47.000000 text2phonemesequence-0.0.9/setup.cfg
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.0.9/setup.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:42:47.000000 text2phonemesequence-0.0.9/text2phonemesequence/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-06-04 02:42:20.000000 text2phonemesequence-0.0.9/text2phonemesequence/__init__.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     7852 2023-06-04 02:41:51.000000 text2phonemesequence-0.0.9/text2phonemesequence/text2phonemesequence.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:42:47.000000 text2phonemesequence-0.0.9/text2phonemesequence.egg-info/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2752 2023-06-04 02:42:46.000000 text2phonemesequence-0.0.9/text2phonemesequence.egg-info/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-06-04 02:42:46.000000 text2phonemesequence-0.0.9/text2phonemesequence.egg-info/SOURCES.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-06-04 02:42:46.000000 text2phonemesequence-0.0.9/text2phonemesequence.egg-info/dependency_links.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-06-04 02:42:46.000000 text2phonemesequence-0.0.9/text2phonemesequence.egg-info/requires.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-06-04 02:42:46.000000 text2phonemesequence-0.0.9/text2phonemesequence.egg-info/top_level.txt
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2752 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1889 2023-06-03 08:29:56.000000 text2phonemesequence-0.1.0/README.md
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/setup.cfg
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.1.0/setup.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-06-04 02:47:20.000000 text2phonemesequence-0.1.0/text2phonemesequence/__init__.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     7863 2023-06-04 02:46:39.000000 text2phonemesequence-0.1.0/text2phonemesequence/text2phonemesequence.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2752 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/requires.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/top_level.txt
```

### Comparing `text2phonemesequence-0.0.9/PKG-INFO` & `text2phonemesequence-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
```

### Comparing `text2phonemesequence-0.0.9/README.md` & `text2phonemesequence-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.0.9/setup.py` & `text2phonemesequence-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.0.9/text2phonemesequence/text2phonemesequence.py` & `text2phonemesequence-0.1.0/text2phonemesequence/text2phonemesequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             preds = self.model.generate(**out, num_beams=1, max_length=self.phoneme_length[self.language + '.tsv'])
             phones = self.tokenizer.batch_decode(preds.tolist(),skip_special_tokens=True)
             assert len(phones) == len(list_words_p_batch[j])
 
             for i in range(len(phones)):
                 if list_words_p_batch[j][i] in self.punctuation:
                     phones[i] = list_words_p_batch[j][i]
-                self.phone_dict[list_words[i]] = [phones[i]]
+                self.phone_dict[list_words_p_batch[j][i]] = [phones[i]]
         for w in self.phone_dict.keys():
             try:
                 segmented_phone = self.segment_tool(self.phone_dict[w][0], ipa=True)
             except:
                 segmented_phone = self.segment_tool(self.phone_dict[w][0])
             self.phone_dict[w].append(segmented_phone)
```

### Comparing `text2phonemesequence-0.0.9/text2phonemesequence.egg-info/PKG-INFO` & `text2phonemesequence-0.1.0/text2phonemesequence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
```

