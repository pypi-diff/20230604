# Comparing `tmp/once-utils-0.0.4.tar.gz` & `tmp/once-utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "once-utils-0.0.4.tar", last modified: Sat Oct  8 16:05:55 2022, max compression
+gzip compressed data, was "once-utils-0.0.5.tar", last modified: Sun Jun  4 14:42:52 2023, max compression
```

## Comparing `once-utils-0.0.4.tar` & `once-utils-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-10-08 16:05:55.134197 once-utils-0.0.4/
--rw-rw-rw-   0        0        0      800 2022-10-08 16:05:55.133197 once-utils-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       56 2022-09-25 12:18:04.000000 once-utils-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2022-10-08 16:05:55.119197 once-utils-0.0.4/once_utils.egg-info/
--rw-rw-rw-   0        0        0      800 2022-10-08 16:05:55.000000 once-utils-0.0.4/once_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2022-10-08 16:05:55.000000 once-utils-0.0.4/once_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-08 16:05:55.000000 once-utils-0.0.4/once_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-10-08 16:05:55.000000 once-utils-0.0.4/once_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-08 16:05:55.128198 once-utils-0.0.4/onceutils/
--rw-rw-rw-   0        0        0      160 2022-09-24 05:45:52.000000 once-utils-0.0.4/onceutils/__init__.py
--rw-rw-rw-   0        0        0     3469 2022-10-08 15:55:55.000000 once-utils-0.0.4/onceutils/_cmd.py
--rw-rw-rw-   0        0        0     1115 2022-09-10 06:29:17.000000 once-utils-0.0.4/onceutils/_convert.py
--rw-rw-rw-   0        0        0      436 2022-09-24 05:27:27.000000 once-utils-0.0.4/onceutils/_iter.py
--rw-rw-rw-   0        0        0      629 2022-08-26 16:47:36.000000 once-utils-0.0.4/onceutils/_pymodule.py
--rw-rw-rw-   0        0        0     6652 2022-09-25 11:20:31.000000 once-utils-0.0.4/onceutils/_random.py
--rw-rw-rw-   0        0        0      618 2022-09-24 13:55:11.000000 once-utils-0.0.4/onceutils/const.py
-drwxrwxrwx   0        0        0        0 2022-10-08 16:05:55.130197 once-utils-0.0.4/onceutils/github/
--rw-rw-rw-   0        0        0        0 2022-08-28 14:34:38.000000 once-utils-0.0.4/onceutils/github/__init__.py
--rw-rw-rw-   0        0        0     4764 2022-08-29 14:40:26.000000 once-utils-0.0.4/onceutils/github/personal_token.py
-drwxrwxrwx   0        0        0        0 2022-10-08 16:05:55.132197 once-utils-0.0.4/onceutils/xjson/
--rw-rw-rw-   0        0        0      125 2022-08-28 14:34:36.000000 once-utils-0.0.4/onceutils/xjson/__init__.py
--rw-rw-rw-   0        0        0      736 2022-08-28 14:34:36.000000 once-utils-0.0.4/onceutils/xjson/encoder.py
--rw-rw-rw-   0        0        0       42 2022-10-08 16:05:55.134197 once-utils-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1165 2022-10-08 16:00:27.000000 once-utils-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:42:52.041295 once-utils-0.0.5/
+-rw-rw-rw-   0        0        0      852 2023-06-04 14:42:52.041295 once-utils-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2022-09-25 12:18:04.000000 once-utils-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 14:42:52.029190 once-utils-0.0.5/once_utils.egg-info/
+-rw-rw-rw-   0        0        0      852 2023-06-04 14:42:51.000000 once-utils-0.0.5/once_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2023-06-04 14:42:51.000000 once-utils-0.0.5/once_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:42:51.000000 once-utils-0.0.5/once_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 14:42:51.000000 once-utils-0.0.5/once_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 14:42:52.041295 once-utils-0.0.5/onceutils/
+-rw-rw-rw-   0        0        0      184 2023-04-16 05:52:44.000000 once-utils-0.0.5/onceutils/__init__.py
+-rw-rw-rw-   0        0        0     3805 2023-06-04 14:37:47.000000 once-utils-0.0.5/onceutils/_cmd.py
+-rw-rw-rw-   0        0        0     1115 2022-09-10 06:29:17.000000 once-utils-0.0.5/onceutils/_convert.py
+-rw-rw-rw-   0        0        0      436 2022-09-24 05:27:27.000000 once-utils-0.0.5/onceutils/_iter.py
+-rw-rw-rw-   0        0        0      629 2022-08-26 16:47:36.000000 once-utils-0.0.5/onceutils/_pymodule.py
+-rw-rw-rw-   0        0        0     6652 2022-09-25 11:20:31.000000 once-utils-0.0.5/onceutils/_random.py
+-rw-rw-rw-   0        0        0      618 2022-09-24 13:55:11.000000 once-utils-0.0.5/onceutils/const.py
+-rw-rw-rw-   0        0        0      322 2023-04-16 05:49:32.000000 once-utils-0.0.5/onceutils/ex_dict.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:42:52.041295 once-utils-0.0.5/onceutils/github/
+-rw-rw-rw-   0        0        0        0 2022-08-28 14:34:38.000000 once-utils-0.0.5/onceutils/github/__init__.py
+-rw-rw-rw-   0        0        0     4764 2022-08-29 14:40:26.000000 once-utils-0.0.5/onceutils/github/personal_token.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:42:52.041295 once-utils-0.0.5/onceutils/xjson/
+-rw-rw-rw-   0        0        0      125 2022-08-28 14:34:36.000000 once-utils-0.0.5/onceutils/xjson/__init__.py
+-rw-rw-rw-   0        0        0      736 2022-08-28 14:34:36.000000 once-utils-0.0.5/onceutils/xjson/encoder.py
+-rw-rw-rw-   0        0        0       42 2023-06-04 14:42:52.041295 once-utils-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-06-04 14:40:21.000000 once-utils-0.0.5/setup.py
```

### Comparing `once-utils-0.0.4/PKG-INFO` & `once-utils-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: once-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simplest utils.
 Home-page: https://github.com/Mingyueyixi/once-utils
 Author: Lu
 Author-email: Mingyueyixi@hotmail.com
 License: MIT Licence
 Keywords: pip,once-utils
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
 # once-utils
```

### Comparing `once-utils-0.0.4/once_utils.egg-info/PKG-INFO` & `once-utils-0.0.5/once_utils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: once-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simplest utils.
 Home-page: https://github.com/Mingyueyixi/once-utils
 Author: Lu
 Author-email: Mingyueyixi@hotmail.com
 License: MIT Licence
 Keywords: pip,once-utils
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
 # once-utils
```

### Comparing `once-utils-0.0.4/onceutils/_cmd.py` & `once-utils-0.0.5/onceutils/_cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 # -*- coding: utf-8 -*-
 # @Date:2021/07/15 9:44
 # @Author: Lu
 # @Description
 import io
-import os
 import subprocess
 import tempfile
 import time
-import traceback
 from concurrent.futures.thread import ThreadPoolExecutor
 from typing import Union
 
-import httpx
-import requests
-
 from onceutils import bin2text, text2bin
 
 
-def run_cmd(cmd, prt=True):
-    if prt:
-        print(cmd)
-    p = os.popen(cmd)
-    result = p.read()
-    p.close()
-    return result
+def run_cmd(cmd, prt=True, read=True):
+    return Shell().run(cmd, prt, read)
 
 
 class Shell(object):
+    def run(self, cmd: str, read=True, prt=True):
+        if prt:
+            print(cmd)
+        if read:
+            p = subprocess.run(cmd, text=False, stdout=subprocess.PIPE)
+            return bin2text(p.stdout)
+        subprocess.run(cmd, capture_output=False)
+
+
+class SameProcessShell(Shell):
     def __init__(self, shell_args='sh'):
         self.proc: subprocess.Popen = None
         self.shell_args = shell_args
         self.pool = ThreadPoolExecutor(max_workers=6)
 
     def run(self, cmd: str, timeout: Union[set, list, int] = (5, 5)):
+        """
+        Run cmd by the same process.
+        The result is only use on develop, because it was not unreliable
+        :param cmd: command line
+        :param timeout: read break when it timeout
+        :return: command's output
+        """
         if not cmd:
             return
         if type(timeout) is int:
             timeout = (timeout, timeout)
-        if not self.proc or self.proc.stdout.closed:
+        if not self.proc or self.proc.returncode is not None:
             std_out = self.stdout_io()
             std_err = self.stderr_io()
             self.proc = subprocess.Popen(args=self.shell_args,
                                          shell=True,
                                          text=False,
                                          start_new_session=True,
                                          stdin=subprocess.PIPE,
@@ -57,32 +64,27 @@
         proc.stdin.write(b_cmd + b'\n')
         proc.stdin.flush()
 
         # read result
         content = b''
         error = None
         try:
-            content = Shell._read_std_io(proc.stdout, timeout[0])
+            content = self._read_std_io(proc.stdout, timeout[0])
         except TimeoutError as e:
             # traceback.print_exc()
             pass
-        finally:
-            proc.stdout.close()
         try:
-            error = Shell._read_std_io(proc.stderr, timeout[1])
+            error = self._read_std_io(proc.stderr, timeout[1])
         except TimeoutError as e:
             # traceback.print_exc()
+            proc.terminate()
             pass
-        finally:
-            proc.stderr.close()
-        proc.terminate()
         return bin2text(content), bin2text(error)
 
-    @classmethod
-    def _read_std_io(cls, std_io: io.FileIO, timeout: int):
+    def _read_std_io(selp, std_io: io.FileIO, timeout: int):
         content = b''
         if not std_io:
             return content
         curr_time = time.time()
         while True:
             std_io.seek(0)
             rc = std_io.read()
```

### Comparing `once-utils-0.0.4/onceutils/_convert.py` & `once-utils-0.0.5/onceutils/_convert.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.4/onceutils/_pymodule.py` & `once-utils-0.0.5/onceutils/_pymodule.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.4/onceutils/_random.py` & `once-utils-0.0.5/onceutils/_random.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.4/onceutils/const.py` & `once-utils-0.0.5/onceutils/const.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.4/onceutils/github/personal_token.py` & `once-utils-0.0.5/onceutils/github/personal_token.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.4/onceutils/xjson/encoder.py` & `once-utils-0.0.5/onceutils/xjson/encoder.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.4/setup.py` & `once-utils-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,27 +9,28 @@
     with open(readme_md_path) as f:
         ret = f.read()
     return ret
 
 
 setup(
     name="once-utils",
-    version="0.0.4",
+    version="0.0.5",
     keywords=["pip", "once-utils"],
     description="Simplest utils.",
     long_description=readme_md(),
     long_description_content_type='text/markdown',
     license="MIT Licence",
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers'],
 
     url="https://github.com/Mingyueyixi/once-utils",
     author="Lu",
     author_email="Mingyueyixi@hotmail.com",
```

