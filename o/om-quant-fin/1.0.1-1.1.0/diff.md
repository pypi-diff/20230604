# Comparing `tmp/om_quant_fin-1.0.1.tar.gz` & `tmp/om_quant_fin-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "om_quant_fin-1.0.1.tar", last modified: Sun May 14 10:34:51 2023, max compression
+gzip compressed data, was "om_quant_fin-1.1.0.tar", last modified: Sun Jun  4 07:18:05 2023, max compression
```

## Comparing `om_quant_fin-1.0.1.tar` & `om_quant_fin-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:34:51.236713 om_quant_fin-1.0.1/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     4121 2023-05-14 10:34:51.236562 om_quant_fin-1.0.1/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)     3479 2023-05-14 10:34:21.000000 om_quant_fin-1.0.1/README.md
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:34:51.235714 om_quant_fin-1.0.1/om_quant_fin/
--rw-r--r--   0 leandroguerra   (501) staff       (20)      241 2023-05-14 10:34:27.000000 om_quant_fin-1.0.1/om_quant_fin/__init__.py
--rw-r--r--   0 leandroguerra   (501) staff       (20)    11873 2023-05-14 10:34:31.000000 om_quant_fin-1.0.1/om_quant_fin/om_quant_fin.py
-drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-05-14 10:34:51.236372 om_quant_fin-1.0.1/om_quant_fin.egg-info/
--rw-r--r--   0 leandroguerra   (501) staff       (20)     4121 2023-05-14 10:34:51.000000 om_quant_fin-1.0.1/om_quant_fin.egg-info/PKG-INFO
--rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-05-14 10:34:51.000000 om_quant_fin-1.0.1/om_quant_fin.egg-info/SOURCES.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-05-14 10:34:51.000000 om_quant_fin-1.0.1/om_quant_fin.egg-info/dependency_links.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       51 2023-05-14 10:34:51.000000 om_quant_fin-1.0.1/om_quant_fin.egg-info/requires.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-05-14 10:34:51.000000 om_quant_fin-1.0.1/om_quant_fin.egg-info/top_level.txt
--rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-05-14 10:34:51.236768 om_quant_fin-1.0.1/setup.cfg
--rw-r--r--   0 leandroguerra   (501) staff       (20)     1181 2023-05-14 10:34:40.000000 om_quant_fin-1.0.1/setup.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-06-04 07:18:05.678492 om_quant_fin-1.1.0/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     4958 2023-06-04 07:18:05.678332 om_quant_fin-1.1.0/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     4233 2023-06-04 07:15:46.000000 om_quant_fin-1.1.0/README.md
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-06-04 07:18:05.677178 om_quant_fin-1.1.0/om_quant_fin/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      396 2023-06-04 07:09:04.000000 om_quant_fin-1.1.0/om_quant_fin/__init__.py
+-rw-r--r--   0 leandroguerra   (501) staff       (20)    19818 2023-06-04 07:15:56.000000 om_quant_fin-1.1.0/om_quant_fin/om_quant_fin.py
+drwxr-xr-x   0 leandroguerra   (501) staff       (20)        0 2023-06-04 07:18:05.678134 om_quant_fin-1.1.0/om_quant_fin.egg-info/
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     4958 2023-06-04 07:18:05.000000 om_quant_fin-1.1.0/om_quant_fin.egg-info/PKG-INFO
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      251 2023-06-04 07:18:05.000000 om_quant_fin-1.1.0/om_quant_fin.egg-info/SOURCES.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)        1 2023-06-04 07:18:05.000000 om_quant_fin-1.1.0/om_quant_fin.egg-info/dependency_links.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)      105 2023-06-04 07:18:05.000000 om_quant_fin-1.1.0/om_quant_fin.egg-info/requires.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       13 2023-06-04 07:18:05.000000 om_quant_fin-1.1.0/om_quant_fin.egg-info/top_level.txt
+-rw-r--r--   0 leandroguerra   (501) staff       (20)       38 2023-06-04 07:18:05.678550 om_quant_fin-1.1.0/setup.cfg
+-rw-r--r--   0 leandroguerra   (501) staff       (20)     1362 2023-06-04 07:09:14.000000 om_quant_fin-1.1.0/setup.py
```

### Comparing `om_quant_fin-1.0.1/PKG-INFO` & `om_quant_fin-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,46 @@
-Metadata-Version: 2.1
-Name: om_quant_fin
-Version: 1.0.1
-Summary: A modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
-Home-page: UNKNOWN
-Author: Outspoken Market
-Author-email: info@outspokenmarket.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-
 # OM Quant Fin
 
-OM Quant Fin is a modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
+The Outspoken Market is training the next quantitative generation. OM Quant Fin is a modern Python package for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
 
 ## Project Structure
 
 ```python
 om_quant_fin/               # Root directory of the project
 ├── om_quant_fin/           # Python package containing the library's code
 │   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
 │   └── om_quant_fin.py     # Contains library's functions
 ├── setup.py                # Provides package metadata and dependencies for packaging and distribution
 ├── .gitignore              # Lists files and folders that should not be tracked by Git
 └── README.md               # Markdown file with a description of the project, usage instructions, and other information
 ```
 
-## What's new in version 1.0.0
+## What's new in version 1.1.0
 
-- OM Quant Fin is now beta!
-- Pain Index - by Dr. Thomas Becker and Aaron Moore of Zephyr Associates
-- Bootstrapping methodology for model robustness evaluation
-- Plot funcions for the Pain Index and Bootstrapping
-- QCutTransformer is a custom transformer class that extends the BaseEstimator and TransformerMixin classes from sklearn.
-    - This is a fit and transform for the qcut method!
-    - This transformer performs quantile-based discretization on the input data.
-    - The constructor function initializes the transformer with the number of quantiles (default is 10)
-    and optional labels for the bins.
-- Removal of the logistic regression model; the package will focus on attributes, indicators and relevant metrics
-    - for modelling please use the very well known Python packages
+- OM Quant Fin now introduces the iFat! The iFat is a fantastic indicator for the measurement of the presence of fat tails. The closest to 0, fatter are the tails. Thin tails otherwise.
+- You also have a new function that create 27 attributes optimizide for the volatility estimation of any give asset. Apply the model methodology of choice into this attributes, evaluate it with the "regression_metrics" method and forecast the volatility with the "prediction_report" method.
 
-## Features
+## OM Quant Fin Features
 
 - Download stock data from Yahoo Finance
-- Calculate rolling Z-scores
-- Calculate rolling ratio of adjusted close and its mean
-- Evaluates the model with AUC and Gini for classification models and respective plots
-- QCut fit method for proper binning in unseen data
+- Calculates rolling Z-scores
+- Calculates the rolling ratio of adjusted close and its mean (RSL indicator)
+- Evaluates a model with AUC and Gini for classification models and respective plots
+- QCut fit method for the proper binning of unseen data
 - Robustness test with bootstrapping
-- Calculate the Pain Index that is a measure of portfolio risk that takes into account both the depth and duration of drawdowns
+- Calculates the Pain Index which is a measure of portfolio risk that takes into account both the depth and duration of drawdowns
+- Calculates the first ACF component for a given time series
+- Z-score function only (no rolling)
+- Z-score based on the median
+- Function to find the next business day given an input date
+- Mean Standard Deviation (MAD) Python implementation
+- iFat: fat tail index calculation
+- Function to create a data frame with 27 attributes for volatility estimation
+- Generates a report with main regression metrics: RMSE and MAE
+- Generates a report with predicted value and actions to take for a given volatility model
 
 ## Installation
 
 Install the library using pip:
 
 ```python
 pip install om_quant_fin
@@ -67,21 +50,21 @@
 
 ```python
 import om_quant_fin as mql
 
 #Download stock data:
   data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
 
-#Calculate rolling Z-score:
+#Calculates rolling Z-score:
   z_score = mql.rolling_z_score(data["Adj Close"], window = 20)
 
-#Calculate rolling ratio:
+#Calculates rolling ratio:
   ratio = mql.rolling_ratio(data["Adj Close"], window = 20)
 
-#Calculate returns:
+#Calculates returns:
   returns = mql.calculate_returns(data["Adj Close"], period = 1)
 
 #Pain index
   window_size = 52 #rolling window for the pain index
   data["Pain_index"] = data["Adj Close"].rolling(window_size).apply(mql.pain_index, raw = True)
   mql.plot_pain_index(ticker1, data.index, data["Adj Close"], data["Pain_index"])
 
@@ -92,13 +75,28 @@
 
 #qcut fit and transformer
 labels = ["bin1", "bin2", "bin3", "bin4", "bin5", "bin6", "bin7", "bin8", "bin9", "bin10"
           ,"bin11", "bin12", "bin13", "bin14", "bin15", "bin16", "bin17", "bin18", "bin19", "bin20"]
 qcut_transformer = mql.QCutTransformer(q = 20, labels = labels)
 qcut_transformer.fit(data["column"])
 qcut_transformer.transform(data["column"])
+
+#Creates a data frame with 27 attributes for volatility estimation
+start_date = = "2015-01-01" 
+end_date = "2023-12-31"
+data = create_vars("^VIX", start_date, end_date, p = 10):
+data.head(5)
+
+#Creates a data frame with 27 attributes for volatility estimation
+start_date = = "2015-01-01" 
+end_date = "2023-12-31"
+data = create_vars("^VIX", start_date, end_date, p = 10):
+data.head(5)
+
+#Calculates the iFat
+ifat, mstd = ifat(data["Returns"], p = 67)
+
 ```
+
 ## License
 
 This project is licensed under the MIT License.
-
-
```

### Comparing `om_quant_fin-1.0.1/README.md` & `om_quant_fin-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,63 @@
+Metadata-Version: 2.1
+Name: om_quant_fin
+Version: 1.1.0
+Summary: The Outspoken Market is training the next quantitative generation. OM Quant Fin is a modern Python package for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
+Home-page: UNKNOWN
+Author: Outspoken Market
+Author-email: info@outspokenmarket.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+
 # OM Quant Fin
 
-OM Quant Fin is a modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
+The Outspoken Market is training the next quantitative generation. OM Quant Fin is a modern Python package for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
 
 ## Project Structure
 
 ```python
 om_quant_fin/               # Root directory of the project
 ├── om_quant_fin/           # Python package containing the library's code
 │   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
 │   └── om_quant_fin.py     # Contains library's functions
 ├── setup.py                # Provides package metadata and dependencies for packaging and distribution
 ├── .gitignore              # Lists files and folders that should not be tracked by Git
 └── README.md               # Markdown file with a description of the project, usage instructions, and other information
 ```
 
-## What's new in version 1.0.0
+## What's new in version 1.1.0
 
-- OM Quant Fin is now beta!
-- Pain Index - by Dr. Thomas Becker and Aaron Moore of Zephyr Associates
-- Bootstrapping methodology for model robustness evaluation
-- Plot funcions for the Pain Index and Bootstrapping
-- QCutTransformer is a custom transformer class that extends the BaseEstimator and TransformerMixin classes from sklearn.
-    - This is a fit and transform for the qcut method!
-    - This transformer performs quantile-based discretization on the input data.
-    - The constructor function initializes the transformer with the number of quantiles (default is 10)
-    and optional labels for the bins.
-- Removal of the logistic regression model; the package will focus on attributes, indicators and relevant metrics
-    - for modelling please use the very well known Python packages
+- OM Quant Fin now introduces the iFat! The iFat is a fantastic indicator for the measurement of the presence of fat tails. The closest to 0, fatter are the tails. Thin tails otherwise.
+- You also have a new function that create 27 attributes optimizide for the volatility estimation of any give asset. Apply the model methodology of choice into this attributes, evaluate it with the "regression_metrics" method and forecast the volatility with the "prediction_report" method.
 
-## Features
+## OM Quant Fin Features
 
 - Download stock data from Yahoo Finance
-- Calculate rolling Z-scores
-- Calculate rolling ratio of adjusted close and its mean
-- Evaluates the model with AUC and Gini for classification models and respective plots
-- QCut fit method for proper binning in unseen data
+- Calculates rolling Z-scores
+- Calculates the rolling ratio of adjusted close and its mean (RSL indicator)
+- Evaluates a model with AUC and Gini for classification models and respective plots
+- QCut fit method for the proper binning of unseen data
 - Robustness test with bootstrapping
-- Calculate the Pain Index that is a measure of portfolio risk that takes into account both the depth and duration of drawdowns
+- Calculates the Pain Index which is a measure of portfolio risk that takes into account both the depth and duration of drawdowns
+- Calculates the first ACF component for a given time series
+- Z-score function only (no rolling)
+- Z-score based on the median
+- Function to find the next business day given an input date
+- Mean Standard Deviation (MAD) Python implementation
+- iFat: fat tail index calculation
+- Function to create a data frame with 27 attributes for volatility estimation
+- Generates a report with main regression metrics: RMSE and MAE
+- Generates a report with predicted value and actions to take for a given volatility model
 
 ## Installation
 
 Install the library using pip:
 
 ```python
 pip install om_quant_fin
@@ -50,21 +67,21 @@
 
 ```python
 import om_quant_fin as mql
 
 #Download stock data:
   data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
 
-#Calculate rolling Z-score:
+#Calculates rolling Z-score:
   z_score = mql.rolling_z_score(data["Adj Close"], window = 20)
 
-#Calculate rolling ratio:
+#Calculates rolling ratio:
   ratio = mql.rolling_ratio(data["Adj Close"], window = 20)
 
-#Calculate returns:
+#Calculates returns:
   returns = mql.calculate_returns(data["Adj Close"], period = 1)
 
 #Pain index
   window_size = 52 #rolling window for the pain index
   data["Pain_index"] = data["Adj Close"].rolling(window_size).apply(mql.pain_index, raw = True)
   mql.plot_pain_index(ticker1, data.index, data["Adj Close"], data["Pain_index"])
 
@@ -75,11 +92,30 @@
 
 #qcut fit and transformer
 labels = ["bin1", "bin2", "bin3", "bin4", "bin5", "bin6", "bin7", "bin8", "bin9", "bin10"
           ,"bin11", "bin12", "bin13", "bin14", "bin15", "bin16", "bin17", "bin18", "bin19", "bin20"]
 qcut_transformer = mql.QCutTransformer(q = 20, labels = labels)
 qcut_transformer.fit(data["column"])
 qcut_transformer.transform(data["column"])
+
+#Creates a data frame with 27 attributes for volatility estimation
+start_date = = "2015-01-01" 
+end_date = "2023-12-31"
+data = create_vars("^VIX", start_date, end_date, p = 10):
+data.head(5)
+
+#Creates a data frame with 27 attributes for volatility estimation
+start_date = = "2015-01-01" 
+end_date = "2023-12-31"
+data = create_vars("^VIX", start_date, end_date, p = 10):
+data.head(5)
+
+#Calculates the iFat
+ifat, mstd = ifat(data["Returns"], p = 67)
+
 ```
+
 ## License
 
 This project is licensed under the MIT License.
+
+
```

### Comparing `om_quant_fin-1.0.1/om_quant_fin.egg-info/PKG-INFO` & `om_quant_fin-1.1.0/om_quant_fin.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: om-quant-fin
-Version: 1.0.1
-Summary: A modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
+Version: 1.1.0
+Summary: The Outspoken Market is training the next quantitative generation. OM Quant Fin is a modern Python package for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
 Home-page: UNKNOWN
 Author: Outspoken Market
 Author-email: info@outspokenmarket.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -13,51 +13,51 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
 # OM Quant Fin
 
-OM Quant Fin is a modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
+The Outspoken Market is training the next quantitative generation. OM Quant Fin is a modern Python package for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.
 
 ## Project Structure
 
 ```python
 om_quant_fin/               # Root directory of the project
 ├── om_quant_fin/           # Python package containing the library's code
 │   ├── __init__.py         # Marks the directory as a package and can contain package-level code or imports
 │   └── om_quant_fin.py     # Contains library's functions
 ├── setup.py                # Provides package metadata and dependencies for packaging and distribution
 ├── .gitignore              # Lists files and folders that should not be tracked by Git
 └── README.md               # Markdown file with a description of the project, usage instructions, and other information
 ```
 
-## What's new in version 1.0.0
+## What's new in version 1.1.0
 
-- OM Quant Fin is now beta!
-- Pain Index - by Dr. Thomas Becker and Aaron Moore of Zephyr Associates
-- Bootstrapping methodology for model robustness evaluation
-- Plot funcions for the Pain Index and Bootstrapping
-- QCutTransformer is a custom transformer class that extends the BaseEstimator and TransformerMixin classes from sklearn.
-    - This is a fit and transform for the qcut method!
-    - This transformer performs quantile-based discretization on the input data.
-    - The constructor function initializes the transformer with the number of quantiles (default is 10)
-    and optional labels for the bins.
-- Removal of the logistic regression model; the package will focus on attributes, indicators and relevant metrics
-    - for modelling please use the very well known Python packages
+- OM Quant Fin now introduces the iFat! The iFat is a fantastic indicator for the measurement of the presence of fat tails. The closest to 0, fatter are the tails. Thin tails otherwise.
+- You also have a new function that create 27 attributes optimizide for the volatility estimation of any give asset. Apply the model methodology of choice into this attributes, evaluate it with the "regression_metrics" method and forecast the volatility with the "prediction_report" method.
 
-## Features
+## OM Quant Fin Features
 
 - Download stock data from Yahoo Finance
-- Calculate rolling Z-scores
-- Calculate rolling ratio of adjusted close and its mean
-- Evaluates the model with AUC and Gini for classification models and respective plots
-- QCut fit method for proper binning in unseen data
+- Calculates rolling Z-scores
+- Calculates the rolling ratio of adjusted close and its mean (RSL indicator)
+- Evaluates a model with AUC and Gini for classification models and respective plots
+- QCut fit method for the proper binning of unseen data
 - Robustness test with bootstrapping
-- Calculate the Pain Index that is a measure of portfolio risk that takes into account both the depth and duration of drawdowns
+- Calculates the Pain Index which is a measure of portfolio risk that takes into account both the depth and duration of drawdowns
+- Calculates the first ACF component for a given time series
+- Z-score function only (no rolling)
+- Z-score based on the median
+- Function to find the next business day given an input date
+- Mean Standard Deviation (MAD) Python implementation
+- iFat: fat tail index calculation
+- Function to create a data frame with 27 attributes for volatility estimation
+- Generates a report with main regression metrics: RMSE and MAE
+- Generates a report with predicted value and actions to take for a given volatility model
 
 ## Installation
 
 Install the library using pip:
 
 ```python
 pip install om_quant_fin
@@ -67,21 +67,21 @@
 
 ```python
 import om_quant_fin as mql
 
 #Download stock data:
   data = mql.download_data("AAPL", "2020-01-01", "2022-12-31")
 
-#Calculate rolling Z-score:
+#Calculates rolling Z-score:
   z_score = mql.rolling_z_score(data["Adj Close"], window = 20)
 
-#Calculate rolling ratio:
+#Calculates rolling ratio:
   ratio = mql.rolling_ratio(data["Adj Close"], window = 20)
 
-#Calculate returns:
+#Calculates returns:
   returns = mql.calculate_returns(data["Adj Close"], period = 1)
 
 #Pain index
   window_size = 52 #rolling window for the pain index
   data["Pain_index"] = data["Adj Close"].rolling(window_size).apply(mql.pain_index, raw = True)
   mql.plot_pain_index(ticker1, data.index, data["Adj Close"], data["Pain_index"])
 
@@ -92,13 +92,30 @@
 
 #qcut fit and transformer
 labels = ["bin1", "bin2", "bin3", "bin4", "bin5", "bin6", "bin7", "bin8", "bin9", "bin10"
           ,"bin11", "bin12", "bin13", "bin14", "bin15", "bin16", "bin17", "bin18", "bin19", "bin20"]
 qcut_transformer = mql.QCutTransformer(q = 20, labels = labels)
 qcut_transformer.fit(data["column"])
 qcut_transformer.transform(data["column"])
+
+#Creates a data frame with 27 attributes for volatility estimation
+start_date = = "2015-01-01" 
+end_date = "2023-12-31"
+data = create_vars("^VIX", start_date, end_date, p = 10):
+data.head(5)
+
+#Creates a data frame with 27 attributes for volatility estimation
+start_date = = "2015-01-01" 
+end_date = "2023-12-31"
+data = create_vars("^VIX", start_date, end_date, p = 10):
+data.head(5)
+
+#Calculates the iFat
+ifat, mstd = ifat(data["Returns"], p = 67)
+
 ```
+
 ## License
 
 This project is licensed under the MIT License.
```

### Comparing `om_quant_fin-1.0.1/setup.py` & `om_quant_fin-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,28 +6,32 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name = "om_quant_fin",
-    version = "1.0.1",
+    version = "1.1.0",
     packages = find_packages(),
     install_requires = [
         "yfinance",
         "pandas",
         "scikit-learn",
         "numpy",
         "time",
         "sys",
-        "plotly"
+        "plotly",
+        "statsmodels.tsa.stattools",
+        "numpy_ext",
+        "warnings",
+        "datetime"
     ],
     author = "Outspoken Market",
     author_email = "info@outspokenmarket.com",
-    description = "A modern Python library for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.",
+    description = "The Outspoken Market is training the next quantitative generation. OM Quant Fin is a modern Python package for quantitative trading analysis. Our mission is to make your quant life easier and more accurate.",
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     classifiers = [
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

