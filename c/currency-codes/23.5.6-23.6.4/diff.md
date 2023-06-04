# Comparing `tmp/currency_codes-23.5.6.tar.gz` & `tmp/currency_codes-23.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "currency_codes-23.5.6.tar", max compression
+gzip compressed data, was "currency_codes-23.6.4.tar", max compression
```

## Comparing `currency_codes-23.5.6.tar` & `currency_codes-23.6.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-05-06 13:04:34.509440 currency_codes-23.5.6/LICENSE
--rw-r--r--   0        0        0     3609 2023-05-06 13:04:34.509440 currency_codes-23.5.6/README.md
--rw-r--r--   0        0        0      406 2023-05-06 13:04:34.509440 currency_codes-23.5.6/currency_codes/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 13:05:15.662226 currency_codes-23.5.6/currency_codes/assets/__init__.py
--rw-r--r--   0        0        0    10607 2023-05-06 21:04:45.707666 currency_codes-23.5.6/currency_codes/assets/crypto.py
--rw-r--r--   0        0        0    13074 2023-05-06 13:04:34.509440 currency_codes-23.5.6/currency_codes/assets/fiat.py
--rw-r--r--   0        0        0     2770 2023-05-06 13:04:34.509440 currency_codes-23.5.6/currency_codes/assets/other.py
--rw-r--r--   0        0        0      443 2023-05-06 13:04:34.509440 currency_codes-23.5.6/currency_codes/exceptions.py
--rw-r--r--   0        0        0     1748 2023-05-06 13:04:34.513440 currency_codes-23.5.6/currency_codes/main.py
--rw-r--r--   0        0        0      699 2023-05-06 21:04:45.707666 currency_codes-23.5.6/currency_codes/models.py
--rw-r--r--   0        0        0     1027 2023-05-06 21:04:45.711666 currency_codes-23.5.6/pyproject.toml
--rw-r--r--   0        0        0     4370 1970-01-01 00:00:00.000000 currency_codes-23.5.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-04 15:14:41.892839 currency_codes-23.6.4/LICENSE
+-rw-r--r--   0        0        0     3614 2023-06-04 15:24:12.916839 currency_codes-23.6.4/README.md
+-rw-r--r--   0        0        0      406 2023-06-04 15:14:41.892839 currency_codes-23.6.4/currency_codes/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 15:15:22.732839 currency_codes-23.6.4/currency_codes/assets/__init__.py
+-rw-r--r--   0        0        0    10607 2023-06-04 15:14:41.892839 currency_codes-23.6.4/currency_codes/assets/crypto.py
+-rw-r--r--   0        0        0    27472 2023-06-04 15:14:41.892839 currency_codes-23.6.4/currency_codes/assets/fiat.py
+-rw-r--r--   0        0        0     4018 2023-06-04 15:35:42.552839 currency_codes-23.6.4/currency_codes/assets/other.py
+-rw-r--r--   0        0        0      423 2023-06-04 15:14:41.892839 currency_codes-23.6.4/currency_codes/exceptions.py
+-rw-r--r--   0        0        0     1771 2023-06-04 15:14:41.892839 currency_codes-23.6.4/currency_codes/main.py
+-rw-r--r--   0        0        0      699 2023-06-04 15:14:41.892839 currency_codes-23.6.4/currency_codes/models.py
+-rw-r--r--   0        0        0     1178 2023-06-04 15:17:17.724839 currency_codes-23.6.4/pyproject.toml
+-rw-r--r--   0        0        0     4385 1970-01-01 00:00:00.000000 currency_codes-23.6.4/PKG-INFO
```

### Comparing `currency_codes-23.5.6/LICENSE` & `currency_codes-23.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `currency_codes-23.5.6/README.md` & `currency_codes-23.6.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ## Description
 Comprehensive Python package for managing currency codes across different types of assets. Having all the currency codes in one package can simplify the development process for applications that involve multiple currencies and assets. This package could also help to ensure consistency and accuracy in managing currency codes across different parts of an application  
 The package provides currency codes for different types of assets. Such as 
 - fiat (US dollar, UAE Dirham, ...)
-- crypto (Bitcoin, Solana, ...)
-- others (Palladium, Gold, WIR Franc, CFP Franc, ...) 
+- crypto (Bitcoin, Solana, Cardano, ...)
+- others (Palladium, Gold, Unidad Previsional, ...) 
 
 ## Sources
- - [Coinmarketcap website](https://coinmarketcap.com) for crypto
- - [ISO's website](https://www.iso.org/iso-4217-currency-codes.html) for rest
+- [Coinmarketcap website](https://coinmarketcap.com) for crypto
+- [ISO's website](https://www.iso.org/iso-4217-currency-codes.html) for rest
 
 ## Installation
 Install the package with the following command:
 ```shell
 pip install currency_codes
 ```
```

### Comparing `currency_codes-23.5.6/currency_codes/assets/crypto.py` & `currency_codes-23.6.4/currency_codes/assets/crypto.py`

 * *Files identical despite different names*

### Comparing `currency_codes-23.5.6/currency_codes/main.py` & `currency_codes-23.6.4/currency_codes/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 
 def get_currency_by_code(code: str, case_sensitive: bool = False) -> Currency:
     """Provides a currency by a code
 
     Args:
         code (str): country code
-        case_sensitive (bool): determines whether filters will be treated as case-sensitive for a given code
+        case_sensitive (bool): determines whether filters will be treated as a case-sensitive
+            for a given currency code
 
     Returns:
         Currency: a corresponding currency
 
     Raises:
         CurrencyNotFoundError: if there's no corresponding currency
     """
```

### Comparing `currency_codes-23.5.6/currency_codes/models.py` & `currency_codes-23.6.4/currency_codes/models.py`

 * *Files identical despite different names*

### Comparing `currency_codes-23.5.6/pyproject.toml` & `currency_codes-23.6.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 [tool.poetry]
 name = "currency_codes"
-version = "23.05.06"
-description = "All currency codes in one package"
+version = "23.06.04"
+description = "Comprehensive Python package for managing currency codes across different types of assets"
 authors = ["Artem Kuchumov <duketemon@gmail.com>"]
 keywords = ["ISO 4217", "ISO-4217", "Currency Codes", "Currencies", "fiat", "crypto", "commodity"]
 readme = "README.md"
 homepage = "https://github.com/duketemon/currency_codes/blob/main/README.md#description"
 repository = "https://github.com/duketemon/currency_codes"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.7.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 black = "^23.3.0"
 isort = "5.10"
 mypy = "^1.2.0"
+pylint = "^2.17.4"
 
 
 [tool.black]
 line-length = 99
 target-version = ["py311", "py310", "py39", "py38", "py37"]
 
 
 [tool.isort]
 profile = "black"
 
 
+[tool.pylint.'MESSAGES CONTROL']
+disable = ["missing-module-docstring"]
+
+
 [tool.pytest.ini_options]
 testpaths = "tests"
 addopts = [
     "--strict-markers",
     "--verbose",
     "--cov=currency_codes",
     "--cov-branch",
```

### Comparing `currency_codes-23.5.6/PKG-INFO` & `currency_codes-23.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: currency-codes
-Version: 23.5.6
-Summary: All currency codes in one package
+Version: 23.6.4
+Summary: Comprehensive Python package for managing currency codes across different types of assets
 Home-page: https://github.com/duketemon/currency_codes/blob/main/README.md#description
 Keywords: ISO 4217,ISO-4217,Currency Codes,Currencies,fiat,crypto,commodity
 Author: Artem Kuchumov
 Author-email: duketemon@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/duketemon/currency_codes
 Description-Content-Type: text/markdown
 
 ## Description
 Comprehensive Python package for managing currency codes across different types of assets. Having all the currency codes in one package can simplify the development process for applications that involve multiple currencies and assets. This package could also help to ensure consistency and accuracy in managing currency codes across different parts of an application  
 The package provides currency codes for different types of assets. Such as 
 - fiat (US dollar, UAE Dirham, ...)
-- crypto (Bitcoin, Solana, ...)
-- others (Palladium, Gold, WIR Franc, CFP Franc, ...) 
+- crypto (Bitcoin, Solana, Cardano, ...)
+- others (Palladium, Gold, Unidad Previsional, ...) 
 
 ## Sources
- - [Coinmarketcap website](https://coinmarketcap.com) for crypto
- - [ISO's website](https://www.iso.org/iso-4217-currency-codes.html) for rest
+- [Coinmarketcap website](https://coinmarketcap.com) for crypto
+- [ISO's website](https://www.iso.org/iso-4217-currency-codes.html) for rest
 
 ## Installation
 Install the package with the following command:
 ```shell
 pip install currency_codes
 ```
```

