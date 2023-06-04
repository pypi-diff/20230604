# Comparing `tmp/Blockthon-2.3.6.tar.gz` & `tmp/Blockthon-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Blockthon-2.3.6.tar", last modified: Sun Jun  4 02:17:40 2023, max compression
+gzip compressed data, was "Blockthon-2.4.6.tar", last modified: Sun Jun  4 19:21:50 2023, max compression
```

## Comparing `Blockthon-2.3.6.tar` & `Blockthon-2.4.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 02:17:40.261268 Blockthon-2.3.6/
-drwxrwxrwx   0        0        0        0 2023-06-04 02:17:40.245613 Blockthon-2.3.6/Blockthon/
--rw-rw-rw-   0        0        0     2160 2023-06-02 20:46:04.000000 Blockthon-2.3.6/Blockthon/Base58.py
--rw-rw-rw-   0        0        0     3088 2023-06-03 19:21:06.000000 Blockthon-2.3.6/Blockthon/Bitcoin.py
--rw-rw-rw-   0        0        0     1159 2023-06-03 18:38:02.000000 Blockthon-2.3.6/Blockthon/BitcoinGold.py
--rw-rw-rw-   0        0        0     1041 2023-06-03 18:38:02.000000 Blockthon-2.3.6/Blockthon/Dash.py
--rw-rw-rw-   0        0        0     1032 2023-06-03 18:38:02.000000 Blockthon-2.3.6/Blockthon/DigiByte.py
--rw-rw-rw-   0        0        0      497 2023-06-03 12:50:01.000000 Blockthon-2.3.6/Blockthon/Dogecoin.py
--rw-rw-rw-   0        0        0      492 2023-06-02 23:40:53.000000 Blockthon-2.3.6/Blockthon/Ethereum.py
--rw-rw-rw-   0        0        0     1407 2023-06-03 13:19:05.000000 Blockthon-2.3.6/Blockthon/Litecoin.py
--rw-rw-rw-   0        0        0      859 2023-06-04 00:55:43.000000 Blockthon-2.3.6/Blockthon/Qtum.py
--rw-rw-rw-   0        0        0      847 2023-06-04 00:59:12.000000 Blockthon-2.3.6/Blockthon/Ravencoin.py
--rw-rw-rw-   0        0        0      495 2023-06-02 23:40:53.000000 Blockthon-2.3.6/Blockthon/Tron.py
--rw-rw-rw-   0        0        0    24350 2023-06-04 00:55:43.000000 Blockthon-2.3.6/Blockthon/Utils.py
--rw-rw-rw-   0        0        0     1484 2023-06-04 01:02:25.000000 Blockthon-2.3.6/Blockthon/Wallet.py
--rw-rw-rw-   0        0        0      588 2023-06-04 01:02:25.000000 Blockthon-2.3.6/Blockthon/__init__.py
--rw-rw-rw-   0        0        0      822 2023-06-04 00:29:18.000000 Blockthon-2.3.6/Blockthon/zCash.py
-drwxrwxrwx   0        0        0        0 2023-06-04 02:17:40.261268 Blockthon-2.3.6/Blockthon.egg-info/
--rw-rw-rw-   0        0        0     3514 2023-06-04 02:17:40.000000 Blockthon-2.3.6/Blockthon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2023-06-04 02:17:40.000000 Blockthon-2.3.6/Blockthon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 02:17:40.000000 Blockthon-2.3.6/Blockthon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2023-06-04 02:17:40.000000 Blockthon-2.3.6/Blockthon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 02:17:40.000000 Blockthon-2.3.6/Blockthon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3514 2023-06-04 02:17:40.261268 Blockthon-2.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     2674 2023-06-04 01:48:32.000000 Blockthon-2.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-04 02:17:40.261268 Blockthon-2.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1477 2023-06-04 02:00:50.000000 Blockthon-2.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:21:50.726609 Blockthon-2.4.6/
+drwxrwxrwx   0        0        0        0 2023-06-04 19:21:50.704579 Blockthon-2.4.6/Blockthon/
+-rw-rw-rw-   0        0        0     2160 2023-06-02 20:46:04.000000 Blockthon-2.4.6/Blockthon/Base58.py
+-rw-rw-rw-   0        0        0     3705 2023-06-04 19:05:17.000000 Blockthon-2.4.6/Blockthon/Bitcoin.py
+-rw-rw-rw-   0        0        0     1159 2023-06-03 18:38:02.000000 Blockthon-2.4.6/Blockthon/BitcoinGold.py
+-rw-rw-rw-   0        0        0     1041 2023-06-03 18:38:02.000000 Blockthon-2.4.6/Blockthon/Dash.py
+-rw-rw-rw-   0        0        0     1032 2023-06-03 18:38:02.000000 Blockthon-2.4.6/Blockthon/DigiByte.py
+-rw-rw-rw-   0        0        0      497 2023-06-03 12:50:01.000000 Blockthon-2.4.6/Blockthon/Dogecoin.py
+-rw-rw-rw-   0        0        0      492 2023-06-02 23:40:53.000000 Blockthon-2.4.6/Blockthon/Ethereum.py
+-rw-rw-rw-   0        0        0     1407 2023-06-03 13:19:05.000000 Blockthon-2.4.6/Blockthon/Litecoin.py
+-rw-rw-rw-   0        0        0      859 2023-06-04 00:55:43.000000 Blockthon-2.4.6/Blockthon/Qtum.py
+-rw-rw-rw-   0        0        0      847 2023-06-04 00:59:12.000000 Blockthon-2.4.6/Blockthon/Ravencoin.py
+-rw-rw-rw-   0        0        0      495 2023-06-02 23:40:53.000000 Blockthon-2.4.6/Blockthon/Tron.py
+-rw-rw-rw-   0        0        0    24954 2023-06-04 19:05:17.000000 Blockthon-2.4.6/Blockthon/Utils.py
+-rw-rw-rw-   0        0        0     1497 2023-06-04 15:50:24.000000 Blockthon-2.4.6/Blockthon/Wallet.py
+-rw-rw-rw-   0        0        0      588 2023-06-04 01:02:25.000000 Blockthon-2.4.6/Blockthon/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-06-04 00:29:18.000000 Blockthon-2.4.6/Blockthon/zCash.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:21:50.726609 Blockthon-2.4.6/Blockthon.egg-info/
+-rw-rw-rw-   0        0        0     3514 2023-06-04 19:21:50.000000 Blockthon-2.4.6/Blockthon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2023-06-04 19:21:50.000000 Blockthon-2.4.6/Blockthon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 19:21:50.000000 Blockthon-2.4.6/Blockthon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      166 2023-06-04 19:21:50.000000 Blockthon-2.4.6/Blockthon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 19:21:50.000000 Blockthon-2.4.6/Blockthon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3514 2023-06-04 19:21:50.726609 Blockthon-2.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2674 2023-06-04 19:14:44.000000 Blockthon-2.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 19:21:50.726609 Blockthon-2.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1477 2023-06-04 19:16:06.000000 Blockthon-2.4.6/setup.py
```

### Comparing `Blockthon-2.3.6/Blockthon/Base58.py` & `Blockthon-2.4.6/Blockthon/Base58.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.3.6/Blockthon/Bitcoin.py` & `Blockthon-2.4.6/Blockthon/Bitcoin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 from .Utils import (
+    Wif_To_DEC,
+    Wif_To_Addr,
+    Wif_To_HEX,
+    Mnemonic_To_Bytes,
+    Bytes_To_PrivateKey as Bytes_To_HEX,
     PrivateKey_To_Addr,
     PrivateKey_To_Mnemonics,
     PrivateKey_From_Passphrase as Word_To_Hex,
     PrivateKey_From_Dec,
     Btc_Balance,
     BTC,
     Wallet_,
@@ -74,9 +79,28 @@
 def PrivateKey_To_Mnemonic(privatekey): return PrivateKey_To_Mnemonics(privatekey)
 
 
 # convert Private Key HEX To Word Character and Return word string
 def PrivateKey_From_Passphrase(passphrase): return Word_To_Hex(passphrase)
 
 
+def Mnemonic_To_PrivateKey(mnemonicWords):
+    """
+    convert mnemonic to private key hex
+    @param mnemonicWords: string
+    @return: privatekey [string]
+    """
+    byte_string = Mnemonic_To_Bytes(mnemonicWords)
+    return Bytes_To_PrivateKey(byte_string)
+
+
+def Bytes_To_PrivateKey(byteString): return Bytes_To_HEX(byteString)
+
+
+def Wif_To_PrivateKey(wif): return Wif_To_HEX(wif)
+
+def Wif_To_Dec(wif): return Wif_To_DEC(wif)
+
+def Wif_To_Address(wif): return Wif_To_Addr(wif)
+
 # Send Request For Per Address Balance and Return Value Balance [string]
 def Balance_BTC(address): return Btc_Balance(address)
```

### Comparing `Blockthon-2.3.6/Blockthon/BitcoinGold.py` & `Blockthon-2.4.6/Blockthon/BitcoinGold.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.3.6/Blockthon/Dash.py` & `Blockthon-2.4.6/Blockthon/Dash.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.3.6/Blockthon/DigiByte.py` & `Blockthon-2.4.6/Blockthon/DigiByte.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.3.6/Blockthon/Litecoin.py` & `Blockthon-2.4.6/Blockthon/Litecoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.3.6/Blockthon/Qtum.py` & `Blockthon-2.4.6/Blockthon/Qtum.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.3.6/Blockthon/Ravencoin.py` & `Blockthon-2.4.6/Blockthon/Ravencoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.3.6/Blockthon/Utils.py` & `Blockthon-2.4.6/Blockthon/Utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,27 @@
     sha256_2_nbpk = _SHA256(Hash256N_digest)
     sha256_2_nbpk_digest = sha256_2_nbpk.digest()
     sha256_2_hex = codecs.encode(sha256_2_nbpk_digest, 'hex')
     checksum = sha256_2_hex[:8]
     addrHex = (NetBTCBytePubKey + checksum).decode('utf-8')
     return Base58_(addrHex)
 
+# =========================================================
+
+def getBin(size=256):
+    """ Generated Random Binary : return [str]
+    :param size:
+    :type size: int
+    :return: str
+    """
+    bs_ = ''
+    for _ in range(size):
+        bs_ += random.choice(['0', '1'])
+    return bs_
+
 
 # ==========================================================
 
 def getMnemonic(size=12):
     """
 Generate random mnemonic (word's) with size . size default= 12
     @param size: [integer]
@@ -234,14 +247,29 @@
 
 def Bytes_To_PublicKey(bytestring, compress=False):
     if compress:
         return PrivateKey_To_PublicKey(Bytes_To_PrivateKey(bytestring), True)
     else:
         return PrivateKey_To_PublicKey(Bytes_To_PrivateKey(bytestring))
 
+# -------------------------------------------------------------------------------
+
+def Wif_To_Addr(wif):
+    btc = Wallet(wif)
+    return btc.address
+
+
+def Wif_To_HEX(wif):
+    btc = Wallet(wif)
+    return btc.to_hex()
+
+def Wif_To_DEC(wif):
+    btc = Wallet(wif)
+    return btc.to_int()
+
 # --------------------------------------------------------------------------------
 # Check Value Bitcoin Address Balance Return [str]
 def Btc_Balance(addr):
     req = requests.get(f"https://bitcoin.atomicwallet.io/api/v2/address/{addr}").json()
     return dict(req)['balance']
 
 # --------------------------------------------------------------------------------
```

### Comparing `Blockthon-2.3.6/Blockthon/Wallet.py` & `Blockthon-2.4.6/Blockthon/Wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     PrivateKey_From_Passphrase,
     PrivateKey_From_RootKey,
     PrivateKey_From_Binary,
     PrivateKey_From_Dec,
     PrivateKey,
     getMnemonic,
     getBytes,
+    getBin,
     Mnemonic_To_Bytes,
     Mnemonic_To_RootKey,
     Bytes_To_PrivateKey,
     Bytes_To_PublicKey,
     Bytes_To_Mnemonic,
     Bytes_To_Wif
 )
```

### Comparing `Blockthon-2.3.6/Blockthon/__init__.py` & `Blockthon-2.4.6/Blockthon/__init__.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.3.6/Blockthon/zCash.py` & `Blockthon-2.4.6/Blockthon/zCash.py`

 * *Files identical despite different names*

### Comparing `Blockthon-2.3.6/Blockthon.egg-info/PKG-INFO` & `Blockthon-2.4.6/Blockthon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Blockthon
-Version: 2.3.6
+Version: 2.4.6
 Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
 Home-page: https://github.com/Blockthon/Blockthon
 Author: Pymmdrza
 Author-email: Pymmdrza@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://mmdrza.gitbook.io/blockthon/
 Project-URL: Personal Website, https://mmdrza.com
```

### Comparing `Blockthon-2.3.6/PKG-INFO` & `Blockthon-2.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Blockthon
-Version: 2.3.6
+Version: 2.4.6
 Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
 Home-page: https://github.com/Blockthon/Blockthon
 Author: Pymmdrza
 Author-email: Pymmdrza@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://mmdrza.gitbook.io/blockthon/
 Project-URL: Personal Website, https://mmdrza.com
```

### Comparing `Blockthon-2.3.6/README.md` & `Blockthon-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `Blockthon-2.3.6/setup.py` & `Blockthon-2.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Blockthon",
-    version="2.3.6",
+    version="2.4.6",
     author="Pymmdrza",
     author_email="Pymmdrza@gmail.com",
     description="Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.",
     keywords=['blockthon','bitcoin', 'ethereum', 'tron', 'dogecoin', 'dash', 'qtum', 'litecoin', 'bitcoingold', 'wallet', 'private key', 'mnemonic', 'seed', 'binary', 'hex', 'hunter', 'compress', 'un compress', 'compress address', 'un compress address'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Blockthon/Blockthon",
```

