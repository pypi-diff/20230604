# Comparing `tmp/pylwr-1.0.7.tar.gz` & `tmp/pylwr-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylwr-1.0.7.tar", last modified: Sun Jun  4 16:08:11 2023, max compression
+gzip compressed data, was "pylwr-1.0.8.tar", last modified: Sun Jun  4 16:13:21 2023, max compression
```

## Comparing `pylwr-1.0.7.tar` & `pylwr-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 16:08:11.380983 pylwr-1.0.7/
--rw-rw-rw-   0        0        0    35821 2023-06-04 13:25:02.000000 pylwr-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      790 2023-06-04 16:08:11.379984 pylwr-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-04 15:23:09.000000 pylwr-1.0.7/README.md
--rw-rw-rw-   0        0        0      488 2023-06-04 16:07:21.000000 pylwr-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 16:08:11.380983 pylwr-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-06-04 16:07:24.000000 pylwr-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 16:08:11.338737 pylwr-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 16:08:11.351557 pylwr-1.0.7/src/pylwr/
--rw-rw-rw-   0        0        0       33 2023-06-04 15:40:53.000000 pylwr-1.0.7/src/pylwr/__init__.py
--rw-rw-rw-   0        0        0     1728 2023-06-04 14:27:15.000000 pylwr-1.0.7/src/pylwr/mysql.py
-drwxrwxrwx   0        0        0        0 2023-06-04 16:08:11.377957 pylwr-1.0.7/src/pylwr.egg-info/
--rw-rw-rw-   0        0        0      790 2023-06-04 16:08:11.000000 pylwr-1.0.7/src/pylwr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-06-04 16:08:11.000000 pylwr-1.0.7/src/pylwr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 16:08:11.000000 pylwr-1.0.7/src/pylwr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 16:08:11.000000 pylwr-1.0.7/src/pylwr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 16:13:21.318573 pylwr-1.0.8/
+-rw-rw-rw-   0        0        0    35821 2023-06-04 13:25:02.000000 pylwr-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      790 2023-06-04 16:13:21.318573 pylwr-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-04 15:23:09.000000 pylwr-1.0.8/README.md
+-rw-rw-rw-   0        0        0      488 2023-06-04 16:11:50.000000 pylwr-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 16:13:21.320034 pylwr-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-06-04 16:11:44.000000 pylwr-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 16:13:21.281504 pylwr-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 16:13:21.296701 pylwr-1.0.8/src/pylwr/
+-rw-rw-rw-   0        0        0       33 2023-06-04 16:12:10.000000 pylwr-1.0.8/src/pylwr/__init__.py
+-rw-rw-rw-   0        0        0     1728 2023-06-04 14:27:15.000000 pylwr-1.0.8/src/pylwr/mysql.py
+drwxrwxrwx   0        0        0        0 2023-06-04 16:13:21.317433 pylwr-1.0.8/src/pylwr.egg-info/
+-rw-rw-rw-   0        0        0      790 2023-06-04 16:13:21.000000 pylwr-1.0.8/src/pylwr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-06-04 16:13:21.000000 pylwr-1.0.8/src/pylwr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 16:13:21.000000 pylwr-1.0.8/src/pylwr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-04 16:13:21.000000 pylwr-1.0.8/src/pylwr.egg-info/top_level.txt
```

### Comparing `pylwr-1.0.7/LICENSE` & `pylwr-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pylwr-1.0.7/PKG-INFO` & `pylwr-1.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylwr
-Version: 1.0.7
+Version: 1.0.8
 Summary: 各种包使用的二次封装
 Home-page: https://gitee.com/linwanrui/pylwr
 Author: linwr
 Author-email: linwr <953297255@qq.com>
 Project-URL: Homepage, https://gitee.com/linwanrui/pylwr
 Project-URL: Bug Tracker, https://gitee.com/linwanrui/pylwr/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylwr-1.0.7/setup.py` & `pylwr-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="pylwr",  # 项目名称，保证它的唯一性，不要跟pypi上已存在的包名冲突即可
-    version="1.0.7",  # 程序版本
+    version="1.0.8",  # 程序版本
     # py_modules=['mysql'],  # 需要上传的模块名称，这样可以让这些模块直接import导入
     author="linwr",  # 项目作者
     author_email="953297255@qq.com",  # 作者邮件
     description="各种包使用的二次封装",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://gitee.com/linwanrui/pylwr",  # 项目地址
```

### Comparing `pylwr-1.0.7/src/pylwr/mysql.py` & `pylwr-1.0.8/src/pylwr/mysql.py`

 * *Files identical despite different names*

### Comparing `pylwr-1.0.7/src/pylwr.egg-info/PKG-INFO` & `pylwr-1.0.8/src/pylwr.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylwr
-Version: 1.0.7
+Version: 1.0.8
 Summary: 各种包使用的二次封装
 Home-page: https://gitee.com/linwanrui/pylwr
 Author: linwr
 Author-email: linwr <953297255@qq.com>
 Project-URL: Homepage, https://gitee.com/linwanrui/pylwr
 Project-URL: Bug Tracker, https://gitee.com/linwanrui/pylwr/issues
 Classifier: Programming Language :: Python :: 3
```

