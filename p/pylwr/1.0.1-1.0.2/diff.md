# Comparing `tmp/pylwr-1.0.1.tar.gz` & `tmp/pylwr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylwr-1.0.1.tar", last modified: Sun Jun  4 14:55:05 2023, max compression
+gzip compressed data, was "pylwr-1.0.2.tar", last modified: Sun Jun  4 15:01:44 2023, max compression
```

## Comparing `pylwr-1.0.1.tar` & `pylwr-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:55:05.537557 pylwr-1.0.1/
--rw-rw-rw-   0        0        0    35821 2023-06-04 13:25:02.000000 pylwr-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      755 2023-06-04 14:55:05.536559 pylwr-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-06-04 14:38:53.000000 pylwr-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 14:55:05.534555 pylwr-1.0.1/pylwr.egg-info/
--rw-rw-rw-   0        0        0      755 2023-06-04 14:55:05.000000 pylwr-1.0.1/pylwr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-06-04 14:55:05.000000 pylwr-1.0.1/pylwr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:55:05.000000 pylwr-1.0.1/pylwr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 14:55:05.000000 pylwr-1.0.1/pylwr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      488 2023-06-04 14:54:41.000000 pylwr-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 14:55:05.537557 pylwr-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      876 2023-06-04 14:54:23.000000 pylwr-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 15:01:44.359010 pylwr-1.0.2/
+-rw-rw-rw-   0        0        0    35821 2023-06-04 13:25:02.000000 pylwr-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      755 2023-06-04 15:01:44.357608 pylwr-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-06-04 14:57:38.000000 pylwr-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 15:01:44.351853 pylwr-1.0.2/pylwr.egg-info/
+-rw-rw-rw-   0        0        0      755 2023-06-04 15:01:44.000000 pylwr-1.0.2/pylwr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-06-04 15:01:44.000000 pylwr-1.0.2/pylwr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 15:01:44.000000 pylwr-1.0.2/pylwr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 15:01:44.000000 pylwr-1.0.2/pylwr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      488 2023-06-04 15:01:13.000000 pylwr-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 15:01:44.360175 pylwr-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      871 2023-06-04 15:01:11.000000 pylwr-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 15:01:44.354781 pylwr-1.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-06-04 14:54:07.000000 pylwr-1.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0     1728 2023-06-04 14:27:15.000000 pylwr-1.0.2/src/mysql.py
```

### Comparing `pylwr-1.0.1/LICENSE` & `pylwr-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylwr-1.0.1/PKG-INFO` & `pylwr-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylwr
-Version: 1.0.1
+Version: 1.0.2
 Summary: 各种包使用的二次封装
 Home-page: https://gitee.com/linwanrui/pylwr
 Author: linwr
 Author-email: linwr <953297255@qq.com>
 Project-URL: Homepage, https://gitee.com/linwanrui/pylwr
 Project-URL: Bug Tracker, https://gitee.com/linwanrui/pylwr/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylwr-1.0.1/pylwr.egg-info/PKG-INFO` & `pylwr-1.0.2/pylwr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylwr
-Version: 1.0.1
+Version: 1.0.2
 Summary: 各种包使用的二次封装
 Home-page: https://gitee.com/linwanrui/pylwr
 Author: linwr
 Author-email: linwr <953297255@qq.com>
 Project-URL: Homepage, https://gitee.com/linwanrui/pylwr
 Project-URL: Bug Tracker, https://gitee.com/linwanrui/pylwr/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylwr-1.0.1/setup.py` & `pylwr-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
  
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="pylwr",  # 项目名称，保证它的唯一性，不要跟pypi上已存在的包名冲突即可
-    version="1.0.1",  # 程序版本
+    version="1.0.2",  # 程序版本
     py_modules=['mysql'],  # 需要上传的模块名称，这样可以让这些模块直接import导入
     author="linwr",  # 项目作者
     author_email="953297255@qq.com",  # 作者邮件
     description="各种包使用的二次封装",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://gitee.com/linwanrui/pylwr",  # 项目地址
-    packages=setuptools.find_packages("src"),  # 无需修改
+    packages=setuptools.find_packages(),  # 无需修改
     # install_requires=['docutils>=0.3'], # 依赖包增加
 )
```

