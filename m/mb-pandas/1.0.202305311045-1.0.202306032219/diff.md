# Comparing `tmp/mb_pandas-1.0.202305311045-py3-none-any.whl.zip` & `tmp/mb_pandas-1.0.202306032219-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9954 bytes, number of entries: 13
+Zip file size: 9953 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx      162 b- defN 23-May-25 03:48 mb_pandas/src/__init__.py
 -rw-rw-r--  2.0 unx     1612 b- defN 23-May-25 03:36 mb_pandas/src/aio.py
 -rw-rw-r--  2.0 unx      482 b- defN 23-May-25 03:36 mb_pandas/src/convert_data.py
 -rw-rw-r--  2.0 unx     3516 b- defN 23-May-29 10:17 mb_pandas/src/dfload.py
 -rw-rw-r--  2.0 unx     2418 b- defN 23-May-25 03:36 mb_pandas/src/profiler.py
--rw-rw-r--  2.0 unx     8084 b- defN 23-May-31 10:45 mb_pandas/src/transform.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-31 10:45 mb_pandas/src/version.py
--rwxrwxr-x  2.0 unx     1671 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.data/scripts/df_profile
--rwxrwxr-x  2.0 unx     3683 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.data/scripts/df_view
--rw-rw-r--  2.0 unx      224 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1128 b- defN 23-May-31 10:45 mb_pandas-1.0.202305311045.dist-info/RECORD
-13 files, 23478 bytes uncompressed, 8046 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx     8085 b- defN 23-Jun-03 22:18 mb_pandas/src/transform.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-03 22:19 mb_pandas/src/version.py
+-rwxrwxr-x  2.0 unx     1671 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.data/scripts/df_profile
+-rwxrwxr-x  2.0 unx     3683 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.data/scripts/df_view
+-rw-rw-r--  2.0 unx      224 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1128 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.dist-info/RECORD
+13 files, 23479 bytes uncompressed, 8045 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mb_pandas/src/transform.py
 Comment: 
 
 Filename: mb_pandas/src/version.py
 Comment: 
 
-Filename: mb_pandas-1.0.202305311045.data/scripts/df_profile
+Filename: mb_pandas-1.0.202306032219.data/scripts/df_profile
 Comment: 
 
-Filename: mb_pandas-1.0.202305311045.data/scripts/df_view
+Filename: mb_pandas-1.0.202306032219.data/scripts/df_view
 Comment: 
 
-Filename: mb_pandas-1.0.202305311045.dist-info/METADATA
+Filename: mb_pandas-1.0.202306032219.dist-info/METADATA
 Comment: 
 
-Filename: mb_pandas-1.0.202305311045.dist-info/WHEEL
+Filename: mb_pandas-1.0.202306032219.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pandas-1.0.202305311045.dist-info/top_level.txt
+Filename: mb_pandas-1.0.202306032219.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pandas-1.0.202305311045.dist-info/RECORD
+Filename: mb_pandas-1.0.202306032219.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pandas/src/transform.py

```diff
@@ -29,29 +29,29 @@
         raise ValueError("No common columns to merge on") 
     
     list_df = [df2[i:i+chunksize] for i in range(0, df2.shape[0],chunksize)]
     if logger:
         logger.info(f'Size of chunk: {chunksize}')
         logger.info(f'Number of chunks: {len(list_df)}')
     
-    merged_chunks = []
+    #merged_chunks = []
 
-    for chunk in list_df:
-        merged_chunk = pd.merge(df1, chunk, **kwargs)
-        merged_chunks.append(merged_chunk)
+    # for chunk in list_df:
+    #     merged_chunk = pd.merge(df1, chunk, **kwargs)
+    #     merged_chunks.append(merged_chunk)
 
-    res = pd.concat(merged_chunks,ignore_index=True)
-    return res    
+    # res = pd.concat(merged_chunks,ignore_index=True)
+    # return res    
     
-    # for chunk in list_df:
-    #     merged_chunk = pd.merge(df1,chunk,**kwargs)
-    #     res = pd.concat([res, merged_chunk])
+    for chunk in list_df:
+        merged_chunk = pd.merge(df1,chunk,**kwargs)
+        res = pd.concat([res, merged_chunk])
     
-    # res = res.reset_index(drop=True)
-    # return res
+    res = res.reset_index(drop=True)
+    return res
     
  
 def merge_dask(df1,df2,logger=None,**kwargs):
     """
     Use dask to merge 2 DataFrames
     
     Args:
```

## mb_pandas/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
-VERSION_MONTH = int('05')
-VERSION_DAY = int('31')
-VERSION_HOUR = int('10')
-VERSION_MINUTE = int('45')
+VERSION_MONTH = int('06')
+VERSION_DAY = int('03')
+VERSION_HOUR = int('22')
+VERSION_MINUTE = int('19')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202305311045
-version_date = '2023/05/31 10:45'
+PATCH_VERSION = 202306032219
+version_date = '2023/06/03 22:19'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_pandas-1.0.202305311045.data/scripts/df_profile` & `mb_pandas-1.0.202306032219.data/scripts/df_profile`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305311045.data/scripts/df_view` & `mb_pandas-1.0.202306032219.data/scripts/df_view`

 * *Files identical despite different names*

