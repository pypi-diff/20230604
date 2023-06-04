# Comparing `tmp/infinstor-2.0.8-py3-none-any.whl.zip` & `tmp/infinstor-2.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 35275 bytes, number of entries: 16
+Zip file size: 35321 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx    77744 b- defN 22-Jan-05 20:05 infinstor/__init__.py
 -rw-rw-r--  2.0 unx     2528 b- defN 21-Dec-20 22:55 infinstor/bootstrap.py
 -rw-rw-r--  2.0 unx     4907 b- defN 21-Dec-12 02:00 infinstor/gnode.py
 -rw-rw-r--  2.0 unx     8936 b- defN 21-Dec-12 02:00 infinstor/infin_ast.py
--rw-rw-r--  2.0 unx    27236 b- defN 22-Jan-06 02:21 infinstor/infin_boto3.py
+-rw-rw-r--  2.0 unx    27533 b- defN 22-Jan-06 02:53 infinstor/infin_boto3.py
 -rw-rw-r--  2.0 unx     1098 b- defN 21-Dec-12 02:00 infinstor/mlflow_run.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Dec-12 02:00 infinstor/infinfs/__init__.py
 -rw-rw-r--  2.0 unx     4205 b- defN 21-Dec-12 02:00 infinstor/infinfs/infin_download.py
 -rw-rw-r--  2.0 unx     1339 b- defN 21-Dec-12 02:00 infinstor/infinfs/infin_prefetch.py
 -rw-rw-r--  2.0 unx    13940 b- defN 21-Dec-12 02:00 infinstor/infinfs/infinfs.py
 -rw-rw-r--  2.0 unx     2362 b- defN 21-Dec-12 02:00 infinstor/infinfs/infinmount.py
--rw-rw-r--  2.0 unx       31 b- defN 22-Jan-06 02:29 infinstor-2.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx      798 b- defN 22-Jan-06 02:29 infinstor-2.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Jan-06 02:29 infinstor-2.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 22-Jan-06 02:29 infinstor-2.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1308 b- defN 22-Jan-06 02:29 infinstor-2.0.8.dist-info/RECORD
-16 files, 146534 bytes uncompressed, 33123 bytes compressed:  77.4%
+-rw-rw-r--  2.0 unx       31 b- defN 22-Jan-06 03:00 infinstor-2.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      798 b- defN 22-Jan-06 03:00 infinstor-2.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-Jan-06 03:00 infinstor-2.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 22-Jan-06 03:00 infinstor-2.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1308 b- defN 22-Jan-06 03:00 infinstor-2.0.9.dist-info/RECORD
+16 files, 146831 bytes uncompressed, 33169 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: infinstor/infinfs/infinfs.py
 Comment: 
 
 Filename: infinstor/infinfs/infinmount.py
 Comment: 
 
-Filename: infinstor-2.0.8.dist-info/LICENSE
+Filename: infinstor-2.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: infinstor-2.0.8.dist-info/METADATA
+Filename: infinstor-2.0.9.dist-info/METADATA
 Comment: 
 
-Filename: infinstor-2.0.8.dist-info/WHEEL
+Filename: infinstor-2.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: infinstor-2.0.8.dist-info/top_level.txt
+Filename: infinstor-2.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: infinstor-2.0.8.dist-info/RECORD
+Filename: infinstor-2.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## infinstor/infin_boto3.py

```diff
@@ -218,24 +218,27 @@
     def get_version_id(self, bucket, prefix):
         print('InfinBotoClient.get_version_id[' + str(os.getpid()) + ']: Entered. bucket='
                 + str(bucket) + ', prefix=' + str(prefix))
         tokfile = os.path.join(expanduser("~"), ".infinstor", "token")
         attempt = 0
         while attempt < 2:
             if attempt == 0:
+                print('get_version_id: attempt = ' + str(attempt) + ', force False')
                 force = False
             else:
+                print('get_version_id: attempt = ' + str(attempt) + ', force True')
                 force = True
             attempt = attempt + 1
             token, service = infinstor_mlflow_plugin.tokenfile.get_token(builtins.region,
                 tokfile, force)
             headers = {
                 'Content-Type': 'application/x-www-form-urlencoded',
                 'Authorization': token
                 }
+            print('get_version_id: headers=' + str(headers))
             url = 'https://' + builtins.apiserver + '/webhdfs/v1/' + prefix\
                     + '?op=GETFILESTATUS&bucket=' + bucket\
                     + '&gets3url=true'
             if self.input_spec['type'] == 'infinsnap-implicit':
                 url = url + '&time=' + str(self.input_spec['epoch_time'])
             elif self.input_spec['type'] == 'infinsnap':
                 time_spec = self.input_spec['time_spec']
@@ -250,14 +253,15 @@
             except HTTPError as http_err:
                 print('HTTP error occurred: ' + str(http_err))
                 raise
             except Exception as err:
                 print('Other error occurred: ' + str(err))
                 raise
             if 'Login expired. Please login again' in response.text:
+                print('get_version_id: got ' + str(response.text))
                 continue
             js = response.json()
             if 'versionId' in js:
                 return js['versionId'], js['s3url']
             else:
                 print('get_version_id: versionId not present in response')
                 return None, None
```

## Comparing `infinstor-2.0.8.dist-info/METADATA` & `infinstor-2.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinstor
-Version: 2.0.8
+Version: 2.0.9
 Summary: InfinStor Utilities usually run in ipython from jupyterlab cells
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `infinstor-2.0.8.dist-info/RECORD` & `infinstor-2.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 infinstor/__init__.py,sha256=gVtcRhWLNQGe3yiXR5-o1ARsaoB0HLLZ957vkOOBvQ0,77744
 infinstor/bootstrap.py,sha256=HttqHyOOB-reM0c6U3KHGuvsLisr4IksX3b9-EhlOVo,2528
 infinstor/gnode.py,sha256=DVSJpLnHhpgJkoUoPWerggzZ9ftUWJ-tFxvnEcje8pg,4907
 infinstor/infin_ast.py,sha256=WKMgvDWNBuIo-cn1CfCuPy18n7pJqxT3CTNd7jTCTuY,8936
-infinstor/infin_boto3.py,sha256=4fWLpkHGYmefWZxBi9xsLQVUuA00_ArkHm74cddKCq0,27236
+infinstor/infin_boto3.py,sha256=KxzlTCbDbTDzEXVQVzrFAW2kTKANonJIs5X-8Ugo6oE,27533
 infinstor/mlflow_run.py,sha256=9g7D2KU72RF9LfO2iXfDdJrTQy3ZD9kNG0D4OsmKHkI,1098
 infinstor/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 infinstor/infinfs/infin_download.py,sha256=WVN4A01583bEcEPZ3ckW4SX7gxpP5EIsgEkQUeofzRY,4205
 infinstor/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 infinstor/infinfs/infinfs.py,sha256=WoMntjqud2Tex08S1AFU1zpkfCN7E91XuFWrJju_3Es,13940
 infinstor/infinfs/infinmount.py,sha256=FhPKtdNhJ4X7nWQ7gFmYPXK9Jhxv5UFEdbyvtWcekuQ,2362
-infinstor-2.0.8.dist-info/LICENSE,sha256=-d8bHexyCOv7P5zVqbOL7bd4wEDzDlsizj6KGbPeCVI,31
-infinstor-2.0.8.dist-info/METADATA,sha256=efTBRWwzoy9IllqMfuoRY_mBmtrOGZd1J1KZqu0FCK0,798
-infinstor-2.0.8.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-infinstor-2.0.8.dist-info/top_level.txt,sha256=MW0CTQKThlkupD5bjg3zvNux77mwdeZ5ua_DVFuCi3s,10
-infinstor-2.0.8.dist-info/RECORD,,
+infinstor-2.0.9.dist-info/LICENSE,sha256=-d8bHexyCOv7P5zVqbOL7bd4wEDzDlsizj6KGbPeCVI,31
+infinstor-2.0.9.dist-info/METADATA,sha256=Kx7HqjU9Ngx_BMVOWJF08ru8P09QCvbaG8zoUYKw9aU,798
+infinstor-2.0.9.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+infinstor-2.0.9.dist-info/top_level.txt,sha256=MW0CTQKThlkupD5bjg3zvNux77mwdeZ5ua_DVFuCi3s,10
+infinstor-2.0.9.dist-info/RECORD,,
```

