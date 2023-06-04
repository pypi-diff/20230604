# Comparing `tmp/probayes-0.0.5.tar.gz` & `tmp/probayes-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/probayes-0.0.5.tar", last modified: Sun Jun  4 10:53:06 2023, max compression
+gzip compressed data, was "dist/probayes-0.0.6.tar", last modified: Sun Jun  4 11:06:10 2023, max compression
```

## Comparing `probayes-0.0.5.tar` & `probayes-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 10:53:06.000000 probayes-0.0.5/
--rwxrwxrwx   0 root         (0) root         (0)     1952 2023-06-04 10:53:06.000000 probayes-0.0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1443 2023-02-19 15:32:03.000000 probayes-0.0.5/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 10:53:06.000000 probayes-0.0.5/probayes/
--rwxrwxrwx   0 root         (0) root         (0)     1152 2023-06-04 10:46:39.000000 probayes-0.0.5/probayes/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8183 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/cf.py
--rwxrwxrwx   0 root         (0) root         (0)     2649 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/cond_cov.py
--rwxrwxrwx   0 root         (0) root         (0)     1308 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/constants.py
--rwxrwxrwx   0 root         (0) root         (0)    17024 2023-06-03 17:23:46.000000 probayes-0.0.5/probayes/dependence.py
--rwxrwxrwx   0 root         (0) root         (0)    10720 2023-06-04 09:44:48.000000 probayes-0.0.5/probayes/distribution.py
--rwxrwxrwx   0 root         (0) root         (0)    11752 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/expr.py
--rwxrwxrwx   0 root         (0) root         (0)    17772 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/expression.py
--rwxrwxrwx   0 root         (0) root         (0)    24783 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/field.py
--rwxrwxrwx   0 root         (0) root         (0)    13044 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/func.py
--rwxrwxrwx   0 root         (0) root         (0)     6946 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/functional.py
--rwxrwxrwx   0 root         (0) root         (0)     1945 2023-06-03 17:23:46.000000 probayes-0.0.5/probayes/functional_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     3708 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/icon.py
--rwxrwxrwx   0 root         (0) root         (0)     3871 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/likelihoods.py
--rwxrwxrwx   0 root         (0) root         (0)     1058 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/named_dict.py
--rwxrwxrwx   0 root         (0) root         (0)     3318 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/ops.py
--rwxrwxrwx   0 root         (0) root         (0)    26417 2023-06-04 08:59:54.000000 probayes-0.0.5/probayes/pd.py
--rwxrwxrwx   0 root         (0) root         (0)    21453 2023-06-04 10:35:20.000000 probayes-0.0.5/probayes/pd_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    16636 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/prob.py
--rwxrwxrwx   0 root         (0) root         (0)     8398 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/pscales.py
--rwxrwxrwx   0 root         (0) root         (0)    25737 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/rf.py
--rwxrwxrwx   0 root         (0) root         (0)     6216 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/rf_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    24110 2023-06-03 17:23:46.000000 probayes-0.0.5/probayes/rv.py
--rwxrwxrwx   0 root         (0) root         (0)     4207 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/rv_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    11573 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/sd.py
--rwxrwxrwx   0 root         (0) root         (0)     1975 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/sd_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    10831 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/sp.py
--rwxrwxrwx   0 root         (0) root         (0)     3467 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/sp_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     7409 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/sympy_prob.py
--rwxrwxrwx   0 root         (0) root         (0)    29277 2023-06-03 17:23:46.000000 probayes-0.0.5/probayes/variable.py
--rwxrwxrwx   0 root         (0) root         (0)     2088 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/variable_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     6771 2023-02-19 15:32:03.000000 probayes-0.0.5/probayes/vtypes.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 10:53:06.000000 probayes-0.0.5/probayes.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1952 2023-06-04 10:53:05.000000 probayes-0.0.5/probayes.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      828 2023-06-04 10:53:05.000000 probayes-0.0.5/probayes.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-04 10:53:05.000000 probayes-0.0.5/probayes.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       59 2023-06-04 10:53:05.000000 probayes-0.0.5/probayes.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2023-06-04 10:53:05.000000 probayes-0.0.5/probayes.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      437 2023-06-04 10:53:06.000000 probayes-0.0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)       89 2023-02-19 15:32:03.000000 probayes-0.0.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 11:06:10.000000 probayes-0.0.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1952 2023-06-04 11:06:10.000000 probayes-0.0.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1443 2023-02-19 15:32:03.000000 probayes-0.0.6/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 11:06:10.000000 probayes-0.0.6/probayes/
+-rwxrwxrwx   0 root         (0) root         (0)     1152 2023-06-04 11:05:38.000000 probayes-0.0.6/probayes/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8183 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/cf.py
+-rwxrwxrwx   0 root         (0) root         (0)     2649 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/cond_cov.py
+-rwxrwxrwx   0 root         (0) root         (0)     1308 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/constants.py
+-rwxrwxrwx   0 root         (0) root         (0)    17024 2023-06-03 17:23:46.000000 probayes-0.0.6/probayes/dependence.py
+-rwxrwxrwx   0 root         (0) root         (0)    10720 2023-06-04 09:44:48.000000 probayes-0.0.6/probayes/distribution.py
+-rwxrwxrwx   0 root         (0) root         (0)    11752 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/expr.py
+-rwxrwxrwx   0 root         (0) root         (0)    17772 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/expression.py
+-rwxrwxrwx   0 root         (0) root         (0)    24783 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/field.py
+-rwxrwxrwx   0 root         (0) root         (0)    13044 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/func.py
+-rwxrwxrwx   0 root         (0) root         (0)     6946 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/functional.py
+-rwxrwxrwx   0 root         (0) root         (0)     1945 2023-06-03 17:23:46.000000 probayes-0.0.6/probayes/functional_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     3708 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/icon.py
+-rwxrwxrwx   0 root         (0) root         (0)     3871 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/likelihoods.py
+-rwxrwxrwx   0 root         (0) root         (0)     1058 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/named_dict.py
+-rwxrwxrwx   0 root         (0) root         (0)     3318 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/ops.py
+-rwxrwxrwx   0 root         (0) root         (0)    26417 2023-06-04 08:59:54.000000 probayes-0.0.6/probayes/pd.py
+-rwxrwxrwx   0 root         (0) root         (0)    21451 2023-06-04 11:01:13.000000 probayes-0.0.6/probayes/pd_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    16636 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/prob.py
+-rwxrwxrwx   0 root         (0) root         (0)     8398 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/pscales.py
+-rwxrwxrwx   0 root         (0) root         (0)    25737 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/rf.py
+-rwxrwxrwx   0 root         (0) root         (0)     6216 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/rf_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    24110 2023-06-03 17:23:46.000000 probayes-0.0.6/probayes/rv.py
+-rwxrwxrwx   0 root         (0) root         (0)     4207 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/rv_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    11573 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/sd.py
+-rwxrwxrwx   0 root         (0) root         (0)     1975 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/sd_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    10831 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/sp.py
+-rwxrwxrwx   0 root         (0) root         (0)     3467 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/sp_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     7409 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/sympy_prob.py
+-rwxrwxrwx   0 root         (0) root         (0)    29277 2023-06-03 17:23:46.000000 probayes-0.0.6/probayes/variable.py
+-rwxrwxrwx   0 root         (0) root         (0)     2088 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/variable_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     6771 2023-02-19 15:32:03.000000 probayes-0.0.6/probayes/vtypes.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 11:06:10.000000 probayes-0.0.6/probayes.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1952 2023-06-04 11:06:10.000000 probayes-0.0.6/probayes.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      828 2023-06-04 11:06:10.000000 probayes-0.0.6/probayes.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-04 11:06:10.000000 probayes-0.0.6/probayes.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       59 2023-06-04 11:06:10.000000 probayes-0.0.6/probayes.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-06-04 11:06:10.000000 probayes-0.0.6/probayes.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      437 2023-06-04 11:06:10.000000 probayes-0.0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)       89 2023-02-19 15:32:03.000000 probayes-0.0.6/setup.py
```

### Comparing `probayes-0.0.5/PKG-INFO` & `probayes-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: probayes
-Version: 0.0.5
+Version: 0.0.6
 Summary: Probability package supporting multiple Bayesian methods including MCMC
 Home-page: https://github.com/Bhumbra/probayes
 Author: Bhumbra
 Author-email: bhumbra@gmail.com
 License: UNKNOWN
 Description: # probayes
         Probability package supporting multiple Bayesian methods including MCMC
```

### Comparing `probayes-0.0.5/README.md` & `probayes-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/__init__.py` & `probayes-0.0.6/probayes/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 from probayes.constants import NEARLY_POSITIVE_ZERO, \
                                NEARLY_POSITIVE_INF, \
                                NEARLY_NEGATIVE_INF, \
                                LOG_NEARLY_POSITIVE_INF, \
                                COMPLEX_ZERO
 from probayes.vtypes import OO
 from probayes.named_dict import NamedDict
```

### Comparing `probayes-0.0.5/probayes/cf.py` & `probayes-0.0.6/probayes/cf.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/cond_cov.py` & `probayes-0.0.6/probayes/cond_cov.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/constants.py` & `probayes-0.0.6/probayes/constants.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/dependence.py` & `probayes-0.0.6/probayes/dependence.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/distribution.py` & `probayes-0.0.6/probayes/distribution.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/expr.py` & `probayes-0.0.6/probayes/expr.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/expression.py` & `probayes-0.0.6/probayes/expression.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/field.py` & `probayes-0.0.6/probayes/field.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/func.py` & `probayes-0.0.6/probayes/func.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/functional.py` & `probayes-0.0.6/probayes/functional.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/functional_utils.py` & `probayes-0.0.6/probayes/functional_utils.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/icon.py` & `probayes-0.0.6/probayes/icon.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/likelihoods.py` & `probayes-0.0.6/probayes/likelihoods.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/named_dict.py` & `probayes-0.0.6/probayes/named_dict.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/ops.py` & `probayes-0.0.6/probayes/ops.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/pd.py` & `probayes-0.0.6/probayes/pd.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/pd_utils.py` & `probayes-0.0.6/probayes/pd_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,16 +467,16 @@
     assert isinstance(key, str) and ' ' in key, \
       f"Aux dict must keyed by space-containing string, found {key}"
     assert isinstance(val, dict), \
       f"Aux dict must be a nested dictionary of dicts - found {type(val)}"
     for subkey, subval in val.items():
       assert isinstance(subkey, str), \
         f"Aux dict subkeys must be str, found {subkey}"
-      assert isinstance(subvals, np.ndarray), \
-        f"Aux dict subvals must be NumPy arrays, found {type(subvals)}"
+      assert isinstance(subval, np.ndarray), \
+        f"Aux dict subvals must be NumPy arrays, found {type(subval)}"
   with h5py.File(path, 'w', libver='latest') as hdf_write:
     for dist_name, dist_dict in serialised.items():
       group_write = hdf_write.create_group(dist_name)
       for key, val in dist_dict.items():
         if key == 'attrs':
           attrs = dist_dict['attrs']
           for k, v in attrs.items():
```

### Comparing `probayes-0.0.5/probayes/prob.py` & `probayes-0.0.6/probayes/prob.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/pscales.py` & `probayes-0.0.6/probayes/pscales.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/rf.py` & `probayes-0.0.6/probayes/rf.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/rf_utils.py` & `probayes-0.0.6/probayes/rf_utils.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/rv.py` & `probayes-0.0.6/probayes/rv.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/rv_utils.py` & `probayes-0.0.6/probayes/rv_utils.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/sd.py` & `probayes-0.0.6/probayes/sd.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/sd_utils.py` & `probayes-0.0.6/probayes/sd_utils.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/sp.py` & `probayes-0.0.6/probayes/sp.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/sp_utils.py` & `probayes-0.0.6/probayes/sp_utils.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/sympy_prob.py` & `probayes-0.0.6/probayes/sympy_prob.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/variable.py` & `probayes-0.0.6/probayes/variable.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/variable_utils.py` & `probayes-0.0.6/probayes/variable_utils.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes/vtypes.py` & `probayes-0.0.6/probayes/vtypes.py`

 * *Files identical despite different names*

### Comparing `probayes-0.0.5/probayes.egg-info/PKG-INFO` & `probayes-0.0.6/probayes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: probayes
-Version: 0.0.5
+Version: 0.0.6
 Summary: Probability package supporting multiple Bayesian methods including MCMC
 Home-page: https://github.com/Bhumbra/probayes
 Author: Bhumbra
 Author-email: bhumbra@gmail.com
 License: UNKNOWN
 Description: # probayes
         Probability package supporting multiple Bayesian methods including MCMC
```

### Comparing `probayes-0.0.5/probayes.egg-info/SOURCES.txt` & `probayes-0.0.6/probayes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

