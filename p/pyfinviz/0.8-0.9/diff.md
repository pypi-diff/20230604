# Comparing `tmp/pyfinviz-0.8.tar.gz` & `tmp/pyfinviz-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfinviz-0.8.tar", last modified: Sun Oct  2 01:56:23 2022, max compression
+gzip compressed data, was "pyfinviz-0.9.tar", last modified: Fri Oct  7 15:53:55 2022, max compression
```

## Comparing `pyfinviz-0.8.tar` & `pyfinviz-0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-10-02 01:56:23.356400 pyfinviz-0.8/
--rw-rw-rw-   0        0        0      563 2022-09-08 14:06:27.000000 pyfinviz-0.8/LICENSE.txt
--rw-rw-rw-   0        0        0    10393 2022-10-02 01:56:23.357400 pyfinviz-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     9443 2022-09-08 14:06:27.000000 pyfinviz-0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-02 01:56:23.338395 pyfinviz-0.8/pyfinviz/
--rw-rw-rw-   0        0        0      216 2022-09-08 14:06:27.000000 pyfinviz-0.8/pyfinviz/__init__.py
--rw-rw-rw-   0        0        0      639 2022-09-08 14:06:27.000000 pyfinviz-0.8/pyfinviz/crypto.py
--rw-rw-rw-   0        0        0     1420 2022-09-08 22:39:28.000000 pyfinviz-0.8/pyfinviz/groups.py
--rw-rw-rw-   0        0        0      736 2022-09-08 14:06:27.000000 pyfinviz-0.8/pyfinviz/insider.py
--rw-rw-rw-   0        0        0      993 2022-09-08 14:55:13.000000 pyfinviz-0.8/pyfinviz/news.py
--rw-rw-rw-   0        0        0     5300 2022-09-08 14:47:05.000000 pyfinviz-0.8/pyfinviz/quote.py
--rw-rw-rw-   0        0        0    80532 2022-09-08 14:06:27.000000 pyfinviz-0.8/pyfinviz/screener.py
--rw-rw-rw-   0        0        0     2289 2022-09-08 14:44:44.000000 pyfinviz-0.8/pyfinviz/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-02 01:56:23.356400 pyfinviz-0.8/pyfinviz.egg-info/
--rw-rw-rw-   0        0        0    10393 2022-10-02 01:56:23.000000 pyfinviz-0.8/pyfinviz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2022-10-02 01:56:23.000000 pyfinviz-0.8/pyfinviz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-02 01:56:23.000000 pyfinviz-0.8/pyfinviz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2022-10-02 01:56:23.000000 pyfinviz-0.8/pyfinviz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-10-02 01:56:23.000000 pyfinviz-0.8/pyfinviz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      169 2022-10-02 01:56:23.361401 pyfinviz-0.8/setup.cfg
--rw-rw-rw-   0        0        0     1857 2022-10-02 01:55:01.000000 pyfinviz-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-07 15:53:55.599500 pyfinviz-0.9/
+-rw-rw-rw-   0        0        0      563 2022-09-08 14:06:27.000000 pyfinviz-0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0    10393 2022-10-07 15:53:55.599500 pyfinviz-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9443 2022-09-08 14:06:27.000000 pyfinviz-0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-07 15:53:55.581493 pyfinviz-0.9/pyfinviz/
+-rw-rw-rw-   0        0        0      216 2022-09-08 14:06:27.000000 pyfinviz-0.9/pyfinviz/__init__.py
+-rw-rw-rw-   0        0        0      639 2022-09-08 14:06:27.000000 pyfinviz-0.9/pyfinviz/crypto.py
+-rw-rw-rw-   0        0        0     1420 2022-09-08 22:39:28.000000 pyfinviz-0.9/pyfinviz/groups.py
+-rw-rw-rw-   0        0        0      736 2022-09-08 14:06:27.000000 pyfinviz-0.9/pyfinviz/insider.py
+-rw-rw-rw-   0        0        0      993 2022-09-08 14:55:13.000000 pyfinviz-0.9/pyfinviz/news.py
+-rw-rw-rw-   0        0        0     5391 2022-10-07 15:37:47.000000 pyfinviz-0.9/pyfinviz/quote.py
+-rw-rw-rw-   0        0        0    80532 2022-09-08 14:06:27.000000 pyfinviz-0.9/pyfinviz/screener.py
+-rw-rw-rw-   0        0        0     2289 2022-09-08 14:44:44.000000 pyfinviz-0.9/pyfinviz/utils.py
+drwxrwxrwx   0        0        0        0 2022-10-07 15:53:55.598499 pyfinviz-0.9/pyfinviz.egg-info/
+-rw-rw-rw-   0        0        0    10393 2022-10-07 15:53:55.000000 pyfinviz-0.9/pyfinviz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2022-10-07 15:53:55.000000 pyfinviz-0.9/pyfinviz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-07 15:53:55.000000 pyfinviz-0.9/pyfinviz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2022-10-07 15:53:55.000000 pyfinviz-0.9/pyfinviz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-10-07 15:53:55.000000 pyfinviz-0.9/pyfinviz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      169 2022-10-07 15:53:55.600500 pyfinviz-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1857 2022-10-07 15:53:40.000000 pyfinviz-0.9/setup.py
```

### Comparing `pyfinviz-0.8/LICENSE.txt` & `pyfinviz-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfinviz-0.8/PKG-INFO` & `pyfinviz-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyfinviz
-Version: 0.8
+Version: 0.9
 Summary: Scrape data from finviz.com
 Home-page: https://github.com/oscar0812/pyfinviz
 Author: Oscar R. Torres
 Author-email: oscar0812torres@gmail.com
 License: apache-2.0
-Download-URL: https://github.com/oscar0812/pyfinviz/archive/v_08.tar.gz
+Download-URL: https://github.com/oscar0812/pyfinviz/archive/v_09.tar.gz
 Keywords: FINVIZ,STOCKS,SCRAPER,BITTLE
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfinviz-0.8/README.md` & `pyfinviz-0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyfinviz-0.8/pyfinviz/crypto.py` & `pyfinviz-0.9/pyfinviz/crypto.py`

 * *Files identical despite different names*

### Comparing `pyfinviz-0.8/pyfinviz/groups.py` & `pyfinviz-0.9/pyfinviz/groups.py`

 * *Files identical despite different names*

### Comparing `pyfinviz-0.8/pyfinviz/insider.py` & `pyfinviz-0.9/pyfinviz/insider.py`

 * *Files identical despite different names*

### Comparing `pyfinviz-0.8/pyfinviz/news.py` & `pyfinviz-0.9/pyfinviz/news.py`

 * *Files identical despite different names*

### Comparing `pyfinviz-0.8/pyfinviz/quote.py` & `pyfinviz-0.9/pyfinviz/quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         tags__ = ['Date', 'Headline', 'URL', 'From']
         prev_date = None
         for tr_ in outer_news_trs:
             o_tds = tr_.find_all('td', recursive=False)
             if len(o_tds) < 2:
                 continue
             news_a = o_tds[1].find('a')
+            if news_a is None:
+                # broken news
+                continue
+
             news_from = o_tds[1].find('span')
             date_ = o_tds[0].text.strip()
             if '-' not in date_:
                 date_ = prev_date.split(' ')[0] + ' ' + date_
 
             prev_date = date_
             info_ = [date_, news_a.text, news_a['href'], news_from.text]
```

### Comparing `pyfinviz-0.8/pyfinviz/screener.py` & `pyfinviz-0.9/pyfinviz/screener.py`

 * *Files identical despite different names*

### Comparing `pyfinviz-0.8/pyfinviz/utils.py` & `pyfinviz-0.9/pyfinviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyfinviz-0.8/pyfinviz.egg-info/PKG-INFO` & `pyfinviz-0.9/pyfinviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyfinviz
-Version: 0.8
+Version: 0.9
 Summary: Scrape data from finviz.com
 Home-page: https://github.com/oscar0812/pyfinviz
 Author: Oscar R. Torres
 Author-email: oscar0812torres@gmail.com
 License: apache-2.0
-Download-URL: https://github.com/oscar0812/pyfinviz/archive/v_08.tar.gz
+Download-URL: https://github.com/oscar0812/pyfinviz/archive/v_09.tar.gz
 Keywords: FINVIZ,STOCKS,SCRAPER,BITTLE
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfinviz-0.8/setup.py` & `pyfinviz-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='pyfinviz',  # How you named your package folder (MyLib)
     packages=['pyfinviz'],  # Chose the same as "name"
-    version='0.8',  # Start with a small number and increase it with every change you make
+    version='0.9',  # Start with a small number and increase it with every change you make
     license='apache-2.0',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Scrape data from finviz.com',  # Give a short description about your library
     author='Oscar R. Torres',  # Type in your name
     author_email='oscar0812torres@gmail.com',  # Type in your E-Mail
     url='https://github.com/oscar0812/pyfinviz',  # Provide either the link to your github or to your website
-    download_url='https://github.com/oscar0812/pyfinviz/archive/v_08.tar.gz',
+    download_url='https://github.com/oscar0812/pyfinviz/archive/v_09.tar.gz',
     keywords=['FINVIZ', 'STOCKS', 'SCRAPER', 'BITTLE'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
         'validators',
         'beautifulsoup4',
         'free-proxy',
         'pandas',
         'numpy',
```

