# Comparing `tmp/text2phonemesequence-0.1.0.tar.gz` & `tmp/text2phonemesequence-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/text2phonemesequence-0.1.0.tar", last modified: Sun Jun  4 02:47:23 2023, max compression
+gzip compressed data, was "dist/text2phonemesequence-0.1.1.tar", last modified: Sun Jun  4 02:53:55 2023, max compression
```

## Comparing `text2phonemesequence-0.1.0.tar` & `text2phonemesequence-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2752 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1889 2023-06-03 08:29:56.000000 text2phonemesequence-0.1.0/README.md
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/setup.cfg
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.1.0/setup.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-06-04 02:47:20.000000 text2phonemesequence-0.1.0/text2phonemesequence/__init__.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     7863 2023-06-04 02:46:39.000000 text2phonemesequence-0.1.0/text2phonemesequence/text2phonemesequence.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2752 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/SOURCES.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/dependency_links.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/requires.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-06-04 02:47:23.000000 text2phonemesequence-0.1.0/text2phonemesequence.egg-info/top_level.txt
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2752 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1889 2023-06-03 08:29:56.000000 text2phonemesequence-0.1.1/README.md
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/setup.cfg
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.1.1/setup.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/text2phonemesequence/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-06-04 02:49:40.000000 text2phonemesequence-0.1.1/text2phonemesequence/__init__.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     7857 2023-06-04 02:53:33.000000 text2phonemesequence-0.1.1/text2phonemesequence/text2phonemesequence.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2752 2023-06-04 02:53:54.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-06-04 02:53:54.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/requires.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-06-04 02:53:55.000000 text2phonemesequence-0.1.1/text2phonemesequence.egg-info/top_level.txt
```

### Comparing `text2phonemesequence-0.1.0/PKG-INFO` & `text2phonemesequence-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
```

### Comparing `text2phonemesequence-0.1.0/README.md` & `text2phonemesequence-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.1.0/setup.py` & `text2phonemesequence-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.1.0/text2phonemesequence/text2phonemesequence.py` & `text2phonemesequence-0.1.1/text2phonemesequence/text2phonemesequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             for w in words:
                 w = w.replace(seperate_syllabel_token, " ").lower()
                 if w not in self.phone_dict.keys():
                     list_words.append(w)
         list_words_p = ['<' + self.language + '>: ' + i for i in list_words]
         list_words_p_batch = []
         temp_list = []
-        for w in list_words_p_batch:
+        for w in list_words_p:
             temp_list.append(w)
             if len(temp_list) == batch_size:
                 list_words_p_batch.append(temp_list)
                 temp_list = []
         if len(temp_list) != 0:
             list_words_p_batch.append(temp_list)
```

### Comparing `text2phonemesequence-0.1.0/text2phonemesequence.egg-info/PKG-INFO` & `text2phonemesequence-0.1.1/text2phonemesequence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
```

