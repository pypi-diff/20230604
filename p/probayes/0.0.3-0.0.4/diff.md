# Comparing `tmp/probayes-0.0.3.tar.gz` & `tmp/probayes-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/probayes-0.0.3.tar", last modified: Mon Sep 21 12:35:52 2020, max compression
+gzip compressed data, was "dist/probayes-0.0.4.tar", last modified: Sat Jun  3 17:33:28 2023, max compression
```

## Comparing `probayes-0.0.3.tar` & `probayes-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,44 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-09-21 12:35:52.000000 probayes-0.0.3/
--rwxrwxrwx   0 root         (0) root         (0)     2007 2020-09-21 12:35:52.000000 probayes-0.0.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1490 2020-09-01 08:50:50.000000 probayes-0.0.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-09-21 12:35:52.000000 probayes-0.0.3/ex/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-08-26 16:53:02.000000 probayes-0.0.3/ex/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      369 2020-09-21 12:12:34.000000 probayes-0.0.3/ex/bqa_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1495 2020-09-07 09:18:04.000000 probayes-0.0.3/ex/bqa_res.py
--rwxrwxrwx   0 root         (0) root         (0)     1241 2020-09-05 09:52:30.000000 probayes-0.0.3/ex/bqa_sim.py
--rwxrwxrwx   0 root         (0) root         (0)     1158 2020-09-18 09:06:03.000000 probayes-0.0.3/ex/bqa_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1379 2020-08-03 14:09:26.000000 probayes-0.0.3/ex/mctest.py
--rwxrwxrwx   0 root         (0) root         (0)      443 2020-08-26 13:39:30.000000 probayes-0.0.3/ex/pymc_ex.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-09-21 12:35:52.000000 probayes-0.0.3/probayes/
--rwxrwxrwx   0 root         (0) root         (0)      326 2020-09-21 12:29:43.000000 probayes-0.0.3/probayes/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2660 2020-08-26 07:47:59.000000 probayes-0.0.3/probayes/cond_cov.py
--rwxrwxrwx   0 root         (0) root         (0)    26732 2020-09-21 12:33:28.000000 probayes-0.0.3/probayes/dist.py
--rwxrwxrwx   0 root         (0) root         (0)    16277 2020-09-03 16:10:52.000000 probayes-0.0.3/probayes/dist_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    20971 2020-09-18 08:59:07.000000 probayes-0.0.3/probayes/domain.py
--rwxrwxrwx   0 root         (0) root         (0)    11988 2020-09-10 14:56:46.000000 probayes-0.0.3/probayes/func.py
--rwxrwxrwx   0 root         (0) root         (0)     9249 2020-09-10 16:27:47.000000 probayes-0.0.3/probayes/manifold.py
--rwxrwxrwx   0 root         (0) root         (0)     9688 2020-09-14 15:43:42.000000 probayes-0.0.3/probayes/prob.py
--rwxrwxrwx   0 root         (0) root         (0)     9254 2020-09-10 15:37:27.000000 probayes-0.0.3/probayes/pscales.py
--rwxrwxrwx   0 root         (0) root         (0)    16560 2020-08-26 09:20:37.000000 probayes-0.0.3/probayes/rf.py
--rwxrwxrwx   0 root         (0) root         (0)     1151 2020-08-26 07:47:59.000000 probayes-0.0.3/probayes/rf_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    34099 2020-08-27 09:50:51.000000 probayes-0.0.3/probayes/rj.py
--rwxrwxrwx   0 root         (0) root         (0)     2414 2020-08-26 07:49:31.000000 probayes-0.0.3/probayes/rj_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    22269 2020-09-18 08:50:15.000000 probayes-0.0.3/probayes/rv.py
--rwxrwxrwx   0 root         (0) root         (0)     4874 2020-09-14 14:18:53.000000 probayes-0.0.3/probayes/rv_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     9890 2020-08-26 09:43:38.000000 probayes-0.0.3/probayes/sp.py
--rwxrwxrwx   0 root         (0) root         (0)     3488 2020-08-26 07:47:59.000000 probayes-0.0.3/probayes/sp_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     6172 2020-09-10 15:14:06.000000 probayes-0.0.3/probayes/vtypes.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-09-21 12:35:52.000000 probayes-0.0.3/probayes.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     2007 2020-09-21 12:35:52.000000 probayes-0.0.3/probayes.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      624 2020-09-21 12:35:52.000000 probayes-0.0.3/probayes.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2020-09-21 12:35:52.000000 probayes-0.0.3/probayes.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       23 2020-09-21 12:35:52.000000 probayes-0.0.3/probayes.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2020-09-21 12:35:52.000000 probayes-0.0.3/probayes.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      397 2020-09-21 12:35:52.000000 probayes-0.0.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)       89 2020-08-06 09:04:39.000000 probayes-0.0.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-03 17:33:28.000000 probayes-0.0.4/
+-rwxrwxrwx   0 root         (0) root         (0)     1952 2023-06-03 17:33:28.000000 probayes-0.0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1443 2023-02-19 15:32:03.000000 probayes-0.0.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-03 17:33:28.000000 probayes-0.0.4/probayes/
+-rwxrwxrwx   0 root         (0) root         (0)     1152 2023-06-03 17:33:08.000000 probayes-0.0.4/probayes/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8183 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/cf.py
+-rwxrwxrwx   0 root         (0) root         (0)     2649 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/cond_cov.py
+-rwxrwxrwx   0 root         (0) root         (0)     1308 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/constants.py
+-rwxrwxrwx   0 root         (0) root         (0)    17024 2023-06-03 17:23:46.000000 probayes-0.0.4/probayes/dependence.py
+-rwxrwxrwx   0 root         (0) root         (0)    10726 2023-06-03 17:23:46.000000 probayes-0.0.4/probayes/distribution.py
+-rwxrwxrwx   0 root         (0) root         (0)    11752 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/expr.py
+-rwxrwxrwx   0 root         (0) root         (0)    17772 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/expression.py
+-rwxrwxrwx   0 root         (0) root         (0)    24783 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/field.py
+-rwxrwxrwx   0 root         (0) root         (0)    13044 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/func.py
+-rwxrwxrwx   0 root         (0) root         (0)     6946 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/functional.py
+-rwxrwxrwx   0 root         (0) root         (0)     1945 2023-06-03 17:23:46.000000 probayes-0.0.4/probayes/functional_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     3708 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/icon.py
+-rwxrwxrwx   0 root         (0) root         (0)     3871 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/likelihoods.py
+-rwxrwxrwx   0 root         (0) root         (0)     1058 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/named_dict.py
+-rwxrwxrwx   0 root         (0) root         (0)     3318 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/ops.py
+-rwxrwxrwx   0 root         (0) root         (0)    26427 2023-06-03 17:23:46.000000 probayes-0.0.4/probayes/pd.py
+-rwxrwxrwx   0 root         (0) root         (0)    19739 2023-06-03 17:23:46.000000 probayes-0.0.4/probayes/pd_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    16636 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/prob.py
+-rwxrwxrwx   0 root         (0) root         (0)     8398 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/pscales.py
+-rwxrwxrwx   0 root         (0) root         (0)    25737 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/rf.py
+-rwxrwxrwx   0 root         (0) root         (0)     6216 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/rf_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    24110 2023-06-03 17:23:46.000000 probayes-0.0.4/probayes/rv.py
+-rwxrwxrwx   0 root         (0) root         (0)     4207 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/rv_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    11573 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/sd.py
+-rwxrwxrwx   0 root         (0) root         (0)     1975 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/sd_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    10831 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/sp.py
+-rwxrwxrwx   0 root         (0) root         (0)     3467 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/sp_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     7409 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/sympy_prob.py
+-rwxrwxrwx   0 root         (0) root         (0)    29277 2023-06-03 17:23:46.000000 probayes-0.0.4/probayes/variable.py
+-rwxrwxrwx   0 root         (0) root         (0)     2088 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/variable_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     6771 2023-02-19 15:32:03.000000 probayes-0.0.4/probayes/vtypes.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-03 17:33:28.000000 probayes-0.0.4/probayes.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1952 2023-06-03 17:33:28.000000 probayes-0.0.4/probayes.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      828 2023-06-03 17:33:28.000000 probayes-0.0.4/probayes.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-03 17:33:28.000000 probayes-0.0.4/probayes.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       59 2023-06-03 17:33:28.000000 probayes-0.0.4/probayes.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-06-03 17:33:28.000000 probayes-0.0.4/probayes.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      437 2023-06-03 17:33:28.000000 probayes-0.0.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)       89 2023-02-19 15:32:03.000000 probayes-0.0.4/setup.py
```

### Comparing `probayes-0.0.3/PKG-INFO` & `probayes-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: probayes
-Version: 0.0.3
+Version: 0.0.4
 Summary: Probability package supporting multiple Bayesian methods including MCMC
 Home-page: https://github.com/Bhumbra/probayes
 Author: Bhumbra
 Author-email: bhumbra@gmail.com
 License: UNKNOWN
 Description: # probayes
         Probability package supporting multiple Bayesian methods including MCMC
@@ -13,27 +13,26 @@
         of probability. Since probayes is its infancy and in a state of flux, there is no manual. Currently probayes supports
         the following:
         
         1. Multiple random variable sampling in untransformed and transformed domain space. 
         2. Transitional simulation, including random walks, using Markov chain conditionals.
         3. Discrete grid exact inference.
         4. Ordinary Monte Carlo random sampling.
-        5. Ordinary Monto Carlo rejection sampling.
+        5. Ordinary Monte Carlo rejection sampling.
         6. Metropolis-Hastings MCMC sampling.
         7. Limited support for multivariate normal-covariance Gibbs sampling.
         
         In the near-future, it is intended to expand the scope of probayes to include:
         
-        1. Support Gibbs sampling using semi-conjugacy.
-        2. Code initial support for approximate inference using using dense mean field messaging.
-        3. Support derivative-based updates (HMC, gradient ascent/descent optimisation).
+        1. Code initial support for approximate inference using using dense mean field messaging.
+        2. Support derivative-based updates (HMC, gradient ascent/descent optimisation).
         
         A quickstart is also intended, but for now there are examples in the examples/ subdirectories:
         
-        1. tests/        Simple test scripts
+        1. checks/       Simple check scripts
         2. rv_examples/  Random variable examples
         3. markov/       Markov chain examples
         4. cov_examples/ Examples of using covariance matrices
         5. dgei/         Discrete grid exact inference examples
         6. omc/          Ordinary Monte-Carlo examples
         7. mcmc/         Markov chain Monte Carlo examples (Metropolis-Hastings, Gibbs...)
```

### Comparing `probayes-0.0.3/README.md` & `probayes-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 of probability. Since probayes is its infancy and in a state of flux, there is no manual. Currently probayes supports
 the following:
 
 1. Multiple random variable sampling in untransformed and transformed domain space. 
 2. Transitional simulation, including random walks, using Markov chain conditionals.
 3. Discrete grid exact inference.
 4. Ordinary Monte Carlo random sampling.
-5. Ordinary Monto Carlo rejection sampling.
+5. Ordinary Monte Carlo rejection sampling.
 6. Metropolis-Hastings MCMC sampling.
 7. Limited support for multivariate normal-covariance Gibbs sampling.
 
 In the near-future, it is intended to expand the scope of probayes to include:
 
-1. Support Gibbs sampling using semi-conjugacy.
-2. Code initial support for approximate inference using using dense mean field messaging.
-3. Support derivative-based updates (HMC, gradient ascent/descent optimisation).
+1. Code initial support for approximate inference using using dense mean field messaging.
+2. Support derivative-based updates (HMC, gradient ascent/descent optimisation).
 
 A quickstart is also intended, but for now there are examples in the examples/ subdirectories:
 
-1. tests/        Simple test scripts
+1. checks/       Simple check scripts
 2. rv_examples/  Random variable examples
 3. markov/       Markov chain examples
 4. cov_examples/ Examples of using covariance matrices
 5. dgei/         Discrete grid exact inference examples
 6. omc/          Ordinary Monte-Carlo examples
 7. mcmc/         Markov chain Monte Carlo examples (Metropolis-Hastings, Gibbs...)
```

### Comparing `probayes-0.0.3/probayes/cond_cov.py` & `probayes-0.0.4/probayes/cond_cov.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 A covariance-matrix-based conditional sampling class.
 """
 import numpy as np
 import scipy.stats
-from probayes.vtypes import isunitsetint, isscalar, uniform
+from probayes.vtypes import isunitsetint, uniform
 
 #-------------------------------------------------------------------------------
 class CondCov:
 
   # Protected
   _mean = None # Means 
   _cov = None  # Covariance matrix
@@ -60,9 +60,8 @@
     mean = self._mean[idx] + float(self._coef[idx].dot(dmu))
     stdv = self._stdv[idx]
     vals = scipy.stats.norm.ppf(cdf, loc=mean, scale=stdv)
     if not cond_pdf:
       return vals
     return vals, scipy.stats.norm.pdf(vals, loc=mean, scale=stdv)
 
-
 #-------------------------------------------------------------------------------
```

### Comparing `probayes-0.0.3/probayes/dist.py` & `probayes-0.0.4/probayes/pd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,236 +1,249 @@
-# A module for realised probability distributions, a triple comprising 
-# variable names, their values (vals), and respective probabilities (prob).
+""" Provides probability distribution funciontlaity based on Distribution """
 
 #-------------------------------------------------------------------------------
 import collections
 import numpy as np
-from probayes.dist_utils import str_margcond, margcond_str, product, summate, \
-                                rekey_dict, ismonotonic
-from probayes.vtypes import issingleton, isscalar
+from probayes.named_dict import NamedDict
+from probayes.pd_utils import str_margcond, margcond_str, product, summate, \
+                              rekey_dict, ismonotonic
+from probayes.vtypes import isscalar
 from probayes.pscales import eval_pscale, rescale, iscomplex
-from probayes.pscales import prod_pscale, prod_rule, div_prob
-from probayes.manifold import Manifold
+from probayes.pscales import div_prob
+from probayes.distribution import Distribution
 
 #-------------------------------------------------------------------------------
-class Dist (Manifold):
-
-  # Public
-  prob = None   # Numpy array
-  name = None   # Name of distribution
-  marg = None   # Ordered dictionary of marginals: {key: name}
-  cond = None   # Ordered dictionary of conditionals: key: name}
-
+class PD (Distribution):
+  """ A probability distribution is a distribution with corresponding 
+  probabilities. The dimensions of the probability scalar or array must be
+  commensurate with the values of the distribution according to their assigned
+  dimensions. 
+
+  While it is intended for PD instances to come from RV, RF, SD, or SP calls,
+  PDs can be instantiated directly.
+  """
   # Protected
-  _keyset = None         # Keys as set according to name
-  _pscale = None         # Same convention as _Prob
+  _prob = None    # Probability
+  _pscale = None  # Same convention as Prob()
+  _marg = None    # Ordered dictionary of marginals: {key: name}
+  _cond = None    # Ordered dictionary of conditionals: key: name}
 
 #-------------------------------------------------------------------------------
-  def __init__(self, name=None, vals=None, dims=None, prob=None, pscale=None):
-    self.set_name(name)
-    self.set_vals(vals, dims)
-    self.set_prob(prob, pscale)
+  def __init__(self, name, *args, **kwds):
+    """ Initialises the PD with a name, args, and kwds in the same way as 
+    Distribution(), except with the following reserved keywords:
+      
+      'dims': sets the dimensionality. 
+      'prob': sets the probability scalar or array. 
+      'pscale': sets the pscale
+    """
+    args = tuple(args)
+    kwds = dict(kwds)
+    prob = None if 'prob' not in kwds else kwds.pop('prob')
+    pscale = None if 'pscale' not in kwds else kwds.pop('pscale')
+    super().__init__(name, *args, **kwds)
+    self.pscale = pscale
+    self.prob = prob
 
 #-------------------------------------------------------------------------------
-  def set_name(self, name=None):
+  @property
+  def name(self):
+    return self._name
+
+  @property
+  def marg(self):
+    return self._marg
+
+  @property
+  def cond(self):
+    return self._cond
+
+  @name.setter
+  def name(self, name):
     # Only the name is sensitive to what are marginal and conditional variables
-    self.name = name
-    self.marg, self.cond = str_margcond(self.name)
-    self._keyset = set(self.marg).union(set(self.cond))
-    return self._keyset
+    NamedDict.name.fset(self, name)
+    self._marg, self._cond = str_margcond(self.name)
+    
+  @property
+  def short_name(self):
+    marg_keys = list(self._marg.keys())
+    cond_keys = list(self._cond.keys())
+    marg_str = ','.join(marg_keys)
+    cond_str = ','.join(cond_keys)
+    return '|'.join([marg_str, cond_str]) if cond_str else marg_str
 
 #-------------------------------------------------------------------------------
-  def set_vals(self, vals=None, dims=None):
-    argout = super().set_vals(vals, dims)
-    if not self._keys or not any(self._aresingleton):
-      return argout
+  @property
+  def pscale(self):
+    return self._pscale
 
-    # Override name entries for scalar values
-    for i, key in enumerate(self._keys):
-      assert key in self._keyset, \
-          "Value key {} not found among name keys {}".format(key, self._keyset)
-      if self._aresingleton[i]:
-        if key in self.marg.keys():
-          self.marg[key] = "{}={}".format(key, self.vals[key])
-        elif key in self.cond.keys():
-          self.cond[key] = "{}={}".format(key, self.vals[key])
-        else:
-          raise ValueError("Variable {} not accounted for in name {}".format(
-                            key, self.name))
-    self.name = margcond_str(self.marg, self.cond)
-    return argout
+  @pscale.setter
+  def pscale(self, pscale=None):
+    self._pscale = eval_pscale(pscale)
 
 #-------------------------------------------------------------------------------
-  def set_prob(self, prob=None, pscale=None):
-    self.prob = prob
-    self._pscale = eval_pscale(pscale)
-    if self.prob is None:
-      return self._pscale
+  @property
+  def prob(self):
+    return self._prob
+
+  @prob.setter
+  def prob(self, prob=None):
+    self._prob = prob
+    if self._prob is None:
+      return
     if self._issingleton:
-      assert isscalar(self.prob), "Singleton vals with non-scalar prob"
+      assert isscalar(self._prob), "Singleton vals with non-scalar prob"
     else:
-      assert not isscalar(self.prob), "Non singleton values with scalar prob"
-      assert self.ndim == self.prob.ndim, \
+      assert not isscalar(self._prob), "Non singleton values with scalar prob"
+      assert self._ndim == self._prob.ndim, \
         "Mismatch in dimensionality between values {} and probabilities {}".\
-        format(self.ndim, self.prob.ndim)
-      assert np.all(np.array(self.shape) == np.array(self.prob.shape)), \
+        format(self.ndim, self._prob.ndim)
+      assert np.all(np.array(self._shape) == np.array(self._prob.shape)), \
         "Mismatch in dimensions between values {} and probabilities {}".\
-        format(self.shape, self.prob.shape)
-    return self._pscale
+        format(self._shape, self._prob.shape)
 
 #-------------------------------------------------------------------------------
-  def ret_vals(self, keys=None):
-    keys = keys or self._keys
-    keys = set(keys)
-    vals = collections.OrderedDict()
-    seen_keys = set()
-    for i, key in enumerate(self._keys):
-      if key in keys and key not in seen_keys:
-        if self._aresingleton[i]:
-          seen_keys.add(key)
-          vals.update({key: self.vals[key]})
-        else:
-          shared_keys = [key]
-          for j, cand_key in enumerate(self._keys):
-            if j > i and cand_key in keys and not self._aresingleton[j]:
-              if self.dims[key] == self.dims[cand_key]:
-                shared_keys.append(cand_key)
-          if len(shared_keys) == 1:
-            vals.update({key: np.ravel(self.vals[key])})
-            seen_keys.add(key)
-          else:
-            val = [None] * len(shared_keys)
-            for j, shared_key in enumerate(shared_keys):
-              val[j] = np.ravel(self.vals[shared_key])
-              seen_keys.add(shared_key)
-            vals.update({','.join(shared_keys): tuple(val)})
-    return vals
+  @property
+  def dims(self):
+    return self._dims
 
-#-------------------------------------------------------------------------------
-  def ret_marg_vals(self):
-    return self.ret_vals(self.marg.keys())
+  @dims.setter
+  def dims(self, dims=None):
+    """ Sets the dimensions for each of the variables.
 
-#-------------------------------------------------------------------------------
-  def ret_cond_vals(self):
-    assert self.cond, "No conditioning variables"
-    return self.ret_vals(self.cond.keys())
+    :param dims: a dictionary of {variable_name: variable_dim}
+
+    The keys should correspond to that of a dictionary. If dims
+    is None, then the dimensionality is set according to the
+    order in values.
+    """
+    Distribution.dims.fset(self, dims)
+
+    # Override name entries for scalar values
+    for i, key in enumerate(self._keylist):
+      assert key in self._keyset, \
+          "Value key {} not found among name keys {}".format(key, self._keyset)
+      if self._aresingleton[i]:
+        if key in self.marg.keys():
+          self.marg[key] = "{}={}".format(key, self[key])
+        elif key in self.cond.keys():
+          self.cond[key] = "{}={}".format(key, self[key])
+        else:
+          raise ValueError("Variable {} not accounted for in name {}".format(
+                            key, self.name))
+    self._name = margcond_str(self.marg, self.cond)
 
 #-------------------------------------------------------------------------------
   def marginalise(self, keys):
     # from p(A, key | B), returns P(A | B)
     if isinstance(keys, str):
       keys = [keys]
     for key in keys:
-      assert key in self.marg.keys(), \
-        "Key {} not marginal in distribution {}".format(key, self.name)
+      assert key in self._marg.keys(), \
+        "Key {} not marginal in distribution {}".format(key, self._name)
     keys  = set(keys)
-    marg = collections.OrderedDict(self.marg)
-    cond = collections.OrderedDict(self.cond)
+    marg = collections.OrderedDict(self._marg)
+    cond = collections.OrderedDict(self._cond)
     vals = collections.OrderedDict()
     dims = collections.OrderedDict()
     dim_delta = 0
     sum_axes = set()
-    for i, key in enumerate(self._keys):
-      new_dim = None
+    for i, key in enumerate(self._keylist):
       if key in keys:
         assert not self._aresingleton[i], \
             "Cannot marginalise along scalar for key {}".format(key)
-        sum_axes.add(self.dims[key])
+        sum_axes.add(self._dims[key])
         marg.pop(key)
         dim_delta += 1
       else:
         if not self._aresingleton[i]:
-          dims.update({key: self.dims[key] - dim_delta})
-        vals.update({key:self.vals[key]})
+          dims.update({key: self._dims[key] - dim_delta})
+        vals.update({key:self[key]})
     name = margcond_str(marg, cond)
-    prob = rescale(self.prob, self._pscale, 1.)
+    prob = rescale(self._prob, self._pscale, 1.)
     sum_prob = np.sum(prob, axis=tuple(sum_axes), keepdims=False)
     prob = rescale(sum_prob, 1., self._pscale)
-    return Dist(name=name, 
-                vals=vals, 
-                dims=dims, 
-                prob=prob, 
-                pscale=self._pscale)
+    return PD(name, vals, dims=dims, prob=prob, pscale=self._pscale)
 
 #-------------------------------------------------------------------------------
   def marginal(self, keys):
     # from p(A, key | B), returns P(key | B)
     if isinstance(keys, str):
       keys = [keys]
 
     # Check keys arg marginal
     keys = set(keys)
     dims = set()
     for key in keys:
-      assert key in self.marg.keys(), \
-        "Key {} not marginal in distribution {}".format(key, self.name)
-      dim = self.dims[key]
+      assert key in self._marg.keys(), \
+        "Key {} not marginal in distribution {}".format(key, self._name)
+      dim = self._dims[key]
       if dim is not None:
         dims.add(dim)
 
     # Check consistency of marginal dims
-    for key in self._keys:
-      dim = self.dims[key]
+    for key in self._keylist:
+      dim = self._dims[key]
       if dim in dims:
         assert key in keys, \
             "Dimensionality precludes marginalising {} without: {}".\
             format(keys, key)
 
     # Determine keys to marginalise by exclusion
     marginalise_keys = set()
     aresingletons = []
     marg_scalars = set()
-    for i, key in enumerate(self._keys):
+    for i, key in enumerate(self._keylist):
       singleton = self._aresingleton[i]
       marginal = key in keys
-      if key in self.marg.keys():
+      if key in self._marg.keys():
         aresingletons.append(singleton)
         if singleton:
           marg_scalars.add(key)
         if not singleton and not marginal:
           marginalise_keys.add(key)
 
     # If including any marginal scalars, must include all scalars
     if any(aresingletons):
       assert marg_scalars.issubset(keys), \
         "If evaluating marginal for key {}".format(key) + ", " + \
-        "must include all marginal scalars in {}".format(self.marg.keys())
+        "must include all marginal scalars in {}".format(self._marg.keys())
 
     return self.marginalise(marginalise_keys)
         
 #-------------------------------------------------------------------------------
   def conditionalise(self, keys):
     # from P(A, key | B), returns P(A | B, key).
     # if vals[key] is a scalar, this effectively normalises prob
     if isinstance(keys, str):
       keys = [keys]
     keys = set(keys)
     for key in keys:
-      assert key in self.marg.keys(), \
+      assert key in self._marg.keys(), \
         "Key {} not marginal in distribution {}".format(key, self.name)
     dims = collections.OrderedDict()
-    marg = collections.OrderedDict(self.marg)
-    cond = collections.OrderedDict(self.cond)
+    marg = collections.OrderedDict(self._marg)
+    cond = collections.OrderedDict(self._cond)
     normalise = False
     delta = 0
     marg_scalars = set()
-    for i, key in enumerate(self._keys):
+    for i, key in enumerate(self._keylist):
       if key in keys:
         cond.update({key: marg.pop(key)})
       if self._aresingleton[i]:
         dims.update({key: None})
         if key in keys:
           normalise = True
-      elif key in self.marg.keys():
+      elif key in self._marg.keys():
         if self._aresingleton[i]:
           marg_scalars.add(key)
         if key in keys:
           delta += 1 # Don't add to dim just yet
         else:
-          dim = self.dims[key]
+          dim = self._dims[key]
           dims.update({key: dim})
       else:
         dim = self.dims[key] - delta
         dims.update({key: dim})
 
     # Reduce remaining marginals to lowest dimension
     dim_val = [val for val in dims.values() if val is not None]
@@ -244,212 +257,196 @@
           dim_max = max(dim_max, dim)
     dim_min = self.ndim
     for key in keys:
       dim = self.dims[key]
       if dim is not None:
         dim_min = min(dim_min, dim)
     for key in keys:
-      dim = self.dims[key]
+      dim = self._dims[key]
       if dim is not None:
         dims.update({key: dim-dim_min+dim_max+1})
     if normalise:
       assert marg_scalars.issubset(set(keys)), \
         "If conditionalising for key {}".format(key) + "," + \
-        "must include all marginal scalars in {}".format(self.marg.keys())
+        "must include all marginal scalars in {}".format(self._marg.keys())
 
     # Setup vals dimensions and evaluate probabilities
     name = margcond_str(marg, cond)
-    vals = super().redim(dims).vals
+    vals = collections.OrderedDict(super().redim(dims))
     old_dims = []
     new_dims = []
     sum_axes = set()
-    for key in self._keys:
-      old_dim = self.dims[key]
+    for key in self._keylist:
+      old_dim = self._dims[key]
       if old_dim is not None and old_dim not in old_dims:
         old_dims.append(old_dim)
         new_dims.append(dims[key])
-        if key not in keys and key in self.marg.keys():
+        if key not in keys and key in self._marg.keys():
           sum_axes.add(dims[key])
-    prob = np.moveaxis(self.prob, old_dims, new_dims)
+    prob = np.moveaxis(self._prob, old_dims, new_dims)
     if normalise and iscomplex(self._pscale): 
       prob = prob - prob.max()
     prob = rescale(prob, self._pscale, 1.)
     if normalise:
       prob = div_prob(prob, np.sum(prob))
     if len(sum_axes):
       prob = div_prob(prob, \
                          np.sum(prob, axis=tuple(sum_axes), keepdims=True))
     prob = rescale(prob, 1., self._pscale)
-    return Dist(name=name, 
-                vals=vals, 
-                dims=dims, 
-                prob=prob, 
-                pscale=self._pscale)
+    return PD(name, vals, dims=dims, prob=prob, pscale=self._pscale)
 
 #-------------------------------------------------------------------------------
   def redim(self, dims):
     """ 
     Returns a distribution according to redimensionised values in dims, index-
     ordered by the order in dims
     """
-    manifold = super().redim(dims)
-    vals, dims = manifold.vals, manifold.dims
-    prob = self.prob
+    dist = super().redim(dims)
+    vals, dims = dict(dist), dist.dims
+    prob = self._prob
 
     # Need to realign prob axes to new dimensions
     if not self._issingleton:
       old_dims = []
       new_dims = []
-      for i, key in enumerate(self._keys):
+      for i, key in enumerate(self._keylist):
         if not self._aresingletons[i]:
           old_dims.append(self._dims[key])
           new_dims.append(dims[key])
       prob = np.moveaxis(prob, old_dims, new_dims)
 
-    return Dist(name=self._name, 
-                vals=vals, 
-                dims=dims, 
-                prob=prob, 
-                pscale=self._pscale)
+    return PD(self._name, vals, dims=dims, prob=prob, pscale=self._pscale)
 
 #-------------------------------------------------------------------------------
   def rekey(self, keymap):
     """
     Returns a distribution with modified key names without axes changes.
     """
-    manifold = super().rekey(keymap)
-    marg = rekey_dict(self.marg, keymap) 
-    cond = rekey_dict(self.cond, keymap)
+    dist = super().rekey(keymap)
+    marg = rekey_dict(self._marg, keymap) 
+    cond = rekey_dict(self._cond, keymap)
     name = margcond_str(marg, cond)
-    return Dist(name=name, 
-                vals=manifold.vals, 
-                dims=manifold.dims, 
-                prob=self.prob, 
-                pscale=self._pscale)
+    return PD(name, dict(dist), dims=dist.dims, 
+              prob=self.prob, pscale=self._pscale)
 
 #-------------------------------------------------------------------------------
   def prod(self, keys):
     # from P(A, key | B), returns P(A, {} | B)
     if isinstance(keys, str):
       keys = [keys]
     for key in keys:
       assert key in self.marg.keys(), \
         "Key {} not marginal in distribution {}".format(key, self.name)
     keys  = set(keys)
-    marg = collections.OrderedDict(self.marg)
-    cond = collections.OrderedDict(self.cond)
+    marg = collections.OrderedDict(self._marg)
+    cond = collections.OrderedDict(self._cond)
     vals = collections.OrderedDict()
     dims = collections.OrderedDict()
     dim_delta = 0
     prod_axes = []
-    for i, key in enumerate(self._keys):
-      new_dim = None
+    for i, key in enumerate(self._keylist):
       if key in keys:
         assert not self._aresingleton[i], \
             "Cannot apply product along scalar for key {}".format(key)
-        if self.dims[key] not in prod_axes:
+        if self._dims[key] not in prod_axes:
           prod_axes.append(self.dims[key])
           dim_delta += 1
         marg.update({key: key+"={}"})
-        vals.update({key: {self.vals[key].size}})
+        vals.update({key: {self[key].size}})
       else:
         if not self._aresingleton[i]:
-          dims.update({key: self.dims[key] - dim_delta})
-        vals.update({key:self.vals[key]})
+          dims.update({key: self._dims[key] - dim_delta})
+        vals.update({key:self[key]})
     name = margcond_str(marg, cond)
     pscale = self._pscale
     pscale_product = pscale
     if pscale_product not in [0., 1.]:
       pscale_scaling = np.prod(np.array(self.shape)[prod_axes])
       if iscomplex(pscale):
         pscale_product += pscale*pscale_scaling 
       else:
         pscale_product *= pscale**pscale_scaling 
     prob = np.sum(self.prob, axis=tuple(prod_axes)) if iscomplex(pscale) \
            else np.prod(self.prob, axis=tuple(prod_axes))
-    return Dist(name=name, 
-                vals=vals, 
-                dims=dims, 
-                prob=prob, 
-                pscale=pscale_product)
+    return PD(name, vals, dims=dims, prob=prob, pscale=pscale_product)
 
 #-------------------------------------------------------------------------------
   def expectation(self, keys=None, exponent=None):
     keys = keys or self.marg.keys()
     if isinstance(keys, str):
       keys = [keys]
     for key in keys:
-      assert key in self.marg.keys(), \
-        "Key {} not marginal in distribution {}".format(key, self.name)
+      assert key in self._marg.keys(), \
+        "Key {} not marginal in distribution {}".format(key, self._name)
     keys = set(keys)
     sum_axes = []
-    dims = collections.OrderedDict(self.dims)
-    for i, key in enumerate(self._keys):
+    dims = collections.OrderedDict(self._dims)
+    for i, key in enumerate(self._keylist):
       if key in keys:
-        if self.dims[key] is not None:
-          sum_axes.append(self.dims[key])
+        if self._dims[key] is not None:
+          sum_axes.append(self._dims[key])
         dims[key] = None
-    prob = rescale(self.prob, self._pscale, 1.)
+    prob = rescale(self._prob, self._pscale, 1.)
     if sum_axes:
       sum_prob = np.sum(prob, axis=tuple(set(sum_axes)), keepdims=False)
     else:
       sum_prob = np.sum(prob)
     vals = collections.OrderedDict()
-    for i, key in enumerate(self._keys):
+    for i, key in enumerate(self._keylist):
       if key in keys:
-        val = self.vals[key] if not exponent else self.vals[key]**exponent
+        val = self[key] if not exponent else self[key]**exponent
         if self._aresingleton[i]:
           vals.update({key: val})
         else:
-          expt_numerator = np.sum(prob*val, 
+          expt_numerator = np.sum(prob*np.array(val, dtype=float), 
                                   axis=tuple(set(sum_axes)), keepdims=False)
           vals.update({key: div_prob(expt_numerator, sum_prob)})
-      elif key in self.cond.keys():
-        vals.update({key: self.vals[key]})
+      elif key in self._cond.keys():
+        vals.update({key: self[key]})
     return vals
 
 #-------------------------------------------------------------------------------
   def quantile(self, q=0.5):
     """ Returns probability quantiles in distribution for sorted values """
     quants = [q] if isscalar(q) else q
 
     # Deal with trivial scalar case
     if self._issingleton:
-      quantiles = [self.vals] * len(quants)
+      quantiles = [collections.OrderedDict(self)] * len(quants)
       if isscalar(q):
         return quantiles[0]
       return quantiles
 
     # Check for monotonicity
     unsorted = set()
-    for i, key in enumerate(self._keys):
+    for i, key in enumerate(self._keylist):
       if not self._aresingleton[i]:
-        if not ismonotonic(self.vals[key]):
+        if not ismonotonic(self[key]):
           unsorted.add(key)
 
     # Evaluate quantiles from cumulative probability
     ravprob = rescale(np.ravel(self.prob), self._pscale, 1.)
     cumprob = np.cumsum(ravprob)
     cumprob = div_prob(cumprob, cumprob[-1])
     cum_idx = np.maximum(0, np.digitize(np.array(quants), cumprob)-1).tolist()
 
     # Interpolate in last axis
     quantiles = [None] * len(cum_idx)
     for j, _cum_idx in enumerate(cum_idx):
       rav_idx = int(_cum_idx)
-      unr_idx = np.unravel_index(rav_idx, self.shape)
+      unr_idx = np.unravel_index(rav_idx, self._shape)
       quantiles[j] = collections.OrderedDict()
-      for i, key in enumerate(self._keys):
+      for i, key in enumerate(self._keylist):
         if self._aresingleton[i]:
-          quantiles[j].update({key: self.vals[key]})
+          quantiles[j].update({key: self[key]})
         elif key in unsorted:
-          quantiles[j].update({key: {self.vals[key].size}})
+          quantiles[j].update({key: {self[key].size}})
         else:
-          dim = self.dims[key]
-          val = np.ravel(self.vals[key])
+          dim = self._dims[key]
+          val = np.ravel(self[key])
           idx = np.minimum(unr_idx[dim], len(val) - 1)
           if dim < self.ndim - 1 or idx == len(val) - 1:
             quantiles[j].update({key: val[idx]})
           else:
             vals = val[idx:idx+2]
             ravp = ravprob[rav_idx:rav_idx+2]
             if np.abs(np.diff(ravp)) < min(quants[j], 1. - quants[j]):
@@ -462,119 +459,110 @@
     if isscalar(q):
       return quantiles[0]
     return quantiles
 
 #-------------------------------------------------------------------------------
   def sorted(self, key):
     """ Returns a distribution ordered by key """
-    dim = self.dims[key]
+    dim = self._dims[key]
 
     # Handle trivial case
     if dim is None:
-      return Dist(self.name, self.vals, self.dims, self.prob, self._pscale)
+      return PD(self._name, dict(self), dims=self._dims, 
+                prob=self._prob, pscale=self._pscale)
 
     # Argsort needed to sort probabilities
-    ravals = np.ravel(self.vals[key])
+    ravals = np.ravel(self[key])
     keyidx = np.argsort(ravals)
     keyval = ravals[keyidx]
 
     # Reorder probabilities in affected dimension
-    slices = [slice(i) for i in self.shape]
+    slices = [slice(i) for i in self._shape]
     slices[dim] = keyidx
-    prob = self.prob[tuple(slices)]
+    prob = self._prob[tuple(slices)]
 
     # Evaluate values arrays
     vals = collections.OrderedDict()
-    for _key, _val in self.vals.items():
-      if self.dims[_key] != dim:
+    for _key, _val in self.items():
+      if self._dims[_key] != dim:
         vals.update({_key: _val})
       elif _key == key:
         vals.update({_key: keyval})
       else:
         vals.update({_key: np.ravel(_val)[keyidx]})
-    return Dist(self.name, vals, self.dims, prob, self._pscale)
+    return PD(self.name, vals, dims=self._dims, 
+              prob=prob, pscale=self._pscale)
     
 #-------------------------------------------------------------------------------
   def rescaled(self, pscale=None):
     prob = rescale(np.copy(self.prob), self._pscale, pscale)
-    return Dist(name=self.name, 
-                vals=self.vals, 
-                dims=self.dims,
-                prob=prob, 
-                pscale=pscale)
+    return PD(self.name, dict(self), dims=self.dims,
+              prob=prob, pscale=pscale)
 
 #-------------------------------------------------------------------------------
-  def ret_keyset(self):
-    return self._keyset
-
-#-------------------------------------------------------------------------------
-  def ret_pscale(self):
-    return self._pscale
-
- 
-#-------------------------------------------------------------------------------
   def __call__(self, values, keepdims=False):
     # Slices distribution according to scalar values given as a dictionary
 
+    if isinstance(values, str):
+      assert values in ['marg', 'cond'], \
+          "String call must be either 'marg' or 'cond'"
+      dictionary = self.marg if values == 'marg' else self.cond
+      return self.lookup(list(dictionary.keys()))
     assert isinstance(values, dict),\
         "Values must be dict type, not {}".format(type(values))
     keys = values.keys()
     keyset = set(values.keys())
     assert len(keyset.union(self._keyset)) == len(self._keyset),\
         "Unrecognised key among values keys: {}".format(keys())
-    marg = collections.OrderedDict(self.marg)
-    cond = collections.OrderedDict(self.cond)
-    dims = collections.OrderedDict(self.dims)
-    vals = collections.OrderedDict(self.vals)
+    marg = collections.OrderedDict(self._marg)
+    cond = collections.OrderedDict(self._cond)
+    dims = collections.OrderedDict(self._dims)
+    vals = collections.OrderedDict(self)
     slices = [slice(None) for _ in range(self.ndim)]
     dim_delta = 0
-    for i, key in enumerate(self._keys):
+    for i, key in enumerate(self._keylist):
       check_dims = False
       if not self._aresingleton[i]:
         dim = self.dims[key]
         if key in keyset:
           assert np.isscalar(values[key]), \
               "Values must contain scalars but found {} for {}".\
               format(values[key], key)
-          match = np.ravel(self.vals[key]) == values[key]
+          match = np.ravel(self[key]) == values[key]
           n_matches = match.sum()
           post_eq = '{}'.format(values[key])
           if n_matches == 0:
             slices[dim] = slice(0, 0)
             vals[key] = np.array([])
           elif n_matches == 1 and not keepdims:
             dim_delta += 1
             slices[dim] = int(np.nonzero(match)[0])
             vals[key] = values[key]
             dims[key] = None
           else:
             post_eq = '[]'
             slices[dim] = np.nonzero(match)[0]
-            vals[key] = self.vals[key][slices[dim]]
+            vals[key] = self[key][slices[dim]]
             check_dims = True
           update_keys = [key]
           if check_dims:
-            for k, v in self.vals.items():
-              if dim == self.dims[k] and k not in keyset:
-                vals[k] = self.vals[k][slices[dim]]
+            for k, v in self.items():
+              if dim == self._dims[k] and k not in keyset:
+                vals[k] = self[k][slices[dim]]
                 update_keys.append(k)
           for update_key in update_keys:
             if key in marg.keys():
               marg[key] = "{}={}".format(key, post_eq)
             elif key in cond.keys():
               cond[key] = "{}={}".format(key, post_eq)
         elif dim_delta:
           dims[key] = dims[key] - dim_delta
     name = margcond_str(marg, cond)
-    prob = self.prob[tuple(slices)]
-    return Dist(name=name, 
-                vals=vals, 
-                dims=dims, 
-                prob=prob, 
-                pscale=self._pscale)
+    prob = self._prob[tuple(slices)]
+    return PD(name, vals, dims=dims, prob=prob, pscale=self._pscale)
 
 #-------------------------------------------------------------------------------
   def __mul__(self, other):
     return product(*tuple([self, other]))
 
 #-------------------------------------------------------------------------------
   def __add__(self, other):
@@ -588,128 +576,130 @@
     The conditionals must match.
     The scalar marginals must match.
     """
     # Assert scalar division and operands compatible
     assert set(self.cond.keys())== set(other.cond.keys()),  \
       "Conditionals must match"
 
-    divs = other.ret_issingleton()
+    divs = other.issingleton
     if divs:
       marg_scalars = set()
-      for i, key in enumerate(self._keys):
-        if key in self.marg.keys() and self._aresingleton[i]:
+      for i, key in enumerate(self._keylist):
+        if key in self._marg.keys() and self._aresingleton[i]:
           marg_scalars.add(key)
       assert marg_scalars == set(other.marg.keys()), \
         "For divisor singletons, scalar marginals must match"
 
     # Prepare quotient marg and cond keys
     keys = other.marg.keys()
-    marg = collections.OrderedDict(self.marg)
-    cond = collections.OrderedDict(self.cond)
-    vals = collections.OrderedDict(self.cond)
-    re_shape = np.ones(self.ndim, dtype=int)
-    for i, key in enumerate(self._keys):
+    marg = collections.OrderedDict(self._marg)
+    cond = collections.OrderedDict(self._cond)
+    vals = collections.OrderedDict(self._cond)
+    re_shape = np.ones(self._ndim, dtype=int)
+    for i, key in enumerate(self._keylist):
       if key in keys:
         cond.update({key:marg.pop(key)})
         if not self._aresingleton[i] and not divs:
-          re_shape[self.dims[key]] = other.vals[key].size
+          re_shape[self.dims[key]] = other[key].size
       else:
-        vals.update({key:self.vals[key]})
+        vals.update({key:self[key]})
 
     # Append the marginalised variables and end of vals
-    for i, key in enumerate(self._keys):
+    for i, key in enumerate(self._keylist):
       if key in keys:
-        vals.update({key:self.vals[key]})
+        vals.update({key:self[key]})
 
     # Evaluate probabilities
     name = margcond_str(marg, cond)
     divp = other.prob if divs else other.prob.reshape(re_shape)
-    prob = div_prob(self.prob, divp, self._pscale, other.ret_pscale())
-    return Dist(name=name, 
-                vals=vals, 
-                dims=self.dims, 
-                prob=prob, 
-                pscale=self._pscale)
+    prob = div_prob(self._prob, divp, self._pscale, other.pscale)
+    return PD(name, vals, dims=self._dims, prob=prob, pscale=self._pscale)
 
 #-------------------------------------------------------------------------------
-  def remarginalise(self, manifold, *args, **kwds):
-    """ Redistributes probability distribution within manifold according to a
+  def remarginalise(self, distribution, *args, **kwds):
+    """ Redistributes probability distribution within distribution according to a
     dictionary (in args[0]) or keywords, for which the keys represent the
     marginal keys and corresponding values contain their corresponding values
     according to the shape of self.prob. Conditional variables are unchanged.
     """
 
     # Simple assertions
     assert not self._issingleton,\
         "Function dist.remarginalise() not operative for scalar probabilities"
-    assert isinstance(manifold, Manifold),\
-        "First argument must be Manifold type not {}".format(type(manifold))
+    assert isinstance(distribution, Distribution),\
+        "First argument must be Distribution type not {}".format(type(distribution))
 
     # Read and check dictionary
     vals = None
     if args:
       assert len(args) == 1 and not kwds, \
           "Use a single dictionary argument or keywords, not both"
       vals = args[0]
     elif kwds:
       vals = dict(kwds)
     assert isinstance(vals, dict), \
         "Dictionary argument expected, not {}".format(type(vals))
-    marg_keys = list(manifold.vals.keys())
-    dims = manifold.dims
+    marg_keys = list(distribution.keys())
+    dims = distribution.dims
     for key, val in vals.items():
       if dims[key] is not None:
         assert np.all(np.array(val.shape) == np.array(self.shape)),\
             "Values for {} incommensurate".format
         assert key in marg_keys, \
-            "Key {} not present in inputted manifold"
+            "Key {} not present in inputted distribution"
 
     # Evaluate output indices for each space in probability
-    shape = manifold.shape
+    shape = distribution.shape
     indices = [np.empty(_size, dtype=int) for _size in shape]
     for key, dim in dims.items():
       if dim is not None:
-        edges = np.array(np.ravel(manifold.vals[key]), dtype=float)
+        edges = np.array(np.ravel(distribution[key]), dtype=float)
         rav_vals = np.array(np.ravel(vals[key]), dtype=float)
         indices[dim] = np.maximum(0, np.minimum(len(edges)-1, \
                                      np.digitize(rav_vals, edges)-1))
 
     # Iterate through every self.prob value
-    rav_prob = np.ravel(rescale(self.prob, self._pscale, 1.))
-    rem_prob = np.zeros(manifold.shape, dtype=float)
+    rav_prob = np.ravel(rescale(self._prob, self._pscale, 1.))
+    rem_prob = np.zeros(distribution.shape, dtype=float)
     for i in range(self.size):
       rem_idx = tuple([idx[i] for idx in indices])
       rem_prob[rem_idx] += rav_prob[i]
 
     # Replace marginal keys and keep conditional keys
-    rem_vals = collections.OrderedDict(manifold.vals)
-    rem_dims = collections.OrderedDict(manifold.dims)
+    rem_vals = collections.OrderedDict(distribution)
+    rem_dims = collections.OrderedDict(distribution.dims)
     marg_str = []
-    for key, val in manifold.vals.items():
+    for key, val in distribution.items():
       marg_str.append(key)
       if val is not None:
         if np.isscalar(val):
           marg_str[-1] = "{}={}".format(key, val)
         else:
           marg_str[-1] = key + "=[]"
     rem_name = ','.join(marg_str)
-    if '|' in self.name:
-      rem_name += self.name.split('|')[1]
-    cond_keys = list(self.cond.keys())
+    if '|' in self._name:
+      rem_name += self._name.split('|')[1]
+    cond_keys = list(self._cond.keys())
     if cond_keys:
       for key in cond_keys:
-        rem_vals.update({key: self.vals[key]})
-        rem_dims.update({key: self.dims[key]})
+        rem_vals.update({key: self[key]})
+        rem_dims.update({key: self._dims[key]})
 
-    return Dist(rem_name,
-                rem_vals,
-                rem_dims,
-                rescale(rem_prob, 1., self._pscale),
-                self._pscale)
+    return PD(rem_name, rem_vals, dims=rem_dims,
+              prob=rescale(rem_prob, 1., self._pscale),
+              pscale=self._pscale)
 
 #-------------------------------------------------------------------------------
   def __repr__(self):
     prefix = 'logp' if iscomplex(self._pscale) else 'p'
     suffix = '' if not self._issingleton else '={}'.format(self.prob)
-    return super().__repr__() + ": " + prefix + "(" + self.name + ")" + suffix
+    return prefix + "(" + self._name + ")" + suffix
+
+#-------------------------------------------------------------------------------
+  def serialise(self):
+    serialised = super().serialise()
+    short_name = self.short_name
+    serialised[short_name].update({'prob': self._prob})
+    serialised[short_name]['attrs'].update({'pscale': self._pscale})
+    return serialised
 
 #-------------------------------------------------------------------------------
```

### Comparing `probayes-0.0.3/probayes/dist_utils.py` & `probayes-0.0.4/probayes/pd_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 
-# A module to perform utility functions for Dist() instances.
+# A module to perform utility functions for PD() instances.
 
 #-------------------------------------------------------------------------------
 import collections
 import functools
 import numpy as np
-from probayes.vtypes import isscalar, issingleton, isunitsetint, isunitset
-from probayes.pscales import rescale, prod_pscale, prod_rule, iscomplex
+import h5py
+from probayes.vtypes import isscalar, issingleton, isunitsetint
+from probayes.pscales import prod_pscale, prod_rule, iscomplex
 
 #-------------------------------------------------------------------------------
 def str2key(string):
   if isinstance(string, str):
     k = string.find('=')
     if k > 0:
       return string[:k]
@@ -78,35 +79,35 @@
       else:
         string = map_key
       rekeyed.update({map_key: string})
   return rekeyed
 
 #-------------------------------------------------------------------------------
 def product(*args, **kwds):
-  """ Multiplies two or more distributions subject to the following:
+  """ Multiplies two or more PDs subject to the following:
   1. They must not share the same marginal variables. 
   2. Conditional variables must be identical unless contained as marginal from
      another distribution.
   """
-  from probayes.dist import Dist
+  from probayes.pd import PD
 
   # Check pscales, scalars, possible fasttrack
   if not len(args):
     return None
   kwds = dict(kwds)
-  pscales = [arg.ret_pscale() for arg in args]
+  pscales = [arg.pscale for arg in args]
   pscale = kwds.get('pscale', None) or prod_pscale(pscales)
-  aresingleton = [arg.ret_issingleton() for arg in args]
+  aresingleton = [arg.issingleton for arg in args]
   maybe_fasttrack = all(aresingleton) and \
                     np.all(pscale == np.array(pscales)) and \
                     pscale in [0, 1.]
 
 
   # Collate vals, probs, marg_names, and cond_names as lists
-  vals = [arg.vals for arg in args]
+  vals = [collections.OrderedDict(arg) for arg in args]
   probs = [arg.prob for arg in args]
   marg_names = [list(arg.marg.values()) for arg in args]
   cond_names = [list(arg.cond.values()) for arg in args]
 
   # Detect uniqueness in marginal keys and identical conditionals
   all_marg_keys = []
   for arg in args:
@@ -122,15 +123,15 @@
         break
       if cond_keys is None:
         cond_keys = list(arg.cond.keys())
       elif cond_keys != list(arg.cond.keys()):
         marg_keys = None
         break
       if marg_keys:  
-        are_marg_sets = np.array([isunitsetint(arg.vals[marg_key]) for
+        are_marg_sets = np.array([isunitsetint(arg[marg_key]) for
                                   marg_key in marg_keys])
         if marg_sets is None:
           if np.any(are_marg_sets):
             marg_sets = are_marg_sets
           else:
             marg_keys = None
             break
@@ -156,16 +157,16 @@
       if not cond_same:
         cond_same = True
         for name in cond_names[1:]:
           if cond_names[0] != name:
             cond_same = False
             break
     if marg_same and cond_same:
-      marg_names =  marg_names[0]
-      cond_names =  cond_names[0]
+      marg_names = marg_names[0]
+      cond_names = cond_names[0]
       prod_marg_name = ','.join(marg_names)
       prod_cond_name = ','.join(cond_names)
       prod_name = '|'.join([prod_marg_name, prod_cond_name])
       prod_vals = collections.OrderedDict()
       for i, val in enumerate(vals):
         areunitsetints = np.array([isunitsetint(_val) 
                                    for _val in val.values()])
@@ -180,18 +181,18 @@
           else:
             for j, key in enumerate(prod_vals.keys()):
               if areunitsetints[j]:
                 prod_vals.update({key: {list(prod_vals[key])[0] + \
                                         list(val[key])[0]}})
       if marg_sets is not None:
         prob, pscale = prod_rule(*tuple(probs), pscales=pscales, pscale=pscale)
-        return Dist(prod_name, prod_vals, args[0].dims, prob, pscale)
+        return PD(prod_name, prod_vals, dims=args[0].dims, prob=prob, pscale=pscale)
       else:
         prod_prob = float(sum(probs)) if iscomplex(pscale) else float(np.prod(probs))
-        return Dist(prod_name, prod_vals, {}, prob, pscale)
+        return PD(prod_name, prod_vals, prob=prod_prob, pscale=pscale)
 
   # Check cond->marg accounts for all differences between conditionals
   prod_marg = [name for dist_marg_names in marg_names \
                           for name in dist_marg_names]
   prod_marg_name = ','.join(prod_marg)
   flat_cond_names = [name for dist_cond_names in cond_names \
                           for name in dist_cond_names]
@@ -207,16 +208,16 @@
   for i, arg in enumerate(args):
     cond_set = set(cond_names[i]) - cond2marg_set
     if cond_set:
       assert prod_cond_set == cond_set, \
           "Incompatible product conditional {} for conditional set {}: ".format(
               prod_cond_set, cond_set)
     for name in cond2marg:
-      if name in arg.vals:
-        values = arg.vals[name]
+      if name in arg.keys():
+        values = arg[name]
         if not isscalar(values):
           values = np.ravel(values)
         if cond2marg_dict[name] is None:
           cond2marg_dict[name] = values
         elif not np.allclose(cond2marg_dict[name], values):
           raise ValueError("Mismatch in values for condition {}".format(name))
 
@@ -274,15 +275,15 @@
 
   prod_cdims = np.cumsum(prod_newdims)
   prod_ndims = prod_cdims[-1]
 
   # Fast-track scalar products
   if maybe_fasttrack and prod_ndims == 0:
      prob = float(sum(probs)) if iscomplex(pscale) else float(np.prod(probs))
-     return Dist(prod_name, prod_vals, {}, prob, pscale)
+     return PD(prod_name, prod_vals, prob=prob, pscale=pscale)
 
   # Reshape values - they require no axes swapping
   ones_ndims = np.ones(prod_ndims, dtype=int)
   prod_shape = np.ones(prod_ndims, dtype=int)
   scalarset = set()
   prod_dims = collections.OrderedDict()
   for i, key in enumerate(prod_keys):
@@ -294,15 +295,14 @@
       dim = prod_cdims[i]-1
       prod_dims.update({key: dim})
       re_shape[dim] = values.size
       prod_shape[dim] = values.size
       prod_vals.update({key: values.reshape(re_shape)})
   
   # Match probability axes and shapes with axes swapping then reshaping
-  prod_probs = [None] * len(args)
   for i in range(len(args)):
     prob = probs[i]
     if not isscalar(prob):
       dims = collections.OrderedDict()
       for key, val in args[i].dims.items():
         if val is not None:
           dims.update({val: prod_dims[key]})
@@ -321,25 +321,25 @@
       for dim in new_dims:
         re_shape[dim] = prod_shape[dim]
       probs[i] = prob.reshape(re_shape)
 
   # Multiply the probabilities and output the result as a distribution instance
   prob, pscale = prod_rule(*tuple(probs), pscales=pscales, pscale=pscale)
 
-  return Dist(prod_name, prod_vals, prod_dims, prob, pscale)
+  return PD(prod_name, prod_vals, dims=prod_dims, prob=prob, pscale=pscale)
 
 
 #-------------------------------------------------------------------------------
 def summate(*args):
   """ Quick and dirty concatenation """
-  from probayes.dist import Dist
+  from probayes.pd import PD
   if not len(args):
     return None
-  pscales = [arg.ret_pscale() for arg in args]
-  vals = [arg.vals for arg in args]
+  pscales = [arg.pscale for arg in args]
+  vals = [dict(arg) for arg in args]
   probs = [arg.prob for arg in args]
 
   # Check pscales are the same
   pscale = pscales[0]
   for _pscale in pscales[1:]:
     assert pscale == _pscale, \
         "Cannot summate distributions with different pscales"
@@ -354,21 +354,21 @@
       "Conditional variable names not identical across distributions: {}"
   sum_keys = marg_keys + cond_keys
   sum_name = ','.join(marg_keys)
   if cond_keys:
     sum_name += '|' + ','.join(cond_keys)
 
   # If all singleton, concatenate in dimension 0
-  if all([arg.ret_issingleton() for arg in args]):
-    unitsets = {key: isunitsetint(args[0].vals[key]) for key in sum_keys}
+  if all([arg.issingleton for arg in args]):
+    unitsets = {key: isunitsetint(args[0][key]) for key in sum_keys}
     sum_dims = {key: None if unitsets[key] else 0 for key in sum_keys}
     sum_vals = {key: 0 if unitsets[key] else [] for key in sum_keys}
     sum_prob = []
     for arg in args:
-      for key, val in arg.vals.items():
+      for key, val in arg.items():
         if unitsets[key]:
           assert isunitsetint(val), \
               "Cannot mix unspecified set and specified values"
           sum_vals[key] += list(val)[0]
         else:
           assert not isunitsetint(val), \
               "Cannot mix unspecified set and specified values"
@@ -376,43 +376,43 @@
       sum_prob.append(arg.prob)
     for key in sum_keys:
       if unitsets[key]:
         sum_vals[key] = {sum_vals[key]}
       else:
         sum_vals[key] = np.ravel(sum_vals[key])
     sum_prob = np.ravel(sum_prob)
-    return Dist(sum_name, sum_vals, sum_dims, sum_prob, pscale)
+    return PD(sum_name, sum_vals, dims=sum_dims, prob=sum_prob, pscale=pscale)
 
   # 2. all identical but in one dimension: concatenate in that dimension
   # TODO: fix the remaining code of this function below
-  sum_vals = collections.OrderedDict(args[0].vals)
+  sum_vals = collections.OrderedDict(args[0])
   sum_dims = [None] * (len(args) - 1)
   for i, arg in enumerate(args):
     if i == 0:
       continue
     for key in marg_keys:
       if sum_dims[i-1] is not None:
         continue
-      elif not arg.ret_is_singleton(key):
-        key_vals = arg.vals[key]
+      elif not arg.singleton(key):
+        key_vals = arg[key]
         if key_vals.size == sum_vals[key].size:
           if np.allclose(key_vals, sum_vals[key]):
             continue
-        sum_dims[i-1] = arg.ret_dimension(key)
+        sum_dims[i-1] = arg.dims[key]
   assert len(set(sum_dims)) > 1, "Cannot find unique concatenation axis"
   sum_dim = sum_dims[0]
   sum_dims = args[0].dims
   key = marg_keys[sum_dim]
   sum_prob = np.copy(probs[0])
   for i, val in enumerate(vals):
     if i == 0:
       continue
     sum_vals[key] = np.concatenate([sum_vals[key], val[key]], axis=sum_dim)
     sum_prob = np.concatenate([sum_prob, probs[i]], axis=sum_dim)
-  return Dist(sum_name, sum_vals, sum_dims, sum_prob, pscale)
+  return PD(sum_name, sum_vals, dims=sum_dims, prob=sum_prob, pscale=pscale)
 
 #-------------------------------------------------------------------------------
 def ismonotonic(vals):
   if issingleton(vals):
     return True
   vals = np.ravel(vals)
   is_ge = vals[1:] >= vals[:-1]
@@ -426,7 +426,95 @@
   return collections.OrderedDict(
       {key: [_dict[key] for _dict in dicts if key in _dict]
              for key in functools.reduce(set.union, [set(_dict.keys()) 
                                                      for _dict in dicts])}
                                 )
 
 #-------------------------------------------------------------------------------
+def serialise(*args):
+  from probayes import Distribution
+  from probayes import PD
+  serialised = {}
+  for arg in args:
+    if not isinstance(arg, (PD, Distribution)):
+      raise TypeError(f"Unrecogised type to serialise: {type(arg)}")
+    serialised.update(arg.serialise())
+  return serialised
+
+#-------------------------------------------------------------------------------
+def deserialise(serialised):
+  from probayes import Distribution
+  from probayes import PD
+  assert isinstance(serialised, dict), \
+    f"Dict-type serialised input expected, not {type(serialised)}"
+  dists = []
+  for dist_name, _dist_dict in serialised.items():
+    dist_dict = dict(_dist_dict)
+    attrs = {} if 'attrs' not in dist_dict else dist_dict.pop('attrs')
+    prob = None if 'prob' not in dist_dict else dist_dict.pop('prob')
+    if attrs is not None and 'pscale' in attrs:
+      pscale = attrs.pop('pscale')
+      attrs = {'pscale': pscale, 'dims': attrs}
+    import pdb; pdb.set_trace()
+    if prob is None:
+      dists.append(Distribution(dist_name, dist_dict, **attrs))
+    else:
+      dists.append(PD(dist_name, dist_dict, prob=prob, **attrs))
+  return tuple(dists)
+
+#-------------------------------------------------------------------------------
+def write_serialised(path, serialised):
+  assert isinstance(serialised, dict), \
+    f"Dict-type serialised input expected, not {type(serialised)}"
+  with h5py.File(path, 'w', libver='latest') as hdf_write:
+    for dist_name, dist_dict in serialised.items():
+      group_write = hdf_write.create_group(dist_name)
+      for key, val in dist_dict.items():
+        if key == 'attrs':
+          attrs = dist_dict['attrs']
+          for k, v in attrs.items():
+            if v is None:
+              attrs[k] = 'None'
+          group_write[key] = np.array(len(attrs))
+          group_write[key].attrs.update(attrs)
+        else:
+          if isinstance(val, np.ndarray):
+            group_write[key] = val
+          elif isinstance(val, set):
+            element = int(list(val)[0])
+            val_set = np.zeros([element], dtype='S')
+            group_write[key] = val_set
+
+#-------------------------------------------------------------------------------
+def read_serialised(path):
+  serialised = {}
+  attrs = {}
+  with h5py.File(path, 'r', libver='latest') as hdf_read:
+    dist_names = hdf_read.keys()
+    for dist_name in dist_names:
+      serialised[dist_name] = {}
+      group_read = hdf_read[dist_name]
+      for key, val in group_read.items():
+        if key == 'attrs':
+          attrs.update({dist_name: dict(val.attrs)})
+        else:
+          for key, val in group_read.items():
+            serialised[dist_name][key] = np.array(val)
+            if serialised[dist_name][key].dtype in (np.dtype('S'), np.dtype('S21'), np.dtype('|S1')):
+              serialised[dist_name][key] = set([val.size])
+      if dist_name in attrs:
+        attrs_dict  = attrs[dist_name]
+        serialised[dist_name]['attrs'] = attrs_dict
+        for k, v in attrs_dict.items():
+          if v == 'None':
+            serialised[dist_name]['attrs'][k] = None
+  return serialised
+
+#-------------------------------------------------------------------------------
+def write_dist(path, *args):
+  return write_serialised(path, serialise(*args))
+
+#-------------------------------------------------------------------------------
+def read_dist(path):
+  return deserialise(read_serialised(path))
+
+#-------------------------------------------------------------------------------
```

### Comparing `probayes-0.0.3/probayes/domain.py` & `probayes-0.0.4/probayes/rv.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,557 +1,590 @@
-"""
-A domain defines a variable set over which a function can be defined. It thus
-comprises a name and variable set. The function itself is not supported although
-invertible variable transformations are.
-"""
+""" Random variable module """
 
 #-------------------------------------------------------------------------------
-import numpy as np
 import collections
-from probayes.vtypes import eval_vtype, isunitsetint, isscalar, \
-                        revtype, uniform, VTYPES
-from probayes.func import Func
+import warnings
+import numpy as np
+import sympy
+from probayes.variable import Variable, DEFAULT_VNAME
+from probayes.prob import Prob
+from probayes.vtypes import uniform, VTYPES, isscalar, \
+                        isunitset, isunitsetint, isunitsetfloat, issingleton
+from probayes.pscales import rescale
+from probayes.expression import Expression
+from probayes.sympy_prob import bernoulli_prob, bernoulli_sfun
+from probayes.rv_utils import uniform_prob, matrix_cond_sample, \
+                          lookup_square_matrix
+from probayes.distribution import Distribution
+from probayes.pd import PD
 
-#-------------------------------------------------------------------------------
-DEFAULT_VSET = {False, True}
+"""
+A random variable is a triple (x, A_x, P_x) defined for an outcome x for every 
+possible realisation defined over the alphabet set A_x with probabilities P_x.
+It therefore requires a name for x (id), a variable alphabet set (vset), and its 
+associated probability distribution function (prob).
+"""
 
 #-------------------------------------------------------------------------------
-class Domain:
-  """ Base class for probayes.RV although this class can be called itself.
-  A domain defines a variable set over which a function can be defined. It
-  therefore needs a name and corresponding variable. While this class
-  does not support respective probability density functions (use RV for that), 
-  it does include an optional to specify an invertible monotic variable 
-  transformation function:
+class RV (Variable, Prob):
+  """ A random variable is a variable with a defined probability function.
+  It therefore inherits from classes Variable and and Prob. Each instance therefore 
+  requires a name, a variable set, and probability function. Additionally RV
+  supports transitional probabilities the cdf/icdf equivalents specified using
+  RV.set_tran() and RV.set_tfun() equivalents, and accessed using RV.step().
 
   :example:
   >>> import numpy as np
   >>> import probayes as pb
-  >>> scalar = pb.Domain('scalar', [-np.inf, np.inf], vtype=float)
-  >>> scalar.set_mfun((np.exp, np.log))
-  >>> print(scalar.ret_limits())
-  [ 0. inf]
+  >>> var = pb.RV('var', vtype=bool)
+  >>> var.set_tran(np.array([0.2, 0.8, 0.3, 0.7]).reshape(2,2,))
+  >>> step = var.step()
+  >>> print(step.prob)
+  [[0.2 0.8]
+   [0.3 0.7]]
   """
 
-  # Public
-  delta = None       # A named tuple generator
-                    
-  # Protected       
-  _name = "var"      # Name of the variable
-  _vset = None       # Variable set (array or 2-length tuple range)
-  _vtype = None      # Variable type
-  _mfun = None       # 2-length tuple of monotonic mutually inverting functions
-  _lims = None       # Numpy array of bounds of vset
-  _limits = None     # Transformed self._lims
-  _length = None     # Difference in self._limits
-  _inside = None     # Lambda function for defining inside vset
-  _delta = None      # Default delta operation
-  _delta_args = None # Optional delta arguments 
-  _delta_kwds = None # Optional delta keywords 
+  # Protected
+  _tran = None          # Transitional prob - can be a matrix
+  _tfun = None          # Like pfun for transitional conditionals
+  _is_stochastic = True # Flag of whether stochastic
+
+  # Private
+  __def_prob = None   # Flag to denote prob is defaulted
+  __sym_tran = None   # Flag to denote symmetric transitional
+  __prime_key = None  # Modified-string to denote prime key for variable
 
 #-------------------------------------------------------------------------------
-  def __init__(self, name=None,
+  def __init__(self, name, 
                      vset=None, 
                      vtype=None,
-                     mfun=None,
+                     prob=None,
                      *args,
                      **kwds):
-    """ Initialiser sets name, vset, and mfun:
+    """ Initialises a random variable combining Variable and Prob initialisation
+    except invertible monotonic must be specified separately using set_ufun().
 
     :param name: Name of the domain - string as valid identifier.
-    :param vset: variable set over which domain defined (see set_vset).
+    :param vset: variable set over which domain defined (see Variable.vset).
     :param vtype: variable type (bool, int, or float).
-    :param mfun: two-length tuple of monotonic functions (see set_mfun).
-    :param *args: args to pass to mfun functions.
-    :param **kwds: kwds to pass to mfun functions.
-
-    Every Domain instance offers a factory function for delta specifications:
-
-    :example:
-    >>> import numpy as np
-    >>> import probayes as pb
-    >>> x = pb.Domain('x', [-np.inf, np.inf], vtype=float)
-    >>> dx = x.delta(0.5)
-    >>> print(x.apply_delta(1.5, dx))
-    2.0
-    """
-    self.set_name(name)
-    self.set_vset(vset, vtype)
-    self.set_mfun(mfun, *args, **kwds)
-    self.set_delta()
-
-#-------------------------------------------------------------------------------
-  def set_name(self, name):
-    """ Sets name of variable over which domain is defined:
-
-    :param name: Name of the domain - string as valid identifier.
-    """
-    # Identifier name required
-    self._name = name
-    assert isinstance(self._name, str), \
-        "Mandatory variable name must be a string: {}".format(self._name)
-    assert self._name.isidentifier(), \
-        "Variable name must ba a valid identifier: {}".format(self._name)
-    self.delta = collections.namedtuple('ð', [self._name])
-
-#-------------------------------------------------------------------------------
-  def set_vset(self, vset=None, vtype=None):
-    """ Sets the variable set and variable type over which the domain is defined.
-
-    :param vset: variable set over which domain defined (default [False, True])
-    :param vtype: variable type (bool, int, or float; default bool).
-
-    For non-float vtypes, vset may be a list, set, range, or NumPy array.
-
-    For float vtypes, vset represents limits in the form:
-
-    [lower, upper] - inclusive of both lower of upper values
-    [(lower), upper] - exclusive of lower and inclusive of upper.
-    [lower, (upper)] - inclusive of lower and exclusive of upper.
-    [(lower), (upper)] - exclusive of both lower and upper values.
-
-    The last case may also set using a simple two-value tuple:
-
-    :example:
-    >>> import probayes as pb
-    >>> scalar = pb.Domain('scalar')
-    >>> scalar.set_vset((1, 2), vtype=float)
-    >>> print(scalar.ret_vset())
-    [(1.0,), (2.0,)]
-    """
-
-    # Default vset to nominal
-    if vset is None: 
-      vset = list(DEFAULT_VSET)
-    elif isinstance(vset, (set, range)):
-      vset = sorted(vset)
-    elif np.isscalar(self._vset):
-      vset = [self._vset]
-    elif isinstance(vset, tuple):
-      assert len(vset) == 2, \
-          "Tuple vsets contain pairs of values, not {}".format(vset)
-      vset = sorted(vset)
-      vset = [(vset[0],), (vset[1],)]
-    elif isinstance(vset, np.ndarray):
-      vset = np.sort(vset).tolist()
-    else:
-      assert isinstance(vset, list), \
-          "Unrecognised vset specification: {}".format(vset)
-
-    # At this point, vset can only be a list, but may contain tuples
-    aretuples = ([isinstance(_vset, tuple) for _vset in vset])
-    if not any(aretuples):
-      if vtype is None:
-        vset = np.array(vset)
-        vtype = eval_vtype(vset)
-      else:
-        vset = np.array(vset, dtype=vtype)
-    else:
-      if vtype is not None:
-        assert vtype in VTYPES[float], \
-            "Bounded variables supported only for float vtypes, not {}".\
-            format(vtype)
-      vtype = float
-      assert len(vset) == 2, \
-          "Unrecognised set specification: {}".vset
-      for i in range(len(vset)):
-        if isinstance(vset[i], tuple):
-          assert len(vset[i]) == 1, \
-              "Unrecognised set specification: {}".vset[i]
-          vset[i] = vtype(vset[i][0])
-    self._vset = vset
-    for i, istuple in enumerate(aretuples):
-      if istuple:
-        self._vset[i] = self._vset[i],
-    self._vtype = eval_vtype(vtype)
-    self._eval_lims()
-
-#-------------------------------------------------------------------------------
-  def _eval_lims(self):
-    """ Evaluates untransformed (self._lims) and transformed (self._limits) 
-
-    :returns: the length of the domain.
-    """
-    self._lims = None
-    self._limits = None
-    self._length = None
-    self._inside = None
-    
-    if self._vset is None:
-      return self._length
-
-    if self._vtype not in VTYPES[float]:
-      self._lims = np.array([min(self._vset), max(self._vset)])
-      self._limits = self._lims
-      self._length = True if self._vtype in VTYPES[bool] else len(self._vset)
-      self._inside = lambda x: np.isin(x, self._vset, assume_unique=True)
-      return self._length
-
-    """ Evaluates the limits from vset assuming vtype is set """
-    # Set up limits and inside function if float
-    if any([isinstance(_vset, tuple) for _vset in self._vset]):
-      lims = np.concatenate([np.array(_vset).reshape([1]) 
-                             for _vset in self._vset])
-    else:
-      lims = np.array(self._vset)
-    assert len(lims) == 2, \
-        "Floating point vset must be two elements, not {}".format(self._vset)
-    if lims[1] < lims[0]:
-      vset = vset[::-1]
-      self._vset = vset
-    self._lims = np.sort(lims)
-    self._limits = self._lims if self._mfun is None \
-                   else self.ret_mfun(0)(self._lims)
-    self._length = max(self._limits) - min(self._limits)
-
-    # Now set inside function
-    if not isinstance(self._vset[0], tuple) and \
-        not isinstance(self._vset[1], tuple):
-      self._inside = lambda x: np.logical_and(x >= self._lims[0],
-                                              x <= self._lims[1])
-    elif not isinstance(self._vset[0], tuple) and \
-        isinstance(self._vset[1], tuple):
-      self._inside = lambda x: np.logical_and(x >= self._lims[0],
-                                              x < self._lims[1])
-    elif isinstance(self._vset[0], tuple) and \
-        not isinstance(self._vset[1], tuple):
-      self._inside = lambda x: np.logical_and(x > self._lims[0],
-                                              x <= self._lims[1])
-    else:
-      self._inside = lambda x: np.logical_and(x > self._lims[0],
-                                              x < self._lims[1])
-    return self._length
-
-#-------------------------------------------------------------------------------
-  def set_mfun(self, mfun=None, *args, **kwds):
-    """ Sets a monotonic invertible tranformation for the domain as a tuple of
-    two functions in the form (transforming_function, inverse_function) 
-    operating on the first argument with optional further args and kwds.
-
-    :param mfun: two-length tuple of monotonic functions.
-    :param *args: args to pass to mfun functions.
-    :param **kwds: kwds to pass to mfun functions.
-
-    Support for this transformation is only valid for float-type vtypes.
+    :param prob : uncallable or callable probability expression (see set_prob).
+    :param *args: optional arguments to pass if prob is callable.
+    :param **kwds: optional keywords to pass if prob is callable.
     """
-    self._mfun = mfun
-    if self._mfun is None:
-      return
-
-    assert self._vtype in VTYPES[float], \
-        "Values transformation function only supported for floating point"
-    message = "Input mfun be a two-sized tuple of callable functions"
-    assert isinstance(self._mfun, tuple), message
-    assert len(self._mfun) == 2, message
-    assert callable(self._mfun[0]), message
-    assert callable(self._mfun[1]), message
-    self._mfun = Func(self._mfun, *args, **kwds)
-    self._eval_lims()
-
-#-------------------------------------------------------------------------------
-  def set_delta(self, delta=None, *args, **kwds):
-    """ Sets the default delta operation for the domain.
-
-    :param delta: a callable or uncallable argument (see below)
-    :param *args: args to pass if delta is callable.
-    :param **kwds: kwds to pass if delta is callable (except scale and bound)
-
-    The first argument delta may be:
-
-    1. A callable function (operating on the first term).
-    2. A Domain.delta instance (this defaults all Domain deltas).
-    3. A scalar that may or may not be contained in a container:
-      a) No container - the scalar is treated as a fixed delta.
-      b) List - delta is uniformly sampled from [-scalar to +scalar].
-      c) Tuple - operation is +/-delta within the polarity randomised
-
-    Two reserved keywords can be passed for specifying (default False):
-      'scale': Flag to denote scaling deltas to Domain lengths
-      'bound': Flag to constrain delta effects to Domain bounds
-    """
-    self._delta = delta
-    self._delta_args = args
-    self._delta_kwds = dict(kwds)
-    if self._delta is None:
-      return
-    elif callable(self._delta):
-      self._delta = Func(self._delta, *args, **kwds)
-      return
 
-    # Default scale and bound
-    if 'scale' not in self._delta_kwds:
-      self._delta_kwds.update({'scale': False})
-    if 'bound' not in self._delta_kwds:
-      self._delta_kwds.update({'bound': False})
+    Variable.__init__(self, name, vtype, vset)
+    Prob.__init__(self, prob, *args, **kwds)
+    self._tran, self._tfun = None, None
 
 #-------------------------------------------------------------------------------
-  def ret_name(self):
-    """ Returns the domain name """
+  @property
+  def name(self):
     return self._name
 
+  @name.setter
+  def name(self, name=DEFAULT_VNAME):
+    self._name = name
+    self._Delta = collections.namedtuple('ð', [self._name])
+    self.__prime_key = self._name + "'"
+
 #-------------------------------------------------------------------------------
-  def ret_vset(self):
-    """ Returns the variable set """
+  @property
+  def vset(self):
     return self._vset
 
-#-------------------------------------------------------------------------------
-  def ret_vtype(self):
-    """ Returns the variable type """
-    return self._vtype
+  @Variable.vset.setter
+  def vset(self, vset=None):
+    Variable.vset.fset(self, vset)
+    if self.__def_prob:
+      self._prob = None
+      self._default_prob()
 
 #-------------------------------------------------------------------------------
-  def ret_mfun(self, index=None):
-    r""" Returns the monotonic invertible function(s). If not specified, then
-    an identity lambda is passed.
-    
-    :param index: optional index $i$ if to isolate the $i$th function.
+  @property
+  def vtype(self):
+    return self._vtype
 
-    :return: monotonic inverible function(s).
+  @Variable.vtype.setter
+  def vtype(self, vtype=None):
+    Variable.vtype.fset(self, vtype)
+    if self.__def_prob:
+      self._prob = None
+      self._default_prob()
+
+#-------------------------------------------------------------------------------
+  @property
+  def prob(self):
+    return self._prob
+
+  @property
+  def def_prob(self):
+    return self.__def_prob
+
+  def set_prob(self, prob=None, *args, **kwds):
+    """ Sets the probability and pscale with optional arguments and keywords.
+
+    :param prob: may be a scalar, array, or callable function.
+    :param *args: optional arguments to pass if prob is callable.
+    :param **kwds: optional keywords to pass if prob is callable.
+
+    'pscale' is a reserved keyword. See Prob.pscale for explanation of how 
+    pscale is used.
+    """
+    super().set_prob(prob, *args, **kwds)
+    if self._prob is None:
+      self._default_prob()
+    else:
+      self.__def_prob = False
 
-    .. warnings:: the flexibility of this interface comes at the cost of requiring
-                  a maximum of ret_mfun() being called per line of code.
-    """
-    if self._mfun is None:
-      return lambda x:x
-    if index is None:
-      return self._mfun
-    return self._mfun[index]
+    # Check uncallable probabilities commensurate with self._vset
+    if self._vset is not None and \
+        not self.callable and not self.isscalar:
+      assert len(self._prob) == len(self._vset), \
+          "Probability of length {} incommensurate with Vset of length {}".format(
+              len(self._prob), len(self._vset))
 
-#-------------------------------------------------------------------------------
-  def ret_lims(self):
-    """ Returns the untransformed limits """
-    return self._lims
+    # Reassign non-0.5 Bernoulli probabilities to a formal distribution
+    if self._vtype in VTYPES[bool] and self.isscalar:
+      prob = float(self._prob)
+      if not np.isclose(prob, 0.5):
+        super().set_prob(bernoulli_prob(self.icon, bias=prob))
+        super().set_sfun(bernoulli_sfun, bias=prob)
 
 #-------------------------------------------------------------------------------
-  def ret_limits(self):
-    """ Returns the transformed limits """
-    return self._limits
-
-#-------------------------------------------------------------------------------
-  def ret_length(self):
-    """ Returns the length of the domain """
-    return self._length
+  def _default_prob(self):
+    """ Defaults unspecified probabilities to uniform over self._vset.
+    This will not override a previously specified non-default probability.
+    """
 
-#-------------------------------------------------------------------------------
-  def ret_delta(self):
-    """ Returns the delta function if set """
-    return self._delta
+    if self._prob is not None and not self.__def_prob:
+      return
+    prob = rescale(self._nlhv, 'log', self._pscale)
+    if self._ufun is not None and self.no_ucov:
+      prob = prob + sympy.log(self._ufun.derinv.expr) if self._logp else \
+             prob * self._ufun.derinv.expr
+    super().set_prob(prob)
+    self.set_tran(prob)
+    self.__def_prob = True
+
+#-------------------------------------------------------------------------------
+  def set_pfun(self, pfun=None, *args, **kwds):
+    """ Sets a two-length tuple of functions that should correspond to the
+    (cumulative probability function, inverse cumulative function) with respect
+    to the callable function set by set_prob(). It is necessary to set these
+    functions if sampling variables with non-flat distributions.
+
+    :param pfun: two-length tuple of callable functions
+    :param *args: arguments to pass to callable functions
+    :param **kwds: keywords to pass to callable functions
+    """
+    super().set_pfun(pfun, *args, **kwds)
+    if self._ufun is None or self._pfun is None:
+      return
+    assert self._ufun is None, \
+      "Cannot assign non-uniform distribution alongside " + \
+      "values transformation functions"
 
 #-------------------------------------------------------------------------------
-  def eval_vals(self, values=None):
-    r""" Evaluates value(s) belonging to the domain.
-
-    :param values: None, set of a single integer, array, or scalar.
+  def set_ufun(self, ufun=None, *args, **kwds):
+    """ Sets a monotonic invertible tranformation for the domain as a tuple of
+    two functions in the form (transforming_function, inverse_function) 
+    operating on the first argument with optional further args and kwds.
 
-    :return: a NumPy array of the values in accordance to the following:
+    :param ufun: two-length tuple of monotonic functions.
+    :param *args: args to pass to ufun functions.
+    :param **kwds: kwds to pass to ufun functions.
 
-    If values is a NumPy array, it is returned unchanged.
+    Support for this transformation is only valid for float-type vtypes.
+    """
+    super().set_ufun(ufun, *args, **kwds)
+    if self._ufun is None:
+      return
 
-    If values is None, it defaults to the entire variable set (vset) if not
-    the variable type vtype is not float; otherwise a single scalar within the
-    vset is randomly evaluated (see below).
+    # Recalibrate defaulted probabilities for floating point vtypes
+    if self._vtype in VTYPES[float]:
+      self._default_prob()
+
+    # Assert pfun is unspecified
+    assert self._pfun is None, \
+      "Cannot assign univariate function alongside CDF/ICDF specification"
+
+#-------------------------------------------------------------------------------
+  @property
+  def tran(self):
+    """ Returns the transitional probability expression if specified """
+    return self._tran
+
+  def set_tran(self, tran=None, *args, **kwds):
+    """ Sets a transitional function as a conditional probability. This can
+    be specified numerically or one or two callable functions.
+
+    :param tran: conditional scalar, array, or callable function (see below).
+    :param *args: args to pass to tran functions.
+    :param **kwds: kwds to pass to tran functions.
+
+    If tran is a scalar, array, or callable function, then the transitional
+    conditionality is treated as symmetrical. If tran is a two-length tuple,
+    then assymetry is assumed in the form: (p[var'|var], p[var|var']).
+
+    If intending to sample from a transitional conditional probability density
+    function, the corresponding (CDF, ICDF) must be set using set_tfun().
+    """
+    self._tran = tran
+    self.__sym_tran = None
+    if self._tran is None:
+      return
+    self._tran = Expression(self._tran, *args, **kwds)
+    self.__sym_tran = not self._tran.ismulti
+    if self._tran.callable or self._tran.isscalar:
+      return
+    assert self._vtype not in VTYPES[float],\
+      "Scalar or callable transitional required for floating point data types"
+    tran = self._tran() if self.__sym_tran else self._tran[0]()
+    message = "Transition matrix must a square 2D Numpy array " + \
+              "covering variable set of size {}".format(len(self._vset))
+    assert isinstance(tran, np.ndarray), message
+    assert tran.ndim == 2, message
+    assert np.all(np.array(tran.shape) == len(self._vset)), message
+    self.__sym_tran = np.allclose(tran, tran.T)
+
+#-------------------------------------------------------------------------------
+  @property
+  def tfun(self):
+    """ Returns the transitional CDF/ICDF expression if specified """
+    return self._tfun
+
+  def set_tfun(self, tfun=None, *args, **kwds):
+    """ Sets a two-length tuple of functions that should correspond to the
+    (cumulative probability function, inverse cumulative function) with respect
+    to the callable function set by set_tran(). It is necessary to set these
+    functions if conditionally sampling variables with continuous distributions.
+
+    :param tfun: two-length tuple of callable functions
+    :param *args: arguments to pass to tfun functions
+    :param **kwds: keywords to pass to tfun functions
+    """
+    self._tfun = tfun if tfun is None else Expression(tfun, *args, **kwds)
+    if self._tfun is None:
+      return
+    assert self._tfun.ismulti, "Tuple of two functions required"
 
-    If values is a set containing a single integer (i.e. $\{n\}$), , then the 
-    output depends on the number $n$:
+#-------------------------------------------------------------------------------
+  def evaluate(self, values, use_pfun=True):
+    """ Evaluates value(s) belonging to the domain of the variable.
 
-    If positive ($n$), then $n$ values are uniformly sampled.
-    If zero ($n=0$), then a scalar value is randomly sampled.
-    if negative($-n$), then $n$ values are randomly sampled.
+    :param values: None, set of a single integer, array, or scalar.
+    :param use_pfun: boolean flag to make use of pfun if previously set.
 
-    For non-float types, the values are evaluated from by ordered (if $n>0) or 
-    random permutations of vset. For float types, then uniformly sampled is
-    performed in accordance for any transformations set by Domain.set_mfun().
+    :return: a NumPy array of the values (see Variable.evaluate()):
     """
+    use_pfun = use_pfun and self._pfun is not None and isunitsetint(values)
 
-    # Default to arrays of complete sets
+    # If not using pfun while random sampling, we use sfun for booleans
+    if not use_pfun:
+      if self._vtype in VTYPES[bool] and hasattr(self._sfun, 'expr'):
+        if isunitsetint(values) and self._sfun.expr == bernoulli_sfun:
+          number = list(values)[0]
+          if not number or number < 0:
+            number = number if not number else -number
+            return Distribution(self._name, 
+                                {self.name: self._sfun[None](number)})
+      return super().evaluate(values)
+
+    # Evaluate values from inverse cdf bounded within cdf limits
+    number = list(values)[0]
+    assert self.isfinite, \
+        "Cannot evaluate {} values for bounds: {}".format(values, self._ulims)
+    lims = self.pfun[0](self._ulims)
+    values = uniform(
+                     lims[0], lims[1], number, 
+                     isinstance(self._vset[0], tuple),
+                     isinstance(self._vset[1], tuple)
+                    )
+    return Distribution(self._name, {self.name: self.pfun[1](values)})
+
+#-------------------------------------------------------------------------------
+  def eval_prob(self, values=None):
+    """ Evaluates the probability inputting optional args for callable cases
+
+    :param values: values of the variable used for evaluating probabilities.
+    :param *args: optional arguments for callable probability objects.
+    :param **kwds: optional arguments to include pscale for rescaling.
+
+    :return: evaluated probabilities
+    """
+    values = values[self.name] if isinstance(values, dict) else values
+    if not self.isscalar:
+      return super().eval_prob(values)
+    return uniform_prob(values, 
+                        prob=float(self._prob), 
+                        inside=self._inside,
+                        pscale=self._pscale)
+
+#-------------------------------------------------------------------------------
+  def eval_dist_name(self, values, suffix=None):
+    """ Evaluates a distribution name for a probability distribution based on
+    the values set in the first input argument with an optional suffix. """
+    name = self._name if not suffix else self._name + suffix
     if values is None:
-      if self._vtype in VTYPES[float]:
-        values = {0}
-      else:
-        return np.array(list(self._vset), dtype=self._vtype)
-
-    # Sets may be used to sample from support sets
-    if isunitsetint(values):
-      number = list(values)[0]
-
-      # Non-continuous
-      if self._vtype not in VTYPES[float]:
-        values = np.array(list(self._vset), dtype=self._vtype)
-        if not number:
-          values = values[np.random.randint(0, len(values))]
-        else:
-          if number > 0:
-            indices = np.arange(number, dtype=int) % self._length
-          else:
-            indices = np.random.permutation(-number, dtype=int) % self._length
-          values = values[indices]
-        return values
-       
-      # Continuous
-      else:
-        assert np.all(np.isfinite(self._limits)), \
-            "Cannot evaluate {} values for bounds: {}".format(
-                values, self._limits)
-        values = uniform(self._limits[0], self._limits[1], number, 
-                           isinstance(self._vset[0], tuple), 
-                           isinstance(self._vset[1], tuple)
-                        )
-
-      # Only use mfun when isunitsetint(values)
-      if self._mfun:
-        return self.ret_mfun(1)(values)
-    return values
+      dist_str = name
+    elif np.isscalar(values):
+      dist_str = "{}={}".format(name, values)
+    else:
+      dist_str = name + "=[]"
+    return dist_str
 
 #-------------------------------------------------------------------------------
-  def __call__(self, values=None):
-    """ See Domain.eval_vals() 
-
-    :example:
+  def eval_step(self, pred_vals, succ_vals, reverse=False):
+    """ Evaluates a successive values from previous values with an optional
+    direction reversal flag, outputting a three-length tuple that includes the
+    successive values in the first argument.
+
+    :param pred_vals: predecessor values (NumPy array).
+    :param succ_vals: succecessor values (see step()).
+    :param reverse: boolean flag (default False) to reverse direction.
+
+    :return vals: a dictionary including both predecessor and successor values.
+    :return dims: a dictionary with dimension indices for the values in vals.
+    :return kwargs: a dictionary that includes optional keywords for eval_tran()
+    """
+
+    if succ_vals is None:
+      assert self._tran is not None, "No transitional function specified"
+    if isinstance(pred_vals, dict):
+      pred_vals = pred_vals[self.name]
+    kwargs = dict() # to pass over to eval_tran()
+    if succ_vals is None:
+      if self._delta is None:
+        succ_vals = {0} if isscalar(pred_vals) else pred_vals
+      else:
+        delta = self.eval_delta()
+        succ_vals = self.apply_delta(pred_vals, delta)
 
-    >>> import numpy as np
-    >>> import probayes as pb
-    >>> freq = pb.Domain('freq', [1,8], vtype=float)
-    >>> freq.set_mfun((np.log, np.exp))
-    >>> print(freq({4})
-    [1. 2. 4. 8.]
-    """
-    return self.eval_vals(values)
-
-#------------------------------------------------------------------------------- 
-  def eval_delta(self, delta=None):
-    """ Evaluates the value(s) of a delta operation without applying them.
-
-    :param delta: delta value(s) to offset (see Domain.apply_delta).
-    :return: the evaluated delta offset values.
-    :rtype Domain.delta()
-
-    If delta is not entered, then the default set by Domain.set_delta() is used.
-    """
-    delta = delta or self._delta
-    if delta is None:
-      return None
-    if isinstance(delta, Func):
-      if delta.ret_callable():
-        return delta
-      delta = delta()
-    if isinstance(delta, self.delta):
-      delta = delta[0]
-    orand = isinstance(delta, tuple)
-    urand = isinstance(delta, list)
-    if orand:
-      assert len(delta) == 1, "Tuple delta must contain one element"
-      delta = delta[0]
-      if self._vtype not in VTYPES[bool]:
-        delta = delta if np.random.uniform() > 0.5 else -delta
-    elif urand:
-      assert len(delta) == 1, "List delta must contain one element"
-      delta = delta[0]
-      if self._vtype in VTYPES[bool]:
-        pass
-      elif self._vtype in VTYPES[int]:
-        delta = np.random.randint(-delta, delta)
+    #---------------------------------------------------------------------------
+    def _reshape_vals(pred, succ):
+      dims = {}
+      ndim = 0
+
+      # Now reshape the values according to succ > prev dimensionality
+      if issingleton(succ):
+        dims.update({self._name+"'": None})
       else:
-        delta = np.random.uniform(-delta, delta)
-    assert isscalar(delta), "Unrecognised delta type: {}".format(delta)
-    if delta == self._delta and self._delta_kwds['scale']:
-      assert np.isfinite(self._length), "Cannot scale by infinite length"
-      delta *= self._length
-    return self.delta(delta)
-
-#------------------------------------------------------------------------------- 
-  def apply_delta(self, values, delta=None, bound=None):
-    """ Applies delta operation  to values optionally contrained by bounds.
-
-    :param values: Numpy array values to apply.
-    :param delta: delta value(s) to offset to the values
-    :param bound: optional argument to contrain outputs.
-
-    :return: Returns the values following the delta operation.
-
-    If delta is not entered, then the default set by Domain.set_delta() is used.
-    Delta may be a scalar or a single scalar value contained in a tuple or list.
-
-    1. A scalar value: is summated to values (transformed if mfun is specified).
-    2. A tuple: the polarity of the scalar value is randomised for the delta.
-    3. A list: the delta is uniformly sampled in the range [0, scalar].
-    """
-
-    # Call eval_delta() if values is a list and return values if delta is None
-    delta = delta or self._delta
-    if isinstance(delta, Func):
-      if delta.ret_callable():
-        return delta(values)
-      delta = delta()
-    elif self._vtype not in VTYPES[bool]:
-      if isinstance(delta, (list, tuple)):
-        delta = self.eval_delta(delta)
-    if isinstance(delta, self.delta):
-      delta = delta[0]
-    if delta is None:
-      return values
-
-    # Apply the delta, treating bool as a special case
-    if self._vtype in VTYPES[bool]:
-      orand = isinstance(delta, tuple)
-      urand = isinstance(delta, list)
-      if orand or urand:
-        assert len(delta) == 1, "Tuple/list delta must contain one element"
-        delta = delta[0]
-        if isscalar(values) or orand:
-          vals = values if delta > np.random.uniform() > 0.5 \
-                 else np.logical_not(values)
-        else:
-          flip = delta > np.random.uniform(size=values.shape)
-          vals = np.copy(values)
-          vals[flip] = np.logical_not(vals[flip])
+        dims.update({self._name+"'": ndim})
+        ndim += 1
+      if issingleton(pred):
+        dims.update({self._name: None})
       else:
-        vals = np.array(values, dtype=int) + np.array(delta, dtype=int)
-        vals = np.array(np.mod(vals, 2), dtype=bool)
-    elif self._mfun is None:
-      vals = values + delta
+        dims.update({self._name: ndim})
+        ndim += 1
+
+      if ndim == 2: # pred_vals distributed along inner dimension:
+        pred = pred.reshape([1, pred.size])
+        succ = succ.reshape([succ.size, 1])
+      return pred, succ, dims
+
+    #---------------------------------------------------------------------------
+    # Scalar treatment is the most trivial and ignores reverse
+    if self._tran is None or self._tran.isscalar:
+      if isunitsetint(succ_vals):
+        succ_vals = self.evaluate(succ_vals, use_pfun=False)[self._name]
+      elif isunitsetfloat(succ_vals):
+        assert self._vtype in VTYPES[float], \
+            "Inverse CDF sampling for scalar probabilities unavailable for " + \
+            "{} data type".format(self._vtype)
+        cdf_val = list(succ_vals)[0]
+        lo, hi = min(self._limits), max(self._limits)
+        succ_val = lo*(1.-cdf_val) + hi*cdf_val
+        if self._ufun is not None:
+          succ_val = self.ufun[-1](succ_val)
+
+      prob = self._tran() if self._tran is not None else None
+      pred_vals, succ_vals, dims = _reshape_vals(pred_vals, succ_vals)
+                  
+    # Handle discrete non-callables
+    elif not self._tran.callable:
+      if reverse and not self._tran.ismulti and not self.__sym_tran:
+        warnings.warn("Reverse direction called from asymmetric transitional")
+      prob = self._tran() if not self._tran.ismulti else \
+             self._tran[int(reverse)]()
+      if isunitset(succ_vals):
+        succ_vals, pred_idx, succ_idx = matrix_cond_sample(pred_vals, 
+                                                           succ_vals, 
+                                                           prob=prob, 
+                                                           vset=self._vset) 
+        kwargs.update({'pred_idx': pred_idx, 'succ_idx': succ_idx})
+      pred_vals, succ_vals, dims = _reshape_vals(pred_vals, succ_vals)
+
+    # That just leaves callables
     else:
-      transformed_vals = self.ret_mfun(0)(values) + delta
-      vals = self.ret_mfun(1)(transformed_vals)
-    vals = revtype(vals, self._vtype)
-
-    # Apply bounds
-    if bound is None:
-      bound = False if 'bound' not in self._delta_kwds \
-             else self._delta_kwds['bound']
-    if not bound:
-      return vals
-    maybe_bounce = [False] if self._vtype not in VTYPES[float] else \
-                   [isinstance(self._vset[0], tuple), 
-                    isinstance(self._vset[1], tuple)]
-    if not any(maybe_bounce):
-      return np.maximum(self._lims[0], np.minimum(self._lims[1], vals))
-
-    # Bouncing scalars and arrays without and with boolean indexing respectively
-    if isscalar(vals):
-      if all(maybe_bounce):
-        if not self._inside(vals):
-          vals = values
-      elif maybe_bounce[0]:
-        if vals < self._lims[0]:
-          vals = values
-        else:
-          vals = np.minimum(self._lims[1], vals)
-      else:
-        if vals > self._lims[1]:
-          vals = values
+      kwds = {self._name: pred_vals}
+      if isunitset(succ_vals):
+        assert self._tfun is not None, \
+            "Conditional sampling requires setting CDF and ICDF " + \
+            "conditional functions using rv.set.tfun()"
+        assert isscalar(pred_vals), \
+            "Successor sampling only possible with scalar predecessors"
+        succ_vals = list(succ_vals)[0]
+        if type(succ_vals) in VTYPES[int] or type(succ_vals) in VTYPES[np.uint]:
+          lo, hi = min(self._ulims), max(self._ulims)
+          kwds.update({self._name+"'": np.array([lo, hi], dtype=float)})
+          lohi = self._tfun[0](**kwds)
+          lo, hi = float(min(lohi)), float(max(lohi))
+          succ_vals = uniform(lo, hi, succ_vals,
+                              isinstance(self._vset[0], tuple),
+                              isinstance(self._vset[1], tuple))
         else:
-          vals = np.maximum(self._lims[0], vals)
+          succ_vals = np.atleast_1d(succ_vals)
+        kwds.update({self._name: pred_vals,
+                     self._name+"'": succ_vals})
+        succ_vals = self._tfun[1](**kwds)
+      elif not isscalar(succ_vals):
+        succ_vals = np.atleast_1d(succ_vals)
+      pred_vals, succ_vals, dims = _reshape_vals(pred_vals, succ_vals)
+
+    vals = collections.OrderedDict({self._name+"'": succ_vals,
+                                    self._name: pred_vals})
+    kwargs.update({'reverse': reverse})
+    return vals, dims, kwargs
+
+#-------------------------------------------------------------------------------
+  def eval_tran(self, vals, **kwargs):
+    """ Evaluates the transitional conditional probability for the dictionary 
+    arguments in vals with optional keywords in **kwargs.
+    """
+    reverse = False if 'reverse' not in kwargs else kwargs['reverse']
+    pred_vals, succ_vals = vals[self._name], vals[self._name+"'"]
+    pred_idx = None if 'pred_idx' not in kwargs else kwargs['pred_idx'] 
+    succ_idx = None if 'succ_idx' not in kwargs else kwargs['succ_idx'] 
+    cond = None
+
+    # No transitional means no conditional
+    if self._tran is None:
+      pass
+
+    # Scalar treatment is the most trivial and ignores reverse
+    elif self._tran.isscalar:
+      prob = None if self._tran is None else self._tran()
+      cond = uniform_prob(pred_vals,
+                          succ_vals, 
+                          prob=float(prob), 
+                          inside=self._inside) 
+                  
+
+    # Handle discrete non-callables
+    elif not self._tran.callable:
+      prob = self._tran() if not self._tran.ismulti else \
+             self._tran[int(reverse)]()
+      cond = lookup_square_matrix(pred_vals,
+                                  succ_vals, 
+                                  sq_matrix=prob, 
+                                  vset=self._vset,
+                                  col_idx=pred_idx,
+                                  row_idx=succ_idx) 
+
+
+    # That just leaves callables
     else:
-      if all(maybe_bounce):
-        outside = np.logical_not(self._inside(vals))
-        vals[outside] = values[outside]
-      elif maybe_bounce[0]:
-        outside = vals <= self._lims[0]
-        vals[outside] = values[outside]
-        vals = np.minimum(self._lims[1], vals)
+      prob = self._tran if not self._tran.ismulti else \
+             self._tran[int(reverse)]
+      kwds = {self._name: pred_vals,
+              self._name+"'": succ_vals}
+      cond = prob(**kwds)
+
+    return cond
+
+#-------------------------------------------------------------------------------
+  def __call__(self, values=None):
+    """ Return a probability distribution for the quantities in values. """
+    dist_name = self.eval_dist_name(values)
+    vals = self.evaluate(values)
+    prob = self.eval_prob(vals)
+    dims = {self._name: None} if isscalar(vals[self.name]) else {self._name: 0}
+    return PD(dist_name, vals, dims=dims, prob=prob, pscale=self._pscale)
+
+#-------------------------------------------------------------------------------
+  def step(self, *args, reverse=False):
+    """ Returns a conditional probability distribution for quantities in args.
+
+    :param *args: predecessor, successor values to evaluate conditionals.
+    :param reverse: Boolean flag to evaluate conditional probability in reverse.
+
+    :return a Dist instance of the conditional probability distribution
+    """
+    pred_vals, succ_vals = None, None 
+    if len(args) == 1:
+      if isinstance(args[0], (list, tuple)) and len(args[0]) == 2:
+        pred_vals, succ_vals = args[0][0], args[0][1]
       else:
-        outside = vals >= self._lims[1]
-        vals[outside] = values[outside]
-        vals = np.maximum(self._lims[0], vals)
-    return vals
+        pred_vals = args[0]
+    elif len(args) == 2:
+      pred_vals, succ_vals = args[0], args[1]
+    dist_pred_name = self.eval_dist_name(pred_vals)
+    dist_succ_name = None
+    if pred_vals is None and succ_vals is None and \
+        self._vtype not in VTYPES[float]:
+      dist_succ_name = self.eval_dist_name(succ_vals, "'")
+    pred_vals = self.evaluate(pred_vals)
+    vals, dims, kwargs = self.eval_step(pred_vals, succ_vals, reverse=reverse)
+    cond = self.eval_tran(vals, **kwargs)
+    if dist_succ_name is None:
+      dist_succ_name = self.eval_dist_name(vals[self.__prime_key], "'")
+    dist_name = '|'.join([dist_succ_name, dist_pred_name])
+
+    # TODO - distinguish between probabilistic and non-probabistic outputs
+    if cond is None:
+      cond = 1.
+      for val in vals.values():
+        if isinstance(val, np.ndarray):
+          cond = cond * np.ones(val.shape, dtype=float)
+
+    return PD(dist_name, vals, dims=dims, prob=cond, pscale=self._pscale)
+
+#-------------------------------------------------------------------------------
+  def __and__(self, other):
+    """ Combination operator between RV and another RV, RF, or SD. """
+    from probayes.rf import RF
+    from probayes.sd import SD
+    if isinstance(other, SD):
+      leafs = [self] + list(other.leafs.vars.values())
+      stems = other.stems
+      roots = other.roots
+      args = RF(*tuple(leafs))
+      if stems:
+        args += list(stems.values())
+      if roots:
+        args += list(roots.values())
+      return SD(*args)
+
+    if isinstance(other, RF):
+      rvs = [self] + list(other.vars.values())
+      return RF(*tuple(rvs))
+
+    if isinstance(other, RV):
+      return RF(self, other)
+
+    raise TypeError("Unrecognised post-operand type {}".format(type(other)))
+
+#-------------------------------------------------------------------------------
+  def __or__(self, other):
+    """ Conditional operator between RV and another RV, RF, or SD. """
+    from probayes.sd import SD
+    return SD(self, other)
+
+#-------------------------------------------------------------------------------
+  def __getitem__(self, arg):
+    """ If arg is a slice (i.e. RV[:]) then Variable icon is returned,
+    otherwise the Prob.__getitem__ method is called.
+    """
+    if isinstance(arg, slice):
+      return Variable.__getitem__(self, arg)
+    return Prob.__getitem__(self, arg)
+
+#-------------------------------------------------------------------------------
+#-------------------------------------------------------------------------------
+#-------------------------------------------------------------------------------
+def RVs(names, vtype=None, vset=None, prob=None, *args, **kwds):
+  if isinstance(names, str):
+    names = names.split(',')
+  varlist = [RV(name, vtype, vset, prob, *args, **kwds) for name in names]
+  return tuple(varlist)
 
 #-------------------------------------------------------------------------------
```

### Comparing `probayes-0.0.3/probayes/func.py` & `probayes-0.0.4/probayes/func.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 similarly used to may differences in form var_name'-var_name,
 making also a disallowed keyword.
 
 Func may be a tuple of callable/uncallable functions
 '''
 import numpy as np
 import scipy.stats
+import collections
 from probayes.vtypes import isscalar, isunitary
 
 #-------------------------------------------------------------------------------
 """ 
 Scipy calls is supported a special case for following call convention:"
 func() pdf
 func[0]() pdf
@@ -50,15 +51,15 @@
 
   # Protected
   _func = None
   _args = None
   _kwds = None
 
   # Private
-  __istuple = None
+  __ismulti = None
   __isscalar = None # not of interest to Func but to objects that call Func
   __isscipy = None
   __callable = None
   __scipyobj = None
   __scipycalls = None
   __order = None
   __delta = None
@@ -95,17 +96,17 @@
     self.__callable = None
     self.__scipyobj = None
     self.__isscipy = False
 
     # Sanity check func
     if self._func is None:
       assert not args and not kwds, "No optional args without a function"
-    self.__istuple = isinstance(self._func, tuple)
+    self.__ismulti = isinstance(self._func, tuple)
     self.__isscalar = False
-    if not self.__istuple:
+    if not self.__ismulti:
       self.__callable = callable(self._func)
       if not self.__callable:
         assert not args and not kwds, "No optional args with uncallable function"
         self.__isscalar = isscalar(self._func)
     else:
       func_callable = [callable(func) for func in self._func]
       func_isscalar = [isscalar(func) for func in self._func]
@@ -128,30 +129,30 @@
                            3: self.__scipyobj.logcdf,
                            4: self.__scipyobj.rvs,
                           }
     if 'order' in self._kwds:
       self.set_order(self._kwds.pop('order'))
     if 'delta' in self._kwds:
       self.set_delta(self._kwds.pop('delta'))
-    
+
 #-------------------------------------------------------------------------------
   def set_order(self, order=None):
     """ Sets an order remapping dictionary for functional calls in which
     keyword arguments are mapped to position (in numeric) or rekeyed (if str).
     """
     self.__order = order
     if self.__order is None:
       return
     assert self.__delta is None, "Cannot set both order and delta"
     assert self.__scipyobj is None, \
         "Optional 'order' keyword prohibited for scipy objectts"
     self._check_mapping(self.__order)
 
 #-------------------------------------------------------------------------------
-  def set_delta(self, order=None):
+  def set_delta(self, delta=None):
     """ Sets a difference remapping dictionary for functional calls in which
     keyword arguments are mapped to position (in numeric) or rekeyed (if str).
     """
     self.__delta = delta
     if self.__delta is None:
       return
     assert self.__order is None, "Cannot set both order and delta"
@@ -181,44 +182,75 @@
         raise TypeError("Cannot interpret index specification value: {}".ind)
     indset = set(inds)
     if len(indset):
       assert indset == set(range(min(indset), max(indset)+1)), \
           "Index specification non_sequitur: {}".format(indset)
 
 #-------------------------------------------------------------------------------
+  def ret_func(self):
+    """ Returns function argument set by set_func() """
+    return self._func
+
+#-------------------------------------------------------------------------------
+  def ret_args(self):
+    """ Returns args as set by set_func() """
+    return self._args
+
+#-------------------------------------------------------------------------------
+  def ret_kwds(self):
+    """ Returns kwds as set by set_func() """
+    return self._kwds
+
+#-------------------------------------------------------------------------------
   def ret_callable(self):
     """ Returns boolean flag as to whether func is callable """
     return self.__callable
 
 #-------------------------------------------------------------------------------
   def ret_isscalar(self):
     """ Returns boolean flag as to whether func is a scalar """
     return self.__isscalar
 
 #-------------------------------------------------------------------------------
-  def ret_istuple(self):
-    """ Returns boolean flag as to whether func comprises a tuple """
-    return self.__istuple
+  def ret_ismulti(self):
+    """ Returns boolean flag as to whether func comprises a multiple """
+    return self.__ismulti
 
 #-------------------------------------------------------------------------------
   def ret_isscipy(self):
     """ Returns boolean flag as to whether func comprises a scipy object """
     return self.__isscipy
 
 #-------------------------------------------------------------------------------
   def ret_scipyobj(self):
     """ Returns scipy object if specified """
     return self.__scipyobj
 
 #-------------------------------------------------------------------------------
+  def ret_order(self):
+    """ Returns order object if set """
+    return self.__order
+
+#-------------------------------------------------------------------------------
+  def ret_delta(self):
+    """ Returns delta object if set """
+    return self.__delta
+
+#-------------------------------------------------------------------------------
   def _call(self, *args, **kwds):
     """ Private call used by the wrapped Func interface.
     (see __call__ and __getitem__).
     """
 
+    """
+    # For debugging:
+    argsin = args
+    kwdsin = kwds
+    """
+
     # Handle scipy objects separately
     if self.__isscipy:
       return self._call_scipy(*args, **kwds)
 
     # Check for indexing and reset if necessary
     func = self._func
     if self.__index is not None:
@@ -227,21 +259,29 @@
 
     # Non-callables
     if not self.__callable:
       assert not args and not kwds, "No optional args with uncallable function"
       return func
 
     # Callables order-free
-    if not kwds and len(args) == 1 and isinstance(args[0], dict):
-      args, kwds = (), dict(args[0])
+    if len(args) == 1 and isinstance(args[0], dict):
+      args, kwds = (), {**kwds, **dict(args[0])}
     if self._args:
       args = tuple(list(self._args) + list(args))
     if self._kwds:
       kwds = {**kwds, **self._kwds}
     if not self.__order and not self.__delta:
+
+      """
+      # For debugging:
+      argsout = args
+      kwdsout = kwds
+      import pdb; pdb.set_trace()
+      """
+
       return func(*args, **kwds)
 
     # Append None to args according to mapping index specification
     n_args = len(args)
     mapping = self.__order or self.__delta
     for val in mapping.values():
       if type(val) is int:
@@ -286,15 +326,14 @@
     """ Private call used by the wrapped Func interface for scipy objects.
     (see __call__ and __getitem__).
     """
     index = 0
     if self.__index is not None:
       index = self.__index
       self.__index = None
-    vals = args[0]
     if index < 4:
       if len(args) == 1 and isinstance(args[0], dict):
         args = [np.ravel(val) for val in args[0].values()]
       elif not len(args) and len(kwds):
         args = list(collections.OrderedDict(**kwds).values())
         kwds = {}
       if isinstance(args, list) and not np.all([isunitary(arg) for arg in args]):
@@ -307,29 +346,29 @@
     return self.__scipycalls[index](*args, **kwds)
 
 #-------------------------------------------------------------------------------
   def __call__(self, *args, **kwds):
    """ Wrapper call to the function with optional inclusion of additional
    args and kwds. """
 
-   assert not self.__istuple or self.__isscipy, \
-       "Cannot call with tuple func, use Func[]"
+   assert not self.__ismulti or self.__isscipy, \
+       "Cannot call with multiple func, use Func[]"
    return self._call(*args, **kwds)
 
 #-------------------------------------------------------------------------------
-  def __getitem__(self, index=None):
-   r""" Calls the $i$th function from the Func tuple where the index is $i$ """
-   if index is None:
+  def __getitem__(self, spec=None):
+   r""" Calls the $i$th function from the Func tuple where the spec is $i$ """
+   if spec is None:
      return self._func
-   assert self.__istuple or self.__isscipy, \
+   assert self.__ismulti or self.__isscipy, \
      "Cannot index without single func, use Func()"
-   self.__index = index
+   self.__index = spec
    return self._call
 
 #-------------------------------------------------------------------------------
   def __len__(self):
     """ Returns the number of functions in the tuple set by set_func() """
-    if not self.__istuple:
+    if not self.__ismulti:
       return None
     return len(self._func)
 
 #-------------------------------------------------------------------------------
```

### Comparing `probayes-0.0.3/probayes/prob.py` & `probayes-0.0.4/probayes/cf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,243 +1,220 @@
-"""
-A probability class supporting probability distributions without specification 
-of a variable set.
-"""
-
-#-------------------------------------------------------------------------------
-import warnings
-import numpy as np
-import scipy.stats
-from probayes.vtypes import isscalar
-from probayes.pscales import eval_pscale, rescale, iscomplex
+# This module is to be deprecated along with Func.
+'''A conditional function is a functional wrapper that describes the 
+dependence of an about output RF with respect to an input RF or the
+by the dependence of a subgroup of RVs with respect to the others. 
+'''
+import collections
+from probayes.rv import RV
 from probayes.func import Func
 
 #-------------------------------------------------------------------------------
-SCIPY_STATS_CONT = {scipy.stats.rv_continuous}
-SCIPY_STATS_DISC = {scipy.stats.rv_discrete}
-SCIPY_STATS_DIST = SCIPY_STATS_CONT.union(SCIPY_STATS_DISC)
-
-#-------------------------------------------------------------------------------
-def is_scipy_stats_cont(arg, scipy_stats_cont=SCIPY_STATS_CONT):
-  """ Returns if argument belongs to scipy.stats.continuous """
-  return isinstance(arg, tuple(scipy_stats_cont))
-
-#-------------------------------------------------------------------------------
-def is_scipy_stats_dist(arg, scipy_stats_dist=SCIPY_STATS_DIST):
-  """ Returns if argument belongs to scipy.stats.continuous or discrete """
-  return isinstance(arg, tuple(scipy_stats_dist))
-
-#-------------------------------------------------------------------------------
-class Prob:
-  """ A probability is quantification of degrees of belief concerning outcomes.
-  Typically these outcomes are defined over the domains of one or more variables. 
-  Since this is not a requirement, this class is not abstract, but it is 
-  nevertheless not so useful as probayes.RV if instantiated directly. 
-  This class can be used to define a probability distribution.
-
-  :example:
-  >>> import scipy.stats
-  >>> import probayes as pb
-  >>> norm = pb.Prob(scipy.stats.norm)
-  >>> print(norm(0.))
-  0.3989422804014327
-  """
+def _to_rf(obj=None):
+  """ Converts obj (which may be an RV/RF) or list/tuple of such to an RF """
+  from probayes.rf import RF
+  if obj is None:
+    return obj
+  if isinstance(obj, RF):
+    assert not obj.stems and not obj.roots, \
+        "RFs must be rootless and stemless"
+    return obj
+  elif isinstance(obj, RV):
+    return RF(obj)
+  elif isinstance(obj, (list, tuple)):
+    rvs = []
+    for subobj in obj:
+      if isinstance(subobj, RV):
+        rvs += [subobj]
+      elif isinstance(subobj, RF):
+        assert not obj.stems and not obj.roots, \
+            "RFs must be rootless and stemless"
+        rvs += subobj.varlist
+      else:
+        raise TypeError("Unexpected type: {}".format(type(subobj)))
+    return RF(*tuple(rvs))
+  else:
+    raise TypeError("Unexpected type: {}".format(type(subobj)))
 
+#-------------------------------------------------------------------------------
+#-------------------------------------------------------------------------------
+#-------------------------------------------------------------------------------
+class CF (Func):
+  '''A conditional function is a functional wrapper that describes the 
+  dependence of an about output RF with respect to an input RF or the
+  by the dependence of a subgroup of RVs with respect to the others. 
+  '''
   # Protected
-  _prob = None      # Probability distribution function
-  _pscale = None    # Probability type (can be a scipy.stats.dist object)
-  _pfun = None      # 2-length tuple of cdf/icdf
+  _out = None
+  _inp = None
+  _name = None
+  _passprob = None
+  _passdims = None
 
   # Private
-  __pset = None     # Set of pdfs/logpdfs/cdfs/icdfs
-  __scalar = None   # Flag for being a scalar
-  __callable = None # Flag for callable function
-
-#-------------------------------------------------------------------------------
-  def __init__(self, prob=None, pscale=None, *args, **kwds):
-    """ Initialises the probability and pscale (see set_prob). """
-    self.set_prob(prob, pscale, *args, **kwds)
+  __inpdict = None
+  __unknown = None
 
 #-------------------------------------------------------------------------------
-  def set_prob(self, prob=None, pscale=None, *args, **kwds):
-    """ Sets the probability and pscale with optional arguments and keywords.
-
-    :param prob: may be a scalar, array, or callable function.
-    :param pscale: represents the scale used to represent probabilities.
-    :param *args: optional arguments to pass if prob is callable.
-    :param **kwds: optional keywords to pass if prob is callable.
-
-    See set_pscale() for explanation of how pscale is used.
+  @property
+  def callable(self):
+    return self._Func__callable
+
+  @property
+  def isscipy(self):
+    return self._Func__isscipy
+
+  @property
+  def isscalar(self):
+    return self._Func__isscalar
+
+  @property
+  def ismulti(self):
+    return self._Func__ismulti
+
+  def __init__(self, out=None, inp=None, func=None, *args, **kwds):
+    """ Sets the output and input random fields out and inp and initialises 
+    the function according to object in func, which may be an uncallable
+    object, a callable function, or a tuple of callable functions. See Func.
     """
-    self._pfun = None
-    pset = prob if is_scipy_stats_dist(prob) else None
-    self.__scalar = None
-    self.__callable = None
-
-    # Handle SciPy distributions and scalars, 
-    if pset is not None:
-      prob = None        # needed to pass set_pset assertion
-      self.__pset = pset # needed to pass set_pscale assertion
-    elif isscalar(prob): 
-      prob = float(prob)
-    self._prob = prob 
-
-    # Set pscalar before pset
-    self.set_pscale(pscale) # this defaults self._pfun
-
-    # Create functional interface for prob
-    if pset is not None:
-      self.set_pset(pset, *args, **kwds)
-    elif  self._prob is not None:
-      self._prob = Func(self._prob, *args, **kwds)
-    else:
-      return
-
-    # Set pscale and distinguish between non-callable and callable self._prob
-    self.__isscalar = self._prob.ret_isscalar()
-    self.__callable = self._prob.ret_callable()
-
-#-------------------------------------------------------------------------------
-  def set_pscale(self, pscale=None):
-    """ Sets the probability scaling constant used for probabilities.
-
-    :param pscale: can be None, a real number, or a complex number, or 'log'
-
-       if pscale is None (default) the normalisation constant is set as 1.
-       if pscale is real, this defines the normalisation constant.
-       if pscale is complex, this defines the offset for log probabilities.
-       if pscale is 'log', this denotes a logarithmic scale with an offset of 0.
-
-    :return: pscale (either as a real or complex number)
+    self.set_out(out)
+    self.set_inp(inp)
+    self.set_func(func, *args, **kwds)
+    
+#-------------------------------------------------------------------------------
+  def set_out(self, out=None):
+    """ Sets the output and input random fields out, which may be an RF an RV or 
+    tuple or RFs and RVs but not an SD. 
     """
-    self._pscale = eval_pscale(pscale)
-
-    # Probe pset to set functions based on pscale setting
-    if self.__pset is None:
-      if self._pscale != 1.:
-        assert self._prob is not None, \
-            "Cannot specify pscale without setting prob"
-      self.set_pfun()
-
-    return self._pscale
+    self._out = _to_rf(out)
 
 #-------------------------------------------------------------------------------
-  def set_pset(self, pset, *args, **kwds):
-    """ Sets a set of probability functions if prob is a scipy.stats object.
-    Normally this function should not require calling if set_prob is set.
+  def set_inp(self, inp=None):
+    """ Sets the output and input random fields out and inp, each of which may 
+    be an RF an RV or tuple or RFs and RVs but not an SD. Optionally inp may
+    be an OrderedDict with RV names in the form (only keys are checked):
+    {'x_0,x_1': 'x_2,x_3,x_4', 'x_2': 'x_0', 'x_3,x_4': 'x_0,x_1,x_2'}. 
     """
-    self.__pset = pset if is_scipy_stats_dist(pset) else None
-    if self.__pset is None:
-      return
-    assert self._prob is None, "Cannot use scipy.stats.dist while also setting prob"
-    if not iscomplex(self._pscale):
-      if hasattr(self.__pset, 'pdf'):
-        self._prob = Func(self.__pset.pdf, *args, **kwds)
-      elif hasattr(self.__pset, 'pmf'):
-        self._prob = Func(self.__pset.pmf, *args, **kwds)
-      else: 
-        warnings.warn("Cannot find probability function for {}"\
-                      .format(self.__pset))
-    else:
-      if hasattr(self.__pset, 'logpdf'):
-        self._prob = Func(self.__pset.logpdf, *args, **kwds)
-      elif hasattr(self.__pset, 'logpmf'):
-        self._prob = Func(self.__pset.logpmf, *args, **kwds)
-      else: 
-        warnings.warn("Cannot find log probability function for {}"\
-                      .format(self.__pset))
-    if hasattr(self.__pset, 'cdf') and  hasattr(self.__pset, 'ppf'):
-      self.set_pfun((self.__pset.cdf, self.__pset.ppf), *args, **kwds)
-    else:
-      warnings.warn("Cannot find cdf and ppf functions for {}"\
-                    .format(self._pscale))
-      self.set_pfun()
-
-#-------------------------------------------------------------------------------
-  def ret_pset(self):
-    """ Returns object set by set_pset() """
-    return self.__pset
-
-#-------------------------------------------------------------------------------
-  def set_pfun(self, pfun=None, *args, **kwds):
-    """ Sets a two-length tuple of functions that should correspond to the
-    (cumulative probability function, inverse cumulative function) with respect
-    to the callable function set by set_prob(). It is necessary to set these
-    functions if sampling variables with non-flat distributions.
-
-    :param pfun: two-length tuple of callable functions
-    :param *args: arguments to pass to pfun functions
-    :param **kwds: keywords to pass to pfun functions
-    """
-    self._pfun = pfun
-    if self._pfun is None:
+    self.__inpdict = isinstance(inp, (tuple, list, dict))
+    if self.__inpdict:
+      if isinstance(inp, (tuple, list)):
+        inp = {key: '' for key in inp}
+    self.__unknown = None
+
+    # Handle inp is a random field first
+    if not self.__inpdict and inp is not None:
+      assert self._out is not None, "Set outputs before inputs"
+      self._inp = _to_rf(inp)
+      self._name = '|'.join([self._out.name, self._inp.name])
       return 
-    
-    message = "Input pfun be a two-sized tuple of callable functions"
-    assert isinstance(self._pfun, tuple), message
-    assert len(self._pfun) == 2, message
-    assert callable(self._pfun[0]), message
-    assert callable(self._pfun[1]), message
-    self._pfun = Func(self._pfun, *args, **kwds)
+    elif inp is not None and not isinstance(inp, collections.OrderedDict):
+      raise TypeError("Dictionary specification for inp must be an OrderedDict")
 
-#-------------------------------------------------------------------------------
-  def ret_pfun(self, index=None):
-    """ Returns object set by set_pfun() """
-    if self._pfun is None or index is None:
-      return self._pfun
-    return self._pfun[index]
-
-#-------------------------------------------------------------------------------
-  def ret_prob(self):
-    """ Returns object set by set_prob() """
-    return self._prob
-
-#-------------------------------------------------------------------------------
-  def ret_callable(self):
-    """ Returns whether object set by set_prob() is callable """
-    return self.__callable
-
-#-------------------------------------------------------------------------------
-  def ret_isscalar(self):
-    """ Returns whether prob is a scalar """
-    return self.__isscalar
+    # At this stage, there must be at least two RVs
+    rv_keys = self._out.keylist
+    assert len(rv_keys) > 1, "Multiple RVs required for conditional functions"
+
+    # Check inp if entered
+    if inp:
+      all_inp_keys = [] 
+      for key, val in inp.items():
+        inp_keys = key.split(',')
+        val_keys = val.split(',')
+        for val_key in val_keys:
+          if len(inp) > 1:
+            assert val_key not in inp_keys, \
+                "Circular key reference {}:{}".format(key, val)
+          assert val_key in rv_keys, \
+              "Key {} not recognised in RF {}".format(val_key, self._out)
+        all_inp_keys += inp_keys
+      assert set(rv_keys) == set(all_inp_keys), \
+          "Conditional function {} specification incommensurate with RF {}".\
+          format(inp, self._out)
+      self._inp = inp
+    prime_keys = ["{}'".format(rv_key) for rv_key in rv_keys]
+    self._name = '|'.join([','.join(prime_keys), ','.join(rv_keys)])
+
+#-------------------------------------------------------------------------------
+  def set_func(self, func=None, *args, **kwds):
+    """ Set the CF instance's function object.
+
+    :param func: an uncallable object, callable function, or tuple of functions
+    :param *args: arguments to pass onto callables
+    :param **kwds: keywords to pass onto callables
+
+    Note that the following two reserved keywords are disallowed:
+
+    'order': which instead denotes a dictionary of remappings.
+    'delta': which instead denotes a mapping of differences.
+    'passdims': which provides an auxiliary flag to SD to pass dims
+    'passprob': which provides an auxiliary flag to SD to pass prob`
 
-#-------------------------------------------------------------------------------
-  def ret_pscale(self):
-    """ Returns the real or complex scaling constant set for pscale """
-    return self._pscale
-
-#-------------------------------------------------------------------------------
-  def rescale(self, probs, **kwds):
-    """ Returns a rescaling of probs from current pscale to the values according
-    to the keyword pscale=new_pscale. """
-    if 'pscale' not in kwds:
-      return probs
-    return rescale(probs, self._pscale, kwds['pscale'])
-
-#-------------------------------------------------------------------------------
-  def eval_prob(self, *args, **kwds):
-    """ Evaluates the probability inputting optional args for callable cases
-
-    :param *args: optional arguments for callable probability objects.
-    :param **kwds: optional arguments to include pscale for rescaling.
-
-    :return: evaluated probabilities
     """
-    # Callable and non-callable evaluations
-    probs = self._prob
-    if self.__callable:
-      probs = probs(*args)
-    else:
-      assert not len(args), \
-          "Cannot evaluate from values from an uncallable probability function"
-      probs = probs()
-    if 'pscale' in kwds:
-      return self.rescale(probs, kwds['pscale'])
-    return probs
-
-#-------------------------------------------------------------------------------
-  def __call__(self, *args, **kwds):
-    """ See eval_prob() """
-    return self.eval_prob(*args, **kwds)
+
+    self._func = func
+    self._args = tuple(args)
+    self._kwds = dict(kwds)
+    self._passdims = None if 'passdims' not in kwds else self._kwds.pop('passdims')
+    self._passprob = None if 'passprob' not in kwds else self._kwds.pop('passprob')
+    if isinstance(self._func, Func) and not self._args and not self._kwds:
+      func = self._func.ret_func()
+      args = self._func.ret_args()
+      kwds = self._func.ret_kwds()
+      order = self._func.ret_order()
+      delta = self._func.ret_delta()
+      argout = super().set_func(func, *args, **kwds)
+      self.set_order(order)
+      self.set_delta(delta)
+      return argout
+    super().set_func(self._func, *self._args, **self._kwds)
+
+#-------------------------------------------------------------------------------
+  def ret_name(self):
+    """ Return the conditional function name determined from the RFs """
+    return self._name
+
+#-------------------------------------------------------------------------------
+  def ret_out(self):
+    """ Returns output RF """
+    return self._out
+
+#-------------------------------------------------------------------------------
+  def ret_inp(self):
+    """ Returns input RF """
+    return self._inp
+
+#-------------------------------------------------------------------------------
+  def ret_passdims(self):
+    """ Returns passdims flag if specified """
+    return self._passdims
+
+#-------------------------------------------------------------------------------
+  def ret_passprob(self):
+    """ Returns passprob flag if specified """
+    return self._passprob
+
+#-------------------------------------------------------------------------------
+  def ret_inpdict(self):
+    """ Returns flag inpdict indicating whether a dict """
+    return self.__inpdict
+
+#-------------------------------------------------------------------------------
+  def __getitem__(self, spec=None):
+   r""" Calls the $i$th function from the Func tuple where the spec is $i$.
+   If spec is a string, then the specification is changed.
+   """
+   if not isinstance(spec, str):
+     return super().__getitem__(spec)
+   assert self.__inpdict, \
+       "Input spec as a string only supported with a OrderedDict inp"
+   self.__unknown = spec
+   return self._call
+
+#-------------------------------------------------------------------------------
+  def _call(self, *args, **kwds):
+    if self.__unknown is None:
+      return super()._call(*args, **kwds)
+    kwds = dict(kwds)
+    kwds.update({'unknown': self.__unknown})
+    self.__unknown = None
+    return super()._call(*args, **kwds)
 
 #-------------------------------------------------------------------------------
```

### Comparing `probayes-0.0.3/probayes/pscales.py` & `probayes-0.0.4/probayes/pscales.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,45 +2,19 @@
 A module that handles probability calculations according different pscales that
 may represent probability coefficients (positive float scalars) or log 
 probability offsets (complex float scalars).
 """
 
 #-------------------------------------------------------------------------------
 import numpy as np
-""" Set limits to 32-bit precision """
-
-DEFAULT_FP_PRECISION = 64
-COMPLEX_ZERO = complex(0., 0.)
-FP_CONSTANTS = {32: {'nearly_positive_zero': 1.175494351e-38,
-                     'nearly_positive_inf': 3.4022823466e38},
-                64: {'nearly_positive_zero': 2.2250738585072014e-308,
-                     'nearly_positive_inf': 1.7976931348623158e+308},
-               }
-
-NEARLY_POSITIVE_ZERO = None
-NEARLY_POSITIVE_INF = None
-NEARLY_NEGATIVE_INF = None
-LOG_NEARLY_POSITIVE_INF =  None
-
-def SET_FP_CONSTANTS(precision=DEFAULT_FP_PRECISION):
-  """ Sets global floating point constants whether using precision=32 or
-  precision=64 (default)
-  """
-  global NEARLY_POSITIVE_ZERO
-  global NEARLY_POSITIVE_INF
-  global NEARLY_NEGATIVE_INF
-  global NEARLY_POSITIVE_INF
-  global LOG_NEARLY_POSITIVE_INF
-  NEARLY_POSITIVE_ZERO = FP_CONSTANTS[precision]['nearly_positive_zero']
-  NEARLY_POSITIVE_INF = FP_CONSTANTS[precision]['nearly_positive_inf']
-  NEARLY_NEGATIVE_INF = -NEARLY_POSITIVE_INF
-  LOG_NEARLY_POSITIVE_INF = np.log(NEARLY_POSITIVE_INF)
-
-if NEARLY_NEGATIVE_INF is None or LOG_NEARLY_POSITIVE_INF is None:
-  SET_FP_CONSTANTS()
+from probayes.constants import NEARLY_POSITIVE_ZERO, \
+                               NEARLY_POSITIVE_INF, \
+                               NEARLY_NEGATIVE_INF, \
+                               LOG_NEARLY_POSITIVE_INF, \
+                               COMPLEX_ZERO
 
 #-------------------------------------------------------------------------------
 def iscomplex(pscale):
   """ Returns whether pscale is an instance of a complex number """
   return isinstance(pscale, complex)
 
 #-------------------------------------------------------------------------------
@@ -127,23 +101,22 @@
   """ Rescales prob according to pscales given in args """
   pscale, rtype = None, None
   prob = prob if np.isscalar(prob) \
            or prob.dtype in [float, np.dtype('float32'), np.dtype('float64')] \
          else np.array(prob, dtype=float)
   if len(args) == 0: 
     return prob
-  elif len(args) ==  1: 
+  elif len(args) == 1: 
     rtype = args[0]
   else: 
     pscale, rtype = args[0], args[1]
   pscale, rtype = eval_pscale(pscale), eval_pscale(rtype)
-  if pscale == rtype:
-    return prob
-  
   p_log, r_log = iscomplex(pscale), iscomplex(rtype)
+  if p_log == r_log and pscale == rtype:
+    return prob
 
   # Support non-logarithmic conversion (maybe used to avoid logging zeros)
   if not p_log and not r_log:
     coef = pscale / rtype
     if coef == 1.:
       return prob
     else:
```

### Comparing `probayes-0.0.3/probayes/rf.py` & `probayes-0.0.4/probayes/dependence.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,449 +1,454 @@
-"""
-A random field is a random junction (here called marg) that may be conditioned 
-by a another random junction (here called cond) according to a conditional
-probability distribution function.
-"""
-#-------------------------------------------------------------------------------
-import numpy as np
-import collections
-from probayes.rj import RJ
-from probayes.func import Func
-from probayes.dist import Dist
-from probayes.dist_utils import product
-from probayes.rf_utils import desuffix, get_suffixed
+""" Provides Dependence class """
 
 #-------------------------------------------------------------------------------
-class RF (RJ):
-  # Public
-  opqr = None          # (p(pred), p(succ), q(succ|pred), q(pred|succ))
+import collections
+import networkx as nx
+from probayes.variable import Variable
+from probayes.field import Field
+from probayes.cf import CF
+from probayes.functional import Functional
+NX_DIRECTED_GRAPH = nx.DiGraph
+
+#-------------------------------------------------------------------------------
+class Dependence (NX_DIRECTED_GRAPH, Field):
+  """ A dependence is field with an explicit directed conditionality. The 
+  dependences are represented as a graph, representing variables as vertices, 
+  and edges for their corresponding inter-relations. 
+  
+  Direct conditional dependences across groups of variables are set using 
+  conditional functions that inter-relate fields. This can be performed via 
+  the implicit architectural interface or explicit dependency interface 
+  (self.add_deps()).
+
+  Modification of a dependence functional can be made from an instance, only
+  affecting its correspondence leaf vertices. Intermediate dependence functions
+  can be set only from dependence predecessors.
+
+  For convenience to define deltas, Dependence supports defaulting of proposal 
+  objects without actually supporting proposals.
+  """
 
   # Protected
-  _marg = None
-  _cond = None
-  _marg_cond = None    # {'marg': marg, 'cond': cond}
-  _def_prop_obj = None
-  _prop_obj = None
-  _unit_prob = None # Flag for single RV probability
-  _unit_tran = None # Flag for single RV transitional
-
-  # Private
-  __sym_tran = None
+  _arch = None             # Implicit archectectural configuration
+  _leafs = None            # Field of variables that do not condition others
+  _roots = None            # Field of variables not dependent on others
+  _stems = None            # OrderedDict of latent RVs
+  _preds = None            # Field of variables that are predecessors to leafs
+  _def_prop_obj = None     # Default value for prop_obj
+  _prop_obj = None         # Object referencing propositional conditions
+  _variable_cls = Variable # Variable class
+  _field_cls = Field       # Field class
+  _subfields = None        # Convenience dictionary for the roots and leafs RFs
+  _is_stochastic = False   # Flag of stochasticity status
 
 #------------------------------------------------------------------------------- 
   def __init__(self, *args):
-    self.set_prob()
-    assert len(args) < 3, "Maximum of two initialisation arguments"
-    arg0 = None if len(args) < 1 else args[0]
-    arg1 = None if len(args) < 2 else args[1]
-    if arg0 is not None: self.set_marg(arg0)
-    if arg1 is not None: self.set_cond(arg1)
+    """ Initialises the Dependence with Variables, Fields, or Dependences. 
+    See def_deps().; """
+    NX_DIRECTED_GRAPH.__init__(self)
+    self.def_deps(*args)
+
+#-------------------------------------------------------------------------------
+  @property
+  def preds(self):
+    return self._preds
+
+  @property
+  def deps(self):
+    return self._deps
+
+  @property
+  def arch(self):
+    return self._arch
+
+  def def_deps(self, *args):
+    """ Defaults the dependence with variables, fields, or dependence arguments.
+
+    :param args: each arg may be a variable, field, or dependence with the 
+                 dependence chain with running right to left. If one argument is
+                 a dependence, then all arguments must comprise of dependence 
+                 instances.
+    """
+    self._deps = None
+    self._arch = None
+    if not args:
+      return
+    arg_aredep = [isinstance(arg, type(self)) for arg in args]
 
-#-------------------------------------------------------------------------------
-  def set_marg(self, arg):
-    if isinstance(arg, RJ):
-      assert not isinstance(arg, RF), "Marginal must be RJ class type"
-      self._marg = arg
-      self._refresh()
-    else:
-      self.add_marg(arg)
+    # Absence of Dependence instances means at most a single direct dependency
+    if not any(arg_aredep):
+      self._arch = self
+      fields = [None] * len(args)
+      for i, arg in enumerate(args):
+        if isinstance(arg, self._variable_cls):
+          fields[i] = self._field_cls(arg)
+        elif isinstance(arg, self._field_cls):
+          fields[i] = arg
+        else:
+          raise TypeError("Unrecognised input argument type: {}".format(
+              type(arg)))
 
-#-------------------------------------------------------------------------------
-  def set_cond(self, arg):
-    if isinstance(arg, RJ):
-      assert not isinstance(arg, RF), "Conditional must be RJ class type"
-      self._cond = arg
-      self._refresh()
-    else:
-      self.add_cond(arg)
+      # Declare vertices, adding edges if there are multiple arguments
+      if len(fields) == 1:
+        variables = list(fields[0].varlist)
+        for var in variables:
+          NX_DIRECTED_GRAPH.add_node(self, var)
+        return self._refresh(fields[0])
+      leafs_vars = fields[0].varlist
+      roots_vars = fields[-1].varlist
+      if len(fields) > 2:
+        for field in fields[1:-1]:
+          leafs_vars += list(field.varlist)
+
+      # Add leafs then roots
+      for var in leafs_vars:
+        NX_DIRECTED_GRAPH.add_node(self, var)
+      for var in roots_vars:
+        NX_DIRECTED_GRAPH.add_node(self, var)
+
+      # Add edges
+      for roots_var in roots_vars:
+        for leafs_var in leafs_vars:
+          NX_DIRECTED_GRAPH.add_edge(self, roots_var, leafs_var)
+      if len(fields) == 2:
+        return self._refresh(fields[0], fields[1])
+      return self._refresh(self._field_cls(*tuple(leafs_var)), fields[-1])
+
+    # At this point, all arguments must be dependences
+    assert all(arg_aredep), "Cannot mix Dependences with other input types"
+
+    # Adding all vertices in forward order, starting with leafs then the rest
+    for arg in args:
+      leafs = list(arg.leafs.varlist)
+      for leaf in leafs:
+        NX_DIRECTED_GRAPH.add_node(self, leaf)
+    for arg in args:
+      variables = list(arg.nodes)
+      for var in variables:
+        NX_DIRECTED_GRAPH.add_node(self, var)
+
+    # Adding all edges in reverse order
+    for arg in args[::-1]:
+      NX_DIRECTED_GRAPH.add_edges_from(self, arg.edges())
+
+    # Explicit dependences to be added in reverse order with all implicit bets off
+    deps = [arg.deps for arg in args[::-1]]
+    if any(deps):
+      self._arch = None
+      [self.add_deps(dep) for dep in deps]
+      return self._refresh()
+
+    # Implicit dependences may either be in parallel or in series, but not both
+
+    # Iterate args, add RV vertices, detect running roots/leafs and explicit
+    run_leafs = [None] * len(args)
+    run_roots = [None] * len(args)
+    for i, arg in enumerate(args):
+      run_leafs[i] = list(arg.leafs.varlist)
+      run_roots[i] = list(arg.roots.varlist)
+
+    # Detect for implicit serial dependences
+    serial = len(args) > 1
+    for i in range(len(args)-1):
+      if run_roots[i] is None or set(run_roots[i]) != set(run_leafs[i+1]):
+        serial = False
+        break
+    if serial:
+      self._arch = list(args[::-1])
+      leafs, roots = None, None
+      for i, arg in enumerate(args):
+        if i == 0:
+          leafs = arg.leafs
+          roots = arg.roots
+        elif i == len(args) - 1:
+          roots = arg.roots
+      return self._refresh(leafs, roots)
+
+    # Detect for implicit parallel dependences
+    parallel = len(args) > 1 
+    leafs = set()
+    roots = []
+    if parallel:
+      for i, arg in enumerate(args):
+        roots += run_roots[i]
+        if not leafs:
+          leafs = run_leafs[i]
+        elif not len(run_roots[i]) or leafs != run_leafs[i]:
+          parallel = False
+          break
+    if parallel:
+      self._arch = tuple(args[::-1])
+      leafs = args[0].leafs
+      roots = self._field_cls(*tuple(roots))
+      return self._refresh(leafs, roots)
+
+    return self._refresh()
+
+#-------------------------------------------------------------------------------
+  @property
+  def subfields(self):
+    return self._subfields
+
+  def _refresh(self, leafs=None, roots=None):
+    """ Refreshes tree summaries, Dependence name and identity, and default 
+    states. While roots and leafs are represented as Fields, stems are contained 
+    within a single ordered dictionary to be flexible enough to accommodate 
+    dependence  arborisations.
 
-#-------------------------------------------------------------------------------
-  def add_marg(self, *args):
-    if self._marg is None: 
-      self._marg = RJ()
-    self._marg.add_rv(*args)
-    self._refresh()
-
-#-------------------------------------------------------------------------------
-  def add_cond(self, *args):
-    if self._cond is None: self._cond = RJ()
-    self._cond.add_rv(*args)
-    self._refresh()
-
-#-------------------------------------------------------------------------------
-  def _refresh(self):
-    marg_name, cond_name = None, None
-    marg_id, cond_id = None, None
-    self._rvs = []
-    self._keys = []
-    if self._marg:
-      marg_name = self._marg.ret_name()
-      marg_id = self._marg.ret_id()
-      marg_rvs = [rv for rv in self._marg.ret_rvs()]
-      self._rvs.extend([rv for rv in self._marg.ret_rvs()])
-    if self._cond:
-      cond_name = self._cond.ret_name()
-      cond_id = self._cond.ret_id()
-      cond_rvs = [rv for rv in self._cond.ret_rvs()]
-      self._rvs.extend([rv for rv in self._cond.ret_rvs()])
-    if self._marg is None and self._cond is None:
-      return
-    self._marg_cond = {'marg': self._marg, 'cond': self._cond}
-    self._nrvs = len(self._rvs)
-    self._keys = [rv.ret_name() for rv in self._rvs]
-    self._keyset = set(self._keys)
-    self._defiid = self._marg.ret_keyset()
-    names = [name for name in [marg_name, cond_name] if name]
-    self._name = '|'.join(names)
-    ids = [_id for _id in [marg_id, cond_id] if _id]
-    self._id = '_with_'.join(ids)
-    self.set_pscale()
+    :param leafs: sets default for leafs
+    :param roots: sets default for roots
+    """
+    self._leafs = None
+    self._stems = collections.OrderedDict()
+    self._roots = None
+
+    # If defaulting leafs, then assume a simple RF specification
+    if leafs:
+      assert type(leafs) is self._field_cls, \
+          "Input leafs cannot be type {}".format(type(leafs))
+      self._leafs = leafs
+      self._roots = roots
+      if self._roots:
+        assert type(self._roots) is self._field_cls, \
+          "Input roots cannot be type {}".format(type(roots))
+
+    # Otherwise distinguish Variables belonging to leafs, roots, and stems
+    else:
+      leafs = [] # Field of vertices with no children/successors
+      roots = [] # Field of vertices with no parents/predecessors (and not a leaf)
+      self._stems = collections.OrderedDict()
+      variables = list(self.nodes)
+      for var in variables:
+        parents = list(self.predecessors(var))
+        children = list(self.successors(var))
+        if parents and children:
+          self._stems.update({var.name: var})
+        elif children: # roots must have children
+          roots += [var]
+        else: # leafs can be parentless
+          leafs += [var]
+      self._leafs = self._field_cls(*tuple(leafs))
+      if roots:
+        self._roots = self._field_cls(*tuple(roots))
+
+    # Evaluate leafs predecessors 
+    self._preds = None
+    if not self._stems:
+      self._preds = None if not self._roots else self._roots
+    else:
+      preds = set()
+      for leaf_var in self._leafs.varlist:
+        [preds.add(pred_var) for pred_var in self.predecessors(leaf_var)]
+      self._preds = self._field_cls(*tuple(preds))
+
+    # Default functions for implicit architectures
+    if self._arch: # TODO self._arch must always be defined by this point
+      self._func = Functional(self._leafs, self._preds)
+
+    # Set convenience subfields, and evaluate name and id from leafs and roots only
+    super()._refresh()
+    self._name = self._leafs.name
+    self._id = self._leafs.id
+    self._subfields = {'leafs': self._leafs}
+    if self._roots:
+      self._name += "|{}".format(self._roots.name)
+      self._id += "_with_{}".format(self._roots.id)
+      self._subfields.update({'roots': self._roots})
     self.eval_length()
-    self.opqr = collections.namedtuple(self._id, ['o', 'p', 'q', 'r'])
 
     # Set the default proposal object and default the delta accordingly
-    self._def_prop_obj = self._cond if self._cond is not None else self._marg
-    self.delta = self._def_prop_obj.delta
+    self._def_prop_obj = self._roots if self._roots is not None else self._leafs
+    self._Delta = self._def_prop_obj.Delta
     self._delta_type = self._def_prop_obj._delta_type
-    self.set_prop_obj(None)
+    self.set_prop_obj(None) # this is for the instantiater to decide
 
-    # Determine unit RVRF
-    self._unit_prob = False
-    self._unit_tran = False
-    if self._nrvs == 1:
-      rv = self._rvs[0]
-      self._unit_prob = self._prob is None and rv.ret_prob() is not None
-      self._unit_tran = self._tran is None and rv.ret_tran() is not None
+#-------------------------------------------------------------------------------
+  @property
+  def func(self):
+    return self._func
+
+  def add_func(self, spec, func, *args, **kwds):
+    assert self._func, \
+        "Architectual specification not able to accommodate functionals"
+    self._func.add_func(spec, func, *args, **kwds)
 
 #-------------------------------------------------------------------------------
+  def add_deps(self, out, inp=None, func=None, *args, **kwds):
+    """ Adds a conditional dependence that conditions conditioning with respect
+    to out being conditioned by inp by function func with *args and **kwds.
+    """
+    if self._arch:
+      self.remove_edges_from(self.edges)
+      self._arch = None
+    if self._deps is None:
+      self._deps = collections.OrderedDict()
+    assert not self._prob, \
+        "Cannot assign conditional dependencies alongside specified probability"
+    if inp is None and func is None:
+      for key, val in out.items():
+        self._deps.update({key: val})
+        self.add_edges_from(val)
+
+    dep = CF(out, inp, func, *args, **kwds)
+    dep_key = dep.ret_name()
+    self._deps.update({dep_key: dep})
+    out_keys = list(dep.ret_out().ret_keys(as_list=True))
+    inp_keys = list(dep.ret_inp().ret_keys(as_list=True))
+    for out_key in out_keys:
+      for inp_key in inp_keys:
+        self.add_edge(inp_key, out_key)
+    return collections.OrderedDict({dep_key: self._deps[dep_key]})
+
+#-------------------------------------------------------------------------------
+  @property
+  def prop_obj(self):
+    return self._prop_obj
+
   def set_prop_obj(self, prop_obj=None):
     """ Sets the object used for assigning proposal distributions """
     self._prop_obj = prop_obj
     if self._prop_obj is None:
       return
-    self.delta = self._prop_obj.delta
+    self._Delta = self._prop_obj.Delta
     self._delta_type = self._prop_obj._delta_type
 
 #-------------------------------------------------------------------------------
-  def set_prop(self, prop=None, *args, **kwds):
-    if not isinstance(prop, str) and prop not in self._marg_cond.values():
-      return super().set_prop(prop, *args, **kwds)
-    if isinstance(prop, str):
-      prop = self._marg_cond[prop]
-    self.set_prop_obj(prop)
-    self._prop = prop._prop
-    return self._prop
+  def leafs_roots(self, spec=None):
+    """ Returns a proxy object from _subfields. """
+    if spec is None:
+      return self._subfields
+    if not isinstance(spec, str) and spec not in self._subfields.values(): 
+      return False
+    if isinstance(spec, str):
+      assert spec in self._subfields, \
+          '{} absent from {}'.format(spec, self._name)
+      return self._subfields[spec]
+    return spec
 
 #-------------------------------------------------------------------------------
   def set_delta(self, delta=None, *args, **kwds):
-    if not isinstance(delta, str) and delta not in self._marg_cond.values(): 
+    _delta = self.leafs_roots(delta)
+    if not _delta:
       return super().set_delta(delta, *args, **kwds)
-    if isinstance(delta, str):
-      delta = self._marg_cond[delta]
-    self.set_prop_obj(delta)
-    self._delta = delta._delta
-    self._delta_args = delta._delta_args
-    self._delta_kwds = delta._delta_kwds
-    self._delta_type = delta._delta_type
-    self._spherise = delta._spherise
+    self.set_prop_obj(_delta)
+    self._delta = _delta.delta
+    self._delta_args = _delta._delta_args
+    self._delta_kwds = _delta._delta_kwds
+    self._delta_type = _delta._delta_type
+    self._spherise = _delta._spherise
     return self._delta
 
 #-------------------------------------------------------------------------------
-  def set_tran(self, tran=None, *args, **kwds):
-    if not isinstance(tran, str) and tran not in self._marg_cond.values(): 
-      return super().set_tran(tran, *args, **kwds)
-    if isinstance(tran, str):
-      tran = self._marg_cond[tran]
-    self.set_prop_obj(tran)
-    self._tran = tran._tran
-    return self._tran
-
-#-------------------------------------------------------------------------------
-  def set_tfun(self, tfun=None, *args, **kwds):
-    if not isinstance(tfun, str) and tfun not in self._marg_cond.values(): 
-      return super().set_tfun(tfun, *args, **kwds)
-    if isinstance(tfun, str):
-      tfun = self._marg_cond[tfun]
-    self.set_prop_obj(tfun)
-    self._tfun = tfun._tfun
-    return self._tfun
-
-#-------------------------------------------------------------------------------
-  def set_cfun(self, cfun=None, *args, **kwds):
-    if not isinstance(cfun, str) and cfun not in self._marg_cond.values(): 
-      return super().set_cfun(cfun, *args, **kwds)
-    if isinstance(cfun, str):
-      cfun = self._marg_cond[cfun]
-    self.set_prop_obj(cfun)
-    self._cfun = cfun._cfun
-    self._cfun_lud = cfun._cfun_lud
-    return self._cfun
-
-#-------------------------------------------------------------------------------
   def eval_dist_name(self, values, suffix=None):
     if suffix is not None:
       return super().eval_dist_name(values, suffix)
-    keys = self._keys 
+    keys = self._keylist 
     vals = collections.OrderedDict()
     if not isinstance(vals, dict):
       vals.update({key: vals for key in keys})
     else:
       for key, val in values.items():
         if ',' in key:
           subkeys = key.split(',')
           for i, subkey in enumerate(subkeys):
             vals.update({subkey: val[i]})
         else:
           vals.update({key: val})
-      for key in self._keys:
+      for key in self._keylist:
         if key not in vals.keys():
           vals.update({key: None})
     marg_vals = collections.OrderedDict()
-    if self._marg:
-      for key in self._marg.ret_keys():
+    if self._leafs:
+      for key in self._leafs.keylist:
         if key in keys:
           marg_vals.update({key: vals[key]})
     cond_vals = collections.OrderedDict()
-    if self._cond:
-      for key in self._cond.ret_keys():
+    if self._roots:
+      for key in self._roots.keylist:
         if key in keys:
           cond_vals.update({key: vals[key]})
-    marg_dist_name = self._marg.eval_dist_name(marg_vals)
-    cond_dist_name = '' if not self._cond else \
-                     self._cond.eval_dist_name(cond_vals)
+    marg_dist_name = self._leafs.eval_dist_name(marg_vals)
+    cond_dist_name = '' if not self._roots else \
+                     self._roots.eval_dist_name(cond_vals)
     dist_name = marg_dist_name
     if len(cond_dist_name):
       dist_name += "|{}".format(cond_dist_name)
     return dist_name
 
 #-------------------------------------------------------------------------------
-  def ret_marg(self):
-    return self._marg
-
-#-------------------------------------------------------------------------------
-  def ret_cond(self):
-    return self._cond
-
-#-------------------------------------------------------------------------------
-  def set_rvs(self, *args):
+  def set_vars(self, *args):
     raise NotImplementedError()
 
 #-------------------------------------------------------------------------------
-  def add_rv(self, rv):
+  def add_var(self, rv):
     raise NotImplementedError()
 
 #-------------------------------------------------------------------------------
   def eval_marg_prod(self, samples):
     raise NotImplementedError()
 
 #-------------------------------------------------------------------------------
-  def eval_vals(self, *args, _skip_parsing=False, **kwds):
-    assert self._marg, "No marginal stochastic random variables defined"
-    return super().eval_vals(*args, _skip_parsing=_skip_parsing, **kwds)
+  def eval_deps(self, *args, _skip_parsing=False, **kwds):
+    if self._deps is None:
+      return None
+    vals = self.parse_args(*args, **kwds) if not _skip_parsing else args[0]
+    for key, val in self._deps.items():
+      output = val(vals)
+      evals, dims = None, None
+      if isinstance(output, dict):
+        evals = output
+      elif not isinstance(output, tuple):
+        raise TypeError("Unrecognised type {} for output for dependency {}".\
+                        format(type(output), key))
+      else: 
+        evals = output[0] 
+        assert isinstance(evals, dict),\
+            "Unrecognised dependency evaluation output type: {}".format(
+                type(evals))
+        assert len(output) < 3, \
+            "Maximum for 3 outputs from dependency evaluation"
+        for argout in output:
+          if isinstance(argout, dict):
+            assert dims is None, "Output ambiguous for dimensionality"
+            dims = argout
+    return vals
+
+#-------------------------------------------------------------------------------
+  def eval_func(self, *args, _skip_parsing=False, **kwds):
+    """ Evaluates leaf values from immediate predecessors """
+    assert len(self._func), \
+        "No functions defined for functional {}".format(self._func)
+    vals = self.parse_args(*args, **kwds) if not _skip_parsing else args[0]
+
+    # Can only evaluate architectures
+    if not self._arch: 
+      return vals
+
+    # Iconics should be evaluable directly:
+    if self._func.isiconic:
+      pass
+
+#-------------------------------------------------------------------------------
+  def evaluate(self, *args, _skip_parsing=False, **kwds):
+    """ Returns evaluation for Field() if there are no dependencies otherwise
+    evaluation is based on functionals defined for each Dependences.
+    """
+    assert self._leafs, "No leaf stochastic random variables defined"
+    if not self._arch or not self._func or not len(self._func):
+      return super().evaluate(*args, _skip_parsing=_skip_parsing, **kwds)
+    
 
 #-------------------------------------------------------------------------------
   def __call__(self, *args, **kwds):
-    """ Like RJ.__call__ but optionally takes 'joint' keyword """
-
-    if self._rvs is None:
-      return None
-    joint = False if 'joint' not in kwds else kwds.pop('joint')
-    dist = super().__call__(*args, **kwds)
-    if not joint:
-      return dist
-    vals = dist.ret_cond_vals()
-    cond_dist = self._cond(vals)
-    return product(cond_dist, dist)
+    """ Currently calls Field.__call__ """
+    return super().__call__(*args, **kwds)
 
 #-------------------------------------------------------------------------------
   def step(self, *args, **kwds):
     prop_obj = self._prop_obj
-    if prop_obj is None and (self._tran is not None or self._prop is not None):
+    if prop_obj is None:
       return super().step(*args, **kwds)
     prop_obj = prop_obj or self._def_prop_obj
     return prop_obj.step(*args, **kwds)
 
 #-------------------------------------------------------------------------------
-  def propose(self, *args, **kwds):
-    prop_obj = self._prop_obj
-    if prop_obj is None and (self._tran is not None or self._prop is not None):
-      return super().propose(*args, **kwds)
-    prop_obj = prop_obj or self._def_prop_obj
-    return prop_obj.propose(*args, **kwds)
-
-#-------------------------------------------------------------------------------
-  def parse_pred_args(self, arg):
-    obj = None
-    if self._tran == 'marg': obj = self._marg
-    if self._tran == 'cond': obj = self._cond
-    if obj is None:
-      return self.parse_args(args)
-    if not isinstance(arg, dict):
-      return obj.parse_args(args)
-    keyset = obj.ret_keyset()
-    pred = collections.OrderedDict({key: val for key, val in arg.items() 
-                                             if key in keyset})
-    return obj.parse_args(pred)
-
-#-------------------------------------------------------------------------------
-  def sample(self, *args, **kwds):
-    """ A function for unconditional and conditional sampling. For conditional
-    sampling, use RF.set_delta() to set the delta specification. if neither
-    set_prob() nor set_tran() are set, then opqr inputs are disallowed and this
-    function outputs a normal __call__(). Otherwise this function returns a 
-    namedtuple-generated opqr object that can be accessed using opqr.p or 
-    opqr[1] for the probability distribution and opqr.q or opqr[2] for the 
-    proposal. Unavailable values are set to None. 
-    
-    If using set_prop() the output opqr comprises:
-
-    opqr.o: None
-    opqr.p: Probability distribution 
-    opqr.q: Proposition distribution
-    opqr.r: None
-
-    If using set_tran() the output opqr comprises:
-
-    opqr.o: Probability distribution for predecessor
-    opqr.p: Probability distribution for successor
-    opqr.q: Proposition distribution (successor | predecessor)
-    opqr.r: None [for now, reserved for proposition (predecessor | successor)]
-
-    If inputting and opqr object using set_prop(), the values for performing any
-    delta operations are taken from the entered proposition distribution. If using
-    set_prop(), optional keyword flag suffix=False may be used to remove prime
-    notation in keys.
-
-    An optional argument args[1] can included in order to input a dictionary
-    of values beyond outside the proposition distribution required to evaluate
-    the probability distribution.
-    """
-    if not args:
-      args = {0},
-    assert len(args) < 3, "Maximum of two positional arguments"
-    if self._tran is None and not self._unit_tran:
-      if self._prop is None:
-        assert not isinstance(args[0], self.opqr),\
-            "Cannot input opqr object with neither set_prob() nor set_tran() set"
-        return self.__call__(*args, **kwds)
-      return self._sample_prop(*args, **kwds)
-    return self._sample_tran(*args, **kwds)
-
-#-------------------------------------------------------------------------------
-  def _sample_prop(self, *args, **kwds):
-
-    # Extract suffix status; it is latter popped by propose()
-    suffix = "'" if 'suffix' not in kwds else kwds['suffix'] 
-
-    # Non-opqr argument requires no parsing
-    if not isinstance(args[0], self.opqr):
-      prop = self.propose(args[0], **kwds)
-
-    # Otherwise parse:
-    else:
-      assert args[0].q is not None, \
-          "An input opqr argument must contain a non-None value for opqr.q"
-      vals = desuffix(args[0].q.vals)
-      prop = self.propose(vals, **kwds)
-
-    # Evaluation of probability
-    vals = desuffix(prop.vals)
-    if len(args) > 1:
-      assert isinstance(args[1], dict),\
-          "Second argument must be dictionary type, not {}".format(
-              type(args[1]))
-      vals.update(args[1])
-    call = self.__call__(vals, **kwds)
-
-    return self.opqr(None, call, prop, None)
-
-#-------------------------------------------------------------------------------
-  def _sample_tran(self, *args, **kwds):
-    assert 'suffix' not in kwds, \
-        "Disallowed keyword 'suffix' when using set_tran()"
-
-    # Original probability distribution, proposal, and revp defaults to None
-    orig = None
-    prop = None
-    revp = None
-
-    # Non-opqr argument requires no parsing
-    if not isinstance(args[0], self.opqr):
-      prop = self.step(args[0], **kwds)
-
-    # Otherwise parse successor:
-    else:
-      dist = args[0].q
-      orig = args[0].p
-      assert dist is not None, \
-          "An input opqr argument must contain a non-None value for opqr.q"
-      vals = get_suffixed(dist.vals)
-      prop = self.step(vals, **kwds)
-
-    # Evaluate reverse proposal if transition function not symmetric
-    if not self._sym_tran and not self._unit_tran:
-      revp = self.reval_tran(prop)
-
-    # Extract values evaluating probability
-    vals = get_suffixed(prop.vals)
-    if len(args) > 1:
-      assert isinstance(args[1], dict),\
-          "Second argument must be dictionary type, not {}".format(
-              type(args[1]))
-      vals.update(args[1])
-    prob = self.__call__(vals, **kwds)
-
-    return self.opqr(orig, prob, prop, revp)
-
-#-------------------------------------------------------------------------------
-  def __getitem__(self, key):
-    if isinstance(key, str):
-      if key not in self._keys:
-        return None
-      key = self._keys.index(key)
-    return self._rvs[key]
-
-#-------------------------------------------------------------------------------
-  def __mul__(self, other):
-    from probayes.rv import RV
-    from probayes.rj import RJ
-
-    marg = self.ret_marg().ret_rvs()
-    cond = self.ret_cond().ret_rvs()
-    if isinstance(other, RF):
-      marg = marg + other.ret_marg().ret_rvs()
-      cond = cond + other.ret_cond().ret_rvs()
-      return RF(marg, cond)
-
-    if isinstance(other, RJ):
-      marg = marg + other.ret_rvs()
-      return RF(marg, cond)
-
-    if isinstance(other, RV):
-      marg = marg + [other]
-      return RF(marg, cond)
-
-    raise TypeError("Unrecognised post-operand type {}".format(type(other)))
-
-#-------------------------------------------------------------------------------
-  def __truediv__(self, other):
-    from probayes.rv import RV
-    from probayes.rj import RJ
-
-    marg = self.ret_marg().ret_rvs()
-    cond = self.ret_cond().ret_rvs()
-    if isinstance(other, RF):
-      marg = marg + other.ret_cond().ret_rvs()
-      cond = cond + other.ret_marg().ret_rvs()
-      return RF(marg, cond)
-
-    if isinstance(other, RJ):
-      cond = cond + other.ret_rvs()
-      return RF(marg, cond)
-
-    if isinstance(other, RV):
-      cond = cond + [self]
-      return RF(marg, cond)
-
-    raise TypeError("Unrecognised post-operand type {}".format(type(other)))
-
-#-------------------------------------------------------------------------------
```

### Comparing `probayes-0.0.3/probayes/rj.py` & `probayes-0.0.4/probayes/field.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,393 +1,374 @@
 """
-A random junction comprises a collection of a random variables that 
-participate in a joint probability distribution function.
+A field is a collection of a functionally-related variables without explictly
+directional dependences.
 """
 #-------------------------------------------------------------------------------
-import warnings
 import collections
 import numpy as np
-import scipy.stats
 
-from probayes.rv import RV
-from probayes.dist import Dist
-from probayes.dist_utils import margcond_str
-from probayes.vtypes import isscalar, isunitsetint, issingleton, isdimensionless, \
-                            revtype, uniform
-from probayes.pscales import iscomplex, real_sqrt, prod_rule, \
-                         rescale, eval_pscale, prod_pscale
-from probayes.rj_utils import rv_prod_rule, call_scipy_prob, sample_cond_cov
-from probayes.func import Func
-from probayes.cond_cov import CondCov
-
-#-------------------------------------------------------------------------------
-class RJ:
-  # Public
-  delta = None
+from probayes.variable import Variable
+from probayes.variable_utils import parse_as_str_dict
+from probayes.vtypes import isscalar, isunitsetint, issingleton, isdimensionless
+from probayes.pscales import real_sqrt
+from probayes.ops import and_op, or_op
+from probayes.expression import Expression
+from probayes.functional import NX_UNDIRECTED_GRAPH
+from probayes.distribution import Distribution
+
+#-------------------------------------------------------------------------------
+class Field (NX_UNDIRECTED_GRAPH):
+  """
+  A field is a collection of a variables that are functionally inter-related
+  without explicit directional dependencies. This lack of directionality means
+  Field does not support Functionals. 
+  """
 
   # Protected
-  _name = None       # Cannot be set externally
-  _rvs = None        # Dict of random variables
-  _nrvs = None      
-  _keys = None      
-  _keyset = None    
-  _defiid = None    
-  _pscale = None    
-  _prob = None      
-  _pscale = None    
-  _prop = None       # Non-transitional proposition function
+  _name = None       # Random field name cannot be set externally
+  _Delta = None      # A namedtuple generator for delta operations
+  _vars = None       # OrderedDict of variables
+  _nvars = None      # Number of variables
+  _unitvar = None    # Boolean flag for one variable
+  _anyfloat = None   # Boolean flag to denote if any variables are float type
+  _anystoch = None   # Boolean flag of whether any variable stochastic
+  _varlist = None    # List of variable objects
+  _keylist = None    # List of keys of variable names
+  _keyset = None     # Unordered set of keys of random variable names
   _delta = None      # Delta function (to replace step)
   _delta_args = None # Optional delta args (must be dictionaries)
   _delta_kwds = None # Optional delta kwds
-  _delta_type = None # Same as delta
-  _tran = None       # Transitional proposition function
-  _tfun = None       # CDF/IDF of transition function
-  _t1vt = None       # Flag for transitional conditioning one variable at a time
-  _cfun = None       # Covariance function
-  _length = None     # Length of junction
-  _lengths = None    # Lengths of RVs
-  _sym_tran = None
-  _cfun_lud = None
-  _spherise = None
-
-  # Private
-  __isscalar = None
-  __callable = None
-  __cond_mod = None
-  __cond_cov = None
-
-#-------------------------------------------------------------------------------
-  def __init__(self, *args):
-    self.set_rvs(*args)
-    self.set_prob()
-    self.set_prop()
+  _delta_type = None # Proxy for delta used for casting
+  _length = None     # Length of field
+  _lengths = None    # Lengths of Variables
+  _leafs = None      # Field of Variables that do not condition others (for SD)
+  _roots = None      # Field of Vairables not dependent on others (for SD)
+  _stems = None      # OrderedDict of latent Variables (for Dependencies)
+  _is_stochastic = False      # Flag of whether stochastic
+  _func = False      # Functional
+
+#-------------------------------------------------------------------------------
+  @property
+  def is_stochastic(self):
+    return self._is_stochastic
+
+  def __init__(self, *args): # over-rides NX_GRAPH.__init__()
+    """ Initialises a random field with Variables for in args. See set_vars(). """
+    super().__init__()
+    self.set_vars(*args)
     self.set_delta()
-    self.set_tran()
-    self.set_cfun()
-    self.set_t1vt()
 
 #-------------------------------------------------------------------------------
-  def set_rvs(self, *args):
-    if len(args) == 1 and isinstance(args[0], (RJ, dict, set, tuple, list)):
+  def add_node(self, *args, **kwds):
+    """ Direct adding of nodes disallowed """
+    raise NotImplementedError("Not implemented for this class")
+
+#-------------------------------------------------------------------------------
+  def add_node_from(self, *args, **kwds):
+    """ Direct adding of nodes disallowed """
+    raise NotImplementedError("Not implemented for this class")
+
+#-------------------------------------------------------------------------------
+  def remove_node(self, *args, **kwds):
+    """ Removal of nodes disallowed """
+    raise NotImplementedError("Not implemented for this class")
+
+#-------------------------------------------------------------------------------
+  def add_edge(self, *args, **kwds):
+    """ Direct adding of edges disallowed """
+    raise NotImplementedError("Not implemented for this class")
+
+#-------------------------------------------------------------------------------
+  def add_edges_from(self, *args, **kwds):
+    """ Direct adding of edges disallowed """
+    raise NotImplementedError("Not implemented for this class")
+
+#-------------------------------------------------------------------------------
+  @property
+  def leafs(self):
+    return self._leafs
+
+  @property
+  def stems(self):
+    return self._stems
+
+  @property
+  def roots(self):
+    return self._roots
+
+  def set_vars(self, *args):
+    """ Initialises a field with variables for each arg in args.
+
+    :param *args: each arg may be an Variable instance or the first arg may be a Field.
+    
+    """
+    self._leafs, self._stems, self._roots = self, None, None
+    if len(args) == 1 and isinstance(args[0], (Variable, set, tuple, list)):
       args = args[0]
     else:
       args = tuple(args)
-    self.add_rv(args)
-    return self.ret_rvs()
+    self.add_var(args)
 
 #-------------------------------------------------------------------------------
-  def add_rv(self, rv):
-    assert self._prob is None, \
-      "Cannot assign new randon variables after specifying joint/condition prob"
-    if self._rvs is None:
-      self._rvs = collections.OrderedDict()
-    if isinstance(rv, (RJ, dict, set, tuple, list)):
-      rvs = rv
-      if isinstance(rvs, RJ):
-        rvs = rvs.ret_rvs()
-      if isinstance(rvs, dict):
-        rvs = rvs.values()
-      [self.add_rv(rv) for rv in rvs]
+  def add_var(self, var):
+    """ Adds one or more variables to the field.
+
+    :param var: a Variable or Field instance, or a list/tuple of Variable instances.
+    """
+    variables = []
+    if isinstance(var, (Field, dict, set, tuple, list)):
+      variables = var
+      if isinstance(variables, Field):
+        variables = variables.varlist
+      elif isinstance(variables, dict):
+        variables = list(variables.values())
+    for var in variables:
+      assert isinstance(var, Variable), \
+          "Input not a variable instance but of type: {}".format(type(var))
+      if self._nvars:
+        assert var not in list(self.nodes), \
+            "Existing variable {} already present in collection".format(var)
+      super().add_node(var)
     else:
-      assert isinstance(rv, RV), \
-          "Input not a RV instance but of type: {}".format(type(rv))
-      key = rv.ret_name()
-      assert key not in self._rvs.keys(), \
-          "Existing RV name {} already present in collection".format(rv_name)
-      self._rvs.update({key: rv})
-    self._nrvs = len(self._rvs)
-    self._keys = list(self._rvs.keys())
-    self._keyset = set(self._keys)
-    self._defiid = self._keyset
-    self._name = ','.join(self._keys)
-    self._id = '_and_'.join(self._keys)
+      assert isinstance(var, Variable), \
+          "Input not a variable instance but of type: {}".format(type(var))
+      if self._nvars:
+        assert var not in list(self.nodes), \
+            "Existing variable {} already present in collection".format(var)
+      super().add_node(var)
+    self._refresh()
+
+#-------------------------------------------------------------------------------
+  @property
+  def vars(self):
+    return self._vars
+
+  @property
+  def nvars(self):
+    return self._nvars
+
+  @property
+  def unitvar(self):
+    return self._unitvar
+
+  @property
+  def anyfloat(self):
+    return self._anyfloat
+
+  @property
+  def anystoch(self):
+    return self._anystoch
+
+  def __len__(self):
+    return self._nvars
+
+  def __bool__(self):
+    if self._nvars:
+      return True
+    return False
+
+  @property
+  def varlist(self):
+    return self._varlist
+
+  @property
+  def keylist(self):
+    return self._keylist
+
+  @property
+  def keyset(self):
+    return self._keyset
+
+  @property
+  def name(self):
+    return self._name
+
+  @property
+  def id(self):
+    return self._id
+
+  @property
+  def Delta(self):
+    return self._Delta
+
+  def _refresh(self):
+    """ Updates Variable summary objects, Field name and id, and delta factory. """
+    self._vars = collections.OrderedDict({var.name: var for var in list(self.nodes)})
+    self._nvars = self.number_of_nodes()
+    self._unitvar = self._nvars == 1
+    self._varlist = list(self._vars.values())
+    self._anyfloat = any([var.vtype is float for var in self._varlist])
+    self._anystoch = any([var.is_stochastic for var in self._varlist])
+    if not self._is_stochastic:
+      assert not self._anystoch,\
+          "Stochastic variables cannot contribute to a non-stochastic field"
+    self._keylist = list(self._vars.keys())
+    self._keyset = frozenset(self._keylist)
+    self._defiid = self._leafs.keylist
+    self._name = ','.join(self._keylist)
+    self._id = '_and_'.join(self._keylist)
     if self._id:
-      self.delta = collections.namedtuple('ð', self._keys)
-      self._delta_type = self.delta
-    self.set_pscale()
+      self._Delta = collections.namedtuple('ð', self._keylist)
+      self._delta_type = self._Delta
     self.eval_length()
-    return self._nrvs
 
 #-------------------------------------------------------------------------------
-  def set_prob(self, prob=None, *args, **kwds):
-    # Set joint probability distribution function
-    kwds = dict(kwds)
-    if 'pscale' in kwds:
-      pscale = kwds.pop('pscale')
-      self.set_pscale(pscale)
-    self.__callable = None
-    self.__isscalar = None
-    self._prob = prob
-    if self._prob is None:
-      return self.__callable
-    self._prob = Func(self._prob, *args, **kwds)
-    self.__callable = self._prob.ret_callable()
-    self.__isscalar = self._prob.ret_isscalar()
-    return self.__callable
-
-#-------------------------------------------------------------------------------
-  def set_pscale(self, pscale=None):
-    if pscale is not None or not self._nrvs:
-      self._pscale = eval_pscale(pscale)
-      return self._pscale
-    rvs = self.ret_rvs(aslist=True)
-    pscales = [rv.ret_pscale() for rv in rvs]
-    self._pscale = prod_pscale(pscales)
-    return self._pscale
-
-#-------------------------------------------------------------------------------
-  def set_prop(self, prop=None, *args, **kwds):
-    # Set joint proposition function
-    self._prop = prop
-    if self._prop is None:
-      return
-    assert self._tran is None, \
-        "Cannot assign both proposition and transition probabilities"
-    self._prop = Func(self._prop, *args, **kwds)
+  @property
+  def delta(self):
+    """ Returns the default delta object if specified """
+    return self._delta
 
-#-------------------------------------------------------------------------------
   def set_delta(self, delta=None, *args, **kwds):
-    """ Input argument delta may be:
+    """ Sets the default delta function or operation.
+
+    :param delta: the delta function or operation (see below)
+    :param *args: optional arguments to pass if delta is callable.
+    :param **kwds: optional keywords to pass if delta is callable.
+
+    The input delta may be:
 
     1. A callable function (for which args and kwds are passed on as usual).
-    2. An sj.delta instance (this defaults all RV deltas).
-    3. A dictionary for RVs, this is converted to an sj.delta.
+    2. An Variable.Delta instance (this defaults all Variable Deltas).
+    3. A dictionary for Variables, this is converted to an Field.Delta.
     4. A scalar that may contained in a list or tuple:
       a) No container - the scalar is treated as a fixed delta.
-      b) List - delta is uniformly and independently sampled across RVs.
-      c) Tuple - delta is spherically sampled across RVs.
+      b) List - delta is uniformly and independently sampled across Variabless.
+      c) Tuple - delta is spherically sampled across Variables.
 
       For non-tuples, an optional argument (args[0]) can be included as a 
-      dictionary to specify by RV-name deltas following the above conventions
-      except their values are not subject to scaling even if 'scale' is given,
-      but they are subject to bounding if 'bound' is specified.
+      dictionary to specify by Variable-name deltas following the above 
+      conventions except their values are not subject to scaling even if 
+      'scale' is given, but they are subject to bounding if 'bound' is 
+      specified.
 
     For setting types 2-4, optional keywords are (default False):
-      'scale': Flag to denote scaling deltas to RV lengths
-      'bound': Flag to constrain delta effects to RV bounds (None bounces)
+      'scale': Flag to denote scaling deltas to Variable lengths
+      'bound': Flag to constrain delta effects to Variable bounds (None bounces)
       
     """
     self._delta = delta
     self._delta_args = args
     self._delta_kwds = dict(kwds)
     self._spherise = {}
     if self._delta is None:
       return
     elif callable(self._delta):
-      self._delta = Func(self._delta, *args, **kwds)
+      self._delta = Expression(self._delta, *args, **kwds)
       return
 
     # Default scale and bound
     if 'scale' not in self._delta_kwds:
       self._delta_kwds.update({'scale': False})
     if 'bound' not in self._delta_kwds:
       self._delta_kwds.update({'bound': False})
+    scale = self._delta_kwds['scale']
+    bound = self._delta_kwds['bound']
 
     # Handle deltas and dictionaries
     if isinstance(self._delta, dict):
       self._delta = self._delta_type(**self._delta)
     if isinstance(delta, self._delta_type):
       assert not args, \
         "Optional args prohibited for dict/delta instance inputs"
-      rvs = self.ret_rvs(aslist=True)
-      for i, rv in enumerate(rvs):
-        rv.set_delta(self._delta[i], scale=scale, bound=bound)
+      for i, var in enumerate(self._varlist):
+        var.set_delta(self._delta[i], scale=scale, bound=bound)
       return
 
     # Default scale and bound and check args
-    scale = self._delta_kwds['scale']
-    bound = self._delta_kwds['bound']
     if self._delta_args:
       assert len(self._delta_args) == 1, \
           "Optional positional arguments must comprises a single dict"
       unscale = self._delta_args[0]
       assert isinstance(unscale, dict), \
           "Optional positional arguments must comprises a single dict"
 
     # Non tuples can be converted to deltas; can pre-scale here
     if not isinstance(self._delta, tuple):
-      scaling = self._lengths
       delta = self._delta 
       urand = isinstance(delta, list)
       if urand:
         assert len(delta) == 1, "List delta requires a single element"
         delta = delta[0]
-      deltas = {key: delta for key in self._keys}
+      deltas = {key: delta for key in self._keylist}
       unscale = {} if not self._delta_args else self._delta_args[0]
       deltas.update(unscale)
       delta_dict = collections.OrderedDict(deltas)
       for i, (key, val) in enumerate(deltas.items()):
         delta = val
         if scale and key not in unscale:
           assert np.isfinite(self._lengths[i]), \
-              "Cannot scale by infinite length for RV {}".format(key)
+              "Cannot scale by infinite length for Variable {}".format(key)
           delta = val * self._lengths[i]
         if urand:
           delta = [delta]
         delta_dict.update({key: delta})
       self._delta = self._delta_type(**delta_dict)
-      rvs = self.ret_rvs(aslist=True)
-      for i, rv in enumerate(rvs):
-        rv.set_delta(self._delta[i], scale=False, bound=bound)
+      for i, var in enumerate(self._varlist):
+        var.set_delta(self._delta[i], scale=False, bound=bound)
 
     # Tuple deltas must be evaluated on-the-fly and cannot be pre-scaled
     else:
       unscale = {} if not self._delta_args else self._delta_args[0]
       self._spherise = {}
-      for i, key in enumerate(self._keys):
+      for i, key in enumerate(self._keylist):
         if key not in unscale.keys():
           length = self._lengths[i]
           assert np.isfinite(length), \
-              "Cannot spherise RV {} with infinite length".format(key)
+              "Cannot spherise Variable {} with infinite length".format(key)
           self._spherise.update({key: length})
 
 #-------------------------------------------------------------------------------
-  def set_tran(self, tran=None, *args, **kwds):
-    # Set transition function
-    self._tran = tran
-    self._sym_tran = False
-    if self._tran is None:
-      return
-    assert self._prop is None, \
-        "Cannot assign both proposition and transition probabilities"
-    self._tran = Func(self._tran, *args, **kwds)
-    self._sym_tran = not self._tran.ret_istuple()
-    if self._tran.ret_isscipy():
-      scipyobj = self._tran.ret_scipyobj()
-      self.set_tfun(self._tran, scipyobj=self._tran.ret_scipyobj())
-
-#-------------------------------------------------------------------------------
-  def set_tfun(self, tfun=None, *args, **kwds):
-    # Set cdf and inverse cdf of transitional for conditional sampling
-    scipyobj = None if 'scipyobj' not in kwds else kwds['scipyobj']
-    self._tfun = tfun 
-    if self._tfun is None:
-      return
-    if scipyobj is None:
-       self._tfun = Func(self._tfun, *args, **kwds)
-       return
-    rvs = self.ret_rvs(aslist=True)
-    lims = np.array([rv.ret_lims() for rv in rvs])
-    mean = scipyobj.mean
-    cov = scipyobj.cov
-    self._cond_cov = CondCov(mean, cov, lims)
-    scipy_cond = sample_cond_cov if self._sym_tran else \
-                 (sample_cond_cov, sample_cond_cov)
-    self._tfun = Func(scipy_cond, cond_cov=self._cond_cov)
-
-#-------------------------------------------------------------------------------
-  def set_t1vt(self, t1vt=False):
-    self._t1vt = t1vt
-
-#-------------------------------------------------------------------------------
-  def set_cfun(self, cfun=None, *args, **kwds):
-    # Set covariance function for kernel-based sampling
-    self._cfun = cfun
-    self._cfun_lud = None
-    if self._cfun is None:
-      return
-    self._cfun = Func(self._cfun, *args, **kwds)
-    if not self._cfun.ret_callable():
-      message = "Non-callable cfun objects must be a square 2D Numpy array " + \
-                "of size corresponding to number of variables {}".format(self._nrvs)
-      assert isinstance(cfun, np.ndarray), message
-      assert cfun.ndim == 2, message
-      assert np.all(np.array(cfun.shape) == self._nrvs), message
-      self._cfun_lud = np.linalg.cholesky(cfun)
-
-#-------------------------------------------------------------------------------
-  def ret_rvs(self, aslist=True):
-    # Defaulting aslist=True plays more nicely with inheriting classes
-    rvs = self._rvs
-    if aslist:
-      if isinstance(rvs, dict):
-        rvs = list(rvs.values())
-      assert isinstance(rvs, list), "RVs not a recognised variable type: {}".\
-                                    format(type(rvs))
-    return rvs
-
-#-------------------------------------------------------------------------------
   def eval_length(self):
-    rvs = self.ret_rvs(aslist=True)
-    self._lengths = np.array([rv.ret_length() for rv in rvs], dtype=float)
-    self._length = np.sqrt(np.sum(self._lengths))
-    return self._length
-
-#-------------------------------------------------------------------------------
-  def ret_length(self):
+    """ Evaluates and returns the joint length of the field. """
+    self._lengths = np.array([var.length for var in self._varlist], 
+                             dtype=float)
+    self._length = np.sqrt(np.sum(self._lengths**2))
     return self._length
 
 #-------------------------------------------------------------------------------
-  def ret_name(self):
-    return self._name
-
-#-------------------------------------------------------------------------------
-  def ret_id(self):
-    return self._id
-#-------------------------------------------------------------------------------
-  def ret_nrvs(self):
-    return self._nrvs
-
-#-------------------------------------------------------------------------------
-  def ret_keys(self):
-    return self._keys
-
-#-------------------------------------------------------------------------------
-  def ret_keyset(self):
-    return self._keyset
-
-#-------------------------------------------------------------------------------
-  def ret_pscale(self):
-    return self._pscale
-
-#-------------------------------------------------------------------------------
   def parse_args(self, *args, **kwds):
     """ Returns (values, iid) from *args and **kwds """
-    args = tuple(args)
-    kwds = dict(kwds)
     pass_all = False if 'pass_all' not in kwds else kwds.pop('pass_all')
-    
-    if not args and not kwds:
-      args = (None,)
-    if args:
-      assert len(args) == 1 and not kwds, \
-        "With order specified, calls argument must be a single " + \
-              "dictionary or keywords only"
-      kwds = dict(args[0]) if isinstance(args[0], dict) else \
-             ({key: args[0] for key in self._keys})
-
-    elif kwds:
-      assert not args, \
-        "With order specified, calls argument must be a single " + \
-              "dictionary or keywords only"
-    values = dict(kwds)
+    values = parse_as_str_dict(*args, **kwds)
     seen_keys = []
     for key, val in values.items():
       count_comma = key.count(',')
       if count_comma:
         seen_keys.extend(key.split(','))
         if isinstance(val, (tuple, list)):
           assert len(val) == count_comma+1, \
               "Mismatch in key specification {} and number of values {}".\
               format(key, len(val))
         else:
           values.update({key: [val] * (count_comma+1)})
       else:
         seen_keys.append(key)
       if not pass_all:
-        assert seen_keys[-1] in self._keys, \
-            "Unrecognised key {} among available RVs {}".format(
-                seen_keys[-1], self._keys)
-    for key in self._keys:
+        assert seen_keys[-1] in self._keyset, \
+            "Unrecognised key {} among available Variables {}".format(
+                seen_keys[-1], self._keyset)
+
+    # Default values
+    def_val = None
+    if self._anyfloat:
+      if not len(values):
+        def_val = {0}
+      else:
+        def_val = {0}
+        for val in values.values():
+          if isunitsetint(val):
+            if val == {0}:
+              def_val = None
+    for key in self._keylist:
       if key not in seen_keys:
-        values.update({key: None})
+        values.update({key: def_val})
     if pass_all:
       list_keys = list(values.keys())
       for key in list_keys:
-        if key not in self._keys:
+        if key not in self._keylist:
           values.pop(key)
 
     return values
 
 #-------------------------------------------------------------------------------
   def eval_dist_name(self, values=None, suffix=None):
     # Evaluates the string used to set the distribution name
@@ -396,50 +377,49 @@
       for key, val in values.items():
         if ',' in key:
           subkeys = key.split(',')
           for i, subkey in enumerate(subkeys):
             vals.update({subkey: val[i]})
         else:
           vals.update({key: val})
-      for key in self._keys:
+      for key in self._keylist:
         if key not in vals.keys():
           vals.update({key: None})
     else:
-      vals.update({key: values for key in keys})
-    rvs = self.ret_rvs()
-    rv_dist_names = [rv.eval_dist_name(vals[rv.ret_name()], suffix) \
-                     for rv in rvs]
-    dist_name = ','.join(rv_dist_names)
+      vals.update({key: values for key in self._keylist})
+    var_dist_names = [var.eval_dist_name(vals[var.name], suffix) \
+                     for var in self._varlist]
+    dist_name = ','.join(var_dist_names)
     return dist_name
 
 #-------------------------------------------------------------------------------
-  def eval_vals(self, *args, _skip_parsing=False, min_dim=0, **kwds):
+  def evaluate(self, *args, _skip_parsing=False, min_dim=0, **kwds):
     """ 
     Keep args and kwds since could be called externally. This ignores self._prob.
     """
     values = self.parse_args(*args, **kwds) if not _skip_parsing else args[0]
-    dims = {}
+    dims = collections.OrderedDict()
     
     # Don't reshape if all scalars (and therefore by definition no shared keys)
     if all([np.isscalar(value) for value in values.values()]): # use np.scalar
       return values, dims
 
-    # Create reference mapping for shared keys across rvs
-    values_ref = collections.OrderedDict({key: [key, None] for key in self._keys})
+    # Create reference mapping for shared keys across vars
+    values_ref = collections.OrderedDict({key: [key, None] for key in self._keylist})
     for key in values.keys():
       if ',' in key:
         subkeys = key.split(',')
         for i, subkey in enumerate(subkeys):
           values_ref[subkey] = [key, i]
 
-    # Share dimensions for joint variables and do not dimension scalars
+    # Share dimensions for joint variables and do not dimensionalise scalars
     ndim = min_dim
-    dims = collections.OrderedDict({key: None for key in self._keys})
+    dims = collections.OrderedDict({key: None for key in self._keylist})
     seen_keys = set()
-    for i, key in enumerate(self._keys):
+    for i, key in enumerate(self._keylist):
       new_dim = False
       if values_ref[key][1] is None: # i.e. not shared
         if not isdimensionless(values[key]):
           dims[key] = ndim
           new_dim = True
         seen_keys.add(key)
       elif key not in seen_keys:
@@ -454,111 +434,76 @@
         ndim += 1
 
     # Reshape
     vdims = [dim for dim in dims.values() if dim is not None]
     ndims = max(vdims) + 1 if len(vdims) else 0
     ones_ndims = np.ones(ndims, dtype=int)
     vals = collections.OrderedDict()
-    rvs = self.ret_rvs(aslist=True)
-    for i, rv in enumerate(rvs):
-      key = rv.ret_name()
+    for i, var in enumerate(self._varlist):
+      key = var.name
       reshape = True
       if key in values.keys():
         vals.update({key: values[key]})
         reshape = not np.isscalar(vals[key])
         if vals[key] is None or isinstance(vals[key], set):
-          vals[key] = rv.eval_vals(vals[key])
+          vals.update(var.evaluate(vals[key]))
       else:
         val_ref = values_ref[key]
         vals_val = values[val_ref[0]][val_ref[1]]
         if vals_val is None or isinstance(vals_val, set):
-          vals_val = rv.eval_vals(vals_val)
-        vals.update({key: vals_val})
+          vals.update(var.evaluate(vals_val))
+        else:
+          vals.update({key: vals_val})
       if reshape and not isscalar(vals[key]):
         re_shape = np.copy(ones_ndims)
         re_dim = dims[key]
         re_shape[re_dim] = vals[key].size
         vals[key] = vals[key].reshape(re_shape)
     
     # Remove dimensionality for singletons
-    for key in self._keys:
+    for key in self._keylist:
       if issingleton(vals[key]):
         dims[key] = None
     return vals, dims
 
 #-------------------------------------------------------------------------------
-  def eval_prob(self, values=None):
-    if values is None:
-      values = {}
-    assert isinstance(values, dict), "Input to eval_prob() requires values dict"
-    assert set(values.keys()) == self._keyset, \
-      "Sample dictionary keys {} mismatch with RV names {}".format(
-        values.keys(), self._keys())
-
-    # If not specified, treat as independent variables
-    if self._prob is None:
-      rvs = self.ret_rvs(aslist=True)
-      if len(rvs) == 1 and rvs[0]._prob is not None:
-        prob = rvs[0].eval_prob(values[rvs[0].ret_name()])
-      else:
-        prob, _ = rv_prod_rule(values, rvs=rvs, pscale=self._pscale)
-      return prob
-
-    # Otherwise distinguish between uncallable and callables
-    if not self.__callable:
-      return self._prob()
-    elif isinstance(self._prob, Func) and self._prob.ret_isscipy():
-      return call_scipy_prob(self._prob, self._pscale, values)
-    return self._prob(values)
-
-#-------------------------------------------------------------------------------
   def eval_delta(self, delta=None):
 
-    # Handle native delta types within RV deltas
+    # Handle native delta types within Variable deltas
     if delta is None: 
       if self._delta is None:
-        rvs = self.ret_rvs(aslist=True)
-        if len(rvs) == 1 and rvs[0]._delta is not None:
-          return rvs[0]._delta
+        variables = list(self._varlist)
+        if len(variables) == 1 and variables[0]._delta is not None:
+          return variables[0]._delta
         return None
-      elif isinstance(self._delta, Func):
+      elif isinstance(self._delta, Expression):
         delta = self._delta()
       elif isinstance(self._delta, self._delta_type):
         delta_dict = collections.OrderedDict()
-        rvs = self.ret_rvs(aslist=True)
-        for i, key in enumerate(self._keys):
-          delta_dict.update({key: rvs[i].eval_delta()})
+        variables = self._varlist
+        for i, key in enumerate(self._keylist):
+          delta_dict.update({key: variables[i].eval_delta()})
         delta = self._delta_type(**delta_dict)
       else:
         delta = self._delta
-    elif isinstance(delta, Func):
+    elif isinstance(delta, Expression):
       delta = delta()
     elif isinstance(delta, self._delta_type):
       delta_dict = collections.OrderedDict()
-      rvs = self.ret_rvs(aslist=True)
-      for i, key in enumerate(self._keys):
-        delta_dict.update({key: rvs[i].eval_delta(delta[i])})
+      variables = self.ret_vars(aslist=True)
+      for i, key in enumerate(self._keylist):
+        delta_dict.update({key: variables[i].eval_delta(delta[i])})
       delta = self._delta_type(**delta_dict)
 
     # Non spherical case
-    if not isinstance(self._delta_type, Func) and \
+    if not isinstance(self._delta_type, Expression) and \
          isinstance(delta, self._delta_type): # i.e. non-spherical
-      if self._cfun is None:
-        return delta
-      elif self._cfun_lud is not None:
-        delta = np.ravel(delta)
-        delta = self._cfun_lud.dot(delta)
-        return self._delta_type(*delta)
-      else:
-        delta = self._cfun(delta)
-        assert isinstance(delta, self._delta_type), \
-            "User supplied cfun did not output delta typoe {}".format(self._delta_type)
-        return delta
+      return delta
 
-    # Rule out possibility of all RVs contained in unscaling argument
+    # Rule out possibility of all variables contained in unscaling argument
     assert isinstance(delta, tuple), \
         "Unknown delta type: {}".format(delta)
     unscale = {} if not self._delta_args else self._delta_args
     if not len(self._spherise):
       return self._delta_type(**unscale)
 
     # Spherical version
@@ -568,345 +513,163 @@
     rss = real_sqrt(np.sum(np.array(list(spherise.values()))**2))
     if self._delta_kwds['scale']:
       delta *= rss
     deltas = np.random.uniform(-delta, delta, size=len(spherise))
     rss_deltas = real_sqrt(np.sum(deltas ** 2.))
     deltas = (deltas * delta) / rss_deltas
     delta_dict = collections.OrderedDict()
-    rvs = [self[key] for key in keys]
     idx = 0
     for i, key in enumerate(keys):
       if key in unscale:
         val = unscale[key]
       else:
         val = deltas[idx]
         idx += 1
         if self._delta_kwds['scale']:
           val *= self._lengths[i]
       delta_dict.update({key: val})
     delta = self._delta_type(**delta_dict)
-    if self._cfun is None:
-      return delta
-    elif self._cfun_lud is not None:
-      delta = self._cfun_lud.dot(np.array(delta, dtype=float))
-      return self._delta_type(*deltas)
-    else:
-      delta = self._cfun(delta)
-      assert isinstance(delta, self._delta_type), \
-          "User supplied cfun did not output delta type {}".format(self._delta_type)
-      return delta
+    return delta
 
 #-------------------------------------------------------------------------------
   def apply_delta(self, values, delta=None):
     delta = delta or self._delta
     if delta is None:
       return values
     if not isinstance(delta, self._delta_type):
-      rvs = self.ret_rvs(aslist=True)
-      if len(rvs) == 1 and isinstance(delta, rvs[0].delta):
-        return rvs[0].apply_delta(values, delta)
+      variables = self._varlist
+      if len(variables) == 1 and isinstance(delta, variables[0].delta):
+        return variables[0].apply_delta(values, delta)
       raise TypeError("Cannot apply delta without providing delta type {}".\
         format(self._delta_type))
     bound = False if 'bound' not in self._delta_kwds \
            else self._delta_kwds['bound']
     vals = collections.OrderedDict(values)
     keys = delta._fields
-    rvs = [self[key] for key in keys]
     for i, key in enumerate(keys):
-      vals.update({key: rvs[i].apply_delta(values[key], delta[i], bound=bound)})
+      vals.update({key: self._vars[key].apply_delta(values[key], 
+                                                    delta[i], 
+                                                    bound=bound)})
     return vals
 
 #-------------------------------------------------------------------------------
-  def eval_prop(self, values, **kwargs):
-    if self._tran is not None:
-      return self.eval_tran(values, **kwargs)
-    if values is None:
-      values = {}
-    if self._prop is None:
-      return self.eval_prob(values, **kwargs)
-    if not self._prop.ret_callable():
-      return self._prop()
-    return self._prop(values)
-
-#-------------------------------------------------------------------------------
   def eval_step(self, pred_vals, succ_vals, reverse=False):
     """ Returns adjusted succ_vals """
 
     # Evaluate deltas if required
     if succ_vals is None:
       if self._delta is None:
         pred_values = list(pred_vals.values())
         if all([isscalar(pred_value) for pred_value in pred_values]):
-          succ_vals = {0}
+          raise ValueError("Stochastic step sampling not supported for Field; use RF")
         else:
           succ_vals = pred_vals
       else:
         succ_vals = self.eval_delta()
-    elif isinstance(succ_vals, Func) or \
+    elif isinstance(succ_vals, Expression) or \
         isinstance(succ_vals, (tuple, self._delta_type)):
       succ_vals = self.eval_delta(succ_vals)
 
     # Apply deltas
     cond = None
     if isinstance(succ_vals, self._delta_type):
       succ_vals = self.apply_delta(pred_vals, succ_vals)
     elif isunitsetint(succ_vals):
-      if self._tfun is not None and self._tfun.ret_callable():
-        number = list(succ_vals)[0]
-        succ_vals = collections.OrderedDict()
-        succ_lims = collections.OrderedDict()
-        succ_vset = collections.OrderedDict()
-        for key in self._keys:
-          if key in pred_vals:
-            succ_vals.update({key: pred_vals[key]})
-            lims = self[key].ret_lims()
-            assert np.all(np.isfinite(lims)), \
-                "Cannot sample RV {} exhibiting limits {}".\
-                format(key, lims)
-            succ_vals.update({key: pred_vals[key]})
-            succ_lims.update({key: lims})
-            succ_vset.update({key: self[key].ret_vset()})
-      elif self._nrvs == 1:
-        rv = self.ret_rvs(aslist=True)[0]
-        tran = rv.ret_tran()
-        tfun = rv.ret_tfun()
-        if (tran is not None and not tran.ret_callable()) or \
-            (tfun is not None and tfun.ret_callable()):
-          vals, dims, kwargs = rv.eval_step(pred_vals[rv.ret_name()], succ_vals, reverse=reverse)
-          return vals, dims, kwargs
-        raise ValueError("Transitional CDF calling requires callable tfun")
-      else:
-        raise ValueError("Transitional CDF calling requires callable tfun")
-      keys = list(succ_vals.keys())
-
-      # One variable at a time modification
-      if self._t1vt:
-        if self.__cond_mod is None:
-          self.__cond_mod = 0
-        keys = [keys[self.__cond_mod]]
-        self.__cond_mod += 1
-        if self.__cond_mod >= len(succ_vals):
-          self.__cond_mod = 0
-
-      # Iterate through values
-      cond = np.nan
-      if self._tfun.ret_istuple():
-        for key in keys:
-          succ_vals[key] = {0}
-          succ_vals[key] = self._tfun[int(reverse)](succ_vals)
-      else:
-        for key in keys:
-          succ_vals[key] = {0}
-          succ_vals[key] = self._tfun(succ_vals)
+      raise ValueError("Stochastic step sampling not supported for Field; use RF")
 
     # Initialise outputs with predecessor values
     dims = {}
     kwargs = {'reverse': reverse}
     if cond is not None:
       kwargs = {'cond': cond}
     vals = collections.OrderedDict()
-    for key in self._keys:
+    for key in self._keylist:
       vals.update({key: pred_vals[key]})
-    if succ_vals is None and self._tran is None:
+    if succ_vals is None:
       return vals, dims, kwargs
 
-    # If stepping or have a transition function, add successor values
-    for key in self._keys:
+    # If stepping, add successor values
+    for key in self._keylist:
       mod_key = key+"'"
       succ_key = key if mod_key not in succ_vals else mod_key
       vals.update({key+"'": succ_vals[succ_key]})
 
     return vals, dims, kwargs
 
 #-------------------------------------------------------------------------------
-  def eval_tran(self, values, **kwargs):
-    if 'cond' in kwargs:
-      return kwargs['cond']
-    reverse = False if 'reverse' not in kwargs else kwargs['reverse']
-    if self._tran is None:
-      rvs = self.ret_rvs(aslist=True)
-      if len(rvs) == 1 and rvs[0]._tran is not None:
-        return rvs[0].eval_tran(values, **kwargs)
-      pred_vals = dict()
-      succ_vals = dict()
-      for key_, val in values.items():
-        prime = key_[-1] == "'"
-        key = key_[:-1] if prime else key_
-        if key in self._keys:
-          if prime:
-            succ_vals.update({key: val})
-          else:
-            pred_vals.update({key: val})
-      cond, _ = rv_prod_rule(pred_vals, succ_vals, rvs=rvs, pscale=self._pscale)
-    else:
-      assert self._tran.ret_callable(), \
-          "Only callable transitional functions supported for multidimensionals"
-      cond = self._tran(values) if self._sym_tran else \
-             self._tran[int(reverse)](values)
-    return cond
+  def subfield(self, vertices):
+    """ Returns a view of vertices, which must all be members, as a Field.
 
-#-------------------------------------------------------------------------------
-  def reval_tran(self, dist):
-    """ Evaluates the conditional reverse-transition function for corresponding 
-    transition conditional distribution dist. This requires a tuple input for
-    self.set_tran() to evaluate a new conditional.
+    :param vertices: str/variable/field or list/tuple of str/variable/field use.
+
+    :return: an Field including only those vertices
     """
-    assert isinstance(dist, Dist), \
-        "Input must be a distribution, not {} type.".format(type(dist))
-    marg, cond = dist.cond, dist.marg
-    name = margcond_str(marg, cond)
-    vals = dist.vals
-    dims = dist.dims
-    prob = dist.prob if self._sym_tran else self._tran[1](dist.vals)
-    pscale = dist.ret_pscale()
-    return Dist(name, vals, dims, prob, pscale)
-
-#-------------------------------------------------------------------------------
-  def _eval_iid(self, dist_name, vals, dims, prob, iid):
-    if not iid: 
-      return Dist(dist_name, vals, dims, prob, self._pscale)
-
-    # Deal with IID cases
-    max_dim = None
-    for dim in dims.values():
-      if dim is not None:
-        max_dim = dim if max_dim is None else max(dim, max_dim)
-
-    # If scalar or prob is expected shape then perform product here
-    if max_dim is None or max_dim == prob.ndim - 1:
-      dist = Dist(dist_name, vals, dims, prob, self._pscale)
-      return dist.prod(iid)
-
-    # Otherwise it is left to the user function to perform the iid product
-    for key in iid:
-      vals[key] = {len(vals[key])}
-      dims[key] = None
 
-    # Tidy up probability
-    return Dist(dist_name, vals, dims, prob, self._pscale)
+    # Convert to list
+    if isinstance(vertices, tuple):
+      vertices = list(vertices)
+    if not isinstance(vertices, list):
+      vertices = [vertices]
+
+    # Collate variables and return as Field
+    variables = []
+    for vertex in vertices:
+      if isinstance(vertex, Field):
+        variables += [vertex.ret_vars(aslist=True)]
+      elif isinstance(vertex, Variable):
+        variables += [vertex]
+      elif isinstance(vertex, str):
+        variables += [self._vars[vertex]]
+      else:
+        raise TypeError("Unrecognised vertex specification type: {}".format(
+            type(vertex)))
+    return Field(*tuple(variables))
 
 #-------------------------------------------------------------------------------
   def __call__(self, *args, **kwds):
-    """ Returns a joint distribution p(args) """
-    if self._rvs is None:
+    """ Returns a distribution p(args) """
+    if not self._nvars:
       return None
     iid = False if 'iid' not in kwds else kwds.pop('iid')
     if type(iid) is bool and iid:
       iid = self._defiid
     values = self.parse_args(*args, **kwds)
-    dist_name = self.eval_dist_name(values)
-    vals, dims = self.eval_vals(values, _skip_parsing=True)
-    prob = self.eval_prob(vals)
-    return self._eval_iid(dist_name, vals, dims, prob, iid)
+    vals, dims = self.evaluate(values, _skip_parsing=True)
+    name = ','.join(list(vals.keys()))
+    return Distribution(name, vals, dims=dims)
 
 #-------------------------------------------------------------------------------
-  def propose(self, *args, **kwds):
-    """ Returns a proposal distribution p(args[0]) for values """
-    suffix = "'" if 'suffix' not in kwds else kwds.pop('suffix')
-    values = self.parse_args(*args, **kwds)
-    dist_name = self.eval_dist_name(values, suffix)
-    vals, dims = self.eval_vals(values, _skip_parsing=True)
-    prop = self.eval_prop(vals) if self._prop is not None else \
-           self.eval_prob(vals)
-    if suffix:
-      keys = list(vals.keys())
-      for key in keys:
-        mod_key = key + suffix
-        vals.update({mod_key: vals.pop(key)})
-        if key in dims:
-          dims.update({mod_key: dims.pop(key)})
-    return Dist(dist_name, vals, dims, prop, self._pscale)
-
-#-------------------------------------------------------------------------------
-  def step(self, *args, **kwds):
-    """ Returns a proposal distribution p(args[1]) given args[0], depending on
-    whether using self._prop, that denotes a simple proposal distribution,
-    or self._tran, that denotes a transitional distirbution. """
-
-    reverse = False if 'reverse' not in kwds else kwds.pop('reverse')
-    pred_vals, succ_vals = None, None 
-    if len(args) == 1:
-      if isinstance(args[0], (list, tuple)) and len(args[0]) == 2:
-        pred_vals, succ_vals = args[0][0], args[0][1]
-      else:
-        pred_vals = args[0]
-    elif len(args) == 2:
-      pred_vals, succ_vals = args[0], args[1]
-
-    # Evaluate predecessor values
-    pred_vals = self.parse_args(pred_vals, pass_all=True)
-    dist_pred_name = self.eval_dist_name(pred_vals)
-    pred_vals, pred_dims = self.eval_vals(pred_vals)
-
-    # Default successor values if None and delta is None
-    if succ_vals is None and self._delta is None:
-      pred_values = list(pred_vals.values())
-      if all([isscalar(pred_value) for pred_value in pred_values]):
-        succ_vals = {0}
-      else:
-        succ_vals = pred_vals
+  def __and__(self, other):
+    return and_op(self, other)
 
-    # Evaluate successor evaluates
-    vals, dims, kwargs = self.eval_step(pred_vals, succ_vals, reverse=reverse)
-    succ_vals = {key[:-1]: val for key, val in vals.items() if key[-1] == "'"}
-    cond = self.eval_tran(vals, **kwargs)
-    dist_succ_name = self.eval_dist_name(succ_vals, "'")
-    dist_name = '|'.join([dist_succ_name, dist_pred_name])
+#-------------------------------------------------------------------------------
+  def __or__(self, other):
+    return or_op(self, other)
 
-    return Dist(dist_name, vals, dims, cond, self._pscale)
+#-------------------------------------------------------------------------------
+  def __eq__(self, other):
+    """ Equality for Fields is defined as comprising the same Variables """
+    if type(self) is not Field or type(other) is not Field:
+      return super().__eq__(other)
+    return self._keyset == other.keyset
 
 #-------------------------------------------------------------------------------
-  def __len__(self):
-    return self._nrvs
+  def __ne__(self, other):
+    """ Equality for Field is defined as comprising the same Variables """
+    return not self.__eq__(other)
 
 #-------------------------------------------------------------------------------
   def __getitem__(self, key):
     if type(key) is int:
-      key = self._keys[key]
+      key = self._keylist[key]
     if isinstance(key, str):
-      if key not in self._keys:
+      if key not in self._keylist:
         return None
-    return self._rvs[key]
+    return self._vars[key]
 
 #-------------------------------------------------------------------------------
   def __repr__(self):
     if not self._name:
-      return super().__repr__()
-    return super().__repr__() + ": '" + self._name + "'"
-
-#-------------------------------------------------------------------------------
-  def __mul__(self, other):
-    from probayes.rv import RV
-    from probayes.rf import RF
-    if isinstance(other, RF):
-      marg = self.ret_rvs() + other.ret_marg().ret_rvs()
-      cond = other.ret_cond().ret_rvs()
-      return RF(marg, cond)
-
-    if isinstance(other, RJ):
-      rvs = self.ret_rvs() + other.ret_rvs()
-      return RJ(*tuple(rvs))
-
-    if isinstance(other, RV):
-      rvs = self.ret_rvs() + [other]
-      return RJ(*tuple(rvs))
-
-    raise TypeError("Unrecognised post-operand type {}".format(type(other)))
-
-#-------------------------------------------------------------------------------
-  def __truediv__(self, other):
-    from probayes.rv import RV
-    from probayes.rf import RF
-    if isinstance(other, RF):
-      marg = self.ret_rvs() + other.ret_cond().ret_rvs()
-      cond = other.ret_marg().ret_rvs()
-      return RF(marg, cond)
-
-    if isinstance(other, RJ):
-      return RF(self, other)
-
-    if isinstance(other, RV):
-      return RF(self, other)
-
-    raise TypeError("Unrecognised post-operand type {}".format(type(other)))
+      return NX_UNDIRECTED_GRAPH.__repr__(self)
+    return NX_UNDIRECTED_GRAPH.__repr__(self) + ": '" + self._name + "'"
 
 #-------------------------------------------------------------------------------
```

### Comparing `probayes-0.0.3/probayes/rv.py` & `probayes-0.0.4/probayes/rf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,529 +1,658 @@
-""" Random variable module """
+""" Provides Random Field class: RF """
 
 #-------------------------------------------------------------------------------
 import collections
 import numpy as np
-import scipy.stats
-from probayes.domain import Domain
-from probayes.prob import Prob, is_scipy_stats_cont
-from probayes.dist import Dist
-from probayes.vtypes import eval_vtype, uniform, VTYPES, isscalar, \
-                        isunitset, isunitsetint, isunitsetfloat, issingleton
-from probayes.pscales import div_prob, rescale, eval_pscale
-from probayes.func import Func
-from probayes.rv_utils import nominal_uniform_prob, matrix_cond_sample, \
-                          lookup_square_matrix
-
-"""
-A random variable is a triple (x, A_x, P_x) defined for an outcome x for every 
-possible realisation defined over the alphabet set A_x with probabilities P_x.
-It therefore requires a name for x (id), a variable alphabet set (vset), and its 
-associated probability distribution function (prob).
-"""
-
-#-------------------------------------------------------------------------------
-class RV (Domain, Prob):
-  """ A random variable is a domain with a defined probability function.
-  It therefore inherits from classes Domain and and Prob. Each instance therefore 
-  requires a name, a variable set, and probability function. Additionally RV
-  supports transitional probabilities the cdf/icdf equivalents specified using
-  RV.set_tran() and RV.set_tfun() equivalents, and accessed using RV.step().
-
-  :example:
-  >>> import numpy as np
-  >>> import probayes as pb
-  >>> var = pb.RV('var', vtype=bool)
-  >>> var.set_tran(np.array([0.2, 0.8, 0.3, 0.7]).reshape(2,2,))
-  >>> step = var.step()
-  >>> print(step.prob)
-  [[0.2 0.8]
-   [0.3 0.7]]
-  """
 
-  # Protected
-  _tran = None      # Transitional prob - can be a matrix
-  _tfun = None      # Like pfun for transitional conditionals
+from probayes.field import Field
+from probayes.rv import RV
+from probayes.prob import Prob
+from probayes.pd import PD
+from probayes.pd_utils import margcond_str
+from probayes.vtypes import isscalar, isunitsetint
+from probayes.pscales import iscomplex, prod_pscale
+from probayes.rf_utils import rv_prod_rule, sample_cond_cov
+from probayes.expr import Expr
+from probayes.expression import Expression
+from probayes.cf import CF
+from probayes.cond_cov import CondCov
 
-  # Private
-  __sym_tran = None
-  __prime_key = None
+DEFAULT_CONDITIONAL_PROBABILITY = {False: 1., True: 0.}
 
 #-------------------------------------------------------------------------------
-  def __init__(self, name, 
-                     vset=None, 
-                     vtype=None,
-                     prob=None,
-                     pscale=None,
-                     *args,
-                     **kwds):
-    """ Initialises a random variable combining Domain and Prob initialisation
-    except invertible monotonic must be specified separately using set_mfun().
-
-    :param name: Name of the domain - string as valid identifier.
-    :param vset: variable set over which domain defined (see set_vset).
-    :param vtype: variable type (bool, int, or float).
-    :param prob: may be a scalar, array, or callable function.
-    :param pscale: represents the scale used to represent probabilities.
-    :param *args: optional arguments to pass if prob is callable.
-    :param **kwds: optional keywords to pass if prob is callable.
-    """
-
-    self.set_name(name)
-    self.set_vset(vset, vtype)
-    self.set_prob(prob, pscale, *args, **kwds)
-    self.set_mfun()
-    self.set_delta()
+class RF (Field, Prob):
+  """
+  A random field is a collection of a variables, that includes at least one RV, 
+  that participate in a joint probability distribution function without 
+  explicit directional conditionality.
+  
+  Since this class is intended as a building block for SD instances and networkx 
+  cannot mix undirected and directed graphs, edges cannot be defined explicitly 
+  within this class. Use SD if directed edges are required. Implicit support for
+  undirected edges is provided by the set_prob(), set_prop(), and set_tran()
+  methods.
+  """
 
-#-------------------------------------------------------------------------------
-  def set_name(self, name):
-    """ Sets name of variable over which domain is defined:
+  # Protected
+  _defiid = None     # Default IID random variables for calling distributions
+  _passdims = None   # Flag to pass dimensions to probability function
+  _prop = None       # Non-transitional proposition function
+  _prop_deps = None  # Set of proposition dependencies
+  _tran = None       # Transitional proposition function
+  _tfun = None       # CDF/IDF of transition function 
+  _tsteps = None     # Number of steps per transitional modificiation
+  _cvars = None      # Conditional random variable sampling specification
+  _sym_tran = None   # Flag for symmetrical transitional conditional functions
+  _is_stochastic = True # Flag of whether stochastic
 
-    :param name: Name of the domain - string as valid identifier.
-    """
-    super().set_name(name)
-    self.__prime_key = self._name + "'"
+  # Private
+  __def_prob = None   # Flag to denote prob is defaulted
+  __cond_mod = None  # conditional RV index modulus
+  __cond_cov = None  # conditional covariance matrix
+
+#-------------------------------------------------------------------------------
+  def __init__(self, *args): # over-rides NX_GRAPH.__init__()
+    """ Initialises a random field with RVs for in args. See set_vars(). """
+    super().__init__(*args)
+    self.set_prob()
+    self.set_prop()
+    self.set_tran()
+
+#-------------------------------------------------------------------------------
+  def add_cd(self, *args, **kwds):
+    """ Adding of conditional dependences disallowed """
+    raise NotImplementedError("Not implemented for this class")
+
+#-------------------------------------------------------------------------------
+  def _refresh(self):
+    """ Updates RV summary objects, RF name and id, and delta factory. """
+    super()._refresh()
+    if self._nvars:
+      pscales = [var.pscale for var in self._vars.values()]
+      self.pscale = prod_pscale(pscales)
+    self.eval_length()
+    self._prop = None
+    self._tran = None
+    self._tfun = None
+
+#-------------------------------------------------------------------------------
+  @property
+  def prob(self):
+    return self._prob
+
+  @property
+  def passdims(self):
+    return self.passdims
+
+  @property
+  def def_prob(self):
+    return self.__def_prob
 
-#-------------------------------------------------------------------------------
-  def set_prob(self, prob=None, pscale=None, *args, **kwds):
-    """ Sets the probability and pscale with optional arguments and keywords.
+  def set_prob(self, prob=None, *args, **kwds):
+    """ Sets the joint probability with optional arguments and keywords.
 
     :param prob: may be a scalar, array, or callable function.
-    :param pscale: represents the scale used to represent probabilities.
     :param *args: optional arguments to pass if prob is callable.
     :param **kwds: optional keywords to pass if prob is callable.
 
-    See set_pscale() for explanation of how pscale is used.
-    """
-    self._tran, self._tfun = None, None
-    if prob is not None:
-      super().set_prob(prob, pscale, *args, **kwds)
-    else:
-      self._default_prob(pscale)
-
-    # Check uncallable probabilities commensurate with self._vset
-    if self._vset is not None and \
-        not self.ret_callable() and not self.ret_isscalar():
-      assert len(self._prob()) == len(self._vset), \
-          "Probability of length {} incommensurate with Vset of length {}".format(
-              len(self._prob), len(self._vset))
-
-    # If using scipy stats, ensure vset is float type
-    pset = self.ret_pset()
-    if is_scipy_stats_cont(pset):
-      if self._vtype not in VTYPES[float]:
-        self.set_vset(self._vset, vtype=float)
-   
-#-------------------------------------------------------------------------------
-  def _default_prob(self, pscale=None):
-    """ Defaults unspecified probabilities to uniform over self._vset """
-    self._pscale = eval_pscale(pscale)
+    'pscale' is a reserved keyword. See Prob.pscale for explanation of how 
+    pscale is used. Keyword 'passdims' is reserved to pass a flag to callable
+    prob functions to pass the dimensionality dictionary for values.
+    """
+    kwds = dict(kwds)
+    self._passdims = False if 'passdims' not in kwds else kwds.pop('passdims')
+    if 'pscale' not in kwds and self._nvars:
+      pscales = [var.pscale for var in self._varlist]
+      kwds.update({'pscale': prod_pscale(pscales)})
+    super().set_prob(prob, *args, **kwds)
     if self._prob is None:
-      if self._vset is None:
-        return self.ret_callable()
-      else:
-        prob = div_prob(1., float(self._length))
-        if self._pscale != 1.:
-          prob = rescale(prob, 1., self._pscale)
-        super().set_prob(prob, self._pscale)
-        self.set_tran(prob)
+      self._default_prob()
+      return
+    assert self._anystoch, \
+        "Cannot set field probability without any random variables"
+    self.__def_prob = False
 
 #-------------------------------------------------------------------------------
-  def set_pfun(self, pfun=None, *args, **kwds):
-    """ Sets a two-length tuple of functions that should correspond to the
-    (cumulative probability function, inverse cumulative function) with respect
-    to the callable function set by set_prob(). It is necessary to set these
-    functions if sampling variables with non-flat distributions.
-
-    :param pfun: two-length tuple of callable functions
-    :param *args: arguments to pass to pfun functions
-    :param **kwds: keywords to pass to pfun functions
-    """
-    super().set_pfun(pfun, *args, **kwds)
-    if self._mfun is None or self._pfun is None:
+  def _default_prob(self):
+    if not self._anystoch or (self._prob is not None and not self.__def_prob):
       return
-    if self.ret_pfun(0) != scipy.stats.uniform.cdf or \
-        self.ret_pfun(1) != scipy.stats.uniform.ppf:
-      assert self._mfun is None, \
-        "Cannot assign non-uniform distribution alongside " + \
-        "values transformation functions"
-
-#-------------------------------------------------------------------------------
-  def set_mfun(self, mfun=None, *args, **kwds):
-    """ Sets a monotonic invertible tranformation for the domain as a tuple of
-    two functions in the form (transforming_function, inverse_function) 
-    operating on the first argument with optional further args and kwds.
-
-    :param mfun: two-length tuple of monotonic functions.
-    :param *args: args to pass to mfun functions.
-    :param **kwds: kwds to pass to mfun functions.
-
-    Support for this transformation is only valid for float-type vtypes.
-    """
-    super().set_mfun(mfun, *args, **kwds)
-    if self._mfun is None:
+    if all([var.isiconic for var in self._varlist]):
+      prob = None
+      for var in self._varlist:
+        if var.is_stochastic:
+          var_prob = var.prob
+          mul = var_prob if not isinstance(var_prob, Expr) else var_prob._expr
+          if prob is not None:
+            prob = prob * mul
+          else:
+            prob = mul
+      self.set_prob(prob, pscale=self._pscale)
+      self.__def_prob = True
+
+#-------------------------------------------------------------------------------
+  def eval_length(self):
+    """ Evaluates and returns the joint length of the field. """
+    self._lengths = np.array([var.length for var in self._varlist \
+                              if var.is_stochastic], dtype=float)
+    self._length = np.sqrt(np.sum(self._lengths**2))
+    return self._length
+
+#-------------------------------------------------------------------------------
+  @property
+  def prop(self):
+    """ Returns the proposal probability expression if specified """
+    return self._prop
+
+  def set_prop(self, prop=None, *args, **kwds):
+    """ Sets the joint proposition function with optional arguments and keywords.
+
+    :param prop: may be a scalar, array, or callable function.
+    :param *args: optional arguments to pass if prop is callable.
+    :param **kwds: optional keywords to pass if prop is callable.
+    """
+    self._prop = prop
+    self._prop_deps = self._keylist if 'deps' not in kwds else kwds.pop['deps']
+    if self._prop is None:
       return
-
-    # Recalibrate scalar probabilities for floating point vtypes
-    if self.ret_isscalar() and \
-        self._vtype in VTYPES[float]:
-      self._default_prob(self._pscale)
-
-    # Check pfun is unspecified or uniform
-    if self._pfun is None:
-      return
-    if self.ret_pfun(0) != scipy.stats.uniform.cdf or \
-        self.ret_pfun(1) != scipy.stats.uniform.ppf:
-      assert self._pfun is None, \
-        "Cannot assign values tranformation function alongside " + \
-        "non-uniform distribution"
+    assert self._anystoch, \
+        "Cannot set field proposition without any random variables"
+    assert self._tran is None, \
+        "Cannot assign both proposition and transition probabilities"
+    self._prop = Expression(self._prop, *args, **kwds)
 
 #-------------------------------------------------------------------------------
-  def set_tran(self, tran=None, *args, **kwds):
-    """ Sets a transitional function as a conditional probability. This can
-    be specified numerically or one or two callable functions.
+  @property
+  def tran(self):
+    """ Returns the transitional probability expression if specified """
+    return self._tran
 
-    :param tran: conditional scalar, array, or callable function (see below).
-    :param *args: args to pass to tran functions.
-    :param **kwds: kwds to pass to tran functions.
-
-    If tran is a scalar, array, or callable function, then the transitional
-    conditionality is treated as symmetrical. If tran is a two-length tuple,
-    then assymetry is assumed in the form: (p[var'|var], p[var|var']).
+  def set_tran(self, tran=None, *args, **kwds):
+    """ Sets the conditional transition function with optional arguments and 
+    keywords.
 
-    If intending to sample from a transitional conditional probability density
-    function, the corresponding (CDF, ICDF) must be set using set_tfun().
+    :param tran: may be a scalar, covariance array, or callable function.
+    :param *args: optional arguments to pass if tran is callable.
+    :param **kwds: optional keywords to pass if tran is callable.
     """
+    # Set transition function
     self._tran = tran
-    self.__sym_tran = None
+    self._sym_tran = False
+    self._tsteps = None
     if self._tran is None:
       return
-    self._tran = Func(self._tran, *args, **kwds)
-    self.__sym_tran = not self._tran.ret_istuple()
-    if self._tran.ret_callable() or self._tran.ret_isscalar():
-      return
-    assert self._vtype not in VTYPES[float],\
-      "Scalar or callable transitional required for floating point data types"
-    tran = self._tran() if self.__sym_tran else self._tran[0]()
-    message = "Transition matrix must a square 2D Numpy array " + \
-              "covering variable set of size {}".format(len(self._vset))
-    assert isinstance(tran, np.ndarray), message
-    assert tran.ndim == 2, message
-    assert np.all(np.array(tran.shape) == len(self._vset)), message
-    self.__sym_tran = np.allclose(tran, tran.T)
+    assert self._anystoch, \
+        "Cannot set field transitional without any random variables"
+    assert self._prop is None, \
+        "Cannot assign both proposition and transition probabilities"
+    kwds = dict(kwds)
+    if 'tsteps' in kwds:
+      self._tsteps = kwds.pop('tsteps')
+      if self._tsteps:
+        assert type(self._tsteps) is int, "Input tsteps must be int"
+
+    # Pass CF objects directly
+    if isinstance(tran, CF):
+      assert not args and not kwds, \
+        "Setting args and kwds not supported if inputting a CF instance"
+      self._tran = CF(self, 
+                      tran.ret_inp(), 
+                      tran.ret_func(), 
+                      *tran.ret_args(), 
+                      **tran.ret_kwds())
+      self._sym_tran = not self._tran.ret_ismulti()
+      return
+
+    # Set as general function
+    self._tran = Prob(tran, *args, **kwds)
+    self._sym_tran = not self._tran.ismulti
+
+    # If a covariance matrix, set the LU decomposition as the tfun
+    if not self._tran.callable and not self._tran.isscalar:
+      message = "Non-callable non-scalar tran objects must be a square 2D " + \
+                "Numpy array of size corresponding to number of variables {}".\
+                 format(self._nvars)
+      assert isinstance(tran, np.ndarray), message
+      assert tran.ndim == 2, message
+      assert np.all(np.array(tran.shape) == self._nvars), message
+      self.set_tfun(np.linalg.cholesky(tran))
+      assert self._tsteps is None, \
+          "Setting tsteps not supported for covariance transitions"
+      return
+
+    # If a scipy object, set the tfun
+    elif self._tran.isscipy:
+      scipyobj = self._tran.expr
+      self.set_tfun(self._tran, scipyobj=scipyobj)
+      return
+
+    # Return for unit variable RFs
+    elif self._unitvar:
+      return
+
+    # Otherwise reinstantiate self._tran as an explicit conditional function
+    inp = None
+    if len(args):
+      if isinstance(args[0], (dict, list, tuple)):
+        args = tuple(args)
+        inp, args = args[0], args[1:]
+    self._tran = CF(self, inp, tran, *args, **kwds)
+    self._sym_tran = not self._tran.ret_ismulti()
 
 #-------------------------------------------------------------------------------
+  @property
+  def tfun(self):
+    """ Returns the transitional CDF/ICDF expression if specified """
+    return self._tfun
+
   def set_tfun(self, tfun=None, *args, **kwds):
     """ Sets a two-length tuple of functions that should correspond to the
     (cumulative probability function, inverse cumulative function) with respect
     to the callable function set by set_tran(). It is necessary to set these
-    functions if conditionally sampling variables with continuous distributions.
+    functions for conditional sampling variables with non-flat distributions.
 
-    :param tfun: two-length tuple of callable functions
+    :param tfun: two-length tuple of callable functions or an LU decomposition
     :param *args: arguments to pass to tfun functions
     :param **kwds: keywords to pass to tfun functions
     """
-    self._tfun = tfun if tfun is None else Func(tfun, *args, **kwds)
+    scipyobj = None if 'scipyobj' not in kwds else kwds['scipyobj']
+    self._tfun = tfun 
     if self._tfun is None:
       return
-    assert self._tfun.ret_istuple(), "Tuple of two functions required"
-    assert len(self._tfun) == 2, "Tuple of two functions required."
-
-#-------------------------------------------------------------------------------
-  def ret_tran(self):
-    """ Returns the set transitional conditional probability object(s) """
-    return self._tran
+    if 'tsteps' in kwds:
+      self._tsteps = kwds.pop('tsteps')
 
-#-------------------------------------------------------------------------------
-  def ret_tfun(self):
-    """ Returns the set transitional conditional (CDF, ICDF) object(s) """
-    return self._tfun
+    # Pass CF objects directly
+    if isinstance(tfun, CF):
+      assert not args and not kwds, \
+        "Setting args and kwds not supported if inputting a CF instance"
+      self._tfun = CF(self, 
+                      tfun.ret_inp(), 
+                      tfun.ret_func(), 
+                      *tfun.ret_args(), 
+                      **tfun.ret_kwds())
+      return
 
-#-------------------------------------------------------------------------------
-  def eval_vals(self, values, use_pfun=True):
-    """ Evaluates value(s) belonging to the domain of the variable.
+    # Handle SciPy objects specifically
+    elif scipyobj is not None:      
+      lims = np.array([rv.ulims for rv in self._varlist])
+      mean = scipyobj.mean
+      cov = scipyobj.cov
+      self._cond_cov = CondCov(mean, cov, lims)
+      scipy_cond = sample_cond_cov if self._sym_tran else \
+                   (sample_cond_cov, sample_cond_cov)
+      self._tfun = CF(self, None, scipy_cond, cond_cov=self._cond_cov)
+      return
 
-    :param values: None, set of a single integer, array, or scalar.
-    :param use_pfun: boolean flag to make use of pfun if previously set.
+    # Non-callables are treated as LUD matrices
+    elif not callable(self._tfun): 
+        self._tfun = Prob(self._tfun, *args, **kwds)
+        message = "Non-callable tran objects must be a triangular 2D Numpy array " + \
+                  "of size corresponding to number of variables {}".format(self._nvars)
+        assert isinstance(tfun, np.ndarray), message
+        assert tfun.ndim == 2, message
+        assert np.all(np.array(tfun.shape) == self._nvars), message
+        assert np.allclose(tfun, np.tril(tfun)) or \
+               np.allclose(tfun, np.triu(tfun)), message
+        return
+
+    # Otherwise instantiate a formal conditional function
+    inp = None
+    if len(args):
+      if isinstance(args[0], (dict, list, tuple)):
+        args = tuple(args)
+        inp, args = args[0], args[1:]
+    self._tfun = CF(self, inp, self._tfun, *args, **kwds)
 
-    :return: a NumPy array of the values (see Domain.eval_vals()):
-    """
-    use_pfun = use_pfun and self._pfun is not None and isunitsetint(values)
-    if not use_pfun:
-      return super().eval_vals(values)
-
-    # Evaluate values from inverse cdf bounded within cdf limits
-    number = list(values)[0]
-    assert np.all(np.isfinite(self._lims)), \
-        "Cannot evaluate {} values for bounds: {}".format(values, self._lims)
-    lims = self.ret_pfun(0)(self._lims)
-    values = uniform(
-                     lims[0], lims[1], number, 
-                     isinstance(self._vset[0], tuple),
-                     isinstance(self._vset[1], tuple)
-                    )
-    return self.ret_pfun(1)(values)
-
-#-------------------------------------------------------------------------------
-  def eval_prob(self, values=None):
-    """ Evaluates the probability inputting optional args for callable cases
-
-    :param values: values of the variable used for evaluating probabilities.
-    :param *args: optional arguments for callable probability objects.
-    :param **kwds: optional arguments to include pscale for rescaling.
+#-------------------------------------------------------------------------------
+  def eval_prob(self, values=None, dims=None):
+    if values is None:
+      values = {}
+    else:
+      assert isinstance(values, dict), \
+          "Input to eval_prob() requires values dict"
+      assert set(values.keys()) == self._keyset, \
+        "Sample dictionary keys {} mismatch with RV names {}".format(
+          values.keys(), self._keylist)
+
+    # If not specified, treat as independent variables
+    if self._prob is None or self.__def_prob:
+      rvs = self._varlist
+      if len(rvs) == 1 and rvs[0]._prob is not None:
+        prob = rvs[0].eval_prob(values[rvs[0].name])
+      else:
+        prob, _ = rv_prod_rule(values, rvs=rvs, pscale=self._pscale)
+      return prob
 
-    :return: evaluated probabilities
-    """
-    if not self.ret_isscalar():
-      return super().eval_prob(values)
-    return nominal_uniform_prob(values, 
-                                prob=self._prob(), 
-                                inside=self._inside,
-                                pscale=self._pscale)
+    # Otherwise distinguish between uncallable and callables
+    if not self._callable:
+      return self._call()
+    if self.issympy:
+      prob = self._partials['logp'](values) if iscomplex(self._pscale) else \
+             self._partials['prob'](values)
+      return prob
+
+    # Pass-dims is to replaced when passing Distributions()
+    if self._passdims:
+      return super().eval_prob(values, dims=dims)
+    return super().eval_prob(values)
+
+#-------------------------------------------------------------------------------
+  def eval_delta(self, delta=None):
+    delta = super().eval_delta(delta)
+
+    # Adjust delta if there is LUD tfun
+    if self._tfun is None or self._tfun.isscalar:
+      return delta
+    elif not self._tfun.callable:
+      delta = self._tfun().dot(np.array(delta, dtype=float))
+      return self._delta_type(*delta)
+    else:
+      delta = self._tfun(delta)
+      assert isinstance(delta, self._delta_type), \
+          "User supplied tfun did not output delta type {}".\
+          format(self._delta_type)
+      return delta
 
 #-------------------------------------------------------------------------------
-  def eval_dist_name(self, values, suffix=None):
-    """ Evaluates a distribution name for a probability distribution based on
-    the values set in the first input argument with an optional suffix. """
-    name = self._name if not suffix else self._name + suffix
+  def eval_prop(self, values, **kwargs):
+    if self._tran is not None:
+      return self.eval_tran(values, **kwargs)
     if values is None:
-      dist_str = name
-    elif np.isscalar(values):
-      dist_str = "{}={}".format(name, values)
-    else:
-      dist_str = name + "=[]"
-    return dist_str
+      values = {}
+    if self._prop is None:
+      return self.eval_prob(values, **kwargs)
+    if not self._prop.callable:
+      return self._prop()
+    return self._prop(values)
 
 #-------------------------------------------------------------------------------
   def eval_step(self, pred_vals, succ_vals, reverse=False):
-    """ Evaluates a successive values from previous values with an optional
-    direction reversal flag, outputting a three-length tuple that includes the
-    successive values in the first argument.
-
-    :param pred_vals: predecessor values (NumPy array).
-    :param succ_vals: succecessor values (see step()).
-    :param reverse: boolean flag (default False) to reverse direction.
-
-    :return vals: a dictionary including both predecessor and successor values.
-    :return dims: a dictionary with dimension indices for the values in vals.
-    :return kwargs: a dictionary that includes optional keywords for eval_tran()
-    """
-
-    assert self._tran is not None, "No transitional function specified"
-    kwargs = dict() # to pass over to eval_tran()
+    """ Returns adjusted succ_vals """
     if succ_vals is None:
       if self._delta is None:
-        succ_vals = {0} if isscalar(pred_vals) else pred_vals
-      else:
-        delta = self.eval_delta()
-        succ_vals = self.apply_delta(pred_vals, delta)
+        if all([isscalar(pred_value) for pred_value in pred_vals]):
+          succ_vals = {0}
+
+    # If not sampling succeeding values, use deterministic call
+    if not isunitsetint(succ_vals):
+      return super().eval_step(pred_vals, succ_vals, reverse=reverse)
+
+    if self._tfun is not None and self._tfun.callable:
+      succ_vals = self.eval_tfun(pred_vals)
+    elif self._nvars == 1:
+      var = self._varlist[0]
+      tran = var.tran
+      tfun = var.tfun
+      if (tran is not None and not tran.callable) or \
+          (tfun is not None and tfun.callable):
+        vals, dims, kwargs = var.eval_step(pred_vals[var.name], 
+                                           succ_vals, reverse=reverse)
+        return vals, dims, kwargs
+      raise ValueError("Transitional CDF calling requires callable tfun")
+    else:
+      raise ValueError("Transitional CDF calling requires callable tfun")
+
+    # Initialise outputs with predecessor values
+    dims = {}
+    kwargs = {'reverse': reverse}
+    vals = collections.OrderedDict()
+    for key in self._keylist:
+      vals.update({key: pred_vals[key]})
+    if succ_vals is None and self._tran is None:
+      return vals, dims, kwargs
+
+    # If stepping or have a transition function, add successor values
+    for key in self._keylist:
+      mod_key = key+"'"
+      succ_key = key if mod_key not in succ_vals else mod_key
+      vals.update({key+"'": succ_vals[succ_key]})
+
+    return vals, dims, kwargs
+
+#-------------------------------------------------------------------------------
+  def eval_tfun(self, values, *args, reverse=False, **kwds):
+    """ Evaluates tfun from values """
 
-    #---------------------------------------------------------------------------
-    def _reshape_vals(pred, succ):
-      dims = {}
-      ndim = 0
-
-      # Now reshape the values according to succ > prev dimensionality
-      if issingleton(succ):
-        dims.update({self._name+"'": None})
+    # Handle non-callables first
+    if self._tfun is None:
+      return None
+    if self._tfun.isscalar:
+      if self._tfun.ismulti:
+        return self._tfun[int(reverse)]() * values()
       else:
-        dims.update({self._name+"'": ndim})
-        ndim += 1
-      if issingleton(pred):
-        dims.update({self._name: None})
+        return self._tfun() * values
+    if not self._tfun.callable:
+      if self._tfun.ismulti:
+        return self._tfun[int(reverse)]().dot(values)
       else:
-        dims.update({self._name: ndim})
-        ndim += 1
+        return self._tfun().dot(values)
 
-      if ndim == 2: # pred_vals distributed along inner dimension:
-        pred = pred.reshape([1, pred.size])
-        succ = succ.reshape([succ.size, 1])
-      return pred, succ, dims
-
-    #---------------------------------------------------------------------------
-    # Scalar treatment is the most trivial and ignores reverse
-    if self._tran.ret_isscalar():
-      if isunitsetint(succ_vals):
-        succ_vals = self.eval_vals(succ_vals, use_pfun=False)
-      elif isunitsetfloat(succ_vals):
-        assert self._vtype in VTYPES[float], \
-            "Inverse CDF sampling for scalar probabilities unavailable for " + \
-            "{} data type".format(self._vtype)
-        cdf_val = list(succ_vals)[0]
-        lo, hi = min(self._limits), max(self._limits)
-        succ_val = lo*(1.-cdf_val) + hi*cdf_val
-        if self._mfun is not None:
-          succ_val = self.ret_mfun(1)(succ_val)
-
-      prob = self._tran()
-      pred_vals, succ_vals, dims = _reshape_vals(pred_vals, succ_vals)
-                  
-    # Handle discrete non-callables
-    elif not self._tran.ret_callable():
-      if reverse and not self._tran.ret_istuple() and not self.__sym_tran:
-        warning.warn("Reverse direction called from asymmetric transitional")
-      prob = self._tran() if not self._tran.ret_istuple() else \
-             self._tran[int(reverse)]()
-      if isunitset(succ_vals):
-        succ_vals, pred_idx, succ_idx = matrix_cond_sample(pred_vals, 
-                                                           succ_vals, 
-                                                           prob=prob, 
-                                                           vset=self._vset) 
-        kwargs.update({'pred_idx': pred_idx, 'succ_idx': succ_idx})
-      pred_vals, succ_vals, dims = _reshape_vals(pred_vals, succ_vals)
+    # If values is not a dictionary then allow a custom call
+    if not isinstance(values, dict):
+      if self._tfun.ismulti:
+        return self._tfun[int(reverse)](values, *args, **kwds).dot(values)
+      else:
+        return self._tfun(values, *args, **kwds)
 
-    # That just leaves callables
-    else:
-      kwds = {self._name: pred_vals}
-      if isunitset(succ_vals):
-        assert self._tfun is not None, \
-            "Conditional sampling requires setting CDF and ICDF " + \
-            "conditional functions using rv.set.tfun()"
-        assert isscalar(pred_vals), \
-            "Successor sampling only possible with scalar predecessors"
-        succ_vals = list(succ_vals)[0]
-        if type(succ_vals) in VTYPES[int] or type(succ_vals) in VTYPES[np.uint]:
-          lo, hi = min(self._lims), max(self._lims)
-          kwds.update({self._name+"'": np.array([lo, hi], dtype=float)})
-          lohi = self._tfun[0](**kwds)
-          lo, hi = float(min(lohi)), float(max(lohi))
-          succ_vals = uniform(lo, hi, succ_vals,
-                              isinstance(self._vset[0], tuple),
-                              isinstance(self._vset[1], tuple))
+    # Support variable sampling one-or-more at-a-time
+    succ_vals = collections.OrderedDict(values)
+
+    # For conditional functions, iterate through keys
+    assert isinstance(self._tfun, CF), "Callable conditionals must be CF type"
+
+    # Determine keys distinguishing between default and custom specifications
+    inp = self._tfun.ret_inp() # ?
+    keys = list(succ_vals.keys()) if not inp else list(inp.keys())
+    if self._tsteps:
+      if self.__cond_mod is None:
+        self.__cond_mod = 0
+      keys = keys[self.__cond_mod:(self.__cond_mod+self._tsteps)]
+      self.__cond_mod += self._tsteps
+      if self.__cond_mod >= len(succ_vals):
+        self.__cond_mod = 0
+
+    # Handle unspecified input key handling separately
+    if not inp:
+      if self._tfun.ismulti:
+        for key in keys:
+          succ_vals[key] = self._tfun[int(reverse)](succ_vals, *args, unknown=key, **kwds)
+      else:
+        for key in keys:
+          succ_vals[key] = self._tfun(succ_vals, *args, unknown=key, **kwds)
+      return succ_vals
+
+    # Explicit conditionals require more sophisticated handling
+    assert not reverse, \
+        "Reverse-direction sampling not supported for explicit conditionals"
+    assert self._tfun.ismulti, \
+        "Transitional sampling function not specified as a multiple sampler"
+    for key in keys:
+      values = self._tfun[key](succ_vals, *args, **kwds)
+      rv_names = [key] if ',' not in keys else key.split(',')
+      if len(rv_names) > 1:
+        assert isinstance(values, dict), \
+            "Ambiguous output from CF {} for RV {}".format(self._tfun, key)
+        for rv_key, rv_val in values.items():
+          assert rv_key in succ_vals.keys(), \
+              "Key {} not found in {}".format(rv_key, succ_vals.keys())
+          succ_vals[key] = rv_val
+      else:
+        rv_name = rv_names[0]
+        if isinstance(values, dict):
+          assert rv_name in values.keys(), \
+              "Value key {} not found from output {}".format(rv_name, values.keys())
+          succ_vals[rv_name] = values[rv_name]
         else:
-          succ_vals = np.atleast_1d(succ_vals)
-        kwds.update({self._name: pred_vals,
-                     self._name+"'": succ_vals})
-        succ_vals = self._tfun[1](**kwds)
-      elif not isscalar(succ_vals):
-        succ_vals = np.atleast_1d(succ_vals)
-      pred_vals, succ_vals, dims = _reshape_vals(pred_vals, succ_vals)
-
-    vals = collections.OrderedDict({self._name+"'": succ_vals,
-                                    self._name: pred_vals})
-    kwargs.update({'reverse': reverse})
-    return vals, dims, kwargs
+          succ_vals[rv_name] = values
+    return succ_vals
 
 #-------------------------------------------------------------------------------
-  def eval_tran(self, vals, **kwargs):
-    """ Evaluates the transitional conditional probability for the dictionary 
-    arguments in vals with optional keywords in **kwargs.
-    """
+  def eval_tran(self, values, **kwargs):
+    if 'cond' in kwargs:
+      return kwargs['cond']
+    cond = DEFAULT_CONDITIONAL_PROBABILITY[iscomplex(self._pscale)]
     reverse = False if 'reverse' not in kwargs else kwargs['reverse']
-    pred_vals, succ_vals = vals[self._name], vals[self._name+"'"]
-    pred_idx = None if 'pred_idx' not in kwargs else kwargs['pred_idx'] 
-    succ_idx = None if 'succ_idx' not in kwargs else kwargs['succ_idx'] 
-    cond = None
-
-    # Scalar treatment is the most trivial and ignores reverse
-    if self._tran.ret_isscalar():
-      cond = nominal_uniform_prob(pred_vals,
-                                  succ_vals, 
-                                  prob=self._tran(), 
-                                  inside=self._inside) 
-                  
-
-    # Handle discrete non-callables
-    elif not self._tran.ret_callable():
-      prob = self._tran() if not self._tran.ret_istuple() else \
-             self._tran[int(reverse)]()
-      cond = lookup_square_matrix(pred_vals,
-                                  succ_vals, 
-                                  sq_matrix=prob, 
-                                  vset=self._vset,
-                                  col_idx=pred_idx,
-                                  row_idx=succ_idx) 
-
-
-    # That just leaves callables
+    if self._tran is None:
+      if self._tfun is not None: # tfun without tran means no cond. prob.
+        return cond
+      rvs = self._varlist
+      if len(rvs) == 1 and rvs[0]._tran is not None:
+        return rvs[0].eval_tran(values, **kwargs)
+      pred_vals = dict()
+      succ_vals = dict()
+      for key_, val in values.items():
+        prime = key_[-1] == "'"
+        key = key_[:-1] if prime else key_
+        if key in self._keylist:
+          if prime:
+            succ_vals.update({key: val})
+          else:
+            pred_vals.update({key: val})
+      cond, _ = rv_prod_rule(pred_vals, succ_vals, rvs=rvs, pscale=self._pscale)
+    elif not self._tran.callable or self._tran.isscipy:
+      return cond
     else:
-      prob = self._tran if not self._tran.ret_istuple() else \
-             self._tran[int(reverse)]
-      kwds = {self._name: pred_vals,
-              self._name+"'": succ_vals}
-      cond = prob(**kwds)
-
+      cond = self._tran(values) if self._sym_tran else \
+             self._tran[int(reverse)](values)
     return cond
 
 #-------------------------------------------------------------------------------
-  def __call__(self, values=None):
-    """ Return a probability distribution for the quantities in values. """
+  def reval_tran(self, dist):
+    """ Evaluates the conditional reverse-transition function for corresponding 
+    transition conditional distribution dist. This requires a tuple input for
+    self.set_tran() to evaluate a new conditional.
+    """
+    assert isinstance(dist, PD), \
+        "Input must be a distribution, not {} type.".format(type(dist))
+    marg, cond = dist.cond, dist.marg
+    name = margcond_str(marg, cond)
+    vals = collections.OrderedDict(dist)
+    dims = dist.dims
+    # This next line needs to be modified to handle new API
+    """
+    prob = dist.prob if self._sym_tran or self._tran is None \
+           else self._tran[1](dist)
+    """
+    prob = dist.prob
+    pscale = dist.pscale
+    return PD(name, vals, dims=dims, prob=prob, pscale=pscale)
+
+#-------------------------------------------------------------------------------
+  def _eval_iid(self, dist_name, vals, dims, prob, iid):
+    if not iid: 
+      return PD(dist_name, vals, dims=dims, prob=prob, pscale=self._pscale)
+
+    # Deal with IID cases
+    max_dim = None
+    for dim in dims.values():
+      if dim is not None:
+        max_dim = dim if max_dim is None else max(dim, max_dim)
+
+    # If scalar or prob is expected shape then perform product here
+    if max_dim is None or max_dim == prob.ndim - 1:
+      dist = PD(dist_name, vals, dims=dims, prob=prob, pscale=self._pscale)
+      return dist.prod(iid)
+
+    # Otherwise it is left to the user function to perform the iid product
+    for key in iid:
+      vals[key] = {len(vals[key])}
+      dims[key] = None
+
+    # Tidy up probability
+    return PD(dist_name, vals, dims=dims, prob=prob, pscale=self._pscale)
+
+#-------------------------------------------------------------------------------
+  def __call__(self, *args, **kwds):
+    """ Returns a joint distribution p(args) """
+    if not self.anystoch:
+      return Field.__call__(self, *args, **kwds)
+    if not self._nvars:
+      return None
+    iid = False if 'iid' not in kwds else kwds.pop('iid')
+    if type(iid) is bool and iid:
+      iid = self._defiid
+    if not kwds and len(args) == 1 and not isinstance(args[0], dict):
+      arg = {key: args[0] for key in self._keyset}
+      args = arg,
+    values = self.parse_args(*args, **kwds)
     dist_name = self.eval_dist_name(values)
-    vals = self.eval_vals(values)
-    prob = self.eval_prob(vals)
-    dims = {self._name: None} if isscalar(vals) else {self._name: 0}
-    vals = collections.OrderedDict({self._name: vals})
-    return Dist(dist_name, vals, dims, prob, self._pscale)
-
-#-------------------------------------------------------------------------------
-  def step(self, *args, reverse=False):
-    """ Returns a conditional probability distribution for quantities in args.
+    vals, dims = self.evaluate(values, _skip_parsing=True)
+    prob = self.eval_prob(vals, dims)
+    return self._eval_iid(dist_name, vals, dims, prob, iid)
+
+#-------------------------------------------------------------------------------
+  def propose(self, *args, **kwds):
+    """ Returns a proposal distribution p(args[0]) for values """
+    suffix = "'" if 'suffix' not in kwds else kwds.pop('suffix')
+    if not kwds and len(args) == 1 and not isinstance(args[0], dict):
+      arg = {key: args[0] for key in self._keyset}
+      args = arg,
+    values = self.parse_args(*args, **kwds)
+    dist_name = self.eval_dist_name(values, suffix)
+    vals, dims = self.evaluate(values, _skip_parsing=True)
+    prop = self.eval_prop(vals) if self._prop is not None else \
+           self.eval_prob(vals, dims)
+    if suffix:
+      keys = list(vals.keys())
+      for key in keys:
+        mod_key = key + suffix
+        vals.update({mod_key: vals.pop(key)})
+        if key in dims:
+          dims.update({mod_key: dims.pop(key)})
+    return PD(dist_name, vals, dims=dims, prob=prop, pscale=self._pscale)
+
+#-------------------------------------------------------------------------------
+  def step(self, *args, **kwds):
+    """ Returns a proposal distribution p(args[1]) given args[0], depending on
+    whether using self._prop, that denotes a simple proposal distribution,
+    or self._tran, that denotes a transitional distirbution. """
 
-    :param *args: predecessor, successor values to evaluate conditionals.
-    :param reverse: Boolean flag to evaluate conditional probability in reverse.
-
-    :return a Dist instance of the conditional probability distribution
-    """
+    reverse = False if 'reverse' not in kwds else kwds.pop('reverse')
     pred_vals, succ_vals = None, None 
     if len(args) == 1:
       if isinstance(args[0], (list, tuple)) and len(args[0]) == 2:
         pred_vals, succ_vals = args[0][0], args[0][1]
       else:
         pred_vals = args[0]
     elif len(args) == 2:
       pred_vals, succ_vals = args[0], args[1]
+
+    # Evaluate predecessor values
+    if not isinstance(pred_vals, dict):
+      pred_vals = {key: pred_vals for key in self._keyset}
+    pred_vals = self.parse_args(pred_vals, pass_all=True)
     dist_pred_name = self.eval_dist_name(pred_vals)
-    dist_succ_name = None
-    if pred_vals is None and succ_vals is None and \
-        self._vtype not in VTYPES[float]:
-      dist_succ_name = self.eval_dist_name(succ_vals, "'")
-    pred_vals = self.eval_vals(pred_vals)
+    pred_vals, pred_dims = self.evaluate(pred_vals)
+
+    # Default successor values if None and delta is None
+    if succ_vals is None and self._delta is None:
+      pred_values = list(pred_vals.values())
+      if all([isscalar(pred_value) for pred_value in pred_values]):
+        succ_vals = {0}
+      else:
+        succ_vals = pred_vals
+
+    # Evaluate successor evaluates
     vals, dims, kwargs = self.eval_step(pred_vals, succ_vals, reverse=reverse)
+    succ_vals = {key[:-1]: val for key, val in vals.items() if key[-1] == "'"}
     cond = self.eval_tran(vals, **kwargs)
-    if dist_succ_name is None:
-      dist_succ_name = self.eval_dist_name(vals[self.__prime_key], "'")
+    dist_succ_name = self.eval_dist_name(succ_vals, "'")
     dist_name = '|'.join([dist_succ_name, dist_pred_name])
-    return Dist(dist_name, vals, dims, cond, self._pscale)
-    
-#-------------------------------------------------------------------------------
-  def __repr__(self):
-    """ Print representation of RV name """
-    return super().__repr__() + ": '" + self._name + "'"
-
-#-------------------------------------------------------------------------------
-  def __mul__(self, other):
-    """ Logical 'AND' operator between RV and another RV, RJ, or RF. """
-    from probayes.rj import RJ
-    from probayes.rf import RF
-    if isinstance(other, RF):
-      marg = [self] + other.ret_marg().ret_rvs()
-      cond = other.ret_cond().ret_rvs()
-      return RF(marg, cond)
 
-    if isinstance(other, RJ):
-      rvs = [self] + other.ret_rvs()
-      return RJ(*tuple(rvs))
-
-    if isinstance(other, RV):
-      return RJ(self, other)
-
-    raise TypeError("Unrecognised post-operand type {}".format(type(other)))
+    return PD(dist_name, vals, dims=dims, prob=cond, pscale=self._pscale)
 
 #-------------------------------------------------------------------------------
-  def __truediv__(self, other):
-    """ Conditional operator between RV and another RV, RJ, or RF. """
-    from probayes.rj import RJ
-    from probayes.rf import RF
-    if isinstance(other, RF):
-      marg = [self] + other.ret_cond().ret_rvs()
-      cond = other.ret_marg().ret_rvs()
-      return RF(marg, cond)
-
-    if isinstance(other, RJ):
-      return RF(self, other)
+  def __eq__(self, other):
+    """ Equality for RFs is defined as comprising the same RVs """
+    if type(self) is not RF or type(other) is not RF:
+      return super().__eq__(other)
+    return self._keyset == other.keyset
 
-    if isinstance(other, RV):
-      return RF(self, other)
-
-    raise TypeError("Unrecognised post-operand type {}".format(type(other)))
+#-------------------------------------------------------------------------------
+  def __getitem__(self, arg):
+    if not self.issympy or isinstance(arg, int) or \
+        (isinstance(arg, str) and arg in self._keyset):
+      return Field.__getitem__(self, arg)
+    return Prob.__getitem__(self, arg)
 
 #-------------------------------------------------------------------------------
```

### Comparing `probayes-0.0.3/probayes/rv_utils.py` & `probayes-0.0.4/probayes/rv_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,53 @@
 import numpy as np
-from probayes.vtypes import isunitsetint, isunitsetfloat, isunitset, isscalar, \
-                        uniform, eval_vtype, VTYPES
-
-from probayes.pscales import eval_pscale, rescale, iscomplex, NEARLY_NEGATIVE_INF
+from probayes.vtypes import isunitset, isscalar, uniform, eval_vtype, VTYPES
+from probayes.pscales import eval_pscale, iscomplex, NEARLY_NEGATIVE_INF
 """
 A module to provide functional support to rv.py
 """
 #-------------------------------------------------------------------------------
-def nominal_uniform_prob(*args, prob=None, inside=None, pscale=1.):
-  """ Also handles categorical data types if inside is a list. Inside can
-  (and should) be a callable function """
+def uniform_prob(*args, prob=None, inside=None, pscale=1.):
+  """ Uniform probability function for discrete and continuous vtypes. """
 
   # Detect ptype, default to prob if no values, otherwise detect vtype  
   assert len(args) >= 1, "Minimum of a single positional argument"
   pscale = eval_pscale(pscale)
   use_logs = iscomplex(pscale)
   if prob is None:
     prob = 0. if use_logs else 1.
   vals = args[0]
   if vals is None:
     return prob
-  vtype = eval_vtype(vals) if callable(inside) else eval_type(inside)
+  vtype = eval_vtype(vals) if callable(inside) else eval_vtype(inside)
 
   # Set inside function by vtype if not specified
   if not callable(inside):
-    if vtype in VTYPES[bool]:
-      pass
-    elif vtype in VTYPES[float]:
+    if vtype in VTYPES[float]:
       inside = lambda x: np.logical_and(x >= min(inside), x <= max(inside))
     else:
       inside = lambda x: np.isin(x, inside)
 
   # If scalar, check within variable set
   p_zero = NEARLY_NEGATIVE_INF if use_logs else 0.
   if isscalar(vals):
-    if vtype in VTYPES[bool]:
-      prob = prob if vals else \
-             rescale(1. - rescale(prob, pscale, 1.), 1., pscale)
-    else:
-      prob = prob if inside(vals) else p_zero
+    prob = prob if inside(vals) else p_zero
 
-  # Otherwise perform array operations
+  # Otherwise treat as uniform within range
   else:
-
-    # Handle nominal probabilities, that ignores inside
-    if vtype in VTYPES[bool]:
-      prob = rescale(prob, pscale, 1.)
-      p_false = 1. - prob
-      prob = np.tile(prob, vals.shape)
-      prob[np.logical_not(vals)] = p_false
-      prob = rescale(prob, 1., pscale)
-
-    # Otherwise treat as uniform within range
-    else:
-      p_true = prob
-      prob = np.tile(p_zero, vals.shape)
-      prob[inside(vals)] = p_true
+    p_true = prob
+    prob = np.tile(p_zero, vals.shape)
+    prob[inside(vals)] = p_true
 
   # This section below is there just to play nicely with conditionals
   if len(args) > 1:
     for arg in args[1:]:
       if use_logs:
-        prob = prob + nominal_uniform_prob(arg, inside=inside, pscale=0.j)
+        prob = prob + uniform_prob(arg, inside=inside, pscale=0.j)
       else:
-        prob = prob * nominal_uniform_prob(arg, inside=inside)
+        prob = prob * uniform_prob(arg, inside=inside)
   return prob
 
 #-------------------------------------------------------------------------------
 def matrix_cond_sample(pred_vals, succ_vals, prob, vset=None):
   """ Returns succ_vals with sampling """
   if not isunitset(succ_vals):
     return succ_vals
@@ -108,15 +88,14 @@
     vset = sorted(vset)
   rc_scalar = False
   if row_idx is None:
     if isscalar(row_vals):
       rc_scalar = True
       row_idx = vset.index(row_vals)
     else:
-      row_shape = None
       if isinstance(row_vals, np.ndarray):
         row_vals = np.ravel(row_vals).tolist()
       row_idx = [vset.index(row_val) for row_val in row_vals]
   elif isscalar(row_idx):
       rc_scalar = True
   if col_idx is None:
     if isscalar(col_vals):
```

### Comparing `probayes-0.0.3/probayes/sp.py` & `probayes-0.0.4/probayes/sp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-"""
-A stocastic process is an indexable sequence of realisations of a stochastic 
-condition. It is therefore implemented here using a sample generator that 
-iteratively samples a stochastic condition.
-"""
+""" Provides SP, a class for stochastic processes """
+
 #-------------------------------------------------------------------------------
-import numpy as np
 import collections
 import inspect
 import warnings
-from probayes.rf import RF
-from probayes.func import Func
-from probayes.dist import Dist
-from probayes.dist_utils import summate
+from probayes.sd import SD
+from probayes.expression import Expression
+from probayes.pd import PD
+from probayes.pd_utils import summate
 from probayes.sp_utils import sample_generator, MCMC_SAMPLERS
 
 #-------------------------------------------------------------------------------
-class SP (RF):
-
-  # Public
-  stuv = None     # scores + thresholds + update + veridct
-  opqrstuv = None # opqr + stuv
+class SP (SD):
+  """ A stocastic process is stochastic dependence that supports an indexable 
+  sequence of realisations from a directed graph. It is therefore implemented 
+  here using a sample generator that iteratively samples a directed graph.
+  """
 
   # Protected
   _scores = None # Scores function used for the basis of acceptance
   _thresh = None # Threshold function to compare with scores
   _update = None # Update function (output True, None, or False)
 
   # Private
@@ -33,108 +29,137 @@
 
 #-------------------------------------------------------------------------------
   def __init__(self, *args, **kwds):
     super().__init__(*args, **kwds)
     self.reset()
 
 #-------------------------------------------------------------------------------
-  def _refresh(self):
-    super()._refresh()
-    if self._marg is None and self._cond is None:
+  @property
+  def stuv(self):
+    return self._stuv
+
+  @property
+  def opqrstuv(self):
+    return self._opqrstuv
+
+  def _refresh(self, *args, **kwds):
+    super()._refresh(*args, **kwds)
+    if not self._nvars:
       return
-    self.stuv = collections.namedtuple(self._id, ['s', 't', 'u', 'v'])
-    self.opqrstuv = collections.namedtuple(self._id, 
+    self._stuv = collections.namedtuple(self._id, ['s', 't', 'u', 'v'])
+    self._opqrstuv = collections.namedtuple(self._id, 
                         ['o', 'p', 'q', 'r', 's', 't', 'u', 'v'])
 
 #-------------------------------------------------------------------------------
+  @property
+  def scores(self):
+    return self._scores
+
   def set_scores(self, scores=None, *args, **kwds):
     self._scores = scores
     if self._scores is None:
       return
     if self._scores in MCMC_SAMPLERS:
       assert not args and not kwds, \
           "Neither args nor kwds permitted with spec '{}'".format(self._scores)
       self.set_scores(MCMC_SAMPLERS[self._scores][0], pscale=self._pscale)
       self.set_thresh(scores)
       return
-    self._scores = Func(self._scores, *args, **kwds)
+    self._scores = Expression(self._scores, *args, **kwds)
 
 #-------------------------------------------------------------------------------
+  @property
+  def thresh(self):
+    return self._thresh
+
   def set_thresh(self, thresh=None, *args, **kwds):
     self._thresh = thresh
     if self._thresh is None:
       return
     if self._thresh in MCMC_SAMPLERS:
       assert not args and not kwds, \
           "Neither args nor kwds permitted with spec '{}'".format(self._thresh)
       self.set_thresh(MCMC_SAMPLERS[self._thresh][1])
       self.set_update(thresh)
       return
-    self._thresh = Func(self._thresh, *args, **kwds)
+    self._thresh = Expression(self._thresh, *args, **kwds)
 
 #-------------------------------------------------------------------------------
+  @property
+  def update(self):
+    return self._update
+
   def set_update(self, update=None, *args, **kwds):
     self._update = update
     if self._update is None:
       return
     if self._update in MCMC_SAMPLERS:
       assert not args and not kwds, \
           "Neither args nor kwds permitted with spec '{}'".format(self._update)
       self.set_update(MCMC_SAMPLERS[self._update][2])
       return
-    self._update = Func(self._update, *args, **kwds)
+    self._update = Expression(self._update, *args, **kwds)
 
 #-------------------------------------------------------------------------------
-  def eval_func(self, func=None, *args, **kwds):
-    if func is None:
-      return func
-    assert isinstance(func, Func), \
-        "Evaluation of func no possible for type {}".format(type(func))
-    if not func.ret_callable():
-      return func()
-    return func(*args, **kwds)
+  def eval_expr(self, expr=None, *args, **kwds):
+    if expr is None:
+      return expr
+    assert isinstance(expr, Expression), \
+        "Evaluation of expr no possible for type {}".format(type(expr))
+    if not expr.callable:
+      return expr()
+    return expr(*args, **kwds)
 
 #-------------------------------------------------------------------------------
   def reset(self, sampler_id=None, reset_last=True): # Leave option to preseve
     if self.__samplers is None or sampler_id is None:
       self.__samplers = []
     if self.__counter is None:
       self.__counter = collections.Counter()
     if self.__last is None:
       self.__last = collections.OrderedDict()
     if sampler_id is None:
       return
-    sampler = self.ret_sampler(sampler_id)
+    sampler = self.get_sampler(sampler_id)
     self.__counter[sampler] = 0
     if sampler not in self.__last:
       self.__last[sampler] = None
     elif reset_last:
       self.__last[sampler] = None
     return self.__samplers, self.__counter, self.__last
 
 #-------------------------------------------------------------------------------
   def __call__(self, *args, **kwds):
-    if not len(args) or len(kwds) or \
-        not isinstance(args[0], (list, tuple, collections.deque)):
-      return super().__call__(*args, **kwds)
-    samples = args[0]
-    if not len(samples):
-      return super().__call__(*args, **kwds)
+    conditionalise = None if 'conditionalise' not in kwds else \
+                     kwds.pop('conditionalise')
 
     # Summating distributions is straightforward
-    if isinstance(samples[0], Dist):
+    samples = None if not len(args) else args[0]
+    if samples and isinstance(samples, (list, tuple, collections.deque)) \
+        and len(samples) and isinstance(samples[0], PD):
       samples = list(samples)
       for sample in samples[1:]:
-        assert isinstance(sample, Dist),\
+        assert isinstance(sample, PD),\
             "If using distributions, all samples must be distributions, not {}".\
             format(type(sample))
       if isinstance(samples, (list, collections.deque)):
         samples = tuple(samples)
-      return summate(*samples)
+      dist = summate(*samples)
+      if not conditionalise:
+        return dist
+      return dist.conditionalise(self._leafs.keyset)
+
+    # If empty call or dictionary arguments, pass to SD
+    if not samples or len(kwds) or \
+        not isinstance(samples, (list, tuple, collections.deque)):
+      return super().__call__(*args, **kwds)
+    if not len(samples):
+      return super().__call__(*args, **kwds)
 
+    # Otherwise this call is SP-specific
     opqrstuv = collections.OrderedDict({key: None for key in \
         ['o', 'p', 'q', 'r', 's', 't', 'u', 'v']})
 
     # We exclude update=False from the summation
     opqrstuv['u'] = []
 
     def _maybe_append(element, key):
@@ -147,15 +172,15 @@
       if isinstance(sample, self.opqr):
         _maybe_append(sample.o, 'o')
         _maybe_append(sample.p, 'p')
         _maybe_append(sample.q, 'q')
         _maybe_append(sample.r, 'r')
       
       else:
-        assert isinstance(sample, self.opqrstuv), \
+        assert isinstance(sample, self._opqrstuv), \
             "Sample must be outputted from sampler: {}".format(self._id)
         if sample.u == False:
           continue
         if self._update is not None:
           opqrstuv['u'].append(sample.u)
         _maybe_append(sample.o, 'o')
         _maybe_append(sample.p, 'p')
@@ -164,80 +189,84 @@
         _maybe_append(sample.s, 's')
         _maybe_append(sample.t, 't')
         _maybe_append(sample.v, 'v')
           
     for key in ['o', 'p', 'q', 'r', 'v']:
       if opqrstuv[key] is not None:
         opqrstuv[key] = summate(*tuple(opqrstuv[key]))
-    return self.opqrstuv(**opqrstuv)
+        if conditionalise and key in ['o', 'p', 'v']:
+          opqrstuv[key] = opqrstuv[key].conditionalise(self._leafs.keyset)
+    return self._opqrstuv(**opqrstuv)
 
 #-------------------------------------------------------------------------------
-  def ret_sampler(self, sampler_id=None):
+  def get_sampler(self, sampler_id=None):
     if sampler_id is None:
       return self.__samplers
     if type(sampler_id) is int:
       return self.__samplers[sampler_id]
     return sampler_id
 
 #-------------------------------------------------------------------------------
-  def ret_counter(self, sampler_id=None):
+  def get_counter(self, sampler_id=None):
     if sampler_id is None:
       return self.__counter
-    return self.__counter[self.ret_sampler(sampler_id)]
+    return self.__counter[self.get_sampler(sampler_id)]
 
 #-------------------------------------------------------------------------------
-  def ret_last(self, sampler_id=None):
+  def get_last(self, sampler_id=None):
     if sampler_id is None:
       return self.__last
-    return self.__last[self.ret_sampler(sampler_id)]
+    return self.__last[self.get_sampler(sampler_id)]
 
 #-------------------------------------------------------------------------------
   def next(self, sampler_id, *args, **kwds):
 
     # Reset counters
-    sampler = self.ret_sampler(sampler_id)
+    sampler = self.get_sampler(sampler_id)
     self.__counter[sampler] += 1
     last = self.__last[sampler]
+    no_proposal = self._tran is None and self._tfun is None and \
+                  not self._unit_tran and self._prop is None
 
     # Treat sampling without proposals as a distribution call
-    if last is None or \
-        (self._tran is None and not self._unit_tran and self._prop is None):
+    if last is None or no_proposal:
       opqr = self.sample(*args, **kwds)
-      if self._tran is None and not self._unit_tran and self._prop is None:
+      if no_proposal:
         return opqr
 
     # Otherwise refeed last proposals into sample function
     else:
-      if self._tran is None and not self._unit_tran and self._delta is None:
+      if self._tran is None and self._tfun is None and not self._unit_tran and \
+          self._delta is None:
         last = {0}
       if len(args) < 2:
         opqr = self.sample(last, **kwds)
       else:
         args = tuple([last] + list(args[1:]))
         opqr = self.sample(*args, **kwds)
 
     # Set to last if accept is not False
-    stuv = self.stuv(self.eval_func(self._scores, opqr),
-                     self.eval_func(self._thresh),
-                     None,
-                     None)
-    update = self.eval_func(self._update, stuv)
+    stuv = self._stuv(self.eval_expr(self._scores, opqr),
+                      self.eval_expr(self._thresh),
+                      None,
+                      None)
+    update = self.eval_expr(self._update, stuv)
     verdit = opqr.o
     if self._update is None or self.__last[sampler] is None or update:
       self.__last[sampler] = opqr
       verdit = opqr.p
-    return self.opqrstuv(opqr.o, opqr.p, opqr.q, opqr.r, 
-                         stuv.s, stuv.t, update, verdit)
+    return self._opqrstuv(opqr.o, opqr.p, opqr.q, opqr.r, 
+                          stuv.s, stuv.t, update, verdit)
 
 #-------------------------------------------------------------------------------
   def sampler(self, *args, **kwds):
     if self.__samplers is None:
       self.reset()
     if not args:
-      args = {0},
+      args = {0}, # Default to randomly sampling variables as scalars
     elif len(args) == 1 and type(args[0]) is int and 'stop' not in kwds:
       kwds.update({'stop': args[0]})
       args = {0},
     stop = None if 'stop' not in kwds else kwds.pop('stop')
     sampler = sample_generator(self, 
                                len(self.__samplers), 
                                *args, 
@@ -262,8 +291,7 @@
     for sample in sampler:
       if len(steps) >= stop:
         break
       steps.append(sample)
     return steps
 
 #-------------------------------------------------------------------------------
-
```

### Comparing `probayes-0.0.3/probayes/sp_utils.py` & `probayes-0.0.4/probayes/sp_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """ A utility module for stochasptic process classes """
 
 import numpy as np
 from probayes.vtypes import isscalar
-from probayes.pscales import iscomplex, rescale, log_prob, div_prob
+from probayes.pscales import rescale, div_prob
 
 #-------------------------------------------------------------------------------
 def sample_generator(sp, sampler_id, *args, stop=None, **kwds):
   if stop is None:
     while True:
       yield sp.next(sampler_id, *args, **kwds)
   else:
-    while sp.ret_counter(sampler_id) < stop:
+    while sp.get_counter(sampler_id) < stop:
       yield sp.next(sampler_id, *args, **kwds)
     else:
       sp.reset(sampler_id)
 
 #-------------------------------------------------------------------------------
 def metropolis_scores(opqr, pscale=None):
   pred, succ = opqr.o, opqr.p
```

### Comparing `probayes-0.0.3/probayes/vtypes.py` & `probayes-0.0.4/probayes/vtypes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """
 A module that handles variable data types.
 """
 
 #-------------------------------------------------------------------------------
 import numpy as np
+import sympy
 import functools
 import operator
 
 #-------------------------------------------------------------------------------
 VTYPES = {
-          bool: (bool, np.dtype('bool')),
-          int:  (int, np.dtype('int'), np.dtype('int32'), np.dtype('int64'),
-                 np.uint, np.uint8, np.uint16, np.uint32, np.uint64),
-          float: (float, np.dtype('float'),  np.dtype('float32'), np.dtype('float64')),
+          bool: {bool, np.dtype('bool')},
+          int:  {int, np.dtype('int'), np.dtype('int32'), np.dtype('int64'),
+                 np.uint, np.uint8, np.uint16, np.uint32, np.uint64},
+          float: {float, np.dtype('float'),  np.dtype('float32'), np.dtype('float64')},
          }
 
+
+OO = sympy.oo
+OO_TO_NP = {OO: np.inf, -OO: -np.inf}
+
 #-------------------------------------------------------------------------------
 def eval_vtype(vtype):
   """ Evaluates a variable type from input vtype.
 
   :param vtype: input object
 
   :return: either bool, int, float if correctly detected. 
@@ -28,24 +33,25 @@
     vtype = list(vtype)
   if isinstance(vtype, (list, tuple)):
     if any([isinstance(_vtype, tuple) for _vtype in vtype]):
         vtype = np.concatenate([np.array(_vtype).reshape([1]) \
                                 for _vtype in vtype]).dtype
     else:
       vtype = np.array(vtype)
-  if isinstance(vtype, np.ndarray):
+  if hasattr(vtype, 'dtype'):
     vtype = vtype.dtype
-  elif hasattr(vtype, 'type'):
-    vtype = vtype.type
+  else:
+    _vtype = vtype
+    while _vtype != type:
+      vtype = _vtype
+      _vtype = type(vtype)
+  if vtype in VTYPES.keys():
+    return vtype
   for key, val in VTYPES.items():
-    try:
-      found = vtype in val
-    except TypeError:
-      vtype = type(vtype)
-      found = vtype in val
+    found = vtype in set(val)
     if found:
       vtype = key
       break
   return vtype
 
 #-------------------------------------------------------------------------------
 def isunitset(var, vtype=None):
@@ -54,15 +60,15 @@
   :param var: variable to assess.
   :param vtype: optional filter for variable type (e.g. int or float)
   """
   if vtype is None:
     vtype = list(VTYPES.keys())
   elif not isinstance(vtype, (tuple,list)):
     vtype = [vtype]
-  vtypes = functools.reduce(operator.concat, [VTYPES[key] for key in vtype])
+  vtypes = functools.reduce(operator.concat, [list(VTYPES[key]) for key in vtype])
   if isinstance(var, set):
     if len(var) == 1:
       element_type = type(list(var)[0])
       if element_type in vtypes:
         return True
   return False
 
@@ -82,20 +88,23 @@
   """ Returns boolean flag as to whether var is a set of one float element.
   Usage requests a sampling of value from a ICDF for then given P.
   """
   return isunitset(var, float)
 
 #-------------------------------------------------------------------------------
 def isscalar(var):
-  """ If var is a dimensionless numpy array of size, this function returns True
-  otherwise np.isscalar(var) is returned.
+  """ If var is a dimensionless numpy array of size 1 or if the var is a Sympy 
+  Float or Integer, this function returns True, otherwise it returns 
+  np.isscalar(var).
   """
   if isinstance(var, np.ndarray):
     if var.ndim == 0 and var.size == 1:
       return True
+  if isinstance(var, (sympy.Float, sympy.Integer)):
+    return True
   return np.isscalar(var)
 
 #-------------------------------------------------------------------------------
 def issingleton(var):
   """ If isunitset(var) is True, this function returns True, 
   otherwise isscalar(var) is returned.
   """
@@ -114,14 +123,27 @@
     return True
   if isinstance(var, np.ndarray):
     if var.size == 1:
       return True
   return False
 
 #-------------------------------------------------------------------------------
+def isfinite(var):
+  if isinstance(var, np.ndarray) or np.isscalar(var):
+    return np.isfinite(var)
+  if isinstance(var, (tuple, list)):
+    isfin = [isfinite(subvar) for subvar in var]
+    if isinstance(var, list):
+      return isfin
+    return tuple(isfin)
+  if var == OO or var == -OO:
+    return False
+  return True
+
+#-------------------------------------------------------------------------------
 def isdimensionless(var):
   """ If var is {0}, then True is returned, otherwise np.isscalar(var) is
   returned.
   """
   if isinstance(var, set):
     if len(var) == 1:
       var = list(var)[0]
@@ -177,8 +199,9 @@
     return np.linspace(v_0, v_1, n+1)[1:]
   if not ex_0 and ex_1:
     return np.linspace(v_0, v_1, n+1)[:-1]
 
   # We shouldn't reach here
   raise ValueError("Unrecognised exclusions {} and {}".format(ex_0, ex_1))
 
+
 #-------------------------------------------------------------------------------
```

### Comparing `probayes-0.0.3/probayes.egg-info/PKG-INFO` & `probayes-0.0.4/probayes.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: probayes
-Version: 0.0.3
+Version: 0.0.4
 Summary: Probability package supporting multiple Bayesian methods including MCMC
 Home-page: https://github.com/Bhumbra/probayes
 Author: Bhumbra
 Author-email: bhumbra@gmail.com
 License: UNKNOWN
 Description: # probayes
         Probability package supporting multiple Bayesian methods including MCMC
@@ -13,27 +13,26 @@
         of probability. Since probayes is its infancy and in a state of flux, there is no manual. Currently probayes supports
         the following:
         
         1. Multiple random variable sampling in untransformed and transformed domain space. 
         2. Transitional simulation, including random walks, using Markov chain conditionals.
         3. Discrete grid exact inference.
         4. Ordinary Monte Carlo random sampling.
-        5. Ordinary Monto Carlo rejection sampling.
+        5. Ordinary Monte Carlo rejection sampling.
         6. Metropolis-Hastings MCMC sampling.
         7. Limited support for multivariate normal-covariance Gibbs sampling.
         
         In the near-future, it is intended to expand the scope of probayes to include:
         
-        1. Support Gibbs sampling using semi-conjugacy.
-        2. Code initial support for approximate inference using using dense mean field messaging.
-        3. Support derivative-based updates (HMC, gradient ascent/descent optimisation).
+        1. Code initial support for approximate inference using using dense mean field messaging.
+        2. Support derivative-based updates (HMC, gradient ascent/descent optimisation).
         
         A quickstart is also intended, but for now there are examples in the examples/ subdirectories:
         
-        1. tests/        Simple test scripts
+        1. checks/       Simple check scripts
         2. rv_examples/  Random variable examples
         3. markov/       Markov chain examples
         4. cov_examples/ Examples of using covariance matrices
         5. dgei/         Discrete grid exact inference examples
         6. omc/          Ordinary Monte-Carlo examples
         7. mcmc/         Markov chain Monte Carlo examples (Metropolis-Hastings, Gibbs...)
```

