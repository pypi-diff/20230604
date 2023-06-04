# Comparing `tmp/pylwr-1.0.4.tar.gz` & `tmp/pylwr-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylwr-1.0.4.tar", last modified: Sun Jun  4 15:23:32 2023, max compression
+gzip compressed data, was "pylwr-1.0.5.tar", last modified: Sun Jun  4 15:41:02 2023, max compression
```

## Comparing `pylwr-1.0.4.tar` & `pylwr-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 15:23:32.313328 pylwr-1.0.4/
--rw-rw-rw-   0        0        0    35821 2023-06-04 13:25:02.000000 pylwr-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      790 2023-06-04 15:23:32.312327 pylwr-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-04 15:23:09.000000 pylwr-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 15:23:32.295980 pylwr-1.0.4/pylwr/
--rw-rw-rw-   0        0        0     1728 2023-06-04 14:27:15.000000 pylwr-1.0.4/pylwr/mysql.py
-drwxrwxrwx   0        0        0        0 2023-06-04 15:23:32.310326 pylwr-1.0.4/pylwr/pylwr.egg-info/
--rw-rw-rw-   0        0        0      790 2023-06-04 15:23:32.000000 pylwr-1.0.4/pylwr/pylwr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-06-04 15:23:32.000000 pylwr-1.0.4/pylwr/pylwr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 15:23:32.000000 pylwr-1.0.4/pylwr/pylwr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 15:23:32.000000 pylwr-1.0.4/pylwr/pylwr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      488 2023-06-04 15:23:14.000000 pylwr-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 15:23:32.313328 pylwr-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1200 2023-06-04 15:23:17.000000 pylwr-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 15:41:02.378112 pylwr-1.0.5/
+-rw-rw-rw-   0        0        0    35821 2023-06-04 13:25:02.000000 pylwr-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      790 2023-06-04 15:41:02.375986 pylwr-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-04 15:23:09.000000 pylwr-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 15:41:02.362484 pylwr-1.0.5/pylwr/
+-rw-rw-rw-   0        0        0       33 2023-06-04 15:40:53.000000 pylwr-1.0.5/pylwr/__init__.py
+-rw-rw-rw-   0        0        0     1728 2023-06-04 14:27:15.000000 pylwr-1.0.5/pylwr/mysql.py
+drwxrwxrwx   0        0        0        0 2023-06-04 15:41:02.372824 pylwr-1.0.5/pylwr.egg-info/
+-rw-rw-rw-   0        0        0      790 2023-06-04 15:41:02.000000 pylwr-1.0.5/pylwr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-04 15:41:02.000000 pylwr-1.0.5/pylwr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 15:41:02.000000 pylwr-1.0.5/pylwr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-04 15:41:02.000000 pylwr-1.0.5/pylwr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      488 2023-06-04 15:37:04.000000 pylwr-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 15:41:02.378112 pylwr-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1121 2023-06-04 15:37:00.000000 pylwr-1.0.5/setup.py
```

### Comparing `pylwr-1.0.4/LICENSE` & `pylwr-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pylwr-1.0.4/PKG-INFO` & `pylwr-1.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylwr
-Version: 1.0.4
+Version: 1.0.5
 Summary: 各种包使用的二次封装
 Home-page: https://gitee.com/linwanrui/pylwr
 Author: linwr
 Author-email: linwr <953297255@qq.com>
 Project-URL: Homepage, https://gitee.com/linwanrui/pylwr
 Project-URL: Bug Tracker, https://gitee.com/linwanrui/pylwr/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylwr-1.0.4/pylwr/mysql.py` & `pylwr-1.0.5/pylwr/mysql.py`

 * *Files identical despite different names*

### Comparing `pylwr-1.0.4/pylwr/pylwr.egg-info/PKG-INFO` & `pylwr-1.0.5/pylwr.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylwr
-Version: 1.0.4
+Version: 1.0.5
 Summary: 各种包使用的二次封装
 Home-page: https://gitee.com/linwanrui/pylwr
 Author: linwr
 Author-email: linwr <953297255@qq.com>
 Project-URL: Homepage, https://gitee.com/linwanrui/pylwr
 Project-URL: Bug Tracker, https://gitee.com/linwanrui/pylwr/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylwr-1.0.4/setup.py` & `pylwr-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import setuptools
  
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="pylwr",  # 项目名称，保证它的唯一性，不要跟pypi上已存在的包名冲突即可
-    version="1.0.4",  # 程序版本
+    version="1.0.5",  # 程序版本
     py_modules=['mysql'],  # 需要上传的模块名称，这样可以让这些模块直接import导入
     author="linwr",  # 项目作者
     author_email="953297255@qq.com",  # 作者邮件
     description="各种包使用的二次封装",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://gitee.com/linwanrui/pylwr",  # 项目地址
-    packages=setuptools.find_packages("pylwr"),  # 无需修改
-    package_dir = {"":"pylwr"},		# 告诉 setuptools 包都在 src 下
+    packages=setuptools.find_packages(),  # 无需修改
     package_data = {
     ## 包含 data 文件夹下所有的 *.dat 文件
         "":[".txt", ".info", "*.properties", ".py"],
         "":["data/*.*"],
     },
     # 取消所有测试包
     exclude = ["*.test", "*.test.*", "test.*", "test"]
```

