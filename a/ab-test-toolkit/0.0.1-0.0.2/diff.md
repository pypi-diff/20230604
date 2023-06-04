# Comparing `tmp/ab-test-toolkit-0.0.1.tar.gz` & `tmp/ab-test-toolkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab-test-toolkit-0.0.1.tar", last modified: Sat Jun  3 07:37:52 2023, max compression
+gzip compressed data, was "ab-test-toolkit-0.0.2.tar", last modified: Sun Jun  4 21:13:04 2023, max compression
```

## Comparing `ab-test-toolkit-0.0.1.tar` & `ab-test-toolkit-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-03 07:37:52.763974 ab-test-toolkit-0.0.1/
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     1064 2023-06-03 07:13:56.000000 ab-test-toolkit-0.0.1/LICENSE
--rw-rw-r--   0 kolja     (1000) kolja     (1000)      111 2023-04-27 10:12:58.000000 ab-test-toolkit-0.0.1/MANIFEST.in
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     7471 2023-06-03 07:37:52.759974 ab-test-toolkit-0.0.1/PKG-INFO
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     5039 2023-06-03 07:24:25.000000 ab-test-toolkit-0.0.1/README.md
-drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-03 07:37:52.759974 ab-test-toolkit-0.0.1/ab_test_toolkit/
--rw-rw-r--   0 kolja     (1000) kolja     (1000)       22 2023-06-03 07:21:57.000000 ab-test-toolkit-0.0.1/ab_test_toolkit/__init__.py
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     3968 2023-06-03 07:21:57.000000 ab-test-toolkit-0.0.1/ab_test_toolkit/_modidx.py
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     3099 2023-06-03 07:21:57.000000 ab-test-toolkit-0.0.1/ab_test_toolkit/generator.py
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     5872 2023-06-03 07:21:57.000000 ab-test-toolkit-0.0.1/ab_test_toolkit/plotting.py
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     7906 2023-06-03 07:21:57.000000 ab-test-toolkit-0.0.1/ab_test_toolkit/power.py
--rw-rw-r--   0 kolja     (1000) kolja     (1000)      291 2023-06-03 07:21:57.000000 ab-test-toolkit-0.0.1/ab_test_toolkit/wrappers.py
-drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-03 07:37:52.759974 ab-test-toolkit-0.0.1/ab_test_toolkit.egg-info/
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     7471 2023-06-03 07:37:52.000000 ab-test-toolkit-0.0.1/ab_test_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 kolja     (1000) kolja     (1000)      490 2023-06-03 07:37:52.000000 ab-test-toolkit-0.0.1/ab_test_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 kolja     (1000) kolja     (1000)        1 2023-06-03 07:37:52.000000 ab-test-toolkit-0.0.1/ab_test_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 kolja     (1000) kolja     (1000)       73 2023-06-03 07:37:52.000000 ab-test-toolkit-0.0.1/ab_test_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 kolja     (1000) kolja     (1000)        1 2023-06-03 07:19:15.000000 ab-test-toolkit-0.0.1/ab_test_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 kolja     (1000) kolja     (1000)       98 2023-06-03 07:37:52.000000 ab-test-toolkit-0.0.1/ab_test_toolkit.egg-info/requires.txt
--rw-rw-r--   0 kolja     (1000) kolja     (1000)       16 2023-06-03 07:37:52.000000 ab-test-toolkit-0.0.1/ab_test_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 kolja     (1000) kolja     (1000)      972 2023-06-03 07:14:25.000000 ab-test-toolkit-0.0.1/settings.ini
--rw-rw-r--   0 kolja     (1000) kolja     (1000)       38 2023-06-03 07:37:52.763974 ab-test-toolkit-0.0.1/setup.cfg
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     2711 2023-06-03 07:16:06.000000 ab-test-toolkit-0.0.1/setup.py
+drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-04 21:13:04.804359 ab-test-toolkit-0.0.2/
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     1064 2023-06-03 07:13:56.000000 ab-test-toolkit-0.0.2/LICENSE
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)      111 2023-04-27 10:12:58.000000 ab-test-toolkit-0.0.2/MANIFEST.in
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     7231 2023-06-04 21:13:04.804359 ab-test-toolkit-0.0.2/PKG-INFO
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     4868 2023-06-04 21:03:55.000000 ab-test-toolkit-0.0.2/README.md
+drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-04 21:13:04.804359 ab-test-toolkit-0.0.2/ab_test_toolkit/
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       22 2023-06-04 21:03:08.000000 ab-test-toolkit-0.0.2/ab_test_toolkit/__init__.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     3968 2023-06-04 21:03:08.000000 ab-test-toolkit-0.0.2/ab_test_toolkit/_modidx.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     3570 2023-06-04 21:03:08.000000 ab-test-toolkit-0.0.2/ab_test_toolkit/generator.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     5872 2023-06-04 21:03:08.000000 ab-test-toolkit-0.0.2/ab_test_toolkit/plotting.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     8334 2023-06-04 21:03:08.000000 ab-test-toolkit-0.0.2/ab_test_toolkit/power.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     2033 2023-06-04 21:03:08.000000 ab-test-toolkit-0.0.2/ab_test_toolkit/wrappers.py
+drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-04 21:13:04.804359 ab-test-toolkit-0.0.2/ab_test_toolkit.egg-info/
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     7231 2023-06-04 21:13:04.000000 ab-test-toolkit-0.0.2/ab_test_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)      490 2023-06-04 21:13:04.000000 ab-test-toolkit-0.0.2/ab_test_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)        1 2023-06-04 21:13:04.000000 ab-test-toolkit-0.0.2/ab_test_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       73 2023-06-04 21:13:04.000000 ab-test-toolkit-0.0.2/ab_test_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)        1 2023-06-03 07:19:15.000000 ab-test-toolkit-0.0.2/ab_test_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       98 2023-06-04 21:13:04.000000 ab-test-toolkit-0.0.2/ab_test_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       16 2023-06-04 21:13:04.000000 ab-test-toolkit-0.0.2/ab_test_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)      951 2023-06-04 21:13:01.000000 ab-test-toolkit-0.0.2/settings.ini
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       38 2023-06-04 21:13:04.804359 ab-test-toolkit-0.0.2/setup.cfg
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     2711 2023-06-03 07:16:06.000000 ab-test-toolkit-0.0.2/setup.py
```

### Comparing `ab-test-toolkit-0.0.1/LICENSE` & `ab-test-toolkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.1/PKG-INFO` & `ab-test-toolkit-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ab-test-toolkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolkit to simulate and analyze AB tests
 Home-page: https://github.com/k111git/ab-test-toolkit
 Author: Kolja
-Author-email: kolja.kleineberg@dwins.de
+Author-email: 
 License: Apache Software License 2.0
 Description: ab-test-toolkit
         ================
         
         <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
         
         ## Install
@@ -39,15 +39,15 @@
         ```
         
         ## Binary target (e.g. conversion rate experiments)
         
         ### Sample size:
         
         We can calculate the sample size required with the function
-        “sample_size_chi2”. Input needed is:
+        “sample_size_binary”. Input needed is:
         
         - Conversion rate control: cr0
         
         - Conversion rate variant for minimal detectable effect: cr1 (for
           example, if we have a conversion rate of 1% and want to detect an
           effect of at least 20% relate, we would set cr0=0.010 and cr1=0.012)
         
@@ -77,31 +77,27 @@
             alpha=0.05,
             power=0.8,
             one_sided=True,
         )
         print(f"Required sample size per variant is {int(n_sample)}.")
         ```
         
-            Required sample size per variant is 33560.
-        
         ``` python
         n_sample_two_sided = sample_size_binary(
             cr0=0.01,
             cr1=0.012,
             alpha=0.05,
             power=0.8,
             one_sided=False,
         )
         print(
             f"For the two-sided experiment, required sample size per variant is {int(n_sample_two_sided)}."
         )
         ```
         
-            For the two-sided experiment, required sample size per variant is 42606.
-        
         ### Power simulations
         
         What happens if we use a smaller sample size? And how can we understand
         the sample size?
         
         Let us analyze the statistical power with synthethic data. We can do
         this with the simulate_power_binary function. We are using some default
@@ -138,15 +134,15 @@
         
         Here we assume normally distributed data (which usually holds due to the
         central limit theorem).
         
         ### Sample size
         
         We can calculate the sample size required with the function
-        “continuous_sample_size”. Input needed is:
+        “sample_size_continuous”. Input needed is:
         
         - mu1: Mean of the control group
         
         - mu2: Mean of the variant group assuming minimal detectable effect
           (e.g. if the mean it 5, and we want to detect an effect as small as
           0.05, mu1=5.00 and mu2=5.05)
         
@@ -160,16 +156,14 @@
         ``` python
         n_sample = sample_size_continuous(
             mu1=5.0, mu2=5.05, sigma=1, alpha=0.05, power=0.8, one_sided=True
         )
         print(f"Required sample size per variant is {int(n_sample)}.")
         ```
         
-            Required sample size per variant is 4946.
-        
         Let us also do some simulations. These show results for the t-test as
         well as bayesian testing (only 1-sided).
         
         ``` python
         # simulation = simulate_power_continuous()
         ```
         
@@ -207,15 +201,15 @@
         
         ``` python
         df = generate_binary_data()
         df_contingency = data_to_contingency(df)
         # fig = plot_betas(df_contingency, xmin=0, xmax=0.04)
         ```
         
-Keywords: nbdev jupyter notebook python
+Keywords: python experimentation AB-testing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ab-test-toolkit-0.0.1/README.md` & `ab-test-toolkit-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ```
 
 ## Binary target (e.g. conversion rate experiments)
 
 ### Sample size:
 
 We can calculate the sample size required with the function
-“sample_size_chi2”. Input needed is:
+“sample_size_binary”. Input needed is:
 
 - Conversion rate control: cr0
 
 - Conversion rate variant for minimal detectable effect: cr1 (for
   example, if we have a conversion rate of 1% and want to detect an
   effect of at least 20% relate, we would set cr0=0.010 and cr1=0.012)
 
@@ -69,31 +69,27 @@
     alpha=0.05,
     power=0.8,
     one_sided=True,
 )
 print(f"Required sample size per variant is {int(n_sample)}.")
 ```
 
-    Required sample size per variant is 33560.
-
 ``` python
 n_sample_two_sided = sample_size_binary(
     cr0=0.01,
     cr1=0.012,
     alpha=0.05,
     power=0.8,
     one_sided=False,
 )
 print(
     f"For the two-sided experiment, required sample size per variant is {int(n_sample_two_sided)}."
 )
 ```
 
-    For the two-sided experiment, required sample size per variant is 42606.
-
 ### Power simulations
 
 What happens if we use a smaller sample size? And how can we understand
 the sample size?
 
 Let us analyze the statistical power with synthethic data. We can do
 this with the simulate_power_binary function. We are using some default
@@ -130,15 +126,15 @@
 
 Here we assume normally distributed data (which usually holds due to the
 central limit theorem).
 
 ### Sample size
 
 We can calculate the sample size required with the function
-“continuous_sample_size”. Input needed is:
+“sample_size_continuous”. Input needed is:
 
 - mu1: Mean of the control group
 
 - mu2: Mean of the variant group assuming minimal detectable effect
   (e.g. if the mean it 5, and we want to detect an effect as small as
   0.05, mu1=5.00 and mu2=5.05)
 
@@ -152,16 +148,14 @@
 ``` python
 n_sample = sample_size_continuous(
     mu1=5.0, mu2=5.05, sigma=1, alpha=0.05, power=0.8, one_sided=True
 )
 print(f"Required sample size per variant is {int(n_sample)}.")
 ```
 
-    Required sample size per variant is 4946.
-
 Let us also do some simulations. These show results for the t-test as
 well as bayesian testing (only 1-sided).
 
 ``` python
 # simulation = simulate_power_continuous()
 ```
```

### Comparing `ab-test-toolkit-0.0.1/ab_test_toolkit/_modidx.py` & `ab-test-toolkit-0.0.2/ab_test_toolkit/_modidx.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.1/ab_test_toolkit/generator.py` & `ab-test-toolkit-0.0.2/ab_test_toolkit/generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,27 +60,37 @@
         users=("target", "size"), converted=("target", "sum")
     )
     df_result["not_converted"] = df_result["users"] - df_result["converted"]
     df_result["cvr"] = df_result["converted"] / df_result["users"]
     return df_result
 
 # %% ../nbs/00_data_generation.ipynb 11
-def generate_contingency(N=1000, split=0.50, cr0=0.010, cr1=0.011):
+def generate_contingency(N=1000, split=0.50, cr0=0.010, cr1=0.011,exact=False):
     """
     Generate contingency table using binominal distribution
+    For exact=False, we draw the numbers from the binominal distribution.
+    For exact=True, we calculate the numbers from multiplying number users * conversion rate
     """
     assert N > 5, "N need to be more than 5"
     assert split >= 0.01, "Split needs to be >= 1%"
     assert split <= 0.99, "Split needs to be <= 99%"
-    while True:
-        n1 = binom.rvs(N, split, loc=0, size=1)[0]
-        if n1 < N and n1 > 0:
-            break
-    n0 = N - n1
-    c0 = binom.rvs(n0, cr0, loc=0, size=1)[0]
-    c1 = binom.rvs(n1, cr1, loc=0, size=1)[0]
+    if exact==False:
+        while True:
+            n1 = binom.rvs(N, split, loc=0, size=1)[0]
+            if n1 < N and n1 > 0:
+                break
+        n0 = N - n1
+        c0 = binom.rvs(n0, cr0, loc=0, size=1)[0]
+        c1 = binom.rvs(n1, cr1, loc=0, size=1)[0]
+    elif exact==True:
+        n0=int(np.round(N*split))
+        n1=N-n1
+        c0=int(np.round(n0*cr0))
+        c1=int(np.round(n1*cr1))
+    else:
+        raise Exception("Invalid input for exact parameter in generate_contingency function.")
     df_result = pd.DataFrame(
         {"group": [0, 1], "users": [n0, n1], "converted": [c0, c1]}
     )
     df_result["not_converted"] = df_result["users"] - df_result["converted"]
     df_result["cvr"] = df_result["converted"] / df_result["users"]
     return df_result.set_index('group')
```

### Comparing `ab-test-toolkit-0.0.1/ab_test_toolkit/plotting.py` & `ab-test-toolkit-0.0.2/ab_test_toolkit/plotting.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.1/ab_test_toolkit/power.py` & `ab-test-toolkit-0.0.2/ab_test_toolkit/power.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from scipy.stats import chi2_contingency, ttest_ind, fisher_exact, binom, norm
 
 
 from ab_test_toolkit.generator import (
     generate_binary_data,
     data_to_contingency,
     generate_continuous_data,
+    generate_contingency
 )
 
 from bayesian_testing.experiments import BinaryDataTest, NormalDataTest
 
 # %% ../nbs/01_power.ipynb 7
 def _compute_sample_size_from_powerline(sizes, powerline, power):
     """
@@ -45,18 +46,21 @@
     sizes=np.arange(10000, 100001, 10000),
     cr0=0.010,
     cr1=0.012,
     realizations=1000,
     alpha=0.05,
     one_sided=True,
     power=0.8,
+    fast=True
 ):
     """
     Simulates the power using two test: Bayesian testing (Probability B>A) and fisher test (p-value).
     Return total sample size (e.g. we need to devide by 2 for each variant sample size given 50/50 split)
+    Fast = True: Contigency table drawn from binom distribution
+    Fast = False: Contigency table built form data generated at individual level
     """
     if one_sided == True:
         alternative = "greater"
         alternative_z = "larger"
         print("One sided.")
     else:
         alternative = "two-sided"
@@ -67,16 +71,21 @@
     pvs_z = dict()
     # run simulations for each sample size
     for idx, size in enumerate(sizes):
         pvs[idx] = []
         pvs_fisher[idx] = []
         pvs_z[idx] = []
         for realization in range(0, realizations):
-            df_binary = generate_binary_data(N=size, cr0=cr0, cr1=cr1)
-            df_contingency = data_to_contingency(df_binary)
+            if fast==False:
+                df_binary = generate_binary_data(N=size, cr0=cr0, cr1=cr1)
+                df_contingency = data_to_contingency(df_binary)
+            elif fast==True:
+                df_contingency = generate_contingency(N=size, cr0=cr0, cr1=cr1,exact=False)
+            else:
+                raise Exception("Invalid input for fast parameter.")
             test = BinaryDataTest()
             for group in [0, 1]:
                 nUser = df_contingency.loc[group].users
                 nConverted = df_contingency.loc[group].converted
                 test.add_variant_data_agg(
                     str(group), totals=nUser, positives=nConverted
                 )
```

### Comparing `ab-test-toolkit-0.0.1/ab_test_toolkit.egg-info/PKG-INFO` & `ab-test-toolkit-0.0.2/ab_test_toolkit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ab-test-toolkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolkit to simulate and analyze AB tests
 Home-page: https://github.com/k111git/ab-test-toolkit
 Author: Kolja
-Author-email: kolja.kleineberg@dwins.de
+Author-email: 
 License: Apache Software License 2.0
 Description: ab-test-toolkit
         ================
         
         <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
         
         ## Install
@@ -39,15 +39,15 @@
         ```
         
         ## Binary target (e.g. conversion rate experiments)
         
         ### Sample size:
         
         We can calculate the sample size required with the function
-        “sample_size_chi2”. Input needed is:
+        “sample_size_binary”. Input needed is:
         
         - Conversion rate control: cr0
         
         - Conversion rate variant for minimal detectable effect: cr1 (for
           example, if we have a conversion rate of 1% and want to detect an
           effect of at least 20% relate, we would set cr0=0.010 and cr1=0.012)
         
@@ -77,31 +77,27 @@
             alpha=0.05,
             power=0.8,
             one_sided=True,
         )
         print(f"Required sample size per variant is {int(n_sample)}.")
         ```
         
-            Required sample size per variant is 33560.
-        
         ``` python
         n_sample_two_sided = sample_size_binary(
             cr0=0.01,
             cr1=0.012,
             alpha=0.05,
             power=0.8,
             one_sided=False,
         )
         print(
             f"For the two-sided experiment, required sample size per variant is {int(n_sample_two_sided)}."
         )
         ```
         
-            For the two-sided experiment, required sample size per variant is 42606.
-        
         ### Power simulations
         
         What happens if we use a smaller sample size? And how can we understand
         the sample size?
         
         Let us analyze the statistical power with synthethic data. We can do
         this with the simulate_power_binary function. We are using some default
@@ -138,15 +134,15 @@
         
         Here we assume normally distributed data (which usually holds due to the
         central limit theorem).
         
         ### Sample size
         
         We can calculate the sample size required with the function
-        “continuous_sample_size”. Input needed is:
+        “sample_size_continuous”. Input needed is:
         
         - mu1: Mean of the control group
         
         - mu2: Mean of the variant group assuming minimal detectable effect
           (e.g. if the mean it 5, and we want to detect an effect as small as
           0.05, mu1=5.00 and mu2=5.05)
         
@@ -160,16 +156,14 @@
         ``` python
         n_sample = sample_size_continuous(
             mu1=5.0, mu2=5.05, sigma=1, alpha=0.05, power=0.8, one_sided=True
         )
         print(f"Required sample size per variant is {int(n_sample)}.")
         ```
         
-            Required sample size per variant is 4946.
-        
         Let us also do some simulations. These show results for the t-test as
         well as bayesian testing (only 1-sided).
         
         ``` python
         # simulation = simulate_power_continuous()
         ```
         
@@ -207,15 +201,15 @@
         
         ``` python
         df = generate_binary_data()
         df_contingency = data_to_contingency(df)
         # fig = plot_betas(df_contingency, xmin=0, xmax=0.04)
         ```
         
-Keywords: nbdev jupyter notebook python
+Keywords: python experimentation AB-testing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ab-test-toolkit-0.0.1/settings.ini` & `ab-test-toolkit-0.0.2/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ab-test-toolkit
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ab_test_toolkit
@@ -25,18 +25,18 @@
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
 title = %(lib_name)s
 
 ### PyPI ###
 audience = Developers
 author = Kolja
-author_email = kolja.kleineberg@dwins.de
+author_email = 
 copyright = 2023 onwards, %(author)s
 description = Toolkit to simulate and analyze AB tests
-keywords = nbdev jupyter notebook python
+keywords = python experimentation AB-testing
 language = English
 status = 3
 user = k111git
 
 ### Optional ###
 # requirements = fastcore pandas
 # dev_requirements =
```

### Comparing `ab-test-toolkit-0.0.1/setup.py` & `ab-test-toolkit-0.0.2/setup.py`

 * *Files identical despite different names*

