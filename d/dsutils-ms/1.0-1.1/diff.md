# Comparing `tmp/dsutils_ms-1.0.tar.gz` & `tmp/dsutils_ms-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsutils_ms-1.0.tar", last modified: Tue May 30 02:08:16 2023, max compression
+gzip compressed data, was "dsutils_ms-1.1.tar", last modified: Sun Jun  4 01:26:38 2023, max compression
```

## Comparing `dsutils_ms-1.0.tar` & `dsutils_ms-1.1.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 02:08:16.082410 dsutils_ms-1.0/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    34903 2023-05-29 20:18:43.000000 dsutils_ms-1.0/LICENSE.md
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      563 2023-05-30 02:08:16.086410 dsutils_ms-1.0/PKG-INFO
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-29 20:06:27.000000 dsutils_ms-1.0/README.md
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 02:08:16.082410 dsutils_ms-1.0/dsutils_ms/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-29 20:26:01.000000 dsutils_ms-1.0/dsutils_ms/__init__.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 02:08:16.082410 dsutils_ms-1.0/dsutils_ms/adapters/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-29 20:26:01.000000 dsutils_ms-1.0/dsutils_ms/adapters/__init__.py
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)     5336 2023-05-30 02:07:35.000000 dsutils_ms-1.0/dsutils_ms/adapters/google_sheets.py
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)     1223 2023-05-30 01:29:24.000000 dsutils_ms-1.0/dsutils_ms/adapters/interface.py
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)     3489 2023-05-30 02:07:35.000000 dsutils_ms-1.0/dsutils_ms/adapters/mysql.py
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)     3199 2023-05-30 02:07:35.000000 dsutils_ms-1.0/dsutils_ms/adapters/s3.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 02:08:16.082410 dsutils_ms-1.0/dsutils_ms/cleaning/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-29 20:26:01.000000 dsutils_ms-1.0/dsutils_ms/cleaning/__init__.py
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)     2913 2023-05-30 01:32:53.000000 dsutils_ms-1.0/dsutils_ms/cleaning/a.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 02:08:16.082410 dsutils_ms-1.0/dsutils_ms/helpers/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-29 20:26:01.000000 dsutils_ms-1.0/dsutils_ms/helpers/__init__.py
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)      789 2023-05-30 02:07:35.000000 dsutils_ms-1.0/dsutils_ms/helpers/dataframe.py
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)      867 2023-05-30 02:07:35.000000 dsutils_ms-1.0/dsutils_ms/helpers/env.py
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)      112 2023-05-29 22:49:40.000000 dsutils_ms-1.0/dsutils_ms/helpers/google_chat.py
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)      776 2023-05-16 16:00:49.000000 dsutils_ms-1.0/dsutils_ms/helpers/log.py
-drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 02:08:16.082410 dsutils_ms-1.0/dsutils_ms.egg-info/
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      563 2023-05-30 02:08:16.000000 dsutils_ms-1.0/dsutils_ms.egg-info/PKG-INFO
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      638 2023-05-30 02:08:16.000000 dsutils_ms-1.0/dsutils_ms.egg-info/SOURCES.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-05-30 02:08:16.000000 dsutils_ms-1.0/dsutils_ms.egg-info/dependency_links.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      214 2023-05-30 02:08:16.000000 dsutils_ms-1.0/dsutils_ms.egg-info/requires.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       11 2023-05-30 02:08:16.000000 dsutils_ms-1.0/dsutils_ms.egg-info/top_level.txt
--rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-05-30 02:08:16.000000 dsutils_ms-1.0/dsutils_ms.egg-info/zip-safe
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)       80 2023-05-16 15:38:32.000000 dsutils_ms-1.0/pyproject.toml
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)     1070 2023-05-30 02:08:16.086410 dsutils_ms-1.0/setup.cfg
--rw-r--r--   0 msserpa   (1000) msserpa   (1000)       69 2023-05-16 15:49:04.000000 dsutils_ms-1.0/setup.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.521625 dsutils_ms-1.1/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    34903 2023-05-30 17:35:50.000000 dsutils_ms-1.1/LICENSE.md
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      635 2023-06-04 01:26:38.521625 dsutils_ms-1.1/PKG-INFO
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       71 2023-05-30 17:35:50.000000 dsutils_ms-1.1/README.md
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.513625 dsutils_ms-1.1/dsutils_ms/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/__init__.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.513625 dsutils_ms-1.1/dsutils_ms/adapters/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/adapters/__init__.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2206 2023-06-04 01:19:54.000000 dsutils_ms-1.1/dsutils_ms/adapters/dynamo.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     5336 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/adapters/google_sheets.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1223 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/adapters/interface.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3489 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/adapters/mysql.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3199 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/adapters/s3.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.517624 dsutils_ms-1.1/dsutils_ms/helpers/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        0 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/helpers/__init__.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     7202 2023-06-04 00:51:17.000000 dsutils_ms-1.1/dsutils_ms/helpers/cleaning.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      789 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/helpers/dataframe.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      748 2023-06-03 23:40:41.000000 dsutils_ms-1.1/dsutils_ms/helpers/datetime.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      738 2023-06-03 23:40:42.000000 dsutils_ms-1.1/dsutils_ms/helpers/dict.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      867 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/helpers/env.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      112 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/helpers/google_chat.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      776 2023-05-30 17:35:50.000000 dsutils_ms-1.1/dsutils_ms/helpers/log.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.513625 dsutils_ms-1.1/dsutils_ms.egg-info/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      635 2023-06-04 01:26:38.000000 dsutils_ms-1.1/dsutils_ms.egg-info/PKG-INFO
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      788 2023-06-04 01:26:38.000000 dsutils_ms-1.1/dsutils_ms.egg-info/SOURCES.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-06-04 01:26:38.000000 dsutils_ms-1.1/dsutils_ms.egg-info/dependency_links.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)      191 2023-06-04 01:26:38.000000 dsutils_ms-1.1/dsutils_ms.egg-info/requires.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       11 2023-06-04 01:26:38.000000 dsutils_ms-1.1/dsutils_ms.egg-info/top_level.txt
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)        1 2023-05-30 18:22:49.000000 dsutils_ms-1.1/dsutils_ms.egg-info/zip-safe
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       80 2023-05-30 17:35:50.000000 dsutils_ms-1.1/pyproject.toml
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     1044 2023-06-04 01:26:38.525625 dsutils_ms-1.1/setup.cfg
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)       69 2023-05-30 17:35:50.000000 dsutils_ms-1.1/setup.py
+drwxrwxr-x   0 msserpa   (1000) msserpa   (1000)        0 2023-06-04 01:26:38.521625 dsutils_ms-1.1/tests/
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)    15766 2023-06-04 01:02:31.000000 dsutils_ms-1.1/tests/test_cleaning.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2980 2023-05-30 17:35:50.000000 dsutils_ms-1.1/tests/test_google_sheets.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     3456 2023-05-30 17:35:50.000000 dsutils_ms-1.1/tests/test_mysql.py
+-rw-rw-r--   0 msserpa   (1000) msserpa   (1000)     2342 2023-05-30 17:35:50.000000 dsutils_ms-1.1/tests/test_s3.py
```

### Comparing `dsutils_ms-1.0/LICENSE.md` & `dsutils_ms-1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.0/PKG-INFO` & `dsutils_ms-1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Metadata-Version: 2.1
 Name: dsutils_ms
-Version: 1.0
+Version: 1.1
 Summary: My Data Science Utils
 Home-page: https://www.linkedin.com/in/matheusserpa/
 Author: Matheus Serpa
 Author-email: matheusserpa@gmail.com
 License: GNU General Public License v3.0
 Keywords: data science,data engineering,machine learning,data analysis,data visualization
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+
+python3.11 setup.py sdist
+
+twine upload dist/*
+
+
+pip3.11 install -e .
+
```

### Comparing `dsutils_ms-1.0/dsutils_ms/adapters/google_sheets.py` & `dsutils_ms-1.1/dsutils_ms/adapters/google_sheets.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.0/dsutils_ms/adapters/interface.py` & `dsutils_ms-1.1/dsutils_ms/adapters/interface.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.0/dsutils_ms/adapters/mysql.py` & `dsutils_ms-1.1/dsutils_ms/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.0/dsutils_ms/adapters/s3.py` & `dsutils_ms-1.1/dsutils_ms/adapters/s3.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.0/dsutils_ms/helpers/dataframe.py` & `dsutils_ms-1.1/dsutils_ms/helpers/dataframe.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.0/dsutils_ms/helpers/env.py` & `dsutils_ms-1.1/dsutils_ms/helpers/env.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.0/dsutils_ms/helpers/log.py` & `dsutils_ms-1.1/dsutils_ms/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dsutils_ms-1.0/dsutils_ms.egg-info/PKG-INFO` & `dsutils_ms-1.1/dsutils_ms.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Metadata-Version: 2.1
 Name: dsutils-ms
-Version: 1.0
+Version: 1.1
 Summary: My Data Science Utils
 Home-page: https://www.linkedin.com/in/matheusserpa/
 Author: Matheus Serpa
 Author-email: matheusserpa@gmail.com
 License: GNU General Public License v3.0
 Keywords: data science,data engineering,machine learning,data analysis,data visualization
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+
+python3.11 setup.py sdist
+
+twine upload dist/*
+
+
+pip3.11 install -e .
+
```

### Comparing `dsutils_ms-1.0/setup.cfg` & `dsutils_ms-1.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsutils_ms
-version = 1.0
+version = 1.1
 author = Matheus Serpa
 author_email = matheusserpa@gmail.com
 url = https://www.linkedin.com/in/matheusserpa/
 description = My Data Science Utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = data science, data engineering, machine learning, data analysis, data visualization
@@ -16,26 +16,25 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 zip_safe = True
 include_package_data = True
 install_requires = 
+	boto3 == 1.26.*
+	databricks-connect == 13.0.*
+	gspread == 5.9.*
+	nltk == 3.8.*
+	openpyxl == 3.1.*
 	pyspark == 3.4.*
 	pytest == 7.3.*
-	pytest-runner == 6.0.*
 	pytest-cov == 4.0.*
-	databricks-connect == 13.0.*
+	pytest-runner == 6.0.*
 	python-dotenv == 1.0.*
 	sqlalchemy == 2.0.*
-	gspread == 5.9.*
-	unidecode == 1.3.*
-	inflection == 0.5.*
-	boto3 == 1.26.*
-	openpyxl == 3.1.*
 
 [options.packages.find]
 include = 
 	dsutils_ms
 	dsutils_ms.*
 
 [aliases]
```

