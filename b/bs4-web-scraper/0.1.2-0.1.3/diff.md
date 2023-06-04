# Comparing `tmp/bs4_web_scraper-0.1.2.tar.gz` & `tmp/bs4_web_scraper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs4_web_scraper-0.1.2.tar", last modified: Sun May 28 18:50:27 2023, max compression
+gzip compressed data, was "bs4_web_scraper-0.1.3.tar", last modified: Sun Jun  4 14:34:29 2023, max compression
```

## Comparing `bs4_web_scraper-0.1.2.tar` & `bs4_web_scraper-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 18:50:27.829218 bs4_web_scraper-0.1.2/
--rw-rw-rw-   0        0        0     1104 2023-03-07 14:14:59.000000 bs4_web_scraper-0.1.2/LICENSE.md
--rw-rw-rw-   0        0        0    19798 2023-05-28 18:50:27.829218 bs4_web_scraper-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    18458 2023-05-28 18:46:31.000000 bs4_web_scraper-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 18:50:27.644941 bs4_web_scraper-0.1.2/bs4_web_scraper/
--rw-rw-rw-   0        0        0     3635 2023-05-28 18:48:55.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/__init__.py
--rw-rw-rw-   0        0        0    41852 2023-05-28 18:29:56.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/base.py
--rw-rw-rw-   0        0        0     2102 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/exceptions.py
--rw-rw-rw-   0        0        0    12777 2023-05-23 09:26:13.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/file_handler.py
--rw-rw-rw-   0        0        0     5642 2023-05-27 10:03:10.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/logging.py
--rw-rw-rw-   0        0        0     4858 2023-05-27 19:09:12.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/request_limiter.py
--rw-rw-rw-   0        0        0    39596 2023-05-28 18:47:14.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/scraper.py
--rw-rw-rw-   0        0        0    22737 2023-05-27 12:41:04.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/translate.py
--rw-rw-rw-   0        0        0     3906 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.2/bs4_web_scraper/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 18:50:27.821211 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/
--rw-rw-rw-   0        0        0    19798 2023-05-28 18:50:27.000000 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-05-28 18:50:27.000000 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 18:50:27.000000 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2023-05-28 18:50:27.000000 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 18:50:27.000000 bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1731 2023-05-28 18:49:10.000000 bs4_web_scraper-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 18:50:27.829218 bs4_web_scraper-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 14:34:29.141370 bs4_web_scraper-0.1.3/
+-rw-rw-rw-   0        0        0     1104 2023-03-07 14:14:59.000000 bs4_web_scraper-0.1.3/LICENSE.md
+-rw-rw-rw-   0        0        0    19798 2023-06-04 14:34:29.141370 bs4_web_scraper-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    18458 2023-05-28 18:46:31.000000 bs4_web_scraper-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 14:34:29.013367 bs4_web_scraper-0.1.3/bs4_web_scraper/
+-rw-rw-rw-   0        0        0     3635 2023-05-28 18:48:55.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/__init__.py
+-rw-rw-rw-   0        0        0    44567 2023-05-31 20:43:03.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/base.py
+-rw-rw-rw-   0        0        0     2102 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/exceptions.py
+-rw-rw-rw-   0        0        0    13603 2023-06-04 13:45:20.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/file_handler.py
+-rw-rw-rw-   0        0        0     5642 2023-05-27 10:03:10.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/logger.py
+-rw-rw-rw-   0        0        0     4864 2023-06-01 03:31:13.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/request_limiter.py
+-rw-rw-rw-   0        0        0    44240 2023-06-02 17:56:05.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/scraper.py
+-rw-rw-rw-   0        0        0    23599 2023-06-04 14:12:14.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/translate.py
+-rw-rw-rw-   0        0        0     3906 2023-03-29 00:08:41.000000 bs4_web_scraper-0.1.3/bs4_web_scraper/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:34:29.109377 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/
+-rw-rw-rw-   0        0        0    19798 2023-06-04 14:34:28.000000 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-06-04 14:34:28.000000 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:34:28.000000 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-06-04 14:34:28.000000 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-04 14:34:28.000000 bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1731 2023-06-04 14:32:54.000000 bs4_web_scraper-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 14:34:29.149369 bs4_web_scraper-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 14:34:29.141370 bs4_web_scraper-0.1.3/tests/
+-rw-rw-rw-   0        0        0    10390 2023-06-03 23:28:03.000000 bs4_web_scraper-0.1.3/tests/test_base.py
+-rw-rw-rw-   0        0        0     9022 2023-06-04 11:38:04.000000 bs4_web_scraper-0.1.3/tests/test_file_handler.py
+-rw-rw-rw-   0        0        0     9088 2023-06-02 18:09:58.000000 bs4_web_scraper-0.1.3/tests/test_scraper.py
+-rw-rw-rw-   0        0        0     3938 2023-06-04 14:15:02.000000 bs4_web_scraper-0.1.3/tests/test_translate.py
```

### Comparing `bs4_web_scraper-0.1.2/LICENSE.md` & `bs4_web_scraper-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.2/PKG-INFO` & `bs4_web_scraper-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs4_web_scraper
-Version: 0.1.2
+Version: 0.1.3
 Summary: A web scraper based on the BeautifulSoup4 library and translators package.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/bs4_web_scraper
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/bs4_web_scraper/issues
 Project-URL: Repository, https://github.com/ti-oluwa/bs4_web_scraper
 Keywords: web scraper,bs4,beautifulsoup4,web scraping,web scraping with python,web scraping with bs4,web scraping with beautifulsoup4,web scraping with translation,web scraping with translation to other languages,web scraping with translation to other languages with python,web scraping with translation to other languages with bs4,web scraping with translation to other languages with beautifulsoup4,web scraping with translation to other languages with python and bs4,web scraping with translation to other languages with python and beautifulsoup4
```

### Comparing `bs4_web_scraper-0.1.2/README.md` & `bs4_web_scraper-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.2/bs4_web_scraper/__init__.py` & `bs4_web_scraper-0.1.3/bs4_web_scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.2/bs4_web_scraper/base.py` & `bs4_web_scraper-0.1.3/bs4_web_scraper/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 DESCRIPTION: ::
     This module contains the BS4BaseScraper class which is the base class for creating scraper subclasses.
 """
 
-from os.path import isabs
 from typing import IO, Any, Dict, List
 import requests
 import os
 import random
 import time
 import json
 import math
@@ -15,15 +14,15 @@
 from bs4.element import Tag
 from urllib3.util.url import parse_url, Url
 from urllib.parse import urljoin
 from concurrent.futures import ThreadPoolExecutor
 
 from . import utils
 from . import translate
-from .logging import Logger
+from .logger import Logger
 from .exceptions import (InvalidURLError, UnsupportedLanguageError, FileError, InvalidScrapableTagError)
 from .request_limiter import RequestLimitSetting
 from .file_handler import FileHandler
 
 
 class BS4BaseScraper:
     """
@@ -193,14 +192,51 @@
             if __value < 1:
                 raise ValueError(f"`{__name}` cannot be less than 1")
             if __value > 10:
                 raise ValueError(f"`{__name}` cannot be greater than 10")
         return super().__setattr__(__name, __value)
 
 
+    def __exit__(self, exc_type, exc_value, traceback):
+        return self.reset()
+
+
+    def reset(self):
+        """
+        Resets the web scraper instance to its initial state.
+
+        Resets the following attributes to their initial values:
+        `_auth_credentials`, `_auth_url`, `_base_url`, `_is_authenticated`, `_level_reached`, `
+        _max_no_of_threads`, `url_query_params`, `translator`, `translate_to`, `logger`, `_scrapable_tags`.
+
+        Clears/closes the previous `session` object, reassigns a `requests.Session` instance and closes all file handlers.
+        """
+        self._auth_credentials = None
+        self._auth_url = None
+        self._base_url = None
+        self._is_authenticated = False
+        self._level_reached = 0
+        self._max_no_of_threads = 10
+        self.url_query_params = {}
+        self.translator = None
+        self.translate_to = None
+        self.logger = None
+        self._scrapable_tags = (
+            'script', 'link|{"rel": "stylesheet"}', 'img', 'use', 'audio',
+            'video', 'link|{"as": "font"}', 'link|{"rel": "shortcut"}', 'link|{"rel": "icon"}',
+            'link|{"rel": "shortcut icon"}', 'link|{"rel": "apple-touch-icon"}',
+            'link|{"type": "image/x-icon"}', 'link|{"type": "image/png"}',
+            'link|{"type": "image/jpg"}', 'link|{"type": "image/jpeg"}',
+            'link|{"type": "image/svg"}', 'link|{"type": "image/webp"}',
+            'meta|{"content": "og:image"}',
+        )
+        self._tc_ = []
+        self.close_session()
+        return self.renew_session()
+
     def log(self, msg: str, level: str | None = None) -> None:
         """
         Logs a message using `self.logger` or prints it out if `self.logger` is None.
 
         Args:
             msg (str): The message to log
             level (str | None): The level of message to log.
@@ -209,14 +245,26 @@
             level = level if level else 'INFO'
             return self.logger.log(msg, level)
         elif self.logger and not isinstance(self.logger, Logger):
             raise TypeError('Invalid type for `self.logger`. `self.logger` should be an instance of bs4_web_scraper.logging.Logger')
         return print(msg + '\n')
 
 
+    def close_session(self):
+        """Closes the session assigned to `self._session` (usually re-assigning a new session after) clearing all cookies in the process."""
+        if self._session:
+            self._session.cookies.clear()
+            return self._session.close()
+
+
+    def renew_session(self):
+        """Reassigns a new session to `self._session`"""
+        self._session = requests.Session()
+
+
     def get_base_url(self, url: str) -> str:
         '''
         Returns a base url containing only the host, scheme and port
 
         Args:
             url (str): The url to be parsed. The url should be of the format `http://www.example.com:80/path/to/resource?query=string`,
             The base url will be `http://www.example.com:80`.
@@ -322,15 +370,15 @@
         Returns a soup.
 
         Args::
             * markup (str | bytes | IO ): string, readable bytes or file containing markup.
         """
         if isinstance(markup, IO) and not markup.readable():
             raise FileError("file object provided for `markup` does not support read")
-                
+               
         return BeautifulSoup(markup, self.parser, **kwargs)
 
     
     def make_soup_from_url(self, url: str, **kwargs: Any):
         """
         Similar to `make_soup` but a url can be provided instead of markup. 
         The function will get the url's markup and make a BeautifulSoup with it.
@@ -376,15 +424,15 @@
         if translate_to:
             if not self.translator:
                 self.set_translator(translation_engine)
             self.log(f"TRANSLATION ENGINE: {self.translator.translation_engine.upper()}\n")
             self.translate_to = translate_to
 
         if self.level_reached == 0:
-            self._base_url = self.get_base_url(url)
+            self.set_base_url(url)
         if credentials:
             self.set_auth_credentials(credentials)   
 
         # Scraping 'n' levels (for n >= 0)
         # Initially, Scrape base level -> 'n = 0'
         self.log(f'~~~SCRAPING BASE LEVEL~~~\n')
         self.log('GETTING --> %s \n' % url)
@@ -393,15 +441,15 @@
             index_file_hdl = self.save_to_file(self.markup_filename, self.storage_path, content=response.content)
         else:
             raise Exception('Unexpected response: %s' % response)
 
         soup = self.get_associated_files_and_return_soup(index_file_hdl)
         self.save_to_file(self.markup_filename, self.storage_path, content=soup.prettify(encoding='utf-8'), translate=False)
 
-        while scrape_depth > 0:
+        while True and scrape_depth > 0:
             # Start scraping at level 'n = n + 1'
             link_tags = soup.find_all('a') # get all links on the page
             self.log(f'~~~SCRAPING AT LEVEL {self.level_reached + 1}~~~\n')
             with ThreadPoolExecutor() as executor:
                 no_of_threads = self._get_suitable_no_threads(len(link_tags))
                 for link_tags_sub_list in utils.slice_iterable(link_tags, no_of_threads):
                     results = executor.map(lambda link_tag: self.get_link_tag(link_tag, True), link_tags_sub_list)
@@ -414,14 +462,15 @@
         
             # If `scrape_depth` is still greater than zero, prepare data for scraping next level
             if scrape_depth > 0:
                 results = filter(lambda result: isinstance(result, FileHandler) and all(result), results)
                 for markup_file_hdl in results:
                     markup_file_hdl.open_file('r')
                     soup = self.make_soup(markup_file_hdl.file)
+                    markup_file_hdl.close_file()
                     self.storage_path = markup_file_hdl.filepath
                     self.markup_filename = markup_file_hdl.filename
             continue
         return None
 
 
     def scrape(self, url: str, scrape_depth: int = 0, credentials: Dict[str, str] | None=None, translate_to: str = None) -> None:
@@ -439,14 +488,16 @@
         is automatically detected by `self.translator`. Defaults to None.
         """
         raise NotImplementedError("Oops! You forgot to implement this method. Your method should pass the required arguments to the `_scrape` method.")
 
 
     def get_request_headers(self) -> dict:
         '''Returns a suitable request header'''
+        if not self.base_url:
+            raise AttributeError('Attribute `base_url` not set.')
         if self.auth_credentials:
             if not self._request_user_agent:
                 user_agents = utils.generate_random_user_agents()
                 random.shuffle(user_agents)
                 self._request_user_agent = random.choice(user_agents)
         else:
             user_agents = utils.generate_random_user_agents()
@@ -462,14 +513,15 @@
             'referer': self.base_url,
             'User-Agent': self._request_user_agent,
             "Dnt": "1",
             "Sec-Fetch-Dest": "document", 
             "Sec-Fetch-Mode": "navigate",
             "Sec-Fetch-Site": "none", 
             "Sec-Fetch-User": "?1", 
+            "Keep-Alive": "True",
         }
         return headers
 
 
     def authenticate(self, credentials: Dict[str, str] | None = None) -> None:
         '''
         Authenticates the scraper to scrape websites that require authentication.
@@ -492,25 +544,26 @@
 
         if self.is_authenticated:
             self.log('AUTHENTICATED!!!\n')
         else:
             self.log('AUTHENTICATION FAILED!!!\n', level='ERROR')
 
 
-    def get(self, url: str) -> requests.Response | None:  
+    def get(self, url: str,):  
         '''
         Makes a GET request to url given, authenticates requests and limits request rate based on limit setting if provided. 
         
         Returns response if status code is OK. Returns None if request is stale(failed even after multiple retries)
 
         Args:
         * `url` (str): url to make request to.
         '''  
         url_obj = parse_url(url)
         url = url_obj.url
+        self.set_base_url(url)
         headers = self.get_request_headers()
         self._session.headers.update(headers)        
 
         # authenticate if credentials are already set
         if not self.is_authenticated and (self.auth_credentials and self.auth_url):
             self.authenticate()
 
@@ -582,48 +635,51 @@
         if mode in ['rb', 'r']:
             raise ValueError("`%s` is not an allowed mode. Allowed modes: 'w+', 'wb+', 'w', 'wb', 'a', ..." % mode)
         if 'b' in mode and isinstance(content, str):
             raise TypeError("`mode` specified is a byte mode. content provide is of type str not bytes")
         if not 'b' in mode and isinstance(content, bytes):
             raise TypeError("`mode` specified is a string mode. content provide is of type bytes not str")
 
+        storage_path = storage_path.replace('/', '\\')
+        storage_path = os.path.normpath(storage_path.removeprefix('\\').removesuffix('\\'))
         try:
             if os.path.isabs(storage_path):
+                os.makedirs(os.path.dirname(storage_path), exist_ok=True)
                 if os.path.isdir(storage_path):
                     file_path = f"{storage_path}\{filename}"
                 else:
                     file_path = storage_path   
             else:
                 file_path = os.path.normpath(f"{self.base_storage_dir}\{storage_path}\{filename}")
-                
+               
             file_hdl = FileHandler(file_path, encoding, exists_ok=True, allow_any=True)
-
+            file_hdl.close_file()
             # Translate content if necessary
             if translate and (self.translate_to and file_hdl.filetype in ['xhtml', 'htm', 'shtml', 'html', 'xml']):
                 content = self.translator.translate_markup(content, target_lang=self.translate_to)
 
             file_hdl.write_to_file(content, mode)
             return file_hdl
         
-        except Exception as e:
+        except (Exception, BaseException) as e:
             self.log(e.__str__(), level='error')
             pass
             
 
-    def parse_storage_path_from_Url(self, url_obj: Url, remove_str: str | None = None) -> str:
+    def parse_storage_path_from_Url(self, url_obj: Url, remove_str: str | None = None):
         '''
         Returns a suitable storage path from a Url object.
 
         Args:
         * `url_obj` (Url): Url object to be parsed.
         * `remove_str` (str): string to be removed from the path. Defaults to None.
         '''
-        url_path = url_obj.path or ''
+        url_path = url_obj.path if url_obj.path is not None else ''
         url_path = url_path.replace(remove_str, '') if remove_str else url_path
-        path = os.path.normpath(url_path.replace('/', '\\'))
+        path = os.path.normpath(url_path.replace('/', '\\').removeprefix('\\'))
         return path
 
 
     def get_rra_by_tag_name(self, tag_name: str) -> str | None:
         '''
         Return the tag attribute that contains the src url/path.
 
@@ -671,16 +727,25 @@
 
         Example Usage::
             >>> bs4_scraper.download_url(url="https://example.com/", save_as="example.html", save_to="/examples", check_ext="False")
         '''
         url_obj = parse_url(url.removesuffix('/'))
         if not url_obj.netloc:
             raise InvalidURLError
-    
-        url_based_name, url_based_ext = os.path.splitext((url_obj.path or '').removesuffix('/').split('/')[-1])
+        self.set_base_url(url_obj.url)
+
+        # Find file name and extension in url if any
+        url_path = (url_obj.path or '').removesuffix('/')
+        url_based_filepath, url_based_file_ext = os.path.splitext(url_path)
+        if url_based_file_ext:
+            url_based_name = url_based_filepath.split('/')[-1]
+            url_based_ext = url_based_file_ext
+        else:
+            url_based_name, url_based_ext = ('', '')
+
         if check_ext and not url_based_ext:
             raise ValueError('Invalid url. No extension found in url. The url may be incorrect.')
         filename = f"{url_based_name}{url_based_ext}"
 
         if save_as:
             if not isinstance(save_as, str):
                 raise TypeError('`save_as` should be of type str')
@@ -696,37 +761,38 @@
 
         response = None
         file_storage_path = save_to.replace('/', '\\').strip() if save_to else save_to
         file_storage_path = os.path.abspath(file_storage_path) if file_storage_path and file_storage_path.startswith('.') else file_storage_path
         # check if url has query params
         has_query_params = bool(url_obj.query)
         if file_storage_path is None:
-            file_storage_path = self.parse_storage_path_from_Url(url_obj, remove_str=f"{url_based_name}{url_based_ext}")  
-            file_storage_path = file_storage_path.removeprefix('\\').removesuffix('\\')    
+            file_storage_path = self.parse_storage_path_from_Url(url_obj=url_obj, remove_str=f"{url_based_name}{url_based_ext}")
    
         if has_query_params and (url_obj.query not in self.url_query_params.keys()):
             if unique_if_query_params is True:
                 filename = utils.generate_unique_filename(filename)
                 
         if has_query_params and (url_obj.query in self.url_query_params.keys()):
             file_hdl: FileHandler = self.url_query_params[url_obj.query]
             return file_hdl
 
         if not has_query_params or (url_obj.query not in self.url_query_params.keys()):
             if os.path.isabs(file_storage_path):
                 full_path = f'{file_storage_path}/{filename}'
-                os.makedirs(os.path.dirname(full_path), exist_ok=True)
             else:
                 full_path = f'{self.base_storage_dir}\{file_storage_path}\{filename}'
             full_path = os.path.normpath(full_path)
+            os.makedirs(os.path.dirname(full_path), exist_ok=True)
+
             # check if file already exists
             if os.path.exists(full_path) is False:
                 response = self.get(url_obj.url)
             else:
                 file_hdl = FileHandler(full_path, exists_ok=True, allow_any=True)
+                file_hdl.close_file()
                 if overwrite is True:
                     file_hdl.delete_file()
                     response = self.get(url_obj.url)
                 else:
                     return file_hdl
 
         if response:
@@ -748,16 +814,16 @@
         * `markup_file_handler` (FileHandler): Markup FileHandler object.
         '''
         if not isinstance(markup_file_handler, FileHandler):
             raise TypeError("`markup_file_handler` should be of type FileHandler")
         if markup_file_handler.filetype not in ['xhtml', 'htm', 'shtml', 'html', 'xml']:
             raise FileError('Unsupported file type')
 
-        markup_file_handler.open_file('r')
-        soup = self.make_soup(markup_file_handler.file)
+        soup = self.make_soup(markup_file_handler.read_file('rb'))
+        markup_file_handler.close_file()
         tags = ResultSet(soup)
         for scrapable_tag in self._scrapable_tags:
             try:
                 parts = scrapable_tag.split('|')
                 if len(parts) == 1:
                     tag_name = scrapable_tag
                     tags.extend(soup.find_all(tag_name))
@@ -791,24 +857,22 @@
     def get_actual_url_from_rra(self, rra: str):
         '''
         Parses the url from a bs4.element.Tag rra
 
         Args::
         * `rra` (str): bs4.element.Tag resource-related-attribute
         '''
+        if not self.base_url:
+            raise AttributeError('`self._base_url` is not set. Ensure to set it before call this method4')
+        rra = rra.replace('\\', '/')
+        # Formatting rra properly
+        rra = '/'.join([ i for i in rra.split('/') if i ])
         url_obj = parse_url(rra)
-        if url_obj.scheme and url_obj.netloc:
-            actual_url = url_obj.url
-        elif url_obj.netloc and not url_obj.scheme:
-            actual_url = Url(
-                scheme='http', host=url_obj.host, 
-                path=url_obj.path, port= url_obj.port, 
-                query=url_obj.query, auth=url_obj.auth,
-                fragment=url_obj.fragment
-            ).url
+        if url_obj.scheme:
+            actual_url = rra
         else:
             actual_url = urljoin(self.base_url, url_obj.url)
         return actual_url
 
 
     def get_tag_rra(self, tag: Tag, download: bool = False):
         '''
```

### Comparing `bs4_web_scraper-0.1.2/bs4_web_scraper/exceptions.py` & `bs4_web_scraper-0.1.3/bs4_web_scraper/exceptions.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.2/bs4_web_scraper/file_handler.py` & `bs4_web_scraper-0.1.3/bs4_web_scraper/file_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,21 @@
 
 
 
 class FileHandler:
     """
     #### Handles basic read and write operations on supported file types.
 
+    NOTE:
+        On instantiation, the file object is opened in 'a+' mode and stored in the `file` attribute.
+        Remember to close the file object by calling the `close_file` method when done with the file.
+
     #### Supported File Types:
     .csv, .json, .txt, .html, .xml, .yml, .yaml, .js, .css, .md, .toml
-    .doc, .docx, .pdf, .pickle, .pkl, .log, 'htm', 'xht', etc. Mostly text based file types.
+    .doc, .docx, .pdf, .pickle, .pkl, .log, '.htm', '.xht', '.xhtml', '.shtml' etc. Mostly text based file types.
 
     #### Parameters:
     @param str `filepath`: path to the file to be read or written to.
 
     @param str `encoding`: encoding to be used when reading or writing to the file. Defaults to 'utf-8'.
 
     @param bool `not_found_ok`: Whether to raise FileNotFoundError if file object specified by `filepath`
@@ -41,56 +45,69 @@
 
     @attr str `created_file`: returns True if file was created by handler, returns False if file was existent.
 
     AVOID USING THE `file` ATTRIBUTE DIRECTLY. USE THE `open_file` AND `close_file` METHODS INSTEAD.
     USE THE `read_file` AND `write_to_file` METHODS TO READ AND WRITE TO THE FILE. PRIVATE METHODS ARE NOT GUARANTEED TO WORK.
     """
 
-    file: IO | None = None
+    _file: IO = None
     created_file: bool = False
 
     def __init__(self, filepath: str, encoding: str = 'utf-8', not_found_ok: bool = True, 
                     exists_ok: bool = True, allow_any: bool = False) -> None:
         self.filepath = os.path.abspath(filepath)
         self.encoding = encoding
         self.allow_any = allow_any
+        
         if not os.path.exists(self.filepath):
             if not_found_ok is False:
                 raise FileNotFoundError(f"File not found: {self.filepath}")
             os.makedirs(os.path.dirname(self.filepath), exist_ok=True)
+            open(self.filepath, 'x').close()
             self.created_file = True
-        elif os.path.exists(self.filepath) and exists_ok is False:
-            raise FileExistsError(f"File already exist: {self.filepath}")
+
+        else:
+            if exists_ok is False:
+                raise FileExistsError(f"File already exist: {self.filepath}")
+        if not os.path.isfile(self.filepath):
+            raise FileError(f"File not created: {self.filepath}. Check if the path points to a file.")
         # open file in append mode by default so it can be written into and read from 
         # even if the `open_file` method has not being called yet.
         self.open_file('a+')
 
 
     def __str__(self) -> str:
         return self.read_file()
 
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.close_file()
+
+    @property
+    def file(self):
+        return self._file
+
     @property
     def filetype(self) -> str:
         filetype = os.path.splitext(self.filepath)[-1].removeprefix('.').lower()
         if filetype in ['yaml', 'yml']:
             filetype = 'yaml'
         elif filetype in ['pickle', 'pkl']:
             filetype = 'pickle'
         return filetype
 
-    
     @property
     def filename(self) -> str:
         filename = self.filepath.replace(os.path.dirname(self.filepath), '')
         return filename.replace('\\', '')
     
-
     @property
     def file_content(self):
-        return self.read_file('r')
+        content = self.read_file('r')
+        self.close_file()
+        return content
 
 
     @staticmethod
     def supported_file_types() -> Tuple[str]:
         return (
         'txt', 'doc', 'docx', 'pdf', 'html', 'htm', 'xml',
          'js', 'css', 'md', 'json', 'csv', 'yaml', 'yml', 
@@ -107,33 +124,34 @@
         '''
         try:
             self.close_file()
         except Exception:
             pass
         try:
             if 'b' in mode:
-                self.file = open(self.filepath, mode=mode)
+                self._file = open(self.filepath, mode=mode)
             else:
-                self.file = open(self.filepath, mode=mode, encoding=self.encoding)
+                self._file = open(self.filepath, mode=mode, encoding=self.encoding)
             return self.file
         except Exception as e:
             raise FileError(f"File cannot be opened. {e}")
 
 
     def close_file(self) -> None:
         '''
         Closes the file.
         '''
-        self.file.close()
+        if self.file:
+         return self.file.close()
         return None
 
 
     def clear_file(self):
         """
-        Deletes file content.
+        Empties file.
 
         Returns the file open in the mode it was being used in before clearing was done.
         """
         im_ = self.file.mode
         self.open_file('w')
         self.file.write('')
         # Opens the file using mode before the the file was cleared to ensure that the file is 
@@ -141,15 +159,17 @@
         return self.open_file(im_)
 
 
     def delete_file(self):
         '''Deletes the file.'''
         try:
             self.close_file()
-            return os.remove(self.filepath)
+            os.remove(self.filepath)
+            self._file = None
+            self.file_path = None
         except Exception as e:
             raise FileError(f"File could not be deleted. {e}")
 
 
     def copy_to(self, destination: str):
         '''
         Copies the file to the specified destination.
@@ -161,14 +181,15 @@
         '''
         # check if destination is a file or directory
         if not os.path.splitext(destination)[1]: # is directory
             hdl = FileHandler(f'{destination}/{self.filename}', encoding=self.encoding)
         else:
             hdl = FileHandler(destination, encoding=self.encoding)
         hdl.write_to_file(self.read_file(), write_mode='w+')
+        self.close_file()
         return hdl
 
 
     def move_to(self, destination: str) -> None:
         '''
         Moves the file to the specified destination. `self.file` becomes the destination file.
 
@@ -177,27 +198,27 @@
 
         Args:
             destination (str): The path to the directory where the file will be moved to.
         '''
         try:
             dst_hdl = self.copy_to(destination)
             self.delete_file()
-            self.file = dst_hdl.file
+            self._file = dst_hdl.file
             self.filepath = dst_hdl.filepath
             return None
         except Exception as e:
             raise FileError(f"File could not be moved. {e}")
     
 
     def read_file(self, read_mode: str | None = None) -> Any:
         '''
         Reads the file and returns the content using the specified `read_mode`.
 
         Args:
-            read_mode(str): The mode to be used to read the file. If None, it reads in 'read(r)' mode.
+            read_mode(str): The mode to be used to read the file. If None, it reads in 'read(r+)' mode.
         '''
         if read_mode and read_mode in ['w', 'wb', 'a', 'ab']:
             raise FileError(f"`{read_mode}` mode does not allow reading from file")
 
         if self.filetype in self.supported_file_types() or self.allow_any is True:
             self.open_file(read_mode or 'r+')
             try:
@@ -332,28 +353,31 @@
 
 
     def _read_pickle(self) -> Any:
         '''
         Reads the file and returns the content.
         '''
         try:
-            return pickle.load(self.file, encoding=self.encoding)
+            self.open_file('rb+')
+            return pickle.load(self.file)
         except Exception as e:
             raise FileError(f'pickle file could not be loaded. {e}')
 
 
     def _write_pickle(self, content: Any) -> None:
         '''
         Writes the content to the file.
 
         Args:
             content (Any): The content to write to the file
         '''
-        pkl = pickle.dumps(content).decode(self.encoding)
-        self.file.write(pkl)
+        # pkl = pickle.dumps(content).decode(self.encoding)
+        # self.file.write(pkl)
+        self.open_file('ab+')
+        pickle.dump(content, self.file)
         return None
 
 
     def _read_toml(self) -> Dict:
         '''
         Reads the file and returns the content as a dictionary.
         '''
```

### Comparing `bs4_web_scraper-0.1.2/bs4_web_scraper/logging.py` & `bs4_web_scraper-0.1.3/bs4_web_scraper/logger.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.2/bs4_web_scraper/request_limiter.py` & `bs4_web_scraper-0.1.3/bs4_web_scraper/request_limiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 from typing import Any
 
-from .logging import Logger
+from .logger import Logger
 
 
 
 class RequestLimitSetting:
     '''
     #### Requests limiting setting.
     Regulates the frequency of requests
@@ -77,15 +77,15 @@
 
         Args:
             message (str): The message to log
             level (str | None): The level of message to log.
         '''
             
         if self.logger and isinstance(self.logger, Logger):
-            self.logger.log(message, level)
+            return self.logger.log(message, level)
         elif self.logger and not isinstance(self.logger, Logger):
             raise TypeError('Invalid type for `self.logger`. `self.logger` should be an instance of bs4_web_scraper.logging.Logger')
         return print(message + '\n')        
 
 
     def got_response_error(self) -> None:
         '''Registers a request response error.'''
```

### Comparing `bs4_web_scraper-0.1.2/bs4_web_scraper/scraper.py` & `bs4_web_scraper-0.1.3/bs4_web_scraper/scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,22 @@
     used to scrape websites.
 
     Don't make high frequency requests! Scrape responsibly!
     If you are using this module to scrape websites for commercial purposes, please consider supporting the
     websites you are scraping by making a donation.
 """
 import os
+from os.path import isabs
 import re
 from typing import (AnyStr, Dict, List, Tuple)
 from collections.abc import Iterable
 import time
-from bs4 import Comment
+from bs4 import Comment, Tag
 from concurrent.futures import ThreadPoolExecutor
+from bs4.element import ResultSet
 from urllib3.util.url import parse_url
 
 from . import utils
 from .base import BS4BaseScraper
 from .file_handler import FileHandler
 
 
@@ -201,15 +203,16 @@
 
         return None
 
     
     def download_urls(self, urls: Iterable[Dict[str, str]] | Iterable[str], save_to: str | None = None, overwrite: bool = False,
                         check_ext: bool = True, fast_download: bool = False, unique_if_query_params: bool = False):
         '''
-        Download files from the given urls using the `download_url` method. Saves the files in a storage path in `self.base_storage_dir`.
+        Download files from the given urls using the `download_url` method. Saves the files in a storage path in `self.base_storage_dir`
+        or in an absolute path as provided.
 
         Returns the storage path of the downloaded files.
 
         Args:
             - urls (Iterable[Dict[str, str]] | Iterable[str]): List of urls to be downloaded. The url in the list can be of type str or dict[str, str].
             - save_to Optional[str]: Path to the directory where the file should be saved in `self.base_storage_dir`.
             - overwrite (bool, optional): Whether to overwrite existing files. Defaults to False.
@@ -291,15 +294,15 @@
             return file_handler.write_to_file(detailed_url_list)
         for r in result: 
             file_handler.write_to_file(f'{r}\n') 
         return None
 
 
     def find_urls(self, url: str, target: str, attrs: Dict[str, str] | Iterable[Dict[str, str]] = {}, 
-                        depth: int = 0, count: int = None, recursive: bool = True):
+                        depth: int = 0, count: int = None, recursive: bool = True) -> List[str]:
         """
         Parses out the url/links on all elements with the target name in specified url.
         NOTE: This only works for elements with a resource(url) related attribute. To get markup elements with no resource related attribute, use `find_all_tags`.
 
         Removes duplicates and returns a list of the links/urls.
 
         Args::
@@ -308,50 +311,67 @@
             * attrs (Dict[str, str] | Iterable[Dict[str, str]]): A dictionary or list of dictionaries of filters on attribute values.
             * depth (int): Number of levels to recursively search for target items. Defaults to 0.
             * count (int): Number of target items to be found on a url page before stopping.
             * recursive (bool): Performs a recursive search of url page's children
         """
         self.set_base_url(url)
         base_url_obj = parse_url(self.base_url)
-        urls = []
+        urls: List[str] = []
         soup = self.make_soup_from_url(url)
         if soup is not None:
-            tags = []
+            tags: ResultSet[Tag] = ResultSet(soup)
             rra = self.get_rra_by_tag_name(target)
             if isinstance(attrs, Iterable) and not isinstance(attrs, dict):
                 for attr in attrs:
-                    tags.extend(soup.find_all(target, attr, recursive=recursive, limit=count))
+                    tags.extend(soup.find_all(target, attr, recursive=recursive))
             else:
-                tags.extend(soup.find_all(target, attrs, recursive=recursive, limit=count))
+                tags = soup.find_all(target, attrs, recursive=recursive)
 
             tags = filter(lambda tag: bool(tag.get(rra)), tags)
             with ThreadPoolExecutor() as executor:
                 results = executor.map(lambda args: self.get_tag_rra(*args), map(lambda tag: (tag, False), tags))
+                results: List[str] = list(set(results))
+
+            if count != None:
+                urls.extend(results[:count])
+                count -= len(urls)
+            else:
                 urls.extend(results)
 
             while depth > 0:
+                if count is not None and count == 0:
+                    break
                 depth -= 1
                 link_tags = soup.find_all('a', recursive=recursive)
                 links = [ self.get_link_tag(link_tag, download=False) for link_tag in link_tags ]
                 links = filter(lambda link: bool(link), links)   
                 link_objs = [ (link, parse_url(link)) for link in links ]
                 links = [ link_obj[0] for link_obj in link_objs if (base_url_obj.netloc and link_obj[1].netloc) and (base_url_obj.netloc in link_obj[1].netloc) ] 
 
-                with ThreadPoolExecutor() as executor:
-                    results = executor.map(lambda args: self.find_urls(*args), map(lambda link: (link, target, attrs, depth, count, recursive), links))
-                    for result in results:
-                        if result:
-                            urls.extend(result)
+                if count is None:
+                    # If count is not specified use threading
+                    with ThreadPoolExecutor() as executor:
+                        results = executor.map(lambda args: self.find_urls(*args), map(lambda link: (link, target, attrs, depth, count, recursive), links))
+                        for result in results:
+                            if result and result not in urls:
+                                urls.extend(result)
+                else:
+                    for link in links:
+                        r = self.find_urls(link, target, attrs, depth, count, recursive)
+                        urls.extend(r[:count])
+                        count -= len(urls)
+                        if count == 0:
+                            break
+                        continue           
                 continue
-        urls = list(set(urls))
         return urls
     
 
     def find_all_tags(self, url: str, target: str, attrs: Dict[str, str] | Iterable[Dict[str, str]] = {},
-                        depth: int = 0, count: int = None, recursive: bool = True):
+                        depth: int = 0, count: int = None, recursive: bool = True) -> ResultSet[Tag]:
         """
         Gets all markup elements with the target name in specified url.
 
         Returns a list of the markup elements with the target name as bs4.element.Tag objects.
 
         Args::
             * url (str): url of page to be parsed and scanned for target elements.
@@ -360,44 +380,61 @@
             * depth (int): Number of levels to recursively search for target items. Defaults to 0.
             * count (int): Number of target items to be found on a url page before stopping.
             * recursive (bool): Performs a recursive search of url page's children
         """
         self.set_base_url(url)
         base_url_obj = parse_url(self.base_url)
         soup = self.make_soup_from_url(url)
-        tags = []
+        tags = ResultSet(soup)
         if soup is not None:
+            r = ResultSet(soup)
             if isinstance(attrs, Iterable) and not isinstance(attrs, dict):
                 for attr in attrs:
-                    tags.extend(soup.find_all(target, attr, recursive=recursive, limit=count))
+                    r.extend(soup.find_all(target, attr, recursive=recursive))
             else:
-                tags.extend(soup.find_all(target, attrs, recursive=recursive, limit=count))
+                r = soup.find_all(target, attrs, recursive=recursive)
+            if count is not None:
+                tags.extend(r[:count])
+                count -= len(tags)
+            else:
+                tags.extend(r)
 
             while depth > 0:
+                if count is not None and count == 0:
+                    break
                 depth -= 1
                 link_tags = soup.find_all('a', recursive=recursive)
                 links = [ self.get_link_tag(link_tag, download=False) for link_tag in link_tags ]
                 links = filter(lambda link: bool(link), links)   
                 link_objs = [ (link, parse_url(link)) for link in links ]
                 links = [ link_obj[0] for link_obj in link_objs if (base_url_obj.netloc and link_obj[1].netloc) and (base_url_obj.netloc in link_obj[1].netloc) ] 
-
-                with ThreadPoolExecutor() as executor:
-                    results = executor.map(lambda args: self.find_all_tags(*args), map(lambda link: (link, target, attrs, depth, count, recursive), links))
-                    for result in results:
-                        if result:
-                            tags.extend(result)
+                if count is None:
+                    # If count is not specified use threading
+                    with ThreadPoolExecutor() as executor:
+                        results = executor.map(lambda args: self.find_all_tags(*args), map(lambda link: (link, target, attrs, depth, count, recursive), links))
+                        for result in results:
+                            if result:
+                                tags.extend(result)
+                else:
+                    for link in links:
+                        r = self.find_all_tags(link, target, attrs, depth, count, recursive)
+                        tags.extend(r[:count])
+                        count -= len(tags)
+                        if count == 0:
+                            break
+                        continue
                 continue
         return tags
 
 
     def find_tags_by_id(self, url: str, id: str, depth: int = 0, count: int = None, recursive: bool = True):
         """
         Gets all markup elements with the target id in specified url.
 
-        Returns a list of the markup elements with the target id as bs4.element.Tag objects.
+        Returns a list of the markup elements as  with the target id as bs4.element.Tag objects.
 
         Args::
             * url (str): url of page to be parsed and scanned for target elements.
             * id (str): id of markup element(s).
             * depth (int): Number of levels to recursively search for target items. Defaults to 0.
             * count (int): Number of target items to be found on a url page before stopping.
             * recursive (bool): Performs a recursive search of url page's children
@@ -432,31 +469,47 @@
             * depth (int): Number of levels to recursively search for target items. Defaults to 0.
             * count (int): Number of target items to be found on a url page before stopping.
             * recursive (bool): Performs a recursive search of url page's children
         """
         self.set_base_url(url)
         base_url_obj = parse_url(self.base_url)
         soup = self.make_soup_from_url(url)
-        comments = []
+        comments = ResultSet(soup)
         if soup is not None:
-            comments = soup.find_all(text=lambda text: isinstance(text, Comment), limit=count, recursive=recursive)
+            r = soup.find_all(string=lambda string: isinstance(string, Comment), recursive=recursive)
+            if count is not None:
+                comments.extend(r[:count])
+                count -= len(comments)
+            else:
+                comments.extend(r)
 
             while depth > 0:
+                if count is not None and count == 0:
+                    break
                 depth -= 1
                 link_tags = soup.find_all('a', recursive=recursive)
                 links = [ self.get_link_tag(link_tag, download=False) for link_tag in link_tags ]
                 links = filter(lambda link: bool(link), links)   
                 link_objs = [ (link, parse_url(link)) for link in links ]
                 links = [ link_obj[0] for link_obj in link_objs if (base_url_obj.netloc and link_obj[1].netloc) and (base_url_obj.netloc in link_obj[1].netloc) ] 
-
-                with ThreadPoolExecutor() as executor:
-                    results = executor.map(lambda args: self.find_comments(*args), map(lambda link: (link, depth, count, recursive), links))
-                    for result in results:
-                        if result:
-                            comments.extend(result)
+                if count is None:
+                    # If count is not specified use threading
+                    with ThreadPoolExecutor() as executor:
+                        results = executor.map(lambda args: self.find_comments(*args), map(lambda link: (link, depth, count, recursive), links))
+                        for result in results:
+                            if result:
+                                comments.extend(result)
+                else:
+                    for link in links:
+                        r = self.find_comments(link, depth, count, recursive)
+                        comments.extend(r[:count])
+                        count -= len(comments)
+                        if count == 0:
+                            break
+                        continue
                 continue
         return comments
 
     
     def find_links(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "links.csv", **kwargs) -> List[str]:
         """
         Gets all the links from the given url.
@@ -467,17 +520,18 @@
             * url (str): Url to get the links from.
             * depth (int, optional): Number of levels to recursively search for links. Defaults to 0.
             * save_to_file (bool, optional): Whether to save the links to a file. Defaults to False.
             * file_path (str, optional): File to save the links to. Defaults to "self.base_storage_dir/links.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats are: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used for 
-                    * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
+                * `count` (int): Number of target items to be found on a url page before stopping.
+                * `csv_head` (str): Heading to be used for saving 'csv' results and is passed to the `save_results` function if `save_to_file` is True.
         """
-        result = self.find_urls(url, target='a', depth=depth)
+        result = self.find_urls(url, target='a', depth=depth, count=kwargs.get('count', None))
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Links')
             self.save_results(result, file_path, **kwargs)
         return result
 
 
     def find_stylesheets(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "styles.csv", **kwargs) -> List[str]:
@@ -490,21 +544,22 @@
             * url (str): Url to get the styles from.
             * depth (int, optional): Number of levels to recursively search for stylesheet links. Defaults to 0.
             * save_to_file (bool, optional): Whether to save the styles to a file. Defaults to False.
             * file_path (str, optional): File to save the links to. Defaults to "self.base_storage_dir/styles.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used for 
-                    * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
+                    * `count` (int): Number of target items to be found on a url page before stopping.
+                    * `csv_head` (str): Heading to be used for saving 'csv' results and is passed to the `save_results` function if `save_to_file` is True.
         """
         attrs = (
             {'rel': 'stylesheet'},
             {'type': 'text/css'}
         )
-        result = self.find_urls(url, target='link', attrs=attrs, depth=depth)
+        result = self.find_urls(url, target='link', attrs=attrs, depth=depth, count=kwargs.get('count', None))
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Stylesheets')
             self.save_results(result, file_path, **kwargs)
         return result
             
 
     def find_scripts(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "scripts.csv", **kwargs) -> List[str]:
@@ -517,17 +572,18 @@
             * `url` (str): Url to get the scripts from.
             * `depth` (int, optional): Number of levels to recursively search for script links. Defaults to 0.
             * `save_to_file` (bool, optional): Whether to save the scripts to a file. Defaults to False.
             * `file_path` (str, optional): File to save the links to. Defaults to "self.base_storage_dir/scripts.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * `**kwargs` (Dict | optional): optional parameters to be used for 
-                    * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
+                * `count` (int): Number of target items to be found on a url page before stopping.
+                * `csv_head` (str): Heading to be used for saving 'csv' results and is passed to the `save_results` function if `save_to_file` is True.
         """
-        result = self.find_urls(url, target='script', depth=depth)
+        result = self.find_urls(url, target='script', depth=depth, count=kwargs.get('count', None))
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Scripts')
             self.save_results(result, file_path, **kwargs)
         return result
 
     
     def find_fonts(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "fonts.csv", **kwargs) -> List[str]:
@@ -540,21 +596,22 @@
             * url (str): Url to get the fonts from.
             * depth (int, optional): Number of levels to recursively search for font links. Defaults to 0.
             * save_to_file (bool, optional): Whether to save the fonts to a file. Defaults to False.
             * file_path (str, optional): File to save the links to. Defaults to "self.base_storage_dir/fonts.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used for 
-                    * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
+                * `count` (int): Number of target items to be found on a url page before stopping.
+                * `csv_head` (str): Heading to be used for saving 'csv' results and is passed to the `save_results` function if `save_to_file` is True.
         """
         attrs = (
             {'rel': 'preload'},
             {'as': 'font'}
         )
-        result = self.find_urls(url, target='link', attrs=attrs, depth=depth)
+        result = self.find_urls(url, target='link', attrs=attrs, depth=depth, count=kwargs.get('count', None))
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Font Links')
             self.save_results(result, file_path, **kwargs)
         return result
 
     
     def find_images(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "images.csv", **kwargs) -> List[str]:
@@ -567,17 +624,18 @@
             * url (str): Url to get the images from.
             * depth (int, optional): Number of levels to recursively search for image links. Defaults to 0.
             * save_to_file (bool, optional): Whether to save the images to a file. Defaults to False.
             * file_path (str, optional): File to save the links to. Defaults to "self.base_storage_dir/images.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used for 
-                    * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
+                * `count` (int): Number of target items to be found on a url page before stopping.
+                * `csv_head` (str): Heading to be used for saving 'csv' results and is passed to the `save_results` function if `save_to_file` is True.
         """
-        result = self.find_urls(url, target='img', depth=depth)
+        result = self.find_urls(url, target='img', depth=depth, count=kwargs.get('count', None))
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Image Links')
             self.save_results(result, file_path, **kwargs)
         return result
 
 
     def find_videos(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "videos.csv", **kwargs) -> List[str]:
@@ -590,19 +648,20 @@
             * url (str): Url to get the videos from.
             * depth (int, optional): Number of levels to recursively search for video links. Defaults to 0.
             * save_to_file (bool, optional): Whether to save the videos to a file. Defaults to False.
             * file_path (str, optional): File to save the links to. Defaults to "self.base_storage_dir/videos.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used when and where necessary
-                    * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
+                * `count` (int): Number of target items to be found on a url page before stopping.
+                * `csv_head` (str): Heading to be used for saving 'csv' results and is passed to the `save_results` function if `save_to_file` is True.
         """
         video_types = ('video/mp4', 'video/mpeg', 'video/ogg', 'video/webm', 'video/3gpp', 'video/quicktime')
         v_list = [ {'type': v} for v in video_types ]
-        result = self.find_urls(url, target='source', attrs=v_list, depth=depth)
+        result = self.find_urls(url, target='source', attrs=v_list, depth=depth, count=kwargs.get('count', None))
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Video Links')
             self.save_results(result, file_path, **kwargs)
         return result
 
 
     def find_audios(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "audios.csv", **kwargs) -> List[str]:
@@ -614,20 +673,21 @@
         Args:
             * url (str): Url to get the audios from.
             * depth (int, optional): Number of levels to recursively search for audio links. Defaults to 0.
             * save_to_file (bool, optional): Whether to save the audios to a file. Defaults to False.
             * file_path (str, optional): File to save the links to. Defaults to "self.base_storage_dir/audios.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
-            * **kwargs (Dict | optional): optional parameters to be used for 
-                    * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
+            * **kwargs (Dict | optional): optional parameters to be used for
+                * `count` (int): Number of target items to be found on a url page before stopping. 
+                * `csv_head` (str): Heading to be used for saving 'csv' results and is passed to the `save_results` function if `save_to_file` is True.
         '''
         audio_types = ('audio/mpeg', 'audio/mp3', 'audio/ogg', 'audio/wav', 'audio/aac', 'audio/flac', 'audio/m4a', 'audio/wma')
         a_list = [ {'type': a} for a in audio_types ]
-        result = self.find_urls(url, target='source', attrs=a_list, depth=depth)
+        result = self.find_urls(url, target='source', attrs=a_list, depth=depth, count=kwargs.get('count', None))
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Audio Links')
             self.save_results(result, file_path, **kwargs)
         return result
         
 
     def find_emails(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "emails.csv", **kwargs) -> List[str]:
@@ -638,21 +698,22 @@
             * url (str): Url to get the emails from.
             * depth (int, optional): Number of levels to recursively search for emails. Defaults to 0.
             * save_to_file (bool, optional): Whether to save the emails to a file. Defaults to False.
             * file_path (str, optional): File to save the links to. Defaults to "self.base_storage_dir/emails.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used for
-                    * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
-                    * `re_flags` (RegexFlag): adding regex flags and is passed to the `re.compile` function.
+                * `count` (int): Number of target items to be found on a url page before stopping.
+                * `csv_head` (str): Heading to be used for saving 'csv' results and is passed to the `save_results` function if `save_to_file` is True.
+                * `re_flags` (RegexFlag): adding regex flags and is passed to the `re.compile` function.
         """
         email_re = r'[-|\w]+@\w+.\w{2,}'
         kwargs['re_flags'] = kwargs.get('re_flags', re.IGNORECASE)
         kwargs['csv_head'] = kwargs.get('csv_head', 'Emails')
-        return self.find_pattern(url, email_re, depth, save_to_file, file_path, kwargs)
+        return self.find_pattern(url, email_re, depth, save_to_file, file_path, **kwargs)
 
 
     def find_phone_numbers(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "phones.csv", **kwargs) -> List[Tuple[str, str]]:
         """
         Searches for and returns a list of phone numbers which conform to the E.164 standard found in the given url. 
 
         Returns a list of phone numbers.
@@ -661,58 +722,80 @@
             * `url` (str): Url to get the phone numbers from.
             * `depth` (int, optional): Number of levels to recursively search for phone numbers. Defaults to 0.
             * `save_to_file` (bool, optional): Whether to save the phone numbers to a file. Defaults to False.
             * `file_path` (str, optional): File to save the links to. Defaults to "self.base_storage_dir/phones.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * `**kwargs` (Dict | optional): optional parameters to be used for
-                    * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
-                    * `re_flags` (RegexFlag): adding regex flags and is passed to the `re.compile` function.
+                * `count` (int): Number of target items to be found on a url page before stopping.
+                * `csv_head` (str): Heading to be used for saving 'csv' results and is passed to the `save_results` function if `save_to_file` is True.
+                * `re_flags` (RegexFlag): adding regex flags and is passed to the `re.compile` function.
         """
         pn_re = r'(\+\d{1,3})?[\s-]?(\d{7,16})'
         kwargs['csv_head'] = kwargs.get('csv_head', 'Phone Numbers')
-        return self.find_pattern(url, pn_re, depth, save_to_file, file_path, kwargs)
+        return self.find_pattern(url, pn_re, depth, save_to_file, file_path, **kwargs)
 
 
-    def find_pattern(self, url: str, regex: str | AnyStr, depth: int = 0, save_to_file: bool = False, file_path: str = "re.csv", kwargs: Dict[str, str] = None) -> List[str]:
+    def find_pattern(self, url: str, regex: str | AnyStr, depth: int = 0, save_to_file: bool = False, file_path: str = "re.csv", count: int = None, **kwargs) -> List[str]:
         """
         Takes a regex pattern and returns a list of matches found in the given url.
 
         Args:
             * url (str): Url to get the matches from.
             * regex (str | AnyStr): Regex pattern to search for.
             * depth (int, optional): Number of levels to recursively search for matches. Defaults to 0.
             * save_to_file (bool, optional): Whether to save the matches to a file. Defaults to False.
             * file_path (str, optional): File to save the links to. Defaults to "self.base_storage_dir/re.csv".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used for
-                    * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
-                    * `re_flags` (RegexFlag): adding regex flags and is passed to the `re.compile` function.
+                * `csv_head` (str): Heading to be used for saving 'csv' results and is passed to the `save_results` function if `save_to_file` is True.
+                * `re_flags` (RegexFlag): adding regex flags and is passed to the `re.compile` function.
         """
         self.set_base_url(url)
         base_url_obj = parse_url(self.base_url)
         pattern = re.compile(regex, flags=kwargs.get('re_flags', re.MULTILINE))
         soup = self.make_soup_from_url(url)
         text = soup.get_text() if soup else ''
         result = list({ match for match in pattern.findall(text) })
-
+        if count is not None:
+            result = result[:count]
+            count -= len(result)
+            
         while depth > 0:
+            if count is not None and count == 0:
+                break
             depth -= 1
             link_tags = soup.find_all('a', recursive=True)
             links = [ self.get_link_tag(link_tag, download=False) for link_tag in link_tags ]
             links = filter(lambda link: bool(link), links)
             link_objs = [ (link, parse_url(link)) for link in links ]
             links = [ link_obj[0] for link_obj in link_objs if (base_url_obj.netloc and link_obj[1].netloc) and (base_url_obj.netloc in link_obj[1].netloc) ]
-
-            with ThreadPoolExecutor() as executor:
-                results = executor.map(lambda args: self.find_pattern(*args), map(lambda link: (link, regex, depth, save_to_file, file_path, kwargs), links))
-                for r in results:
-                    if r:
-                        result.extend(r)
+            if count is None:
+                # If count is not specified use threading
+                with ThreadPoolExecutor() as executor:
+                    kwargs_ = {
+                        'regex': regex,
+                        'depth': depth,
+                        'save_to_file': False,
+                        'file_path': file_path,
+                        **kwargs
+                    }
+                    results = executor.map(lambda kwargs: self.find_pattern(**kwargs), map(lambda link: {'url': link, **kwargs_}, links))
+                    for r in results:
+                        if r:
+                            result.extend(r)
+            else:
+                for link in links:
+                    r = self.find_pattern(link, regex=regex, depth=depth, save_to_file=False, file_path=file_path, count=count, **kwargs)
+                    result.extend(r[:count])
+                    count -= len(result)
+                    if count == 0:
+                        break
+                    continue
             continue
 
         result_ = []
         for r in result:
             if isinstance(r, (list, tuple)):
                 r = ''.join(r)
             result_.append(r)
```

### Comparing `bs4_web_scraper-0.1.2/bs4_web_scraper/translate.py` & `bs4_web_scraper-0.1.3/bs4_web_scraper/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 DESCRIPTION: ::
     This module contains the Translator class for translating text and markup (html, xml, xhtml...) content using the `translators` package.
 
     Avoid making high frequency requests to the translation engine. This may result in your IP address being blocked.
     Enterprises provide free services, we should be grateful instead of making trouble.
 """
 
-from typing import Dict, List
+from typing import Dict, List, IO
 import time
 import copy
 import random
 from bs4 import BeautifulSoup
 from bs4.element import Tag
 from concurrent.futures import ThreadPoolExecutor
 import translators as ts
 from translators.server import TranslatorsServer, tss
 
 from . import utils
-from .logging import Logger
+from .logger import Logger
 from .file_handler import FileHandler
 from .exceptions import TranslationError, UnsupportedLanguageError
 
 
 
 translation_engines = ts.translators_pool
 
@@ -80,24 +80,46 @@
         'caption', 'bdo', 'var', 'h3', 'tt', 'address', 'h4', 'legend', 'i', 
         'small', 'b', 'q', 'option', 'code', 'h2', 'a', 'strong', 'span',
     ]
 
     def __init__(self, translation_engine: str = "bing", ) -> None:
         self.translation_engine = translation_engine
 
+    @property
+    def server(self):
+        return self._server
 
     @property
     def supported_languages(self) -> dict:
         if self.translation_engine:
             args = ('yes','en', 'am')
             func = lambda f: getattr(self._server, f"{self.translation_engine}")(*f)
             func(args)
             return getattr(self._server, f"_{self.translation_engine}").language_map
         return {}
 
+
+    def detect_language(self, _s: str) -> Dict:
+        """
+        Detects the language of the specified text.
+
+        NOTE: This method is not guaranteed to work always.
+        An example of a case where the function does not work is in detecting Amharic.
+
+        Returns a dictionary containing the language code and confidence score.
+
+        Args:
+            _s (str): The text to detect the language of.
+        """
+        try:
+            details = self.server.translate_text(query_text=_s, translator='bing', is_detail_result=True)
+        except:
+            return {}
+        return details.get('detectedLanguage', {}) if details else {}
+
     
     def _log(self, message: str, level: str | None = None) -> None:
         '''
         Logs a message using `self.logger` or prints it out if `self.logger` is None.
 
         Args:
             message (str): The message to log
@@ -248,21 +270,21 @@
         }
         kwargs_.update(kwargs)
         try:
             if cache:
                 if self._cache.get(text, None):
                     return self._cache[text]
                 else:
-                    translated_text = ts.translate_text(
+                    translated_text = self.server.translate_text(
                                                 query_text=text, to_language=target_lang, from_language=src_lang, 
                                                 translator=self.translation_engine, **kwargs_
                                                 )
                     self._cache[text] = translated_text
                     return translated_text
-            return ts.translate_text(
+            return self.server.translate_text(
                                 query_text=text, to_language=target_lang, from_language=src_lang, 
                                 translator=self.translation_engine, **kwargs_
                                 )
         except Exception as e:
             error_ = TranslationError(f"Error translating text: {e}")
             self._log(f"{error_}", level='error')
             return text
@@ -275,15 +297,14 @@
         Returns the translated markup.
 
         Args:
             markup (str | bytes): markup content to be translated
             src_lang (str, optional): Source language. Defaults to "auto".
             target_lang (str, optional): Target language. Defaults to "en".
             **kwargs: Keyword arguments to be passed to `translators.translate_markup`.
-                    :param is_detail_result: boolean, default False.
                     :param professional_field: str, support baidu(), caiyun(), alibaba() only.
                     :param timeout: float, default None.
                     :param proxies: dict, default None.
                     :param sleep_seconds: float, default random.random().
                     :param update_session_after_seconds: float, default 1500.
                     :param if_use_cn_host: bool, default False.
                     :param reset_host_url: str, default None.
@@ -293,15 +314,15 @@
                     :param if_show_time_stat: boolean, default False.
                     :param show_time_stat_precision: int, default 4.
                     :param lingvanex_model: str, default 'B2C'.
         '''
         if not isinstance(markup, (str, bytes)):
             raise TypeError("Invalid type for `markup`")
         is_bytes = isinstance(markup, bytes)
-
+        kwargs.pop('is_detail_result', None)
         soup = BeautifulSoup(markup, 'lxml')
         translated_markup = self.translate_soup(soup, src_lang, target_lang, **kwargs).prettify()
 
         # re-encode the markup if the initial markup was in bytes
         if is_bytes:
             translated_markup = translated_markup.encode('utf-8')
         return translated_markup
@@ -360,20 +381,19 @@
         '''
         Translates file from `src_lang` to `target_lang`.
 
         Returns translated file's FileHandler`.
 
         Supported file types include: .txt, .csv, .doc, .docx, .pdf, .md..., mostly files with text content.
 
-        Args:
-            filepath (str): path to the file to be translated.
-            src_lang (str, optional): Source language. Defaults to "auto".
-            target_lang (str, optional): Target language. Defaults to "en".
-            **kwargs: Keyword arguments to be passed to `translators.translate_text`.
-                    :param is_detail_result: boolean, default False.
+        Args::
+            * filepath (str): path to the file to be translated.
+            * src_lang (str, optional): Source language. Defaults to "auto".
+            * target_lang (str, optional): Target language. Defaults to "en".
+            * **kwargs: Keyword arguments to be passed to `translators.translate_text`.
                     :param professional_field: str, support baidu(), caiyun(), alibaba() only.
                     :param timeout: float, default None.
                     :param proxies: dict, default None.
                     :param sleep_seconds: float, default random.random().
                     :param update_session_after_seconds: float, default 1500.
                     :param if_use_cn_host: bool, default False.
                     :param reset_host_url: str, default None.
@@ -384,28 +404,32 @@
                     :param show_time_stat_precision: int, default 4.
                     :param lingvanex_model: str, default 'B2C'.
         '''
         self.set_target_and_src_lang(target_lang, src_lang)
         kwargs_ = {
             'if_ignore_empty_query': True,
         }
+        kwargs.pop('is_detail_result', None)
         kwargs_.update(kwargs)
         file_handler = FileHandler(filepath, not_found_ok=False)
-        file_content = file_handler.read_file()
+        file_content = file_handler.file_content
 
         if file_handler.filetype in ['xhtml', 'htm', 'shtml', 'html', 'xml']:
-            return self.translate_markup(file_content, src_lang, target_lang, **kwargs)
+            translated_markup = self.translate_markup(file_content, src_lang, target_lang, **kwargs)
+            file_handler.write_to_file(translated_markup, 'w')
+            file_handler.close_file()
+            return file_handler
 
         slice_size = kwargs_.get('limit_of_length', 4000)
         contents = utils.slice_iterable(file_content, slice_size)
         try:
             translated_contents = list(map(lambda text: self.translate_text(text, src_lang, target_lang, False, **kwargs_), contents))
             translated_text = "".join(translated_contents)
             file_handler.write_to_file(translated_text, write_mode='w+')
-            file_handler._open_file(mode='r+')
+            file_handler.close_file()
             return file_handler
         except Exception as e:
             raise TranslationError(f"File cannot be translated. {e}")
 
 
     def translate_soup_tag(self, element: Tag, src_lang: str = "auto", target_lang: str = "en", _ct: int = 0, **kwargs) -> None:
         '''
```

### Comparing `bs4_web_scraper-0.1.2/bs4_web_scraper/utils.py` & `bs4_web_scraper-0.1.3/bs4_web_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.1.2/bs4_web_scraper.egg-info/PKG-INFO` & `bs4_web_scraper-0.1.3/bs4_web_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs4-web-scraper
-Version: 0.1.2
+Version: 0.1.3
 Summary: A web scraper based on the BeautifulSoup4 library and translators package.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/bs4_web_scraper
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/bs4_web_scraper/issues
 Project-URL: Repository, https://github.com/ti-oluwa/bs4_web_scraper
 Keywords: web scraper,bs4,beautifulsoup4,web scraping,web scraping with python,web scraping with bs4,web scraping with beautifulsoup4,web scraping with translation,web scraping with translation to other languages,web scraping with translation to other languages with python,web scraping with translation to other languages with bs4,web scraping with translation to other languages with beautifulsoup4,web scraping with translation to other languages with python and bs4,web scraping with translation to other languages with python and beautifulsoup4
```

### Comparing `bs4_web_scraper-0.1.2/pyproject.toml` & `bs4_web_scraper-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bs4_web_scraper"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 description = "A web scraper based on the BeautifulSoup4 library and translators package."
```

