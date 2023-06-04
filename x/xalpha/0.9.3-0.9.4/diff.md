# Comparing `tmp/xalpha-0.9.3.tar.gz` & `tmp/xalpha-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xalpha-0.9.3.tar", last modified: Sat Jun 20 01:34:35 2020, max compression
+gzip compressed data, was "dist/xalpha-0.9.4.tar", last modified: Thu Jul  2 10:51:02 2020, max compression
```

## Comparing `xalpha-0.9.3.tar` & `xalpha-0.9.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 shixin     (502) staff       (20)        0 2020-06-20 01:34:35.000000 xalpha-0.9.3/
-drwxr-xr-x   0 shixin     (502) staff       (20)        0 2020-06-20 01:34:35.000000 xalpha-0.9.3/xalpha/
--rw-r--r--   0 shixin     (502) staff       (20)     8339 2020-05-25 07:53:11.000000 xalpha-0.9.3/xalpha/misc.py
--rw-r--r--   0 shixin     (502) staff       (20)     4342 2020-03-30 12:36:23.000000 xalpha-0.9.3/xalpha/provider.py
--rw-r--r--   0 shixin     (502) staff       (20)     6870 2020-04-14 12:17:39.000000 xalpha-0.9.3/xalpha/realtime.py
--rw-r--r--   0 shixin     (502) staff       (20)    29968 2020-06-05 00:56:48.000000 xalpha-0.9.3/xalpha/trade.py
--rw-r--r--   0 shixin     (502) staff       (20)     3469 2020-01-03 03:47:22.000000 xalpha-0.9.3/xalpha/remain.py
--rw-r--r--   0 shixin     (502) staff       (20)    70728 2020-06-05 02:55:52.000000 xalpha-0.9.3/xalpha/toolbox.py
--rw-r--r--   0 shixin     (502) staff       (20)    23522 2020-06-05 00:49:43.000000 xalpha-0.9.3/xalpha/multiple.py
--rw-r--r--   0 shixin     (502) staff       (20)    25325 2020-05-02 02:51:57.000000 xalpha-0.9.3/xalpha/indicator.py
--rw-r--r--   0 shixin     (502) staff       (20)    12722 2020-04-05 10:43:33.000000 xalpha-0.9.3/xalpha/policy.py
--rw-r--r--   0 shixin     (502) staff       (20)     1043 2020-06-20 01:19:06.000000 xalpha-0.9.3/xalpha/__init__.py
--rw-r--r--   0 shixin     (502) staff       (20)   142471 2020-02-03 11:05:26.000000 xalpha-0.9.3/xalpha/caldate.csv
--rw-r--r--   0 shixin     (502) staff       (20)     8693 2020-06-20 00:40:35.000000 xalpha-0.9.3/xalpha/record.py
--rw-r--r--   0 shixin     (502) staff       (20)     1345 2020-03-29 15:01:45.000000 xalpha-0.9.3/xalpha/exceptions.py
--rw-r--r--   0 shixin     (502) staff       (20)     4551 2020-01-03 03:47:22.000000 xalpha-0.9.3/xalpha/evaluate.py
--rw-r--r--   0 shixin     (502) staff       (20)    53292 2020-06-20 00:30:01.000000 xalpha-0.9.3/xalpha/info.py
--rw-r--r--   0 shixin     (502) staff       (20)    15092 2020-04-30 07:57:40.000000 xalpha-0.9.3/xalpha/cons.py
--rw-r--r--   0 shixin     (502) staff       (20)    91615 2020-06-12 06:07:16.000000 xalpha-0.9.3/xalpha/universal.py
--rw-r--r--   0 shixin     (502) staff       (20)     6039 2020-06-20 01:34:35.000000 xalpha-0.9.3/PKG-INFO
--rw-r--r--   0 shixin     (502) staff       (20)       26 2020-02-19 06:57:39.000000 xalpha-0.9.3/MANIFEST.in
--rw-r--r--   0 shixin     (502) staff       (20)     4488 2020-05-25 04:10:10.000000 xalpha-0.9.3/README.md
--rw-r--r--   0 shixin     (502) staff       (20)     1516 2020-06-20 01:19:02.000000 xalpha-0.9.3/setup.py
--rw-r--r--   0 shixin     (502) staff       (20)       38 2020-06-20 01:34:35.000000 xalpha-0.9.3/setup.cfg
-drwxr-xr-x   0 shixin     (502) staff       (20)        0 2020-06-20 01:34:35.000000 xalpha-0.9.3/xalpha.egg-info/
--rw-r--r--   0 shixin     (502) staff       (20)     6039 2020-06-20 01:34:34.000000 xalpha-0.9.3/xalpha.egg-info/PKG-INFO
--rw-r--r--   0 shixin     (502) staff       (20)      484 2020-06-20 01:34:34.000000 xalpha-0.9.3/xalpha.egg-info/SOURCES.txt
--rw-r--r--   0 shixin     (502) staff       (20)      114 2020-06-20 01:34:34.000000 xalpha-0.9.3/xalpha.egg-info/requires.txt
--rw-r--r--   0 shixin     (502) staff       (20)        7 2020-06-20 01:34:34.000000 xalpha-0.9.3/xalpha.egg-info/top_level.txt
--rw-r--r--   0 shixin     (502) staff       (20)        1 2020-06-20 01:34:34.000000 xalpha-0.9.3/xalpha.egg-info/dependency_links.txt
+drwxr-xr-x   0 shixin     (502) staff       (20)        0 2020-07-02 10:51:02.000000 xalpha-0.9.4/
+drwxr-xr-x   0 shixin     (502) staff       (20)        0 2020-07-02 10:51:02.000000 xalpha-0.9.4/xalpha/
+-rw-r--r--   0 shixin     (502) staff       (20)     8339 2020-05-25 07:53:11.000000 xalpha-0.9.4/xalpha/misc.py
+-rw-r--r--   0 shixin     (502) staff       (20)     4342 2020-03-30 12:36:23.000000 xalpha-0.9.4/xalpha/provider.py
+-rw-r--r--   0 shixin     (502) staff       (20)     6870 2020-04-14 12:17:39.000000 xalpha-0.9.4/xalpha/realtime.py
+-rw-r--r--   0 shixin     (502) staff       (20)    30299 2020-06-25 06:12:33.000000 xalpha-0.9.4/xalpha/trade.py
+-rw-r--r--   0 shixin     (502) staff       (20)     3469 2020-01-03 03:47:22.000000 xalpha-0.9.4/xalpha/remain.py
+-rw-r--r--   0 shixin     (502) staff       (20)    70781 2020-06-26 23:54:00.000000 xalpha-0.9.4/xalpha/toolbox.py
+-rw-r--r--   0 shixin     (502) staff       (20)    23522 2020-06-05 00:49:43.000000 xalpha-0.9.4/xalpha/multiple.py
+-rw-r--r--   0 shixin     (502) staff       (20)    25325 2020-05-02 02:51:57.000000 xalpha-0.9.4/xalpha/indicator.py
+-rw-r--r--   0 shixin     (502) staff       (20)    12722 2020-04-05 10:43:33.000000 xalpha-0.9.4/xalpha/policy.py
+-rw-r--r--   0 shixin     (502) staff       (20)     1043 2020-07-02 10:50:00.000000 xalpha-0.9.4/xalpha/__init__.py
+-rw-r--r--   0 shixin     (502) staff       (20)   142471 2020-02-03 11:05:26.000000 xalpha-0.9.4/xalpha/caldate.csv
+-rw-r--r--   0 shixin     (502) staff       (20)     8890 2020-07-02 10:49:38.000000 xalpha-0.9.4/xalpha/record.py
+-rw-r--r--   0 shixin     (502) staff       (20)     1345 2020-03-29 15:01:45.000000 xalpha-0.9.4/xalpha/exceptions.py
+-rw-r--r--   0 shixin     (502) staff       (20)     4709 2020-06-21 02:06:13.000000 xalpha-0.9.4/xalpha/evaluate.py
+-rw-r--r--   0 shixin     (502) staff       (20)    53292 2020-06-20 00:30:01.000000 xalpha-0.9.4/xalpha/info.py
+-rw-r--r--   0 shixin     (502) staff       (20)    15092 2020-04-30 07:57:40.000000 xalpha-0.9.4/xalpha/cons.py
+-rw-r--r--   0 shixin     (502) staff       (20)    91861 2020-07-02 10:08:49.000000 xalpha-0.9.4/xalpha/universal.py
+-rw-r--r--   0 shixin     (502) staff       (20)     6039 2020-07-02 10:51:02.000000 xalpha-0.9.4/PKG-INFO
+-rw-r--r--   0 shixin     (502) staff       (20)       26 2020-02-19 06:57:39.000000 xalpha-0.9.4/MANIFEST.in
+-rw-r--r--   0 shixin     (502) staff       (20)     4488 2020-05-25 04:10:10.000000 xalpha-0.9.4/README.md
+-rw-r--r--   0 shixin     (502) staff       (20)     1516 2020-07-02 10:50:11.000000 xalpha-0.9.4/setup.py
+-rw-r--r--   0 shixin     (502) staff       (20)       38 2020-07-02 10:51:02.000000 xalpha-0.9.4/setup.cfg
+drwxr-xr-x   0 shixin     (502) staff       (20)        0 2020-07-02 10:51:02.000000 xalpha-0.9.4/xalpha.egg-info/
+-rw-r--r--   0 shixin     (502) staff       (20)     6039 2020-07-02 10:51:01.000000 xalpha-0.9.4/xalpha.egg-info/PKG-INFO
+-rw-r--r--   0 shixin     (502) staff       (20)      484 2020-07-02 10:51:01.000000 xalpha-0.9.4/xalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 shixin     (502) staff       (20)      114 2020-07-02 10:51:01.000000 xalpha-0.9.4/xalpha.egg-info/requires.txt
+-rw-r--r--   0 shixin     (502) staff       (20)        7 2020-07-02 10:51:01.000000 xalpha-0.9.4/xalpha.egg-info/top_level.txt
+-rw-r--r--   0 shixin     (502) staff       (20)        1 2020-07-02 10:51:01.000000 xalpha-0.9.4/xalpha.egg-info/dependency_links.txt
```

### Comparing `xalpha-0.9.3/xalpha/misc.py` & `xalpha-0.9.4/xalpha/misc.py`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/provider.py` & `xalpha-0.9.4/xalpha/provider.py`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/realtime.py` & `xalpha-0.9.4/xalpha/realtime.py`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/trade.py` & `xalpha-0.9.4/xalpha/trade.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,23 +130,27 @@
         #     dt.datetime.strptime(str(a) + "4", "(%Y, %W)%w")
         #     for a, _ in cfmerge.iteritems()
         # ]
         datedata = pd.date_range(
             startdate, yesterdayobj() + pd.Timedelta(days=7), freq="W-THU"
         )
         selldata = [
-            [dt.datetime.strptime(str(a) + "4", "(%Y, %W)%w"), b]
+            [dt.datetime.strptime(str(a) + "4", "(%G, %V)%w"), b]
             for a, b in cfmerge.iteritems()
             if b > 0
         ]
         buydata = [
-            [dt.datetime.strptime(str(a) + "4", "(%Y, %W)%w"), b]
+            [dt.datetime.strptime(str(a) + "4", "(%G, %V)%w"), b]
             for a, b in cfmerge.iteritems()
             if b < 0
         ]
+        # %V pandas gives iso weeknumber which is different from python original %W or %U,
+        # see https://stackoverflow.com/questions/5882405/get-date-from-iso-week-number-in-python for more details
+        # python3.6+ required for %G and %V
+        # but now seems no equal distance between sell and buy data, no idea why
     elif freq == "M":
         cfmerge = cftable.groupby([cftable["date"].dt.year, cftable["date"].dt.month])[
             "cash"
         ].sum()
         # datedata = [
         #     dt.datetime.strptime(str(a) + "15", "(%Y, %m)%d")
         #     for a, _ in cfmerge.iteritems()
```

### Comparing `xalpha-0.9.3/xalpha/remain.py` & `xalpha-0.9.4/xalpha/remain.py`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/toolbox.py` & `xalpha-0.9.4/xalpha/toolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -716,15 +716,18 @@
         if i >= passed:
             cf.append((issue_date_obj + dt.timedelta(days=(i + 1) * 365), r * tax))
     # 关于赎回利息计算： https://www.jisilu.cn/?/question/339
     # https://www.jisilu.cn/question/5807
     # 富投网的算法：将最后一年超出100的部分，全部按照20%计税，
     cf.append((issue_date_obj + dt.timedelta(days=(len(rlist) - 1) * 365), rlist[-1]))
     #     print(cf)
-    return xirr(cf, guess=guess)
+    try:
+        return xirr(cf, guess=guess)
+    except RuntimeError:
+        return
 
 
 class CBCalculator:
     """
     可转债内在价值，简单计算器，期权价值与债券价值估算
     """
```

### Comparing `xalpha-0.9.3/xalpha/multiple.py` & `xalpha-0.9.4/xalpha/multiple.py`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/indicator.py` & `xalpha-0.9.4/xalpha/indicator.py`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/policy.py` & `xalpha-0.9.4/xalpha/policy.py`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/__init__.py` & `xalpha-0.9.4/xalpha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 __author__ = "refraction-ray"
 __name__ = "xalpha"
 
 import xalpha.policy
 import xalpha.remain
 import xalpha.misc
 import xalpha.exceptions
```

### Comparing `xalpha-0.9.3/xalpha/caldate.csv` & `xalpha-0.9.4/xalpha/caldate.csv`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/record.py` & `xalpha-0.9.4/xalpha/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,29 @@
     ``record(path, fund_property=True)`` 设定 fund_property 参数, 或直接在记账单第二行日期栏写上 property 即可。每个基金代码对应一个 0 到 7 的数字。
     也可为空，默认为 0。
 
     此外如不改变记账单，也可在 :class:`xalpha.multiple.mul` 类初始化时，传入 property=dict, 字典内容为 {"基金代码"：0-7 数字}。默认为0的代码可不添加。
 
     对于不同格式的记账单的例子，可在 github repo 中 tests 文件夹内的 demo*.csv 参考。
 
-    :param path: string for the csv file path
+    :param path: string for the csv file path or pd.DataFrame
     :param format: str. Default is "matrix". Can also be "list"。list 形式的账单更类似流水单。总共三列，每行由日期基金号和金额组成。
                 三栏标题分别为 date，fund 和 trade。其中日期的形式是 %Y/%m/%d. 该形式与默认的 matrix 不包含 "/" 不同。
     :param fund_property: bool. Default False. If True, 基金号下第一行的数字标记对应基金参数（暂时只支持 matrix 形式账单）。
     :param readkwds: keywords options for pandas.read_csv() function. eg. skiprows=1, skipfooter=2,
         see more on `pandas doc <https://pandas.pydata.org/pandas-docs/stable/generated/pandas.read_csv.html>`_.
     """
 
     def __init__(
         self, path="input.csv", format="matrix", fund_property=False, **readkwds
     ):
-        df = pd.read_csv(path, **readkwds)
+        if isinstance(path, str):
+            df = pd.read_csv(path, **readkwds)
+        else:  # path itself is a pd.DataFrame
+            df = path
         if df.iloc[0]["date"] == "property":
             fund_property = True
         if format == "matrix":
             df.fillna(0, inplace=True)
             df.columns = ["date"] + [
                 c.zfill(6) if c.isdigit() else c for c in df.columns[1:]
             ]
@@ -127,15 +130,18 @@
     代码格式与 :func:`xalpha.universal.get_daily` 要求相同。对于常见的 A 股标的，格式为 SH501018。
     value 列记录买入卖出或场内申购赎回对应的成交净值单价。share 记录实际上份额的增减，正数代表买入。
     fee 栏对应了每笔交易实际的佣金，也可不记录，则默认均为0。记账单不要求严格按时间排序。
     该类处理的记账单可以提供给 :class:`xalpha.trade.itrade` 和 :class:`xalpha.multiple.imul` 使用，进行场内交易的整合分析。
     """
 
     def __init__(self, path="input.csv", **readkwds):
-        df = pd.read_csv(path, **readkwds)
+        if isinstance(path, str):
+            df = pd.read_csv(path, **readkwds)
+        else:
+            df = path
         df.fillna(0, inplace=True)
         df.date = [
             pd.to_datetime(df.iloc[i].date, format="%Y%m%d") for i in range(len(df))
         ]
         if "fee" not in df.columns:
             df = df.assign(fee=[0] * len(df))
         df = df.sort_values(by="date", ascending=True)
```

### Comparing `xalpha-0.9.3/xalpha/exceptions.py` & `xalpha-0.9.4/xalpha/exceptions.py`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/evaluate.py` & `xalpha-0.9.4/xalpha/evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 self.start = start
                 self.totprice = self.totprice[self.totprice["date"] >= self.start]
         self.totprice = self.totprice.reset_index(drop=True)
         for col in self.totprice.columns:
             if col != "date":
                 self.totprice[col] = self.totprice[col] / self.totprice[col].iloc[0]
 
-    def v_netvalue(self, end=yesterdayobj(), vopts=None):
+    def v_netvalue(self, end=yesterdayobj(), vopts=None, rendered=True):
         """
         起点对齐归一的，各参考基金或指数的净值比较可视化
 
         :param end: string or object of date, the end date of the line
         :param vkwds: pyechart line.add() options
         :param vopts: dict, options for pyecharts instead of builtin settings
         :returns: pyecharts.charts.Line.render_notebook()
@@ -68,28 +68,31 @@
         line.add_xaxis([d.date() for d in list(partprice.date)])
         for fund in self.fundobjs:
             line.add_yaxis(
                 series_name=fund.name,
                 y_axis=list(partprice[fund.code]),
                 is_symbol_show=False,
             )
-        return line.render_notebook()
+        if rendered:
+            return line.render_notebook()
+        else:
+            return line
 
     def correlation_table(self, end=yesterdayobj()):
         """
         give the correlation coefficient amongst referenced funds and indexes
 
         :param end: string or object of date, the end date of the line
         :returns: pandas DataFrame, with correlation coefficient as elements
         """
         partprice = self.totprice[self.totprice["date"] <= end]
         covtable = partprice.iloc[:, 1:].pct_change().corr()
         return covtable
 
-    def v_correlation(self, end=yesterdayobj(), vopts=None):
+    def v_correlation(self, end=yesterdayobj(), vopts=None, rendered=True):
         """
         各基金净值的相关程度热力图可视化
 
         :param end: string or object of date, the end date of the line
         :returns: pyecharts.charts.Heatmap.render_notebook object
         """
         ctable = self.correlation_table(end)
@@ -101,9 +104,11 @@
         ]
         heatmap = HeatMap()
         heatmap.add_xaxis(x_axis)
         heatmap.add_yaxis(series_name="相关性", yaxis_data=x_axis, value=data)
         if vopts is None:
             vopts = heatmap_opts
         heatmap.set_global_opts(**vopts)
-
-        return heatmap.render_notebook()
+        if rendered:
+            return heatmap.render_notebook()
+        else:
+            return heatmap
```

### Comparing `xalpha-0.9.3/xalpha/info.py` & `xalpha-0.9.4/xalpha/info.py`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/cons.py` & `xalpha-0.9.4/xalpha/cons.py`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/xalpha/universal.py` & `xalpha-0.9.4/xalpha/universal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1717,14 +1717,17 @@
             else:
                 code = kws.get("code")
             date = ioconf.get("date", "date")  # 没利用上这个栏的名字变化
             precached = ioconf.get("precached", None)
             precached = kws.get("precached", precached)
             key = kws.get("key", code)
             key = key.replace("/", " ")
+            key_func = ioconf.get("key_func", None)
+            if key_func is not None:
+                key = key_func(key)
             defaultend = ioconf.get("defaultend", today_obj)
             defaultend = ioconf.get("default_end", defaultend)
             defaultprev = ioconf.get("defaultprev", 365)
             defaultprev = ioconf.get("default_prev", defaultprev)
             if isinstance(defaultend, str):
                 defaultend = defaultend.replace("/", "").replace("-", "")
                 defaultend = dt.datetime.strptime(defaultend, "%Y%m%d")
@@ -1754,14 +1757,16 @@
                     start.replace("/", "").replace("-", ""), "%Y%m%d"
                 )
 
             start_str = start_obj.strftime("%Y%m%d")
             end_str = end_obj.strftime("%Y%m%d")
             backend = ioconf.get("backend")
             backend = kws.get("backend", backend)
+            # if backend == "sql": # reserved for case insensitive database settings
+            #     key = key.lower()
             refresh = ioconf.get("refresh", False)
             refresh = kws.get("refresh", refresh)
             fetchonly = ioconf.get("fetchonly", False)
             fetchonly = ioconf.get("fetch_only", fetchonly)
             fetchonly = kws.get("fetchonly", fetchonly)
             fetchonly = kws.get("fetch_only", fetchonly)
             path = ioconf.get("path")
```

### Comparing `xalpha-0.9.3/PKG-INFO` & `xalpha-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xalpha
-Version: 0.9.3
+Version: 0.9.4
 Summary: all about fund investment
 Home-page: https://github.com/refraction-ray/xalpha
 Author: refraction-ray
 Author-email: refraction-ray@protonmail.com
 License: UNKNOWN
 Description: xalpha
         ========
```

### Comparing `xalpha-0.9.3/README.md` & `xalpha-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `xalpha-0.9.3/setup.py` & `xalpha-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 for f in excludes:
     absf = os.path.join(os.getcwd(), "xalpha", f)
     if os.path.exists(absf):
         shutil.move(absf, os.path.join(os.getcwd(), "xalpha", f + ".keep"))
 
 setuptools.setup(
     name="xalpha",
-    version="0.9.3",
+    version="0.9.4",
     author="refraction-ray",
     author_email="refraction-ray@protonmail.com",
     description="all about fund investment",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/refraction-ray/xalpha",
     packages=setuptools.find_packages(),
```

### Comparing `xalpha-0.9.3/xalpha.egg-info/PKG-INFO` & `xalpha-0.9.4/xalpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xalpha
-Version: 0.9.3
+Version: 0.9.4
 Summary: all about fund investment
 Home-page: https://github.com/refraction-ray/xalpha
 Author: refraction-ray
 Author-email: refraction-ray@protonmail.com
 License: UNKNOWN
 Description: xalpha
         ========
```

