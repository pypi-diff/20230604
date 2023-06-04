# Comparing `tmp/translategram-0.1.1.tar.gz` & `tmp/translategram-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translategram-0.1.1.tar", last modified: Tue May 23 00:42:39 2023, max compression
+gzip compressed data, was "translategram-0.1.2.tar", last modified: Sun Jun  4 16:06:14 2023, max compression
```

## Comparing `translategram-0.1.1.tar` & `translategram-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-23 00:42:39.419198 translategram-0.1.1/
--rw-r--r--   0 akbar     (1000) akbar     (1000)     1069 2023-05-06 14:12:58.000000 translategram-0.1.1/LICENSE
--rw-r--r--   0 akbar     (1000) akbar     (1000)       26 2023-05-06 14:28:03.000000 translategram-0.1.1/MANIFEST.in
--rw-r--r--   0 akbar     (1000) akbar     (1000)     4142 2023-05-23 00:42:39.418198 translategram-0.1.1/PKG-INFO
--rw-r--r--   0 akbar     (1000) akbar     (1000)     3351 2023-05-07 15:28:54.000000 translategram-0.1.1/README.md
-drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-23 00:42:39.417198 translategram-0.1.1/auto_translategram/
--rw-r--r--   0 akbar     (1000) akbar     (1000)      188 2023-05-06 14:22:50.000000 translategram-0.1.1/auto_translategram/__init__.py
-drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-23 00:42:39.417198 translategram-0.1.1/auto_translategram/auto_translategram/
--rw-r--r--   0 akbar     (1000) akbar     (1000)        0 2023-04-29 15:46:48.000000 translategram-0.1.1/auto_translategram/auto_translategram/__init__.py
--rw-r--r--   0 akbar     (1000) akbar     (1000)       69 2023-05-17 17:58:22.000000 translategram-0.1.1/auto_translategram/auto_translategram/service_libs.py
--rw-r--r--   0 akbar     (1000) akbar     (1000)     1183 2023-05-22 23:44:48.000000 translategram-0.1.1/auto_translategram/auto_translategram/translator.py
--rw-r--r--   0 akbar     (1000) akbar     (1000)     1283 2023-05-17 18:00:58.000000 translategram-0.1.1/auto_translategram/auto_translategram/translator_services.py
-drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-23 00:42:39.418198 translategram-0.1.1/auto_translategram/python_telegram_bot_translator/
--rw-r--r--   0 akbar     (1000) akbar     (1000)        0 2023-04-30 15:04:38.000000 translategram-0.1.1/auto_translategram/python_telegram_bot_translator/__init__.py
--rw-r--r--   0 akbar     (1000) akbar     (1000)     2769 2023-05-22 23:56:52.000000 translategram-0.1.1/auto_translategram/python_telegram_bot_translator/adapter.py
--rw-r--r--   0 akbar     (1000) akbar     (1000)       38 2023-05-23 00:42:39.419198 translategram-0.1.1/setup.cfg
--rw-r--r--   0 akbar     (1000) akbar     (1000)     1154 2023-05-23 00:38:41.000000 translategram-0.1.1/setup.py
-drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-23 00:42:39.418198 translategram-0.1.1/translategram.egg-info/
--rw-r--r--   0 akbar     (1000) akbar     (1000)     4142 2023-05-23 00:42:39.000000 translategram-0.1.1/translategram.egg-info/PKG-INFO
--rw-r--r--   0 akbar     (1000) akbar     (1000)      593 2023-05-23 00:42:39.000000 translategram-0.1.1/translategram.egg-info/SOURCES.txt
--rw-r--r--   0 akbar     (1000) akbar     (1000)        1 2023-05-23 00:42:39.000000 translategram-0.1.1/translategram.egg-info/dependency_links.txt
--rw-r--r--   0 akbar     (1000) akbar     (1000)       11 2023-05-23 00:42:39.000000 translategram-0.1.1/translategram.egg-info/requires.txt
--rw-r--r--   0 akbar     (1000) akbar     (1000)       19 2023-05-23 00:42:39.000000 translategram-0.1.1/translategram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:14.294062 translategram-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-04 16:06:04.000000 translategram-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 16:06:04.000000 translategram-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-04 16:06:14.290062 translategram-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-04 16:06:04.000000 translategram-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:14.290062 translategram-0.1.2/auto_translategram/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:14.290062 translategram-0.1.2/auto_translategram/auto_translategram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/auto_translategram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/auto_translategram/service_libs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/auto_translategram/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/auto_translategram/translator_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:14.290062 translategram-0.1.2/auto_translategram/python_telegram_bot_translator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/python_telegram_bot_translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-04 16:06:04.000000 translategram-0.1.2/auto_translategram/python_telegram_bot_translator/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 16:06:14.294062 translategram-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-04 16:06:04.000000 translategram-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:06:14.290062 translategram-0.1.2/translategram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-04 16:06:14.000000 translategram-0.1.2/translategram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-04 16:06:14.000000 translategram-0.1.2/translategram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:06:14.000000 translategram-0.1.2/translategram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 16:06:14.000000 translategram-0.1.2/translategram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-04 16:06:14.000000 translategram-0.1.2/translategram.egg-info/top_level.txt
```

### Comparing `translategram-0.1.1/LICENSE` & `translategram-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `translategram-0.1.1/PKG-INFO` & `translategram-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: translategram
-Version: 0.1.1
-Summary: Python library for translating messages in Telegram
+Version: 0.1.2
+Summary: Python library for translating messages are sent by Bot in Telegram
 Home-page: https://github.com/EkberHasanov/translategram
 Author: Akbar
 Author-email: hasanvakbar@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `translategram-0.1.1/README.md` & `translategram-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `translategram-0.1.1/auto_translategram/auto_translategram/translator.py` & `translategram-0.1.2/auto_translategram/auto_translategram/translator.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         Initializes a new Translator instance using the specified `translator_service`.
 
         :param translator_service: The `BaseTranslatorService` to use for translations.
         """
         ...
 
     @abstractmethod
-    def handler_translator(self, func: Callable[..., None], message: str) -> Callable[..., Coroutine[Any, Any, Any]]:
+    def handler_translator(
+        self,
+        message: str
+    ) -> Callable[[Callable[..., T]], Callable[[Any, Any, str], Coroutine[Any, Any, Any]]]:
         """
         Translate a message based on the users' language
         :param func: The handler function that is used for handling commands by Frameworks.
         :param message: The message to translate.
         """
         ...
```

### Comparing `translategram-0.1.1/auto_translategram/auto_translategram/translator_services.py` & `translategram-0.1.2/auto_translategram/auto_translategram/translator_services.py`

 * *Files identical despite different names*

### Comparing `translategram-0.1.1/auto_translategram/python_telegram_bot_translator/adapter.py` & `translategram-0.1.2/auto_translategram/python_telegram_bot_translator/adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,38 +24,41 @@
 
         :param translator_service: The `TranslatorService` to use for translations.
         """
         self._translator_service = translator_service()
 
     def handler_translator(
             self,
-            func: Callable[[Update, ContextTypes.DEFAULT_TYPE, str], _T],
-            message: str) -> Callable[[Update, ContextTypes.DEFAULT_TYPE, str], Coroutine[Any, Any, Any]]:
+            message: str
+            ) -> Callable[[Callable[[Any, Any, str], _T]], Callable[[Any, Any, str], Coroutine[Any, Any, Any]]]:
         """
         A decorator that wraps a python-telegram-bot `handler` function to provide translation functionality.
 
         The decorated function will be executed after being wrapped with a new function that translates
         the incoming message into the user's preferred language (if it is not already in that language).
         If the user does not have a preferred language set or if it is set to 'en', the message will not be translated.
 
         :param func: The handler function that is used for handling commands by the Python-telegram-bot framework.
         :param message: The message to translate.
         :return: A coroutine that wraps the handler function and provides translation functionality.
         """
+        def decorator(func: Callable[[Update, ContextTypes.DEFAULT_TYPE, str], _T]) \
+                -> Callable[[Any, Any, str], Coroutine[Any, Any, Any]]:
 
-        async def wrapper(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str = message) -> Any:
-            user_lang = update.effective_user.language_code if update.effective_user else 'en'
-            message = message
-            if user_lang != 'en' and user_lang is not None:
-                message = await self._translator_service.translate_str(
-                    text=message,
-                    target_language=user_lang,
-                    source_language='en'
-                    )
-            is_async = inspect.iscoroutinefunction(func)
-            if is_async:
-                result = await func(update, context, message)  # type: ignore[misc]
-            else:
-                result = func(update, context, message)
-            return result
+            async def wrapper(update: Update, context: ContextTypes.DEFAULT_TYPE, message: str = message) -> Any:
+                user_lang = update.effective_user.language_code if update.effective_user else 'en'
+                message = message
+                if user_lang != 'en' and user_lang is not None:
+                    message = await self._translator_service.translate_str(
+                        text=message,
+                        target_language=user_lang,
+                        source_language='en'
+                        )
+                is_async = inspect.iscoroutinefunction(func)
+                if is_async:
+                    result = await func(update, context, message)  # type: ignore[misc]
+                else:
+                    result = func(update, context, message)
+                return result
 
-        return wrapper
+            return wrapper
+        return decorator
```

### Comparing `translategram-0.1.1/setup.py` & `translategram-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='translategram',
-    version='0.1.1',
-    description='Python library for translating messages in Telegram',
+    version='0.1.2',
+    description='Python library for translating messages are sent by Bot in Telegram',
     url='https://github.com/EkberHasanov/translategram',
     author='Akbar',
     author_email='hasanvakbar@gmail.com',
     license='MIT',
     install_requires=[
         'mtranslate',
     ],
```

### Comparing `translategram-0.1.1/translategram.egg-info/PKG-INFO` & `translategram-0.1.2/translategram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: translategram
-Version: 0.1.1
-Summary: Python library for translating messages in Telegram
+Version: 0.1.2
+Summary: Python library for translating messages are sent by Bot in Telegram
 Home-page: https://github.com/EkberHasanov/translategram
 Author: Akbar
 Author-email: hasanvakbar@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `translategram-0.1.1/translategram.egg-info/SOURCES.txt` & `translategram-0.1.2/translategram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

