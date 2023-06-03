# Comparing `tmp/rtmilk-0.2.2.tar.gz` & `tmp/rtmilk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtmilk-0.2.2.tar", max compression
+gzip compressed data, was "rtmilk-0.2.3.tar", max compression
```

## Comparing `rtmilk-0.2.2.tar` & `rtmilk-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2021-07-04 08:58:00.981162 rtmilk-0.2.2/LICENSE
--rw-r--r--   0        0        0     1866 2023-04-06 03:33:10.227794 rtmilk-0.2.2/README.md
--rw-r--r--   0        0        0     2139 2023-04-06 06:59:19.653429 rtmilk-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       90 2023-04-06 03:33:10.229614 rtmilk-0.2.2/src/rtmilk/__init__.py
--rw-r--r--   0        0        0    10556 2023-04-06 03:33:10.230033 rtmilk-0.2.2/src/rtmilk/api_async.py
--rw-r--r--   0        0        0      528 2023-03-28 08:04:55.802718 rtmilk-0.2.2/src/rtmilk/api_base.py
--rw-r--r--   0        0        0    10514 2023-04-06 03:33:10.230595 rtmilk-0.2.2/src/rtmilk/api_sync.py
--rw-r--r--   0        0        0      634 2023-03-28 08:04:55.803821 rtmilk-0.2.2/src/rtmilk/authorization.py
--rw-r--r--   0        0        0     4660 2023-03-28 08:04:55.804395 rtmilk-0.2.2/src/rtmilk/client.py
--rw-r--r--   0        0        0     6497 2023-03-28 08:00:56.865528 rtmilk-0.2.2/src/rtmilk/filter.py
--rw-r--r--   0        0        0     5089 2023-04-06 06:59:19.673186 rtmilk-0.2.2/src/rtmilk/models.py
--rw-r--r--   0        0        0     4809 2023-04-06 06:57:41.737118 rtmilk-0.2.2/src/rtmilk/properties.py
--rw-r--r--   0        0        0        0 2022-01-03 07:25:19.434211 rtmilk-0.2.2/src/rtmilk/py.typed
--rw-r--r--   0        0        0    14176 2023-04-06 03:33:10.232284 rtmilk-0.2.2/src/rtmilk/sansio.py
--rw-r--r--   0        0        0      951 2022-01-03 07:25:19.435129 rtmilk-0.2.2/src/rtmilk/secrets.py
--rw-r--r--   0        0        0      649 2022-11-06 02:22:50.944741 rtmilk-0.2.2/src/rtmilk/utils.py
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 rtmilk-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-07-04 08:58:00.981162 rtmilk-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1866 2023-05-18 06:15:11.906916 rtmilk-0.2.3/README.md
+-rw-r--r--   0        0        0     2137 2023-06-03 22:29:03.902264 rtmilk-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       90 2023-04-06 03:33:10.229614 rtmilk-0.2.3/src/rtmilk/__init__.py
+-rw-r--r--   0        0        0    10556 2023-05-18 06:15:11.907280 rtmilk-0.2.3/src/rtmilk/api_async.py
+-rw-r--r--   0        0        0      528 2023-05-18 06:15:11.907573 rtmilk-0.2.3/src/rtmilk/api_base.py
+-rw-r--r--   0        0        0    10514 2023-05-18 06:15:11.907782 rtmilk-0.2.3/src/rtmilk/api_sync.py
+-rw-r--r--   0        0        0      634 2023-05-18 06:15:11.908067 rtmilk-0.2.3/src/rtmilk/authorization.py
+-rw-r--r--   0        0        0     4670 2023-06-03 22:07:57.318329 rtmilk-0.2.3/src/rtmilk/client.py
+-rw-r--r--   0        0        0     6497 2023-03-28 08:00:56.865528 rtmilk-0.2.3/src/rtmilk/filter.py
+-rw-r--r--   0        0        0     5089 2023-05-18 06:15:11.908658 rtmilk-0.2.3/src/rtmilk/models.py
+-rw-r--r--   0        0        0     4809 2023-05-18 06:15:11.908901 rtmilk-0.2.3/src/rtmilk/properties.py
+-rw-r--r--   0        0        0        0 2022-01-03 07:25:19.434211 rtmilk-0.2.3/src/rtmilk/py.typed
+-rw-r--r--   0        0        0    14176 2023-05-18 06:15:11.909163 rtmilk-0.2.3/src/rtmilk/sansio.py
+-rw-r--r--   0        0        0      951 2023-05-18 06:15:11.909400 rtmilk-0.2.3/src/rtmilk/secrets.py
+-rw-r--r--   0        0        0      649 2023-05-18 06:15:11.909631 rtmilk-0.2.3/src/rtmilk/utils.py
+-rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 rtmilk-0.2.3/PKG-INFO
```

### Comparing `rtmilk-0.2.2/LICENSE` & `rtmilk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/README.md` & `rtmilk-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/pyproject.toml` & `rtmilk-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rtmilk"
-version = "0.2.2"
+version = "0.2.3"
 description = "RTM API wrapper"
 authors = ["Rehan Khwaja <rehan@khwaja.name>"]
 license = "MIT"
 homepage = "https://github.com/rkhwaja/rtmilk"
 keywords = ["RememberTheMilk"]
 readme = "README.md"
 classifiers = [
@@ -81,9 +81,9 @@
 	"protected-access" # temporary until I figure out the privacy
 ]
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 
 [build-system]
-requires = ["poetry_core>=1.0.0"]
+requires = ["poetry_core>=1.1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rtmilk-0.2.2/src/rtmilk/api_async.py` & `rtmilk-0.2.3/src/rtmilk/api_async.py`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/src/rtmilk/api_base.py` & `rtmilk-0.2.3/src/rtmilk/api_base.py`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/src/rtmilk/api_sync.py` & `rtmilk-0.2.3/src/rtmilk/api_sync.py`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/src/rtmilk/authorization.py` & `rtmilk-0.2.3/src/rtmilk/authorization.py`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/src/rtmilk/client.py` & `rtmilk-0.2.3/src/rtmilk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 def _CreateFromTaskSeries(client, listId, taskSeries):
 	_log.info(f'{taskSeries=}')
 	task0 = taskSeries.task[0]
 	result = Task(client, listId, taskSeries.id, task0.id)
 
 	result.name._LoadValue(taskSeries.name)
-	result.tags._LoadValue(taskSeries.tags.tag if hasattr(taskSeries.tags, 'tag') else taskSeries.tags)
+	result.tags._LoadValue(set(taskSeries.tags.tag) if hasattr(taskSeries.tags, 'tag') else set(taskSeries.tags))
 	result.startDate._LoadValue(task0.start.date() if task0.start is not None else None) # None means no change
 	result.dueDate._LoadValue(task0.due.date() if task0.due is not None else None) # None means no change
 	result.complete._LoadValue(task0.completed is not None)
 	result.notes._LoadValue(taskSeries.notes)
 	result.createTime = taskSeries.created
 	result.modifiedTime = taskSeries.modified
```

### Comparing `rtmilk-0.2.2/src/rtmilk/filter.py` & `rtmilk-0.2.3/src/rtmilk/filter.py`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/src/rtmilk/models.py` & `rtmilk-0.2.3/src/rtmilk/models.py`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/src/rtmilk/properties.py` & `rtmilk-0.2.3/src/rtmilk/properties.py`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/src/rtmilk/sansio.py` & `rtmilk-0.2.3/src/rtmilk/sansio.py`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/src/rtmilk/secrets.py` & `rtmilk-0.2.3/src/rtmilk/secrets.py`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/src/rtmilk/utils.py` & `rtmilk-0.2.3/src/rtmilk/utils.py`

 * *Files identical despite different names*

### Comparing `rtmilk-0.2.2/PKG-INFO` & `rtmilk-0.2.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: rtmilk
-Version: 0.2.2
+Version: 0.2.3
 Summary: RTM API wrapper
 Home-page: https://github.com/rkhwaja/rtmilk
 License: MIT
 Keywords: RememberTheMilk
 Author: Rehan Khwaja
 Author-email: rehan@khwaja.name
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.1)
 Requires-Dist: pydantic (>=1.8.1)
 Requires-Dist: requests (>=2.23.0)
 Requires-Dist: urllib3 (>=1.26) ; python_version >= "3.10" and python_version < "4"
 Description-Content-Type: text/markdown
 
 [![codecov](https://codecov.io/gh/rkhwaja/rtmilk/branch/master/graph/badge.svg?token=RaMYgorajr)](https://codecov.io/gh/rkhwaja/rtmilk) [![PyPI version](https://badge.fury.io/py/rtmilk.svg)](https://badge.fury.io/py/rtmilk)
```

