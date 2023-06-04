# Comparing `tmp/easyNotion-0.0.1.tar.gz` & `tmp/easyNotion-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easyNotion-0.0.1.tar", last modified: Thu Jun  1 13:00:09 2023, max compression
+gzip compressed data, was "dist\easyNotion-0.0.2.tar", last modified: Sun Jun  4 02:31:52 2023, max compression
```

## Comparing `easyNotion-0.0.1.tar` & `easyNotion-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 13:00:09.000000 easyNotion-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-06-01 12:58:31.000000 easyNotion-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     6665 2023-06-01 13:00:09.000000 easyNotion-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6212 2023-06-01 12:03:32.000000 easyNotion-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 13:00:09.000000 easyNotion-0.0.1/easyNotion/
--rw-rw-rw-   0        0        0        0 2023-06-01 11:49:47.000000 easyNotion-0.0.1/easyNotion/__init__.py
--rw-rw-rw-   0        0        0     7313 2023-06-01 11:10:16.000000 easyNotion-0.0.1/easyNotion/easyNotion.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:00:09.000000 easyNotion-0.0.1/easyNotion.egg-info/
--rw-rw-rw-   0        0        0     6665 2023-06-01 13:00:08.000000 easyNotion-0.0.1/easyNotion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-06-01 13:00:09.000000 easyNotion-0.0.1/easyNotion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 13:00:08.000000 easyNotion-0.0.1/easyNotion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-01 13:00:09.000000 easyNotion-0.0.1/easyNotion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 13:00:09.000000 easyNotion-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-06-01 12:57:59.000000 easyNotion-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:31:52.000000 easyNotion-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-06-01 12:58:31.000000 easyNotion-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     6665 2023-06-04 02:31:52.000000 easyNotion-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6212 2023-06-01 12:03:32.000000 easyNotion-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 02:31:52.000000 easyNotion-0.0.2/easyNotion/
+-rw-rw-rw-   0        0        0        0 2023-06-01 11:49:47.000000 easyNotion-0.0.2/easyNotion/__init__.py
+-rw-rw-rw-   0        0        0     8659 2023-06-04 02:30:44.000000 easyNotion-0.0.2/easyNotion/easyNotion.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:31:52.000000 easyNotion-0.0.2/easyNotion.egg-info/
+-rw-rw-rw-   0        0        0     6665 2023-06-04 02:31:51.000000 easyNotion-0.0.2/easyNotion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-06-04 02:31:52.000000 easyNotion-0.0.2/easyNotion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 02:31:51.000000 easyNotion-0.0.2/easyNotion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-04 02:31:51.000000 easyNotion-0.0.2/easyNotion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 02:31:52.000000 easyNotion-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-06-04 02:22:23.000000 easyNotion-0.0.2/setup.py
```

### Comparing `easyNotion-0.0.1/LICENSE.txt` & `easyNotion-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyNotion-0.0.1/PKG-INFO` & `easyNotion-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyNotion
-Version: 0.0.1
+Version: 0.0.2
 Summary: A very easy-to-use Notion API
 Home-page: https://github.com/zuo-shi-yun/easy-notion-API
 Author: zuoShiYun
 Author-email: 2818252801@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `easyNotion-0.0.1/README.md` & `easyNotion-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `easyNotion-0.0.1/easyNotion/easyNotion.py` & `easyNotion-0.0.2/easyNotion/easyNotion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 
 import requests
 
 
 class easyNotion:
-    def __init__(self, database_id, token):
+    def __init__(self, database_id, token, sort_key=''):
         # 基础url
+        self.sort_key = sort_key
         self.baseUrl = 'https://api.notion.com/v1/'
         # 数据库ID
         self.database_id = database_id
         # 请求头
         self.headers = {
             'Accept': 'application/json',
             'Notion-Version': '2022-06-28',
@@ -34,47 +35,58 @@
         if res.status_code != 200:
             raise Exception('An error occurred:网络链接失败' + str(res))
 
         # 转为json对象
         table = json.loads(res.text)
         temp = table['results']
         # 排序
-        table['results'] = sorted(temp, key=lambda x: int(x['properties']['ID']['unique_id']['number']))
+        if len(temp):
+            if 'ID' in temp[0]['properties']:
+                table['results'] = sorted(temp, key=lambda x: int(x['properties']['ID']['unique_id']['number']))
+            elif len(self.sort_key):
+                if 'title' in temp[0]['properties'][self.sort_key]:
+                    table['results'] = sorted(temp,
+                                              key=lambda x: int(
+                                                  x['properties'][self.sort_key]['title'][0]['plain_text']))
+                else:
+                    table['results'] = sorted(temp,
+                                              key=lambda x: int(
+                                                  x['properties'][self.sort_key]['rich_text'][0]['plain_text']))
 
         return table
 
     # 获得处理后的数据表
     def getTable(self):
         """
         获得处理后的数据表
         """
         base_table = self.getTableAll()  # 未处理的表
         table = []
-
-        for row in base_table['results']:
-            info = {'id': row['id']}  # 行id,这是系统的id不是显示的ID
-
-            for col in row['properties']:
-                if row['properties'][col]['type'] == 'unique_id':  # 特殊处理ID列
-                    info['ID'] = row['properties'][col]['unique_id']['prefix'] + '-' + str(
-                        row['properties'][col]['unique_id']['number'])
-                elif row['properties'][col]['type'] == 'title':  # 特殊处理title列
-                    title = row['properties'][col]['title']
-                    if len(title) != 0:
-                        info[col] = row['properties'][col]['title'][0]['plain_text']
-                    else:
-                        info[col] = ''
-                else:
-                    text = info[col] = row['properties'][col]['rich_text']
-                    if len(text) != 0:
-                        info[col] = row['properties'][col]['rich_text'][0]['plain_text']
+        if len(base_table['results']):
+            for row in base_table['results']:
+                info = {'id': row['id']}  # 行id,这是系统的id不是显示的ID
+
+                for col in row['properties']:
+                    if row['properties'][col]['type'] == 'unique_id':  # 特殊处理ID列
+                        info['ID'] = row['properties'][col]['unique_id']['prefix'] + '-' + str(
+                            row['properties'][col]['unique_id']['number'])
+                    elif row['properties'][col]['type'] == 'title':  # 特殊处理title列
+                        title = row['properties'][col]['title']
+                        if len(title) != 0:
+                            info[col] = row['properties'][col]['title'][0]['plain_text']
+                        else:
+                            info[col] = ''
                     else:
-                        info[col] = ''
+                        text = info[col] = row['properties'][col]['rich_text']
+                        if len(text) != 0:
+                            info[col] = row['properties'][col]['rich_text'][0]['plain_text']
+                        else:
+                            info[col] = ''
 
-            table.append(info)
+                table.append(info)
 
         return table
 
     # 根据指定的列名col查询该列
     def queryCol(self, col: str):
         """
         :param col:字符串类型的列名\n
@@ -100,14 +112,29 @@
 
         for row in self.table:
             if row[col] == content:
                 return row
         else:
             return {}
 
+    # 查询一个数据
+    def queryCell(self, key_col: str, content: str, find_col: str):
+        """
+        根据key_col列的content数据查找find_col列的数据
+        :param key_col:标识行的列名
+        :param content:表示行的列的内容
+        :param find_col:查找列的列明
+        :return:返回该单元格的内容
+        """
+        for i in self.table:
+            if i[key_col] == content:
+                return i[find_col]
+        else:
+            return ''
+
     # 获取总行数
     def getRowCnt(self):
         """
         根据数据表判断总行数\n
         :return:返回总行数
         """
         return len(self.table)
```

### Comparing `easyNotion-0.0.1/easyNotion.egg-info/PKG-INFO` & `easyNotion-0.0.2/easyNotion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyNotion
-Version: 0.0.1
+Version: 0.0.2
 Summary: A very easy-to-use Notion API
 Home-page: https://github.com/zuo-shi-yun/easy-notion-API
 Author: zuoShiYun
 Author-email: 2818252801@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `easyNotion-0.0.1/setup.py` & `easyNotion-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="easyNotion",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.1",  # 包版本号，便于维护版本
+    version="0.0.2",  # 包版本号，便于维护版本
     author="zuoShiYun",  # 作者，可以写自己的姓名
     author_email="2818252801@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="A very easy-to-use Notion API",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/zuo-shi-yun/easy-notion-API",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

