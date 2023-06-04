# Comparing `tmp/finary_uapi-0.1.2.tar.gz` & `tmp/finary_uapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finary_uapi-0.1.2.tar", max compression
+gzip compressed data, was "finary_uapi-0.1.4.tar", max compression
```

## Comparing `finary_uapi-0.1.2.tar` & `finary_uapi-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     1064 2022-06-23 13:41:14.000000 finary_uapi-0.1.2/LICENSE
--rw-r--r--   0        0        0     5184 2023-05-22 20:32:05.637450 finary_uapi-0.1.2/README.md
--rw-r--r--   0        0        0      692 2023-05-22 21:06:01.990540 finary_uapi-0.1.2/finary_uapi/__init__.py
--rw-r--r--   0        0        0    16618 2023-05-22 20:29:53.501992 finary_uapi-0.1.2/finary_uapi/__main__.py
--rw-r--r--   0        0        0      323 2022-07-05 06:50:29.000000 finary_uapi-0.1.2/finary_uapi/auth.py
--rw-r--r--   0        0        0      694 2022-07-05 08:25:32.000000 finary_uapi-0.1.2/finary_uapi/bank_account_types.py
--rw-r--r--   0        0        0      118 2022-06-10 11:58:16.000000 finary_uapi-0.1.2/finary_uapi/constants.py
--rw-r--r--   0        0        0      241 2022-07-12 18:54:50.000000 finary_uapi-0.1.2/finary_uapi/crypto_chains.py
--rw-r--r--   0        0        0      824 2022-07-05 08:05:25.000000 finary_uapi-0.1.2/finary_uapi/currencies.py
--rw-r--r--   0        0        0      308 2022-07-04 18:16:08.000000 finary_uapi-0.1.2/finary_uapi/generic_asset_categories.py
--rw-r--r--   0        0        0     1310 2022-07-05 06:40:07.000000 finary_uapi-0.1.2/finary_uapi/importers/crypto_generic_csv.py
--rw-r--r--   0        0        0     3244 2022-07-09 16:21:57.000000 finary_uapi-0.1.2/finary_uapi/importers/cryptocom.py
--rw-r--r--   0        0        0     1204 2022-07-05 08:27:58.000000 finary_uapi-0.1.2/finary_uapi/importers/stocks_generic_csv.py
--rw-r--r--   0        0        0      391 2022-07-05 08:06:29.000000 finary_uapi-0.1.2/finary_uapi/institutions.py
--rw-r--r--   0        0        0      511 2022-07-05 08:07:06.000000 finary_uapi-0.1.2/finary_uapi/precious_metals.py
--rw-r--r--   0        0        0      494 2022-07-12 18:15:05.000000 finary_uapi-0.1.2/finary_uapi/scpis.py
--rw-r--r--   0        0        0     3681 2023-05-19 19:32:14.600649 finary_uapi-0.1.2/finary_uapi/securities.py
--rw-r--r--   0        0        0     2308 2022-07-13 19:33:49.000000 finary_uapi-0.1.2/finary_uapi/signin.py
--rw-r--r--   0        0        0     4177 2022-10-05 12:54:35.628064 finary_uapi-0.1.2/finary_uapi/user_cryptos.py
--rw-r--r--   0        0        0      221 2023-04-30 02:01:09.614218 finary_uapi-0.1.2/finary_uapi/user_fonds_euro.py
--rw-r--r--   0        0        0     2024 2022-07-12 13:10:04.000000 finary_uapi-0.1.2/finary_uapi/user_generic_assets.py
--rw-r--r--   0        0        0     3653 2022-10-05 12:54:35.628338 finary_uapi-0.1.2/finary_uapi/user_holdings_accounts.py
--rw-r--r--   0        0        0      411 2022-07-12 18:47:51.000000 finary_uapi-0.1.2/finary_uapi/user_me.py
--rw-r--r--   0        0        0     1998 2023-05-19 19:32:14.591775 finary_uapi-0.1.2/finary_uapi/user_portfolio.py
--rw-r--r--   0        0        0     1865 2022-07-05 08:11:56.000000 finary_uapi-0.1.2/finary_uapi/user_precious_metals.py
--rw-r--r--   0        0        0      222 2022-07-12 13:28:04.000000 finary_uapi-0.1.2/finary_uapi/user_real_estates.py
--rw-r--r--   0        0        0      208 2022-07-12 13:28:04.000000 finary_uapi-0.1.2/finary_uapi/user_scpis.py
--rw-r--r--   0        0        0     7762 2023-05-19 19:37:06.303119 finary_uapi-0.1.2/finary_uapi/user_securities.py
--rw-r--r--   0        0        0      221 2022-07-12 13:28:04.000000 finary_uapi-0.1.2/finary_uapi/user_startups.py
--rw-r--r--   0        0        0      196 2022-07-12 13:02:13.000000 finary_uapi-0.1.2/finary_uapi/utils.py
--rw-r--r--   0        0        0     3387 2023-04-30 01:57:20.675756 finary_uapi-0.1.2/finary_uapi/views.py
--rw-r--r--   0        0        0      474 2023-04-30 01:57:25.478991 finary_uapi-0.1.2/finary_uapi/watches.py
--rw-r--r--   0        0        0      741 2023-05-22 21:05:55.851620 finary_uapi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5796 1970-01-01 00:00:00.000000 finary_uapi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-06-23 13:41:14.000000 finary_uapi-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7038 2023-05-25 09:44:01.972025 finary_uapi-0.1.4/README.md
+-rw-r--r--   0        0        0      347 2023-05-29 21:09:16.214923 finary_uapi-0.1.4/finary_uapi/CONTRIBUTING.md
+-rw-r--r--   0        0        0      692 2023-06-04 14:32:41.293473 finary_uapi-0.1.4/finary_uapi/__init__.py
+-rw-r--r--   0        0        0    17040 2023-06-04 14:34:54.519126 finary_uapi-0.1.4/finary_uapi/__main__.py
+-rw-r--r--   0        0        0      323 2022-07-05 06:50:29.000000 finary_uapi-0.1.4/finary_uapi/auth.py
+-rw-r--r--   0        0        0      694 2023-05-30 13:57:39.113386 finary_uapi-0.1.4/finary_uapi/bank_account_types.py
+-rw-r--r--   0        0        0      118 2022-06-10 11:58:16.000000 finary_uapi-0.1.4/finary_uapi/constants.py
+-rw-r--r--   0        0        0      241 2022-07-12 18:54:50.000000 finary_uapi-0.1.4/finary_uapi/crypto_chains.py
+-rw-r--r--   0        0        0      842 2023-05-29 20:48:13.831985 finary_uapi-0.1.4/finary_uapi/currencies.py
+-rw-r--r--   0        0        0      308 2022-07-04 18:16:08.000000 finary_uapi-0.1.4/finary_uapi/generic_asset_categories.py
+-rw-r--r--   0        0        0     1310 2022-07-05 06:40:07.000000 finary_uapi-0.1.4/finary_uapi/importers/crypto_generic_csv.py
+-rw-r--r--   0        0        0     3244 2022-07-09 16:21:57.000000 finary_uapi-0.1.4/finary_uapi/importers/cryptocom.py
+-rw-r--r--   0        0        0     1204 2022-07-05 08:27:58.000000 finary_uapi-0.1.4/finary_uapi/importers/stocks_generic_csv.py
+-rw-r--r--   0        0        0      391 2022-07-05 08:06:29.000000 finary_uapi-0.1.4/finary_uapi/institutions.py
+-rw-r--r--   0        0        0      511 2022-07-05 08:07:06.000000 finary_uapi-0.1.4/finary_uapi/precious_metals.py
+-rw-r--r--   0        0        0      494 2022-07-12 18:15:05.000000 finary_uapi-0.1.4/finary_uapi/scpis.py
+-rw-r--r--   0        0        0     3706 2023-06-04 14:30:36.205109 finary_uapi-0.1.4/finary_uapi/securities.py
+-rw-r--r--   0        0        0      788 2023-06-04 14:30:36.205492 finary_uapi-0.1.4/finary_uapi/sharing.py
+-rw-r--r--   0        0        0     2308 2022-07-13 19:33:49.000000 finary_uapi-0.1.4/finary_uapi/signin.py
+-rw-r--r--   0        0        0     4177 2023-05-31 16:05:12.647958 finary_uapi-0.1.4/finary_uapi/user_cryptos.py
+-rw-r--r--   0        0        0      221 2023-04-30 02:01:09.614218 finary_uapi-0.1.4/finary_uapi/user_fonds_euro.py
+-rw-r--r--   0        0        0     2024 2022-07-12 13:10:04.000000 finary_uapi-0.1.4/finary_uapi/user_generic_assets.py
+-rw-r--r--   0        0        0     3653 2022-10-05 12:54:35.628338 finary_uapi-0.1.4/finary_uapi/user_holdings_accounts.py
+-rw-r--r--   0        0        0      731 2023-06-04 14:30:36.205910 finary_uapi-0.1.4/finary_uapi/user_me.py
+-rw-r--r--   0        0        0     2198 2023-06-04 14:34:54.519683 finary_uapi-0.1.4/finary_uapi/user_portfolio.py
+-rw-r--r--   0        0        0     1865 2022-07-05 08:11:56.000000 finary_uapi-0.1.4/finary_uapi/user_precious_metals.py
+-rw-r--r--   0        0        0      222 2022-07-12 13:28:04.000000 finary_uapi-0.1.4/finary_uapi/user_real_estates.py
+-rw-r--r--   0        0        0      208 2022-07-12 13:28:04.000000 finary_uapi-0.1.4/finary_uapi/user_scpis.py
+-rw-r--r--   0        0        0     7762 2023-05-19 19:37:06.303119 finary_uapi-0.1.4/finary_uapi/user_securities.py
+-rw-r--r--   0        0        0      221 2022-07-12 13:28:04.000000 finary_uapi-0.1.4/finary_uapi/user_startups.py
+-rw-r--r--   0        0        0      196 2022-07-12 13:02:13.000000 finary_uapi-0.1.4/finary_uapi/utils.py
+-rw-r--r--   0        0        0     3387 2023-04-30 01:57:20.675756 finary_uapi-0.1.4/finary_uapi/views.py
+-rw-r--r--   0        0        0      474 2023-04-30 01:57:25.478991 finary_uapi-0.1.4/finary_uapi/watches.py
+-rw-r--r--   0        0        0      741 2023-06-04 14:32:34.940468 finary_uapi-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7650 1970-01-01 00:00:00.000000 finary_uapi-0.1.4/PKG-INFO
```

### Comparing `finary_uapi-0.1.2/LICENSE` & `finary_uapi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/__init__.py` & `finary_uapi-0.1.4/finary_uapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 account.
 
 This module is maintained by lasconic.
 You can always get the latest version of this module at:
     https://github.com/lasconic/finary-uapi
 """
 
-__version__ = "0.1.2"
+__version__ = "0.1.4"
 __author__ = "lasconic"
 __copyright__ = """
 Copyright (c) 2021-2022, lasconic
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
 granted, provided that the above copyright notice appear in all copies
 and that both that copyright notice and this permission notice appear
```

### Comparing `finary_uapi-0.1.2/finary_uapi/__main__.py` & `finary_uapi-0.1.4/finary_uapi/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     finary_uapi fonds_euro_view [all | 1w | 1m | ytd | 1y]
     finary_uapi fonds_euro
     finary_uapi other_assets [all | 1w | 1m | ytd | 1y]
     finary_uapi saving_accounts [all | 1w | 1m | ytd | 1y]
     finary_uapi real_estates [all | 1w | 1m | ytd | 1y]
     finary_uapi startups
     finary_uapi investments
+    finary_uapi investments dividends
     finary_uapi crowdlendings
     finary_uapi crowdlendings distribution
     finary_uapi cryptos
     finary_uapi cryptos distribution
     finary_uapi cryptos add <code> <quantity> <price> <account_id>
     finary_uapi cryptos update <code> <quantity> <price> <account_id>
     finary_uapi cryptos delete <code> <account_id>
@@ -54,14 +55,16 @@
     finary_uapi scpis search QUERY
     finary_uapi scpis
     finary_uapi watches search QUERY
     finary_uapi import cryptocom FILENAME [(--new=NAME | --edit=account_id | --add=account_id)]
     finary_uapi import crypto_csv FILENAME [(--new=NAME | --edit=account_id | --add=account_id)]
     finary_uapi import stocks_csv FILENAME [(--new=NAME | --edit=account_id | --add=account_id)] [-d]
     finary_uapi import stocks_json FILENAME [(--new=NAME | --edit=account_id | --add=account_id)] [-d]
+    finary_uapi sharing SHARING_CODE_OR_URL [--secret=SECRET_CODE]
+
 
 Options:
   --new=NAME          Create a new account and import the lines
   --edit=account_id   Edit the line with new value if it exists, create it otherwise
   --add=account_id    If line exists, add the quantity and change the price accordingly, create it otherwise
 """
 import json
@@ -82,30 +85,32 @@
     update_holdings_account,
 )
 from .importers.cryptocom import import_cc_csv
 from .importers.crypto_generic_csv import import_crypto_generic_csv
 from .importers.stocks_generic_csv import import_stocks_generic_csv
 from .institutions import get_institutions
 from .user_portfolio import (
-    get_portfolio_cryptos_distribution,
     get_portfolio_investments,
+    get_portfolio_investments_dividends,
     get_portfolio_crowdlendings,
     get_portfolio_crowdlendings_distribution,
+    get_portfolio_cryptos_distribution,
 )
 from .precious_metals import get_precious_metals
 from .user_generic_assets import (
     add_user_generic_asset,
     delete_user_generic_asset,
     get_user_generic_assets,
     update_user_generic_asset,
 )
 from .user_real_estates import get_user_real_estates
 from .user_scpis import get_user_scpis
 from .scpis import get_scpis
 from .securities import get_securities
+from .sharing import get_sharing
 from .signin import signin
 from .user_startups import get_user_startups
 from .user_cryptos import (
     add_user_crypto_by_code,
     delete_user_crypto_by_code,
     get_user_cryptos,
     update_user_crypto_by_code,
@@ -291,15 +296,18 @@
             result = get_crypto_chains(session)
         elif args["cryptos"]:
             if args["distribution"]:
                 result = get_portfolio_cryptos_distribution(session)
             else:
                 result = get_user_cryptos(session)
         elif args["investments"]:
-            result = get_portfolio_investments(session)
+            if args["dividends"]:
+                result = get_portfolio_investments_dividends(session)
+            else:
+                result = get_portfolio_investments(session)
         elif args["holdings_accounts"]:
             if args["<account_name>"]:
                 result = get_holdings_account_per_name_or_id(
                     session, args["<account_name>"]
                 )
             else:
                 holdings_account_types = ["crypto", "stocks"]
@@ -387,14 +395,16 @@
                             edit=True,
                             dry_run=args["-d"],
                         )
                     elif args["--add"]:
                         add_imported_securities_to_account(
                             session, args["--add"], to_be_imported, dry_run=args["-d"]
                         )
+        elif args["sharing"]:
+            result = get_sharing(args["SHARING_CODE_OR_URL"], args["--secret"] or "")
     if result:
         print(json.dumps(result, indent=4))
 
     return 0
 
 
 if __name__ == "__main__":  # pragma: nocover
```

### Comparing `finary_uapi-0.1.2/finary_uapi/bank_account_types.py` & `finary_uapi-0.1.4/finary_uapi/bank_account_types.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/currencies.py` & `finary_uapi-0.1.4/finary_uapi/currencies.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         params["query"] = query
 
     x = session.get(url, params=params)
     logging.debug(json.dumps(x.json(), indent=4))
     return x.json()
 
 
+# utils functions
 def get_cryptocurrency_by_code(session: requests.Session, code: str):
     currencies = get_currencies(session, "crypto", code)
     if len(currencies["result"]) > 0:
         currency = currencies["result"][0]
         for currency in currencies["result"]:
             if currency["code"] == code:
                 return currency
```

### Comparing `finary_uapi-0.1.2/finary_uapi/importers/crypto_generic_csv.py` & `finary_uapi-0.1.4/finary_uapi/importers/crypto_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/importers/cryptocom.py` & `finary_uapi-0.1.4/finary_uapi/importers/cryptocom.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/importers/stocks_generic_csv.py` & `finary_uapi-0.1.4/finary_uapi/importers/stocks_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/securities.py` & `finary_uapi-0.1.4/finary_uapi/securities.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,17 @@
         params["query"] = query
 
     x = session.get(url, params=params)
     if x.status_code in (200, 304):
         logging.debug(json.dumps(x.json(), indent=4))
         result = x.json()
     else:
-        logging.warn(f"Error searching for [{query}]. Status code = [{x.status_code}]")
+        logging.warning(
+            f"Error searching for [{query}]. Status code = [{x.status_code}]"
+        )
         result = {"result": []}
     return result
 
 
 def guess_security(session: requests.Session, security):
     ratio_cut = 45
     result = get_securities(session, security["isin_code"])
```

### Comparing `finary_uapi-0.1.2/finary_uapi/signin.py` & `finary_uapi-0.1.4/finary_uapi/signin.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/user_cryptos.py` & `finary_uapi-0.1.4/finary_uapi/user_cryptos.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/user_generic_assets.py` & `finary_uapi-0.1.4/finary_uapi/user_generic_assets.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/user_holdings_accounts.py` & `finary_uapi-0.1.4/finary_uapi/user_holdings_accounts.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/user_portfolio.py` & `finary_uapi-0.1.4/finary_uapi/user_portfolio.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,7 +62,13 @@
     url = f"{portfolio_api}/{portfolio_type}/distribution"
     params = {}
     if type:
         params["type"] = type
     x = session.get(url, params=params)
     logging.debug(json.dumps(x.json(), indent=4))
     return x.json()
+
+
+def get_portfolio_investments_dividends(session: requests.Session):
+    portfolio_type = "investments"
+    url = f"{portfolio_api}/{portfolio_type}/dividends"
+    return get_and_print(session, url)
```

### Comparing `finary_uapi-0.1.2/finary_uapi/user_precious_metals.py` & `finary_uapi-0.1.4/finary_uapi/user_precious_metals.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/user_securities.py` & `finary_uapi-0.1.4/finary_uapi/user_securities.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/finary_uapi/views.py` & `finary_uapi-0.1.4/finary_uapi/views.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.2/PKG-INFO` & `finary_uapi-0.1.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: finary-uapi
-Version: 0.1.2
-Summary: Finary API client and command line tool to interact with your Finary account.
-License: MIT
-Author: lasconic
-Author-email: lasconic@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: docopt (>=0.6.2,<0.7.0)
-Requires-Dist: fuzzywuzzy[speedup] (>=0.18.0,<0.19.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
-Description-Content-Type: text/markdown
-
 Finary Unofficial API wrapper
 
 A simple command line tool to interact with your Finary account.
 
 Finary is a real time portfolio & stocks tracker. It supports precious metal, cryptos, stocks and a lot more.
 If you don't already have an account, here is a referral link to sign up: https://finary.com/referral/7a49bf74c6d9cb3fca2a
 
@@ -27,15 +10,15 @@
 ## Project goals
 
 * Provide a command line tool to do a large part of what you can do on Finary website
 * Automate some requested features not yet implemented by finary like CSV import/export
 
 ## Quick start 
 
-1. Install requirements. `pip install -r requirements.txt`.
+1. Install requirements. `pip install finary_uapi`.
 2. Copy paste the `credentials.json.tpl` file to `credentials.json` and file your username and password.
 3. Run `python -m finary_uapi signin`
 4. You are good to go and can explore the API. Run `python -m finary_uapi` for available commands.
 5. Try `python -m finary_uapi me` or `python -m finary_uapi investments`. 
 6. If you get errors about being unauthorized, you need to signin again.
 
 ## Usage
@@ -133,7 +116,35 @@
 * Precious metal update
 * Interactive command line (it would make automation less fun, but manual use easier)
 
 ### Remarks for finary devs
 * Delete responses should be normalized, sometimes we get json back sometimes nothing but the 204 HTTP code.
 
 
+
+## Contributors ✨
+
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
+Thanks go to these people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="16.66%"><a href="http://lasconic.com"><img src="https://avatars.githubusercontent.com/u/234271?v=4?s=100" width="100px;" alt="Nicolas Froment"/><br /><sub><b>Nicolas Froment</b></sub></a><br /><a href="#projectManagement-lasconic" title="Project Management">📆</a> <a href="#promotion-lasconic" title="Promotion">📣</a> <a href="https://github.com/lasconic/finary_uapi/commits?author=lasconic" title="Code">💻</a> <a href="https://github.com/lasconic/finary_uapi/issues?q=author%3Alasconic" title="Bug reports">🐛</a> <a href="#ideas-lasconic" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/lasconic/finary_uapi/commits?author=lasconic" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="16.66%"><a href="http://varal7.fr"><img src="https://avatars.githubusercontent.com/u/8019486?v=4?s=100" width="100px;" alt="Victor Quach"/><br /><sub><b>Victor Quach</b></sub></a><br /><a href="https://github.com/lasconic/finary_uapi/commits?author=Varal7" title="Code">💻</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
```

