# Comparing `tmp/hytest-0.8.6-py3-none-any.whl.zip` & `tmp/hytest-0.8.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27528 bytes, number of entries: 17
+Zip file size: 27551 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat      131 b- defN 23-Jun-01 12:48 hytest/__init__.py
 -rw-rw-rw-  2.0 fat      958 b- defN 23-Jun-01 03:57 hytest/cfg.py
 -rw-rw-rw-  2.0 fat     3294 b- defN 23-Jun-01 13:15 hytest/common.py
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-01 03:35 hytest/product.py
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-03 14:04 hytest/product.py
 -rw-rw-rw-  2.0 fat     6718 b- defN 23-Jun-01 12:42 hytest/run.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-24 03:36 hytest/utils/__init__.py
--rw-rw-rw-  2.0 fat    31024 b- defN 23-Jun-02 10:17 hytest/utils/log.py
--rw-rw-rw-  2.0 fat     3471 b- defN 23-Feb-22 02:05 hytest/utils/report.css
+-rw-rw-rw-  2.0 fat    31114 b- defN 23-Jun-04 03:01 hytest/utils/log.py
+-rw-rw-rw-  2.0 fat     3476 b- defN 23-Jun-03 14:04 hytest/utils/report.css
 -rw-rw-rw-  2.0 fat     1891 b- defN 22-Sep-12 03:09 hytest/utils/report.js
 -rw-rw-rw-  2.0 fat    24790 b- defN 23-Jun-02 03:27 hytest/utils/runner.py
 -rw-rw-rw-  2.0 fat      571 b- defN 21-Jun-03 08:24 hytest/utils/signal.py
--rw-rw-rw-  2.0 fat    11535 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1244 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1309 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/RECORD
-17 files, 87093 bytes uncompressed, 25402 bytes compressed:  70.8%
+-rw-rw-rw-  2.0 fat    11535 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1244 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1309 b- defN 23-Jun-04 03:38 hytest-0.8.7.dist-info/RECORD
+17 files, 87188 bytes uncompressed, 25425 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: hytest/utils/runner.py
 Comment: 
 
 Filename: hytest/utils/signal.py
 Comment: 
 
-Filename: hytest-0.8.6.dist-info/LICENSE.txt
+Filename: hytest-0.8.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hytest-0.8.6.dist-info/METADATA
+Filename: hytest-0.8.7.dist-info/METADATA
 Comment: 
 
-Filename: hytest-0.8.6.dist-info/WHEEL
+Filename: hytest-0.8.7.dist-info/WHEEL
 Comment: 
 
-Filename: hytest-0.8.6.dist-info/entry_points.txt
+Filename: hytest-0.8.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: hytest-0.8.6.dist-info/top_level.txt
+Filename: hytest-0.8.7.dist-info/top_level.txt
 Comment: 
 
-Filename: hytest-0.8.6.dist-info/RECORD
+Filename: hytest-0.8.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hytest/product.py

```diff
@@ -1 +1 @@
-version= '0.8.6'
+version= '0.8.7'
```

## hytest/utils/log.py

```diff
@@ -367,18 +367,16 @@
         
     def checkpoint_fail(self, desc):
         logger.info((f'\n** 检查点 **  {desc} ---->  !! 不通过!!\n',
                      f'\n** checkpoint **  {desc} ---->  !! fail!!\n'
                      )[l.n])
 
 
-
-
     def log_img(self,imgPath: str, width: str = None):
-        logger.info(f'图 {imgPath}')
+        logger.info(f'picture {imgPath}')
 
 
 from dominate.tags import *
 from dominate.util import raw
 from dominate import document
 
 class HtmlLogger:
@@ -399,29 +397,29 @@
         self.doc.head.add(
                         meta(charset="UTF-8"),
                         style(raw(_css_style)),
                         script(raw(_js), type='text/javascript'))
 
         self.main = self.doc.body.add(div(_class='main_section'))
 
-        self.main.add(h1(f'{Settings.report_title} - hytest v{version}', style='font-family: auto'))
+        self.main.add(h1(f'{Settings.report_title}', style='font-family: auto'))
 
         self.main.add(h3(('统计结果','Test Statistics')[l.n]))
 
         resultDiv = self.main.add(div(_class='result'))
 
         self.result_table, self.result_barchart = resultDiv.add(
             table(_class='result_table'),
             div(_class='result_barchart')
         )
 
         _, self.logDiv = self.main.add(
             div(
                 # span('切换到精简模式',_class='h3_button', id='display_mode' ,onclick="toggle_folder_all_cases()"), 
-                h3(('执行日志','Test Log')[l.n],style='display:inline'),
+                h3(('执行日志','Test Execution Log')[l.n],style='display:inline'),
                 style='margin-top:2em'
             ),
             div(_class='exec_log')
         )
 
         # 查看上一个和下一个错误的 
         self.ev = div(
@@ -457,15 +455,17 @@
         execEndTime = time.strftime('%Y%m%d %H:%M:%S',
                                            time.localtime(stats.end_time))
 
         ret = stats.result
 
         errorNum = 0
 
-        trs = []
+        trs = []        
+        
+        trs.append(tr(td(('hytest 版本','hytest version')[l.n]), td(version)))
         trs.append(tr(td(('开始时间','Test Start Time')[l.n]), td(f'{execStartTime}')))
         trs.append(tr(td(('结束时间','Test End Time')[l.n]), td(f'{execEndTime}')))
 
         trs.append(tr(td(('耗时','Duration Of Testing')[l.n]), td(f'{stats.test_duration:.3f}' + (' 秒',' Seconds')[l.n])))
 
         trs.append(tr(td(('预备执行用例数量','number of cases plan to run')[l.n]), td(f"{ret['case_count_to_run']}")))
         trs.append(tr(td(('实际执用例行数量','number of cases actually run')[l.n]), td(f"{ret['case_count']}")))
```

## hytest/utils/report.css

```diff
@@ -79,15 +79,15 @@
     color: #03a9f4;
 }
 
 
 .info
 {
     white-space:pre-wrap;
-    padding: .6em;
+    margin: .8em 1.5em;
 }
 
 
 .error-info
 {
     color: #a64747
 }
```

## Comparing `hytest-0.8.6.dist-info/LICENSE.txt` & `hytest-0.8.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hytest-0.8.6.dist-info/METADATA` & `hytest-0.8.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hytest
-Version: 0.8.6
+Version: 0.8.7
 Summary: 一款系统测试自动化框架 Generic automation framework for QA testing
 Home-page: http://www.byhy.net
 Download-URL: https://pypi.python.org/pypi/hytest
 Author: 白月黑羽 - Jiangchunyang
 Author-email: jcyrss@gmail.com
 License: Apache License 2.0
 Keywords: hytest automation testautomation
```

## Comparing `hytest-0.8.6.dist-info/RECORD` & `hytest-0.8.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 hytest/__init__.py,sha256=5r0TGVbff3M6mDJlVjLNG31qLMHhtIEjtNrh15HiFXg,131
 hytest/cfg.py,sha256=aTV3ZGFPTyHpTtaZ5xrJDAKRloYx3ZBgBVJnWI8wvmE,958
 hytest/common.py,sha256=MvWfCs8eYcRunKjltvr9Sa7KmDCjpy-hIgqQd6Xsiz4,3294
-hytest/product.py,sha256=4VoXm3xeJFRoXE9ygSdtjyA-7OgkdhjJ0YroYmEapls,16
+hytest/product.py,sha256=yKM6atM7PTfxXxj0H-Rg15_SVoYKhpOPGe517aoU0Ew,16
 hytest/run.py,sha256=shI8HjiVEvl24eV6CgW_fkl2hjRjoDvE3jZR87oPKvg,6718
 hytest/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hytest/utils/log.py,sha256=EliB_g0V9-t9qwBvsbZFfAs3ov8hkRn7FUyJ8mkUBtQ,31024
-hytest/utils/report.css,sha256=Z5HA_BY7lNXHjJWu8ac7Z6_NlrO7jtARIsZqIrZcjAQ,3471
+hytest/utils/log.py,sha256=abKoDCSrHRirjR6ex03VM34H3TydA61xiZFa4dqlIBI,31114
+hytest/utils/report.css,sha256=ZU0NqixISjleCE-M7aLhCdMKThsWTQeL-GFBqpcLvuc,3476
 hytest/utils/report.js,sha256=WN6rsPyK0smI-1gL2CC1mk2fo3rTRgoBHzK3N_yZRXY,1891
 hytest/utils/runner.py,sha256=Tgjh_mPMC_ltujsKfVL6gMVI_zIaQbA8btwoBTw_aNY,24790
 hytest/utils/signal.py,sha256=J45d7BVO1e2oO0tfqWB26ozd0f1EDYT2kj56AtyP0OE,571
-hytest-0.8.6.dist-info/LICENSE.txt,sha256=KmdujD1z5SnrNIuBIyrwfCrwMpq0oMIfCVF_unj7hOA,11535
-hytest-0.8.6.dist-info/METADATA,sha256=_0Geytu5B37zCRzwWKWdLHjsl2bZi2RS7B_YqOvmNgQ,1244
-hytest-0.8.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hytest-0.8.6.dist-info/entry_points.txt,sha256=92p-5tIrvS1iq_ZMXOUEuhfjr3BDyfuWESt7FpeNP_k,42
-hytest-0.8.6.dist-info/top_level.txt,sha256=UQV_P0cF4XBYxd8wZW0nATrwbqWbWcMstjkj786kst0,7
-hytest-0.8.6.dist-info/RECORD,,
+hytest-0.8.7.dist-info/LICENSE.txt,sha256=KmdujD1z5SnrNIuBIyrwfCrwMpq0oMIfCVF_unj7hOA,11535
+hytest-0.8.7.dist-info/METADATA,sha256=LBSPq1Av6I4tbLW5HIn47HxR4zFYazttnEd1H2d7_mg,1244
+hytest-0.8.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hytest-0.8.7.dist-info/entry_points.txt,sha256=92p-5tIrvS1iq_ZMXOUEuhfjr3BDyfuWESt7FpeNP_k,42
+hytest-0.8.7.dist-info/top_level.txt,sha256=UQV_P0cF4XBYxd8wZW0nATrwbqWbWcMstjkj786kst0,7
+hytest-0.8.7.dist-info/RECORD,,
```

