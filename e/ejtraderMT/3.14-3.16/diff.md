# Comparing `tmp/ejtraderMT-3.14.tar.gz` & `tmp/ejtraderMT-3.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejtraderMT-3.14.tar", last modified: Sat May 20 18:00:26 2023, max compression
+gzip compressed data, was "ejtraderMT-3.16.tar", last modified: Sun Jun  4 21:17:29 2023, max compression
```

## Comparing `ejtraderMT-3.14.tar` & `ejtraderMT-3.16.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:00:26.631152 ejtraderMT-3.14/
--rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-05-20 18:00:05.000000 ejtraderMT-3.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 18:00:05.000000 ejtraderMT-3.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-20 18:00:26.631152 ejtraderMT-3.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-05-20 18:00:05.000000 ejtraderMT-3.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:00:26.627152 ejtraderMT-3.14/ejtraderMT/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 18:00:05.000000 ejtraderMT-3.14/ejtraderMT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:00:26.631152 ejtraderMT-3.14/ejtraderMT/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:00:05.000000 ejtraderMT-3.14/ejtraderMT/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29827 2023-05-20 18:00:05.000000 ejtraderMT-3.14/ejtraderMT/api/mql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:00:26.631152 ejtraderMT-3.14/ejtraderMT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-20 18:00:26.000000 ejtraderMT-3.14/ejtraderMT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-20 18:00:26.000000 ejtraderMT-3.14/ejtraderMT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:00:26.000000 ejtraderMT-3.14/ejtraderMT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-20 18:00:26.000000 ejtraderMT-3.14/ejtraderMT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 18:00:26.000000 ejtraderMT-3.14/ejtraderMT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-20 18:00:05.000000 ejtraderMT-3.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-20 18:00:26.631152 ejtraderMT-3.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-20 18:00:05.000000 ejtraderMT-3.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:17:29.924077 ejtraderMT-3.16/
+-rw-r--r--   0 runner    (1001) docker     (123)    35128 2023-06-04 21:17:03.000000 ejtraderMT-3.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-04 21:17:03.000000 ejtraderMT-3.16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-06-04 21:17:29.924077 ejtraderMT-3.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-06-04 21:17:03.000000 ejtraderMT-3.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:17:29.924077 ejtraderMT-3.16/ejtraderMT/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-04 21:17:03.000000 ejtraderMT-3.16/ejtraderMT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:17:29.924077 ejtraderMT-3.16/ejtraderMT/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:17:03.000000 ejtraderMT-3.16/ejtraderMT/api/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28094 2023-06-04 21:17:03.000000 ejtraderMT-3.16/ejtraderMT/api/mql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:17:29.924077 ejtraderMT-3.16/ejtraderMT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-06-04 21:17:29.000000 ejtraderMT-3.16/ejtraderMT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-04 21:17:29.000000 ejtraderMT-3.16/ejtraderMT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:17:29.000000 ejtraderMT-3.16/ejtraderMT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-04 21:17:29.000000 ejtraderMT-3.16/ejtraderMT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 21:17:29.000000 ejtraderMT-3.16/ejtraderMT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-04 21:17:03.000000 ejtraderMT-3.16/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 21:17:29.924077 ejtraderMT-3.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-04 21:17:03.000000 ejtraderMT-3.16/setup.py
```

### Comparing `ejtraderMT-3.14/LICENSE` & `ejtraderMT-3.16/LICENSE`

 * *Files identical despite different names*

### Comparing `ejtraderMT-3.14/PKG-INFO` & `ejtraderMT-3.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderMT
-Version: 3.14
+Version: 3.16
 Summary: Metatrader API
 Home-page: https://ejtraderMT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderMT/issues
```

### Comparing `ejtraderMT-3.14/README.md` & `ejtraderMT-3.16/README.md`

 * *Files identical despite different names*

### Comparing `ejtraderMT-3.14/ejtraderMT/api/mql.py` & `ejtraderMT-3.16/ejtraderMT/api/mql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,153 +1,82 @@
-from datetime import datetime, timedelta, date
+from datetime import datetime, timedelta
 from pytz import timezone
 from tzlocal import get_localzone
 from queue import Queue
 from threading import Thread
 import os
 import time
 import zmq
 
 import pandas as pd
-from ejtraderTH import start, stop
+from ejtraderTH import start
 from ejtraderDB import DictSQLite
 from influxdb import DataFrameClient
 from tqdm import tqdm
 import logging
 import sys
 import warnings
 
 # Configuração do logger
 LOGGER = {
     "datefmt": "%Y-%m-%d %H:%M:%S",
-    "format": f"[%(asctime)s.%(msecs)03d]"
-    f"[%(process)s]"
-    f"[%(funcName)s:%(lineno)d]"
-    f"[%(levelname)s]"
-    f": %(message)s",
+    "format": (
+        "[%(asctime)s.%(msecs)03d]"
+        "[%(process)s]"
+        "[%(funcName)s:%(lineno)d]"
+        "[%(levelname)s]"
+        ": %(message)s"
+    ),
     "level": logging.INFO,
     "stream": sys.stdout,
 }
 
 
 class Functions:
     def __init__(self, host=None, debug=None):
         self.HOST = host or "localhost"
         self.SYS_PORT = 15555  # REP/REQ port
-        self.DATA_PORT = 15556  # PUSH/PULL port
-        self.LIVE_PORT = 15557  # PUSH/PULL port
-        self.EVENTS_PORT = 15558  # PUSH/PULL port
-        self.INDICATOR_DATA_PORT = 15559  # REP/REQ port
-        self.CHART_DATA_PORT = 15560  # PUSH
-        self.debug = debug or True
 
         # ZeroMQ timeout in seconds
-        sys_timeout = 100
-        data_timeout = 1000
+        sys_timeout = 1000
 
         # initialise ZMQ context
         context = zmq.Context()
 
         # connect to server sockets
         try:
             self.sys_socket = context.socket(zmq.REQ)
             # set port timeout
-            self.sys_socket.RCVTIMEO = sys_timeout * 1000
+            self.sys_socket.RCVTIMEO = sys_timeout
             self.sys_socket.connect("tcp://{}:{}".format(self.HOST, self.SYS_PORT))
 
-            self.data_socket = context.socket(zmq.PULL)
-            # set port timeout
-            self.data_socket.RCVTIMEO = data_timeout * 1000
-            self.data_socket.connect("tcp://{}:{}".format(self.HOST, self.DATA_PORT))
-
-            self.indicator_data_socket = context.socket(zmq.PULL)
-            # set port timeout
-            self.indicator_data_socket.RCVTIMEO = data_timeout * 1000
-            self.indicator_data_socket.connect(
-                "tcp://{}:{}".format(self.HOST, self.INDICATOR_DATA_PORT)
-            )
-            self.chart_data_socket = context.socket(zmq.PUSH)
-            # set port timeout
-            # TODO check if port is listening and error handling
-            self.chart_data_socket.connect(
-                "tcp://{}:{}".format(self.HOST, self.CHART_DATA_PORT)
-            )
-
         except zmq.ZMQError:
             raise zmq.ZMQBindError("Binding ports ERROR")
         except KeyboardInterrupt:
             self.sys_socket.close()
             self.sys_socket.term()
-            self.data_socket.close()
-            self.data_socket.term()
-            self.indicator_data_socket.close()
-            self.indicator_data_socket.term()
-            self.chart_data_socket.close()
-            self.chart_data_socket.term()
             pass
 
     def _send_request(self, data: dict) -> None:
         """Send request to server via ZeroMQ System socket"""
         try:
             self.sys_socket.send_json(data)
-            msg = self.sys_socket.recv_string()
-            # terminal received the request
-            assert msg == "OK", "Something wrong on server side"
         except AssertionError as err:
             raise zmq.NotDone(err)
         except zmq.ZMQError:
             raise zmq.NotDone("Sending request ERROR")
 
     def _pull_reply(self):
         """Get reply from server via Data socket with timeout"""
         try:
-            msg = self.data_socket.recv_json()
+            msg = self.sys_socket.recv_json()
         except zmq.ZMQError:
             raise zmq.NotDone("Data socket timeout ERROR")
         return msg
 
-    def _indicator_pull_reply(self):
-        """Get reply from server via Data socket with timeout"""
-        try:
-            msg = self.indicator_data_socket.recv_json()
-        except zmq.ZMQError:
-            raise zmq.NotDone("Indicator Data socket timeout ERROR")
-        if self.debug:
-            logging.info("ZMQ INDICATOR DATA REPLY: ", msg)
-        return msg
-
-    def live_socket(self, context=None):
-        """Connect to socket in a ZMQ context"""
-        try:
-            context = context or zmq.Context.instance()
-            socket = context.socket(zmq.PULL)
-            socket.connect("tcp://{}:{}".format(self.HOST, self.LIVE_PORT))
-        except zmq.ZMQError:
-            raise zmq.ZMQBindError("Live port connection ERROR")
-        return socket
-
-    def streaming_socket(self, context=None):
-        """Connect to socket in a ZMQ context"""
-        try:
-            context = context or zmq.Context.instance()
-            socket = context.socket(zmq.PULL)
-            socket.connect("tcp://{}:{}".format(self.HOST, self.EVENTS_PORT))
-        except zmq.ZMQError:
-            raise zmq.ZMQBindError("Data port connection ERROR")
-        return socket
-
-    def _push_chart_data(self, data: dict) -> None:
-        """Send message for chart control to server via ZeroMQ chart data socket"""
-        try:
-            if self.debug:
-                logging.info("ZMQ PUSH CHART DATA: ", data, " -> ", data)
-            self.chart_data_socket.send_json(data)
-        except zmq.ZMQError:
-            raise zmq.NotDone("Sending request ERROR")
-
     def Command(self, **kwargs) -> dict:
         """Construct a request dictionary from default and send it to server"""
 
         # default dictionary
         request = {
             "action": None,
             "actionType": None,
@@ -179,66 +108,14 @@
 
         # send dict to server
         self._send_request(request)
 
         # return server reply
         return self._pull_reply()
 
-    def indicator_construct_and_send(self, **kwargs) -> dict:
-        """Construct a request dictionary from default and send it to server"""
-
-        # default dictionary
-        request = {
-            "action": None,
-            "actionType": None,
-            "id": None,
-            "symbol": None,
-            "chartTF": None,
-            "fromDate": None,
-            "toDate": None,
-            "name": None,
-            "params": None,
-            "linecount": None,
-        }
-
-        # update dict values if exist
-        for key, value in kwargs.items():
-            if key in request:
-                request[key] = value
-            else:
-                raise KeyError("Unknown key in **kwargs ERROR")
-
-        # send dict to server
-        self._send_request(request)
-
-        # return server reply
-        return self._indicator_pull_reply()
-
-    def chart_data_construct_and_send(self, **kwargs) -> dict:
-        """Construct a request dictionary from default and send it to server"""
-
-        # default dictionary
-        message = {
-            "action": None,
-            "actionType": None,
-            "chartId": None,
-            "indicatorChartId": None,
-            "data": None,
-        }
-
-        # update dict values if exist
-        for key, value in kwargs.items():
-            if key in message:
-                message[key] = value
-            else:
-                raise KeyError("Unknown key in **kwargs ERROR")
-
-        # send dict to server
-        self._push_chart_data(message)
-
 
 class Metatrader:
     def __init__(
         self,
         host=None,
         real_volume=None,
         tz_local=None,
@@ -249,15 +126,15 @@
         dbuser=None,
         dbname=None,
         debug=False,
     ):
         if debug:
             logging.basicConfig(**LOGGER)
 
-        self.__api = Functions(host)
+        self.__api = Functions(host, debug=debug)
         self.real_volume = real_volume or False
         self.__tz_local = tz_local
         self.__utc_timezone = timezone("UTC")
         self.__my_timezone = get_localzone()
         self.__utc_brocker_offset = self.___utc_brocker_offset()
         # db settings
         self.dbtype = dbtype or "SQLITE"  # SQLITE OR INFLUXDB
@@ -276,24 +153,50 @@
                 self.dbhost, self.dbport, self.dbuser, self.dbpass, self.dbname
             )
             self.__client.create_database(self.dbname)
 
     def balance(self):
         return self.__api.Command(action="BALANCE")
 
+    def symbols(self):
+        df = None
+        try:
+            df = self.__api.Command(action="LISTSYMBOLS")
+
+        except Exception as e:
+            logging.info(f"Error while processing. Error message: {str(e)}")
+
+        if df is not None and isinstance(df, dict):
+            try:
+                if df["data"]:
+                    df = pd.DataFrame(df["data"])
+                    df.columns = [
+                        "symbol",
+                        "expiration",
+                        "type",
+                    ]
+            except Exception as e:
+                logging.info(
+                    f"Error while processing Dataframe. Error message: {str(e)}"
+                )
+                pass
+        df = df.drop_duplicates(subset="symbol", keep="first")
+
+        return df
+
     def calendar(self, symbol=None, fromDate=None, toDate=None, database=None):
         self._symbol = symbol
         self._fromDate = fromDate
         self._toDate = toDate
         self.__calendarQ = Queue()
         self.__database = database
         try:
             start(self._calendar, repeat=1, max_threads=20)
-        except:
-            logging.info("Error: unable to start History thread")
+        except Exception as e:
+            logging.info(f"Error: {e}")
 
         return self.__calendarQ.get()
 
     def _calendar(self, data):
         symbol = self._symbol
         fromDate = self._fromDate
         toDate = self._toDate
@@ -317,38 +220,28 @@
         while start_date <= end_date:
             pbar.update(delta.days)
             fromDate = start_date.strftime("%d/%m/%Y")
             toDate = start_date
             toDate += delta2
             toDate = toDate.strftime("%d/%m/%Y")
 
-            if fromDate and toDate:
-                try:
-                    df = self.__api.Command(
-                        action="CALENDAR",
-                        actionType="DATA",
-                        symbol=symbol,
-                        fromDate=self.__date_to_timestamp(fromDate),
-                        toDate=self.__date_to_timestamp(toDate),
-                    )
+            try:
+                df = self.__api.Command(
+                    action="CALENDAR",
+                    actionType="DATA",
+                    symbol=symbol,
+                    fromDate=self.__date_to_timestamp(fromDate),
+                    toDate=self.__date_to_timestamp(toDate),
+                )
+            except Exception as e:
+                logging.info(
+                    f"Error while processing {symbol}. Error message: {str(e)}"
+                )
+                pass
 
-                except:
-                    pass
-            elif isinstance(fromDate, str) and toDate == None:
-                try:
-                    df = self.__api.Command(
-                        action="CALENDAR",
-                        actionType="DATA",
-                        symbol=symbol,
-                        fromDate=self.__date_to_timestamp(fromDate),
-                        toDate=self.__date_to_timestamp(toDate),
-                    )
-                except:
-                    pass
-            self.__api.Command(action="RESET")
             try:
                 df = pd.DataFrame(df["data"])
                 df.columns = [
                     "date",
                     "currency",
                     "impact",
                     "event",
@@ -357,25 +250,25 @@
                     "forecast",
                     "previous",
                 ]
                 df["date"] = pd.to_datetime(df["date"], errors="coerce")
                 df = df.dropna(subset=["date"])
                 df = df.set_index("date")
                 df.index = pd.to_datetime(df.index)
-            except:
+            except Exception as e:
+                logging.info(
+                    f"Error while processing {symbol} Dataframe. Error message: {str(e)}"
+                )
                 pass
+
             appended_data.append(df)
             start_date += delta
         pbar.close()
-        # Your code goes here
-        if len(appended_data) > 0:
-            df = pd.concat(appended_data)
-        else:
-            logging.error("No received data, check date")
-            stop()
+
+        df = pd.concat(appended_data)
 
         if self.__database:
             start(self.__save_to_db, data=[df], repeat=1, max_threads=20)
         else:
             try:
                 self.__set_utc_or_localtime_tz_df(df)
                 self.__calendarQ.put(df)
@@ -570,25 +463,23 @@
                 event = event["request"]
                 event = pd.DataFrame(event, index=[0])
                 self.__eventQ.put(event)
             except KeyError:
                 pass
 
     def price(self, symbol, chartTF):
-        self.__api.Command(action="RESET")
         self._allsymbol_ = symbol
         self._allchartTF = chartTF
         for active in symbol:
             self.__api.Command(action="CONFIG", symbol=active, chartTF=chartTF)
         self._start_thread_price()
         time.sleep(0.5)
         return self.__priceQ.get()
 
     def event(self, symbol, chartTF):
-        self.__api.Command(action="RESET")
         self._allsymbol_ = symbol
         self._allchartTF = chartTF
         for active in symbol:
             self.__api.Command(action="CONFIG", symbol=active, chartTF=chartTF)
 
         self._start_thread_event()
         time.sleep(0.5)
@@ -631,18 +522,21 @@
             "D1": 86400,
             "W1": 604800,
             "MN": 2629746,
         }
         return TIMECANDLE[timeframe]
 
     def __set_utc_or_localtime_tz_df(self, df):
-        df.index = df.index.tz_localize(self.__utc_brocker_offset)
-        if self.__tz_local:
-            df.index = df.index.tz_convert(self.__my_timezone)
-        df.index = df.index.tz_localize(None)
+        try:
+            df.index = df.index.tz_localize(self.__utc_brocker_offset)
+            if self.__tz_local:
+                df.index = df.index.tz_convert(self.__my_timezone)
+            df.index = df.index.tz_localize(None)
+        except:
+            pass
         return df
 
     def history(
         self,
         symbol,
         chartTF=None,
         fromDate=None,
@@ -654,74 +548,78 @@
         self.__database = database
         self.fromDate = fromDate
         self.toDate = toDate
         self.__historyQ = Queue()
         self.dataframe = dataframe
         if isinstance(symbol, tuple):
             for symbols in symbol:
-                self._symbol = symbols
-                logging.info(symbols)
+                self.__symbol = symbols
+                print(symbols)
         elif isinstance(symbol, list):
-            self._symbol = symbol
+            self.__symbol = symbol
         else:
-            self._symbol = symbol
+            self.__symbol = [symbol]
 
         if chartTF:
             if self.__database:
                 try:
                     start(self.__historyThread_save, repeat=1, max_threads=20)
-                except:
-                    logging.info("Error: unable to start History thread")
+                except Exception as e:
+                    logging.info(
+                        f"Error: unable to start History thread Error message: {str(e)}"
+                    )
             else:
                 try:
                     start(self.__historyThread_save, repeat=1, max_threads=20)
-                except:
-                    logging.info("Error: unable to start History thread")
+                except Exception as e:
+                    logging.info(
+                        f"Error: unable to start History thread Error message: {str(e)}"
+                    )
+
                 return self.__historyQ.get()
         else:
             q = DictSQLite("history")
             if isinstance(symbol, list):
                 try:
                     if self.dbtype == "SQLITE":
-                        df = q[f"{self._symbol[0]}"]
+                        df = q[f"{self.__symbol[0]}"]
                     else:
-                        df = self.__client.query(f"select * from {self._symbol[0]}")
-                        df = df[self._symbol[0]]
+                        df = self.__client.query(f"select * from {self.__symbol[0]}")
+                        df = df[self.__symbol[0]]
 
                         df.index.name = "date"
                 except KeyError:
-                    df = f" {self._symbol[0]}  isn't on database"
+                    df = f" {self.__symbol[0]}  isn't on database"
                     pass
             else:
                 try:
                     if self.dbtype == "SQLITE":
-                        df = q[f"{self._symbol}"]
+                        df = q[f"{self.__symbol}"]
                     else:
-                        df = self.__client.query(f"select * from {self._symbol}")
-                        df = df[self._symbol]
+                        df = self.__client.query(f"select * from {self.__symbol}")
+                        df = df[self.__symbol]
 
                         df.index.name = "date"
                 except KeyError:
-                    df = f" {self._symbol}  isn't on database"
+                    df = f" {self.__symbol}  isn't on database"
                     pass
             return df
 
     def __historyThread_save(self, data):
-        actives = self._symbol
+        actives = self.__symbol
         chartTF = self.chartTF
         fromDate = self.fromDate
         toDate = self.toDate
         main = pd.DataFrame()
         current = pd.DataFrame()
         self._count = 0
-        if self.__database:
-            try:
-                os.makedirs("DataBase")
-            except OSError:
-                pass
+        try:
+            os.makedirs("DataBase")
+        except OSError:
+            pass
         # count data
         if not isinstance(fromDate, int):
             start_date = datetime.strptime(fromDate, "%d/%m/%Y")
         else:
             start_date = self.__brokerTimeDelta(fromDate)
         if not toDate:
             end_date = self.__brokerTimeDelta(0)
@@ -730,155 +628,195 @@
 
         delta = timedelta(days=1)
         delta2 = timedelta(days=1)
         diff_days = start_date - end_date
         days_count = diff_days.days
         pbar = tqdm(total=abs(days_count))
         appended_data = []
+        active = None
+        df = None
         while start_date <= end_date:
             pbar.update(delta.days)
             fromDate = start_date.strftime("%d/%m/%Y")
             toDate = start_date
             toDate += delta2
             toDate = toDate.strftime("%d/%m/%Y")
-            active = None
+            attempts = 0
+            success = False
+
             # if chartTF == "TICK":
             #     chartConvert = 60
             # else:
             #     chartConvert = self.__timeframe_to_sec(chartTF)
-            if isinstance(actives, list):
-                for active in actives:
-                    self._count += 1
-            else:
-                active = actives
+            for active in actives:
+                self._count += 1
 
                 # the first symbol on list is the main and the rest will merge
                 if active == actives[0]:
                     self.__active_name = active
-                    # get data
-                    if fromDate and toDate:
-                        data = self.__api.Command(
-                            action="HISTORY",
-                            actionType="DATA",
-                            symbol=active,
-                            chartTF=chartTF,
-                            fromDate=self.__date_to_timestamp(fromDate),
-                            toDate=self.__date_to_timestamp(toDate),
-                        )
-
-                    elif isinstance(fromDate, str) and toDate == None:
-                        data = self.__api.Command(
-                            action="HISTORY",
-                            actionType="DATA",
-                            symbol=active,
-                            chartTF=chartTF,
-                            fromDate=self.__date_to_timestamp(fromDate),
-                            toDate=self.__date_to_timestamp(toDate),
-                        )
-
-                    self.__api.Command(action="RESET")
-                    try:
-                        main = pd.DataFrame(data["data"])
-                        main = main.set_index([0])
-                        main.index.name = "date"
-
-                        # TICK DATA
-                        if chartTF == "TICK":
-                            main.columns = ["bid", "ask"]
-                            main.index = pd.to_datetime(main.index, unit="ms")
-                        else:
-                            main.index = pd.to_datetime(main.index, unit="s")
-                            if self.real_volume:
-                                del main[5]
-                            else:
-                                del main[6]
-                            main.columns = [
-                                "open",
-                                "high",
-                                "low",
-                                "close",
-                                "volume",
-                                "spread",
-                            ]
-                    except KeyError:
+                    while not success and attempts < 5:
+                        try:
+                            data = self.__api.Command(
+                                action="HISTORY",
+                                actionType="DATA",
+                                symbol=active,
+                                chartTF=chartTF,
+                                fromDate=self.__date_to_timestamp(fromDate),
+                                toDate=self.__date_to_timestamp(toDate),
+                            )
+                            success = True
+                        except Exception as e:
+                            logging.info(
+                                f"Error while processing {active} from {fromDate}. Error message: {str(e)}"
+                            )
+                            attempts += 1
+                    if attempts == 5 and not success:
+                        logging.info(f"Check if {active} is avalible from {fromDate}")
                         pass
-                else:
-                    data = self.__api.Command(
-                        action="HISTORY",
-                        actionType="DATA",
-                        symbol=active,
-                        chartTF=chartTF,
-                        fromDate=self.__date_to_timestamp(fromDate),
-                        toDate=self.__date_to_timestamp(toDate),
-                    )
 
-                    self.__api.Command(action="RESET")
-                    try:
-                        current = pd.DataFrame(data["data"])
-                        current = current.set_index([0])
-                        current.index.name = "date"
-                        active = active.lower()
-                        # TICK DATA
-                        if chartTF == "TICK":
-                            current.index = pd.to_datetime(current.index, unit="ms")
-                            current.columns = [f"{active}_bid", f"{active}_ask"]
-                        else:
-                            current.index = pd.to_datetime(current.index, unit="s")
-                            if self.real_volume:
-                                del current[5]
-                            else:
-                                del current[6]
-
-                            current.columns = [
-                                f"{active}_open",
-                                f"{active}_high",
-                                f"{active}_low",
-                                f"{active}_close",
-                                f"{active}_volume",
-                                f"{active}_spread",
-                            ]
-
-                        # main = pd.merge(main, current, how='inner',
-                        #                 left_index=True, right_index=True)
-                        main = pd.merge(main, current, on="date")
-                    except KeyError:
+                    if data is not None and isinstance(data, dict):
+                        try:
+                            if data["data"]:
+                                main = pd.DataFrame(data["data"])
+                                main = main.set_index([0])
+                                main.index.name = "date"
+
+                                # TICK DATA
+                                if chartTF == "TICK":
+                                    main.columns = ["bid", "ask"]
+                                    main.index = pd.to_datetime(main.index, unit="ms")
+                                else:
+                                    main.index = pd.to_datetime(main.index, unit="s")
+                                    if self.real_volume:
+                                        del main[5]
+                                    else:
+                                        del main[6]
+                                    main.columns = [
+                                        "open",
+                                        "high",
+                                        "low",
+                                        "close",
+                                        "volume",
+                                        "spread",
+                                    ]
+                        except Exception as e:
+                            logging.info(
+                                f"Error while processing Dataframe {active} from {fromDate}. Error message: {str(e)}"
+                            )
+                            pass
+                else:
+                    while not success and attempts < 2:
+                        try:
+                            data = self.__api.Command(
+                                action="HISTORY",
+                                actionType="DATA",
+                                symbol=active,
+                                chartTF=chartTF,
+                                fromDate=self.__date_to_timestamp(fromDate),
+                                toDate=self.__date_to_timestamp(toDate),
+                            )
+                            success = True
+                        except Exception as e:
+                            logging.info(
+                                f"Error while processing {active}. Error message: {str(e)}"
+                            )
+                            attempts += 1
+                    if attempts == 2 and not success:
+                        logging.info(f"Check if {active} is avalible from {fromDate}")
                         pass
 
-            main = main.loc[~main.index.duplicated(keep="first")]
-            appended_data.append(main)
+                    if data is not None and isinstance(data, dict):
+                        try:
+                            if data["data"]:
+                                current = pd.DataFrame(data["data"])
+                                current = current.set_index([0])
+                                current.index.name = "date"
+                                active = active.lower()
+                                # TICK DATA
+                                if chartTF == "TICK":
+                                    current.index = pd.to_datetime(
+                                        current.index, unit="ms"
+                                    )
+                                    current.columns = [f"{active}_bid", f"{active}_ask"]
+                                else:
+                                    current.index = pd.to_datetime(
+                                        current.index, unit="s"
+                                    )
+                                    if self.real_volume:
+                                        del current[5]
+                                    else:
+                                        del current[6]
+
+                                    current.columns = [
+                                        f"{active}_open",
+                                        f"{active}_high",
+                                        f"{active}_low",
+                                        f"{active}_close",
+                                        f"{active}_volume",
+                                        f"{active}_spread",
+                                    ]
+
+                                # main = pd.merge(main, current, how='inner',
+                                #                 left_index=True, right_index=True)
+                                main = pd.merge(main, current, on="date")
+                        except Exception as e:
+                            logging.info(
+                                f"Error while merge Dataframe {active}. Error message: {str(e)}"
+                            )
+                            pass
 
+            try:
+                main = main.loc[~main.index.duplicated(keep="first")]
+                appended_data.append(main)
+            except Exception as e:
+                logging.info(
+                    f"Error while finishing Dataframe for {active}. Error message: {str(e)}"
+                )
+                pass
             start_date += delta
         pbar.close()
-        # Your code goes here
-        if len(appended_data) > 0:
-            df = pd.concat(appended_data)
-        else:
-            logging.error("No received data, check date")
-            stop()
 
-        if self.__database:
-            start(self.__save_to_db, data=[df], repeat=1, max_threads=20)
-        else:
+        if len(appended_data) > 0:
             try:
-                self.__set_utc_or_localtime_tz_df(df)
-                self.__historyQ.put(df)
-
-            except AttributeError:
+                df = pd.concat(appended_data)
+            except Exception as e:
+                logging.info(
+                    f"Error while processing {active}. Error message: {str(e)}"
+                )
                 pass
 
+            if self.__database:
+                start(self.__save_to_db, data=[df], repeat=1, max_threads=20)
+            else:
+                try:
+                    self.__set_utc_or_localtime_tz_df(df)
+                    self.__historyQ.put(df)
+
+                except Exception as e:
+                    logging.info(
+                        f"Error while processing {active}. Error message: {str(e)}"
+                    )
+                    pass
+
     def __save_to_db(self, df):
         if self.dbtype == "SQLITE":
             q = DictSQLite("history", multithreading=True)
             try:
                 self.__set_utc_or_localtime_tz_df(df)
 
-            except AttributeError:
+            except Exception as e:
+                logging.info(
+                    f"Error while processing database. Error message: {str(e)}"
+                )
                 pass
 
             q[f"{self._symbol}"] = df
         else:
             try:
                 self.__set_utc_or_localtime_tz_df(df)
-            except AttributeError:
+            except Exception as e:
+                logging.info(
+                    f"Error while processing utc or localtime tz. Error message: {str(e)}"
+                )
                 pass
         if self.dbtype == "INFLUXDB":
             self.__client.write_points(df, f"{self._symbol}", protocol=self.protocol)
```

### Comparing `ejtraderMT-3.14/ejtraderMT.egg-info/PKG-INFO` & `ejtraderMT-3.16/ejtraderMT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ejtraderMT
-Version: 3.14
+Version: 3.16
 Summary: Metatrader API
 Home-page: https://ejtraderMT.readthedocs.io/
 Download-URL: https://ejtrader.com
 Author: Emerson Pedroso
 Author-email: support@ejtrader.com
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/traderpedroso/ejtraderMT/issues
```

### Comparing `ejtraderMT-3.14/setup.py` & `ejtraderMT-3.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     reqs = list()
     with io.open(filename, encoding="utf-8") as f:
         for line in f.readlines():
             reqs.append(line.strip())
     return reqs
 
 
-# Version: 3.14
+# Version: 3.16
 setup(
     name="ejtraderMT",
-    version="3.14",
+    version="3.16",
     packages=find_packages(),
     url="https://ejtraderMT.readthedocs.io/",
     download_url="https://ejtrader.com",
     license="GPL-3.0",
     author="Emerson Pedroso",
     author_email="support@ejtrader.com",
     description="Metatrader API",
```

