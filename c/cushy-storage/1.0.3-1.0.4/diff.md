# Comparing `tmp/cushy-storage-1.0.3.tar.gz` & `tmp/cushy-storage-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-j3ydswem/cushy-storage-1.0.3.tar", last modified: Thu May 11 16:06:00 2023, max compression
+gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-pwlr5tu9/cushy-storage-1.0.4.tar", last modified: Sun Jun  4 15:18:19 2023, max compression
```

## Comparing `cushy-storage-1.0.3.tar` & `cushy-storage-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/cushy_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/cushy_storage/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/cushy_storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/cushy_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:06:00.000000 cushy-storage-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/tests/test_base_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/tests/test_cushy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-11 16:05:47.000000 cushy-storage-1.0.3/tests/test_dict_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/cushy_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/cushy_storage/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/cushy_storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/cushy_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:18:19.000000 cushy-storage-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/tests/test_base_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/tests/test_cushy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-04 15:18:08.000000 cushy-storage-1.0.4/tests/test_dict_cache.py
```

### Comparing `cushy-storage-1.0.3/LICENSE` & `cushy-storage-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.3/PKG-INFO` & `cushy-storage-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.0.3
+Version: 1.0.4
 Summary: A data local persistence framework library
 Home-page: https://github.com/Undertone0809/cushy-storage
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: storage,serialization,json,cushy-storage,cushy_storage
 Classifier: Development Status :: 3 - Alpha
@@ -38,39 +38,40 @@
         <img src="https://static.pepy.tech/personalized-badge/cushy-socket?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
    </a>
 </p>
 
 [English](/README_en.md) [中文](/README.md)
 
 # 简介
+
 cushy-storage是一个基于磁盘缓存的Python库，可以将Python对象序列化后缓存到磁盘中，以便下次使用时直接读取，从而提高程序的执行效率。另一方面，
 cushy-storage让你无需花费精力在如何制订一套数据存储规范上，字典般的操作可以减少很多开发的成本。
 
 # 特性
-- 可以方便的将数据进行本地磁盘存储
+
+- 可以方便地将数据(基本数据类型、自定义数据类型)进行本地磁盘存储
 - 免去了直接操作文件的工作
 - 像操作dict一样读写，十分方便
 - 提供序列化操作
 - 提供多种数据压缩方式
 
-
 # 安装
 
 ```bash
 pip install cushy-storage --upgrade 
 ```
 
 # 快速上手
 
 `cushy-storage` 的使用主要分为三个类，`BaseDict` `CushyDict` `disk_cache`，其中`CushyDict`是`BaseDict`的增强版，可以实现
 `BaseDict`的所有功能，还增加了相应序列化操作，因此推荐直接使用`CushyDict`来操作保存数据。
 
 ## BaseDict类
 
-BaseDict类是CushyDict类的基础实现，提供了基本的字典结构和缓存操作。它可以用于缓存任何类型的Python对象，但不支持序列化和反序列化操作。
+BaseDict类是CushyDict类的基础实现，其只支持简单的二进制数据存储。
 
 ```python
 from cushy_storage import BaseDict
 
 # 初始化cache，保存在./data文件夹下
 cache = BaseDict('./data')
 # Base Dict只能存储二进制数据，可以用于流式传输
@@ -78,15 +79,19 @@
 value = cache['key']
 print(value)
 
 ```
 
 ## CushyDict类
 
-CushyDict类是BaseDict库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是一些简单的使用教程。
+CushyDict类是BaseDict库的高级实现，你可以像操作字典一样操作CushyDict；其增加了对值进行序列化和反序列化的功能，可以存储任意类型的数据。
+此外，CushyDict支持多种序列化算法 （pickle和json）和压缩算法（zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是
+一些简单的使用教程。
+
+- 存储Python基本数据类型
 
 ```python
 from cushy_storage import CushyDict
 
 # 初始化cache，保存在./data文件夹下
 cache = CushyDict('./data')
 
@@ -95,96 +100,100 @@
 
 cache['a'] = 1
 print(cache['a'])
 
 cache['b'] = "hello world"
 print(cache['b'])
 
-cache['arr'] = [1,2,3,4,5]
+cache['arr'] = [1, 2, 3, 4, 5]
 print(cache['arr'])
 
 ```
 
+> 以`cache['arr'] = [1, 2, 3, 4, 5]`为例，在指令这段代码之后，CushyDict会将数据存储到指令文件夹下。
+
 - 生成结果
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210730.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210837.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210825.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210809.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210757.png"/>
 
-- 如果在初始化的时候不传入参数，则默认保存在`./data`文件夹下
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-```
-
-
-- 判断key是否存在（和字典操作同理）
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict('./data')
-if 'key' in cache:
-    print("key exist")
-else:
-    print("key not exist")
-
-```
-
-- 用`CushyDict`存储对象信息
+- 存储自定义数据类型
 
 ```python
 from cushy_storage import CushyDict
 
 
 class User:
     def __init__(self, name, age):
         self.name = name
         self.age = age
 
 
 def main():
-    cache = CushyDict('./data', serialize='pickle')
+    cache = CushyDict(serialize='pickle')
     user = User("Jack", 18)
     cache['user'] = user
 
+    user = cache['user']
+    print(type(user))
     print(cache['user'].name)
     print(cache['user'].age)
 
 
 if __name__ == '__main__':
     main()
+```
+
+> 需要说明的是，如果你有定义复杂数据的需求，如List里面存json；或者你没有去文件下看原数据的需求，则推荐使用pickle的方式来进行数据存储。
+
+- 如果在初始化的时候不传入参数，则默认保存在`./cache`文件夹下
+
+```python
+from cushy_storage import CushyDict
 
+cache = CushyDict()
 ```
 
+- 判断key是否存在（和字典操作同理）
 
-## disk_cache装饰器函数
+```python
+from cushy_storage import CushyDict
 
-disk_cache装饰器函数可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
+cache = CushyDict()
+if 'key' in cache:
+    print("key exist")
+else:
+    print("key not exist")
+
+```
+
+## disk_cache装饰器
+
+disk_cache装饰器可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
 
 ```python
 from cushy_storage import disk_cache
 
+
 @disk_cache('./data')
 def my_func():
     return {'value': 42}
 
+
 result = my_func()
 
 ```
- 
- 
+
 # 待办
 
 - [ ] 提供单例模式解决方案，提供更加方便的工具类
 - [ ] 支持更多的压缩和序列化算法，以满足不同类型数据的需求
 - [ ] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
 - [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
 - [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
@@ -193,13 +202,17 @@
 - [ ] 改善文档结构和代码注释，方便用户理解和使用库
 - [ ] 支持Python3中的异步IO，提高程序的并发性和性能
 - [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
 - [ ] 支持更多数据格式的持久化方式，如json,xml的直接存储
 - [ ] 提供ORM框架，封装对象级的CRUD操作
 
 # 鸣谢
-本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage) 进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
 
-This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to RimoChan for his great work.
+本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage)
+进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
+
+This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to
+RimoChan for his great work.
 
 # 贡献
+
 如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
```

### Comparing `cushy-storage-1.0.3/README.md` & `cushy-storage-1.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,39 +16,40 @@
         <img src="https://static.pepy.tech/personalized-badge/cushy-socket?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
    </a>
 </p>
 
 [English](/README_en.md) [中文](/README.md)
 
 # 简介
+
 cushy-storage是一个基于磁盘缓存的Python库，可以将Python对象序列化后缓存到磁盘中，以便下次使用时直接读取，从而提高程序的执行效率。另一方面，
 cushy-storage让你无需花费精力在如何制订一套数据存储规范上，字典般的操作可以减少很多开发的成本。
 
 # 特性
-- 可以方便的将数据进行本地磁盘存储
+
+- 可以方便地将数据(基本数据类型、自定义数据类型)进行本地磁盘存储
 - 免去了直接操作文件的工作
 - 像操作dict一样读写，十分方便
 - 提供序列化操作
 - 提供多种数据压缩方式
 
-
 # 安装
 
 ```bash
 pip install cushy-storage --upgrade 
 ```
 
 # 快速上手
 
 `cushy-storage` 的使用主要分为三个类，`BaseDict` `CushyDict` `disk_cache`，其中`CushyDict`是`BaseDict`的增强版，可以实现
 `BaseDict`的所有功能，还增加了相应序列化操作，因此推荐直接使用`CushyDict`来操作保存数据。
 
 ## BaseDict类
 
-BaseDict类是CushyDict类的基础实现，提供了基本的字典结构和缓存操作。它可以用于缓存任何类型的Python对象，但不支持序列化和反序列化操作。
+BaseDict类是CushyDict类的基础实现，其只支持简单的二进制数据存储。
 
 ```python
 from cushy_storage import BaseDict
 
 # 初始化cache，保存在./data文件夹下
 cache = BaseDict('./data')
 # Base Dict只能存储二进制数据，可以用于流式传输
@@ -56,15 +57,19 @@
 value = cache['key']
 print(value)
 
 ```
 
 ## CushyDict类
 
-CushyDict类是BaseDict库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是一些简单的使用教程。
+CushyDict类是BaseDict库的高级实现，你可以像操作字典一样操作CushyDict；其增加了对值进行序列化和反序列化的功能，可以存储任意类型的数据。
+此外，CushyDict支持多种序列化算法 （pickle和json）和压缩算法（zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是
+一些简单的使用教程。
+
+- 存储Python基本数据类型
 
 ```python
 from cushy_storage import CushyDict
 
 # 初始化cache，保存在./data文件夹下
 cache = CushyDict('./data')
 
@@ -73,96 +78,100 @@
 
 cache['a'] = 1
 print(cache['a'])
 
 cache['b'] = "hello world"
 print(cache['b'])
 
-cache['arr'] = [1,2,3,4,5]
+cache['arr'] = [1, 2, 3, 4, 5]
 print(cache['arr'])
 
 ```
 
+> 以`cache['arr'] = [1, 2, 3, 4, 5]`为例，在指令这段代码之后，CushyDict会将数据存储到指令文件夹下。
+
 - 生成结果
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210730.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210837.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210825.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210809.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210757.png"/>
 
-- 如果在初始化的时候不传入参数，则默认保存在`./data`文件夹下
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-```
-
-
-- 判断key是否存在（和字典操作同理）
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict('./data')
-if 'key' in cache:
-    print("key exist")
-else:
-    print("key not exist")
-
-```
-
-- 用`CushyDict`存储对象信息
+- 存储自定义数据类型
 
 ```python
 from cushy_storage import CushyDict
 
 
 class User:
     def __init__(self, name, age):
         self.name = name
         self.age = age
 
 
 def main():
-    cache = CushyDict('./data', serialize='pickle')
+    cache = CushyDict(serialize='pickle')
     user = User("Jack", 18)
     cache['user'] = user
 
+    user = cache['user']
+    print(type(user))
     print(cache['user'].name)
     print(cache['user'].age)
 
 
 if __name__ == '__main__':
     main()
+```
+
+> 需要说明的是，如果你有定义复杂数据的需求，如List里面存json；或者你没有去文件下看原数据的需求，则推荐使用pickle的方式来进行数据存储。
+
+- 如果在初始化的时候不传入参数，则默认保存在`./cache`文件夹下
+
+```python
+from cushy_storage import CushyDict
 
+cache = CushyDict()
 ```
 
+- 判断key是否存在（和字典操作同理）
 
-## disk_cache装饰器函数
+```python
+from cushy_storage import CushyDict
 
-disk_cache装饰器函数可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
+cache = CushyDict()
+if 'key' in cache:
+    print("key exist")
+else:
+    print("key not exist")
+
+```
+
+## disk_cache装饰器
+
+disk_cache装饰器可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
 
 ```python
 from cushy_storage import disk_cache
 
+
 @disk_cache('./data')
 def my_func():
     return {'value': 42}
 
+
 result = my_func()
 
 ```
- 
- 
+
 # 待办
 
 - [ ] 提供单例模式解决方案，提供更加方便的工具类
 - [ ] 支持更多的压缩和序列化算法，以满足不同类型数据的需求
 - [ ] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
 - [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
 - [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
@@ -171,13 +180,17 @@
 - [ ] 改善文档结构和代码注释，方便用户理解和使用库
 - [ ] 支持Python3中的异步IO，提高程序的并发性和性能
 - [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
 - [ ] 支持更多数据格式的持久化方式，如json,xml的直接存储
 - [ ] 提供ORM框架，封装对象级的CRUD操作
 
 # 鸣谢
-本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage) 进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
 
-This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to RimoChan for his great work.
+本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage)
+进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
+
+This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to
+RimoChan for his great work.
 
 # 贡献
+
 如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
```

### Comparing `cushy-storage-1.0.3/cushy_storage/__init__.py` & `cushy-storage-1.0.4/cushy_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.3/cushy_storage/_core.py` & `cushy-storage-1.0.4/cushy_storage/_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 import zlib
 import lzma
 import json
 import pickle
 import hashlib
 import threading
 from pathlib import Path
-from typing import MutableMapping, Callable, Tuple, Union, Any
+from typing import MutableMapping, Callable, Tuple, Union, Any, List
 
+from cushy_storage.base import _List, BASE_TYPE
 from cushy_storage.utils import get_default_storage_path
 
 __all__ = ['BaseDict', 'CushyDict', 'disk_cache']
 
 # Compression algorithms and their corresponding functions
 _COMPRESS = {
     'zlib': (
@@ -55,15 +56,15 @@
     ),
 }
 
 # Locks for each hash value (hexadecimal representation of 0-255)
 _LOCKS = {hex(i)[2:].zfill(2): threading.Lock() for i in range(256)}
 
 
-def _cf(s: Union[str, Tuple[Callable, Callable], None], d: dict) -> Tuple[Callable, Callable]:
+def _method_convert_helper(s: Union[str, Tuple[Callable, Callable], None], d: dict) -> Tuple[Callable, Callable]:
     """
     Helper function to get the compression or serialization functions based on input parameter
     """
     if s is None:
         return lambda x: x, lambda x: x
     elif isinstance(s, str):
         return d[s]
@@ -74,15 +75,15 @@
 class BaseDict(MutableMapping[str, bytes]):
     def __init__(self, path: str, compress: Union[str, Tuple[Callable, Callable], None] = None):
         self.path = Path(path)
         if self.path.is_file():
             raise Exception('path has exist')  # Raise an exception if the path already exists as a file
         self.path.mkdir(parents=True, exist_ok=True)
         self.dirs = set()
-        self.compress, self.decompress = _cf(compress, _COMPRESS)
+        self.compress, self.decompress = _method_convert_helper(compress, _COMPRESS)
 
     def __contains__(self, k: str):
         """
         Check if the file exists in the cache
 
         Args:
             k: key
@@ -158,48 +159,53 @@
         """
         Args:
             path: the path to save
             compress: zlib or lzma
             serialize: json or pickle
         """
         super().__init__(path, compress)
-        self.serialize, self.deserialize = _cf(serialize, _SERIALIZATION)
+        self.serialize, self.deserialize = _method_convert_helper(serialize, _SERIALIZATION)
 
     def __getitem__(self, k: str):
-        return self.deserialize(super().__getitem__(k))
+        ret = self.deserialize(super().__getitem__(k))
+
+        if isinstance(ret, list):
+            ret: List = _List(ret)
+        return ret
 
     def __setitem__(self, k: str, v: Any):
+        if isinstance(v, list) and self.deserialize is json.loads and len(v) > 0 and type(v[0]) not in BASE_TYPE:
+            raise ValueError((
+                f"Can not use 'json' to serialize your '{type(v[0])}' data in '{k}'. If you want to store "
+                "complex data or custom data, please use 'pickle' to serialize."
+            ))
         return super().__setitem__(k, self.serialize(v))
 
 
-_EXT = {
-    'pickle': 'pkl',
-    'json': 'json',
-}
-
-
 def disk_cache(path: str = None, compress: str = None, serialize: str = 'json'):
     """
     Decorator that caches the output of a function to disk
     """
-    ext = _EXT.get(serialize, '_')
-    dump = _cf(serialize, _SERIALIZATION)[0]
+    if serialize not in ['pickle', 'json']:
+        ValueError("Your serializer must be 'pickle' or 'json'")
+    dump = _method_convert_helper(serialize, _SERIALIZATION)[0]
 
     def decorator(func):
         nonlocal path
         name = func.__name__
         if path is None:
             # If no cache path is specified, create a default one based on the function name and serialization algorithm
             path = f'./_cushycache_{name}_{serialize}'
         map = CushyDict(path, serialize=serialize, compress=compress)
 
         def cached_func(*args, **kwargs):
             # Serialize the function arguments and use their MD5 hash as the cache key
             input_data = [name, args, kwargs]
             md5 = hashlib.md5(dump(input_data)).hexdigest()
+            ext = 'pkl' if serialize == 'pickle' else 'json'
             filename = f'{md5}.{ext}'
 
             if filename in map:
                 # If the cached output exists, return it
                 input_data, output_data = map[filename]
                 return output_data
             else:
```

### Comparing `cushy-storage-1.0.3/cushy_storage/utils.py` & `cushy-storage-1.0.4/cushy_storage/utils.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.3/cushy_storage.egg-info/PKG-INFO` & `cushy-storage-1.0.4/cushy_storage.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.0.3
+Version: 1.0.4
 Summary: A data local persistence framework library
 Home-page: https://github.com/Undertone0809/cushy-storage
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: storage,serialization,json,cushy-storage,cushy_storage
 Classifier: Development Status :: 3 - Alpha
@@ -38,39 +38,40 @@
         <img src="https://static.pepy.tech/personalized-badge/cushy-socket?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
    </a>
 </p>
 
 [English](/README_en.md) [中文](/README.md)
 
 # 简介
+
 cushy-storage是一个基于磁盘缓存的Python库，可以将Python对象序列化后缓存到磁盘中，以便下次使用时直接读取，从而提高程序的执行效率。另一方面，
 cushy-storage让你无需花费精力在如何制订一套数据存储规范上，字典般的操作可以减少很多开发的成本。
 
 # 特性
-- 可以方便的将数据进行本地磁盘存储
+
+- 可以方便地将数据(基本数据类型、自定义数据类型)进行本地磁盘存储
 - 免去了直接操作文件的工作
 - 像操作dict一样读写，十分方便
 - 提供序列化操作
 - 提供多种数据压缩方式
 
-
 # 安装
 
 ```bash
 pip install cushy-storage --upgrade 
 ```
 
 # 快速上手
 
 `cushy-storage` 的使用主要分为三个类，`BaseDict` `CushyDict` `disk_cache`，其中`CushyDict`是`BaseDict`的增强版，可以实现
 `BaseDict`的所有功能，还增加了相应序列化操作，因此推荐直接使用`CushyDict`来操作保存数据。
 
 ## BaseDict类
 
-BaseDict类是CushyDict类的基础实现，提供了基本的字典结构和缓存操作。它可以用于缓存任何类型的Python对象，但不支持序列化和反序列化操作。
+BaseDict类是CushyDict类的基础实现，其只支持简单的二进制数据存储。
 
 ```python
 from cushy_storage import BaseDict
 
 # 初始化cache，保存在./data文件夹下
 cache = BaseDict('./data')
 # Base Dict只能存储二进制数据，可以用于流式传输
@@ -78,15 +79,19 @@
 value = cache['key']
 print(value)
 
 ```
 
 ## CushyDict类
 
-CushyDict类是BaseDict库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是一些简单的使用教程。
+CushyDict类是BaseDict库的高级实现，你可以像操作字典一样操作CushyDict；其增加了对值进行序列化和反序列化的功能，可以存储任意类型的数据。
+此外，CushyDict支持多种序列化算法 （pickle和json）和压缩算法（zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是
+一些简单的使用教程。
+
+- 存储Python基本数据类型
 
 ```python
 from cushy_storage import CushyDict
 
 # 初始化cache，保存在./data文件夹下
 cache = CushyDict('./data')
 
@@ -95,96 +100,100 @@
 
 cache['a'] = 1
 print(cache['a'])
 
 cache['b'] = "hello world"
 print(cache['b'])
 
-cache['arr'] = [1,2,3,4,5]
+cache['arr'] = [1, 2, 3, 4, 5]
 print(cache['arr'])
 
 ```
 
+> 以`cache['arr'] = [1, 2, 3, 4, 5]`为例，在指令这段代码之后，CushyDict会将数据存储到指令文件夹下。
+
 - 生成结果
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210730.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210837.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210825.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210809.png"/>
 
 <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210757.png"/>
 
-- 如果在初始化的时候不传入参数，则默认保存在`./data`文件夹下
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict()
-```
-
-
-- 判断key是否存在（和字典操作同理）
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict('./data')
-if 'key' in cache:
-    print("key exist")
-else:
-    print("key not exist")
-
-```
-
-- 用`CushyDict`存储对象信息
+- 存储自定义数据类型
 
 ```python
 from cushy_storage import CushyDict
 
 
 class User:
     def __init__(self, name, age):
         self.name = name
         self.age = age
 
 
 def main():
-    cache = CushyDict('./data', serialize='pickle')
+    cache = CushyDict(serialize='pickle')
     user = User("Jack", 18)
     cache['user'] = user
 
+    user = cache['user']
+    print(type(user))
     print(cache['user'].name)
     print(cache['user'].age)
 
 
 if __name__ == '__main__':
     main()
+```
+
+> 需要说明的是，如果你有定义复杂数据的需求，如List里面存json；或者你没有去文件下看原数据的需求，则推荐使用pickle的方式来进行数据存储。
+
+- 如果在初始化的时候不传入参数，则默认保存在`./cache`文件夹下
+
+```python
+from cushy_storage import CushyDict
 
+cache = CushyDict()
 ```
 
+- 判断key是否存在（和字典操作同理）
 
-## disk_cache装饰器函数
+```python
+from cushy_storage import CushyDict
 
-disk_cache装饰器函数可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
+cache = CushyDict()
+if 'key' in cache:
+    print("key exist")
+else:
+    print("key not exist")
+
+```
+
+## disk_cache装饰器
+
+disk_cache装饰器可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
 
 ```python
 from cushy_storage import disk_cache
 
+
 @disk_cache('./data')
 def my_func():
     return {'value': 42}
 
+
 result = my_func()
 
 ```
- 
- 
+
 # 待办
 
 - [ ] 提供单例模式解决方案，提供更加方便的工具类
 - [ ] 支持更多的压缩和序列化算法，以满足不同类型数据的需求
 - [ ] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
 - [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
 - [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
@@ -193,13 +202,17 @@
 - [ ] 改善文档结构和代码注释，方便用户理解和使用库
 - [ ] 支持Python3中的异步IO，提高程序的并发性和性能
 - [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
 - [ ] 支持更多数据格式的持久化方式，如json,xml的直接存储
 - [ ] 提供ORM框架，封装对象级的CRUD操作
 
 # 鸣谢
-本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage) 进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
 
-This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to RimoChan for his great work.
+本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage)
+进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
+
+This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to
+RimoChan for his great work.
 
 # 贡献
+
 如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
```

### Comparing `cushy-storage-1.0.3/setup.py` & `cushy-storage-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="cushy-storage",
-    version="1.0.3",
+    version="1.0.4",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A data local persistence framework library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/cushy-storage",
     packages=setuptools.find_packages(),
```

### Comparing `cushy-storage-1.0.3/tests/test_base_dict.py` & `cushy-storage-1.0.4/tests/test_base_dict.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.3/tests/test_cushy_dict.py` & `cushy-storage-1.0.4/tests/test_cushy_dict.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.3/tests/test_dict_cache.py` & `cushy-storage-1.0.4/tests/test_dict_cache.py`

 * *Files identical despite different names*

