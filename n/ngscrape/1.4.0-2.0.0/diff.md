# Comparing `tmp/ngscrape-1.4.0.tar.gz` & `tmp/ngscrape-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngscrape-1.4.0.tar", last modified: Wed May 31 23:52:50 2023, max compression
+gzip compressed data, was "ngscrape-2.0.0.tar", last modified: Sun Jun  4 00:43:46 2023, max compression
```

## Comparing `ngscrape-1.4.0.tar` & `ngscrape-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 23:52:50.858787 ngscrape-1.4.0/
--rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.4.0/LICENSE
--rw-rw-rw-   0        0        0    44094 2023-05-31 23:52:50.857785 ngscrape-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-05-31 23:52:20.000000 ngscrape-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     3057 2023-05-31 22:32:29.000000 ngscrape-1.4.0/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-31 23:52:50.859780 ngscrape-1.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 23:52:50.818781 ngscrape-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 23:52:50.827788 ngscrape-1.4.0/src/ngscrape/
--rw-rw-rw-   0        0        0    11163 2023-05-31 23:51:59.000000 ngscrape-1.4.0/src/ngscrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 23:52:50.852781 ngscrape-1.4.0/src/ngscrape.egg-info/
--rw-rw-rw-   0        0        0    44094 2023-05-31 23:52:50.000000 ngscrape-1.4.0/src/ngscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-31 23:52:50.000000 ngscrape-1.4.0/src/ngscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 23:52:50.000000 ngscrape-1.4.0/src/ngscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-31 23:52:50.000000 ngscrape-1.4.0/src/ngscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 23:52:50.000000 ngscrape-1.4.0/src/ngscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 00:43:46.646937 ngscrape-2.0.0/
+-rw-rw-rw-   0        0        0    35184 2023-06-04 00:16:21.000000 ngscrape-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0    44073 2023-06-04 00:43:46.645936 ngscrape-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-06-04 00:32:50.000000 ngscrape-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     3036 2023-06-04 00:32:26.000000 ngscrape-2.0.0/readme.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 00:43:46.646937 ngscrape-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 00:43:46.600712 ngscrape-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 00:43:46.607714 ngscrape-2.0.0/src/ngscrape/
+-rw-rw-rw-   0        0        0    11246 2023-06-04 00:32:25.000000 ngscrape-2.0.0/src/ngscrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 00:43:46.644936 ngscrape-2.0.0/src/ngscrape.egg-info/
+-rw-rw-rw-   0        0        0    44073 2023-06-04 00:43:46.000000 ngscrape-2.0.0/src/ngscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-06-04 00:43:46.000000 ngscrape-2.0.0/src/ngscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 00:43:46.000000 ngscrape-2.0.0/src/ngscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-04 00:43:46.000000 ngscrape-2.0.0/src/ngscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-04 00:43:46.000000 ngscrape-2.0.0/src/ngscrape.egg-info/top_level.txt
```

### Comparing `ngscrape-1.4.0/LICENSE` & `ngscrape-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ngscrape-1.4.0/PKG-INFO` & `ngscrape-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.4.0
+Version: 2.0.0
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,38 +683,38 @@
 
 Functions:
 - `__init__(debug: bool = False) -> None`
     - Start a new NGScrape Instance.
     - Parameters:
         - debug (bool) = False: Enable/Disable debug mode
         - cache (bool) = False: Enable/Disable caching
-- `scrape_game_by_url(url: str, download: str, filename: str) -> None`
+- `scrape_game(url: str, download: str, filename: str) -> None`
     - Scrape a flash game by url.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
         - `download = 'testdir'`
         - `filename = 'game.swf'`
     - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
         - NGScrape: Downloaded swf file to testdir/game.swf
-- `scrape_desc_by_url(self, url: str) -> str`
+- `scrape_desc(self, url: str) -> str`
     - Scrape a flash game's description by url. Returns the description of the game.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
     - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
-- `scrape_card_by_url(self, url: str, download: str, filename: str) -> str`
+- `scrape_card(self, url: str, download: str, filename: str) -> str`
     - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file. The file extention will be automatically determined.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
```

### Comparing `ngscrape-1.4.0/pyproject.toml` & `ngscrape-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ngscrape"
-version = "1.4.0"
+version = "2.0.0"
 description = "Newgrounds flash game scraper powered by bs4 and requests"
 readme = "readme.md"
 authors = [{ name = "aeiea", email = "dpthn@proton.me" }]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
```

### Comparing `ngscrape-1.4.0/readme.md` & `ngscrape-2.0.0/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 
 Functions:
 - `__init__(debug: bool = False) -> None`
     - Start a new NGScrape Instance.
     - Parameters:
         - debug (bool) = False: Enable/Disable debug mode
         - cache (bool) = False: Enable/Disable caching
-- `scrape_game_by_url(url: str, download: str, filename: str) -> None`
+- `scrape_game(url: str, download: str, filename: str) -> None`
     - Scrape a flash game by url.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
         - `download = 'testdir'`
         - `filename = 'game.swf'`
     - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
         - NGScrape: Downloaded swf file to testdir/game.swf
-- `scrape_desc_by_url(self, url: str) -> str`
+- `scrape_desc(self, url: str) -> str`
     - Scrape a flash game's description by url. Returns the description of the game.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
     - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
-- `scrape_card_by_url(self, url: str, download: str, filename: str) -> str`
+- `scrape_card(self, url: str, download: str, filename: str) -> str`
     - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file. The file extention will be automatically determined.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
```

### Comparing `ngscrape-1.4.0/src/ngscrape/__init__.py` & `ngscrape-2.0.0/src/ngscrape/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,38 +11,41 @@
     NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 
     Please star is this was useful!
 
     Functions:
     - `__init__(debug: bool = False) -> None`
         - Start a new NGScrape Instance.
-    - `scrape_game_by_url(url: str, download: str, filename: str) -> None`
+        - Parameters:
+            - debug (bool) = False: Enable/Disable debug mode
+            - cache (bool) = False: Enable/Disable caching
+    - `scrape_game(url: str, download: str, filename: str) -> None`
         - Scrape a flash game by url.
         - Parameters:
             - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
             - download (str): The directory to download the file to.
             - filename (str): The name of the downloaded file.
         - Example parameters:
             - `url = 'https://www.newgrounds.com/portal/view/59593'`
             - `download = 'testdir'`
             - `filename = 'game.swf'`
         - Example output with debug mode:
             - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
             - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
             - NGScrape: Downloaded swf file to testdir/game.swf
-    - `scrape_desc_by_url(self, url: str) -> str`
+    - `scrape_desc(self, url: str) -> str`
         - Scrape a flash game's description by url. Returns the description of the game.
         - Parameters:
             - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - Example parameters:
             - `url = 'https://www.newgrounds.com/portal/view/59593'`
         - Example output with debug mode:
             - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
             - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
-    - `scrape_card_by_url(self, url: str, download: str, filename: str) -> str`
+    - `scrape_card(self, url: str, download: str, filename: str) -> str`
         - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
         - Parameters:
             - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
             - download (str): The directory to download the file to.
             - filename (str): The name of the downloaded file. The file extention will be automatically determined.
         - Example parameters:
             - `url = 'https://www.newgrounds.com/portal/view/59593'`
@@ -61,15 +64,15 @@
             - cache (bool) = False: Enable/Disable caching
         '''
         self.debug = debug
         self.cache = cache
         self.cachedsites = {}
         return
     
-    def scrape_game_by_url(self, url: str, download: str, filename: str) -> None:
+    def scrape_game(self, url: str, download: str, filename: str) -> None:
         '''
         Scrape a flash game by url.
         - Parameters:
             - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
             - download (str): The directory to download the file to.
             - filename (str): The name of the downloaded file.
         - Example parameters:
@@ -108,15 +111,15 @@
             os.mkdir(download)
         except:
             pass
         open(download + '/' + filename, 'wb').write(requests.get(_gameLink.replace('\\', ''), allow_redirects = True).content)
         if self.debug:
             print('NGScrape: Downloaded swf file to ' + download + '/' + filename)
             
-    def scrape_card_by_url(self, url: str, download: str, filename: str) -> str:
+    def scrape_card(self, url: str, download: str, filename: str) -> str:
         '''
         Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
         - Parameters:
             - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
             - download (str): The directory to download the file to.
             - filename (str): The name of the downloaded file. The file extention will be automatically determined.
         - Example parameters:
@@ -157,15 +160,15 @@
         for i in _commonImageFileTypes:
             if i in _gameLink:
                 _imageFiletype = i
         open(download + '/' + filename + _imageFiletype, 'wb').write(requests.get(_gameLink, allow_redirects = True).content)
         if self.debug:
             print('NGScrape: Downloaded swf file to ' + download + '/' + filename + _imageFiletype)
         return filename + _imageFiletype
-    def scrape_desc_by_url(self, url: str) -> str:
+    def scrape_desc(self, url: str) -> str:
         '''
         Scrape a flash game's description by url. Returns the description of the game.
         - Parameters:
             - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - Example parameters:
             - `url = 'https://www.newgrounds.com/portal/view/59593'`
         - Example output with debug mode:
@@ -195,14 +198,14 @@
             except:
                 pass # This is because some tags don't have the property attribute
         
 if __name__ == '__main__':
     import sys
     scraper = Scraper(debug = True)
     try:
-        scraper.scrape_game_by_url(sys.argv[1], sys.argv[2], sys.argv[3])
-        scraper.scrape_card_by_url(sys.argv[1], sys.argv[2], sys.argv[3].replace('.swf', ''))
-        scraper.scrape_desc_by_url(sys.argv[1])
+        scraper.scrape_game(sys.argv[1], sys.argv[2], sys.argv[3])
+        scraper.scrape_card(sys.argv[1], sys.argv[2], sys.argv[3].replace('.swf', ''))
+        scraper.scrape_desc(sys.argv[1])
     except:
         print('ngscrape [newgrounds url, should be formatted like this: https://www.newgrounds.com/portal/view/xxxxx] [directory to save to] [file to save to]')
         exit(1)
     exit(0)
```

### Comparing `ngscrape-1.4.0/src/ngscrape.egg-info/PKG-INFO` & `ngscrape-2.0.0/src/ngscrape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.4.0
+Version: 2.0.0
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,38 +683,38 @@
 
 Functions:
 - `__init__(debug: bool = False) -> None`
     - Start a new NGScrape Instance.
     - Parameters:
         - debug (bool) = False: Enable/Disable debug mode
         - cache (bool) = False: Enable/Disable caching
-- `scrape_game_by_url(url: str, download: str, filename: str) -> None`
+- `scrape_game(url: str, download: str, filename: str) -> None`
     - Scrape a flash game by url.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
         - `download = 'testdir'`
         - `filename = 'game.swf'`
     - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
         - NGScrape: Downloaded swf file to testdir/game.swf
-- `scrape_desc_by_url(self, url: str) -> str`
+- `scrape_desc(self, url: str) -> str`
     - Scrape a flash game's description by url. Returns the description of the game.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
     - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
-- `scrape_card_by_url(self, url: str, download: str, filename: str) -> str`
+- `scrape_card(self, url: str, download: str, filename: str) -> str`
     - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file. The file extention will be automatically determined.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
```

