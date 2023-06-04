# Comparing `tmp/feign-python-0.0.1.tar.gz` & `tmp/feign-python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feign-python-0.0.1.tar", last modified: Sun Aug 21 06:46:42 2022, max compression
+gzip compressed data, was "feign-python-0.0.3.tar", last modified: Sun Jun  4 02:27:09 2023, max compression
```

## Comparing `feign-python-0.0.1.tar` & `feign-python-0.0.3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.351955 feign-python-0.0.1/
--rw-rw-rw-   0        0        0    35181 2022-08-21 04:28:03.000000 feign-python-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      556 2022-08-21 06:46:42.350964 feign-python-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7124 2022-08-21 04:36:30.000000 feign-python-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.239363 feign-python-0.0.1/feign_python.egg-info/
--rw-rw-rw-   0        0        0      556 2022-08-21 06:46:42.000000 feign-python-0.0.1/feign_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2381 2022-08-21 06:46:42.000000 feign-python-0.0.1/feign_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-21 06:46:42.000000 feign-python-0.0.1/feign_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2022-08-21 06:46:42.000000 feign-python-0.0.1/feign_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.240355 feign-python-0.0.1/ldj/
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.241843 feign-python-0.0.1/ldj/center/
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/center/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.246308 feign-python-0.0.1/ldj/center/nacos/
--rw-rw-rw-   0        0        0     2715 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/center/nacos/NacosClient.py
--rw-rw-rw-   0        0        0     2844 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/center/nacos/NacosIns.py
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/center/nacos/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.249282 feign-python-0.0.1/ldj/center/prop/
--rw-rw-rw-   0        0        0     1674 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/center/prop/Properties.py
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/center/prop/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.253747 feign-python-0.0.1/ldj/common/
--rw-rw-rw-   0        0        0      352 2022-08-21 03:22:00.000000 feign-python-0.0.1/ldj/common/Cache.py
--rw-rw-rw-   0        0        0      353 2022-08-21 01:10:57.000000 feign-python-0.0.1/ldj/common/Constant.py
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/common/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.256723 feign-python-0.0.1/ldj/config/
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/config/__init__.py
--rw-rw-rw-   0        0        0      686 2022-08-21 06:26:05.000000 feign-python-0.0.1/ldj/config/settings.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.270612 feign-python-0.0.1/ldj/example/
--rw-rw-rw-   0        0        0      770 2022-08-21 01:07:19.000000 feign-python-0.0.1/ldj/example/DictApi.py
--rw-rw-rw-   0        0        0      869 2022-08-21 04:08:05.000000 feign-python-0.0.1/ldj/example/DictApi2.py
--rw-rw-rw-   0        0        0      874 2022-08-21 03:42:53.000000 feign-python-0.0.1/ldj/example/DictApi2NoCenter.py
--rw-rw-rw-   0        0        0      923 2022-08-21 03:37:12.000000 feign-python-0.0.1/ldj/example/DictApiNoCenter.py
--rw-rw-rw-   0        0        0      519 2022-08-21 04:09:02.000000 feign-python-0.0.1/ldj/example/ExampleConfig.py
--rw-rw-rw-   0        0        0      846 2022-08-21 03:44:11.000000 feign-python-0.0.1/ldj/example/TestDictApi.py
--rw-rw-rw-   0        0        0      896 2022-08-21 01:10:01.000000 feign-python-0.0.1/ldj/example/TestDictApi2.py
--rw-rw-rw-   0        0        0      844 2022-08-21 03:31:00.000000 feign-python-0.0.1/ldj/example/TestDictApi2NoCenter.py
--rw-rw-rw-   0        0        0      807 2022-08-21 03:37:12.000000 feign-python-0.0.1/ldj/example/TestDictApiNoCenter.py
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/example/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.273588 feign-python-0.0.1/ldj/example/dto/
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/example/dto/__init__.py
--rw-rw-rw-   0        0        0      405 2022-08-19 13:52:54.000000 feign-python-0.0.1/ldj/example/dto/models.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.276595 feign-python-0.0.1/ldj/example/interceptor/
--rw-rw-rw-   0        0        0      704 2022-08-21 03:58:29.000000 feign-python-0.0.1/ldj/example/interceptor/MyInterceptor.py
--rw-rw-rw-   0        0        0      106 2022-08-21 03:57:45.000000 feign-python-0.0.1/ldj/example/interceptor/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.278052 feign-python-0.0.1/ldj/feign/
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.285491 feign-python-0.0.1/ldj/feign/center/
--rw-rw-rw-   0        0        0     1373 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/center/NacosCenter.py
--rw-rw-rw-   0        0        0      421 2022-08-19 14:28:21.000000 feign-python-0.0.1/ldj/feign/center/RegisterCenter.py
--rw-rw-rw-   0        0        0     1570 2022-08-21 01:29:28.000000 feign-python-0.0.1/ldj/feign/center/RegisterCenterHelper.py
--rw-rw-rw-   0        0        0      810 2022-08-19 08:45:48.000000 feign-python-0.0.1/ldj/feign/center/RegisterSelect.py
--rw-rw-rw-   0        0        0      144 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/center/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.288963 feign-python-0.0.1/ldj/feign/context/
--rw-rw-rw-   0        0        0      989 2022-08-21 03:26:15.000000 feign-python-0.0.1/ldj/feign/context/ServiceContext.py
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/context/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.296404 feign-python-0.0.1/ldj/feign/decorator/
--rw-rw-rw-   0        0        0     4842 2022-08-21 03:52:27.000000 feign-python-0.0.1/ldj/feign/decorator/Api.py
--rw-rw-rw-   0        0        0     3480 2022-08-21 03:26:15.000000 feign-python-0.0.1/ldj/feign/decorator/Feign.py
--rw-rw-rw-   0        0        0     4931 2022-08-21 03:52:37.000000 feign-python-0.0.1/ldj/feign/decorator/FeignApi.py
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/decorator/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.303846 feign-python-0.0.1/ldj/feign/enums/
--rw-rw-rw-   0        0        0      410 2022-08-19 14:37:17.000000 feign-python-0.0.1/ldj/feign/enums/BaseEnum.py
--rw-rw-rw-   0        0        0      302 2022-08-19 09:09:26.000000 feign-python-0.0.1/ldj/feign/enums/Method.py
--rw-rw-rw-   0        0        0      303 2022-08-19 14:37:54.000000 feign-python-0.0.1/ldj/feign/enums/RegisterCenterType.py
--rw-rw-rw-   0        0        0      460 2022-08-19 14:34:07.000000 feign-python-0.0.1/ldj/feign/enums/RouterType.py
--rw-rw-rw-   0        0        0      144 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.310293 feign-python-0.0.1/ldj/feign/exception/
--rw-rw-rw-   0        0        0      229 2022-08-19 09:39:50.000000 feign-python-0.0.1/ldj/feign/exception/AuthException.py
--rw-rw-rw-   0        0        0      233 2022-08-19 09:41:02.000000 feign-python-0.0.1/ldj/feign/exception/BusinessException.py
--rw-rw-rw-   0        0        0      247 2022-08-19 09:40:55.000000 feign-python-0.0.1/ldj/feign/exception/FeignException.py
--rw-rw-rw-   0        0        0      144 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.315748 feign-python-0.0.1/ldj/feign/exception/handler/
--rw-rw-rw-   0        0        0      331 2022-08-21 04:01:24.000000 feign-python-0.0.1/ldj/feign/exception/handler/DefaultExceptionHandler.py
--rw-rw-rw-   0        0        0      238 2022-08-19 10:15:33.000000 feign-python-0.0.1/ldj/feign/exception/handler/ExceptionHandler.py
--rw-rw-rw-   0        0        0      106 2022-08-19 09:40:55.000000 feign-python-0.0.1/ldj/feign/exception/handler/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.320212 feign-python-0.0.1/ldj/feign/interceptor/
--rw-rw-rw-   0        0        0     2216 2022-08-21 03:52:08.000000 feign-python-0.0.1/ldj/feign/interceptor/DefaultInterceptor.py
--rw-rw-rw-   0        0        0     1195 2022-08-21 03:50:41.000000 feign-python-0.0.1/ldj/feign/interceptor/Interceptor.py
--rw-rw-rw-   0        0        0      144 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/interceptor/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.329141 feign-python-0.0.1/ldj/feign/model/
--rw-rw-rw-   0        0        0      344 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/model/HostInfo.py
--rw-rw-rw-   0        0        0      414 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/model/Page.py
--rw-rw-rw-   0        0        0      511 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/model/Request.py
--rw-rw-rw-   0        0        0     1451 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/model/Response.py
--rw-rw-rw-   0        0        0      655 2022-08-21 03:26:15.000000 feign-python-0.0.1/ldj/feign/model/ServiceInfo.py
--rw-rw-rw-   0        0        0      144 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/model/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.338069 feign-python-0.0.1/ldj/feign/router/
--rw-rw-rw-   0        0        0      789 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/router/HashRouter.py
--rw-rw-rw-   0        0        0      615 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/router/RandomRouter.py
--rw-rw-rw-   0        0        0      751 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/router/RoundRobinRouter.py
--rw-rw-rw-   0        0        0      389 2022-08-19 14:34:55.000000 feign-python-0.0.1/ldj/feign/router/Router.py
--rw-rw-rw-   0        0        0     1318 2022-08-19 14:34:55.000000 feign-python-0.0.1/ldj/feign/router/RouterHelper.py
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/router/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.343028 feign-python-0.0.1/ldj/feign/seria/
--rw-rw-rw-   0        0        0      173 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/seria/Deserialize.py
--rw-rw-rw-   0        0        0      171 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/seria/Serialize.py
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/seria/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 06:46:42.348979 feign-python-0.0.1/ldj/feign/utils/
--rw-rw-rw-   0        0        0     1067 2022-08-19 08:57:50.000000 feign-python-0.0.1/ldj/feign/utils/IpUtil.py
--rw-rw-rw-   0        0        0      953 2022-08-19 09:31:00.000000 feign-python-0.0.1/ldj/feign/utils/ReflectUtil.py
--rw-rw-rw-   0        0        0      813 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/utils/UrlUtil.py
--rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.1/ldj/feign/utils/__init__.py
--rw-rw-rw-   0        0        0       42 2022-08-21 06:46:42.351955 feign-python-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1004 2022-08-21 06:45:58.000000 feign-python-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.640226 feign-python-0.0.3/
+-rw-rw-rw-   0        0        0    35181 2022-08-21 04:28:03.000000 feign-python-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      506 2023-06-04 02:27:09.640226 feign-python-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7362 2022-08-21 07:18:25.000000 feign-python-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.508577 feign-python-0.0.3/feign_python.egg-info/
+-rw-rw-rw-   0        0        0      506 2023-06-04 02:27:09.000000 feign-python-0.0.3/feign_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2381 2023-06-04 02:27:09.000000 feign-python-0.0.3/feign_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 02:27:09.000000 feign-python-0.0.3/feign_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-04 02:27:09.000000 feign-python-0.0.3/feign_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.509574 feign-python-0.0.3/ldj/
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.510572 feign-python-0.0.3/ldj/center/
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/center/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.514561 feign-python-0.0.3/ldj/center/nacos/
+-rw-rw-rw-   0        0        0     2715 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/center/nacos/NacosClient.py
+-rw-rw-rw-   0        0        0     2844 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/center/nacos/NacosIns.py
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/center/nacos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.517553 feign-python-0.0.3/ldj/center/prop/
+-rw-rw-rw-   0        0        0     1674 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/center/prop/Properties.py
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/center/prop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.521542 feign-python-0.0.3/ldj/common/
+-rw-rw-rw-   0        0        0      352 2022-08-21 03:22:00.000000 feign-python-0.0.3/ldj/common/Cache.py
+-rw-rw-rw-   0        0        0      353 2022-08-21 01:10:57.000000 feign-python-0.0.3/ldj/common/Constant.py
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.523537 feign-python-0.0.3/ldj/config/
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/config/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-08-21 06:26:05.000000 feign-python-0.0.3/ldj/config/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.540492 feign-python-0.0.3/ldj/example/
+-rw-rw-rw-   0        0        0      761 2023-06-04 02:16:31.000000 feign-python-0.0.3/ldj/example/DictApi.py
+-rw-rw-rw-   0        0        0      869 2022-08-21 04:08:05.000000 feign-python-0.0.3/ldj/example/DictApi2.py
+-rw-rw-rw-   0        0        0      874 2022-08-21 03:42:53.000000 feign-python-0.0.3/ldj/example/DictApi2NoCenter.py
+-rw-rw-rw-   0        0        0      923 2022-08-21 03:37:12.000000 feign-python-0.0.3/ldj/example/DictApiNoCenter.py
+-rw-rw-rw-   0        0        0      519 2022-08-21 04:09:02.000000 feign-python-0.0.3/ldj/example/ExampleConfig.py
+-rw-rw-rw-   0        0        0      846 2022-08-21 03:44:11.000000 feign-python-0.0.3/ldj/example/TestDictApi.py
+-rw-rw-rw-   0        0        0      896 2022-08-21 01:10:01.000000 feign-python-0.0.3/ldj/example/TestDictApi2.py
+-rw-rw-rw-   0        0        0      844 2022-08-21 03:31:00.000000 feign-python-0.0.3/ldj/example/TestDictApi2NoCenter.py
+-rw-rw-rw-   0        0        0      807 2022-08-21 03:37:12.000000 feign-python-0.0.3/ldj/example/TestDictApiNoCenter.py
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.543484 feign-python-0.0.3/ldj/example/dto/
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/example/dto/__init__.py
+-rw-rw-rw-   0        0        0      405 2022-08-19 13:52:54.000000 feign-python-0.0.3/ldj/example/dto/models.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.547474 feign-python-0.0.3/ldj/example/interceptor/
+-rw-rw-rw-   0        0        0      704 2022-08-21 03:58:29.000000 feign-python-0.0.3/ldj/example/interceptor/MyInterceptor.py
+-rw-rw-rw-   0        0        0      106 2022-08-21 03:57:45.000000 feign-python-0.0.3/ldj/example/interceptor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.549467 feign-python-0.0.3/ldj/feign/
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.558444 feign-python-0.0.3/ldj/feign/center/
+-rw-rw-rw-   0        0        0     1373 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/center/NacosCenter.py
+-rw-rw-rw-   0        0        0      421 2022-08-19 14:28:21.000000 feign-python-0.0.3/ldj/feign/center/RegisterCenter.py
+-rw-rw-rw-   0        0        0     1570 2022-08-21 01:29:28.000000 feign-python-0.0.3/ldj/feign/center/RegisterCenterHelper.py
+-rw-rw-rw-   0        0        0      810 2022-08-19 08:45:48.000000 feign-python-0.0.3/ldj/feign/center/RegisterSelect.py
+-rw-rw-rw-   0        0        0      144 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/center/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.560438 feign-python-0.0.3/ldj/feign/context/
+-rw-rw-rw-   0        0        0      989 2022-08-21 03:26:15.000000 feign-python-0.0.3/ldj/feign/context/ServiceContext.py
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/context/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.568417 feign-python-0.0.3/ldj/feign/decorator/
+-rw-rw-rw-   0        0        0     4842 2022-08-21 03:52:27.000000 feign-python-0.0.3/ldj/feign/decorator/Api.py
+-rw-rw-rw-   0        0        0     3480 2022-08-21 03:26:15.000000 feign-python-0.0.3/ldj/feign/decorator/Feign.py
+-rw-rw-rw-   0        0        0     4895 2023-05-18 10:19:13.000000 feign-python-0.0.3/ldj/feign/decorator/FeignApi.py
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/decorator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.579388 feign-python-0.0.3/ldj/feign/enums/
+-rw-rw-rw-   0        0        0      410 2022-08-19 14:37:17.000000 feign-python-0.0.3/ldj/feign/enums/BaseEnum.py
+-rw-rw-rw-   0        0        0      302 2022-08-19 09:09:26.000000 feign-python-0.0.3/ldj/feign/enums/Method.py
+-rw-rw-rw-   0        0        0      303 2022-08-19 14:37:54.000000 feign-python-0.0.3/ldj/feign/enums/RegisterCenterType.py
+-rw-rw-rw-   0        0        0      460 2022-08-19 14:34:07.000000 feign-python-0.0.3/ldj/feign/enums/RouterType.py
+-rw-rw-rw-   0        0        0      144 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.588364 feign-python-0.0.3/ldj/feign/exception/
+-rw-rw-rw-   0        0        0      229 2022-08-19 09:39:50.000000 feign-python-0.0.3/ldj/feign/exception/AuthException.py
+-rw-rw-rw-   0        0        0      233 2022-08-19 09:41:02.000000 feign-python-0.0.3/ldj/feign/exception/BusinessException.py
+-rw-rw-rw-   0        0        0      247 2022-08-19 09:40:55.000000 feign-python-0.0.3/ldj/feign/exception/FeignException.py
+-rw-rw-rw-   0        0        0      144 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.594348 feign-python-0.0.3/ldj/feign/exception/handler/
+-rw-rw-rw-   0        0        0      331 2022-08-21 04:01:24.000000 feign-python-0.0.3/ldj/feign/exception/handler/DefaultExceptionHandler.py
+-rw-rw-rw-   0        0        0      238 2022-08-19 10:15:33.000000 feign-python-0.0.3/ldj/feign/exception/handler/ExceptionHandler.py
+-rw-rw-rw-   0        0        0      106 2022-08-19 09:40:55.000000 feign-python-0.0.3/ldj/feign/exception/handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.600332 feign-python-0.0.3/ldj/feign/interceptor/
+-rw-rw-rw-   0        0        0     2216 2022-08-21 03:52:08.000000 feign-python-0.0.3/ldj/feign/interceptor/DefaultInterceptor.py
+-rw-rw-rw-   0        0        0     1195 2022-08-21 03:50:41.000000 feign-python-0.0.3/ldj/feign/interceptor/Interceptor.py
+-rw-rw-rw-   0        0        0      144 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/interceptor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.611303 feign-python-0.0.3/ldj/feign/model/
+-rw-rw-rw-   0        0        0      344 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/model/HostInfo.py
+-rw-rw-rw-   0        0        0      414 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/model/Page.py
+-rw-rw-rw-   0        0        0      511 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/model/Request.py
+-rw-rw-rw-   0        0        0     1437 2023-06-04 02:16:33.000000 feign-python-0.0.3/ldj/feign/model/Response.py
+-rw-rw-rw-   0        0        0      655 2022-08-21 03:26:15.000000 feign-python-0.0.3/ldj/feign/model/ServiceInfo.py
+-rw-rw-rw-   0        0        0      144 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.623271 feign-python-0.0.3/ldj/feign/router/
+-rw-rw-rw-   0        0        0      789 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/router/HashRouter.py
+-rw-rw-rw-   0        0        0      615 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/router/RandomRouter.py
+-rw-rw-rw-   0        0        0      751 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/router/RoundRobinRouter.py
+-rw-rw-rw-   0        0        0      389 2022-08-19 14:34:55.000000 feign-python-0.0.3/ldj/feign/router/Router.py
+-rw-rw-rw-   0        0        0     1318 2022-08-19 14:34:55.000000 feign-python-0.0.3/ldj/feign/router/RouterHelper.py
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/router/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.628257 feign-python-0.0.3/ldj/feign/seria/
+-rw-rw-rw-   0        0        0      173 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/seria/Deserialize.py
+-rw-rw-rw-   0        0        0      171 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/seria/Serialize.py
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/seria/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:27:09.637239 feign-python-0.0.3/ldj/feign/utils/
+-rw-rw-rw-   0        0        0     1067 2022-08-19 08:57:50.000000 feign-python-0.0.3/ldj/feign/utils/IpUtil.py
+-rw-rw-rw-   0        0        0      955 2023-05-18 09:09:11.000000 feign-python-0.0.3/ldj/feign/utils/ReflectUtil.py
+-rw-rw-rw-   0        0        0      813 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/utils/UrlUtil.py
+-rw-rw-rw-   0        0        0      145 2022-08-19 08:33:50.000000 feign-python-0.0.3/ldj/feign/utils/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-04 02:27:09.641223 feign-python-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1004 2023-06-04 02:16:42.000000 feign-python-0.0.3/setup.py
```

### Comparing `feign-python-0.0.1/LICENSE` & `feign-python-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/README.md` & `feign-python-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 ### feign-python
 ### 项目介绍
 ```markdown
    项目描述: 本项目为feign的python实现，方便python项目与微服务项目快捷集成,目前只实现与注册中心nacos2集成,客户端负载支持(HASH,RANDOM,ROUND_ROBIN)默认IP-HASH
    作者: 黑肱
    邮箱: zuiwoxing@qq.com
 ```
+
 ### 项目安装
 ```
 pip install feign-python
-``` 
+```
 ### 使用示例
 #### 一. 第一种使用方式
 ```python
 from requests import Response
 from ldj.feign.decorator.FeignApi import FeignApi
 from ldj.example.dto.models import QueryDto
 from ldj.feign.enums.Method import Method
@@ -199,8 +200,30 @@
  异常默认是通过loguru来做日志记录,其默认实现 DefaultExceptionHandler。如果需要自定义异常处理只需要继承ExceptionHandler
  然后重写 handler 方法就可以（具体可参考 DefaultExceptionHandler实现)。 然后再将自定义异常配置到Feign中即可
 
 my_exception_handler = MyExceptionHandler()
 @Feign(prefix="/shared/dict/api/dict", serviceId="shared", exceptionHandler=my_exception_handler, name="共享服务-字典服务")
 class DictApi2:
  pass
-```
+```
+
+
+
+
+#### 交流
+
+<div>
+  <span>
+  <img src="images/weixin.jpg" width="200" height="200">
+  </span>
+</div>
+
+#### 打赏
+
+<div>
+  <span>
+  <img src="images/support.jpg" width="200" height="200">
+  </span>
+</div>
+
+
+
```

### Comparing `feign-python-0.0.1/feign_python.egg-info/SOURCES.txt` & `feign-python-0.0.3/feign_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/center/nacos/NacosClient.py` & `feign-python-0.0.3/ldj/center/nacos/NacosClient.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/center/nacos/NacosIns.py` & `feign-python-0.0.3/ldj/center/nacos/NacosIns.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/center/prop/Properties.py` & `feign-python-0.0.3/ldj/center/prop/Properties.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/config/settings.py` & `feign-python-0.0.3/ldj/config/settings.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/example/DictApi.py` & `feign-python-0.0.3/ldj/example/DictApi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*-
 # 描述:
 # @author:  <a href="mailto:zuiwoxing@qq.com">dejian.liu</a>
 # @date:  2022-08-15 16:53
-from requests import Response
+from requests import
 from ldj.feign.decorator.FeignApi import FeignApi
 from ldj.example.dto.models import QueryDto
 from ldj.feign.enums.Method import Method
 
 
 class DictApi:
```

### Comparing `feign-python-0.0.1/ldj/example/DictApi2.py` & `feign-python-0.0.3/ldj/example/DictApi2.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/example/DictApi2NoCenter.py` & `feign-python-0.0.3/ldj/example/DictApi2NoCenter.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/example/DictApiNoCenter.py` & `feign-python-0.0.3/ldj/example/DictApiNoCenter.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/example/ExampleConfig.py` & `feign-python-0.0.3/ldj/example/ExampleConfig.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/example/TestDictApi.py` & `feign-python-0.0.3/ldj/example/TestDictApi.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/example/TestDictApi2.py` & `feign-python-0.0.3/ldj/example/TestDictApi2.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/example/TestDictApi2NoCenter.py` & `feign-python-0.0.3/ldj/example/TestDictApi2NoCenter.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/example/TestDictApiNoCenter.py` & `feign-python-0.0.3/ldj/example/TestDictApiNoCenter.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/example/interceptor/MyInterceptor.py` & `feign-python-0.0.3/ldj/example/interceptor/MyInterceptor.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/center/NacosCenter.py` & `feign-python-0.0.3/ldj/feign/center/NacosCenter.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/center/RegisterCenterHelper.py` & `feign-python-0.0.3/ldj/feign/center/RegisterCenterHelper.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/center/RegisterSelect.py` & `feign-python-0.0.3/ldj/feign/center/RegisterSelect.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/context/ServiceContext.py` & `feign-python-0.0.3/ldj/feign/context/ServiceContext.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/decorator/Api.py` & `feign-python-0.0.3/ldj/feign/decorator/Api.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/decorator/Feign.py` & `feign-python-0.0.3/ldj/feign/decorator/Feign.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/decorator/FeignApi.py` & `feign-python-0.0.3/ldj/feign/decorator/FeignApi.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,18 +88,18 @@
                 # 从注册中心获取
                 if service_url is None or len(service_url) == 0:
                     serverInfo = RegisterCenterHelper.get_service_server(self.serviceId, self.groupName)
                     service_url = RouterHelper.get_host_url(settings.HTTP_PROTOCOL, serverInfo)
                 finalUrl = UrlUtil.wrap_url(self.uri, prefix=service_url)
                 # 请求前拦截器
                 pr: ProcessRequest = self.interceptor.encode(method=method,
-                                                                      headers=headers,
-                                                                      params=params,
-                                                                      body=body,
-                                                                      data=data)
+                                                             headers=headers,
+                                                             params=params,
+                                                             body=body,
+                                                             data=data)
                 # 执行请求
                 resp = requests.request(method.name, finalUrl,
                                         params=pr.params, json=pr.body,
                                         headers=pr.headers,
                                         data=pr.data, timeout=self.timeout)
                 # 响应处理
                 func_result = self.interceptor.decode(resp)
```

### Comparing `feign-python-0.0.1/ldj/feign/interceptor/DefaultInterceptor.py` & `feign-python-0.0.3/ldj/feign/interceptor/DefaultInterceptor.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/interceptor/Interceptor.py` & `feign-python-0.0.3/ldj/feign/interceptor/Interceptor.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/model/Response.py` & `feign-python-0.0.3/ldj/feign/model/Response.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,41 +14,41 @@
     :param msg 响应消息
     :param code 业务编码
     :param data 业务数据
     """
     status: int = Constant.HTTP_SUCCESS
     message: str = ""
     code: int = Constant.BIZ_SUCCESS
-    result: object = None
+    data: object = None
 
     def toJson(self):
         return self.json()
 
     @staticmethod
-    def success(status=None, message=None, code=None, result=None):
+    def success(status=None, message=None, code=None, data=None):
         if status is None:
             status = Constant.HTTP_SUCCESS
         if message is None:
             message = "ok"
         if code is None:
             code = Constant.BIZ_SUCCESS
         res = Response()
         res.status = status
         res.message = message
         res.code = code
-        res.result = result
+        res.data = data
         return res
 
     @staticmethod
-    def fail(status=None, message=None, code=None, result=None):
+    def fail(status=None, message=None, code=None, data=None):
         res = Response()
         if status is None:
             status = Constant.HTTP_ERROR
         if message is None:
             message = "error"
         if code is None:
             code = Constant.BIZ_ERROR
         res.status = status
         res.message = message
         res.code = code
-        res.result = result
+        res.data = data
         return res
```

### Comparing `feign-python-0.0.1/ldj/feign/model/ServiceInfo.py` & `feign-python-0.0.3/ldj/feign/model/ServiceInfo.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/router/HashRouter.py` & `feign-python-0.0.3/ldj/feign/router/HashRouter.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/router/RandomRouter.py` & `feign-python-0.0.3/ldj/feign/router/RandomRouter.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/router/RoundRobinRouter.py` & `feign-python-0.0.3/ldj/feign/router/RoundRobinRouter.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/router/RouterHelper.py` & `feign-python-0.0.3/ldj/feign/router/RouterHelper.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/utils/IpUtil.py` & `feign-python-0.0.3/ldj/feign/utils/IpUtil.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/ldj/feign/utils/ReflectUtil.py` & `feign-python-0.0.3/ldj/feign/utils/ReflectUtil.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # 描述:
 # @author:  <a href="mailto:zuiwoxing@qq.com">dejian.liu</a>
 # @date:  2022-08-19 15:02
 
 import ast
 import inspect
 
+
 class ReflectUtil:
 
     @staticmethod
     def get_decorators(cls):
         target = cls
         decorators = {}
```

### Comparing `feign-python-0.0.1/ldj/feign/utils/UrlUtil.py` & `feign-python-0.0.3/ldj/feign/utils/UrlUtil.py`

 * *Files identical despite different names*

### Comparing `feign-python-0.0.1/setup.py` & `feign-python-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 描述:
 # @author:  <a href="mailto:zuiwoxing@qq.com">dejian.liu</a>
 # @date:  2022-08-10 14:02
 from setuptools import setup, find_packages
 
 setup(
     name="feign-python",
-    version="0.0.1",
+    version="0.0.3",
     author="黑肱",
     author_email="zuiwoxing@qq.com",
     description="feign python实现",
     long_description_content_type="text/markdown",
     url="https://github.com/openandopen/feign-python",
     packages= find_packages(),
     classifiers=[
```

