# Comparing `tmp/aklite-0.0.1.tar.gz` & `tmp/aklite-0.0.2.tar.gz`

## Comparing `aklite-0.0.1.tar` & `aklite-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 aklite-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 aklite-0.0.1/requirements.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 aklite-0.0.1/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 aklite-0.0.1/docs/make.bat
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 aklite-0.0.1/docs/requirements.txt
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 aklite-0.0.1/docs/locales/zh_CN/LC_MESSAGES/index.po
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 aklite-0.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aklite-0.0.1/docs/source/index.rst
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 aklite-0.0.1/src/aklite/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aklite-0.0.1/src/aklite/stock/__init__.py
--rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 aklite-0.0.1/src/aklite/stock/stock_hist_em.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aklite-0.0.1/tests/test_ak.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 aklite-0.0.1/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 aklite-0.0.1/LICENSE
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aklite-0.0.1/README.md
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 aklite-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 aklite-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aklite-0.0.2/.readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 aklite-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aklite-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/locales/zh_CN/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/locales/zh_CN/LC_MESSAGES/notebooks/stock.po
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 aklite-0.0.2/docs/source/notebooks/stock.ipynb
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 aklite-0.0.2/src/aklite/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aklite-0.0.2/src/aklite/stock/__init__.py
+-rw-r--r--   0        0        0     6957 2020-02-02 00:00:00.000000 aklite-0.0.2/src/aklite/stock/stock_hist_em.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 aklite-0.0.2/tests/test_ak.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 aklite-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 aklite-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aklite-0.0.2/README.md
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 aklite-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 aklite-0.0.2/PKG-INFO
```

### Comparing `aklite-0.0.1/src/aklite/stock/stock_hist_em.py` & `aklite-0.0.2/src/aklite/stock/stock_hist_em.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from functools import lru_cache
 
 import pandas as pd
-import requests
+import httpx
+from typing import Union
 
 
 @lru_cache()
-def code_id_map_em() -> dict:
+def _code_id_map_em() -> dict:
     """
     东方财富-股票和市场代码
     http://quote.eastmoney.com/center/gridlist.html#hs_a_board
     :return: 股票和市场代码
     :rtype: dict
     """
     url = "http://80.push2.eastmoney.com/api/qt/clist/get"
@@ -22,15 +23,15 @@
         "fltt": "2",
         "invt": "2",
         "fid": "f3",
         "fs": "m:1 t:2,m:1 t:23",
         "fields": "f12",
         "_": "1623833739532",
     }
-    r = requests.get(url, params=params)
+    r = httpx.get(url, params=params)
     data_json = r.json()
     if not data_json["data"]["diff"]:
         return dict()
     temp_df = pd.DataFrame(data_json["data"]["diff"])
     temp_df["market_id"] = 1
     temp_df.columns = ["sh_code", "sh_id"]
     code_id_dict = dict(zip(temp_df["sh_code"], temp_df["sh_id"]))
@@ -43,15 +44,15 @@
         "fltt": "2",
         "invt": "2",
         "fid": "f3",
         "fs": "m:0 t:6,m:0 t:80",
         "fields": "f12",
         "_": "1623833739532",
     }
-    r = requests.get(url, params=params)
+    r = httpx.get(url, params=params)
     data_json = r.json()
     if not data_json["data"]["diff"]:
         return dict()
     temp_df_sz = pd.DataFrame(data_json["data"]["diff"])
     temp_df_sz["sz_id"] = 0
     code_id_dict.update(dict(zip(temp_df_sz["f12"], temp_df_sz["sz_id"])))
     params = {
@@ -63,99 +64,144 @@
         "fltt": "2",
         "invt": "2",
         "fid": "f3",
         "fs": "m:0 t:81 s:2048",
         "fields": "f12",
         "_": "1623833739532",
     }
-    r = requests.get(url, params=params)
+    r = httpx.get(url, params=params)
     data_json = r.json()
     if not data_json["data"]["diff"]:
         return dict()
     temp_df_sz = pd.DataFrame(data_json["data"]["diff"])
     temp_df_sz["bj_id"] = 0
     code_id_dict.update(dict(zip(temp_df_sz["f12"], temp_df_sz["bj_id"])))
     return code_id_dict
 
 
-def stock_zh_a_hist(
-        symbol: str = "000001",
-        period: str = "daily",
-        start_date: str = "19700101",
-        end_date: str = "20500101",
-        adjust: str = "",
-) -> pd.DataFrame:
-    """
-    东方财富网-行情首页-沪深京 A 股-每日行情
-    https://quote.eastmoney.com/concept/sh603777.html?from=classic
-    :param symbol: 股票代码
-    :type symbol: str
-    :param period: choice of {'daily', 'weekly', 'monthly'}
-    :type period: str
-    :param start_date: 开始日期
-    :type start_date: str
-    :param end_date: 结束日期
-    :type end_date: str
-    :param adjust: choice of {"qfq": "前复权", "hfq": "后复权", "": "不复权"}
-    :type adjust: str
-    :return: 每日行情
-    :rtype: pandas.DataFrame
-    """
-    code_id_dict = code_id_map_em()
-    adjust_dict = {"qfq": "1", "hfq": "2", "": "0"}
-    period_dict = {"daily": "101", "weekly": "102", "monthly": "103"}
-    url = "http://push2his.eastmoney.com/api/qt/stock/kline/get"
-    params = {
-        "fields1": "f1,f2,f3,f4,f5,f6",
-        "fields2": "f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61,f116",
-        "ut": "7eea3edcaed734bea9cbfc24409ed989",
-        "klt": period_dict[period],
-        "fqt": adjust_dict[adjust],
-        "secid": f"{code_id_dict[symbol]}.{symbol}",
-        "beg": start_date,
-        "end": end_date,
-        "_": "1623766962675",
-    }
-    r = requests.get(url, params=params)
-    data_json = r.json()
-    if not (data_json["data"] and data_json["data"]["klines"]):
-        return pd.DataFrame()
-    temp_df = pd.DataFrame(
-        [item.split(",") for item in data_json["data"]["klines"]]
-    )
-    temp_df.columns = [
-        "日期",
-        "开盘",
-        "收盘",
-        "最高",
-        "最低",
-        "成交量",
-        "成交额",
-        "振幅",
-        "涨跌幅",
-        "涨跌额",
-        "换手率",
+class StockZhAHist:
+    _columns = [
+        '日期', "股票代码", '开盘', '收盘', '最高', '最低', '成交量',
+        '成交额', '振幅', '涨跌幅', '涨跌额', '换手率'
     ]
-    temp_df.index = pd.to_datetime(temp_df["日期"])
-    temp_df.reset_index(inplace=True, drop=True)
+    _url = "https://quote.eastmoney.com/sh601658.html"
+    _desc = "东方财富-股票行情-日行情"
+
+    def __init__(self,
+                 symbols: str | list[str] = "000001",
+                 period: str = "daily",
+                 start_date: str = "19700101",
+                 end_date: str = "20500101",
+                 adjust: str = "",
+                 *args, **kwargs
+                 ):
+        self.symbols = symbols
+        self.period = period
+        self.start_date = start_date
+        self.end_date = end_date
+        self.adjust = adjust
+        self.extra_args = args
+        self.extra_kwargs = kwargs
+
+    def _fetch_data(self, *args, **kwargs):
+        code_id_dict = _code_id_map_em()
+        adjust_dict = {"qfq": "1", "hfq": "2", "": "0"}
+        period_dict = {"daily": "101", "weekly": "102", "monthly": "103"}
+        url = "http://push2his.eastmoney.com/api/qt/stock/kline/get"
+        big_df = pd.DataFrame()
+        if type(self.symbols) == str:
+            self.symbols = [self.symbols]
+        for symbol in self.symbols:
+            params = {
+                "fields1": "f1,f2,f3,f4,f5,f6",
+                "fields2": "f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61,f116",
+                "ut": "7eea3edcaed734bea9cbfc24409ed989",
+                "klt": period_dict[self.period],
+                "fqt": adjust_dict[self.adjust],
+                "secid": f"{code_id_dict[symbol]}.{symbol}",
+                "beg": self.start_date,
+                "end": self.end_date,
+                "_": "1623766962675",
+            }
+            timeout = self.extra_kwargs.get("timeout", None)
+            proxies = self.extra_kwargs.get("proxies", None)
+            r = httpx.get(url, params=params, timeout=timeout, proxies=proxies)
+            data_json = r.json()
+            if not (data_json["data"] and data_json["data"]["klines"]):
+                return pd.DataFrame()
+            temp_df = pd.DataFrame(
+                [item.split(",") for item in data_json["data"]["klines"]]
+            )
+            temp_df['symbol'] = symbol
+            big_df = pd.concat([big_df, temp_df], ignore_index=True)
+        return big_df
+
+    def _process_data(self, *args, **kwargs):
+        fetched_data = self._fetch_data()
+        fetched_data.columns = [
+            'date', 'open', 'close', 'high', 'low', 'volume',
+            'turnover', 'amplitude', 'price_change_rate', 'price_change', 'turnover_rate', 'symbol'
+        ]
+        fetched_data.index = pd.to_datetime(fetched_data["date"])
+        fetched_data.reset_index(inplace=True, drop=True)
+        fetched_data = fetched_data[[
+            'date', 'symbol', 'open', 'close', 'high', 'low', 'volume',
+            'turnover', 'amplitude', 'price_change_rate', 'price_change', 'turnover_rate'
+        ]]
+        for _column in fetched_data.columns[2:]:
+            fetched_data[_column] = pd.to_numeric(fetched_data[_column], errors="coerce")
+        return fetched_data
+
+    @property
+    def data(self) -> pd.DataFrame:
+        """
+        返回数据
+        :return: pandas.DataFrame
+        """
+        return self._process_data(self)
+
+    @property
+    def columns(self) -> list:
+        """
+        返回数据
+        :return: pandas.DataFrame
+        """
+        return self._columns
+
+    @property
+    def url(self) -> str:
+        return self._url
+
+    @property
+    def desc(self) -> str:
+        return self._desc
 
-    temp_df["开盘"] = pd.to_numeric(temp_df["开盘"])
-    temp_df["收盘"] = pd.to_numeric(temp_df["收盘"])
-    temp_df["最高"] = pd.to_numeric(temp_df["最高"])
-    temp_df["最低"] = pd.to_numeric(temp_df["最低"])
-    temp_df["成交量"] = pd.to_numeric(temp_df["成交量"])
-    temp_df["成交额"] = pd.to_numeric(temp_df["成交额"])
-    temp_df["振幅"] = pd.to_numeric(temp_df["振幅"])
-    temp_df["涨跌幅"] = pd.to_numeric(temp_df["涨跌幅"])
-    temp_df["涨跌额"] = pd.to_numeric(temp_df["涨跌额"])
-    temp_df["换手率"] = pd.to_numeric(temp_df["换手率"])
+    def __str__(self):
+        return "通过调用 .data() 方法返回数据；通过调用 .columns 属性返回数据的列名"
 
-    return temp_df
+    def __call__(self, *args, **kwargs):
+        self._process_data(self)
 
 
 if __name__ == '__main__':
-    stock_zh_a_hist_df = stock_zh_a_hist(symbol="430090",
-                                         period="daily",
-                                         start_date="20220516",
-                                         end_date="20220722",
-                                         adjust="hfq", )
-    print(stock_zh_a_hist_df)
+    stock_zh_a_hist = StockZhAHist
+    proxies = {
+        "http://": "http://127.0.0.1:7890",
+        "https://": "http://127.0.0.1:7890",
+    }
+    stock_zh_a_hist_obj = stock_zh_a_hist(
+        symbols=["430090", "000001", "000002", "600000", "600001"],
+        period="daily",
+        start_date="20000516",
+        end_date="20220722",
+        adjust="hfq",
+        timeout=2.111,
+        proxies=proxies
+    )
+    print(stock_zh_a_hist_obj.data)
+    print(stock_zh_a_hist_obj.columns)
+    print(stock_zh_a_hist_obj.url)
+    print(stock_zh_a_hist_obj.desc)
+    print(stock_zh_a_hist_obj.symbols)
+    print(stock_zh_a_hist_obj.start_date)
+    print(stock_zh_a_hist_obj.end_date)
+    print(stock_zh_a_hist_obj.adjust)
```

### Comparing `aklite-0.0.1/LICENSE` & `aklite-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aklite-0.0.1/pyproject.toml` & `aklite-0.0.2/pyproject.toml`

 * *Files identical despite different names*

