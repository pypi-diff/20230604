# Comparing `tmp/hkfdb-3.3.tar.gz` & `tmp/hkfdb-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.3.tar", last modified: Fri Jun  2 12:32:06 2023, max compression
+gzip compressed data, was "hkfdb-3.4.tar", last modified: Sun Jun  4 18:37:45 2023, max compression
```

## Comparing `hkfdb-3.3.tar` & `hkfdb-3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-02 12:32:06.495645 hkfdb-3.3/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.3/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1618 2023-06-02 12:32:06.495274 hkfdb-3.3/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.3/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-02 12:32:06.493827 hkfdb-3.3/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   106387 2023-06-02 05:18:47.000000 hkfdb-3.3/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.3/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-02 12:32:06.494991 hkfdb-3.3/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1618 2023-06-02 12:32:06.000000 hkfdb-3.3/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-02 12:32:06.000000 hkfdb-3.3/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-02 12:32:06.000000 hkfdb-3.3/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       44 2023-06-02 12:32:06.000000 hkfdb-3.3/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-02 12:32:06.000000 hkfdb-3.3/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-02 12:32:06.495722 hkfdb-3.3/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      761 2023-06-02 12:31:47.000000 hkfdb-3.3/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-04 18:37:45.987755 hkfdb-3.4/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.4/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1618 2023-06-04 18:37:45.987486 hkfdb-3.4/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.4/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-04 18:37:45.986526 hkfdb-3.4/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   106397 2023-06-04 18:34:32.000000 hkfdb-3.4/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.4/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-04 18:37:45.987308 hkfdb-3.4/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1618 2023-06-04 18:37:45.000000 hkfdb-3.4/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-04 18:37:45.000000 hkfdb-3.4/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-04 18:37:45.000000 hkfdb-3.4/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       44 2023-06-04 18:37:45.000000 hkfdb-3.4/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-04 18:37:45.000000 hkfdb-3.4/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-04 18:37:45.987801 hkfdb-3.4/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      761 2023-06-04 18:37:07.000000 hkfdb-3.4/setup.py
```

### Comparing `hkfdb-3.3/LICENSE` & `hkfdb-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.3/PKG-INFO` & `hkfdb-3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.3
+Version: 3.4
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.3/README.md` & `hkfdb-3.4/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.3/hkfdb/Database.py` & `hkfdb-3.4/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
                             df_current = df_single[df_single['current_month'] == current_month].sort_values(
                                 by=['datetime']).reset_index(drop=True)
                             df = df_current.head(1).copy()
 
                             df['open'] = df_current.at[0, 'open']
                             df['high'] = df_current['high'].max()
                             df['low'] = df_current['low'].min()
-                            df['close'] = df_current.at[1, 'close']
+                            df['close'] = df_current.at[len(df) - 1, 'close']
                             df['volume'] = df_current['volume'].sum()
 
                             df_all.append(df.copy())
 
                         dfs.append(pd.concat(df_all))
 
                     df = pd.concat(dfs)
```

### Comparing `hkfdb-3.3/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.4/hkfdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.3
+Version: 3.4
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.3/setup.py` & `hkfdb-3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.3",
+    version="3.4",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

