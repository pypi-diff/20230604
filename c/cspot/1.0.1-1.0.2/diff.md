# Comparing `tmp/cspot-1.0.1.tar.gz` & `tmp/cspot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cspot-1.0.1.tar", max compression
+gzip compressed data, was "cspot-1.0.2.tar", max compression
```

## Comparing `cspot-1.0.1.tar` & `cspot-1.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      113 2023-06-02 23:46:02.832679 cspot-1.0.1/README.md
--rw-r--r--   0        0        0     8196 2023-06-03 14:50:07.931359 cspot-1.0.1/cspot/.DS_Store
--rw-r--r--   0        0        0    32012 2023-03-20 20:58:58.000000 cspot-1.0.1/cspot/UNet.py
--rw-r--r--   0        0        0      567 2023-06-03 00:49:31.038091 cspot-1.0.1/cspot/__init__.py
--rw-r--r--   0        0        0     6483 2023-06-03 13:49:11.927037 cspot-1.0.1/cspot/addPredictions.py
--rw-r--r--   0        0        0    30831 2023-02-04 00:24:05.000000 cspot-1.0.1/cspot/archives/UNet-02032023.py
--rw-r--r--   0        0        0    35278 2023-01-27 16:37:48.000000 cspot-1.0.1/cspot/archives/gator-01272023.py
--rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.1/cspot/archives/toolbox-02032023/GPUselect.py
--rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.1/cspot/archives/toolbox-02032023/PartitionOfImage.py
--rw-r--r--   0        0        0     6075 2023-02-03 20:50:23.000000 cspot-1.0.1/cspot/archives/toolbox-02032023/PartitionOfImageOM.py
--rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.1/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc
--rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.1/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc
--rw-r--r--   0        0        0     2062 2023-02-04 00:05:31.000000 cspot-1.0.1/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc
--rw-r--r--   0        0        0     9960 2023-02-04 00:25:40.000000 cspot-1.0.1/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc
--rw-r--r--   0        0        0     1408 2023-02-03 20:50:23.000000 cspot-1.0.1/cspot/archives/toolbox-02032023/ftools.py
--rw-r--r--   0        0        0    10892 2023-02-04 00:25:24.000000 cspot-1.0.1/cspot/archives/toolbox-02032023/imtools.py
--rw-r--r--   0        0        0     7197 2023-02-03 20:50:23.000000 cspot-1.0.1/cspot/archives/toolbox-02032023/toolbox.py
--rw-r--r--   0        0        0     9954 2023-06-03 13:53:25.094742 cspot-1.0.1/cspot/cloneFolder.py
--rw-r--r--   0        0        0     5420 2023-06-03 01:28:24.250314 cspot-1.0.1/cspot/csExport.py
--rw-r--r--   0        0        0    12110 2023-06-03 01:50:07.683172 cspot-1.0.1/cspot/csObject.py
--rw-r--r--   0        0        0    21396 2023-06-03 02:07:36.877319 cspot-1.0.1/cspot/csPhenotype.py
--rw-r--r--   0        0        0    17767 2023-06-03 02:32:44.390726 cspot-1.0.1/cspot/csPipeline.py
--rw-r--r--   0        0        0    12652 2023-06-03 13:23:44.969631 cspot-1.0.1/cspot/csPredict.py
--rw-r--r--   0        0        0    11509 2023-06-03 13:27:56.675075 cspot-1.0.1/cspot/csTrain.py
--rw-r--r--   0        0        0    41321 2023-06-03 01:15:15.512879 cspot-1.0.1/cspot/cspot.py
--rw-r--r--   0        0        0     7177 2023-06-03 13:31:27.913454 cspot-1.0.1/cspot/generateCSScore.py
--rw-r--r--   0        0        0    26610 2023-06-03 13:55:51.499930 cspot-1.0.1/cspot/generateThumbnails.py
--rw-r--r--   0        0        0    13537 2023-06-03 13:57:51.583210 cspot-1.0.1/cspot/generateTrainTestSplit.py
--rw-r--r--   0        0        0     8597 2023-06-03 13:41:53.258604 cspot-1.0.1/cspot/mergecsObject.py
--rw-r--r--   0        0        0    10197 2023-06-03 14:02:48.939048 cspot-1.0.1/cspot/scatterPlot.py
--rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.1/cspot/toolbox/GPUselect.py
--rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.1/cspot/toolbox/PartitionOfImage.py
--rw-r--r--   0        0        0      196 2023-03-10 02:36:16.000000 cspot-1.0.1/cspot/toolbox/__init__.py
--rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.1/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc
--rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.1/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc
--rw-r--r--   0        0        0      477 2023-03-10 02:39:18.000000 cspot-1.0.1/cspot/toolbox/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      711 2023-02-04 00:52:32.000000 cspot-1.0.1/cspot/toolbox/__pycache__/ftools.cpython-39.pyc
--rw-r--r--   0        0        0     1017 2023-02-04 00:52:32.000000 cspot-1.0.1/cspot/toolbox/__pycache__/imtools.cpython-39.pyc
--rw-r--r--   0        0        0      361 2023-02-04 00:50:12.000000 cspot-1.0.1/cspot/toolbox/ftools.py
--rw-r--r--   0        0        0      671 2023-02-04 00:46:01.000000 cspot-1.0.1/cspot/toolbox/imtools.py
--rw-r--r--   0        0        0     1164 2023-06-03 22:05:01.184803 cspot-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 cspot-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-06-02 23:46:02.832679 cspot-1.0.2/README.md
+-rw-r--r--   0        0        0     8196 2023-06-03 14:50:07.931359 cspot-1.0.2/cspot/.DS_Store
+-rw-r--r--   0        0        0    32012 2023-03-20 20:58:58.000000 cspot-1.0.2/cspot/UNet.py
+-rw-r--r--   0        0        0      567 2023-06-03 00:49:31.038091 cspot-1.0.2/cspot/__init__.py
+-rw-r--r--   0        0        0     6483 2023-06-03 13:49:11.927037 cspot-1.0.2/cspot/addPredictions.py
+-rw-r--r--   0        0        0    30831 2023-02-04 00:24:05.000000 cspot-1.0.2/cspot/archives/UNet-02032023.py
+-rw-r--r--   0        0        0    35278 2023-01-27 16:37:48.000000 cspot-1.0.2/cspot/archives/gator-01272023.py
+-rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.2/cspot/archives/toolbox-02032023/GPUselect.py
+-rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.2/cspot/archives/toolbox-02032023/PartitionOfImage.py
+-rw-r--r--   0        0        0     6075 2023-02-03 20:50:23.000000 cspot-1.0.2/cspot/archives/toolbox-02032023/PartitionOfImageOM.py
+-rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.2/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc
+-rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.2/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc
+-rw-r--r--   0        0        0     2062 2023-02-04 00:05:31.000000 cspot-1.0.2/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc
+-rw-r--r--   0        0        0     9960 2023-02-04 00:25:40.000000 cspot-1.0.2/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc
+-rw-r--r--   0        0        0     1408 2023-02-03 20:50:23.000000 cspot-1.0.2/cspot/archives/toolbox-02032023/ftools.py
+-rw-r--r--   0        0        0    10892 2023-02-04 00:25:24.000000 cspot-1.0.2/cspot/archives/toolbox-02032023/imtools.py
+-rw-r--r--   0        0        0     7197 2023-02-03 20:50:23.000000 cspot-1.0.2/cspot/archives/toolbox-02032023/toolbox.py
+-rw-r--r--   0        0        0     9954 2023-06-03 13:53:25.094742 cspot-1.0.2/cspot/cloneFolder.py
+-rw-r--r--   0        0        0     5420 2023-06-03 01:28:24.250314 cspot-1.0.2/cspot/csExport.py
+-rw-r--r--   0        0        0    12110 2023-06-03 01:50:07.683172 cspot-1.0.2/cspot/csObject.py
+-rw-r--r--   0        0        0    21396 2023-06-03 02:07:36.877319 cspot-1.0.2/cspot/csPhenotype.py
+-rw-r--r--   0        0        0    17767 2023-06-03 02:32:44.390726 cspot-1.0.2/cspot/csPipeline.py
+-rw-r--r--   0        0        0    12652 2023-06-03 13:23:44.969631 cspot-1.0.2/cspot/csPredict.py
+-rw-r--r--   0        0        0    11509 2023-06-03 13:27:56.675075 cspot-1.0.2/cspot/csTrain.py
+-rw-r--r--   0        0        0    41321 2023-06-03 01:15:15.512879 cspot-1.0.2/cspot/cspot.py
+-rw-r--r--   0        0        0     7177 2023-06-03 13:31:27.913454 cspot-1.0.2/cspot/generateCSScore.py
+-rw-r--r--   0        0        0    26610 2023-06-03 13:55:51.499930 cspot-1.0.2/cspot/generateThumbnails.py
+-rw-r--r--   0        0        0    13537 2023-06-03 13:57:51.583210 cspot-1.0.2/cspot/generateTrainTestSplit.py
+-rw-r--r--   0        0        0     8597 2023-06-03 13:41:53.258604 cspot-1.0.2/cspot/mergecsObject.py
+-rw-r--r--   0        0        0    10197 2023-06-03 14:02:48.939048 cspot-1.0.2/cspot/scatterPlot.py
+-rw-r--r--   0        0        0      727 2023-02-03 20:50:23.000000 cspot-1.0.2/cspot/toolbox/GPUselect.py
+-rw-r--r--   0        0        0    10105 2023-02-04 00:04:35.000000 cspot-1.0.2/cspot/toolbox/PartitionOfImage.py
+-rw-r--r--   0        0        0      196 2023-03-10 02:36:16.000000 cspot-1.0.2/cspot/toolbox/__init__.py
+-rw-r--r--   0        0        0      804 2023-02-04 00:05:31.000000 cspot-1.0.2/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc
+-rw-r--r--   0        0        0     7854 2023-02-04 00:05:31.000000 cspot-1.0.2/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc
+-rw-r--r--   0        0        0      477 2023-03-10 02:39:18.000000 cspot-1.0.2/cspot/toolbox/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      711 2023-02-04 00:52:32.000000 cspot-1.0.2/cspot/toolbox/__pycache__/ftools.cpython-39.pyc
+-rw-r--r--   0        0        0     1017 2023-02-04 00:52:32.000000 cspot-1.0.2/cspot/toolbox/__pycache__/imtools.cpython-39.pyc
+-rw-r--r--   0        0        0      361 2023-02-04 00:50:12.000000 cspot-1.0.2/cspot/toolbox/ftools.py
+-rw-r--r--   0        0        0      671 2023-02-04 00:46:01.000000 cspot-1.0.2/cspot/toolbox/imtools.py
+-rw-r--r--   0        0        0     1165 2023-06-03 22:07:27.183289 cspot-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 cspot-1.0.2/PKG-INFO
```

### Comparing `cspot-1.0.1/cspot/.DS_Store` & `cspot-1.0.2/cspot/.DS_Store`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/UNet.py` & `cspot-1.0.2/cspot/UNet.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/__init__.py` & `cspot-1.0.2/cspot/__init__.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/addPredictions.py` & `cspot-1.0.2/cspot/addPredictions.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/UNet-02032023.py` & `cspot-1.0.2/cspot/archives/UNet-02032023.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/gator-01272023.py` & `cspot-1.0.2/cspot/archives/gator-01272023.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/toolbox-02032023/GPUselect.py` & `cspot-1.0.2/cspot/archives/toolbox-02032023/GPUselect.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/toolbox-02032023/PartitionOfImage.py` & `cspot-1.0.2/cspot/archives/toolbox-02032023/PartitionOfImage.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/toolbox-02032023/PartitionOfImageOM.py` & `cspot-1.0.2/cspot/archives/toolbox-02032023/PartitionOfImageOM.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc` & `cspot-1.0.2/cspot/archives/toolbox-02032023/__pycache__/GPUselect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc` & `cspot-1.0.2/cspot/archives/toolbox-02032023/__pycache__/PartitionOfImage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc` & `cspot-1.0.2/cspot/archives/toolbox-02032023/__pycache__/ftools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc` & `cspot-1.0.2/cspot/archives/toolbox-02032023/__pycache__/imtools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/toolbox-02032023/ftools.py` & `cspot-1.0.2/cspot/archives/toolbox-02032023/ftools.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/toolbox-02032023/imtools.py` & `cspot-1.0.2/cspot/archives/toolbox-02032023/imtools.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/archives/toolbox-02032023/toolbox.py` & `cspot-1.0.2/cspot/archives/toolbox-02032023/toolbox.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/cloneFolder.py` & `cspot-1.0.2/cspot/cloneFolder.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/csExport.py` & `cspot-1.0.2/cspot/csExport.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/csObject.py` & `cspot-1.0.2/cspot/csObject.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/csPhenotype.py` & `cspot-1.0.2/cspot/csPhenotype.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/csPipeline.py` & `cspot-1.0.2/cspot/csPipeline.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/csPredict.py` & `cspot-1.0.2/cspot/csPredict.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/csTrain.py` & `cspot-1.0.2/cspot/csTrain.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/cspot.py` & `cspot-1.0.2/cspot/cspot.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/generateCSScore.py` & `cspot-1.0.2/cspot/generateCSScore.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/generateThumbnails.py` & `cspot-1.0.2/cspot/generateThumbnails.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/generateTrainTestSplit.py` & `cspot-1.0.2/cspot/generateTrainTestSplit.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/mergecsObject.py` & `cspot-1.0.2/cspot/mergecsObject.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/scatterPlot.py` & `cspot-1.0.2/cspot/scatterPlot.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/toolbox/GPUselect.py` & `cspot-1.0.2/cspot/toolbox/GPUselect.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/toolbox/PartitionOfImage.py` & `cspot-1.0.2/cspot/toolbox/PartitionOfImage.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc` & `cspot-1.0.2/cspot/toolbox/__pycache__/GPUselect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc` & `cspot-1.0.2/cspot/toolbox/__pycache__/PartitionOfImage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/toolbox/__pycache__/ftools.cpython-39.pyc` & `cspot-1.0.2/cspot/toolbox/__pycache__/ftools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/toolbox/__pycache__/imtools.cpython-39.pyc` & `cspot-1.0.2/cspot/toolbox/__pycache__/imtools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/cspot/toolbox/imtools.py` & `cspot-1.0.2/cspot/toolbox/imtools.py`

 * *Files identical despite different names*

### Comparing `cspot-1.0.1/pyproject.toml` & `cspot-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cspot"
-version = "1.0.1"
+version = "1.0.2"
 description = "CELL SPOTTER (CSPOT): A scalable framework for automated processing of highly multiplexed tissue images"
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 readme = "README.md"
 
 keywords = ["image analysis","multiplex imaging","single cell analysis"]
 
 homepage = "https://pypi.org/project/cspot/"
@@ -24,15 +24,15 @@
 python = ">=3.8,<3.12"
 numpy = "^1.23.2"
 pandas = "^1.4.4"
 tifffile = "^2022.8.12"
 pathlib = "^1.0.1"
 dask = "^2022.8.1"
 zarr = "^2.12.0"
-tensorflow = "^2.12.0"
+tensorflow = "<=2.12.0"
 opencv-python = "^4.6.0.66"
 anndata = "^0.8.0"
 scikit-learn = "^1.2.1"
 argparse = "^1.4.0"
 scikit-image = "^0.19.3"
 Brotli = "^1.0.9"
 matplotlib = "^3.7.1"
```

### Comparing `cspot-1.0.1/PKG-INFO` & `cspot-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cspot
-Version: 1.0.1
+Version: 1.0.2
 Summary: CELL SPOTTER (CSPOT): A scalable framework for automated processing of highly multiplexed tissue images
 Home-page: https://pypi.org/project/cspot/
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
-Requires-Dist: tensorflow (>=2.12.0,<3.0.0)
+Requires-Dist: tensorflow (<=2.12.0)
 Requires-Dist: tifffile (>=2022.8.12,<2023.0.0)
 Requires-Dist: zarr (>=2.12.0,<3.0.0)
 Project-URL: Documentation, https://nirmallab.github.io/cspot/
 Project-URL: Repository, https://github.com/nirmallab/cspot
 Description-Content-Type: text/markdown
 
 # cspot
```

