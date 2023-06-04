# Comparing `tmp/localpdb-0.2.6.tar.gz` & `tmp/localpdb-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localpdb-0.2.6.tar", max compression
+gzip compressed data, was "localpdb-0.2.7.tar", max compression
```

## Comparing `localpdb-0.2.6.tar` & `localpdb-0.2.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1070 2022-12-28 16:48:55.231623 localpdb-0.2.6/LICENSE
--rw-r--r--   0        0        0    21365 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/PDB.py
--rw-r--r--   0        0        0    17442 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/PDBDownloader.py
--rw-r--r--   0        0        0     5131 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/PDBVersioneer.py
--rw-r--r--   0        0        0      103 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/__init__.py
--rw-r--r--   0        0        0    20917 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/localpdb_setup.py
--rw-r--r--   0        0        0     2653 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/Biounit.py
--rw-r--r--   0        0        0     2215 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/DSSP.py
--rw-r--r--   0        0        0     3506 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/ECOD.py
--rw-r--r--   0        0        0     4020 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/MasterChain.py
--rw-r--r--   0        0        0     4570 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/PDBChain.py
--rw-r--r--   0        0        0     4355 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/PDBClustering.py
--rw-r--r--   0        0        0     4704 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/PDBSeqresMapper.py
--rw-r--r--   0        0        0     8224 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/Plugin.py
--rw-r--r--   0        0        0     1344 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/PluginVersioneer.py
--rw-r--r--   0        0        0     5363 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/SIFTS.py
--rw-r--r--   0        0        0    11188 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/Socket.py
--rw-r--r--   0        0        0       47 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/__init__.py
--rw-r--r--   0        0        0      121 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/config/Biounit.yml
--rw-r--r--   0        0        0      158 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/config/DSSP.yml
--rw-r--r--   0        0        0      222 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/config/ECOD.yml
--rw-r--r--   0        0        0      171 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/config/MasterChain.yml
--rw-r--r--   0        0        0      122 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/config/PDBChain.yml
--rw-r--r--   0        0        0      189 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/config/PDBClustering.yml
--rw-r--r--   0        0        0      186 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/config/PDBSeqresMapper.yml
--rw-r--r--   0        0        0      611 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/config/SIFTS.yml
--rw-r--r--   0        0        0      199 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/config/Socket.yml
--rw-r--r--   0        0        0        0 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/config/__init__.py
--rw-r--r--   0        0        0    20277 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/utils/MakeMultimer.py
--rw-r--r--   0        0        0        0 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/plugins/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/__init__.py
--rw-r--r--   0        0        0      842 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/config.py
--rw-r--r--   0        0        0      157 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/errors.py
--rw-r--r--   0        0        0     2125 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/network.py
--rw-r--r--   0        0        0     6222 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/os.py
--rw-r--r--   0        0        0     4064 2022-12-29 14:13:41.236903 localpdb-0.2.6/localpdb/utils/prot.py
--rw-r--r--   0        0        0     1109 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/remote_sources.yml
--rw-r--r--   0        0        0     1102 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/rest_api.py
--rw-r--r--   0        0        0        0 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/search_api/__init__.py
--rw-r--r--   0        0        0     4636 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/search_api/commands.py
--rw-r--r--   0        0        0     1634 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/search_api/parsers.py
--rw-r--r--   0        0        0     1611 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/search_api/queries.py
--rw-r--r--   0        0        0     1108 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/search_api/search.py
--rw-r--r--   0        0        0     2749 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/search_api/services.py
--rw-r--r--   0        0        0        0 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/search_api/tools/__init__.py
--rw-r--r--   0        0        0      794 2022-12-28 16:48:55.239623 localpdb-0.2.6/localpdb/utils/search_api/tools/text_api_input_fetcher.py
--rw-r--r--   0        0        0      692 2022-12-29 14:11:34.045149 localpdb-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1076 2022-12-29 14:18:15.386701 localpdb-0.2.6/setup.py
--rw-r--r--   0        0        0      766 2022-12-29 14:18:15.387046 localpdb-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-09-21 17:23:57.195798 localpdb-0.2.7/LICENSE
+-rw-r--r--   0        0        0    21365 2022-09-21 17:23:57.207797 localpdb-0.2.7/localpdb/PDB.py
+-rw-r--r--   0        0        0    17442 2022-09-22 20:28:58.050794 localpdb-0.2.7/localpdb/PDBDownloader.py
+-rw-r--r--   0        0        0     5131 2022-09-21 17:23:57.207797 localpdb-0.2.7/localpdb/PDBVersioneer.py
+-rw-r--r--   0        0        0      103 2022-09-21 17:23:57.207797 localpdb-0.2.7/localpdb/__init__.py
+-rw-r--r--   0        0        0    20917 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/localpdb_setup.py
+-rw-r--r--   0        0        0     2653 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/Biounit.py
+-rw-r--r--   0        0        0     2215 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/DSSP.py
+-rw-r--r--   0        0        0     3506 2023-06-04 21:00:08.797858 localpdb-0.2.7/localpdb/plugins/ECOD.py
+-rw-r--r--   0        0        0     4020 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/MasterChain.py
+-rw-r--r--   0        0        0     4570 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/PDBChain.py
+-rw-r--r--   0        0        0     4355 2023-06-04 20:56:57.294526 localpdb-0.2.7/localpdb/plugins/PDBClustering.py
+-rw-r--r--   0        0        0     4704 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/PDBSeqresMapper.py
+-rw-r--r--   0        0        0     8224 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/Plugin.py
+-rw-r--r--   0        0        0     1344 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/PluginVersioneer.py
+-rw-r--r--   0        0        0     5363 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/SIFTS.py
+-rw-r--r--   0        0        0    11188 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/Socket.py
+-rw-r--r--   0        0        0       47 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/__init__.py
+-rw-r--r--   0        0        0      121 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/config/Biounit.yml
+-rw-r--r--   0        0        0      158 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/config/DSSP.yml
+-rw-r--r--   0        0        0      222 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/config/ECOD.yml
+-rw-r--r--   0        0        0      171 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/config/MasterChain.yml
+-rw-r--r--   0        0        0      122 2022-09-21 17:23:57.211797 localpdb-0.2.7/localpdb/plugins/config/PDBChain.yml
+-rw-r--r--   0        0        0      189 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/plugins/config/PDBClustering.yml
+-rw-r--r--   0        0        0      186 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/plugins/config/PDBSeqresMapper.yml
+-rw-r--r--   0        0        0      611 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/plugins/config/SIFTS.yml
+-rw-r--r--   0        0        0      199 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/plugins/config/Socket.yml
+-rw-r--r--   0        0        0        0 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/plugins/config/__init__.py
+-rw-r--r--   0        0        0    20277 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/plugins/utils/MakeMultimer.py
+-rw-r--r--   0        0        0        0 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/plugins/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/__init__.py
+-rw-r--r--   0        0        0      842 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/config.py
+-rw-r--r--   0        0        0      157 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/errors.py
+-rw-r--r--   0        0        0     2125 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/network.py
+-rw-r--r--   0        0        0     6222 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/os.py
+-rw-r--r--   0        0        0     4064 2023-06-04 20:56:57.294526 localpdb-0.2.7/localpdb/utils/prot.py
+-rw-r--r--   0        0        0     1109 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/remote_sources.yml
+-rw-r--r--   0        0        0     1102 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/rest_api.py
+-rw-r--r--   0        0        0        0 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/search_api/__init__.py
+-rw-r--r--   0        0        0     4636 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/search_api/commands.py
+-rw-r--r--   0        0        0     1634 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/search_api/parsers.py
+-rw-r--r--   0        0        0     1611 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/search_api/queries.py
+-rw-r--r--   0        0        0     1108 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/search_api/search.py
+-rw-r--r--   0        0        0     2749 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/search_api/services.py
+-rw-r--r--   0        0        0        0 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/search_api/tools/__init__.py
+-rw-r--r--   0        0        0      794 2022-09-21 17:23:57.215797 localpdb-0.2.7/localpdb/utils/search_api/tools/text_api_input_fetcher.py
+-rw-r--r--   0        0        0      692 2023-06-04 21:05:57.020329 localpdb-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1076 2023-06-04 21:09:22.542683 localpdb-0.2.7/setup.py
+-rw-r--r--   0        0        0      766 2023-06-04 21:09:22.542920 localpdb-0.2.7/PKG-INFO
```

### Comparing `localpdb-0.2.6/LICENSE` & `localpdb-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/PDB.py` & `localpdb-0.2.7/localpdb/PDB.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/PDBDownloader.py` & `localpdb-0.2.7/localpdb/PDBDownloader.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/PDBVersioneer.py` & `localpdb-0.2.7/localpdb/PDBVersioneer.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/localpdb_setup.py` & `localpdb-0.2.7/localpdb/localpdb_setup.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/Biounit.py` & `localpdb-0.2.7/localpdb/plugins/Biounit.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/DSSP.py` & `localpdb-0.2.7/localpdb/plugins/DSSP.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/ECOD.py` & `localpdb-0.2.7/localpdb/plugins/ECOD.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def _get_historical_versions(self):
         # Fetch ECOD history
         ecod_content = urllib.request.urlopen(self.plugin_config['ecod_url'])
         soup = BeautifulSoup(ecod_content, "html.parser")
         ecod_history = {}
         for ultag in soup.find('div', class_='history').find_all('ul'):
-            for litag in ultag.find_all('li')[:-1]:
+            for litag in ultag.find_all('li')[:-2]:
                 ver_url = self.plugin_config['ecod_domain'] + litag.find('a')['href']
                 version = int(str(litag.text).split(' ')[0])
                 ecod_history[version] = ver_url # ECOD history dict
         return ecod_history
 
     def _filter_chains(self, chains):
         self.lpdb.ecod = self.lpdb.ecod[self.lpdb.ecod['pdb_chain'].isin(chains)]
```

### Comparing `localpdb-0.2.6/localpdb/plugins/MasterChain.py` & `localpdb-0.2.7/localpdb/plugins/MasterChain.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/PDBChain.py` & `localpdb-0.2.7/localpdb/plugins/PDBChain.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/PDBClustering.py` & `localpdb-0.2.7/localpdb/plugins/PDBClustering.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/PDBSeqresMapper.py` & `localpdb-0.2.7/localpdb/plugins/PDBSeqresMapper.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/Plugin.py` & `localpdb-0.2.7/localpdb/plugins/Plugin.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/PluginVersioneer.py` & `localpdb-0.2.7/localpdb/plugins/PluginVersioneer.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/SIFTS.py` & `localpdb-0.2.7/localpdb/plugins/SIFTS.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/Socket.py` & `localpdb-0.2.7/localpdb/plugins/Socket.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/config/SIFTS.yml` & `localpdb-0.2.7/localpdb/plugins/config/SIFTS.yml`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/plugins/utils/MakeMultimer.py` & `localpdb-0.2.7/localpdb/plugins/utils/MakeMultimer.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/config.py` & `localpdb-0.2.7/localpdb/utils/config.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/network.py` & `localpdb-0.2.7/localpdb/utils/network.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/os.py` & `localpdb-0.2.7/localpdb/utils/os.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/prot.py` & `localpdb-0.2.7/localpdb/utils/prot.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/remote_sources.yml` & `localpdb-0.2.7/localpdb/utils/remote_sources.yml`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/rest_api.py` & `localpdb-0.2.7/localpdb/utils/rest_api.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/search_api/commands.py` & `localpdb-0.2.7/localpdb/utils/search_api/commands.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/search_api/parsers.py` & `localpdb-0.2.7/localpdb/utils/search_api/parsers.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/search_api/queries.py` & `localpdb-0.2.7/localpdb/utils/search_api/queries.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/search_api/search.py` & `localpdb-0.2.7/localpdb/utils/search_api/search.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/search_api/services.py` & `localpdb-0.2.7/localpdb/utils/search_api/services.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/localpdb/utils/search_api/tools/text_api_input_fetcher.py` & `localpdb-0.2.7/localpdb/utils/search_api/tools/text_api_input_fetcher.py`

 * *Files identical despite different names*

### Comparing `localpdb-0.2.6/pyproject.toml` & `localpdb-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "localpdb"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["Jan Ludwiczak <j.ludwiczak@cent.uw.edu.pl>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 pandas = "^1"
```

### Comparing `localpdb-0.2.6/setup.py` & `localpdb-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'tqdm>=4,<5']
 
 entry_points = \
 {'console_scripts': ['localpdb_setup = localpdb.localpdb_setup:main']}
 
 setup_kwargs = {
     'name': 'localpdb',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': '',
     'long_description': None,
     'author': 'Jan Ludwiczak',
     'author_email': 'j.ludwiczak@cent.uw.edu.pl',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `localpdb-0.2.6/PKG-INFO` & `localpdb-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localpdb
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 License: MIT
 Author: Jan Ludwiczak
 Author-email: j.ludwiczak@cent.uw.edu.pl
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

