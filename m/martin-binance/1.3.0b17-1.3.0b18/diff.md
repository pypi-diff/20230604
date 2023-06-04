# Comparing `tmp/martin-binance-1.3.0b17.tar.gz` & `tmp/martin-binance-1.3.0b18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin-binance-1.3.0b17.tar", last modified: Sat Jun  3 20:54:02 2023, max compression
+gzip compressed data, was "martin-binance-1.3.0b18.tar", last modified: Sun Jun  4 09:35:44 2023, max compression
```

## Comparing `martin-binance-1.3.0b17.tar` & `martin-binance-1.3.0b18.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.0b17/.deepsource.toml
--rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.0b17/.dockerignore
--rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.0b17/.github/FUNDING.yml
--rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.0b17/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.0b17/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.0b17/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.0b17/.gitignore
--rwxr-xr-x   0        0        0    17427 2023-06-02 08:47:45.427876 martin-binance-1.3.0b17/CHANGELOG.md
--rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.0b17/Dockerfile
--rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.0b17/LICENSE
--rwxr-xr-x   0        0        0    35437 2023-05-30 12:20:07.843798 martin-binance-1.3.0b17/README.md
--rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.0b17/doc/Create_strategy.png
--rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.0b17/doc/Model of logarithmic grid.ods
--rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.0b17/doc/Modified martingale.svg
--rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.0b17/doc/graf1.png
--rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.0b17/doc/tlg_notify.png
--rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.0b17/doc/tmux.png
--rw-r--r--   0        0        0     1941 2023-06-03 20:53:44.158162 martin-binance-1.3.0b17/martin_binance/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-03 20:42:37.621820 martin-binance-1.3.0b17/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2949 2023-06-03 09:17:19.879857 martin-binance-1.3.0b17/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-06-01 20:26:31.871396 martin-binance-1.3.0b17/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    12120 2023-06-02 12:08:24.729428 martin-binance-1.3.0b17/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6474 2023-06-01 20:26:31.871396 martin-binance-1.3.0b17/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6469 2023-06-01 20:26:31.871396 martin-binance-1.3.0b17/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6475 2023-06-01 20:26:31.871396 martin-binance-1.3.0b17/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4710 2023-06-01 20:26:31.871396 martin-binance-1.3.0b17/martin_binance/client.py
--rw-r--r--   0        0        0   181429 2023-06-03 20:37:07.747079 martin-binance-1.3.0b17/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.0b17/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.0b17/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.0b17/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.0b17/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    77874 2023-06-03 18:24:38.067992 martin-binance-1.3.0b17/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.0b17/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.0b17/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.0b17/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16185 2023-05-30 12:20:07.847793 martin-binance-1.3.0b17/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-05-30 12:20:07.847793 martin-binance-1.3.0b17/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.3.0b17/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.0b17/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.0b17/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1203 2023-06-03 20:53:44.166165 martin-binance-1.3.0b17/pyproject.toml
--rw-r--r--   0        0        0      320 2023-06-03 20:53:44.162164 martin-binance-1.3.0b17/requirements.txt
--rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.0b17/uml/architecture.puml
--rw-r--r--   0        0        0    36614 1970-01-01 00:00:00.000000 martin-binance-1.3.0b17/PKG-INFO
+-rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.0b18/.deepsource.toml
+-rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.0b18/.dockerignore
+-rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.0b18/.github/FUNDING.yml
+-rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.0b18/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.0b18/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.0b18/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.0b18/.gitignore
+-rwxr-xr-x   0        0        0    17466 2023-06-04 09:16:25.405483 martin-binance-1.3.0b18/CHANGELOG.md
+-rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.0b18/Dockerfile
+-rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.0b18/LICENSE
+-rwxr-xr-x   0        0        0    35437 2023-05-30 12:20:07.843798 martin-binance-1.3.0b18/README.md
+-rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.0b18/doc/Create_strategy.png
+-rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.0b18/doc/Model of logarithmic grid.ods
+-rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.0b18/doc/Modified martingale.svg
+-rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.0b18/doc/graf1.png
+-rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.0b18/doc/tlg_notify.png
+-rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.0b18/doc/tmux.png
+-rw-r--r--   0        0        0     1941 2023-06-04 09:02:30.443389 martin-binance-1.3.0b18/martin_binance/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-03 20:42:37.621820 martin-binance-1.3.0b18/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2949 2023-06-03 09:17:19.879857 martin-binance-1.3.0b18/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-06-01 20:26:31.871396 martin-binance-1.3.0b18/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    12120 2023-06-02 12:08:24.729428 martin-binance-1.3.0b18/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6474 2023-06-01 20:26:31.871396 martin-binance-1.3.0b18/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6469 2023-06-01 20:26:31.871396 martin-binance-1.3.0b18/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6475 2023-06-01 20:26:31.871396 martin-binance-1.3.0b18/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4710 2023-06-01 20:26:31.871396 martin-binance-1.3.0b18/martin_binance/client.py
+-rw-r--r--   0        0        0   181446 2023-06-04 09:02:30.439389 martin-binance-1.3.0b18/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.0b18/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.0b18/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.0b18/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.0b18/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    77874 2023-06-03 18:24:38.067992 martin-binance-1.3.0b18/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.0b18/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.0b18/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.0b18/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16185 2023-05-30 12:20:07.847793 martin-binance-1.3.0b18/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-05-30 12:20:07.847793 martin-binance-1.3.0b18/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.3.0b18/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.0b18/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.0b18/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1203 2023-06-03 20:53:44.166165 martin-binance-1.3.0b18/pyproject.toml
+-rw-r--r--   0        0        0      320 2023-06-03 20:53:44.162164 martin-binance-1.3.0b18/requirements.txt
+-rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.0b18/uml/architecture.puml
+-rw-r--r--   0        0        0    36614 1970-01-01 00:00:00.000000 martin-binance-1.3.0b18/PKG-INFO
```

### Comparing `martin-binance-1.3.0b17/.github/ISSUE_TEMPLATE/bug_report.md` & `martin-binance-1.3.0b18/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/.github/ISSUE_TEMPLATE/feature_request.md` & `martin-binance-1.3.0b18/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/.github/workflows/codeql.yml` & `martin-binance-1.3.0b18/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/CHANGELOG.md` & `martin-binance-1.3.0b18/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## v1.3.0b18 2023-06-04
+### Fix
+* #59
+
 ## v1.3.0b12 2023-06-02
 ### Fix
 * deepsource issues
 
 ## v1.3.0b11 2023-06-01
 ### Fix
 * Bitfinex: rename test pair from AAABBB to TESTBTCTESTUSDT, update template
```

### Comparing `martin-binance-1.3.0b17/Dockerfile` & `martin-binance-1.3.0b18/Dockerfile`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/LICENSE` & `martin-binance-1.3.0b18/LICENSE`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/README.md` & `martin-binance-1.3.0b18/README.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/doc/Create_strategy.png` & `martin-binance-1.3.0b18/doc/Create_strategy.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/doc/Model of logarithmic grid.ods` & `martin-binance-1.3.0b18/doc/Model of logarithmic grid.ods`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/doc/Modified martingale.svg` & `martin-binance-1.3.0b18/doc/Modified martingale.svg`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/doc/graf1.png` & `martin-binance-1.3.0b18/doc/graf1.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/doc/tlg_notify.png` & `martin-binance-1.3.0b18/doc/tlg_notify.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/doc/tmux.png` & `martin-binance-1.3.0b18/doc/tmux.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/__init__.py` & `martin-binance-1.3.0b18/martin_binance/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b17"
+__version__ = "1.3.0b18"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 #
 import platform
```

### Comparing `martin-binance-1.3.0b17/martin_binance/backtest/OoTSP.py` & `martin-binance-1.3.0b18/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/backtest/VCoSEL.py` & `martin-binance-1.3.0b18/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/backtest/exchange_simulator.py` & `martin-binance-1.3.0b18/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/cli_0_BTCUSDT.py.template` & `martin-binance-1.3.0b18/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/cli_1_BTCUSDT.py.template` & `martin-binance-1.3.0b18/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin-binance-1.3.0b18/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/client.py` & `martin-binance-1.3.0b18/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/executor.py` & `martin-binance-1.3.0b18/martin_binance/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b16"
+__version__ = "1.3.0b18"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 from decimal import Decimal, ROUND_FLOOR, ROUND_CEILING
@@ -1061,20 +1061,20 @@
             self.message_log("restore_strategy_state from saved state:", log_level=LogLevel.DEBUG)
             self.message_log("\n".join(f"{k}\t{v}" for k, v in strategy_state.items()), log_level=LogLevel.DEBUG)
             #
             self.command = json.loads(strategy_state.get('command'))
             self.cycle_buy = json.loads(strategy_state.get('cycle_buy'))
             self.cycle_buy_count = json.loads(strategy_state.get('cycle_buy_count'))
             self.cycle_sell_count = json.loads(strategy_state.get('cycle_sell_count'))
-            self.cycle_time = datetime.strptime(json.loads(strategy_state.get('cycle_time')), '%Y-%m-%d %H:%M:%S.%f')
+            self.cycle_time = json.loads(strategy_state.get('cycle_time'))
+            if self.cycle_time:
+                self.cycle_time = datetime.strptime(self.cycle_time, '%Y-%m-%d %H:%M:%S.%f')
             self.cycle_time_reverse = json.loads(strategy_state.get('cycle_time_reverse'))
             if self.cycle_time_reverse:
                 self.cycle_time_reverse = datetime.strptime(self.cycle_time_reverse, '%Y-%m-%d %H:%M:%S.%f')
-            else:
-                self.cycle_time_reverse = None
             self.deposit_first = f2d(json.loads(strategy_state.get('deposit_first')))
             self.deposit_second = f2d(json.loads(strategy_state.get('deposit_second')))
             self.last_shift_time = json.loads(strategy_state.get('last_shift_time')) or self.local_time()
             self.martin = f2d(json.loads(strategy_state.get('martin')))
             self.order_q = json.loads(strategy_state.get('order_q'))
             self.orders_grid.restore(json.loads(strategy_state.get('orders')))
             self.orders_hold.restore(json.loads(strategy_state.get('orders_hold')))
```

### Comparing `martin-binance-1.3.0b17/martin_binance/funds_rate.db.template` & `martin-binance-1.3.0b18/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin-binance-1.3.0b18/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/margin_wrapper.py` & `martin-binance-1.3.0b18/martin_binance/margin_wrapper.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/ms_cfg.toml.template` & `martin-binance-1.3.0b18/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/service/funds_rate_exporter.py` & `martin-binance-1.3.0b18/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/service/grafana.json` & `martin-binance-1.3.0b18/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/martin_binance/service/relaunch.py` & `martin-binance-1.3.0b18/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/pyproject.toml` & `martin-binance-1.3.0b18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/uml/architecture.puml` & `martin-binance-1.3.0b18/uml/architecture.puml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b17/PKG-INFO` & `martin-binance-1.3.0b18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.0b17
+Version: 1.3.0b18
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.0b17 Summary: Free
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.0b18 Summary: Free
 trading system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: exchanges-wrapper==1.3.0.post1 Requires-Dist: margin-strategy-sdk==0.0.11
```

