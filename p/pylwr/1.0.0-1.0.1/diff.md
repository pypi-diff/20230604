# Comparing `tmp/pylwr-1.0.0.tar.gz` & `tmp/pylwr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylwr-1.0.0.tar", last modified: Sun Jun  4 14:37:52 2023, max compression
+gzip compressed data, was "pylwr-1.0.1.tar", last modified: Sun Jun  4 14:55:05 2023, max compression
```

## Comparing `pylwr-1.0.0.tar` & `pylwr-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:37:52.102728 pylwr-1.0.0/
--rw-rw-rw-   0        0        0    35821 2023-06-04 13:25:02.000000 pylwr-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      679 2023-06-04 14:37:52.101732 pylwr-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-06-04 13:42:44.000000 pylwr-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 14:37:52.099727 pylwr-1.0.0/pylwr.egg-info/
--rw-rw-rw-   0        0        0      679 2023-06-04 14:37:52.000000 pylwr-1.0.0/pylwr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-06-04 14:37:52.000000 pylwr-1.0.0/pylwr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:37:52.000000 pylwr-1.0.0/pylwr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 14:37:52.000000 pylwr-1.0.0/pylwr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      488 2023-06-04 13:41:35.000000 pylwr-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 14:37:52.102728 pylwr-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-06-04 14:37:32.000000 pylwr-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:55:05.537557 pylwr-1.0.1/
+-rw-rw-rw-   0        0        0    35821 2023-06-04 13:25:02.000000 pylwr-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      755 2023-06-04 14:55:05.536559 pylwr-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-06-04 14:38:53.000000 pylwr-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 14:55:05.534555 pylwr-1.0.1/pylwr.egg-info/
+-rw-rw-rw-   0        0        0      755 2023-06-04 14:55:05.000000 pylwr-1.0.1/pylwr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-06-04 14:55:05.000000 pylwr-1.0.1/pylwr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:55:05.000000 pylwr-1.0.1/pylwr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-04 14:55:05.000000 pylwr-1.0.1/pylwr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      488 2023-06-04 14:54:41.000000 pylwr-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 14:55:05.537557 pylwr-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-06-04 14:54:23.000000 pylwr-1.0.1/setup.py
```

### Comparing `pylwr-1.0.0/LICENSE` & `pylwr-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylwr-1.0.0/PKG-INFO` & `pylwr-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylwr
-Version: 1.0.0
+Version: 1.0.1
 Summary: 各种包使用的二次封装
 Home-page: https://gitee.com/linwanrui/pylwr
 Author: linwr
 Author-email: linwr <953297255@qq.com>
 Project-URL: Homepage, https://gitee.com/linwanrui/pylwr
 Project-URL: Bug Tracker, https://gitee.com/linwanrui/pylwr/issues
 Classifier: Programming Language :: Python :: 3
@@ -19,7 +19,14 @@
 应该会用到一些其他依赖
 
 ## 安装
 
 ```shell
 pip install pylwr
 ```
+
+打包与上传
+
+```shell
+py -m build
+py -m twine upload dist\*
+```
```

### Comparing `pylwr-1.0.0/pylwr.egg-info/PKG-INFO` & `pylwr-1.0.1/pylwr.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylwr
-Version: 1.0.0
+Version: 1.0.1
 Summary: 各种包使用的二次封装
 Home-page: https://gitee.com/linwanrui/pylwr
 Author: linwr
 Author-email: linwr <953297255@qq.com>
 Project-URL: Homepage, https://gitee.com/linwanrui/pylwr
 Project-URL: Bug Tracker, https://gitee.com/linwanrui/pylwr/issues
 Classifier: Programming Language :: Python :: 3
@@ -19,7 +19,14 @@
 应该会用到一些其他依赖
 
 ## 安装
 
 ```shell
 pip install pylwr
 ```
+
+打包与上传
+
+```shell
+py -m build
+py -m twine upload dist\*
+```
```

### Comparing `pylwr-1.0.0/setup.py` & `pylwr-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="pylwr",  # 项目名称，保证它的唯一性，不要跟pypi上已存在的包名冲突即可
-    version="1.0.0",  # 程序版本
+    version="1.0.1",  # 程序版本
     py_modules=['mysql'],  # 需要上传的模块名称，这样可以让这些模块直接import导入
     author="linwr",  # 项目作者
     author_email="953297255@qq.com",  # 作者邮件
     description="各种包使用的二次封装",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://gitee.com/linwanrui/pylwr",  # 项目地址
```

