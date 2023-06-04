# Comparing `tmp/hytest-0.8.8-py3-none-any.whl.zip` & `tmp/hytest-0.8.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27612 bytes, number of entries: 17
+Zip file size: 27790 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat      131 b- defN 23-Jun-01 12:48 hytest/__init__.py
 -rw-rw-rw-  2.0 fat      958 b- defN 23-Jun-01 03:57 hytest/cfg.py
 -rw-rw-rw-  2.0 fat     3294 b- defN 23-Jun-01 13:15 hytest/common.py
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-04 06:45 hytest/product.py
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-04 10:19 hytest/product.py
 -rw-rw-rw-  2.0 fat     6718 b- defN 23-Jun-01 12:42 hytest/run.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-24 03:36 hytest/utils/__init__.py
 -rw-rw-rw-  2.0 fat    31221 b- defN 23-Jun-04 03:58 hytest/utils/log.py
 -rw-rw-rw-  2.0 fat     3476 b- defN 23-Jun-03 14:04 hytest/utils/report.css
 -rw-rw-rw-  2.0 fat     1891 b- defN 22-Sep-12 03:09 hytest/utils/report.js
 -rw-rw-rw-  2.0 fat    24790 b- defN 23-Jun-02 03:27 hytest/utils/runner.py
 -rw-rw-rw-  2.0 fat      571 b- defN 21-Jun-03 08:24 hytest/utils/signal.py
--rw-rw-rw-  2.0 fat    11535 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1244 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1309 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/RECORD
-17 files, 87295 bytes uncompressed, 25486 bytes compressed:  70.8%
+-rw-rw-rw-  2.0 fat    11535 b- defN 23-Jun-04 10:47 hytest-0.8.9.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1802 b- defN 23-Jun-04 10:47 hytest-0.8.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 10:47 hytest-0.8.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-04 10:47 hytest-0.8.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-04 10:47 hytest-0.8.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1309 b- defN 23-Jun-04 10:47 hytest-0.8.9.dist-info/RECORD
+17 files, 87853 bytes uncompressed, 25664 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: hytest/utils/runner.py
 Comment: 
 
 Filename: hytest/utils/signal.py
 Comment: 
 
-Filename: hytest-0.8.8.dist-info/LICENSE.txt
+Filename: hytest-0.8.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hytest-0.8.8.dist-info/METADATA
+Filename: hytest-0.8.9.dist-info/METADATA
 Comment: 
 
-Filename: hytest-0.8.8.dist-info/WHEEL
+Filename: hytest-0.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: hytest-0.8.8.dist-info/entry_points.txt
+Filename: hytest-0.8.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: hytest-0.8.8.dist-info/top_level.txt
+Filename: hytest-0.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: hytest-0.8.8.dist-info/RECORD
+Filename: hytest-0.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hytest/product.py

```diff
@@ -1 +1 @@
-version= '0.8.8'
+version= '0.8.9'
```

## Comparing `hytest-0.8.8.dist-info/LICENSE.txt` & `hytest-0.8.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hytest-0.8.8.dist-info/RECORD` & `hytest-0.8.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 hytest/__init__.py,sha256=5r0TGVbff3M6mDJlVjLNG31qLMHhtIEjtNrh15HiFXg,131
 hytest/cfg.py,sha256=aTV3ZGFPTyHpTtaZ5xrJDAKRloYx3ZBgBVJnWI8wvmE,958
 hytest/common.py,sha256=MvWfCs8eYcRunKjltvr9Sa7KmDCjpy-hIgqQd6Xsiz4,3294
-hytest/product.py,sha256=5cFVpyfRuNdYtLdKgW8sKxTM45rMkn0CdgToszLL50Q,16
+hytest/product.py,sha256=72WCduogC7TIYiEGsoMXUgURNN45hNT9Ee_YUuKEDdE,16
 hytest/run.py,sha256=shI8HjiVEvl24eV6CgW_fkl2hjRjoDvE3jZR87oPKvg,6718
 hytest/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hytest/utils/log.py,sha256=X-kdFlGqrTIwCRNao_8Q6jQ6e7zJQG6vYhhFP7NiF5g,31221
 hytest/utils/report.css,sha256=ZU0NqixISjleCE-M7aLhCdMKThsWTQeL-GFBqpcLvuc,3476
 hytest/utils/report.js,sha256=WN6rsPyK0smI-1gL2CC1mk2fo3rTRgoBHzK3N_yZRXY,1891
 hytest/utils/runner.py,sha256=Tgjh_mPMC_ltujsKfVL6gMVI_zIaQbA8btwoBTw_aNY,24790
 hytest/utils/signal.py,sha256=J45d7BVO1e2oO0tfqWB26ozd0f1EDYT2kj56AtyP0OE,571
-hytest-0.8.8.dist-info/LICENSE.txt,sha256=KmdujD1z5SnrNIuBIyrwfCrwMpq0oMIfCVF_unj7hOA,11535
-hytest-0.8.8.dist-info/METADATA,sha256=GzXwh2aB1mgpPhljntperd8dYdwfX0lNLsByo4huZo0,1244
-hytest-0.8.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hytest-0.8.8.dist-info/entry_points.txt,sha256=92p-5tIrvS1iq_ZMXOUEuhfjr3BDyfuWESt7FpeNP_k,42
-hytest-0.8.8.dist-info/top_level.txt,sha256=UQV_P0cF4XBYxd8wZW0nATrwbqWbWcMstjkj786kst0,7
-hytest-0.8.8.dist-info/RECORD,,
+hytest-0.8.9.dist-info/LICENSE.txt,sha256=KmdujD1z5SnrNIuBIyrwfCrwMpq0oMIfCVF_unj7hOA,11535
+hytest-0.8.9.dist-info/METADATA,sha256=7LSR4d8iUa1Tv1QvGohOc99bgXIMqNDKYzmMSVlruuU,1802
+hytest-0.8.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hytest-0.8.9.dist-info/entry_points.txt,sha256=92p-5tIrvS1iq_ZMXOUEuhfjr3BDyfuWESt7FpeNP_k,42
+hytest-0.8.9.dist-info/top_level.txt,sha256=UQV_P0cF4XBYxd8wZW0nATrwbqWbWcMstjkj786kst0,7
+hytest-0.8.9.dist-info/RECORD,,
```

