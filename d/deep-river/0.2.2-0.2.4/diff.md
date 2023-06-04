# Comparing `tmp/deep_river-0.2.2.tar.gz` & `tmp/deep_river-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_river-0.2.2.tar", last modified: Wed Mar  1 12:46:30 2023, max compression
+gzip compressed data, was "deep_river-0.2.4.tar", last modified: Sun Jun  4 20:35:29 2023, max compression
```

## Comparing `deep_river-0.2.2.tar` & `deep_river-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:46:30.383139 deep_river-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-01 12:46:17.000000 deep_river-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-03-01 12:46:30.383139 deep_river-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-03-01 12:46:17.000000 deep_river-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:46:30.379140 deep_river-0.2.2/deep_river/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:46:30.379140 deep_river-0.2.2/deep_river/anomaly/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/anomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/anomaly/ae.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/anomaly/probability_weighted_ae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/anomaly/rolling_ae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/anomaly/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:46:30.379140 deep_river-0.2.2/deep_river/classification/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/classification/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    23003 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/classification/rolling_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/classification/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:46:30.379140 deep_river-0.2.2/deep_river/regression/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/regression/multioutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/regression/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/regression/rolling_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/regression/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:46:30.383139 deep_river-0.2.2/deep_river/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/utils/estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/utils/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/utils/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/utils/tensor_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/utils/test_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-03-01 12:46:17.000000 deep_river-0.2.2/deep_river/utils/test_tensor_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 12:46:30.379140 deep_river-0.2.2/deep_river.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-03-01 12:46:30.000000 deep_river-0.2.2/deep_river.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-01 12:46:30.000000 deep_river-0.2.2/deep_river.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 12:46:30.000000 deep_river-0.2.2/deep_river.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-03-01 12:46:30.000000 deep_river-0.2.2/deep_river.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-01 12:46:30.000000 deep_river-0.2.2/deep_river.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-01 12:46:17.000000 deep_river-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-01 12:46:30.383139 deep_river-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-03-01 12:46:17.000000 deep_river-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:35:29.506970 deep_river-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-04 20:35:11.000000 deep_river-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-04 20:35:29.506970 deep_river-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-04 20:35:11.000000 deep_river-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:35:29.502970 deep_river-0.2.4/deep_river/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:35:29.502970 deep_river-0.2.4/deep_river/anomaly/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/anomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/anomaly/ae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/anomaly/probability_weighted_ae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/anomaly/rolling_ae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/anomaly/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:35:29.502970 deep_river-0.2.4/deep_river/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/classification/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23003 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/classification/rolling_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/classification/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:35:29.506970 deep_river-0.2.4/deep_river/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/regression/multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/regression/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/regression/rolling_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/regression/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:35:29.506970 deep_river-0.2.4/deep_river/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/utils/estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/utils/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/utils/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/utils/tensor_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/utils/test_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-04 20:35:11.000000 deep_river-0.2.4/deep_river/utils/test_tensor_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:35:29.502970 deep_river-0.2.4/deep_river.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-04 20:35:29.000000 deep_river-0.2.4/deep_river.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-04 20:35:29.000000 deep_river-0.2.4/deep_river.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:35:29.000000 deep_river-0.2.4/deep_river.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-04 20:35:29.000000 deep_river-0.2.4/deep_river.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 20:35:29.000000 deep_river-0.2.4/deep_river.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-04 20:35:11.000000 deep_river-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-04 20:35:29.506970 deep_river-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-04 20:35:11.000000 deep_river-0.2.4/setup.py
```

### Comparing `deep_river-0.2.2/LICENSE` & `deep_river-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/PKG-INFO` & `deep_river-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep_river
-Version: 0.2.2
+Version: 0.2.4
 Summary: Online Deep Learning for river
 Home-page: https://online-ml.github.io/deep-river/
 Author: Cedric Kulbach
 Author-email: cedric.kulbach@googlemail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `deep_river-0.2.2/README.md` & `deep_river-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/anomaly/ae.py` & `deep_river-0.2.4/deep_river/anomaly/ae.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/anomaly/probability_weighted_ae.py` & `deep_river-0.2.4/deep_river/anomaly/probability_weighted_ae.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/anomaly/rolling_ae.py` & `deep_river-0.2.4/deep_river/anomaly/rolling_ae.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/anomaly/scaler.py` & `deep_river-0.2.4/deep_river/anomaly/scaler.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/base.py` & `deep_river-0.2.4/deep_river/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         -------
         DeepEstimator
             The cloned estimator.
         """
         new_params = new_params or {}
         new_params.update(self.kwargs)
         new_params.update(self._get_params())
+        new_params.update({"module": self.module_cls})
 
         clone = self.__class__(**new_params)
         if include_attributes:
             clone.__dict__.update(self.__dict__)
         return clone
```

### Comparing `deep_river-0.2.2/deep_river/classification/classifier.py` & `deep_river-0.2.4/deep_river/classification/classifier.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/classification/rolling_classifier.py` & `deep_river-0.2.4/deep_river/classification/rolling_classifier.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/classification/zoo.py` & `deep_river-0.2.4/deep_river/classification/zoo.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,16 @@
         lr: float = 1e-3,
         output_is_logit: bool = True,
         is_class_incremental: bool = False,
         device: str = "cpu",
         seed: int = 42,
         **kwargs,
     ):
+        if "module" in kwargs:
+            del kwargs["module"]
         super().__init__(
             module=LogisticRegression.LRModule,
             loss_fn=loss_fn,
             output_is_logit=output_is_logit,
             is_class_incremental=is_class_incremental,
             optimizer_fn=optimizer_fn,
             device=device,
@@ -213,14 +215,16 @@
         is_class_incremental: bool = False,
         device: str = "cpu",
         seed: int = 42,
         **kwargs,
     ):
         self.n_width = n_width
         self.n_layers = n_layers
+        if "module" in kwargs:
+            del kwargs["module"]
         super().__init__(
             module=MultiLayerPerceptron.MLPModule,
             loss_fn=loss_fn,
             output_is_logit=output_is_logit,
             is_class_incremental=is_class_incremental,
             optimizer_fn=optimizer_fn,
             device=device,
```

### Comparing `deep_river-0.2.2/deep_river/regression/multioutput.py` & `deep_river-0.2.4/deep_river/regression/multioutput.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/regression/regressor.py` & `deep_river-0.2.4/deep_river/regression/regressor.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/regression/rolling_regressor.py` & `deep_river-0.2.4/deep_river/regression/rolling_regressor.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/regression/zoo.py` & `deep_river-0.2.4/deep_river/regression/zoo.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 from deep_river.regression import Regressor
 
 
 class LinearRegression(Regressor):
     """
     This class implements a linear regression model in PyTorch.
 
-    Parameters
-    ----------
-
     """
 
     class LRModule(nn.Module):
         def __init__(self, n_features):
             super().__init__()
             self.dense0 = nn.Linear(n_features, 1)
 
@@ -28,14 +25,16 @@
         loss_fn: Union[str, Callable] = "mse",
         optimizer_fn: Union[str, Callable] = "sgd",
         lr: float = 1e-3,
         device: str = "cpu",
         seed: int = 42,
         **kwargs,
     ):
+        if "module" in kwargs:
+            del kwargs["module"]
         super().__init__(
             module=LinearRegression.LRModule,
             loss_fn=loss_fn,
             optimizer_fn=optimizer_fn,
             lr=lr,
             device=device,
             seed=seed,
@@ -126,14 +125,16 @@
         lr: float = 1e-3,
         device: str = "cpu",
         seed: int = 42,
         **kwargs,
     ):
         self.n_width = n_width
         self.n_layers = n_layers
+        if "module" in kwargs:
+            del kwargs["module"]
         super().__init__(
             module=MultiLayerPerceptron.MLPModule,
             loss_fn=loss_fn,
             optimizer_fn=optimizer_fn,
             lr=lr,
             device=device,
             seed=seed,
```

### Comparing `deep_river-0.2.2/deep_river/utils/__init__.py` & `deep_river-0.2.4/deep_river/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/utils/estimator_checks.py` & `deep_river-0.2.4/deep_river/utils/estimator_checks.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/utils/hooks.py` & `deep_river-0.2.4/deep_river/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/utils/params.py` & `deep_river-0.2.4/deep_river/utils/params.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/utils/tensor_conversion.py` & `deep_river-0.2.4/deep_river/utils/tensor_conversion.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/utils/test_estimators.py` & `deep_river-0.2.4/deep_river/utils/test_estimators.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river/utils/test_tensor_conversion.py` & `deep_river-0.2.4/deep_river/utils/test_tensor_conversion.py`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river.egg-info/PKG-INFO` & `deep_river-0.2.4/deep_river.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-river
-Version: 0.2.2
+Version: 0.2.4
 Summary: Online Deep Learning for river
 Home-page: https://online-ml.github.io/deep-river/
 Author: Cedric Kulbach
 Author-email: cedric.kulbach@googlemail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `deep_river-0.2.2/deep_river.egg-info/SOURCES.txt` & `deep_river-0.2.4/deep_river.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/deep_river.egg-info/requires.txt` & `deep_river-0.2.4/deep_river.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 scikit-learn~=1.0.2
 torch~=1.13.0
 pandas~=1.3.2
 numpy~=1.24.0
-river~=0.15.0
+river~=0.17.0
 tqdm~=4.61.2
 ordered-set~=4.1.0
 torchviz~=0.0.2
 
 [:python_version == '3.6']
 dataclasses
 
@@ -47,15 +47,15 @@
 watermark==2.3.1
 
 [dev]
 scikit-learn~=1.0.2
 torch~=1.13.0
 pandas~=1.3.2
 numpy~=1.24.0
-river~=0.15.0
+river~=0.17.0
 tqdm~=4.61.2
 ordered-set~=4.1.0
 torchviz~=0.0.2
 graphviz>=0.10.1
 matplotlib>=3.0.2
 mypy>=0.990
 pre-commit>=2.20.0
@@ -69,15 +69,15 @@
 pyupgrade==3.2.0
 
 [docs]
 scikit-learn~=1.0.2
 torch~=1.13.0
 pandas~=1.3.2
 numpy~=1.24.0
-river~=0.15.0
+river~=0.17.0
 tqdm~=4.61.2
 ordered-set~=4.1.0
 torchviz~=0.0.2
 flask>=2.0.2
 ipykernel>=6.9.0
 mike>=0.5.3
 mkdocs>=1.2.3
```

### Comparing `deep_river-0.2.2/pyproject.toml` & `deep_river-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deep_river-0.2.2/setup.py` & `deep_river-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # Package requirements.
 base_packages = [
     "scikit-learn~=1.0.2",
     "torch~=1.13.0",
     "pandas~=1.3.2",
     "numpy~=1.24.0",
-    "river~=0.15.0",
+    "river~=0.17.0",
     "tqdm~=4.61.2",
     "ordered-set~=4.1.0",
     "torchviz~=0.0.2",
 ]
 
 dev_packages = [
     "graphviz>=0.10.1",
```

