# Comparing `tmp/csv-to-info-chunks-1.0.0.tar.gz` & `tmp/csv-to-info-chunks-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-to-info-chunks-1.0.0.tar", last modified: Sun Jun  4 16:12:44 2023, max compression
+gzip compressed data, was "csv-to-info-chunks-1.0.1.tar", last modified: Sun Jun  4 16:18:04 2023, max compression
```

## Comparing `csv-to-info-chunks-1.0.0.tar` & `csv-to-info-chunks-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-04 16:12:44.724870 csv-to-info-chunks-1.0.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4014 2023-06-04 16:12:44.724734 csv-to-info-chunks-1.0.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     3910 2023-06-04 16:12:44.000000 csv-to-info-chunks-1.0.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-04 16:12:44.724568 csv-to-info-chunks-1.0.0/csv_to_info_chunks.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4014 2023-06-04 16:12:44.000000 csv-to-info-chunks-1.0.0/csv_to_info_chunks.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      253 2023-06-04 16:12:44.000000 csv-to-info-chunks-1.0.0/csv_to_info_chunks.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-04 16:12:44.000000 csv-to-info-chunks-1.0.0/csv_to_info_chunks.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       63 2023-06-04 16:12:44.000000 csv-to-info-chunks-1.0.0/csv_to_info_chunks.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       19 2023-06-04 16:12:44.000000 csv-to-info-chunks-1.0.0/csv_to_info_chunks.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     2583 2023-06-04 16:12:44.000000 csv-to-info-chunks-1.0.0/csv_to_info_chunks.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-04 16:12:44.724909 csv-to-info-chunks-1.0.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      536 2023-06-04 16:12:44.000000 csv-to-info-chunks-1.0.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-04 16:18:04.804530 csv-to-info-chunks-1.0.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4361 2023-06-04 16:18:04.804401 csv-to-info-chunks-1.0.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4257 2023-06-04 16:18:04.000000 csv-to-info-chunks-1.0.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-04 16:18:04.804226 csv-to-info-chunks-1.0.1/csv_to_info_chunks.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4361 2023-06-04 16:18:04.000000 csv-to-info-chunks-1.0.1/csv_to_info_chunks.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      253 2023-06-04 16:18:04.000000 csv-to-info-chunks-1.0.1/csv_to_info_chunks.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-04 16:18:04.000000 csv-to-info-chunks-1.0.1/csv_to_info_chunks.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       63 2023-06-04 16:18:04.000000 csv-to-info-chunks-1.0.1/csv_to_info_chunks.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       19 2023-06-04 16:18:04.000000 csv-to-info-chunks-1.0.1/csv_to_info_chunks.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     2583 2023-06-04 16:18:04.000000 csv-to-info-chunks-1.0.1/csv_to_info_chunks.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-04 16:18:04.804568 csv-to-info-chunks-1.0.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      536 2023-06-04 16:18:04.000000 csv-to-info-chunks-1.0.1/setup.py
```

### Comparing `csv-to-info-chunks-1.0.0/PKG-INFO` & `csv-to-info-chunks-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Metadata-Version: 2.1
 Name: csv-to-info-chunks
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # CSV 轉換為資訊區塊
+```
+🐔動機: 
+為了讓每個 CSV row 單獨成為語境探索的資訊區塊，需將 CSV row 轉換成 JSON 資訊區塊。
+切割完畢之後，下一個階段可以針對 content 欄位計算來增添 embeddings 詞向量欄位。
+ 
+💣地雷: 
+這個套件的輸入格式是 google-sheet-downloader 的輸出檔案群CSV and JSON。
+```
+
 ## 簡介
 該工具可以將 CSV 文件中的數據轉換成 JSON 形式的資訊區塊。您可以選擇強制重新生成所有 JSON 文件，或者僅生成不存在的 JSON 文件。
 
 ## 安裝
 ```
 python3 -m pip install csv-to-info-chunks
 ```
```

### Comparing `csv-to-info-chunks-1.0.0/README.md` & `csv-to-info-chunks-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,17 @@
 # CSV 轉換為資訊區塊
+```
+🐔動機: 
+為了讓每個 CSV row 單獨成為語境探索的資訊區塊，需將 CSV row 轉換成 JSON 資訊區塊。
+切割完畢之後，下一個階段可以針對 content 欄位計算來增添 embeddings 詞向量欄位。
+ 
+💣地雷: 
+這個套件的輸入格式是 google-sheet-downloader 的輸出檔案群CSV and JSON。
+```
+
 ## 簡介
 該工具可以將 CSV 文件中的數據轉換成 JSON 形式的資訊區塊。您可以選擇強制重新生成所有 JSON 文件，或者僅生成不存在的 JSON 文件。
 
 ## 安裝
 ```
 python3 -m pip install csv-to-info-chunks
 ```
```

### Comparing `csv-to-info-chunks-1.0.0/csv_to_info_chunks.egg-info/PKG-INFO` & `csv-to-info-chunks-1.0.1/csv_to_info_chunks.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Metadata-Version: 2.1
 Name: csv-to-info-chunks
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # CSV 轉換為資訊區塊
+```
+🐔動機: 
+為了讓每個 CSV row 單獨成為語境探索的資訊區塊，需將 CSV row 轉換成 JSON 資訊區塊。
+切割完畢之後，下一個階段可以針對 content 欄位計算來增添 embeddings 詞向量欄位。
+ 
+💣地雷: 
+這個套件的輸入格式是 google-sheet-downloader 的輸出檔案群CSV and JSON。
+```
+
 ## 簡介
 該工具可以將 CSV 文件中的數據轉換成 JSON 形式的資訊區塊。您可以選擇強制重新生成所有 JSON 文件，或者僅生成不存在的 JSON 文件。
 
 ## 安裝
 ```
 python3 -m pip install csv-to-info-chunks
 ```
```

### Comparing `csv-to-info-chunks-1.0.0/csv_to_info_chunks.py` & `csv-to-info-chunks-1.0.1/csv_to_info_chunks.py`

 * *Files identical despite different names*

### Comparing `csv-to-info-chunks-1.0.0/setup.py` & `csv-to-info-chunks-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="csv-to-info-chunks",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     py_modules=['csv_to_info_chunks'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'csv_to_info_chunks = csv_to_info_chunks:main',
         ],
```

