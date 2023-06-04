# Comparing `tmp/twitter_scraper_selenium-4.1.4.tar.gz` & `tmp/twitter_scraper_selenium-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_scraper_selenium-4.1.4.tar", last modified: Sat Jan 14 10:04:20 2023, max compression
+gzip compressed data, was "twitter_scraper_selenium-4.1.5.tar", last modified: Sun Jun  4 10:25:57 2023, max compression
```

## Comparing `twitter_scraper_selenium-4.1.4.tar` & `twitter_scraper_selenium-4.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-01-14 10:04:20.470622 twitter_scraper_selenium-4.1.4/
--rw-rw-rw-   0        0        0     1090 2022-04-14 08:00:26.000000 twitter_scraper_selenium-4.1.4/LICENSE
--rw-rw-rw-   0        0        0       17 2022-04-13 11:49:45.000000 twitter_scraper_selenium-4.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0    38653 2023-01-14 10:04:20.469614 twitter_scraper_selenium-4.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    37224 2022-12-31 06:12:21.000000 twitter_scraper_selenium-4.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-01-14 10:04:20.470622 twitter_scraper_selenium-4.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1899 2023-01-14 09:52:29.000000 twitter_scraper_selenium-4.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-14 10:04:20.338100 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/
--rw-rw-rw-   0        0        0      790 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/__init__.py
--rw-rw-rw-   0        0        0     5458 2022-10-09 08:22:29.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/driver_initialization.py
--rw-rw-rw-   0        0        0     2225 2022-10-09 08:22:29.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/driver_utils.py
--rw-rw-rw-   0        0        0     8412 2022-10-26 11:52:32.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/element_finder.py
--rw-rw-rw-   0        0        0    12582 2022-12-31 05:52:11.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/keyword.py
--rw-rw-rw-   0        0        0     5253 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/keyword_api.py
--rw-rw-rw-   0        0        0    10869 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/profile.py
--rw-rw-rw-   0        0        0     8395 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/profile_api.py
--rw-rw-rw-   0        0        0     3328 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/profile_details.py
--rw-rw-rw-   0        0        0    12117 2023-01-14 09:53:50.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/scraping_utilities.py
--rw-rw-rw-   0        0        0     3149 2022-12-03 03:44:52.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/topic.py
--rw-rw-rw-   0        0        0     7113 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/topic_api.py
-drwxrwxrwx   0        0        0        0 2023-01-14 10:04:20.468632 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium.egg-info/
--rw-rw-rw-   0        0        0    38653 2023-01-14 10:04:18.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-01-14 10:04:18.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-14 10:04:18.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-01-14 10:04:18.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-01-14 10:04:18.000000 twitter_scraper_selenium-4.1.4/twitter_scraper_selenium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 10:25:57.513852 twitter_scraper_selenium-4.1.5/
+-rw-rw-rw-   0        0        0     1090 2022-04-14 08:00:26.000000 twitter_scraper_selenium-4.1.5/LICENSE
+-rw-rw-rw-   0        0        0       17 2022-04-13 11:49:45.000000 twitter_scraper_selenium-4.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    38653 2023-06-04 10:25:57.428186 twitter_scraper_selenium-4.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    37224 2022-12-31 06:12:21.000000 twitter_scraper_selenium-4.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 10:25:57.513852 twitter_scraper_selenium-4.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1899 2023-06-04 10:25:07.000000 twitter_scraper_selenium-4.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 10:25:57.407183 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/
+-rw-rw-rw-   0        0        0      790 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/__init__.py
+-rw-rw-rw-   0        0        0     5458 2022-10-09 08:22:29.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/driver_initialization.py
+-rw-rw-rw-   0        0        0     2225 2022-10-09 08:22:29.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/driver_utils.py
+-rw-rw-rw-   0        0        0     8411 2023-06-04 10:20:40.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/element_finder.py
+-rw-rw-rw-   0        0        0    12582 2022-12-31 05:52:11.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/keyword.py
+-rw-rw-rw-   0        0        0     5253 2023-02-25 05:15:49.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/keyword_api.py
+-rw-rw-rw-   0        0        0    10869 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/profile.py
+-rw-rw-rw-   0        0        0     8395 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/profile_api.py
+-rw-rw-rw-   0        0        0     3328 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/profile_details.py
+-rw-rw-rw-   0        0        0    12117 2023-06-04 10:23:40.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/scraping_utilities.py
+-rw-rw-rw-   0        0        0     3149 2022-12-03 03:44:52.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/topic.py
+-rw-rw-rw-   0        0        0     7113 2022-12-31 05:58:42.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/topic_api.py
+drwxrwxrwx   0        0        0        0 2023-06-04 10:25:57.426187 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium.egg-info/
+-rw-rw-rw-   0        0        0    38653 2023-06-04 10:25:57.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-06-04 10:25:57.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 10:25:57.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-06-04 10:25:57.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-04 10:25:57.000000 twitter_scraper_selenium-4.1.5/twitter_scraper_selenium.egg-info/top_level.txt
```

### Comparing `twitter_scraper_selenium-4.1.4/LICENSE` & `twitter_scraper_selenium-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/PKG-INFO` & `twitter_scraper_selenium-4.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter_scraper_selenium
-Version: 4.1.4
+Version: 4.1.5
 Summary: Python package to scrap twitter's front-end easily with selenium
 Home-page: https://github.com/shaikhsajid1111/twitter-scraper-selenium
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium social media twitter keyword twitter-profile twitter-keywords automation json csv twitter-hashtag hashtag
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twitter_scraper_selenium Version: 4.1.4 Summary:
+Metadata-Version: 2.1 Name: twitter_scraper_selenium Version: 4.1.5 Summary:
 Python package to scrap twitter's front-end easily with selenium Home-page:
 https://github.com/shaikhsajid1111/twitter-scraper-selenium Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium social media twitter keyword twitter-profile twitter-keywords
 automation json csv twitter-hashtag hashtag Classifier: Development Status :: 4
 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
```

### Comparing `twitter_scraper_selenium-4.1.4/README.md` & `twitter_scraper_selenium-4.1.5/README.md`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/setup.py` & `twitter_scraper_selenium-4.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 
 setuptools.setup(
     name="twitter_scraper_selenium",
-    version="4.1.4",
+    version="4.1.5",
     author="Sajid Shaikh",
     author_email="shaikhsajid3732@gmail.com",
     description="Python package to scrap twitter's front-end easily with selenium",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/shaikhsajid1111/twitter-scraper-selenium",
```

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/__init__.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/driver_initialization.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/driver_initialization.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/driver_utils.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/driver_utils.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/element_finder.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/element_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         """finds the name from the post"""
         try:
             name = "NA"
             anchors = Finder.find_all_anchor_tags(tweet)
             if len(anchors) > 2:
                 if is_retweet:
                     name = tweet.find_element(
-                        By.CSS_SELECTOR, '[data-testid="User-Names"] > div a').text
+                        By.CSS_SELECTOR, '[data-testid="User-Name"] > div a').text
                 else:
                     name = anchors[1].text.split("\n")[0]
             return name
         except Exception as ex:
             logger.exception(
                 "Error at method find_name_from_post : {}".format(ex))
```

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/keyword.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/keyword.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/keyword_api.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/keyword_api.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/profile.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/profile.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/profile_api.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/profile_api.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/profile_details.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/profile_details.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/scraping_utilities.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/scraping_utilities.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/topic.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/topic.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium/topic_api.py` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium/topic_api.py`

 * *Files identical despite different names*

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium.egg-info/PKG-INFO` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-scraper-selenium
-Version: 4.1.4
+Version: 4.1.5
 Summary: Python package to scrap twitter's front-end easily with selenium
 Home-page: https://github.com/shaikhsajid1111/twitter-scraper-selenium
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium social media twitter keyword twitter-profile twitter-keywords automation json csv twitter-hashtag hashtag
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: twitter-scraper-selenium Version: 4.1.4 Summary:
+Metadata-Version: 2.1 Name: twitter-scraper-selenium Version: 4.1.5 Summary:
 Python package to scrap twitter's front-end easily with selenium Home-page:
 https://github.com/shaikhsajid1111/twitter-scraper-selenium Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium social media twitter keyword twitter-profile twitter-keywords
 automation json csv twitter-hashtag hashtag Classifier: Development Status :: 4
 - Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
```

### Comparing `twitter_scraper_selenium-4.1.4/twitter_scraper_selenium.egg-info/SOURCES.txt` & `twitter_scraper_selenium-4.1.5/twitter_scraper_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

