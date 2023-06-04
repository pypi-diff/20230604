# Comparing `tmp/std.algorithm-1.1.3.tar.gz` & `tmp/std.algorithm-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std.algorithm-1.1.3.tar", last modified: Sun May 21 09:44:04 2023, max compression
+gzip compressed data, was "std.algorithm-1.1.4.tar", last modified: Sun Jun  4 15:21:33 2023, max compression
```

## Comparing `std.algorithm-1.1.3.tar` & `std.algorithm-1.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 09:44:04.008292 std.algorithm-1.1.3/
--rw-rw-rw-   0        0        0      324 2023-05-21 09:44:04.008292 std.algorithm-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       47 2022-10-07 01:09:45.000000 std.algorithm-1.1.3/README.md
--rw-rw-rw-   0        0        0      312 2023-05-21 09:44:04.012309 std.algorithm-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      478 2023-02-19 07:05:31.000000 std.algorithm-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:44:03.958368 std.algorithm-1.1.3/std/
--rw-rw-rw-   0        0        0    13868 2023-05-18 13:13:28.000000 std.algorithm-1.1.3/std/MySQL.py
--rw-rw-rw-   0        0        0    20406 2023-04-28 14:40:16.000000 std.algorithm-1.1.3/std/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-04-18 14:54:44.000000 std.algorithm-1.1.3/std/combinatorics.py
--rw-rw-rw-   0        0        0     2819 2023-05-14 09:54:42.000000 std.algorithm-1.1.3/std/data.py
--rw-rw-rw-   0        0        0      214 2022-10-12 06:19:30.000000 std.algorithm-1.1.3/std/error.py
--rw-rw-rw-   0        0        0     8504 2023-05-14 09:57:03.000000 std.algorithm-1.1.3/std/file.py
--rw-rw-rw-   0        0        0     1754 2023-03-04 02:50:47.000000 std.algorithm-1.1.3/std/http.py
--rw-rw-rw-   0        0        0    39598 2023-05-20 02:05:20.000000 std.algorithm-1.1.3/std/keras.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:44:04.006296 std.algorithm-1.1.3/std/lib/
--rw-rw-rw-   0        0        0  2220528 2022-10-22 04:21:48.000000 std.algorithm-1.1.3/std/lib/eigen.dll
--rw-rw-rw-   0        0        0    12858 2022-11-01 16:38:35.000000 std.algorithm-1.1.3/std/nlp.py
--rw-rw-rw-   0        0        0       89 2023-03-11 01:48:50.000000 std.algorithm-1.1.3/std/regexp.py
--rw-rw-rw-   0        0        0      770 2022-10-12 05:55:17.000000 std.algorithm-1.1.3/std/search.py
--rw-rw-rw-   0        0        0    19454 2023-03-11 01:48:50.000000 std.algorithm-1.1.3/std/sets.py
--rw-rw-rw-   0        0        0     1162 2022-10-07 01:27:48.000000 std.algorithm-1.1.3/std/tree.py
--rw-rw-rw-   0        0        0      443 2023-03-17 14:49:04.000000 std.algorithm-1.1.3/std/unicode.py
--rw-rw-rw-   0        0        0    35286 2023-02-05 04:04:59.000000 std.algorithm-1.1.3/std/xml.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:44:03.964354 std.algorithm-1.1.3/std.algorithm.egg-info/
--rw-rw-rw-   0        0        0      324 2023-05-21 09:44:03.000000 std.algorithm-1.1.3/std.algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-05-21 09:44:03.000000 std.algorithm-1.1.3/std.algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 09:44:03.000000 std.algorithm-1.1.3/std.algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-21 09:44:03.000000 std.algorithm-1.1.3/std.algorithm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-21 09:44:03.000000 std.algorithm-1.1.3/std.algorithm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 15:21:33.416764 std.algorithm-1.1.4/
+-rw-rw-rw-   0        0        0      324 2023-06-04 15:21:33.416764 std.algorithm-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2022-10-07 01:09:45.000000 std.algorithm-1.1.4/README.md
+-rw-rw-rw-   0        0        0      312 2023-06-04 15:21:33.417790 std.algorithm-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      478 2023-02-19 07:05:31.000000 std.algorithm-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 15:21:33.388840 std.algorithm-1.1.4/std/
+-rw-rw-rw-   0        0        0    14485 2023-06-03 18:41:19.000000 std.algorithm-1.1.4/std/MySQL.py
+-rw-rw-rw-   0        0        0    20805 2023-05-31 15:05:36.000000 std.algorithm-1.1.4/std/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-04-18 14:54:44.000000 std.algorithm-1.1.4/std/combinatorics.py
+-rw-rw-rw-   0        0        0     2819 2023-05-14 09:54:42.000000 std.algorithm-1.1.4/std/data.py
+-rw-rw-rw-   0        0        0      214 2022-10-12 06:19:30.000000 std.algorithm-1.1.4/std/error.py
+-rw-rw-rw-   0        0        0     8504 2023-05-14 09:57:03.000000 std.algorithm-1.1.4/std/file.py
+-rw-rw-rw-   0        0        0     1754 2023-03-04 02:50:47.000000 std.algorithm-1.1.4/std/http.py
+-rw-rw-rw-   0        0        0    39618 2023-05-24 14:34:06.000000 std.algorithm-1.1.4/std/keras.py
+drwxrwxrwx   0        0        0        0 2023-06-04 15:21:33.414798 std.algorithm-1.1.4/std/lib/
+-rw-rw-rw-   0        0        0  2220528 2022-10-22 04:21:48.000000 std.algorithm-1.1.4/std/lib/eigen.dll
+-rw-rw-rw-   0        0        0    12858 2022-11-01 16:38:35.000000 std.algorithm-1.1.4/std/nlp.py
+-rw-rw-rw-   0        0        0       89 2023-03-11 01:48:50.000000 std.algorithm-1.1.4/std/regexp.py
+-rw-rw-rw-   0        0        0      770 2022-10-12 05:55:17.000000 std.algorithm-1.1.4/std/search.py
+-rw-rw-rw-   0        0        0    19454 2023-03-11 01:48:50.000000 std.algorithm-1.1.4/std/sets.py
+-rw-rw-rw-   0        0        0     1162 2022-10-07 01:27:48.000000 std.algorithm-1.1.4/std/tree.py
+-rw-rw-rw-   0        0        0      443 2023-03-17 14:49:04.000000 std.algorithm-1.1.4/std/unicode.py
+-rw-rw-rw-   0        0        0    35286 2023-02-05 04:04:59.000000 std.algorithm-1.1.4/std/xml.py
+drwxrwxrwx   0        0        0        0 2023-06-04 15:21:33.394823 std.algorithm-1.1.4/std.algorithm.egg-info/
+-rw-rw-rw-   0        0        0      324 2023-06-04 15:21:33.000000 std.algorithm-1.1.4/std.algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-06-04 15:21:33.000000 std.algorithm-1.1.4/std.algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 15:21:33.000000 std.algorithm-1.1.4/std.algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-04 15:21:33.000000 std.algorithm-1.1.4/std.algorithm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-04 15:21:33.000000 std.algorithm-1.1.4/std.algorithm.egg-info/top_level.txt
```

### Comparing `std.algorithm-1.1.3/std/MySQL.py` & `std.algorithm-1.1.4/std/MySQL.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             self.conn = mysql.connector.connect(user=user, password=password, host=host, database=database)
         except mysql.connector.errors.ProgrammingError as err:
             print(err.msg)
             m = re.compile("Unknown database '(\w+)'").search(err.msg)
             assert m
             assert m[1] == database
             self.conn = mysql.connector.connect(user=user, password=password, host=host, database='mysql')
-            self.cursor.execute("create database " + database)
+            self.execute("create database " + database)
             self.conn = mysql.connector.connect(user=user, password=password, host=host, database=database)
 
     def cursor(self, **kwargs):
         return self.conn.cursor(**kwargs)
 
     @property
     def wait_timeout(self):
@@ -331,14 +331,35 @@
                 print('offset =', off + offset)
                 [*data] = self.query(sql, order=order, limit=fetch_size, offset=off + offset, dictionary=dictionary)
                 yield from data
                 
         else:
             yield from self.query(sql, order=order, limit=limit, offset=offset, dictionary=dictionary)
 
+    def __call__(self):
+#         import mysql.connector.pooling
+#          
+#         config = {
+#           "user": "yourusername",
+#           "password": "yourpassword",
+#           "host": "yourhost",
+#           "database": "yourdatabase"
+#         }
+#          
+#         cnxpool = mysql.connector.pooling.MySQLConnectionPool(pool_name="mypool", pool_size=20, **config)
+#          
+#         cnx = cnxpool.get_connection()
+#          
+#         cursor = cnx.cursor()
+#         cursor.execute("SELECT * FROM mytable")
+#          
+#         cursor.close()
+#         cnx.close()        
+        return MySQLConnector()
+
 instance = MySQLConnector()
 
 
 def is_number(Type):
     return re.match('tinyint\(\d+\)|double', Type)
```

### Comparing `std.algorithm-1.1.3/std/__init__.py` & `std.algorithm-1.1.4/std/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-import os
-import json
-import time
-import queue
+import os, json, time, queue, inspect, functools, sys, signal
 from _collections import defaultdict
-import inspect
-import functools
-import sys
 from enum import Enum, unique
-import signal
 
 
 def is_Windows():
     return os.sep == '\\'
 
     
 # is Linux System
@@ -506,27 +499,42 @@
             if self.logger:
                 self.logger.info(message)
             else:
                 print(message)
         
     def __enter__(self):
         self.start = time.time()
+
+    @property
+    def HHmmss(self):
+        lapse = time.time() - self.start
+        seconds = lapse % 60
+        minutes = int(lapse // 60)
+        if minutes > 0:
+            hours = minutes // 60
+            if hours > 0:
+                minutes %= 60
+                return "%02d:%02d:%02d" % (hours, minutes, seconds)
+            
+            return "%02d:%02d" % (minutes, seconds)
         
+        return "%.2f seconds" % seconds
+
     def __exit__(self, *_): 
-        lapse = time.time() - self.start
         if self.message:
-            msg = f'time cost for {self.message} is %.2f seconds' % lapse
+            msg = f'time cost for {self.message} is %s' % self.HHmmss
         else:
-            msg = 'time cost is %.2f seconds' % lapse
+            msg = 'time cost is %s' % self.HHmmss
             
         if self.logger:
             self.logger.info(msg)
         else:
             print(msg)
 
+
 class Timeout:
     """Timeout class using ALARM signal."""
     def __init__(self, sec):
         self.sec = sec
  
     def __enter__(self):
         signal.signal(signal.SIGALRM, self.raise_timeout)
@@ -739,14 +747,15 @@
     else:
         args, = args
         for key, value in args:
             obj[key] = value
 
     return obj
 
+
 def array_split(arr, index):
     if isinstance(index, int):
         return arr[:index], arr[index:]
     
     if isinstance(index, slice):
         start, stop, step = index.start, index.stop, index.step
         if step is None:
@@ -764,14 +773,16 @@
                 stop += len(arr)
 
             if step > 1:
                 rest = (arr[i] for i in {*range(start, stop)} - {*range(start, stop, step)})
                 rest = arr[:start] + type(arr)(rest) + arr[stop:]
             else:
                 rest = arr[:start] + arr[stop:]
+                
+            return arr[index], rest
         else:
             if start is None:
                 start = len(arr) - 1
             elif start < 0:
                 start += len(arr)
 
             if stop is None:
@@ -781,15 +792,15 @@
             
             if step < -1:
                 rest = (arr[i] for i in {*range(start, stop, -1)} - {*range(start, stop, step)})
                 rest = arr[:stop + 1] + type(arr)(rest) + arr[start + 1:]
             else:
                 rest = arr[:stop + 1] + arr[start + 1:]
 
-        return arr[index], rest
+            return rest, arr[index] 
 
 
 if __name__ == '__main__':
     arr = [*range(10)]
     former, latter = array_split(arr, slice(-2, -8, -2))
     print(former)
     print(latter)
```

### Comparing `std.algorithm-1.1.3/std/combinatorics.py` & `std.algorithm-1.1.4/std/combinatorics.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.3/std/data.py` & `std.algorithm-1.1.4/std/data.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.3/std/file.py` & `std.algorithm-1.1.4/std/file.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.3/std/http.py` & `std.algorithm-1.1.4/std/http.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.3/std/keras.py` & `std.algorithm-1.1.4/std/keras.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from std.data import numpify
 
 from _collections import defaultdict
 from types import FunctionType, MethodType
 import inspect
 import traceback
 
+def is_torch(model):
+    # Method Resolution Order by C3 Linearization algorithm
+    return any(str(t) == "<class 'torch.nn.modules.module.Module'>" for t in reversed(type(model).__mro__))
+
 def availableGPU():
 # pip install nvidia-ml-py3
     try:
         import pynvml  # @UnresolvedImport
         pynvml.nvmlInit()
     except Exception as e:
         print(e)
@@ -45,14 +49,19 @@
         print('maxFreeMemory * 0.9 =', maxFreeMemory * 0.9)
         if meminfo.free > maxFreeMemory * 0.999999:
             ids.add(i)
     
     print('ids =', ids)
     device_id = [*ids][random.randrange(0, len(ids))]
     print('selected device_id =', device_id)
+    import os
+    gpu_count = os.environ.get('gpu_count')
+    if gpu_count:
+        ...
+        
     return device_id
 
 def initialize_vocab(file, start=2):
     index = start
     vocab = {}
     from std.file import Text
     for word in Text(file):
@@ -170,19 +179,17 @@
         self.lang = kwargs.pop('lang', None)
         
         if hasattr(self, 'model'):
             if self.is_torch:
                 self.model.eval()
                 import torch
                 if torch.cuda.is_available():
-                    device = availableGPU()
-                    if device >= 0:
-                        self.model.to(device)
-                        self.device = device
-                        return
+                    self.model.to(0)
+                    self.device = 0
+                    return
 
         self.device = -1
 
     def replace_vocab(self, vocab, limit):
 
         def replace_vocab(vocab):
             deletes = set()
@@ -519,38 +526,36 @@
             import torch
             iostream = torch.no_grad()(iostream)
         return iostream
         
     def save_weights(self):
         modelFile = self.modelFile
         print('\nsaving model to', modelFile)
+        import os
+        from std.file import createNewPath
+        createNewPath(os.path.dirname(modelFile))
+
         if modelFile.endswith('.h5'):
             import h5py
-            try:
-                with h5py.File(modelFile, 'w') as f:
-                    self.iostream(self.model, f, mode='w')
-            except FileNotFoundError:
-                import os
-                std.file.createNewPath(os.path.dirname(modelFile))
-                with h5py.File(modelFile, 'w') as f:
-                    self.iostream(self.model, f, mode='w')
+            with h5py.File(modelFile, 'w') as f:
+                self.iostream(self.model, f, mode='w')
+
         elif modelFile.endswith('.pt'):
             import torch
-            try:
-                torch.save(self.model, modelFile)
-            except FileNotFoundError:
-                import os
-                std.file.createNewPath(os.path.dirname(modelFile))
-                torch.save(self.model, modelFile)
+            torch.save(self.model, modelFile)
 
+        elif modelFile.endswith('.bin'):
+            import torch
+            torch.save(self.model.state_dict(), modelFile)
+                
     @computed
     def is_torch(self):
-        return str(type(self.model).__mro__[-2]) == "<class 'torch.nn.modules.module.Module'>"
+        return is_torch(self.model)
+
 
-            
 def get_tensor_shape(tensor, axis=None):
     if axis is None:
         shape = []
         while isinstance(tensor, (list, tuple)):
             shape.append(len(tensor))    
             tensor = tensor[0]
             
@@ -647,50 +652,54 @@
             for x_name in self.x_name:
                 training_list = counting_sort(training_list, x_name, reverse=reverse)
             self.training_list = training_list
         
     def __getitem__(self, index):
         return self.arr[index]
     
+    def get_memory_allocation(self, tensor):
+        shape = get_tensor_shape(tensor)
+        if isinstance(self.dynamic_size, (FunctionType, MethodType)):
+            return self.dynamic_size(*shape)
+
+        from _functools import reduce
+        return reduce(lambda x, y: x * y, shape)
+        
     def batches(self): 
         if self.dynamic_size:
             if isinstance(self.x_name, str):
                 x_name = self.x_name
             else:
                 x_name = self.x_name[0]
                 
-            from _functools import reduce
-            seq_length = 0
+            memorySize = 0
             for inst in self.training_list:
-                shape = get_tensor_shape(getattr(inst, x_name))
+                memorySize += self.get_memory_allocation(getattr(inst, x_name))
 
-                if isinstance(self.dynamic_size, (FunctionType, MethodType)):
-                    seq_length += self.dynamic_size(*shape)
-                else:
-                    seq_length += reduce(lambda x, y: x * y, shape)
+            memorySize /= len(self.training_list)
+            batch_memory = self.batch_size * memorySize
+            
+            batch_size = self.batch_size
+            _memorySize = self.get_memory_allocation(getattr(self.training_list[batch_size - 1], x_name))
+            if _memorySize < memorySize:
+                _batch_size = max(1, int(batch_memory / _memorySize))
+                if _batch_size > batch_size:
+                    batch_size = _batch_size
+                    memorySize = _memorySize
+                    print('initial batch_size =', batch_size)
 
-            seq_length /= len(self.training_list)
-            average_memory = self.batch_size * seq_length
             i = 0
-            batch_size = self.batch_size
             while i < len(self.training_list):
-                batch = self.training_list[i:i + batch_size]
-                shape = get_tensor_shape(getattr(batch[-1], x_name))
-                
-                if isinstance(self.dynamic_size, (FunctionType, MethodType)):
-                    _seq_length = self.dynamic_size(*shape)
-                else:
-                    _seq_length = reduce(lambda x, y: x * y, shape)
-                
-                if _seq_length > seq_length:
-                    seq_length = _seq_length
-                    _batch_size = max(1, int(average_memory / seq_length))
+                _memorySize = self.get_memory_allocation(getattr(self.training_list[i + batch_size - 1], x_name))
+                if _memorySize > memorySize:
+                    _batch_size = max(1, int(batch_memory / _memorySize))
                     if _batch_size < batch_size:
                         batch_size = _batch_size
-                        print('adjust batch_size to', batch_size, 'for', shape)
+                        memorySize = _memorySize
+                        print('adjust batch_size to', batch_size)
      
                 yield self.training_list[i:i + batch_size]
                 i += batch_size
         else: 
             for i in range(0, len(self.training_list), self.batch_size):
                 yield self.training_list[i:i + self.batch_size]
 
@@ -1155,8 +1164,8 @@
         else:
             step_metrics = {method_name(self.accuracy): self.accuracy(y_true, y_pred)}
         
         return loss, loss_dict, step_metrics
 
     @computed
     def is_torch(self):
-        return str(type(self.model).__mro__[-2]) == "<class 'torch.nn.modules.module.Module'>"
+        return is_torch(self.model)
```

### Comparing `std.algorithm-1.1.3/std/lib/eigen.dll` & `std.algorithm-1.1.4/std/lib/eigen.dll`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.3/std/nlp.py` & `std.algorithm-1.1.4/std/nlp.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.3/std/search.py` & `std.algorithm-1.1.4/std/search.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.3/std/sets.py` & `std.algorithm-1.1.4/std/sets.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.3/std/tree.py` & `std.algorithm-1.1.4/std/tree.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.3/std/xml.py` & `std.algorithm-1.1.4/std/xml.py`

 * *Files identical despite different names*

