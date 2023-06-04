# Comparing `tmp/bookio_fetchfox-0.1.0.tar.gz` & `tmp/bookio_fetchfox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-0.1.0.tar", max compression
+gzip compressed data, was "bookio_fetchfox-0.1.1.tar", max compression
```

## Comparing `bookio_fetchfox-0.1.0.tar` & `bookio_fetchfox-0.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     3532 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2140 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      596 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1349 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     1770 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      592 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2664 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/cardano/blockfrostio.py
--rw-r--r--   0        0        0      449 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1056 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/cardano/handleme.py
--rw-r--r--   0        0        0     1570 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/cardano/jpgstore.py
--rw-r--r--   0        0        0        0 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      963 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     4154 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     2573 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      120 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     5670 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      504 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     1430 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0     9675 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0     1061 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0      452 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0     7647 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      619 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0       32 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0      453 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      154 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      158 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      112 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0      296 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0       95 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       28 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      178 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     2359 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     1215 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      463 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1177 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      362 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     1239 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0     1677 2023-06-04 20:09:09.012212 bookio_fetchfox-0.1.0/fetchfox/rest.py
--rw-r--r--   0        0        0     1120 2023-06-04 20:09:09.024212 bookio_fetchfox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4796 1970-01-01 00:00:00.000000 bookio_fetchfox-0.1.0/setup.py
--rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 bookio_fetchfox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3532 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2140 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      596 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1349 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     1770 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      592 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2664 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/cardano/blockfrostio.py
+-rw-r--r--   0        0        0      449 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1056 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/cardano/handleme.py
+-rw-r--r--   0        0        0     1570 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/cardano/jpgstore.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     4154 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     2573 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      120 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     5670 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      504 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     1430 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0     9675 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0     1061 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0      452 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0     7647 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      619 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0       32 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      154 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      112 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0      296 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0       95 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       28 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      178 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     2359 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     1215 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      463 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1177 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      362 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     1239 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0     1677 2023-06-04 20:15:13.927848 bookio_fetchfox-0.1.1/fetchfox/rest.py
+-rw-r--r--   0        0        0     1094 2023-06-04 20:15:13.939849 bookio_fetchfox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 bookio_fetchfox-0.1.1/setup.py
+-rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 bookio_fetchfox-0.1.1/PKG-INFO
```

### Comparing `bookio_fetchfox-0.1.0/README.md` & `bookio_fetchfox-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/cardano/blockfrostio.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/cardano/blockfrostio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/cardano/handleme.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/cardano/handleme.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/evm/moralisio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-0.1.1/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-0.1.1/fetchfox/blockchains/algorand/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/blockchains/base.py` & `bookio_fetchfox-0.1.1/fetchfox/blockchains/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-0.1.1/fetchfox/blockchains/cardano/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-0.1.1/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-0.1.1/fetchfox/blockchains/evm/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-0.1.1/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/dtos/asset.py` & `bookio_fetchfox-0.1.1/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/dtos/campaign.py` & `bookio_fetchfox-0.1.1/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/dtos/listing.py` & `bookio_fetchfox-0.1.1/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/dtos/sale.py` & `bookio_fetchfox-0.1.1/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/fetchfox/rest.py` & `bookio_fetchfox-0.1.1/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-0.1.0/pyproject.toml` & `bookio_fetchfox-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "0.1.0"
+version = "0.1.1"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
-    "Fede <fede@book.com>"
+    "Fede <fede@book.io>"
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -33,17 +33,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 backoff = "^2.2.1"
 asyncio = "^3.4.3"
 aiohttp = "^3.8.4"
 pytz = "^2023.3"
-selenium-wire = "^5.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
-coverage = "^7.2.5"
+coverage = "^7.2.7"
 ddt = "^1.6.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bookio_fetchfox-0.1.0/setup.py` & `bookio_fetchfox-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,23 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0',
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
- 'pytz>=2023.3,<2024.0',
- 'selenium-wire>=5.1.0,<6.0.0']
+ 'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
-    'author_email': 'fede@book.com',
+    'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
```

### Comparing `bookio_fetchfox-0.1.0/PKG-INFO` & `bookio_fetchfox-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
-Author-email: fede@book.com
+Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
-Requires-Dist: selenium-wire (>=5.1.0,<6.0.0)
 Project-URL: Documentation, https://github.com/book-io/fetchfox/blob/main/README.md
 Description-Content-Type: text/markdown
 
 # book.io / fetchfox
 
 > Collection of API services to fetch information from several blockchains.
```

