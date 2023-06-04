# Comparing `tmp/pyAutoSummarizer-1.1.0.tar.gz` & `tmp/pyAutoSummarizer-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyAutoSummarizer-1.1.0.tar", last modified: Sat Jun  3 02:14:36 2023, max compression
+gzip compressed data, was "dist\pyAutoSummarizer-1.1.2.tar", last modified: Sun Jun  4 00:54:49 2023, max compression
```

## Comparing `pyAutoSummarizer-1.1.0.tar` & `pyAutoSummarizer-1.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 02:14:36.000000 pyAutoSummarizer-1.1.0/
--rw-rw-rw-   0        0        0      674 2023-05-18 23:07:37.000000 pyAutoSummarizer-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       50 2023-05-18 23:07:52.000000 pyAutoSummarizer-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4973 2023-06-03 02:14:36.000000 pyAutoSummarizer-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4572 2023-06-03 02:09:56.000000 pyAutoSummarizer-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/
--rw-rw-rw-   0        0        0       31 2023-05-13 15:40:37.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/__init__.py
--rw-rw-rw-   0        0        0    32162 2023-06-03 02:11:24.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/psr.py
-drwxrwxrwx   0        0        0        0 2023-06-03 02:14:36.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/
--rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt
--rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Greek.txt
--rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt
--rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Korean.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt
--rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Thai.txt
--rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/
--rw-rw-rw-   0        0        0     4973 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1724 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-06-03 02:14:36.000000 pyAutoSummarizer-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-03 01:21:36.000000 pyAutoSummarizer-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 00:54:49.000000 pyAutoSummarizer-1.1.2/
+-rw-rw-rw-   0        0        0      674 2023-05-18 23:07:37.000000 pyAutoSummarizer-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-05-18 23:07:52.000000 pyAutoSummarizer-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4973 2023-06-04 00:54:49.000000 pyAutoSummarizer-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4572 2023-06-03 02:09:56.000000 pyAutoSummarizer-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 00:54:48.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 00:54:48.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/
+-rw-rw-rw-   0        0        0       31 2023-05-13 15:40:37.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/__init__.py
+-rw-rw-rw-   0        0        0    32663 2023-06-04 00:53:54.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/psr.py
+drwxrwxrwx   0        0        0        0 2023-06-04 00:54:49.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/
+-rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt
+-rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Greek.txt
+-rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt
+-rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Korean.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt
+-rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Thai.txt
+-rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 00:54:48.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer.egg-info/
+-rw-rw-rw-   0        0        0     4973 2023-06-04 00:54:48.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1724 2023-06-04 00:54:48.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 00:54:48.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-04 00:54:48.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-04 00:54:48.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-04 00:54:48.000000 pyAutoSummarizer-1.1.2/pyAutoSummarizer.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-04 00:54:49.000000 pyAutoSummarizer-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-04 00:54:20.000000 pyAutoSummarizer-1.1.2/setup.py
```

### Comparing `pyAutoSummarizer-1.1.0/LICENSE` & `pyAutoSummarizer-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/PKG-INFO` & `pyAutoSummarizer-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAutoSummarizer
-Version: 1.1.0
+Version: 1.1.2
 Summary: An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence
 Home-page: https://github.com/Valdecy/pyAutoSummarizer
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyAutoSummarizer-1.1.0/README.md` & `pyAutoSummarizer-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/psr.py` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/psr.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,15 +305,17 @@
         tf_idf_matrix = vectorizer.transform(self.corpus)
         tf_idf_m      = tf_idf_matrix.toarray()
         #vectorizer.vocabulary_
         #vectorizer.get_feature_names()
         return tf_idf_m
 
     ##############################################################################
-    
+
+    # ROUGE N
+
     # Function: Rouge N 
     def rouge_N(self, generated_summary, reference_summary, n = 1):
         generated_summary = self.clear_text([generated_summary], stop_words = self.p_sw, lowercase = self.p_lc, rmv_accents = self.p_ra, rmv_special_chars = self.p_rc, rmv_numbers = self.p_rn, rmv_custom_words = self.p_rw)
         reference_summary = self.clear_text([reference_summary], stop_words = self.p_sw, lowercase = self.p_lc, rmv_accents = self.p_ra, rmv_special_chars = self.p_rc, rmv_numbers = self.p_rn, rmv_custom_words = self.p_rw)
         gen_tokens        = generated_summary[0].split()
         ref_tokens        = reference_summary[0].split()
         max_n             = min(len(gen_tokens), len(ref_tokens))
@@ -331,14 +333,16 @@
         precision = overlap / len(gen_ngrams) if len(gen_ngrams) > 0 else 0
         recall    = overlap / len(ref_ngrams) if len(ref_ngrams) > 0 else 0
         f1        = 2 * (precision * recall) / (precision + recall) if (precision + recall) > 0 else 0
         return f1, precision, recall
 
     ##############################################################################
     
+    # ROUGE L
+    
     # Function: LCS
     def LCS(self, gen_tokens, ref_tokens):
         matrix = np.zeros((len(ref_tokens) + 1, len(gen_tokens) + 1))
         for i in range(1, len(ref_tokens) + 1):
             for j in range(1, len(gen_tokens) + 1):
                 if (ref_tokens[i-1] == gen_tokens[j-1] ):
                     matrix[i,j] = matrix[i-1, j-1] + 1
@@ -357,14 +361,16 @@
         precision         = lcs_length / len(gen_tokens) if len(gen_tokens) > 0 else 0
         recall            = lcs_length / len(ref_tokens) if len(ref_tokens) > 0 else 0
         f1                = 2 * (precision * recall) / (precision + recall) if (precision + recall) > 0 else 0
         return f1, precision, recall
     
     ##############################################################################
     
+    # ROUGE S
+    
     # Function: Generate Skip Gram
     def generate_skip_bigrams(self, tokens, skip_distance):
         skip_bigrams = set()
         tokens       = self.clear_text([tokens], stop_words = self.p_sw, lowercase = self.p_lc, rmv_accents = self.p_ra, rmv_special_chars = self.p_rc, rmv_numbers = self.p_rn, rmv_custom_words = self.p_rw)
         tokens       = tokens[0].split()
         for i in range(0, len(tokens)):
             for j in range(i+1, min(i+1+skip_distance, len(tokens))):
@@ -381,14 +387,16 @@
         precision      = overlap / total_g if total_g > 0 else 0
         recall         = overlap / total_r if total_r > 0 else 0
         f1             = 2 * (precision * recall) / (precision + recall) if (precision + recall) > 0 else 0
         return f1, precision, recall
 
     ##############################################################################
     
+    # BLEU
+    
     # Function: Count N-Grams
     def count_ngrams(self, tokens, n):
         ngrams = {}
         if (n == 1):
             for i in range(0, len(tokens) - n + 1):
                 ngram         = tokens[i:i+n][0]
                 ngrams[ngram] = ngrams.get(ngram, 0) + 1
@@ -419,14 +427,16 @@
         rt                = len(ref_tokens) / len(gen_tokens) if  len(gen_tokens) > 0 else 0
         bp                = min(1, np.exp(1 - rt)) # brevity penalty
         bleu_s            = bp * gm
         return bleu_s
 
     ##############################################################################
     
+    # METEOR
+    
     # Function: Match Tokens
     def match_tokens(self, gen_tokens, ref_tokens):
         matches  = 0
         ref_dict = {}
         for token in ref_tokens:
             if (token in ref_dict):
                 ref_dict[token] = ref_dict[token] + 1
@@ -434,14 +444,24 @@
                 ref_dict[token] = 1
         for token in gen_tokens:
             if (token in ref_dict and ref_dict[token] > 0):
                 matches         = matches + 1
                 ref_dict[token] = ref_dict[token] - 1
         return matches
     
+    # Function: Number of Chunks
+    def calculate_num_chunks(self, candidate_chunks, reference_chunks):
+        num_chunks = 0
+        for chunk in candidate_chunks:
+            for ref_chunk in reference_chunks:
+                if any(token in ref_chunk for token in chunk):
+                    num_chunks = num_chunks + 1
+                    break  
+        return num_chunks
+    
     # Function: Chunck Penalty
     def calculate_chunk_penalty(self, gen_tokens, ref_tokens, matches):
         candidate_chunks = set()
         reference_chunks = set()
         chunk_start      = None
         ref_chunk_start  = None
         ref_chunk_end    = None
@@ -454,23 +474,23 @@
                     ref_chunk_start = ref_index
                 ref_chunk_end = ref_index
             else:
                 if (chunk_start is not None ):
                     candidate_chunks.add(tuple(range(chunk_start, i)))
                     chunk_start = None
                 if (ref_chunk_start is not None and ref_chunk_end is not None):
-                    reference_chunks.add(tuple(range(ref_chunk_start, ref_chunk_end+1)))
+                    reference_chunks.add(tuple(range(ref_chunk_start, ref_chunk_end + 1)))
                     ref_chunk_start = None
-                    ref_chunk_end = None
+                    ref_chunk_end   = None
         if (chunk_start is not None):
             candidate_chunks.add(tuple(range(chunk_start, len(gen_tokens))))
         if (ref_chunk_start is not None and ref_chunk_end is not None):
-            reference_chunks.add(tuple(range(ref_chunk_start, ref_chunk_end+1)))
-        num_chunks    = len(candidate_chunks.intersection(reference_chunks))
-        chunk_penalty = 1 - (num_chunks / matches)**0.5 if matches > 0 else 1
+            reference_chunks.add(tuple(range(ref_chunk_start, ref_chunk_end + 1)))
+        num_chunks    = self.calculate_num_chunks(candidate_chunks, reference_chunks)
+        chunk_penalty = 0 if matches == 0 else 0.5*(num_chunks / matches)**3
         return chunk_penalty
     
     # Function: METEOR Score
     def meteor(self, generated_summary, reference_summary, alpha = 0.9, beta = 3):
         generated_summary = self.clear_text([generated_summary], stop_words = self.p_sw, lowercase = self.p_lc, rmv_accents = self.p_ra, rmv_special_chars = self.p_rc, rmv_numbers = self.p_rn, rmv_custom_words = self.p_rw)
         reference_summary = self.clear_text([reference_summary], stop_words = self.p_sw, lowercase = self.p_lc, rmv_accents = self.p_ra, rmv_special_chars = self.p_rc, rmv_numbers = self.p_rn, rmv_custom_words = self.p_rw)
         gen_tokens        = generated_summary[0].split()
```

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Czech.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-English.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-French.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-German.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Greek.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Greek.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Italian.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Korean.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Korean.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Persian.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Polish.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Russian.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Thai.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Thai.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/PKG-INFO` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAutoSummarizer
-Version: 1.1.0
+Version: 1.1.2
 Summary: An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence
 Home-page: https://github.com/Valdecy/pyAutoSummarizer
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/SOURCES.txt` & `pyAutoSummarizer-1.1.2/pyAutoSummarizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.1.0/setup.py` & `pyAutoSummarizer-1.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyAutoSummarizer',
-    version='1.1.0',
+    version='1.1.2',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyAutoSummarizer',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

