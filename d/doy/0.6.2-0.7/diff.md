# Comparing `tmp/doy-0.6.2.tar.gz` & `tmp/doy-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doy-0.6.2.tar", max compression
+gzip compressed data, was "doy-0.7.tar", max compression
```

## Comparing `doy-0.6.2.tar` & `doy-0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-0.6.2/README.md
--rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-0.6.2/doy/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     6393 2022-12-22 18:58:47.001406 doy-0.6.2/doy/__init__.py
--rw-r--r--   0        0        0      307 2022-12-22 19:53:04.992628 doy-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 doy-0.6.2/setup.py
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 doy-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2022-08-20 20:46:44.060197 doy-0.7/README.md
+-rw-r--r--   0        0        0     1121 2022-08-23 10:22:09.091218 doy-0.7/doy/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     6950 2023-06-03 22:40:13.322565 doy-0.7/doy/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-03 22:42:01.559392 doy-0.7/pyproject.toml
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 doy-0.7/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 doy-0.7/PKG-INFO
```

### Comparing `doy-0.6.2/doy/.ipynb_checkpoints/__init__-checkpoint.py` & `doy-0.7/doy/.ipynb_checkpoints/__init__-checkpoint.py`

 * *Files identical despite different names*

### Comparing `doy-0.6.2/doy/__init__.py` & `doy-0.7/doy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import defaultdict
 from pathlib import Path
 import pickle
 import json
 import os
 from matplotlib import pyplot as plt
 import numpy as np
 from collections.abc import Iterable
@@ -206,13 +207,33 @@
     assert len(x.shape) == 4
     if isinstance(x, np.ndarray):
         return x.transpose(0, 3, 1, 2)
     else:
         return x.permute(0, 3, 1, 2)
 
 
-def pt2np(x):
-    return x.detach().cpu().numpy()
-
 
 def count_parameters(model, requires_grad_only=True):
-    return sum(p.numel() for p in model.parameters() if p.requires_grad or not requires_grad_only)
+    return sum(p.numel() for p in model.parameters() if p.requires_grad or not requires_grad_only)
+
+
+class Logger:
+
+    def __init__(self, use_wandb=True):
+        self.data = defaultdict(list)
+        self.use_wandb = use_wandb
+
+    def log(self, data, step):
+        for k, v in data.items():
+            try:
+                self.data[k].append(v.item())
+            except AttributeError:
+                self.data[k].append(v)
+        if self.use_wandb:
+            import wandb
+            wandb.log(data=data, step=step)
+
+    def get(self, key):
+        return self.data[key]
+
+    def get_sm(self, key, alpha=0.9):
+        return smooth_ema(self.data[key], alpha)
```

### Comparing `doy-0.6.2/setup.py` & `doy-0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.2,<4.0.0', 'numpy']
 
 setup_kwargs = {
     'name': 'doy',
-    'version': '0.6.2',
+    'version': '0.7',
     'description': '',
     'long_description': '# Doy\n\nSimple utility package\n',
     'author': 'Dominik Schmidt',
     'author_email': 'schmidtdominik30@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

