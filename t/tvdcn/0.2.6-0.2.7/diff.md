# Comparing `tmp/tvdcn-0.2.6.tar.gz` & `tmp/tvdcn-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.2.6.tar", last modified: Sun May 21 03:58:32 2023, max compression
+gzip compressed data, was "tvdcn-0.2.7.tar", last modified: Sun Jun  4 20:31:18 2023, max compression
```

## Comparing `tvdcn-0.2.6.tar` & `tvdcn-0.2.7.tar`

### file list

```diff
@@ -1,48 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.107993 tvdcn-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 03:56:17.000000 tvdcn-0.2.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-05-21 03:58:32.107993 tvdcn-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-05-21 03:56:17.000000 tvdcn-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-21 03:56:17.000000 tvdcn-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-21 03:58:32.107993 tvdcn-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-21 03:56:17.000000 tvdcn-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.087992 tvdcn-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tests/test_compatibility_with_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.091992 tvdcn-0.2.6/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.091992 tvdcn-0.2.6/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.095992 tvdcn-0.2.6/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.099992 tvdcn-0.2.6/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26828 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27084 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.099992 tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.103993 tvdcn-0.2.6/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.103993 tvdcn-0.2.6/tvdcn/ops/activations/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/activations/mask_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/activations/mask_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    36102 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    39157 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-21 03:56:17.000000 tvdcn-0.2.6/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:58:32.091992 tvdcn-0.2.6/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 03:58:32.000000 tvdcn-0.2.6/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.596329 tvdcn-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-04 20:29:30.000000 tvdcn-0.2.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-04 20:29:30.000000 tvdcn-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-04 20:31:18.596329 tvdcn-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-04 20:29:30.000000 tvdcn-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-04 20:29:30.000000 tvdcn-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 20:29:30.000000 tvdcn-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-04 20:31:18.596329 tvdcn-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-04 20:29:30.000000 tvdcn-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.584329 tvdcn-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.584329 tvdcn-0.2.7/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.584329 tvdcn-0.2.7/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.588328 tvdcn-0.2.7/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.592329 tvdcn-0.2.7/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.592329 tvdcn-0.2.7/tvdcn/csrc/ops/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)    23154 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    29884 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    38246 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29905 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34420 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30898 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35780 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.592329 tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.596329 tvdcn-0.2.7/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.596329 tvdcn-0.2.7/tvdcn/ops/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/activations/mask_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/activations/mask_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36102 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39157 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-04 20:29:30.000000 tvdcn-0.2.7/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:31:18.584329 tvdcn-0.2.7/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 20:31:18.000000 tvdcn-0.2.7/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.2.6/LICENSE.txt` & `tvdcn-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/PKG-INFO` & `tvdcn-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.6
+Version: 0.2.7
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
```

### Comparing `tvdcn-0.2.6/README.md` & `tvdcn-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/pyproject.toml` & `tvdcn-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/setup.cfg` & `tvdcn-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/setup.py` & `tvdcn-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tests/test_compatibility_with_torchvision.py` & `tvdcn-0.2.7/tests/test_compatibility_with_torchvision.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tests/test_grad.py` & `tvdcn-0.2.7/tests/test_grad.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import torch
 from torch.autograd.gradcheck import gradcheck
 
 import tvdcn
 from utils.deform_conv_test_args import DeformConvTestArgs
 
 
-def test_deform_conv_grad(dim=2,
-                          transposed=False,
-                          dtype=torch.float64,
-                          device='cuda'):
+def test_deform_conv(dim=2,
+                     dtype=torch.float64,
+                     device='cuda'):
     torch.manual_seed(12)
-    conv_func = getattr(tvdcn, f'deform_conv{"_transpose" if transposed else ""}{dim}d')
-    args = DeformConvTestArgs(dim=dim, transposed=transposed, dtype=dtype, device=device)
+    conv_func = getattr(tvdcn, f'deform_conv{dim}d')
+    args = DeformConvTestArgs(dim=dim, transposed=False, dtype=dtype, device=device)
     print(args)
 
     c_output = conv_func(args.input,
                          args.weight,
                          args.offset,
                          args.mask,
                          args.bias,
@@ -39,9 +38,49 @@
                                                  args.dilation,
                                                  args.groups),
         (args.input, args.weight, args.offset, args.mask, args.bias), nondet_tol=args.tol)
     args.zero_grad()
     print('grad_check:', grad_ok)
 
 
+def test_deform_conv_transpose(dim=2,
+                               dtype=torch.float64,
+                               device='cuda'):
+    torch.manual_seed(12)
+    conv_func = getattr(tvdcn, f'deform_conv_transpose{dim}d')
+    args = DeformConvTestArgs(dim=dim, transposed=True, dtype=dtype, device=device)
+    print(args)
+
+    c_output = conv_func(args.input,
+                         args.weight,
+                         args.offset,
+                         args.mask,
+                         args.bias,
+                         args.stride,
+                         args.padding,
+                         args.output_padding,
+                         args.dilation,
+                         args.groups)
+    c_output.sum().backward()
+    c_input_grad = args.input.grad.clone()
+    c_weight_grad = args.weight.grad.clone()
+    c_offset_grad = args.offset.grad.clone()
+    c_mask_grad = args.mask.grad.clone()
+    c_bias_grad = args.bias.grad.clone()
+    args.zero_grad()
+    print(c_output)
+
+    grad_ok = gradcheck(
+        lambda inp, wei, off, msk, bi: conv_func(inp, wei, off, msk, bi,
+                                                 args.stride,
+                                                 args.padding,
+                                                 args.output_padding,
+                                                 args.dilation,
+                                                 args.groups),
+        (args.input, args.weight, args.offset, args.mask, args.bias), nondet_tol=args.tol)
+    args.zero_grad()
+    print('grad_check:', grad_ok)
+
+
 if __name__ == '__main__':
-    test_deform_conv_grad()
+    test_deform_conv()
+    test_deform_conv_transpose()
```

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
+#include <torch/autograd.h>
 #include "utils/parallel_helpers.h"
 #include "dispatch/deform_conv1d_kernels.h"
 
 namespace tvdcn {
     namespace ops {
         at::Tensor deform_conv1d_forward(
                 const at::Tensor &input,
@@ -465,9 +466,148 @@
             grad_weight = grad_weight.view_as(weight);
             grad_offset = grad_offset.view_as(offset);
             grad_mask = grad_mask.view_as(mask);
             grad_bias *= grad_out.sum(at::IntArrayRef({0, 2}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
+
+        class DeformConv1dFunction
+                : public torch::autograd::Function<DeformConv1dFunction> {
+        public:
+            static torch::autograd::variable_list forward(
+                    torch::autograd::AutogradContext *ctx,
+                    const torch::autograd::Variable &input,
+                    const torch::autograd::Variable &weight,
+                    const torch::autograd::Variable &offset,
+                    const torch::autograd::Variable &mask,
+                    const torch::autograd::Variable &bias,
+                    int64_t stride,
+                    int64_t pad,
+                    int64_t dilation,
+                    int64_t groups,
+                    int64_t offset_groups,
+                    int64_t mask_groups,
+                    bool deformable,
+                    bool modulated) {
+                at::AutoDispatchBelowADInplaceOrView g;
+                auto output = deform_conv1d_forward(
+                        input,
+                        weight,
+                        offset,
+                        mask,
+                        bias,
+                        stride,
+                        pad,
+                        dilation,
+                        groups,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated);
+
+                ctx->save_for_backward({input, weight, offset, mask, bias});
+                ctx->saved_data["stride"] = stride;
+                ctx->saved_data["pad"] = pad;
+                ctx->saved_data["dilation"] = dilation;
+                ctx->saved_data["groups"] = groups;
+                ctx->saved_data["offset_groups"] = offset_groups;
+                ctx->saved_data["mask_groups"] = mask_groups;
+                ctx->saved_data["deformable"] = deformable;
+                ctx->saved_data["modulated"] = modulated;
+
+                return {
+                        output,
+                };
+            }
+
+            static torch::autograd::variable_list backward(
+                    torch::autograd::AutogradContext *ctx,
+                    const torch::autograd::variable_list &grad_output) {
+                auto saved = ctx->get_saved_variables();
+                auto input = saved[0];
+                auto weight = saved[1];
+                auto offset = saved[2];
+                auto mask = saved[3];
+                auto bias = saved[4];
+
+                auto stride = ctx->saved_data["stride"].toInt();
+                auto pad = ctx->saved_data["pad"].toInt();
+                auto dilation = ctx->saved_data["dilation"].toInt();
+                auto groups = ctx->saved_data["groups"].toInt();
+                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
+                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
+                auto deformable = ctx->saved_data["deformable"].toBool();
+                auto modulated = ctx->saved_data["modulated"].toBool();
+
+                auto grads = deform_conv1d_backward(
+                        grad_output[0],
+                        input,
+                        weight,
+                        offset,
+                        mask,
+                        bias,
+                        stride,
+                        pad,
+                        dilation,
+                        groups,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated);
+                auto grad_input = std::get<0>(grads);
+                auto grad_weight = std::get<1>(grads);
+                auto grad_offset = std::get<2>(grads);
+                auto grad_mask = std::get<3>(grads);
+                auto grad_bias = std::get<4>(grads);
+
+                return {
+                        grad_input,
+                        grad_weight,
+                        grad_offset,
+                        grad_mask,
+                        grad_bias,
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                };
+            }
+        };
+
+        at::Tensor deform_conv1d(
+                const at::Tensor &input,
+                const at::Tensor &weight,
+                const at::Tensor &offset,
+                const at::Tensor &mask,
+                const at::Tensor &bias,
+                const int64_t stride,
+                const int64_t pad,
+                const int64_t dilation,
+                const int64_t groups,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
+                const bool deformable,
+                const bool modulated) {
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv1d");
+            auto result = DeformConv1dFunction::apply(
+                    input,
+                    weight,
+                    offset,
+                    mask,
+                    bias,
+                    stride,
+                    pad,
+                    dilation,
+                    groups,
+                    offset_groups,
+                    mask_groups,
+                    deformable,
+                    modulated);
+            return result[0];
+        }
     }
 }
```

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -65,34 +65,36 @@
 
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
+#include <torch/autograd.h>
 #include "utils/parallel_helpers.h"
-#include "dispatch/deform_conv2d_kernels.h"
+#include "dispatch/deform_conv1d_kernels.h"
 
 namespace tvdcn {
     namespace ops {
-        at::Tensor deform_conv2d_forward(
+        at::Tensor deform_conv_transpose1d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                const std::pair<int, int> &stride,
-                const std::pair<int, int> &padding,
-                const std::pair<int, int> &dilation,
+                const int stride,
+                const int padding,
+                const int output_padding,
+                const int dilation,
                 const int groups,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated) {
-            at::CheckedFrom c = "deform_conv2d_forward";
+            at::CheckedFrom c = "deform_conv_transpose1d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
             at::checkAllSameType(c, args);
@@ -101,452 +103,514 @@
 
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
-            TORCH_CHECK(input_c.ndimension() == 4)
-            TORCH_CHECK(!deformable || offset_c.ndimension() == 4)
-            TORCH_CHECK(!modulated || mask_c.ndimension() == 4)
-            TORCH_CHECK(weight_c.ndimension() == 4)
+            TORCH_CHECK(input_c.ndimension() == 3)
+            TORCH_CHECK(!deformable || offset_c.ndimension() == 3)
+            TORCH_CHECK(!modulated || mask_c.ndimension() == 3)
+            TORCH_CHECK(weight_c.ndimension() == 3)
 
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
-            int in_h = input_c.size(2);
-            int in_w = input_c.size(3);
+            int in_w = input_c.size(2);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(0);
-            int weight_h = weight_c.size(2);
-            int weight_w = weight_c.size(3);
+            int out_channels = weight_c.size(1) * groups;
+            int weight_w = weight_c.size(2);
 
-            int stride_h = stride.first;
-            int stride_w = stride.second;
+            int stride_w = stride;
 
-            int pad_h = padding.first;
-            int pad_w = padding.second;
+            int pad_w = padding;
 
-            int dilation_h = dilation.first;
-            int dilation_w = dilation.second;
+            int out_pad_w = output_padding;
 
-            int out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
-            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+            int dilation_w = dilation;
+
+            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
             TORCH_CHECK(
-                    weight_h > 0 && weight_w > 0,
-                    "weight_h: ",
-                    weight_h,
+                    weight_w > 0,
                     " weight_w: ",
                     weight_w)
             TORCH_CHECK(
-                    stride_h > 0 && stride_w > 0,
-                    "stride_h: ",
-                    stride_h,
+                    stride_w > 0,
                     " stride_w: ",
                     stride_w)
-            TORCH_CHECK(pad_h >= 0 && pad_w >= 0, "pad_h: ", pad_h, " pad_w: ", pad_w)
-            TORCH_CHECK(dilation_h > 0 && dilation_w > 0, "dilation_h: ", dilation_h, " dilation_w: ", dilation_w)
+            TORCH_CHECK(pad_w >= 0, " pad_w: ", pad_w)
+            TORCH_CHECK(dilation_w > 0, " dilation_w: ", dilation_w)
 
-            TORCH_CHECK(weight_c.size(1) * groups == in_channels)
+            TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
-                    (!deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w),
+                    (!deformable || offset_c.size(1) == offset_groups * weight_w),
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
-                    offset_groups * 2 * weight_h * weight_w)
+                    offset_groups * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
-                    (!deformable || (offset_c.size(2) == out_h &&
-                                     offset_c.size(3) == out_w)),
+                    (!deformable || offset_c.size(2) == in_w),
                     "offset output dims: (",
                     offset_c.size(2),
-                    ", ",
-                    offset_c.size(3),
                     ") - ",
-                    "computed output dims: (",
-                    out_h,
-                    ", ",
-                    out_w,
+                    "input dims: (",
+                    in_w,
                     ")")
 
             TORCH_CHECK(
-                    (!modulated || mask_c.size(1) == mask_groups * weight_h * weight_w),
+                    (!modulated || mask_c.size(1) == mask_groups * weight_w),
                     "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
-                    mask_groups * weight_h * weight_w)
+                    mask_groups * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == out_h &&
-                                    mask_c.size(3) == out_w)),
+                    (!modulated || mask_c.size(2) == in_w),
                     "mask output dims: (",
                     mask_c.size(2),
-                    ", ",
-                    mask_c.size(3),
                     ") - ",
-                    "computed output dims: (",
-                    out_h,
-                    ", ",
-                    out_w,
+                    "input dims: (",
+                    in_w,
                     ")")
 
             TORCH_CHECK(
-                    out_h > 0 && out_w > 0,
-                    "Calculated output size too small - out_h: ",
-                    out_h,
-                    " out_w: ",
+                    out_w > 0,
+                    "Calculated output size too small - out_w: ",
                     out_w)
 
-            auto output = at::zeros({batch_sz, out_channels, out_h, out_w}, input_c.options());
+            auto output = at::zeros({batch_sz, out_channels, out_w}, input_c.options());
 
             // Separate batches into blocks
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_h,
-                                    in_w});
+            output = output.view({batch_sz / n_parallel_imgs,
+                                  n_parallel_imgs,
+                                  out_channels,
+                                  out_w});
             if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
-                                          weight_h,
                                           weight_w,
-                                          2,
-                                          out_h,
-                                          out_w});
+                                          1,
+                                          in_w});
             else
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0});
+                                          0, 0, 0, 0});
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
-                                      weight_h,
                                       weight_w,
-                                      out_h,
-                                      out_w});
+                                      in_w});
             else
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
-                                      0, 0, 0, 0, 0});
-
-            output = output.view({batch_sz / n_parallel_imgs,
-                                  n_parallel_imgs,
-                                  out_channels,
-                                  out_h,
-                                  out_w});
-            auto output_buf = at::zeros(
-                    {batch_sz / n_parallel_imgs,
-                     out_channels,
-                     n_parallel_imgs,
-                     out_h,
-                     out_w},
-                    output.options());
+                                      0, 0, 0});
 
             // Separate channels into convolution groups
-            output_buf = output_buf.view({output_buf.size(0),
-                                          groups,
-                                          output_buf.size(1) / groups,
-                                          output_buf.size(2),
-                                          output_buf.size(3),
-                                          output_buf.size(4)});
+            input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                    n_parallel_imgs,
+                                    groups,
+                                    in_channels / groups,
+                                    in_w}).permute({0, 2, 3, 1, 4}).contiguous();
             weight_c = weight_c.view({groups,
                                       weight_c.size(0) / groups,
                                       weight_c.size(1),
-                                      weight_c.size(2),
-                                      weight_c.size(3)});
+                                      weight_c.size(2)});
 
             // Sample points and perform convolution
             auto columns = at::empty({groups,
-                                      in_channels * weight_h * weight_w / groups,
-                                      n_parallel_imgs * out_h * out_w},
+                                      out_channels * weight_w / groups,
+                                      n_parallel_imgs * in_w},
                                      input_c.options());
-            auto columns_view = columns.view({in_channels,
-                                              weight_h,
+            auto columns_view = columns.view({out_channels,
                                               weight_w,
                                               n_parallel_imgs,
-                                              out_h,
-                                              out_w});
+                                              in_w});
             for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                im2col(
-                        input_c[b],
+                columns.zero_();
+                for (int g = 0; g < groups; g++) {
+                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
+                }
+
+                auto output_b = output[b];
+                col2arr(
+                        columns_view,
                         offset_c[b],
                         mask_c[b],
-                        in_channels,
-                        in_h,
-                        in_w,
-                        weight_h,
+                        out_channels,
+                        out_w,
                         weight_w,
-                        stride_h,
                         stride_w,
-                        pad_h,
                         pad_w,
-                        dilation_h,
                         dilation_w,
-                        out_h,
-                        out_w,
+                        in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
-                        columns_view);
-
-                for (int g = 0; g < groups; g++) {
-                    output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
-                }
+                        output_b);
             }
 
-            output_buf = output_buf.view({batch_sz / n_parallel_imgs,
-                                          out_channels,
-                                          n_parallel_imgs,
-                                          out_h,
-                                          out_w});
-            output_buf.transpose_(1, 2);
-            output.copy_(output_buf);
-            output = output.view({batch_sz, out_channels, out_h, out_w});
+            output = output.view({batch_sz, out_channels, out_w});
 
-            return output + bias_c.view({1, out_channels, 1, 1});
+            return output + bias_c.view({1, out_channels, 1});
         }
 
         std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-        deform_conv2d_backward(
+        deform_conv_transpose1d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                const std::pair<int, int> &stride,
-                const std::pair<int, int> &padding,
-                const std::pair<int, int> &dilation,
+                const int stride,
+                const int padding,
+                const int output_padding,
+                const int dilation,
                 const int groups,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated) {
             at::Tensor grad_out_c = grad_out.contiguous();
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
-            int in_h = input_c.size(2);
-            int in_w = input_c.size(3);
+            int in_w = input_c.size(2);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(0);
-            int weight_h = weight_c.size(2);
-            int weight_w = weight_c.size(3);
+            int out_channels = weight_c.size(1) * groups;
+            int weight_w = weight_c.size(2);
 
-            int stride_h = stride.first;
-            int stride_w = stride.second;
+            int stride_w = stride;
 
-            int pad_h = padding.first;
-            int pad_w = padding.second;
+            int pad_w = padding;
 
-            int dilation_h = dilation.first;
-            int dilation_w = dilation.second;
+            int out_pad_w = output_padding;
 
-            int out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
-            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+            int dilation_w = dilation;
+
+            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
             auto grad_input = at::zeros_like(input_c);
             auto grad_weight = at::zeros_like(weight_c);
             auto grad_offset = at::zeros_like(offset_c);
             auto grad_mask = at::zeros_like(mask_c);
             auto grad_bias = at::ones_like(bias_c);
 
             // Separate into blocks
+            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          out_channels,
+                                          out_w});
+
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
-                                    in_h,
                                     in_w});
             grad_input = grad_input.view_as(input_c);
             if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
-                                          weight_h,
                                           weight_w,
-                                          2,
-                                          out_h,
-                                          out_w});
+                                          1,
+                                          in_w});
             else
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0});
+                                          0, 0, 0, 0});
             grad_offset = grad_offset.view_as(offset_c);
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
-                                      weight_h,
                                       weight_w,
-                                      out_h,
-                                      out_w});
+                                      in_w});
             else
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
-                                      0, 0, 0, 0, 0});
+                                      0, 0, 0});
             grad_mask = grad_mask.view_as(mask_c);
 
+            auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
+                                             in_channels,
+                                             n_parallel_imgs,
+                                             in_w}, input_c.options());
+
             // Separate channels into convolution groups
-            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          groups,
-                                          out_channels / groups,
-                                          out_h,
-                                          out_w}).permute({0, 2, 3, 1, 4, 5}).contiguous();
+            input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                    n_parallel_imgs,
+                                    groups,
+                                    in_channels / groups,
+                                    in_w}).permute({0, 2, 3, 1, 4}).contiguous();
+
+            grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
+                                                  groups,
+                                                  grad_input_buf.size(1) / groups,
+                                                  grad_input_buf.size(2),
+                                                  grad_input_buf.size(3)});
 
             weight_c = weight_c.view({groups,
-                                      out_channels / groups,
                                       in_channels / groups,
-                                      weight_h,
+                                      out_channels / groups,
                                       weight_w});
             grad_weight = grad_weight.view_as(weight_c);
 
             auto columns = at::empty({groups,
-                                      in_channels * weight_h * weight_w / groups,
-                                      n_parallel_imgs * out_h * out_w},
+                                      out_channels * weight_w / groups,
+                                      n_parallel_imgs * in_w},
                                      input_c.options());
-            auto columns_view = columns.view({in_channels,
-                                              weight_h,
+            auto columns_view = columns.view({out_channels,
                                               weight_w,
                                               n_parallel_imgs,
-                                              out_h,
-                                              out_w});
+                                              in_w});
             for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
                 columns.zero_();
                 for (int g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), grad_out_c[b][g].flatten(1));
+                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
                 }
 
                 auto grad_offset_b = grad_offset[b];
-                deform_conv2d_compute_grad_offset(
+                deform_conv1d_compute_grad_offset(
                         columns_view,
-                        input_c[b],
+                        grad_out_c[b],
                         offset_c[b],
                         mask_c[b],
-                        in_channels,
-                        in_h,
-                        in_w,
-                        weight_h,
+                        out_channels,
+                        out_w,
                         weight_w,
-                        stride_h,
                         stride_w,
-                        pad_h,
                         pad_w,
-                        dilation_h,
                         dilation_w,
-                        out_h,
-                        out_w,
+                        in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         grad_offset_b);
 
                 auto grad_mask_b = grad_mask[b];
-                deform_conv2d_compute_grad_mask(
+                deform_conv1d_compute_grad_mask(
                         columns_view,
-                        input_c[b],
+                        grad_out_c[b],
                         offset_c[b],
-                        in_channels,
-                        in_h,
-                        in_w,
-                        weight_h,
+                        out_channels,
+                        out_w,
                         weight_w,
-                        stride_h,
                         stride_w,
-                        pad_h,
                         pad_w,
-                        dilation_h,
                         dilation_w,
-                        out_h,
-                        out_w,
+                        in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         grad_mask_b);
 
-                auto grad_input_b = grad_input[b];
-                col2im(
-                        columns_view,
+                arr2col(
+                        grad_out_c[b],
                         offset_c[b],
                         mask_c[b],
-                        in_channels,
-                        in_h,
-                        in_w,
-                        weight_h,
-                        weight_w,
-                        stride_h,
-                        stride_w,
-                        pad_h,
-                        pad_w,
-                        dilation_h,
-                        dilation_w,
-                        out_h,
+                        out_channels,
                         out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_input_b);
-
-                im2col(
-                        input_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_h,
-                        in_w,
-                        weight_h,
                         weight_w,
-                        stride_h,
                         stride_w,
-                        pad_h,
                         pad_w,
-                        dilation_h,
                         dilation_w,
-                        out_h,
-                        out_w,
+                        in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
 
                 for (int g = 0; g < groups; g++) {
-                    grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                    grad_input_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                    grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
                 }
             }
 
+            grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
+                                                  in_channels,
+                                                  n_parallel_imgs,
+                                                  in_w}).transpose_(1, 2);
+            grad_input.copy_(grad_input_buf);
+
             grad_input = grad_input.view_as(input);
             grad_weight = grad_weight.view_as(weight);
             grad_offset = grad_offset.view_as(offset);
             grad_mask = grad_mask.view_as(mask);
-            grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
+            grad_bias *= grad_out.sum(at::IntArrayRef({0, 2}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
+
+        class DeformConvTranspose1dFunction
+                : public torch::autograd::Function<DeformConvTranspose1dFunction> {
+        public:
+            static torch::autograd::variable_list forward(
+                    torch::autograd::AutogradContext *ctx,
+                    const torch::autograd::Variable &input,
+                    const torch::autograd::Variable &weight,
+                    const torch::autograd::Variable &offset,
+                    const torch::autograd::Variable &mask,
+                    const torch::autograd::Variable &bias,
+                    int64_t stride,
+                    int64_t pad,
+                    int64_t out_pad,
+                    int64_t dilation,
+                    int64_t groups,
+                    int64_t offset_groups,
+                    int64_t mask_groups,
+                    bool deformable,
+                    bool modulated) {
+                at::AutoDispatchBelowADInplaceOrView g;
+                auto output = deform_conv_transpose1d_forward(
+                        input,
+                        weight,
+                        offset,
+                        mask,
+                        bias,
+                        stride,
+                        pad,
+                        out_pad,
+                        dilation,
+                        groups,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated);
+
+                ctx->save_for_backward({input, weight, offset, mask, bias});
+                ctx->saved_data["stride"] = stride;
+                ctx->saved_data["pad"] = pad;
+                ctx->saved_data["out_pad"] = out_pad;
+                ctx->saved_data["dilation"] = dilation;
+                ctx->saved_data["groups"] = groups;
+                ctx->saved_data["offset_groups"] = offset_groups;
+                ctx->saved_data["mask_groups"] = mask_groups;
+                ctx->saved_data["deformable"] = deformable;
+                ctx->saved_data["modulated"] = modulated;
+
+                return {
+                        output,
+                };
+            }
+
+            static torch::autograd::variable_list backward(
+                    torch::autograd::AutogradContext *ctx,
+                    const torch::autograd::variable_list &grad_output) {
+                auto saved = ctx->get_saved_variables();
+                auto input = saved[0];
+                auto weight = saved[1];
+                auto offset = saved[2];
+                auto mask = saved[3];
+                auto bias = saved[4];
+
+                auto stride = ctx->saved_data["stride"].toInt();
+                auto pad = ctx->saved_data["pad"].toInt();
+                auto out_pad = ctx->saved_data["out_pad"].toInt();
+                auto dilation = ctx->saved_data["dilation"].toInt();
+                auto groups = ctx->saved_data["groups"].toInt();
+                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
+                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
+                auto deformable = ctx->saved_data["deformable"].toBool();
+                auto modulated = ctx->saved_data["modulated"].toBool();
+
+                auto grads = deform_conv_transpose1d_backward(
+                        grad_output[0],
+                        input,
+                        weight,
+                        offset,
+                        mask,
+                        bias,
+                        stride,
+                        pad,
+                        out_pad,
+                        dilation,
+                        groups,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated);
+                auto grad_input = std::get<0>(grads);
+                auto grad_weight = std::get<1>(grads);
+                auto grad_offset = std::get<2>(grads);
+                auto grad_mask = std::get<3>(grads);
+                auto grad_bias = std::get<4>(grads);
+
+                return {
+                        grad_input,
+                        grad_weight,
+                        grad_offset,
+                        grad_mask,
+                        grad_bias,
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                };
+            }
+        };
+
+        at::Tensor deform_conv_transpose1d(
+                const at::Tensor &input,
+                const at::Tensor &weight,
+                const at::Tensor &offset,
+                const at::Tensor &mask,
+                const at::Tensor &bias,
+                const int64_t stride,
+                const int64_t pad,
+                const int64_t out_pad,
+                const int64_t dilation,
+                const int64_t groups,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
+                const bool deformable,
+                const bool modulated) {
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose1d");
+            auto result = DeformConvTranspose1dFunction::apply(
+                    input,
+                    weight,
+                    offset,
+                    mask,
+                    bias,
+                    stride,
+                    pad,
+                    out_pad,
+                    dilation,
+                    groups,
+                    offset_groups,
+                    mask_groups,
+                    deformable,
+                    modulated);
+            return result[0];
+        }
     }
 }
```

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -65,34 +65,36 @@
 
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
+#include <torch/autograd.h>
 #include "utils/parallel_helpers.h"
 #include "dispatch/deform_conv3d_kernels.h"
 
 namespace tvdcn {
     namespace ops {
-        at::Tensor deform_conv3d_forward(
+        at::Tensor deform_conv_transpose3d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 const std::tuple<int, int, int> &stride,
                 const std::tuple<int, int, int> &padding,
+                const std::tuple<int, int, int> &output_padding,
                 const std::tuple<int, int, int> &dilation,
                 const int groups,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated) {
-            at::CheckedFrom c = "deform_conv3d_forward";
+            at::CheckedFrom c = "deform_conv_transpose3d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
             at::checkAllSameType(c, args);
@@ -114,34 +116,38 @@
             int in_channels = input_c.size(1);
             int in_d = input_c.size(2);
             int in_h = input_c.size(3);
             int in_w = input_c.size(4);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(0);
+            int out_channels = weight_c.size(1) * groups;
             int weight_d = weight_c.size(2);
             int weight_h = weight_c.size(3);
             int weight_w = weight_c.size(4);
 
             int stride_d = std::get<0>(stride);
             int stride_h = std::get<1>(stride);
             int stride_w = std::get<2>(stride);
 
             int pad_d = std::get<0>(padding);
             int pad_h = std::get<1>(padding);
             int pad_w = std::get<2>(padding);
 
+            int out_pad_d = std::get<0>(output_padding);
+            int out_pad_h = std::get<1>(output_padding);
+            int out_pad_w = std::get<2>(output_padding);
+
             int dilation_d = std::get<0>(dilation);
             int dilation_h = std::get<1>(dilation);
             int dilation_w = std::get<2>(dilation);
 
-            int out_d = (in_d + 2 * pad_d - (dilation_d * (weight_d - 1) + 1)) / stride_d + 1;
-            int out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
-            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+            int out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
+            int out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
+            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
             TORCH_CHECK(
                     weight_d > 0 && weight_h > 0 && weight_w > 0,
                     "weight_d: ",
                     weight_d,
                     " weight_h: ",
                     weight_h,
@@ -155,223 +161,203 @@
                     stride_h,
                     " stride_w: ",
                     stride_w)
             TORCH_CHECK(pad_d >= 0 && pad_h >= 0 && pad_w >= 0, "pad_d: ", pad_d, " pad_h: ", pad_h, " pad_w: ", pad_w)
             TORCH_CHECK(dilation_d > 0 && dilation_h > 0 && dilation_w > 0, "dilation_d: ", dilation_d, " dilation_h: ",
                         dilation_h, " dilation_w: ", dilation_w)
 
-            TORCH_CHECK(weight_c.size(1) * groups == in_channels)
+            TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
                     (!deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w),
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
-                    (!deformable || (offset_c.size(2) == out_d &&
-                                     offset_c.size(3) == out_h &&
-                                     offset_c.size(4) == out_w)),
-                    "offset output dims: (",
+                    (!deformable || (offset_c.size(2) == in_d &&
+                                     offset_c.size(3) == in_h &&
+                                     offset_c.size(4) == in_w)),
+                    "offset input dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
                     ", ",
                     offset_c.size(4),
                     ") - ",
-                    "computed output dims: (",
-                    out_d,
+                    "input dims: (",
+                    in_d,
                     ", ",
-                    out_h,
+                    in_h,
                     ", ",
-                    out_w,
+                    in_w,
                     ")")
 
             TORCH_CHECK(
                     (!modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w),
                     "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_d * weight_h * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == out_d &&
-                                    mask_c.size(3) == out_h &&
-                                    mask_c.size(4) == out_w)),
-                    "mask output dims: (",
+                    (!modulated || (mask_c.size(2) == in_d &&
+                                    mask_c.size(3) == in_h &&
+                                    mask_c.size(4) == in_w)),
+                    "mask input dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
                     ", ",
                     mask_c.size(4),
                     ") - ",
-                    "computed output dims: (",
-                    out_d,
+                    "input dims: (",
+                    in_d,
                     ", ",
-                    out_h,
+                    in_h,
                     ", ",
-                    out_w,
+                    in_w,
                     ")")
 
             TORCH_CHECK(
                     out_d > 0 && out_h > 0 && out_w > 0,
                     "Calculated output size too small - out_d: ",
                     out_d,
                     " out_h: ",
                     out_h,
                     " out_w: ",
                     out_w)
 
             auto output = at::zeros({batch_sz, out_channels, out_d, out_h, out_w}, input_c.options());
 
             // Separate batches into blocks
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_d,
-                                    in_h,
-                                    in_w});
+            output = output.view({batch_sz / n_parallel_imgs,
+                                  n_parallel_imgs,
+                                  out_channels,
+                                  out_d,
+                                  out_h,
+                                  out_w});
             if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_d,
                                           weight_h,
                                           weight_w,
                                           3,
-                                          out_d,
-                                          out_h,
-                                          out_w});
+                                          in_d,
+                                          in_h,
+                                          in_w});
             else
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           0, 0, 0, 0, 0, 0, 0, 0});
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_d,
                                       weight_h,
                                       weight_w,
-                                      out_d,
-                                      out_h,
-                                      out_w});
+                                      in_d,
+                                      in_h,
+                                      in_w});
             else
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       0, 0, 0, 0, 0, 0, 0});
 
-            output = output.view({batch_sz / n_parallel_imgs,
-                                  n_parallel_imgs,
-                                  out_channels,
-                                  out_d,
-                                  out_h,
-                                  out_w});
-            auto output_buf = at::zeros(
-                    {batch_sz / n_parallel_imgs,
-                     out_channels,
-                     n_parallel_imgs,
-                     out_d,
-                     out_h,
-                     out_w},
-                    output.options());
-
             // Separate channels into convolution groups
-            output_buf = output_buf.view({output_buf.size(0),
-                                          groups,
-                                          output_buf.size(1) / groups,
-                                          output_buf.size(2),
-                                          output_buf.size(3),
-                                          output_buf.size(4),
-                                          output_buf.size(5)});
+            input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                    n_parallel_imgs,
+                                    groups,
+                                    in_channels / groups,
+                                    in_d,
+                                    in_h,
+                                    in_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
             weight_c = weight_c.view({groups,
                                       weight_c.size(0) / groups,
                                       weight_c.size(1),
                                       weight_c.size(2),
                                       weight_c.size(3),
                                       weight_c.size(4)});
 
             // Sample points and perform convolution
             auto columns = at::empty({groups,
-                                      in_channels * weight_d * weight_h * weight_w / groups,
-                                      n_parallel_imgs * out_d * out_h * out_w},
+                                      out_channels * weight_d * weight_h * weight_w / groups,
+                                      n_parallel_imgs * in_d * in_h * in_w},
                                      input_c.options());
-            auto columns_view = columns.view({in_channels,
+            auto columns_view = columns.view({out_channels,
                                               weight_d,
                                               weight_h,
                                               weight_w,
                                               n_parallel_imgs,
-                                              out_d,
-                                              out_h,
-                                              out_w});
+                                              in_d,
+                                              in_h,
+                                              in_w});
             for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                vol2col(
-                        input_c[b],
+                columns.zero_();
+                for (int g = 0; g < groups; g++) {
+                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
+                }
+
+                auto output_b = output[b];
+                col2vol(
+                        columns_view,
                         offset_c[b],
                         mask_c[b],
-                        in_channels,
-                        in_d,
-                        in_h,
-                        in_w,
+                        out_channels,
+                        out_d,
+                        out_h,
+                        out_w,
                         weight_d,
                         weight_h,
                         weight_w,
                         stride_d,
                         stride_h,
                         stride_w,
                         pad_d,
                         pad_h,
                         pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
-                        out_d,
-                        out_h,
-                        out_w,
+                        in_d,
+                        in_h,
+                        in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
-                        columns_view);
-
-                for (int g = 0; g < groups; g++) {
-                    output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
-                }
+                        output_b);
             }
 
-            output_buf = output_buf.view({batch_sz / n_parallel_imgs,
-                                          out_channels,
-                                          n_parallel_imgs,
-                                          out_d,
-                                          out_h,
-                                          out_w});
-            output_buf.transpose_(1, 2);
-            output.copy_(output_buf);
             output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
 
             return output + bias_c.view({1, out_channels, 1, 1, 1});
         }
 
         std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-        deform_conv3d_backward(
+        deform_conv_transpose3d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 const std::tuple<int, int, int> &stride,
                 const std::tuple<int, int, int> &padding,
+                const std::tuple<int, int, int> &output_padding,
                 const std::tuple<int, int, int> &dilation,
                 const int groups,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated) {
             at::Tensor grad_out_c = grad_out.contiguous();
@@ -385,42 +371,53 @@
             int in_channels = input_c.size(1);
             int in_d = input_c.size(2);
             int in_h = input_c.size(3);
             int in_w = input_c.size(4);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(0);
+            int out_channels = weight_c.size(1) * groups;
             int weight_d = weight_c.size(2);
             int weight_h = weight_c.size(3);
             int weight_w = weight_c.size(4);
 
             int stride_d = std::get<0>(stride);
             int stride_h = std::get<1>(stride);
             int stride_w = std::get<2>(stride);
 
             int pad_d = std::get<0>(padding);
             int pad_h = std::get<1>(padding);
             int pad_w = std::get<2>(padding);
 
+            int out_pad_d = std::get<0>(output_padding);
+            int out_pad_h = std::get<1>(output_padding);
+            int out_pad_w = std::get<2>(output_padding);
+
             int dilation_d = std::get<0>(dilation);
             int dilation_h = std::get<1>(dilation);
             int dilation_w = std::get<2>(dilation);
 
-            int out_d = (in_d + 2 * pad_d - (dilation_d * (weight_d - 1) + 1)) / stride_d + 1;
-            int out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
-            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+            int out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
+            int out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
+            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
             auto grad_input = at::zeros_like(input_c);
             auto grad_weight = at::zeros_like(weight_c);
             auto grad_offset = at::zeros_like(offset_c);
             auto grad_mask = at::zeros_like(mask_c);
             auto grad_bias = at::ones_like(bias_c);
 
             // Separate into blocks
+            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          out_channels,
+                                          out_d,
+                                          out_h,
+                                          out_w});
+
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
                                     in_d,
                                     in_h,
                                     in_w});
             grad_input = grad_input.view_as(input_c);
@@ -428,205 +425,393 @@
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
                                           weight_d,
                                           weight_h,
                                           weight_w,
                                           3,
-                                          out_d,
-                                          out_h,
-                                          out_w});
+                                          in_d,
+                                          in_h,
+                                          in_w});
             else
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           0, 0, 0, 0, 0, 0, 0, 0});
             grad_offset = grad_offset.view_as(offset_c);
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
                                       weight_d,
                                       weight_h,
                                       weight_w,
-                                      out_d,
-                                      out_h,
-                                      out_w});
+                                      in_d,
+                                      in_h,
+                                      in_w});
             else
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       0, 0, 0, 0, 0, 0, 0});
             grad_mask = grad_mask.view_as(mask_c);
 
+            auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
+                                             in_channels,
+                                             n_parallel_imgs,
+                                             in_d,
+                                             in_h,
+                                             in_w}, input_c.options());
+
             // Separate channels into convolution groups
-            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          groups,
-                                          out_channels / groups,
-                                          out_d,
-                                          out_h,
-                                          out_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
+            input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                    n_parallel_imgs,
+                                    groups,
+                                    in_channels / groups,
+                                    in_d,
+                                    in_h,
+                                    in_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
+
+            grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
+                                                  groups,
+                                                  grad_input_buf.size(1) / groups,
+                                                  grad_input_buf.size(2),
+                                                  grad_input_buf.size(3),
+                                                  grad_input_buf.size(4),
+                                                  grad_input_buf.size(5)});
 
             weight_c = weight_c.view({groups,
-                                      out_channels / groups,
                                       in_channels / groups,
+                                      out_channels / groups,
                                       weight_d,
                                       weight_h,
                                       weight_w});
             grad_weight = grad_weight.view_as(weight_c);
 
             auto columns = at::empty({groups,
-                                      in_channels * weight_d * weight_h * weight_w / groups,
-                                      n_parallel_imgs * out_d * out_h * out_w},
+                                      out_channels * weight_d * weight_h * weight_w / groups,
+                                      n_parallel_imgs * in_d * in_h * in_w},
                                      input_c.options());
-            auto columns_view = columns.view({in_channels,
+            auto columns_view = columns.view({out_channels,
                                               weight_d,
                                               weight_h,
                                               weight_w,
                                               n_parallel_imgs,
-                                              out_d,
-                                              out_h,
-                                              out_w});
+                                              in_d,
+                                              in_h,
+                                              in_w});
             for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
                 columns.zero_();
                 for (int g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), grad_out_c[b][g].flatten(1));
+                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
                 }
 
                 auto grad_offset_b = grad_offset[b];
                 deform_conv3d_compute_grad_offset(
                         columns_view,
-                        input_c[b],
+                        grad_out_c[b],
                         offset_c[b],
                         mask_c[b],
-                        in_channels,
-                        in_d,
-                        in_h,
-                        in_w,
+                        out_channels,
+                        out_d,
+                        out_h,
+                        out_w,
                         weight_d,
                         weight_h,
                         weight_w,
                         stride_d,
                         stride_h,
                         stride_w,
                         pad_d,
                         pad_h,
                         pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
-                        out_d,
-                        out_h,
-                        out_w,
+                        in_d,
+                        in_h,
+                        in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         grad_offset_b);
 
                 auto grad_mask_b = grad_mask[b];
                 deform_conv3d_compute_grad_mask(
                         columns_view,
-                        input_c[b],
+                        grad_out_c[b],
                         offset_c[b],
-                        in_channels,
-                        in_d,
-                        in_h,
-                        in_w,
-                        weight_d,
-                        weight_h,
-                        weight_w,
-                        stride_d,
-                        stride_h,
-                        stride_w,
-                        pad_d,
-                        pad_h,
-                        pad_w,
-                        dilation_d,
-                        dilation_h,
-                        dilation_w,
+                        out_channels,
                         out_d,
                         out_h,
                         out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        grad_mask_b);
-
-                auto grad_input_b = grad_input[b];
-                col2vol(
-                        columns_view,
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_d,
-                        in_h,
-                        in_w,
                         weight_d,
                         weight_h,
                         weight_w,
                         stride_d,
                         stride_h,
                         stride_w,
                         pad_d,
                         pad_h,
                         pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
-                        out_d,
-                        out_h,
-                        out_w,
+                        in_d,
+                        in_h,
+                        in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
-                        grad_input_b);
+                        grad_mask_b);
 
                 vol2col(
-                        input_c[b],
+                        grad_out_c[b],
                         offset_c[b],
                         mask_c[b],
-                        in_channels,
-                        in_d,
-                        in_h,
-                        in_w,
+                        out_channels,
+                        out_d,
+                        out_h,
+                        out_w,
                         weight_d,
                         weight_h,
                         weight_w,
                         stride_d,
                         stride_h,
                         stride_w,
                         pad_d,
                         pad_h,
                         pad_w,
                         dilation_d,
                         dilation_h,
                         dilation_w,
-                        out_d,
-                        out_h,
-                        out_w,
+                        in_d,
+                        in_h,
+                        in_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
 
                 for (int g = 0; g < groups; g++) {
-                    grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                    grad_input_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                    grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
                 }
             }
 
+            grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
+                                                  in_channels,
+                                                  n_parallel_imgs,
+                                                  in_d,
+                                                  in_h,
+                                                  in_w}).transpose_(1, 2);
+            grad_input.copy_(grad_input_buf);
+
             grad_input = grad_input.view_as(input);
             grad_weight = grad_weight.view_as(weight);
             grad_offset = grad_offset.view_as(offset);
             grad_mask = grad_mask.view_as(mask);
             grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3, 4}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
+
+        class DeformConvTranspose3dFunction
+                : public torch::autograd::Function<DeformConvTranspose3dFunction> {
+        public:
+            static torch::autograd::variable_list forward(
+                    torch::autograd::AutogradContext *ctx,
+                    const torch::autograd::Variable &input,
+                    const torch::autograd::Variable &weight,
+                    const torch::autograd::Variable &offset,
+                    const torch::autograd::Variable &mask,
+                    const torch::autograd::Variable &bias,
+                    int64_t stride_d,
+                    int64_t stride_h,
+                    int64_t stride_w,
+                    int64_t pad_d,
+                    int64_t pad_h,
+                    int64_t pad_w,
+                    int64_t out_pad_d,
+                    int64_t out_pad_h,
+                    int64_t out_pad_w,
+                    int64_t dilation_d,
+                    int64_t dilation_h,
+                    int64_t dilation_w,
+                    int64_t groups,
+                    int64_t offset_groups,
+                    int64_t mask_groups,
+                    bool deformable,
+                    bool modulated) {
+                at::AutoDispatchBelowADInplaceOrView g;
+                auto output = deform_conv_transpose3d_forward(
+                        input,
+                        weight,
+                        offset,
+                        mask,
+                        bias,
+                        std::make_tuple(stride_d, stride_h, stride_w),
+                        std::make_tuple(pad_d, pad_h, pad_w),
+                        std::make_tuple(out_pad_d, out_pad_h, out_pad_w),
+                        std::make_tuple(dilation_d, dilation_h, dilation_w),
+                        groups,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated);
+
+                ctx->save_for_backward({input, weight, offset, mask, bias});
+                ctx->saved_data["stride_d"] = stride_d;
+                ctx->saved_data["stride_h"] = stride_h;
+                ctx->saved_data["stride_w"] = stride_w;
+                ctx->saved_data["pad_d"] = pad_d;
+                ctx->saved_data["pad_h"] = pad_h;
+                ctx->saved_data["pad_w"] = pad_w;
+                ctx->saved_data["out_pad_d"] = out_pad_d;
+                ctx->saved_data["out_pad_h"] = out_pad_h;
+                ctx->saved_data["out_pad_w"] = out_pad_w;
+                ctx->saved_data["dilation_d"] = dilation_d;
+                ctx->saved_data["dilation_h"] = dilation_h;
+                ctx->saved_data["dilation_w"] = dilation_w;
+                ctx->saved_data["groups"] = groups;
+                ctx->saved_data["offset_groups"] = offset_groups;
+                ctx->saved_data["mask_groups"] = mask_groups;
+                ctx->saved_data["deformable"] = deformable;
+                ctx->saved_data["modulated"] = modulated;
+
+                return {
+                        output,
+                };
+            }
+
+            static torch::autograd::variable_list backward(
+                    torch::autograd::AutogradContext *ctx,
+                    const torch::autograd::variable_list &grad_output) {
+                auto saved = ctx->get_saved_variables();
+                auto input = saved[0];
+                auto weight = saved[1];
+                auto offset = saved[2];
+                auto mask = saved[3];
+                auto bias = saved[4];
+
+                auto stride_d = ctx->saved_data["stride_d"].toInt();
+                auto stride_h = ctx->saved_data["stride_h"].toInt();
+                auto stride_w = ctx->saved_data["stride_w"].toInt();
+                auto pad_d = ctx->saved_data["pad_d"].toInt();
+                auto pad_h = ctx->saved_data["pad_h"].toInt();
+                auto pad_w = ctx->saved_data["pad_w"].toInt();
+                auto out_pad_d = ctx->saved_data["out_pad_d"].toInt();
+                auto out_pad_h = ctx->saved_data["out_pad_h"].toInt();
+                auto out_pad_w = ctx->saved_data["out_pad_w"].toInt();
+                auto dilation_d = ctx->saved_data["dilation_d"].toInt();
+                auto dilation_h = ctx->saved_data["dilation_h"].toInt();
+                auto dilation_w = ctx->saved_data["dilation_w"].toInt();
+                auto groups = ctx->saved_data["groups"].toInt();
+                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
+                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
+                auto deformable = ctx->saved_data["deformable"].toBool();
+                auto modulated = ctx->saved_data["modulated"].toBool();
+
+                auto grads = deform_conv_transpose3d_backward(
+                        grad_output[0],
+                        input,
+                        weight,
+                        offset,
+                        mask,
+                        bias,
+                        std::make_tuple(stride_d, stride_h, stride_w),
+                        std::make_tuple(pad_d, pad_h, pad_w),
+                        std::make_tuple(out_pad_d, out_pad_h, out_pad_w),
+                        std::make_tuple(dilation_d, dilation_h, dilation_w),
+                        groups,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated);
+                auto grad_input = std::get<0>(grads);
+                auto grad_weight = std::get<1>(grads);
+                auto grad_offset = std::get<2>(grads);
+                auto grad_mask = std::get<3>(grads);
+                auto grad_bias = std::get<4>(grads);
+
+                return {
+                        grad_input,
+                        grad_weight,
+                        grad_offset,
+                        grad_mask,
+                        grad_bias,
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                };
+            }
+        };
+
+        at::Tensor deform_conv_transpose3d(
+                const at::Tensor &input,
+                const at::Tensor &weight,
+                const at::Tensor &offset,
+                const at::Tensor &mask,
+                const at::Tensor &bias,
+                const int64_t stride_d,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_d,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t out_pad_d,
+                const int64_t out_pad_h,
+                const int64_t out_pad_w,
+                const int64_t dilation_d,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t groups,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
+                const bool deformable,
+                const bool modulated) {
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose3d");
+            auto result = DeformConvTranspose3dFunction::apply(
+                    input,
+                    weight,
+                    offset,
+                    mask,
+                    bias,
+                    stride_d,
+                    stride_h,
+                    stride_w,
+                    pad_d,
+                    pad_h,
+                    pad_w,
+                    out_pad_d,
+                    out_pad_h,
+                    out_pad_w,
+                    dilation_d,
+                    dilation_h,
+                    dilation_w,
+                    groups,
+                    offset_groups,
+                    mask_groups,
+                    deformable,
+                    modulated);
+            return result[0];
+        }
     }
 }
```

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
+#include <torch/autograd.h>
 #include "utils/parallel_helpers.h"
 #include "dispatch/deform_conv2d_kernels.h"
 
 namespace tvdcn {
     namespace ops {
         at::Tensor deform_conv_transpose2d_forward(
                 const at::Tensor &input,
@@ -536,9 +537,180 @@
             grad_weight = grad_weight.view_as(weight);
             grad_offset = grad_offset.view_as(offset);
             grad_mask = grad_mask.view_as(mask);
             grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
+
+        class DeformConvTranspose2dFunction
+                : public torch::autograd::Function<DeformConvTranspose2dFunction> {
+        public:
+            static torch::autograd::variable_list forward(
+                    torch::autograd::AutogradContext *ctx,
+                    const torch::autograd::Variable &input,
+                    const torch::autograd::Variable &weight,
+                    const torch::autograd::Variable &offset,
+                    const torch::autograd::Variable &mask,
+                    const torch::autograd::Variable &bias,
+                    int64_t stride_h,
+                    int64_t stride_w,
+                    int64_t pad_h,
+                    int64_t pad_w,
+                    int64_t out_pad_h,
+                    int64_t out_pad_w,
+                    int64_t dilation_h,
+                    int64_t dilation_w,
+                    int64_t groups,
+                    int64_t offset_groups,
+                    int64_t mask_groups,
+                    bool deformable,
+                    bool modulated) {
+                at::AutoDispatchBelowADInplaceOrView g;
+                auto output = deform_conv_transpose2d_forward(
+                        input,
+                        weight,
+                        offset,
+                        mask,
+                        bias,
+                        std::make_pair(stride_h, stride_w),
+                        std::make_pair(pad_h, pad_w),
+                        std::make_pair(out_pad_h, out_pad_w),
+                        std::make_pair(dilation_h, dilation_w),
+                        groups,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated);
+
+                ctx->save_for_backward({input, weight, offset, mask, bias});
+                ctx->saved_data["stride_h"] = stride_h;
+                ctx->saved_data["stride_w"] = stride_w;
+                ctx->saved_data["pad_h"] = pad_h;
+                ctx->saved_data["pad_w"] = pad_w;
+                ctx->saved_data["out_pad_h"] = out_pad_h;
+                ctx->saved_data["out_pad_w"] = out_pad_w;
+                ctx->saved_data["dilation_h"] = dilation_h;
+                ctx->saved_data["dilation_w"] = dilation_w;
+                ctx->saved_data["groups"] = groups;
+                ctx->saved_data["offset_groups"] = offset_groups;
+                ctx->saved_data["mask_groups"] = mask_groups;
+                ctx->saved_data["deformable"] = deformable;
+                ctx->saved_data["modulated"] = modulated;
+
+                return {
+                        output,
+                };
+            }
+
+            static torch::autograd::variable_list backward(
+                    torch::autograd::AutogradContext *ctx,
+                    const torch::autograd::variable_list &grad_output) {
+                auto saved = ctx->get_saved_variables();
+                auto input = saved[0];
+                auto weight = saved[1];
+                auto offset = saved[2];
+                auto mask = saved[3];
+                auto bias = saved[4];
+
+                auto stride_h = ctx->saved_data["stride_h"].toInt();
+                auto stride_w = ctx->saved_data["stride_w"].toInt();
+                auto pad_h = ctx->saved_data["pad_h"].toInt();
+                auto pad_w = ctx->saved_data["pad_w"].toInt();
+                auto out_pad_h = ctx->saved_data["out_pad_h"].toInt();
+                auto out_pad_w = ctx->saved_data["out_pad_w"].toInt();
+                auto dilation_h = ctx->saved_data["dilation_h"].toInt();
+                auto dilation_w = ctx->saved_data["dilation_w"].toInt();
+                auto groups = ctx->saved_data["groups"].toInt();
+                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
+                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
+                auto deformable = ctx->saved_data["deformable"].toBool();
+                auto modulated = ctx->saved_data["modulated"].toBool();
+
+                auto grads = deform_conv_transpose2d_backward(
+                        grad_output[0],
+                        input,
+                        weight,
+                        offset,
+                        mask,
+                        bias,
+                        std::make_pair(stride_h, stride_w),
+                        std::make_pair(pad_h, pad_w),
+                        std::make_pair(out_pad_h, out_pad_w),
+                        std::make_pair(dilation_h, dilation_w),
+                        groups,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated);
+                auto grad_input = std::get<0>(grads);
+                auto grad_weight = std::get<1>(grads);
+                auto grad_offset = std::get<2>(grads);
+                auto grad_mask = std::get<3>(grads);
+                auto grad_bias = std::get<4>(grads);
+
+                return {
+                        grad_input,
+                        grad_weight,
+                        grad_offset,
+                        grad_mask,
+                        grad_bias,
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                };
+            }
+        };
+
+        at::Tensor deform_conv_transpose2d(
+                const at::Tensor &input,
+                const at::Tensor &weight,
+                const at::Tensor &offset,
+                const at::Tensor &mask,
+                const at::Tensor &bias,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t out_pad_h,
+                const int64_t out_pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t groups,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
+                const bool deformable,
+                const bool modulated) {
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose2d");
+            auto result = DeformConvTranspose2dFunction::apply(
+                    input,
+                    weight,
+                    offset,
+                    mask,
+                    bias,
+                    stride_h,
+                    stride_w,
+                    pad_h,
+                    pad_w,
+                    out_pad_h,
+                    out_pad_w,
+                    dilation_h,
+                    dilation_w,
+                    groups,
+                    offset_groups,
+                    mask_groups,
+                    deformable,
+                    modulated);
+            return result[0];
+        }
     }
 }
```

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -65,35 +65,35 @@
 
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
+#include <torch/autograd.h>
 #include "utils/parallel_helpers.h"
-#include "dispatch/deform_conv3d_kernels.h"
+#include "dispatch/deform_conv2d_kernels.h"
 
 namespace tvdcn {
     namespace ops {
-        at::Tensor deform_conv_transpose3d_forward(
+        at::Tensor deform_conv2d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                const std::tuple<int, int, int> &stride,
-                const std::tuple<int, int, int> &padding,
-                const std::tuple<int, int, int> &output_padding,
-                const std::tuple<int, int, int> &dilation,
+                const std::pair<int, int> &stride,
+                const std::pair<int, int> &padding,
+                const std::pair<int, int> &dilation,
                 const int groups,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated) {
-            at::CheckedFrom c = "deform_conv_transpose3d_forward";
+            at::CheckedFrom c = "deform_conv2d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
             at::checkAllSameType(c, args);
@@ -102,520 +102,609 @@
 
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
-            TORCH_CHECK(input_c.ndimension() == 5)
-            TORCH_CHECK(!deformable || offset_c.ndimension() == 5)
-            TORCH_CHECK(!modulated || mask_c.ndimension() == 5)
-            TORCH_CHECK(weight_c.ndimension() == 5)
+            TORCH_CHECK(input_c.ndimension() == 4)
+            TORCH_CHECK(!deformable || offset_c.ndimension() == 4)
+            TORCH_CHECK(!modulated || mask_c.ndimension() == 4)
+            TORCH_CHECK(weight_c.ndimension() == 4)
 
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
-            int in_d = input_c.size(2);
-            int in_h = input_c.size(3);
-            int in_w = input_c.size(4);
+            int in_h = input_c.size(2);
+            int in_w = input_c.size(3);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(1) * groups;
-            int weight_d = weight_c.size(2);
-            int weight_h = weight_c.size(3);
-            int weight_w = weight_c.size(4);
-
-            int stride_d = std::get<0>(stride);
-            int stride_h = std::get<1>(stride);
-            int stride_w = std::get<2>(stride);
-
-            int pad_d = std::get<0>(padding);
-            int pad_h = std::get<1>(padding);
-            int pad_w = std::get<2>(padding);
-
-            int out_pad_d = std::get<0>(output_padding);
-            int out_pad_h = std::get<1>(output_padding);
-            int out_pad_w = std::get<2>(output_padding);
-
-            int dilation_d = std::get<0>(dilation);
-            int dilation_h = std::get<1>(dilation);
-            int dilation_w = std::get<2>(dilation);
-
-            int out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
-            int out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
-            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+            int out_channels = weight_c.size(0);
+            int weight_h = weight_c.size(2);
+            int weight_w = weight_c.size(3);
+
+            int stride_h = stride.first;
+            int stride_w = stride.second;
+
+            int pad_h = padding.first;
+            int pad_w = padding.second;
+
+            int dilation_h = dilation.first;
+            int dilation_w = dilation.second;
+
+            int out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
+            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
             TORCH_CHECK(
-                    weight_d > 0 && weight_h > 0 && weight_w > 0,
-                    "weight_d: ",
-                    weight_d,
-                    " weight_h: ",
+                    weight_h > 0 && weight_w > 0,
+                    "weight_h: ",
                     weight_h,
                     " weight_w: ",
                     weight_w)
             TORCH_CHECK(
-                    stride_d > 0 && stride_h > 0 && stride_w > 0,
-                    " stride_d: ",
-                    stride_d,
+                    stride_h > 0 && stride_w > 0,
                     "stride_h: ",
                     stride_h,
                     " stride_w: ",
                     stride_w)
-            TORCH_CHECK(pad_d >= 0 && pad_h >= 0 && pad_w >= 0, "pad_d: ", pad_d, " pad_h: ", pad_h, " pad_w: ", pad_w)
-            TORCH_CHECK(dilation_d > 0 && dilation_h > 0 && dilation_w > 0, "dilation_d: ", dilation_d, " dilation_h: ",
-                        dilation_h, " dilation_w: ", dilation_w)
+            TORCH_CHECK(pad_h >= 0 && pad_w >= 0, "pad_h: ", pad_h, " pad_w: ", pad_w)
+            TORCH_CHECK(dilation_h > 0 && dilation_w > 0, "dilation_h: ", dilation_h, " dilation_w: ", dilation_w)
 
-            TORCH_CHECK(weight_c.size(1) * groups == out_channels)
+            TORCH_CHECK(weight_c.size(1) * groups == in_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
             TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
 
             TORCH_CHECK(
-                    (!deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w),
+                    (!deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w),
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
-                    offset_groups * 3 * weight_d * weight_h * weight_w)
+                    offset_groups * 2 * weight_h * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
-                    (!deformable || (offset_c.size(2) == in_d &&
-                                     offset_c.size(3) == in_h &&
-                                     offset_c.size(4) == in_w)),
-                    "offset input dims: (",
+                    (!deformable || (offset_c.size(2) == out_h &&
+                                     offset_c.size(3) == out_w)),
+                    "offset output dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
-                    ", ",
-                    offset_c.size(4),
                     ") - ",
-                    "input dims: (",
-                    in_d,
-                    ", ",
-                    in_h,
+                    "computed output dims: (",
+                    out_h,
                     ", ",
-                    in_w,
+                    out_w,
                     ")")
 
             TORCH_CHECK(
-                    (!modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w),
+                    (!modulated || mask_c.size(1) == mask_groups * weight_h * weight_w),
                     "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
-                    mask_groups * weight_d * weight_h * weight_w)
+                    mask_groups * weight_h * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == in_d &&
-                                    mask_c.size(3) == in_h &&
-                                    mask_c.size(4) == in_w)),
-                    "mask input dims: (",
+                    (!modulated || (mask_c.size(2) == out_h &&
+                                    mask_c.size(3) == out_w)),
+                    "mask output dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
-                    ", ",
-                    mask_c.size(4),
                     ") - ",
-                    "input dims: (",
-                    in_d,
-                    ", ",
-                    in_h,
+                    "computed output dims: (",
+                    out_h,
                     ", ",
-                    in_w,
+                    out_w,
                     ")")
 
             TORCH_CHECK(
-                    out_d > 0 && out_h > 0 && out_w > 0,
-                    "Calculated output size too small - out_d: ",
-                    out_d,
-                    " out_h: ",
+                    out_h > 0 && out_w > 0,
+                    "Calculated output size too small - out_h: ",
                     out_h,
                     " out_w: ",
                     out_w)
 
-            auto output = at::zeros({batch_sz, out_channels, out_d, out_h, out_w}, input_c.options());
+            auto output = at::zeros({batch_sz, out_channels, out_h, out_w}, input_c.options());
 
             // Separate batches into blocks
-            output = output.view({batch_sz / n_parallel_imgs,
-                                  n_parallel_imgs,
-                                  out_channels,
-                                  out_d,
-                                  out_h,
-                                  out_w});
+            input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                    n_parallel_imgs,
+                                    in_channels,
+                                    in_h,
+                                    in_w});
             if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
-                                          weight_d,
                                           weight_h,
                                           weight_w,
-                                          3,
-                                          in_d,
-                                          in_h,
-                                          in_w});
+                                          2,
+                                          out_h,
+                                          out_w});
             else
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0, 0, 0});
+                                          0, 0, 0, 0, 0, 0});
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
-                                      weight_d,
                                       weight_h,
                                       weight_w,
-                                      in_d,
-                                      in_h,
-                                      in_w});
+                                      out_h,
+                                      out_w});
             else
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
-                                      0, 0, 0, 0, 0, 0, 0});
+                                      0, 0, 0, 0, 0});
+
+            output = output.view({batch_sz / n_parallel_imgs,
+                                  n_parallel_imgs,
+                                  out_channels,
+                                  out_h,
+                                  out_w});
+            auto output_buf = at::zeros(
+                    {batch_sz / n_parallel_imgs,
+                     out_channels,
+                     n_parallel_imgs,
+                     out_h,
+                     out_w},
+                    output.options());
 
             // Separate channels into convolution groups
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    groups,
-                                    in_channels / groups,
-                                    in_d,
-                                    in_h,
-                                    in_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
+            output_buf = output_buf.view({output_buf.size(0),
+                                          groups,
+                                          output_buf.size(1) / groups,
+                                          output_buf.size(2),
+                                          output_buf.size(3),
+                                          output_buf.size(4)});
             weight_c = weight_c.view({groups,
                                       weight_c.size(0) / groups,
                                       weight_c.size(1),
                                       weight_c.size(2),
-                                      weight_c.size(3),
-                                      weight_c.size(4)});
+                                      weight_c.size(3)});
 
             // Sample points and perform convolution
             auto columns = at::empty({groups,
-                                      out_channels * weight_d * weight_h * weight_w / groups,
-                                      n_parallel_imgs * in_d * in_h * in_w},
+                                      in_channels * weight_h * weight_w / groups,
+                                      n_parallel_imgs * out_h * out_w},
                                      input_c.options());
-            auto columns_view = columns.view({out_channels,
-                                              weight_d,
+            auto columns_view = columns.view({in_channels,
                                               weight_h,
                                               weight_w,
                                               n_parallel_imgs,
-                                              in_d,
-                                              in_h,
-                                              in_w});
+                                              out_h,
+                                              out_w});
             for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                columns.zero_();
-                for (int g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
-                }
-
-                auto output_b = output[b];
-                col2vol(
-                        columns_view,
+                im2col(
+                        input_c[b],
                         offset_c[b],
                         mask_c[b],
-                        out_channels,
-                        out_d,
-                        out_h,
-                        out_w,
-                        weight_d,
+                        in_channels,
+                        in_h,
+                        in_w,
                         weight_h,
                         weight_w,
-                        stride_d,
                         stride_h,
                         stride_w,
-                        pad_d,
                         pad_h,
                         pad_w,
-                        dilation_d,
                         dilation_h,
                         dilation_w,
-                        in_d,
-                        in_h,
-                        in_w,
+                        out_h,
+                        out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
-                        output_b);
+                        columns_view);
+
+                for (int g = 0; g < groups; g++) {
+                    output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                }
             }
 
-            output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
+            output_buf = output_buf.view({batch_sz / n_parallel_imgs,
+                                          out_channels,
+                                          n_parallel_imgs,
+                                          out_h,
+                                          out_w});
+            output_buf.transpose_(1, 2);
+            output.copy_(output_buf);
+            output = output.view({batch_sz, out_channels, out_h, out_w});
 
-            return output + bias_c.view({1, out_channels, 1, 1, 1});
+            return output + bias_c.view({1, out_channels, 1, 1});
         }
 
         std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-        deform_conv_transpose3d_backward(
+        deform_conv2d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
-                const std::tuple<int, int, int> &stride,
-                const std::tuple<int, int, int> &padding,
-                const std::tuple<int, int, int> &output_padding,
-                const std::tuple<int, int, int> &dilation,
+                const std::pair<int, int> &stride,
+                const std::pair<int, int> &padding,
+                const std::pair<int, int> &dilation,
                 const int groups,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated) {
             at::Tensor grad_out_c = grad_out.contiguous();
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
             int batch_sz = input_c.size(0);
             int in_channels = input_c.size(1);
-            int in_d = input_c.size(2);
-            int in_h = input_c.size(3);
-            int in_w = input_c.size(4);
+            int in_h = input_c.size(2);
+            int in_w = input_c.size(3);
 
             int n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-            int out_channels = weight_c.size(1) * groups;
-            int weight_d = weight_c.size(2);
-            int weight_h = weight_c.size(3);
-            int weight_w = weight_c.size(4);
-
-            int stride_d = std::get<0>(stride);
-            int stride_h = std::get<1>(stride);
-            int stride_w = std::get<2>(stride);
-
-            int pad_d = std::get<0>(padding);
-            int pad_h = std::get<1>(padding);
-            int pad_w = std::get<2>(padding);
-
-            int out_pad_d = std::get<0>(output_padding);
-            int out_pad_h = std::get<1>(output_padding);
-            int out_pad_w = std::get<2>(output_padding);
-
-            int dilation_d = std::get<0>(dilation);
-            int dilation_h = std::get<1>(dilation);
-            int dilation_w = std::get<2>(dilation);
-
-            int out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
-            int out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
-            int out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+            int out_channels = weight_c.size(0);
+            int weight_h = weight_c.size(2);
+            int weight_w = weight_c.size(3);
+
+            int stride_h = stride.first;
+            int stride_w = stride.second;
+
+            int pad_h = padding.first;
+            int pad_w = padding.second;
+
+            int dilation_h = dilation.first;
+            int dilation_w = dilation.second;
+
+            int out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
+            int out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
             auto grad_input = at::zeros_like(input_c);
             auto grad_weight = at::zeros_like(weight_c);
             auto grad_offset = at::zeros_like(offset_c);
             auto grad_mask = at::zeros_like(mask_c);
             auto grad_bias = at::ones_like(bias_c);
 
             // Separate into blocks
-            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          out_channels,
-                                          out_d,
-                                          out_h,
-                                          out_w});
-
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
-                                    in_d,
                                     in_h,
                                     in_w});
             grad_input = grad_input.view_as(input_c);
             if (deformable)
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           offset_groups,
-                                          weight_d,
                                           weight_h,
                                           weight_w,
-                                          3,
-                                          in_d,
-                                          in_h,
-                                          in_w});
+                                          2,
+                                          out_h,
+                                          out_w});
             else
                 offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0, 0, 0});
+                                          0, 0, 0, 0, 0, 0});
             grad_offset = grad_offset.view_as(offset_c);
             if (modulated)
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       mask_groups,
-                                      weight_d,
                                       weight_h,
                                       weight_w,
-                                      in_d,
-                                      in_h,
-                                      in_w});
+                                      out_h,
+                                      out_w});
             else
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
-                                      0, 0, 0, 0, 0, 0, 0});
+                                      0, 0, 0, 0, 0});
             grad_mask = grad_mask.view_as(mask_c);
 
-            auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
-                                             in_channels,
-                                             n_parallel_imgs,
-                                             in_d,
-                                             in_h,
-                                             in_w}, input_c.options());
-
             // Separate channels into convolution groups
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    groups,
-                                    in_channels / groups,
-                                    in_d,
-                                    in_h,
-                                    in_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
-
-            grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
-                                                  groups,
-                                                  grad_input_buf.size(1) / groups,
-                                                  grad_input_buf.size(2),
-                                                  grad_input_buf.size(3),
-                                                  grad_input_buf.size(4),
-                                                  grad_input_buf.size(5)});
+            grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          groups,
+                                          out_channels / groups,
+                                          out_h,
+                                          out_w}).permute({0, 2, 3, 1, 4, 5}).contiguous();
 
             weight_c = weight_c.view({groups,
-                                      in_channels / groups,
                                       out_channels / groups,
-                                      weight_d,
+                                      in_channels / groups,
                                       weight_h,
                                       weight_w});
             grad_weight = grad_weight.view_as(weight_c);
 
             auto columns = at::empty({groups,
-                                      out_channels * weight_d * weight_h * weight_w / groups,
-                                      n_parallel_imgs * in_d * in_h * in_w},
+                                      in_channels * weight_h * weight_w / groups,
+                                      n_parallel_imgs * out_h * out_w},
                                      input_c.options());
-            auto columns_view = columns.view({out_channels,
-                                              weight_d,
+            auto columns_view = columns.view({in_channels,
                                               weight_h,
                                               weight_w,
                                               n_parallel_imgs,
-                                              in_d,
-                                              in_h,
-                                              in_w});
+                                              out_h,
+                                              out_w});
             for (int b = 0; b < batch_sz / n_parallel_imgs; b++) {
                 columns.zero_();
                 for (int g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
+                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), grad_out_c[b][g].flatten(1));
                 }
 
                 auto grad_offset_b = grad_offset[b];
-                deform_conv3d_compute_grad_offset(
+                deform_conv2d_compute_grad_offset(
                         columns_view,
-                        grad_out_c[b],
+                        input_c[b],
                         offset_c[b],
                         mask_c[b],
-                        out_channels,
-                        out_d,
-                        out_h,
-                        out_w,
-                        weight_d,
+                        in_channels,
+                        in_h,
+                        in_w,
                         weight_h,
                         weight_w,
-                        stride_d,
                         stride_h,
                         stride_w,
-                        pad_d,
                         pad_h,
                         pad_w,
-                        dilation_d,
                         dilation_h,
                         dilation_w,
-                        in_d,
-                        in_h,
-                        in_w,
+                        out_h,
+                        out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         grad_offset_b);
 
                 auto grad_mask_b = grad_mask[b];
-                deform_conv3d_compute_grad_mask(
+                deform_conv2d_compute_grad_mask(
                         columns_view,
-                        grad_out_c[b],
+                        input_c[b],
                         offset_c[b],
-                        out_channels,
-                        out_d,
-                        out_h,
-                        out_w,
-                        weight_d,
+                        in_channels,
+                        in_h,
+                        in_w,
                         weight_h,
                         weight_w,
-                        stride_d,
                         stride_h,
                         stride_w,
-                        pad_d,
                         pad_h,
                         pad_w,
-                        dilation_d,
                         dilation_h,
                         dilation_w,
-                        in_d,
-                        in_h,
-                        in_w,
+                        out_h,
+                        out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         grad_mask_b);
 
-                vol2col(
-                        grad_out_c[b],
+                auto grad_input_b = grad_input[b];
+                col2im(
+                        columns_view,
                         offset_c[b],
                         mask_c[b],
-                        out_channels,
-                        out_d,
-                        out_h,
-                        out_w,
-                        weight_d,
+                        in_channels,
+                        in_h,
+                        in_w,
                         weight_h,
                         weight_w,
-                        stride_d,
                         stride_h,
                         stride_w,
-                        pad_d,
                         pad_h,
                         pad_w,
-                        dilation_d,
                         dilation_h,
                         dilation_w,
-                        in_d,
+                        out_h,
+                        out_w,
+                        n_parallel_imgs,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated,
+                        grad_input_b);
+
+                im2col(
+                        input_c[b],
+                        offset_c[b],
+                        mask_c[b],
+                        in_channels,
                         in_h,
                         in_w,
+                        weight_h,
+                        weight_w,
+                        stride_h,
+                        stride_w,
+                        pad_h,
+                        pad_w,
+                        dilation_h,
+                        dilation_w,
+                        out_h,
+                        out_w,
                         n_parallel_imgs,
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
 
                 for (int g = 0; g < groups; g++) {
-                    grad_input_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
-                    grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                    grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
                 }
             }
 
-            grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
-                                                  in_channels,
-                                                  n_parallel_imgs,
-                                                  in_d,
-                                                  in_h,
-                                                  in_w}).transpose_(1, 2);
-            grad_input.copy_(grad_input_buf);
-
             grad_input = grad_input.view_as(input);
             grad_weight = grad_weight.view_as(weight);
             grad_offset = grad_offset.view_as(offset);
             grad_mask = grad_mask.view_as(mask);
-            grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3, 4}));
+            grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
 
             return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
         }
+
+        class DeformConv2dFunction
+                : public torch::autograd::Function<DeformConv2dFunction> {
+        public:
+            static torch::autograd::variable_list forward(
+                    torch::autograd::AutogradContext *ctx,
+                    const torch::autograd::Variable &input,
+                    const torch::autograd::Variable &weight,
+                    const torch::autograd::Variable &offset,
+                    const torch::autograd::Variable &mask,
+                    const torch::autograd::Variable &bias,
+                    int64_t stride_h,
+                    int64_t stride_w,
+                    int64_t pad_h,
+                    int64_t pad_w,
+                    int64_t dilation_h,
+                    int64_t dilation_w,
+                    int64_t groups,
+                    int64_t offset_groups,
+                    int64_t mask_groups,
+                    bool deformable,
+                    bool modulated) {
+                at::AutoDispatchBelowADInplaceOrView g;
+                auto output = deform_conv2d_forward(
+                        input,
+                        weight,
+                        offset,
+                        mask,
+                        bias,
+                        std::make_pair(stride_h, stride_w),
+                        std::make_pair(pad_h, pad_w),
+                        std::make_pair(dilation_h, dilation_w),
+                        groups,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated);
+
+                ctx->save_for_backward({input, weight, offset, mask, bias});
+                ctx->saved_data["stride_h"] = stride_h;
+                ctx->saved_data["stride_w"] = stride_w;
+                ctx->saved_data["pad_h"] = pad_h;
+                ctx->saved_data["pad_w"] = pad_w;
+                ctx->saved_data["dilation_h"] = dilation_h;
+                ctx->saved_data["dilation_w"] = dilation_w;
+                ctx->saved_data["groups"] = groups;
+                ctx->saved_data["offset_groups"] = offset_groups;
+                ctx->saved_data["mask_groups"] = mask_groups;
+                ctx->saved_data["deformable"] = deformable;
+                ctx->saved_data["modulated"] = modulated;
+
+                return {
+                        output,
+                };
+            }
+
+            static torch::autograd::variable_list backward(
+                    torch::autograd::AutogradContext *ctx,
+                    const torch::autograd::variable_list &grad_output) {
+                auto saved = ctx->get_saved_variables();
+                auto input = saved[0];
+                auto weight = saved[1];
+                auto offset = saved[2];
+                auto mask = saved[3];
+                auto bias = saved[4];
+
+                auto stride_h = ctx->saved_data["stride_h"].toInt();
+                auto stride_w = ctx->saved_data["stride_w"].toInt();
+                auto pad_h = ctx->saved_data["pad_h"].toInt();
+                auto pad_w = ctx->saved_data["pad_w"].toInt();
+                auto dilation_h = ctx->saved_data["dilation_h"].toInt();
+                auto dilation_w = ctx->saved_data["dilation_w"].toInt();
+                auto groups = ctx->saved_data["groups"].toInt();
+                auto offset_groups = ctx->saved_data["offset_groups"].toInt();
+                auto mask_groups = ctx->saved_data["mask_groups"].toInt();
+                auto deformable = ctx->saved_data["deformable"].toBool();
+                auto modulated = ctx->saved_data["modulated"].toBool();
+
+                auto grads = deform_conv2d_backward(
+                        grad_output[0],
+                        input,
+                        weight,
+                        offset,
+                        mask,
+                        bias,
+                        std::make_pair(stride_h, stride_w),
+                        std::make_pair(pad_h, pad_w),
+                        std::make_pair(dilation_h, dilation_w),
+                        groups,
+                        offset_groups,
+                        mask_groups,
+                        deformable,
+                        modulated);
+                auto grad_input = std::get<0>(grads);
+                auto grad_weight = std::get<1>(grads);
+                auto grad_offset = std::get<2>(grads);
+                auto grad_mask = std::get<3>(grads);
+                auto grad_bias = std::get<4>(grads);
+
+                return {
+                        grad_input,
+                        grad_weight,
+                        grad_offset,
+                        grad_mask,
+                        grad_bias,
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                        torch::autograd::Variable(),
+                };
+            }
+        };
+
+        at::Tensor deform_conv2d(
+                const at::Tensor &input,
+                const at::Tensor &weight,
+                const at::Tensor &offset,
+                const at::Tensor &mask,
+                const at::Tensor &bias,
+                const int64_t stride_h,
+                const int64_t stride_w,
+                const int64_t pad_h,
+                const int64_t pad_w,
+                const int64_t dilation_h,
+                const int64_t dilation_w,
+                const int64_t groups,
+                const int64_t offset_groups,
+                const int64_t mask_groups,
+                const bool deformable,
+                const bool modulated) {
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv2d");
+            auto result = DeformConv2dFunction::apply(
+                    input,
+                    weight,
+                    offset,
+                    mask,
+                    bias,
+                    stride_h,
+                    stride_w,
+                    pad_h,
+                    pad_w,
+                    dilation_h,
+                    dilation_w,
+                    groups,
+                    offset_groups,
+                    mask_groups,
+                    deformable,
+                    modulated);
+            return result[0];
+        }
     }
 }
```

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             if (input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 arr2col_cuda(input,
                              offset,
                              mask,
                              in_channels,
                              width,
                              weight_w,
                              stride_w,
@@ -80,15 +80,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             if (grad_input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 col2arr_cuda(columns,
                              offset,
                              mask,
                              in_channels,
                              width,
                              weight_w,
                              stride_w,
@@ -139,15 +139,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 deform_conv1d_compute_grad_offset_cuda(columns,
                                                        input,
                                                        offset,
                                                        mask,
                                                        in_channels,
                                                        width,
                                                        weight_w,
@@ -199,15 +199,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 deform_conv1d_compute_grad_mask_cuda(columns,
                                                      input,
                                                      offset,
                                                      in_channels,
                                                      width,
                                                      weight_w,
                                                      stride_w,
```

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             if (input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 im2col_cuda(input,
                             offset,
                             mask,
                             in_channels,
                             height,
                             width,
                             weight_h,
@@ -104,15 +104,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             if (grad_input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 col2im_cuda(columns,
                             offset,
                             mask,
                             in_channels,
                             height,
                             width,
                             weight_h,
@@ -181,15 +181,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 deform_conv2d_compute_grad_offset_cuda(columns,
                                                        input,
                                                        offset,
                                                        mask,
                                                        in_channels,
                                                        height,
                                                        width,
@@ -259,15 +259,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 deform_conv2d_compute_grad_mask_cuda(columns,
                                                      input,
                                                      offset,
                                                      in_channels,
                                                      height,
                                                      width,
                                                      weight_h,
```

### Comparing `tvdcn-0.2.6/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp` & `tvdcn-0.2.7/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &columns) {
             if (input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 vol2col_cuda(input,
                              offset,
                              mask,
                              in_channels,
                              depth,
                              height,
                              width,
@@ -128,15 +128,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_input) {
             if (grad_input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 col2vol_cuda(columns,
                              offset,
                              mask,
                              in_channels,
                              depth,
                              height,
                              width,
@@ -223,15 +223,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_offset) {
             if (input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 deform_conv3d_compute_grad_offset_cuda(columns,
                                                        input,
                                                        offset,
                                                        mask,
                                                        in_channels,
                                                        depth,
                                                        height,
@@ -319,15 +319,15 @@
                 const int batch_sz,
                 const int offset_groups,
                 const int mask_groups,
                 const bool deformable,
                 const bool modulated,
                 at::Tensor &grad_mask) {
             if (input.device().is_cuda()) {
-#if defined(WITH_CUDA) || defined(WITH_HIP)
+#if defined(WITH_CUDA)
                 deform_conv3d_compute_grad_mask_cuda(columns,
                                                      input,
                                                      offset,
                                                      in_channels,
                                                      depth,
                                                      height,
                                                      width,
```

### Comparing `tvdcn-0.2.6/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.2.7/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tvdcn/extension.py` & `tvdcn-0.2.7/tvdcn/extension.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tvdcn/ops/activations/mask_sigmoid.py` & `tvdcn-0.2.7/tvdcn/ops/activations/mask_sigmoid.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tvdcn/ops/activations/mask_softmax.py` & `tvdcn-0.2.7/tvdcn/ops/activations/mask_softmax.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tvdcn/ops/deform_conv.py` & `tvdcn-0.2.7/tvdcn/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.2.7/tvdcn/ops/deform_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tvdcn/utils.py` & `tvdcn-0.2.7/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.6/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.2.7/tvdcn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.6
+Version: 0.2.7
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
```

### Comparing `tvdcn-0.2.6/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.2.7/tvdcn.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE.txt
+MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
 tests/test_compatibility_with_torchvision.py
 tests/test_grad.py
 tvdcn/__init__.py
 tvdcn/_types.py
 tvdcn/_version.py
@@ -22,14 +24,17 @@
 tvdcn/csrc/ops/deform_conv3d.cpp
 tvdcn/csrc/ops/deform_conv_transpose1d.cpp
 tvdcn/csrc/ops/deform_conv_transpose2d.cpp
 tvdcn/csrc/ops/deform_conv_transpose3d.cpp
 tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
 tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
 tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
+tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
+tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
+tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
 tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
 tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
 tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
 tvdcn/ops/__init__.py
 tvdcn/ops/deform_conv.py
 tvdcn/ops/deform_conv_transpose.py
 tvdcn/ops/activations/__init__.py
```

