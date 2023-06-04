# Comparing `tmp/hytest-0.8.7-py3-none-any.whl.zip` & `tmp/hytest-0.8.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27551 bytes, number of entries: 17
+Zip file size: 27612 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat      131 b- defN 23-Jun-01 12:48 hytest/__init__.py
 -rw-rw-rw-  2.0 fat      958 b- defN 23-Jun-01 03:57 hytest/cfg.py
 -rw-rw-rw-  2.0 fat     3294 b- defN 23-Jun-01 13:15 hytest/common.py
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-03 14:04 hytest/product.py
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-04 06:45 hytest/product.py
 -rw-rw-rw-  2.0 fat     6718 b- defN 23-Jun-01 12:42 hytest/run.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-24 03:36 hytest/utils/__init__.py
--rw-rw-rw-  2.0 fat    31114 b- defN 23-Jun-04 03:01 hytest/utils/log.py
+-rw-rw-rw-  2.0 fat    31221 b- defN 23-Jun-04 03:58 hytest/utils/log.py
 -rw-rw-rw-  2.0 fat     3476 b- defN 23-Jun-03 14:04 hytest/utils/report.css
 -rw-rw-rw-  2.0 fat     1891 b- defN 22-Sep-12 03:09 hytest/utils/report.js
 -rw-rw-rw-  2.0 fat    24790 b- defN 23-Jun-02 03:27 hytest/utils/runner.py
 -rw-rw-rw-  2.0 fat      571 b- defN 21-Jun-03 08:24 hytest/utils/signal.py
--rw-rw-rw-  2.0 fat    11535 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1244 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1309 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/RECORD
-17 files, 87188 bytes uncompressed, 25425 bytes compressed:  70.8%
+-rw-rw-rw-  2.0 fat    11535 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1244 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1309 b- defN 23-Jun-04 06:45 hytest-0.8.8.dist-info/RECORD
+17 files, 87295 bytes uncompressed, 25486 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: hytest/utils/runner.py
 Comment: 
 
 Filename: hytest/utils/signal.py
 Comment: 
 
-Filename: hytest-0.8.7.dist-info/LICENSE.txt
+Filename: hytest-0.8.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hytest-0.8.7.dist-info/METADATA
+Filename: hytest-0.8.8.dist-info/METADATA
 Comment: 
 
-Filename: hytest-0.8.7.dist-info/WHEEL
+Filename: hytest-0.8.8.dist-info/WHEEL
 Comment: 
 
-Filename: hytest-0.8.7.dist-info/entry_points.txt
+Filename: hytest-0.8.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: hytest-0.8.7.dist-info/top_level.txt
+Filename: hytest-0.8.8.dist-info/top_level.txt
 Comment: 
 
-Filename: hytest-0.8.7.dist-info/RECORD
+Filename: hytest-0.8.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hytest/product.py

```diff
@@ -1 +1 @@
-version= '0.8.7'
+version= '0.8.8'
```

## hytest/utils/log.py

```diff
@@ -423,20 +423,22 @@
 
         # 查看上一个和下一个错误的 
         self.ev = div(
                 div('∧', _class = 'menu-item', onclick="previous_error()", title='上一个错误'), 
                 div('∨', _class = 'menu-item', onclick="next_error()", title='下一个错误'),
                 _class = 'error_jumper'
             )
-         
+
+        helpLink = ("http://www.byhy.net/tut/auto/hytest/01",'https://github.com/jcyrss/hytest/Documentation.md') [l.n]
          
         self.doc.body.add(div(
             div(('页首','Home')[l.n], _class = 'menu-item',
                 onclick='document.querySelector("body").scrollIntoView()'),
-            div(('帮助','Help')[l.n], _class = 'menu-item', onclick='window.open("http://www.byhy.net/tut/auto/hytest/01", "_blank"); '),
+            div(('帮助','Help')[l.n], _class = 'menu-item', 
+                onclick=f'window.open("{helpLink}", "_blank"); '),
             div(('Summary','Summary')[l.n],_class='menu-item', id='display_mode' ,onclick="toggle_folder_all_cases()"),
             self.ev,
             id='float_menu')
         )
 
         self.curEle = self.main  # 记录当前所在的 html element
         self.curSuiteEle = None   # 记录当前的套件元素
@@ -446,17 +448,17 @@
         self.curTeardownEle = None   # 记录当前的清除元素
         self.suitepath2element = {}
 
 
     
     def test_end(self, runner):
 
-        execStartTime = time.strftime('%Y%m%d %H:%M:%S',
+        execStartTime = time.strftime('%Y/%m/%d %H:%M:%S',
                                            time.localtime(stats.start_time))
-        execEndTime = time.strftime('%Y%m%d %H:%M:%S',
+        execEndTime = time.strftime('%Y/%m/%d %H:%M:%S',
                                            time.localtime(stats.end_time))
 
         ret = stats.result
 
         errorNum = 0
 
         trs = []
```

## Comparing `hytest-0.8.7.dist-info/LICENSE.txt` & `hytest-0.8.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hytest-0.8.7.dist-info/METADATA` & `hytest-0.8.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hytest
-Version: 0.8.7
+Version: 0.8.8
 Summary: 一款系统测试自动化框架 Generic automation framework for QA testing
 Home-page: http://www.byhy.net
 Download-URL: https://pypi.python.org/pypi/hytest
 Author: 白月黑羽 - Jiangchunyang
 Author-email: jcyrss@gmail.com
 License: Apache License 2.0
 Keywords: hytest automation testautomation
```

## Comparing `hytest-0.8.7.dist-info/RECORD` & `hytest-0.8.8.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 hytest/__init__.py,sha256=5r0TGVbff3M6mDJlVjLNG31qLMHhtIEjtNrh15HiFXg,131
 hytest/cfg.py,sha256=aTV3ZGFPTyHpTtaZ5xrJDAKRloYx3ZBgBVJnWI8wvmE,958
 hytest/common.py,sha256=MvWfCs8eYcRunKjltvr9Sa7KmDCjpy-hIgqQd6Xsiz4,3294
-hytest/product.py,sha256=yKM6atM7PTfxXxj0H-Rg15_SVoYKhpOPGe517aoU0Ew,16
+hytest/product.py,sha256=5cFVpyfRuNdYtLdKgW8sKxTM45rMkn0CdgToszLL50Q,16
 hytest/run.py,sha256=shI8HjiVEvl24eV6CgW_fkl2hjRjoDvE3jZR87oPKvg,6718
 hytest/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hytest/utils/log.py,sha256=abKoDCSrHRirjR6ex03VM34H3TydA61xiZFa4dqlIBI,31114
+hytest/utils/log.py,sha256=X-kdFlGqrTIwCRNao_8Q6jQ6e7zJQG6vYhhFP7NiF5g,31221
 hytest/utils/report.css,sha256=ZU0NqixISjleCE-M7aLhCdMKThsWTQeL-GFBqpcLvuc,3476
 hytest/utils/report.js,sha256=WN6rsPyK0smI-1gL2CC1mk2fo3rTRgoBHzK3N_yZRXY,1891
 hytest/utils/runner.py,sha256=Tgjh_mPMC_ltujsKfVL6gMVI_zIaQbA8btwoBTw_aNY,24790
 hytest/utils/signal.py,sha256=J45d7BVO1e2oO0tfqWB26ozd0f1EDYT2kj56AtyP0OE,571
-hytest-0.8.7.dist-info/LICENSE.txt,sha256=KmdujD1z5SnrNIuBIyrwfCrwMpq0oMIfCVF_unj7hOA,11535
-hytest-0.8.7.dist-info/METADATA,sha256=LBSPq1Av6I4tbLW5HIn47HxR4zFYazttnEd1H2d7_mg,1244
-hytest-0.8.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hytest-0.8.7.dist-info/entry_points.txt,sha256=92p-5tIrvS1iq_ZMXOUEuhfjr3BDyfuWESt7FpeNP_k,42
-hytest-0.8.7.dist-info/top_level.txt,sha256=UQV_P0cF4XBYxd8wZW0nATrwbqWbWcMstjkj786kst0,7
-hytest-0.8.7.dist-info/RECORD,,
+hytest-0.8.8.dist-info/LICENSE.txt,sha256=KmdujD1z5SnrNIuBIyrwfCrwMpq0oMIfCVF_unj7hOA,11535
+hytest-0.8.8.dist-info/METADATA,sha256=GzXwh2aB1mgpPhljntperd8dYdwfX0lNLsByo4huZo0,1244
+hytest-0.8.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hytest-0.8.8.dist-info/entry_points.txt,sha256=92p-5tIrvS1iq_ZMXOUEuhfjr3BDyfuWESt7FpeNP_k,42
+hytest-0.8.8.dist-info/top_level.txt,sha256=UQV_P0cF4XBYxd8wZW0nATrwbqWbWcMstjkj786kst0,7
+hytest-0.8.8.dist-info/RECORD,,
```

