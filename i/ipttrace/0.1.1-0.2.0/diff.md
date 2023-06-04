# Comparing `tmp/ipttrace-0.1.1.tar.gz` & `tmp/ipttrace-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipttrace-0.1.1.tar", max compression
+gzip compressed data, was "ipttrace-0.2.0.tar", max compression
```

## Comparing `ipttrace-0.1.1.tar` & `ipttrace-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2302 2023-06-04 05:56:31.434312 ipttrace-0.1.1/ipttrace/main.py
--rw-r--r--   0        0        0      615 2023-06-04 07:59:37.941898 ipttrace-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      900 2023-06-04 07:59:52.954564 ipttrace-0.1.1/setup.py
--rw-r--r--   0        0        0      687 2023-06-04 07:59:52.954787 ipttrace-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2364 2023-06-04 15:00:38.061158 ipttrace-0.2.0/ipttrace/main.py
+-rw-r--r--   0        0        0      615 2023-06-04 13:12:18.867611 ipttrace-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      900 2023-06-04 15:01:08.756087 ipttrace-0.2.0/setup.py
+-rw-r--r--   0        0        0      687 2023-06-04 15:01:08.756330 ipttrace-0.2.0/PKG-INFO
```

### Comparing `ipttrace-0.1.1/ipttrace/main.py` & `ipttrace-0.2.0/ipttrace/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import subprocess
 import sys
-from dataclasses import dataclass, field, fields
+from dataclasses import asdict, dataclass, field, fields
 from signal import SIGINT, signal
 from types import FrameType
 from typing import Union
 
 from rich import print
 from typer import Argument, Typer
 from typing_extensions import Annotated
@@ -26,47 +26,49 @@
         run_cmd(
             f'iptables -t raw -L {chain} --line-numbers | grep TRACE | awk \'{{ print $1 }}\' | sort -r | xargs -I {{}} iptables -t raw -D {chain} {{}}'
         )
     if signum:
         sys.exit()
 
 
-def add_traces(match_rule: str):
+def set_traces(match_rule: str):
     for chain in ['PREROUTING', 'OUTPUT']:
         run_cmd(f'iptables -t raw -I {chain} 1 {match_rule} -j TRACE')
 
 
 @dataclass
 class Trace:
     IN: str
     OUT: str
     SRC: str
     DST: str
     PROTO: str
-    REF: str = field(repr=False)
+    SPT: str
+    DPT: str
+    REF: str
     RULE: str = field(init=False)
 
     def __post_init__(self):
-        table, chain, _, index = self.REF.split(':')
+        table, chain, index = self.REF.split('.')
         r = run_cmd(f'iptables -t {table} -nL {chain} {index}')
         self.RULE = re.sub(r'\s+', ' ', r.stdout.decode().strip())  # type: ignore
 
 
 def parse_log(log: str):
     T = re.split(r'\s+', log)
     K = [f.name for f in fields(Trace)]
-    D: dict[str, str] = {}
+    D = {'SPT': '', 'DPT': ''}
     for t in T:
         if '=' in t:
             k, v = t.split('=')
             if k in K:
                 D[k] = v
         elif 'rule:' in t:
-            D['REF'] = t
-    return Trace(**D)
+            D['REF'] = t.replace('rule:', '').replace(':', '.')
+    return asdict(Trace(**D))
 
 
 def poll_then_log():
     run_cmd('dmesg -C')
     proc = subprocess.Popen(['dmesg', '-w'], stdout=subprocess.PIPE)
     assert proc.stdout
     while True:
@@ -80,9 +82,9 @@
 def main(
     match_rule: Annotated[
         str, Argument(help='Will be passed to iptables to match packets.')
     ]
 ):
     signal(SIGINT, clear_traces)
     clear_traces()
-    add_traces(match_rule)
+    set_traces(match_rule)
     poll_then_log()
```

### Comparing `ipttrace-0.1.1/pyproject.toml` & `ipttrace-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipttrace"
-version = "0.1.1"
+version = "0.2.0"
 description = "trace iptables rules with ease"
 authors = ["sieginglion <sieginglion@gmail.com>"]
 repository = "https://github.com/sieginglion/ipttrace"
 
 [tool.poetry.dependencies]
 python = "^3.6.3"
 dataclasses = { version = "^0.8", python = "<3.7" }
```

### Comparing `ipttrace-0.1.1/setup.py` & `ipttrace-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {':python_version < "3.7"': ['dataclasses>=0.8,<0.9']}
 
 entry_points = \
 {'console_scripts': ['ipttrace = ipttrace.main:app']}
 
 setup_kwargs = {
     'name': 'ipttrace',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': 'trace iptables rules with ease',
     'long_description': None,
     'author': 'sieginglion',
     'author_email': 'sieginglion@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/sieginglion/ipttrace',
```

### Comparing `ipttrace-0.1.1/PKG-INFO` & `ipttrace-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipttrace
-Version: 0.1.1
+Version: 0.2.0
 Summary: trace iptables rules with ease
 Home-page: https://github.com/sieginglion/ipttrace
 Author: sieginglion
 Author-email: sieginglion@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

