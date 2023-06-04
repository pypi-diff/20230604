# Comparing `tmp/facebook_page_scraper-4.0.3.tar.gz` & `tmp/facebook_page_scraper-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_page_scraper-4.0.3.tar", last modified: Sun Feb 19 06:32:39 2023, max compression
+gzip compressed data, was "facebook_page_scraper-5.0.0.tar", last modified: Sun Jun  4 12:42:06 2023, max compression
```

## Comparing `facebook_page_scraper-4.0.3.tar` & `facebook_page_scraper-5.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 06:32:39.746683 facebook_page_scraper-4.0.3/
--rw-rw-rw-   0        0        0     1090 2021-01-01 03:52:50.000000 facebook_page_scraper-4.0.3/LICENSE
--rw-rw-rw-   0        0        0       17 2022-04-14 08:09:34.000000 facebook_page_scraper-4.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    12498 2023-02-19 06:32:39.746683 facebook_page_scraper-4.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    11177 2022-10-05 09:29:57.000000 facebook_page_scraper-4.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-19 06:32:39.740785 facebook_page_scraper-4.0.3/facebook_page_scraper/
--rw-rw-rw-   0        0        0      322 2022-08-20 06:31:28.000000 facebook_page_scraper-4.0.3/facebook_page_scraper/__init__.py
--rw-rw-rw-   0        0        0     4501 2022-10-05 09:29:57.000000 facebook_page_scraper-4.0.3/facebook_page_scraper/driver_initialization.py
--rw-rw-rw-   0        0        0     7369 2022-11-08 07:01:11.000000 facebook_page_scraper-4.0.3/facebook_page_scraper/driver_utilities.py
--rw-rw-rw-   0        0        0    17022 2023-02-19 06:31:55.000000 facebook_page_scraper-4.0.3/facebook_page_scraper/element_finder.py
--rw-rw-rw-   0        0        0    15701 2022-11-08 07:01:11.000000 facebook_page_scraper-4.0.3/facebook_page_scraper/scraper.py
--rw-rw-rw-   0        0        0     5248 2022-10-05 09:29:57.000000 facebook_page_scraper-4.0.3/facebook_page_scraper/scraping_utilities.py
-drwxrwxrwx   0        0        0        0 2023-02-19 06:32:39.745684 facebook_page_scraper-4.0.3/facebook_page_scraper.egg-info/
--rw-rw-rw-   0        0        0    12498 2023-02-19 06:32:39.000000 facebook_page_scraper-4.0.3/facebook_page_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-02-19 06:32:39.000000 facebook_page_scraper-4.0.3/facebook_page_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 06:32:39.000000 facebook_page_scraper-4.0.3/facebook_page_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-02-19 06:32:39.000000 facebook_page_scraper-4.0.3/facebook_page_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-02-19 06:32:39.000000 facebook_page_scraper-4.0.3/facebook_page_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-19 06:32:39.746683 facebook_page_scraper-4.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1726 2023-02-19 06:31:55.000000 facebook_page_scraper-4.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 12:42:06.834387 facebook_page_scraper-5.0.0/
+-rw-rw-rw-   0        0        0     1090 2021-01-01 03:52:50.000000 facebook_page_scraper-5.0.0/LICENSE
+-rw-rw-rw-   0        0        0       17 2022-04-14 08:09:34.000000 facebook_page_scraper-5.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12291 2023-06-04 12:42:06.833386 facebook_page_scraper-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10970 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 12:42:06.808408 facebook_page_scraper-5.0.0/facebook_page_scraper/
+-rw-rw-rw-   0        0        0      322 2022-08-20 06:31:28.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/driver_initialization.py
+-rw-rw-rw-   0        0        0     7853 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/driver_utilities.py
+-rw-rw-rw-   0        0        0    17022 2023-02-19 06:31:55.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/element_finder.py
+-rw-rw-rw-   0        0        0    15742 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/scraper.py
+-rw-rw-rw-   0        0        0     5248 2022-10-05 09:29:57.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/scraping_utilities.py
+drwxrwxrwx   0        0        0        0 2023-06-04 12:42:06.832387 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/
+-rw-rw-rw-   0        0        0    12291 2023-06-04 12:42:06.000000 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-06-04 12:42:06.000000 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 12:42:06.000000 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-04 12:42:06.000000 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-04 12:42:06.000000 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 12:42:06.834387 facebook_page_scraper-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1726 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.0/setup.py
```

### Comparing `facebook_page_scraper-4.0.3/LICENSE` & `facebook_page_scraper-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-4.0.3/PKG-INFO` & `facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: facebook_page_scraper
-Version: 4.0.3
+Name: facebook-page-scraper
+Version: 5.0.0
 Summary: Python package to scrap facebook's pages front end with no limitations
 Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium facebook facebook-pages
 Classifier: Development Status :: 4 - Beta
@@ -118,15 +118,15 @@
 proxy = "IP:PORT" #if proxy requires authentication then user:password@IP:PORT
 timeout = 600 #600 seconds
 headless = True
 meta_ai = Facebook_scraper(page_name, posts_count, browser, proxy=proxy, timeout=timeout, headless=headless)
 
 ```
 
-<h3 id="scraperParameters"> Parameters for  <code>Facebook_scraper(page_name, posts_count, browser, proxy, timeout, headless, browser_profile) </code> class </h3>
+<h3 id="scraperParameters"> Parameters for  <code>Facebook_scraper(page_name, posts_count, browser, proxy, timeout, headless) </code> class </h3>
 <table>
 <th>
 <tr>
 <td> Parameter Name </td>
 <td> Parameter Type </td>
 <td> Description </td>
 </tr>
@@ -200,25 +200,14 @@
 </td>
 <td>
 Whether to run browser in headless mode?. Default is True
  </code>
 </td>
 </tr>
 
-<tr>
-<td>
-browser_profile
-</td>
-<td>
-String
-</td>
-<td>
-Path to the browser profile where cookies are stored and can be used for scraping data in an authenticated way.
-</td>
-</tr>
 
 </table>
 <br>
 <hr>
 <br>
 
 <h3> Done with instantiation?. <b>Let the scraping begin!</b> </h3>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: facebook_page_scraper Version: 4.0.3 Summary:
+Metadata-Version: 2.1 Name: facebook-page-scraper Version: 5.0.0 Summary:
 Python package to scrap facebook's pages front end with no limitations Home-
 page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
@@ -57,32 +57,29 @@
 ```python #import Facebook_scraper class from facebook_page_scraper from
 facebook_page_scraper import Facebook_scraper #instantiate the Facebook_scraper
 class page_name = "metaai" posts_count = 10 browser = "firefox" proxy = "IP:
 PORT" #if proxy requires authentication then user:password@IP:PORT timeout =
 600 #600 seconds headless = True meta_ai = Facebook_scraper(page_name,
 posts_count, browser, proxy=proxy, timeout=timeout, headless=headless) ```
 **** Parameters for Facebook_scraper(page_name, posts_count, browser, proxy,
-timeout, headless, browser_profile) class ****
+timeout, headless) class ****
 Parameter Name  Parameter Type Description
 page_name       String         Name of the facebook page
 posts_count     Integer        Number of posts to scrap, if not passed default
                                is 10
 browser         String         Which browser to use, either chrome or firefox.
                                if not passed,default is chrome
                                Optional argument, if user wants to set proxy,
 proxy(optional) String         if proxy requires authentication then the format
                                will be user:password@IP:PORT
                                The maximum amount of time the bot should run
 timeout         Integer        for. If not passed, the default timeout is set
                                to 10 minutes
 headless        Boolean        Whether to run browser in headless mode?.
                                Default is True
-                               Path to the browser profile where cookies are
-browser_profile String         stored and can be used for scraping data in an
-                               authenticated way.
 
 ===============================================================================
 
 **** Done with instantiation?. Let the scraping begin! ****
 
 **** For post's data in JSON format: ****
 ```python #call the scrap_to_json() method json_data = meta_ai.scrap_to_json()
```

### Comparing `facebook_page_scraper-4.0.3/README.md` & `facebook_page_scraper-5.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: facebook_page_scraper
+Version: 5.0.0
+Summary: Python package to scrap facebook's pages front end with no limitations
+Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
+Author: Sajid Shaikh
+Author-email: shaikhsajid3732@gmail.com
+License: MIT
+Keywords: web-scraping selenium facebook facebook-pages
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Internet :: WWW/HTTP
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1> Facebook Page Scraper </h1>
 
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https://github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity)
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 
 <p> No need of API key, No limitation on number of requests. Import the library and <b> Just Do It !<b> </p>
 
@@ -88,15 +118,15 @@
 proxy = "IP:PORT" #if proxy requires authentication then user:password@IP:PORT
 timeout = 600 #600 seconds
 headless = True
 meta_ai = Facebook_scraper(page_name, posts_count, browser, proxy=proxy, timeout=timeout, headless=headless)
 
 ```
 
-<h3 id="scraperParameters"> Parameters for  <code>Facebook_scraper(page_name, posts_count, browser, proxy, timeout, headless, browser_profile) </code> class </h3>
+<h3 id="scraperParameters"> Parameters for  <code>Facebook_scraper(page_name, posts_count, browser, proxy, timeout, headless) </code> class </h3>
 <table>
 <th>
 <tr>
 <td> Parameter Name </td>
 <td> Parameter Type </td>
 <td> Description </td>
 </tr>
@@ -170,25 +200,14 @@
 </td>
 <td>
 Whether to run browser in headless mode?. Default is True
  </code>
 </td>
 </tr>
 
-<tr>
-<td>
-browser_profile
-</td>
-<td>
-String
-</td>
-<td>
-Path to the browser profile where cookies are stored and can be used for scraping data in an authenticated way.
-</td>
-</tr>
 
 </table>
 <br>
 <hr>
 <br>
 
 <h3> Done with instantiation?. <b>Let the scraping begin!</b> </h3>
@@ -220,15 +239,15 @@
       "cares": 0,
       "sad": 0,
       "angry": 0,
       "haha": 0
     },
     "reaction_count": 173,
     "comments": 2,
-    "content": "We’ve built data2vec, the first general high-performance self-supervised algorithm for speech, vision, and text. We applied it to different modalities and found it matches or outperforms the best self-supervised algorithms. We hope this brings us closer to a world where computers can learn to solve many different tasks without supervision. Learn more and get the code:  https://ai.facebook.com/…/the-first-high-performance-self-s…",
+    "content": "Weâ€™ve built data2vec, the first general high-performance self-supervised algorithm for speech, vision, and text. We applied it to different modalities and found it matches or outperforms the best self-supervised algorithms. We hope this brings us closer to a world where computers can learn to solve many different tasks without supervision. Learn more and get the code:  https://ai.facebook.com/â€¦/the-first-high-performance-self-sâ€¦",
     "posted_on": "2022-01-20T22:43:35",
     "video": [],
     "image": [
       "https://scontent-bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/272147088_2024182621092014_6532581039236849529_n.jpg?_nc_cat=100&ccb=1-5&_nc_sid=8024bb&_nc_ohc=j4_1PAndJTIAX82OLNq&_nc_ht=scontent-bom1-2.xx&oh=00_AT9us__TvC9eYBqRyQEwEtYSit9r2UKYg0gFoRK7Efrhyw&oe=61F17B71"
     ],
     "post_url": "https://www.facebook.com/MetaAI/photos/a.360372474139712/2024182624425347/?type=3&__xts__%5B0%5D=68.ARBoSaQ-pAC_ApucZNHZ6R-BI3YUSjH4sXsfdZRQ2zZFOwgWGhjt6dmg0VOcmGCLhSFyXpecOY9g1A94vrzU_T-GtYFagqDkJjHuhoyPW2vnkn7fvfzx-ql7fsBYxL5DgQVSsiC1cPoycdCvHmi6BV5Sc4fKADdgDhdFvVvr-ttzXG1ng2DbLzU-XfSes7SAnrPs-gxjODPKJ7AdqkqkSQJ4HrsLgxMgcLFdCsE6feWL7rXjptVWegMVMthhJNVqO0JHu986XBfKKqB60aBFvyAzTSEwJD6o72GtnyzQ-BcH7JxmLtb2_A&__tn__=-R"
   }, ...
@@ -280,15 +299,15 @@
 meta_ai.scrap_to_csv(filename, directory)
 
 ```
 
 content of ```data_file.csv```:
 ```csv
 id,name,shares,likes,loves,wow,cares,sad,angry,haha,reactions_count,comments,content,posted_on,video,image,post_url
-2024182624425347,Meta AI,0,154,19,0,0,0,0,0,173,2,"We’ve built data2vec, the first general high-performance self-supervised algorithm for speech, vision, and text. We applied it to different modalities and found it matches or outperforms the best self-supervised algorithms. We hope this brings us closer to a world where computers can learn to solve many different tasks without supervision. Learn more and get the code:  https://ai.facebook.com/…/the-first-high-performance-self-s…",2022-01-20T22:43:35,,https://scontent-bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/272147088_2024182621092014_6532581039236849529_n.jpg?_nc_cat=100&ccb=1-5&_nc_sid=8024bb&_nc_ohc=j4_1PAndJTIAX82OLNq&_nc_ht=scontent-bom1-2.xx&oh=00_AT9us__TvC9eYBqRyQEwEtYSit9r2UKYg0gFoRK7Efrhyw&oe=61F17B71,https://www.facebook.com/MetaAI/photos/a.360372474139712/2024182624425347/?type=3&__xts__%5B0%5D=68.ARAse4eiZmZQDOZumNZEDR0tQkE5B6g50K6S66JJPccb-KaWJWg6Yz4v19BQFSZRMd04MeBmV24VqvqMB3oyjAwMDJUtpmgkMiITtSP8HOgy8QEx_vFlq1j-UEImZkzeEgSAJYINndnR5aSQn0GUwL54L3x2BsxEqL1lElL7SnHfTVvIFUDyNfAqUWIsXrkI8X5KjoDchUj7aHRga1HB5EE0x60dZcHogUMb1sJDRmKCcx8xisRgk5XzdZKCQDDdEkUqN-Ch9_NYTMtxlchz1KfR0w9wRt8y9l7E7BNhfLrmm4qyxo-ZpA&__tn__=-R
+2024182624425347,Meta AI,0,154,19,0,0,0,0,0,173,2,"Weâ€™ve built data2vec, the first general high-performance self-supervised algorithm for speech, vision, and text. We applied it to different modalities and found it matches or outperforms the best self-supervised algorithms. We hope this brings us closer to a world where computers can learn to solve many different tasks without supervision. Learn more and get the code:  https://ai.facebook.com/â€¦/the-first-high-performance-self-sâ€¦",2022-01-20T22:43:35,,https://scontent-bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/272147088_2024182621092014_6532581039236849529_n.jpg?_nc_cat=100&ccb=1-5&_nc_sid=8024bb&_nc_ohc=j4_1PAndJTIAX82OLNq&_nc_ht=scontent-bom1-2.xx&oh=00_AT9us__TvC9eYBqRyQEwEtYSit9r2UKYg0gFoRK7Efrhyw&oe=61F17B71,https://www.facebook.com/MetaAI/photos/a.360372474139712/2024182624425347/?type=3&__xts__%5B0%5D=68.ARAse4eiZmZQDOZumNZEDR0tQkE5B6g50K6S66JJPccb-KaWJWg6Yz4v19BQFSZRMd04MeBmV24VqvqMB3oyjAwMDJUtpmgkMiITtSP8HOgy8QEx_vFlq1j-UEImZkzeEgSAJYINndnR5aSQn0GUwL54L3x2BsxEqL1lElL7SnHfTVvIFUDyNfAqUWIsXrkI8X5KjoDchUj7aHRga1HB5EE0x60dZcHogUMb1sJDRmKCcx8xisRgk5XzdZKCQDDdEkUqN-Ch9_NYTMtxlchz1KfR0w9wRt8y9l7E7BNhfLrmm4qyxo-ZpA&__tn__=-R
 ...
 ```
 
 <br>
 
 <hr>
 <br>
```

#### html2text {}

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.0 Summary:
+Python package to scrap facebook's pages front end with no limitations Home-
+page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
+Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
+scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
+Beta Classifier: Environment :: Console Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Science/Research Classifier:
+Natural Language :: English Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
+MacOS Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.6 Description-
+Content-Type: text/markdown License-File: LICENSE
 ****** Facebook Page Scraper ******
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https:/
 /github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity) [!
 [PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://
 opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/
 python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 No need of API key, No limitation on number of requests. Import the library and
@@ -40,50 +57,47 @@
 ```python #import Facebook_scraper class from facebook_page_scraper from
 facebook_page_scraper import Facebook_scraper #instantiate the Facebook_scraper
 class page_name = "metaai" posts_count = 10 browser = "firefox" proxy = "IP:
 PORT" #if proxy requires authentication then user:password@IP:PORT timeout =
 600 #600 seconds headless = True meta_ai = Facebook_scraper(page_name,
 posts_count, browser, proxy=proxy, timeout=timeout, headless=headless) ```
 **** Parameters for Facebook_scraper(page_name, posts_count, browser, proxy,
-timeout, headless, browser_profile) class ****
+timeout, headless) class ****
 Parameter Name  Parameter Type Description
 page_name       String         Name of the facebook page
 posts_count     Integer        Number of posts to scrap, if not passed default
                                is 10
 browser         String         Which browser to use, either chrome or firefox.
                                if not passed,default is chrome
                                Optional argument, if user wants to set proxy,
 proxy(optional) String         if proxy requires authentication then the format
                                will be user:password@IP:PORT
                                The maximum amount of time the bot should run
 timeout         Integer        for. If not passed, the default timeout is set
                                to 10 minutes
 headless        Boolean        Whether to run browser in headless mode?.
                                Default is True
-                               Path to the browser profile where cookies are
-browser_profile String         stored and can be used for scraping data in an
-                               authenticated way.
 
 ===============================================================================
 
 **** Done with instantiation?. Let the scraping begin! ****
 
 **** For post's data in JSON format: ****
 ```python #call the scrap_to_json() method json_data = meta_ai.scrap_to_json()
 print(json_data) ``` Output: ```javascript { "2024182624425347": { "name":
 "Meta AI", "shares": 0, "reactions": { "likes": 154, "loves": 19, "wow": 0,
 "cares": 0, "sad": 0, "angry": 0, "haha": 0 }, "reaction_count": 173,
-"comments": 2, "content": "Weâve built data2vec, the first general high-
+"comments": 2, "content": "WeÃ¢â¬â¢ve built data2vec, the first general high-
 performance self-supervised algorithm for speech, vision, and text. We applied
 it to different modalities and found it matches or outperforms the best self-
 supervised algorithms. We hope this brings us closer to a world where computers
 can learn to solve many different tasks without supervision. Learn more and get
-the code: https://ai.facebook.com/â¦/the-first-high-performance-self-sâ¦",
-"posted_on": "2022-01-20T22:43:35", "video": [], "image": [ "https://scontent-
-bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/
+the code: https://ai.facebook.com/Ã¢â¬Â¦/the-first-high-performance-self-
+sÃ¢â¬Â¦", "posted_on": "2022-01-20T22:43:35", "video": [], "image": [ "https:/
+/scontent-bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/
 272147088_2024182621092014_6532581039236849529_n.jpg?_nc_cat=100&ccb=1-
 5&_nc_sid=8024bb&_nc_ohc=j4_1PAndJTIAX82OLNq&_nc_ht=scontent-bom1-
 2.xx&oh=00_AT9us__TvC9eYBqRyQEwEtYSit9r2UKYg0gFoRK7Efrhyw&oe=61F17B71" ],
 "post_url": "https://www.facebook.com/MetaAI/photos/a.360372474139712/
 2024182624425347/?type=3&__xts__%5B0%5D=68.ARBoSaQ-pAC_ApucZNHZ6R-
 BI3YUSjH4sXsfdZRQ2zZFOwgWGhjt6dmg0VOcmGCLhSFyXpecOY9g1A94vrzU_T-
 GtYFagqDkJjHuhoyPW2vnkn7fvfzx-
@@ -102,22 +116,22 @@
 
 **** For saving post's data directly to CSV file ****
 ``` python #call scrap_to_csv(filename,directory) method filename = "data_file"
 #file name without CSV extension,where data will be saved directory = "E:\data"
 #directory where CSV file will be saved meta_ai.scrap_to_csv(filename,
 directory) ``` content of ```data_file.csv```: ```csv
 id,name,shares,likes,loves,wow,cares,sad,angry,haha,reactions_count,comments,content,posted_on,video,image,post_url
-2024182624425347,Meta AI,0,154,19,0,0,0,0,0,173,2,"Weâve built data2vec, the
-first general high-performance self-supervised algorithm for speech, vision,
-and text. We applied it to different modalities and found it matches or
+2024182624425347,Meta AI,0,154,19,0,0,0,0,0,173,2,"WeÃ¢â¬â¢ve built data2vec,
+the first general high-performance self-supervised algorithm for speech,
+vision, and text. We applied it to different modalities and found it matches or
 outperforms the best self-supervised algorithms. We hope this brings us closer
 to a world where computers can learn to solve many different tasks without
-supervision. Learn more and get the code: https://ai.facebook.com/â¦/the-
-first-high-performance-self-sâ¦",2022-01-20T22:43:35,,https://scontent-bom1-
-2.xx.fbcdn.net/v/t39.30808-6/s480x480/
+supervision. Learn more and get the code: https://ai.facebook.com/Ã¢â¬Â¦/the-
+first-high-performance-self-sÃ¢â¬Â¦",2022-01-20T22:43:35,,https://scontent-
+bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/
 272147088_2024182621092014_6532581039236849529_n.jpg?_nc_cat=100&ccb=1-
 5&_nc_sid=8024bb&_nc_ohc=j4_1PAndJTIAX82OLNq&_nc_ht=scontent-bom1-
 2.xx&oh=00_AT9us__TvC9eYBqRyQEwEtYSit9r2UKYg0gFoRK7Efrhyw&oe=61F17B71,https://
 www.facebook.com/MetaAI/photos/a.360372474139712/2024182624425347/
 ?type=3&__xts__%5B0%5D=68.ARAse4eiZmZQDOZumNZEDR0tQkE5B6g50K6S66JJPccb-
 KaWJWg6Yz4v19BQFSZRMd04MeBmV24VqvqMB3oyjAwMDJUtpmgkMiITtSP8HOgy8QEx_vFlq1j-
 UEImZkzeEgSAJYINndnR5aSQn0GUwL54L3x2BsxEqL1lElL7SnHfTVvIFUDyNfAqUWIsXrkI8X5KjoDchUj7aHRga1HB5EE0x60dZcHogUMb1sJDRmKCcx8xisRgk5XzdZKCQDDdEkUqN-
```

### Comparing `facebook_page_scraper-4.0.3/facebook_page_scraper/driver_initialization.py` & `facebook_page_scraper-5.0.0/facebook_page_scraper/driver_initialization.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,35 +15,24 @@
 ch = logging.StreamHandler()
 ch.setFormatter(format)
 logger.addHandler(ch)
 
 
 class Initializer:
 
-    def __init__(self, browser_name, proxy=None, headless=True, profile=None):
+    def __init__(self, browser_name, proxy=None, headless=True):
         self.browser_name = browser_name
         self.proxy = proxy
         self.headless = headless
-        self.profile = profile
 
     def set_properties(self, browser_option):
         """adds capabilities to the driver"""
         if self.headless:
             browser_option.add_argument(
                 '--headless')  # runs browser in headless mode
-        if self.profile and self.browser_name.lower() == "chrome":
-            logger.setLevel(logging.INFO)
-            logger.info("Loading Profile from {}".format(self.profile))
-            browser_option.add_argument(
-                "user-data-dir={}".format(self.profile))
-        if self.profile and self.browser_name.lower() == "firefox":
-            logger.setLevel(logging.INFO)
-            logger.info("Loading Profile from {}".format(self.profile))
-            browser_option.add_argument("-profile")
-            browser_option.add_argument(self.profile)
         browser_option.add_argument('--no-sandbox')
         browser_option.add_argument("--disable-dev-shm-usage")
         browser_option.add_argument('--ignore-certificate-errors')
         browser_option.add_argument('--disable-gpu')
         browser_option.add_argument('--log-level=3')
         browser_option.add_argument('--disable-notifications')
         browser_option.add_argument('--disable-popup-blocking')
```

### Comparing `facebook_page_scraper-4.0.3/facebook_page_scraper/driver_utilities.py` & `facebook_page_scraper-5.0.0/facebook_page_scraper/driver_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,7 +164,18 @@
             pass
         except AttributeError:
             pass
         except IndexError:
             pass
         except Exception as ex:
             logger.exception("Error at click_see_more method : {}".format(ex))
+
+    @staticmethod
+    def __close_cookie_consent_modern_layout(driver):
+        # To avoid the cookie consent prompt
+        try:
+          allow_span = driver.find_element(
+             By.XPATH, '//div[contains(@aria-label, "Allow")]/../following-sibling::div')
+          allow_span.click()
+        except Exception as ex:
+            #if not found, that's fine silently just log thing do not stop
+            logger.info('The Cookie Consent Prompt was not found!: ', ex)
```

### Comparing `facebook_page_scraper-4.0.3/facebook_page_scraper/element_finder.py` & `facebook_page_scraper-5.0.0/facebook_page_scraper/element_finder.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-4.0.3/facebook_page_scraper/scraper.py` & `facebook_page_scraper-5.0.0/facebook_page_scraper/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,66 +13,67 @@
 format = logging.Formatter(
     "%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch = logging.StreamHandler()
 ch.setFormatter(format)
 logger.addHandler(ch)
 
 class Facebook_scraper:
-    __data_dict = {}  # this dictionary stores all post's data
 
     # when we scroll and extract all posts,it may happens that we extract same posts over and over,so this lead to too much iteration
     # and waste time to iterate over and over the same post, to solve that,
     # problem I needed a data structure which
     # 1) removes duplicates from itself automatically,
     # 2) provides search of element,
     # 3) compatible with list's unpacking to quickly add element inside itself from list
     #  set() seems to be doing the work properly
 
-    # __extracted_post contains all the post's ID that have been scraped before and as it set() it avoids post's ID duplication.
-    __extracted_post = set()
-
     # condition,
     # 1) if we reach bottom of the page and post is not longer available, and we don't meet the number of posts that we need to find
     # 2) if we were given wrong page_name, and it does not exists in fb than no post will exist.
     # with above condition being true, the crawler will keep on scrolling the page to find posts
     # and it will stuck in infinite loop, which may cause machine to crash
     # to solve the problem, I have declared a class member "retry",assigned it value 10.
     # it checks 'retry' times if posts does not exists.
     # __no_post_found method subtracts -1 every time the if post is not found.
     # on each iteration __close_after_retry is called to check if retry have turned to 0
     # if it returns true,it will break the loop. After coming out of loop,driver will be closed and it will return post whatever was found
 
-    def __init__(self, page_name, posts_count=10, browser="chrome", proxy=None, timeout=600, headless=True, browser_profile=None):
+    def __init__(self, page_name, posts_count=10, browser="chrome", proxy=None, timeout=600, headless=True):
         self.page_name = page_name
         self.posts_count = int(posts_count)
         #self.URL = "https://en-gb.facebook.com/pg/{}/posts".format(self.page_name)
         self.URL = "https://facebook.com/{}".format(self.page_name)
         self.browser = browser
         self.__driver = ''
         self.proxy = proxy
         self.__layout = ''
         self.timeout = timeout
         self.headless = headless
-        self.browser_profile = browser_profile
+        self.__data_dict = {}  # this dictionary stores all post's data
+        # __extracted_post contains all the post's ID that have been scraped before and as it set() it avoids post's ID duplication.
+        self.__extracted_post = set()
 
     def __start_driver(self):
         """changes the class member __driver value to driver on call"""
         self.__driver = Initializer(
-            self.browser, self.proxy, self.headless, self.browser_profile).init()
+            self.browser, self.proxy, self.headless).init()
 
     def __handle_popup(self, layout):
         # while scrolling, wait for login popup to show, it can be skipped by clicking "Not Now" button
         try:
             if layout == "old":
                 # if during scrolling any of error or signup popup shows
                 Utilities._Utilities__close_error_popup(self.__driver)
                 Utilities._Utilities__close_popup(self.__driver)
             elif layout == "new":
                 Utilities._Utilities__close_modern_layout_signup_modal(
                     self.__driver)
+                Utilities._Utilities__close_cookie_consent_modern_layout(
+                    self.__driver)
+
         except Exception as ex:
             logger.exception("Error at handle_popup : {}".format(ex))
 
     def __check_timeout(self, start_time, current_time):
         return (current_time-start_time) > self.timeout
 
     def scrap_to_json(self):
```

### Comparing `facebook_page_scraper-4.0.3/facebook_page_scraper/scraping_utilities.py` & `facebook_page_scraper-5.0.0/facebook_page_scraper/scraping_utilities.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-4.0.3/facebook_page_scraper.egg-info/PKG-INFO` & `facebook_page_scraper-5.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: facebook-page-scraper
-Version: 4.0.3
-Summary: Python package to scrap facebook's pages front end with no limitations
-Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
-Author: Sajid Shaikh
-Author-email: shaikhsajid3732@gmail.com
-License: MIT
-Keywords: web-scraping selenium facebook facebook-pages
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1> Facebook Page Scraper </h1>
 
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https://github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity)
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 
 <p> No need of API key, No limitation on number of requests. Import the library and <b> Just Do It !<b> </p>
 
@@ -118,15 +88,15 @@
 proxy = "IP:PORT" #if proxy requires authentication then user:password@IP:PORT
 timeout = 600 #600 seconds
 headless = True
 meta_ai = Facebook_scraper(page_name, posts_count, browser, proxy=proxy, timeout=timeout, headless=headless)
 
 ```
 
-<h3 id="scraperParameters"> Parameters for  <code>Facebook_scraper(page_name, posts_count, browser, proxy, timeout, headless, browser_profile) </code> class </h3>
+<h3 id="scraperParameters"> Parameters for  <code>Facebook_scraper(page_name, posts_count, browser, proxy, timeout, headless) </code> class </h3>
 <table>
 <th>
 <tr>
 <td> Parameter Name </td>
 <td> Parameter Type </td>
 <td> Description </td>
 </tr>
@@ -200,25 +170,14 @@
 </td>
 <td>
 Whether to run browser in headless mode?. Default is True
  </code>
 </td>
 </tr>
 
-<tr>
-<td>
-browser_profile
-</td>
-<td>
-String
-</td>
-<td>
-Path to the browser profile where cookies are stored and can be used for scraping data in an authenticated way.
-</td>
-</tr>
 
 </table>
 <br>
 <hr>
 <br>
 
 <h3> Done with instantiation?. <b>Let the scraping begin!</b> </h3>
@@ -250,15 +209,15 @@
       "cares": 0,
       "sad": 0,
       "angry": 0,
       "haha": 0
     },
     "reaction_count": 173,
     "comments": 2,
-    "content": "Weâ€™ve built data2vec, the first general high-performance self-supervised algorithm for speech, vision, and text. We applied it to different modalities and found it matches or outperforms the best self-supervised algorithms. We hope this brings us closer to a world where computers can learn to solve many different tasks without supervision. Learn more and get the code:  https://ai.facebook.com/â€¦/the-first-high-performance-self-sâ€¦",
+    "content": "We’ve built data2vec, the first general high-performance self-supervised algorithm for speech, vision, and text. We applied it to different modalities and found it matches or outperforms the best self-supervised algorithms. We hope this brings us closer to a world where computers can learn to solve many different tasks without supervision. Learn more and get the code:  https://ai.facebook.com/…/the-first-high-performance-self-s…",
     "posted_on": "2022-01-20T22:43:35",
     "video": [],
     "image": [
       "https://scontent-bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/272147088_2024182621092014_6532581039236849529_n.jpg?_nc_cat=100&ccb=1-5&_nc_sid=8024bb&_nc_ohc=j4_1PAndJTIAX82OLNq&_nc_ht=scontent-bom1-2.xx&oh=00_AT9us__TvC9eYBqRyQEwEtYSit9r2UKYg0gFoRK7Efrhyw&oe=61F17B71"
     ],
     "post_url": "https://www.facebook.com/MetaAI/photos/a.360372474139712/2024182624425347/?type=3&__xts__%5B0%5D=68.ARBoSaQ-pAC_ApucZNHZ6R-BI3YUSjH4sXsfdZRQ2zZFOwgWGhjt6dmg0VOcmGCLhSFyXpecOY9g1A94vrzU_T-GtYFagqDkJjHuhoyPW2vnkn7fvfzx-ql7fsBYxL5DgQVSsiC1cPoycdCvHmi6BV5Sc4fKADdgDhdFvVvr-ttzXG1ng2DbLzU-XfSes7SAnrPs-gxjODPKJ7AdqkqkSQJ4HrsLgxMgcLFdCsE6feWL7rXjptVWegMVMthhJNVqO0JHu986XBfKKqB60aBFvyAzTSEwJD6o72GtnyzQ-BcH7JxmLtb2_A&__tn__=-R"
   }, ...
@@ -310,15 +269,15 @@
 meta_ai.scrap_to_csv(filename, directory)
 
 ```
 
 content of ```data_file.csv```:
 ```csv
 id,name,shares,likes,loves,wow,cares,sad,angry,haha,reactions_count,comments,content,posted_on,video,image,post_url
-2024182624425347,Meta AI,0,154,19,0,0,0,0,0,173,2,"Weâ€™ve built data2vec, the first general high-performance self-supervised algorithm for speech, vision, and text. We applied it to different modalities and found it matches or outperforms the best self-supervised algorithms. We hope this brings us closer to a world where computers can learn to solve many different tasks without supervision. Learn more and get the code:  https://ai.facebook.com/â€¦/the-first-high-performance-self-sâ€¦",2022-01-20T22:43:35,,https://scontent-bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/272147088_2024182621092014_6532581039236849529_n.jpg?_nc_cat=100&ccb=1-5&_nc_sid=8024bb&_nc_ohc=j4_1PAndJTIAX82OLNq&_nc_ht=scontent-bom1-2.xx&oh=00_AT9us__TvC9eYBqRyQEwEtYSit9r2UKYg0gFoRK7Efrhyw&oe=61F17B71,https://www.facebook.com/MetaAI/photos/a.360372474139712/2024182624425347/?type=3&__xts__%5B0%5D=68.ARAse4eiZmZQDOZumNZEDR0tQkE5B6g50K6S66JJPccb-KaWJWg6Yz4v19BQFSZRMd04MeBmV24VqvqMB3oyjAwMDJUtpmgkMiITtSP8HOgy8QEx_vFlq1j-UEImZkzeEgSAJYINndnR5aSQn0GUwL54L3x2BsxEqL1lElL7SnHfTVvIFUDyNfAqUWIsXrkI8X5KjoDchUj7aHRga1HB5EE0x60dZcHogUMb1sJDRmKCcx8xisRgk5XzdZKCQDDdEkUqN-Ch9_NYTMtxlchz1KfR0w9wRt8y9l7E7BNhfLrmm4qyxo-ZpA&__tn__=-R
+2024182624425347,Meta AI,0,154,19,0,0,0,0,0,173,2,"We’ve built data2vec, the first general high-performance self-supervised algorithm for speech, vision, and text. We applied it to different modalities and found it matches or outperforms the best self-supervised algorithms. We hope this brings us closer to a world where computers can learn to solve many different tasks without supervision. Learn more and get the code:  https://ai.facebook.com/…/the-first-high-performance-self-s…",2022-01-20T22:43:35,,https://scontent-bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/272147088_2024182621092014_6532581039236849529_n.jpg?_nc_cat=100&ccb=1-5&_nc_sid=8024bb&_nc_ohc=j4_1PAndJTIAX82OLNq&_nc_ht=scontent-bom1-2.xx&oh=00_AT9us__TvC9eYBqRyQEwEtYSit9r2UKYg0gFoRK7Efrhyw&oe=61F17B71,https://www.facebook.com/MetaAI/photos/a.360372474139712/2024182624425347/?type=3&__xts__%5B0%5D=68.ARAse4eiZmZQDOZumNZEDR0tQkE5B6g50K6S66JJPccb-KaWJWg6Yz4v19BQFSZRMd04MeBmV24VqvqMB3oyjAwMDJUtpmgkMiITtSP8HOgy8QEx_vFlq1j-UEImZkzeEgSAJYINndnR5aSQn0GUwL54L3x2BsxEqL1lElL7SnHfTVvIFUDyNfAqUWIsXrkI8X5KjoDchUj7aHRga1HB5EE0x60dZcHogUMb1sJDRmKCcx8xisRgk5XzdZKCQDDdEkUqN-Ch9_NYTMtxlchz1KfR0w9wRt8y9l7E7BNhfLrmm4qyxo-ZpA&__tn__=-R
 ...
 ```
 
 <br>
 
 <hr>
 <br>
```

#### html2text {}

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1 Name: facebook-page-scraper Version: 4.0.3 Summary:
-Python package to scrap facebook's pages front end with no limitations Home-
-page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
-Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
-scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
-Beta Classifier: Environment :: Console Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Science/Research Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
-MacOS Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE
 ****** Facebook Page Scraper ******
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https:/
 /github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity) [!
 [PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://
 opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/
 python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 No need of API key, No limitation on number of requests. Import the library and
@@ -57,50 +40,47 @@
 ```python #import Facebook_scraper class from facebook_page_scraper from
 facebook_page_scraper import Facebook_scraper #instantiate the Facebook_scraper
 class page_name = "metaai" posts_count = 10 browser = "firefox" proxy = "IP:
 PORT" #if proxy requires authentication then user:password@IP:PORT timeout =
 600 #600 seconds headless = True meta_ai = Facebook_scraper(page_name,
 posts_count, browser, proxy=proxy, timeout=timeout, headless=headless) ```
 **** Parameters for Facebook_scraper(page_name, posts_count, browser, proxy,
-timeout, headless, browser_profile) class ****
+timeout, headless) class ****
 Parameter Name  Parameter Type Description
 page_name       String         Name of the facebook page
 posts_count     Integer        Number of posts to scrap, if not passed default
                                is 10
 browser         String         Which browser to use, either chrome or firefox.
                                if not passed,default is chrome
                                Optional argument, if user wants to set proxy,
 proxy(optional) String         if proxy requires authentication then the format
                                will be user:password@IP:PORT
                                The maximum amount of time the bot should run
 timeout         Integer        for. If not passed, the default timeout is set
                                to 10 minutes
 headless        Boolean        Whether to run browser in headless mode?.
                                Default is True
-                               Path to the browser profile where cookies are
-browser_profile String         stored and can be used for scraping data in an
-                               authenticated way.
 
 ===============================================================================
 
 **** Done with instantiation?. Let the scraping begin! ****
 
 **** For post's data in JSON format: ****
 ```python #call the scrap_to_json() method json_data = meta_ai.scrap_to_json()
 print(json_data) ``` Output: ```javascript { "2024182624425347": { "name":
 "Meta AI", "shares": 0, "reactions": { "likes": 154, "loves": 19, "wow": 0,
 "cares": 0, "sad": 0, "angry": 0, "haha": 0 }, "reaction_count": 173,
-"comments": 2, "content": "WeÃ¢â¬â¢ve built data2vec, the first general high-
+"comments": 2, "content": "Weâve built data2vec, the first general high-
 performance self-supervised algorithm for speech, vision, and text. We applied
 it to different modalities and found it matches or outperforms the best self-
 supervised algorithms. We hope this brings us closer to a world where computers
 can learn to solve many different tasks without supervision. Learn more and get
-the code: https://ai.facebook.com/Ã¢â¬Â¦/the-first-high-performance-self-
-sÃ¢â¬Â¦", "posted_on": "2022-01-20T22:43:35", "video": [], "image": [ "https:/
-/scontent-bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/
+the code: https://ai.facebook.com/â¦/the-first-high-performance-self-sâ¦",
+"posted_on": "2022-01-20T22:43:35", "video": [], "image": [ "https://scontent-
+bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/
 272147088_2024182621092014_6532581039236849529_n.jpg?_nc_cat=100&ccb=1-
 5&_nc_sid=8024bb&_nc_ohc=j4_1PAndJTIAX82OLNq&_nc_ht=scontent-bom1-
 2.xx&oh=00_AT9us__TvC9eYBqRyQEwEtYSit9r2UKYg0gFoRK7Efrhyw&oe=61F17B71" ],
 "post_url": "https://www.facebook.com/MetaAI/photos/a.360372474139712/
 2024182624425347/?type=3&__xts__%5B0%5D=68.ARBoSaQ-pAC_ApucZNHZ6R-
 BI3YUSjH4sXsfdZRQ2zZFOwgWGhjt6dmg0VOcmGCLhSFyXpecOY9g1A94vrzU_T-
 GtYFagqDkJjHuhoyPW2vnkn7fvfzx-
@@ -119,22 +99,22 @@
 
 **** For saving post's data directly to CSV file ****
 ``` python #call scrap_to_csv(filename,directory) method filename = "data_file"
 #file name without CSV extension,where data will be saved directory = "E:\data"
 #directory where CSV file will be saved meta_ai.scrap_to_csv(filename,
 directory) ``` content of ```data_file.csv```: ```csv
 id,name,shares,likes,loves,wow,cares,sad,angry,haha,reactions_count,comments,content,posted_on,video,image,post_url
-2024182624425347,Meta AI,0,154,19,0,0,0,0,0,173,2,"WeÃ¢â¬â¢ve built data2vec,
-the first general high-performance self-supervised algorithm for speech,
-vision, and text. We applied it to different modalities and found it matches or
+2024182624425347,Meta AI,0,154,19,0,0,0,0,0,173,2,"Weâve built data2vec, the
+first general high-performance self-supervised algorithm for speech, vision,
+and text. We applied it to different modalities and found it matches or
 outperforms the best self-supervised algorithms. We hope this brings us closer
 to a world where computers can learn to solve many different tasks without
-supervision. Learn more and get the code: https://ai.facebook.com/Ã¢â¬Â¦/the-
-first-high-performance-self-sÃ¢â¬Â¦",2022-01-20T22:43:35,,https://scontent-
-bom1-2.xx.fbcdn.net/v/t39.30808-6/s480x480/
+supervision. Learn more and get the code: https://ai.facebook.com/â¦/the-
+first-high-performance-self-sâ¦",2022-01-20T22:43:35,,https://scontent-bom1-
+2.xx.fbcdn.net/v/t39.30808-6/s480x480/
 272147088_2024182621092014_6532581039236849529_n.jpg?_nc_cat=100&ccb=1-
 5&_nc_sid=8024bb&_nc_ohc=j4_1PAndJTIAX82OLNq&_nc_ht=scontent-bom1-
 2.xx&oh=00_AT9us__TvC9eYBqRyQEwEtYSit9r2UKYg0gFoRK7Efrhyw&oe=61F17B71,https://
 www.facebook.com/MetaAI/photos/a.360372474139712/2024182624425347/
 ?type=3&__xts__%5B0%5D=68.ARAse4eiZmZQDOZumNZEDR0tQkE5B6g50K6S66JJPccb-
 KaWJWg6Yz4v19BQFSZRMd04MeBmV24VqvqMB3oyjAwMDJUtpmgkMiITtSP8HOgy8QEx_vFlq1j-
 UEImZkzeEgSAJYINndnR5aSQn0GUwL54L3x2BsxEqL1lElL7SnHfTVvIFUDyNfAqUWIsXrkI8X5KjoDchUj7aHRga1HB5EE0x60dZcHogUMb1sJDRmKCcx8xisRgk5XzdZKCQDDdEkUqN-
```

### Comparing `facebook_page_scraper-4.0.3/setup.py` & `facebook_page_scraper-5.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                 'webdriver-manager==3.2.2',
                 'selenium-wire==4.3.1',
                 'python-dateutil==2.8.2']
 
 
 setuptools.setup(
     name="facebook_page_scraper",
-    version="4.0.3",
+    version="5.0.0",
     author="Sajid Shaikh",
     author_email="shaikhsajid3732@gmail.com",
     description="Python package to scrap facebook's pages front end with no limitations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/shaikhsajid1111/facebook_page_scraper",
```

