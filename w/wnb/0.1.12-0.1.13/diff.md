# Comparing `tmp/wnb-0.1.12.tar.gz` & `tmp/wnb-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnb-0.1.12.tar", last modified: Sat Jun  3 05:00:13 2023, max compression
+gzip compressed data, was "wnb-0.1.13.tar", last modified: Sun Jun  4 17:17:51 2023, max compression
```

## Comparing `wnb-0.1.12.tar` & `wnb-0.1.13.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:00:12.998049 wnb-0.1.12/
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-03 05:00:12.998049 wnb-0.1.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-03 05:00:03.000000 wnb-0.1.12/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 05:00:12.998049 wnb-0.1.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-03 05:00:03.000000 wnb-0.1.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:00:12.994049 wnb-0.1.12/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-03 05:00:03.000000 wnb-0.1.12/tests/test_gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-03 05:00:03.000000 wnb-0.1.12/tests/test_gwnb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:00:12.998049 wnb-0.1.12/wnb/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/gnb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-06-03 05:00:03.000000 wnb-0.1.12/wnb/gwnb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:00:12.998049 wnb-0.1.12/wnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-03 05:00:12.000000 wnb-0.1.12/wnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-03 05:00:12.000000 wnb-0.1.12/wnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 05:00:12.000000 wnb-0.1.12/wnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-03 05:00:12.000000 wnb-0.1.12/wnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-03 05:00:12.000000 wnb-0.1.12/wnb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:17:50.996507 wnb-0.1.13/
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-04 17:17:50.996507 wnb-0.1.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-04 17:17:39.000000 wnb-0.1.13/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 17:17:50.996507 wnb-0.1.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-04 17:17:39.000000 wnb-0.1.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:17:50.992507 wnb-0.1.13/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-04 17:17:39.000000 wnb-0.1.13/tests/test_gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-04 17:17:39.000000 wnb-0.1.13/tests/test_gwnb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:17:50.992507 wnb-0.1.13/wnb/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/gnb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14969 2023-06-04 17:17:39.000000 wnb-0.1.13/wnb/gwnb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 17:17:50.996507 wnb-0.1.13/wnb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-04 17:17:50.000000 wnb-0.1.13/wnb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-04 17:17:50.000000 wnb-0.1.13/wnb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 17:17:50.000000 wnb-0.1.13/wnb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-04 17:17:50.000000 wnb-0.1.13/wnb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-04 17:17:50.000000 wnb-0.1.13/wnb.egg-info/top_level.txt
```

### Comparing `wnb-0.1.12/PKG-INFO` & `wnb-0.1.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnb
-Version: 0.1.12
+Version: 0.1.13
 Summary: Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.
 Home-page: https://github.com/msamsami/weighted-naive-bayes
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,bayes,naivebayes,classifier,probabilistic
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.12-green)
+![](https://img.shields.io/badge/version-v0.1.13-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
 
 <p>
 <img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
 <br>
```

### Comparing `wnb-0.1.12/README.md` & `wnb-0.1.13/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.12-green)
+![](https://img.shields.io/badge/version-v0.1.13-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
 
 <p>
 <img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
 <br>
```

### Comparing `wnb-0.1.12/setup.py` & `wnb-0.1.13/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import codecs
 from os import path
 from setuptools import setup
 
 
 setup(
     name='wnb',
-    version='0.1.12',
+    version='0.1.13',
     description='Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.',
     keywords=['python', 'bayes', 'naivebayes', 'classifier', 'probabilistic'],
     author='Mehdi Samsami',
     author_email='mehdisamsami@live.com',
     url='https://github.com/msamsami/weighted-naive-bayes',
     long_description=codecs.open(path.join(path.abspath(path.dirname(__file__)), 'README.md'), encoding='utf-8').read(),
     long_description_content_type='text/markdown',
```

### Comparing `wnb-0.1.12/tests/test_gnb.py` & `wnb-0.1.13/tests/test_gnb.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.12/wnb/_base.py` & `wnb-0.1.13/wnb/_base.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.12/wnb/dist.py` & `wnb-0.1.13/wnb/dist.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.12/wnb/gnb.py` & `wnb-0.1.13/wnb/gnb.py`

 * *Files identical despite different names*

### Comparing `wnb-0.1.12/wnb/gwnb.py` & `wnb-0.1.13/wnb/gwnb.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,34 +19,39 @@
     """
     Binary Gaussian Minimum Log-likelihood Difference Weighted Naive Bayes (MLD-WNB) Classifier
     """
 
     def __init__(self, *,
                  priors: Optional[Union[Sequence[float], np.ndarray]] = None,
                  error_weights: Optional[np.ndarray] = None,
-                 max_iter: int = 25, step_size: float = 1e-4, penalty: str = 'l2', C: float = 1.0) -> None:
+                 max_iter: int = 25,
+                 step_size: float = 1e-4,
+                 penalty: str = 'l2',
+                 C: float = 1.0,
+                 learning_hist: bool = False) -> None:
         """Initializes an object of the class.
 
         Args:
             priors (Optional[Union[Sequence[float], np.ndarray]]): Prior probabilities. Defaults to None.
             error_weights (Optional[np.ndarray]): Matrix of error weights (n_classes * n_classes). Defaults to None.
             max_iter (int): Maximum number of gradient descent iterations. Defaults to 25.
             step_size (float): Step size of weight update (i.e., learning rate). Defaults to 1e-4.
             penalty (str): Regularization term; must be either 'l1' or 'l2'. Defaults to 'l2'.
             C (float): Regularization strength; must be a positive float. Defaults to 1.0.
+            learning_hist (bool): Whether to record the learning history, i.e., the value of cost function in each
+                                  learning iteration.
 
-        Returns:
-            self: The instance itself.
         """
         self.priors = priors  # Prior probabilities of classes (n_classes x 1)
         self.error_weights = error_weights  # Matrix of error weights (n_features x n_features)
         self.max_iter = max_iter  # Maximum number of iterations of the learning algorithm
         self.step_size = step_size  # Learning rate
         self.penalty = penalty  # Regularization type ('l1' or 'l2')
         self.C = C  # Regularization parameter
+        self.learning_hist = learning_hist
 
     def _more_tags(self):
         return {
             'binary_only': True,
             'requires_y': True
         }
 
@@ -165,25 +170,22 @@
 
         # Update if no error weights is provided
         if self.error_weights is None:
             self.error_weights_ = np.array([[0, 1], [-1, 0]])
         else:
             self.error_weights_ = self.error_weights
 
-    def fit(self, X: Union[np.ndarray, pd.DataFrame], y: Union[np.ndarray, pd.DataFrame, pd.Series],
-            learning_hist: bool = False):
+    def fit(self, X: Union[np.ndarray, pd.DataFrame], y: Union[np.ndarray, pd.DataFrame, pd.Series]):
         """Fits Gaussian Binary MLD-WNB according to X and y.
 
         Args:
             X (Union[np.ndarray, pd.DataFrame]): Array-like of shape (n_samples, n_features).
                                                  Training vectors, where `n_samples` is the number of samples
                                                  and `n_features` is the number of features.
             y (Union[np.ndarray, pd.DataFrame, pd.Series]): Array-like of shape (n_samples,). Target values.
-            learning_hist (bool): Whether to keep the learning history (i.e., the value of cost function in each
-                                  learning iteration)
 
         Returns:
             self: The instance itself.
         """
         X, y = self._prepare_X_y(X, y, from_fit=True)
 
         self.classes_, y_ = np.unique(y, return_inverse=True)  # Unique class labels and their indices
@@ -203,28 +205,30 @@
         # Learn the weights using gradient descent
         self.n_iter_ = 0
         for self.n_iter_ in range(self.max_iter):
             # Predict on X
             y_hat = self.__predict(X)
 
             # Calculate cost
-            self.cost_hist_[self.n_iter_], _lambda = self._calculate_cost(X, y, y_hat, learning_hist)
+            self.cost_hist_[self.n_iter_], _lambda = self._calculate_cost(X, y, y_hat, self.learning_hist)
 
             # Calculate gradients (most time-consuming)
             _grad = self._calculate_grad(X, _lambda)
 
             # Add regularization
             if self.penalty == 'l1':
                 _grad += self.C * np.sign(self.coef_)
             elif self.penalty == 'l2':
                 _grad += 2 * self.C * self.coef_
 
             # Update weights
             self.coef_ = self.coef_ - self.step_size * _grad
 
+        self.cost_hist_ = None if not self.learning_hist else self.cost_hist_
+
         return self
 
     def _calculate_cost(self, X, y, y_hat, learning_hist):
         _lambda = [self.error_weights_[y[i], y_hat[i]] for i in range(self.__n_samples)]
 
         if learning_hist:
             # Calculate cost
@@ -233,15 +237,15 @@
                 _sum = np.log(self.class_prior_[1] / self.class_prior_[0])
                 x = X[i, :]
                 for j in range(self.n_features_in_):
                     _sum += self.coef_[j] * (np.log(1e-20 + norm.pdf(x[j], self.mu_[j, 1], self.std_[j, 1]))
                                              - np.log(1e-20 + norm.pdf(x[j], self.mu_[j, 0], self.std_[j, 0])))
                 _cost += _lambda[i] * _sum
         else:
-            _cost = None
+            _cost = np.nan
 
         return _cost, _lambda
 
     def _calculate_grad(self, X, _lambda):
         _grad = np.repeat(np.log(self.std_[:, 0] / self.std_[:, 1]).reshape(1, -1), self.__n_samples, axis=0)
         _grad += 0.5 * ((X - np.repeat(self.mu_[:, 0].reshape(1, -1), self.__n_samples, axis=0)) /
                         (np.repeat(self.std_[:, 0].reshape(1, -1), self.__n_samples, axis=0))) ** 2
@@ -311,17 +315,17 @@
         n_samples = X.shape[0]
 
         X = self._prepare_X_y(X=X)
 
         log_priors = np.tile(np.log(self.class_prior_), (n_samples, 1))
         w_reshaped = np.tile(self.coef_.reshape(-1, 1), (1, self.n_classes_))
         term1 = np.sum(np.multiply(w_reshaped, -np.log(np.sqrt(2 * np.pi) * self.std_)))
-        var_inv = np.multiply(w_reshaped, 1/np.multiply(self.std_, self.std_))
+        var_inv = np.multiply(w_reshaped, 1.0/np.multiply(self.std_, self.std_))
         mu_by_var = np.multiply(self.mu_, var_inv)
-        term2 = -0.5*(np.matmul(np.multiply(X, X), var_inv) - 2*np.matmul(X, mu_by_var)
+        term2 = -0.5*(np.matmul(np.multiply(X, X), var_inv) - 2.0*np.matmul(X, mu_by_var)
                       + np.sum(self.mu_.conj()*mu_by_var, axis=0))
         log_proba = log_priors + term1 + term2
 
         log_proba -= np.transpose(np.repeat(logsumexp(log_proba, axis=1).reshape(1, -1), self.n_classes_, axis=0))
         return log_proba
 
     def predict_proba(self, X: Union[np.ndarray, pd.DataFrame]) -> np.ndarray:
```

### Comparing `wnb-0.1.12/wnb.egg-info/PKG-INFO` & `wnb-0.1.13/wnb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnb
-Version: 0.1.12
+Version: 0.1.13
 Summary: Python library for the implementations of general and weighted naive Bayes (WNB) classifiers.
 Home-page: https://github.com/msamsami/weighted-naive-bayes
 Author: Mehdi Samsami
 Author-email: mehdisamsami@live.com
 Keywords: python,bayes,naivebayes,classifier,probabilistic
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # WNB: General and weighted naive Bayes classifiers
 
-![](https://img.shields.io/badge/version-v0.1.12-green)
+![](https://img.shields.io/badge/version-v0.1.13-green)
 ![](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue)
 ![](https://github.com/msamsami/weighted-naive-bayes/actions/workflows/python-publish.yml/badge.svg)
 [![](https://img.shields.io/pypi/v/wnb)](https://pypi.org/project/wnb/)
 
 <p>
 <img src="https://raw.githubusercontent.com/msamsami/weighted-naive-bayes/main/logo.png" alt="wnb logo" width="275" />
 <br>
```

