# Comparing `tmp/granny-pliers-0.0.4.tar.gz` & `tmp/granny-pliers-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granny-pliers-0.0.4.tar", last modified: Sat Jun  3 23:40:37 2023, max compression
+gzip compressed data, was "granny-pliers-0.0.5.tar", last modified: Sun Jun  4 16:30:05 2023, max compression
```

## Comparing `granny-pliers-0.0.4.tar` & `granny-pliers-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 23:40:37.766730 granny-pliers-0.0.4/
--rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.4/LICENSE
--rw-r--r--   0 pd         (501) staff       (20)    13859 2023-06-03 23:40:37.766283 granny-pliers-0.0.4/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)       15 2023-06-03 15:16:58.000000 granny-pliers-0.0.4/README.md
--rw-r--r--   0 pd         (501) staff       (20)     1666 2023-06-03 23:39:43.000000 granny-pliers-0.0.4/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)       38 2023-06-03 23:40:37.766868 granny-pliers-0.0.4/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 23:40:37.755995 granny-pliers-0.0.4/src/
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 23:40:37.758797 granny-pliers-0.0.4/src/granny_pliers/
--rw-r--r--   0 pd         (501) staff       (20)      987 2023-06-03 23:39:49.000000 granny-pliers-0.0.4/src/granny_pliers/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 23:40:37.763337 granny-pliers-0.0.4/src/granny_pliers/config/
--rw-r--r--   0 pd         (501) staff       (20)      865 2023-06-03 18:43:25.000000 granny-pliers-0.0.4/src/granny_pliers/config/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2448 2023-06-03 23:39:30.000000 granny-pliers-0.0.4/src/granny_pliers/config/abstract_config.py
--rw-r--r--   0 pd         (501) staff       (20)     1614 2023-06-03 23:39:30.000000 granny-pliers-0.0.4/src/granny_pliers/config/autowired_config.py
--rw-r--r--   0 pd         (501) staff       (20)     5994 2023-06-03 23:39:30.000000 granny-pliers-0.0.4/src/granny_pliers/config/logger_config.py
--rw-r--r--   0 pd         (501) staff       (20)      860 2023-06-03 18:43:25.000000 granny-pliers-0.0.4/src/granny_pliers/config/project_environment.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 23:40:37.764651 granny-pliers-0.0.4/src/granny_pliers/logger/
--rw-r--r--   0 pd         (501) staff       (20)      859 2023-06-03 18:43:25.000000 granny-pliers-0.0.4/src/granny_pliers/logger/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.4/src/granny_pliers/logger/abstract_logger.py
--rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.4/src/granny_pliers/logger/log_processors.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 23:40:37.765518 granny-pliers-0.0.4/src/granny_pliers/worker/
--rw-r--r--   0 pd         (501) staff       (20)      688 2023-06-03 18:43:25.000000 granny-pliers-0.0.4/src/granny_pliers/worker/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5091 2023-06-03 18:43:25.000000 granny-pliers-0.0.4/src/granny_pliers/worker/abstract_worker.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-03 23:40:37.761154 granny-pliers-0.0.4/src/granny_pliers.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)    13859 2023-06-03 23:40:37.000000 granny-pliers-0.0.4/src/granny_pliers.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      687 2023-06-03 23:40:37.000000 granny-pliers-0.0.4/src/granny_pliers.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-03 23:40:37.000000 granny-pliers-0.0.4/src/granny_pliers.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      235 2023-06-03 23:40:37.000000 granny-pliers-0.0.4/src/granny_pliers.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       14 2023-06-03 23:40:37.000000 granny-pliers-0.0.4/src/granny_pliers.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-04 16:30:05.435545 granny-pliers-0.0.5/
+-rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.5/LICENSE
+-rw-r--r--   0 pd         (501) staff       (20)    13859 2023-06-04 16:30:05.435018 granny-pliers-0.0.5/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)       15 2023-06-03 15:16:58.000000 granny-pliers-0.0.5/README.md
+-rw-r--r--   0 pd         (501) staff       (20)     1915 2023-06-04 16:29:44.000000 granny-pliers-0.0.5/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)       38 2023-06-04 16:30:05.435698 granny-pliers-0.0.5/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-04 16:30:05.420819 granny-pliers-0.0.5/src/
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-04 16:30:05.424396 granny-pliers-0.0.5/src/granny_pliers/
+-rw-r--r--   0 pd         (501) staff       (20)      987 2023-06-04 16:29:44.000000 granny-pliers-0.0.5/src/granny_pliers/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-04 16:30:05.429174 granny-pliers-0.0.5/src/granny_pliers/config/
+-rw-r--r--   0 pd         (501) staff       (20)      985 2023-06-04 16:29:44.000000 granny-pliers-0.0.5/src/granny_pliers/config/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2438 2023-06-04 16:08:02.000000 granny-pliers-0.0.5/src/granny_pliers/config/abstract_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     1614 2023-06-03 23:39:30.000000 granny-pliers-0.0.5/src/granny_pliers/config/autowired_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     5994 2023-06-03 23:39:30.000000 granny-pliers-0.0.5/src/granny_pliers/config/logger_config.py
+-rw-r--r--   0 pd         (501) staff       (20)      860 2023-06-03 18:43:25.000000 granny-pliers-0.0.5/src/granny_pliers/config/project_environment.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-04 16:30:05.430519 granny-pliers-0.0.5/src/granny_pliers/logger/
+-rw-r--r--   0 pd         (501) staff       (20)      884 2023-06-04 16:29:44.000000 granny-pliers-0.0.5/src/granny_pliers/logger/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.5/src/granny_pliers/logger/abstract_logger.py
+-rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.5/src/granny_pliers/logger/log_processors.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-04 16:30:05.432073 granny-pliers-0.0.5/src/granny_pliers/orm/
+-rw-r--r--   0 pd         (501) staff       (20)      785 2023-06-04 16:29:44.000000 granny-pliers-0.0.5/src/granny_pliers/orm/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1328 2023-06-04 16:29:44.000000 granny-pliers-0.0.5/src/granny_pliers/orm/abstract_model.py
+-rw-r--r--   0 pd         (501) staff       (20)     7530 2023-06-04 16:29:44.000000 granny-pliers-0.0.5/src/granny_pliers/orm/abstract_repository.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-04 16:30:05.433428 granny-pliers-0.0.5/src/granny_pliers/testing/
+-rw-r--r--   0 pd         (501) staff       (20)      806 2023-06-04 16:29:44.000000 granny-pliers-0.0.5/src/granny_pliers/testing/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1982 2023-06-04 16:08:02.000000 granny-pliers-0.0.5/src/granny_pliers/testing/abstract_test_case.py
+-rw-r--r--   0 pd         (501) staff       (20)      914 2023-06-04 16:08:02.000000 granny-pliers-0.0.5/src/granny_pliers/testing/async_abstract_test_case.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-04 16:30:05.434355 granny-pliers-0.0.5/src/granny_pliers/worker/
+-rw-r--r--   0 pd         (501) staff       (20)      713 2023-06-04 16:29:44.000000 granny-pliers-0.0.5/src/granny_pliers/worker/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5086 2023-06-04 16:29:44.000000 granny-pliers-0.0.5/src/granny_pliers/worker/abstract_worker.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-04 16:30:05.426801 granny-pliers-0.0.5/src/granny_pliers.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)    13859 2023-06-04 16:30:05.000000 granny-pliers-0.0.5/src/granny_pliers.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      946 2023-06-04 16:30:05.000000 granny-pliers-0.0.5/src/granny_pliers.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-04 16:30:05.000000 granny-pliers-0.0.5/src/granny_pliers.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      235 2023-06-04 16:30:05.000000 granny-pliers-0.0.5/src/granny_pliers.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       14 2023-06-04 16:30:05.000000 granny-pliers-0.0.5/src/granny_pliers.egg-info/top_level.txt
```

### Comparing `granny-pliers-0.0.4/LICENSE` & `granny-pliers-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.4/PKG-INFO` & `granny-pliers-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.4
+Version: 0.0.5
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `granny-pliers-0.0.4/pyproject.toml` & `granny-pliers-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "granny-pliers"
-version = "0.0.4"
+version = "0.0.5"
 
 authors = [
     { name = "Dmytro Stepanenko", email = "dmitrijstepanenko@gmail.com" },
 ]
 
 license = { file = "LICENSE" }
 
@@ -68,8 +68,23 @@
 exclude = '''
 /(
     \.git
   | build
   | dist
   | tool-belt
 )/
-'''
+'''
+
+[tool.pylint.format]
+max-line-length = 120
+
+[tool.pylint.DESIGN]
+max-args = 6
+max-attributes = 7
+max-bool-expr = 5
+max-branches = 12
+max-locals = 15
+max-parents = 7
+max-public-methods = 20
+max-returns = 6
+max-statements = 50
+min-public-methods = 1
```

### Comparing `granny-pliers-0.0.4/src/granny_pliers/__init__.py` & `granny-pliers-0.0.5/src/granny_pliers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Granny Pliers is a Python library that contains a collection of useful
 and helpful tools, designed to simplify developers' lives."""
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __author__ = "Dmytro Stepanenko"
 __copyright__ = "Copyright 2022, Dmytro Stepanenko, Granny Pliers"
 __credits__ = ["Dmytro Stepanenko"]
 __license__ = "Apache License Version 2.0"
 __email__ = "dmitrijstepanenko@gmail.com"
```

### Comparing `granny-pliers-0.0.4/src/granny_pliers/config/__init__.py` & `granny-pliers-0.0.5/src/granny_pliers/config/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,8 +15,13 @@
 """Configs"""
 
 from .abstract_config import *
 from .autowired_config import *
 from .logger_config import *
 from .project_environment import *
 
-__all__ = abstract_config.__all__ + autowired_config.__all__ + logger_config.__all__ + project_environment.__all__
+__all__ = (
+    abstract_config.__all__  # pylint: disable=E0602
+    + autowired_config.__all__  # pylint: disable=E0602
+    + logger_config.__all__  # pylint: disable=E0602
+    + project_environment.__all__  # pylint: disable=E0602
+)
```

### Comparing `granny-pliers-0.0.4/src/granny_pliers/config/abstract_config.py` & `granny-pliers-0.0.5/src/granny_pliers/config/abstract_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,22 +52,22 @@
 
     @classmethod
     def load(cls, config_file: pathlib.Path) -> "AbstractConfig":
         """Load config"""
         log = structlog.get_logger(cls.__name__)
         log.info("Loading config from: %s", config_file)
         if not config_file.exists():
-            msg = f"Can not load config from {config_file.__str__()}, file not found"
+            msg = f"Can not load config from {str(config_file)}, file not found"
             log.error(msg)
             raise ConfigError(msg)
 
         try:
             with config_file.open(mode="rt", encoding="UTF-8") as file:
                 config_dict = yaml.full_load(file)
 
             config = cls(**config_dict[cls.__name__])
             log.info("Configuration loaded [OK]")
             return config
         except Exception as error:
-            msg = f"Can not load config from {config_file.__str__()}"
+            msg = f"Can not load config from {str(config_file)}"
             log.error(msg, error=error)
             raise ConfigError(msg) from error
```

### Comparing `granny-pliers-0.0.4/src/granny_pliers/config/autowired_config.py` & `granny-pliers-0.0.5/src/granny_pliers/config/autowired_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.4/src/granny_pliers/config/logger_config.py` & `granny-pliers-0.0.5/src/granny_pliers/config/logger_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.4/src/granny_pliers/config/project_environment.py` & `granny-pliers-0.0.5/src/granny_pliers/config/project_environment.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.4/src/granny_pliers/logger/__init__.py` & `granny-pliers-0.0.5/src/granny_pliers/logger/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 """Logger - based on the structlog in addition colorized, includes extra
 meta info and can be printed in PLAIN or JSON formats"""
 
 from .abstract_logger import *
 from .log_processors import *
 
-__all__ = abstract_logger.__all__ + log_processors.__all__
+__all__ = abstract_logger.__all__ + log_processors.__all__  # pylint: disable=E0602
```

### Comparing `granny-pliers-0.0.4/src/granny_pliers/logger/abstract_logger.py` & `granny-pliers-0.0.5/src/granny_pliers/logger/abstract_logger.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.4/src/granny_pliers/logger/log_processors.py` & `granny-pliers-0.0.5/src/granny_pliers/logger/log_processors.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.4/src/granny_pliers/worker/__init__.py` & `granny-pliers-0.0.5/src/granny_pliers/worker/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Workers"""
 
 from .abstract_worker import *
 
-__all__ = abstract_worker.__all__
+__all__ = abstract_worker.__all__  # pylint: disable=E0602
```

### Comparing `granny-pliers-0.0.4/src/granny_pliers/worker/abstract_worker.py` & `granny-pliers-0.0.5/src/granny_pliers/worker/abstract_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,22 +75,21 @@
             self.loop.close()
 
     def shutdown(self):
         """Graceful process shutdown"""
         name = multiprocessing.current_process().name
         self.log.info("Shutting down %s ...", name)
         tasks = [task for task in asyncio.all_tasks(self.loop) if task is not asyncio.current_task(self.loop)]
-
         for task in tasks:
             task.cancel()
 
         self.loop.run_until_complete(asyncio.gather(*tasks, return_exceptions=True))
         self.log.info("Process %s is shutdown", name)
 
-    def windows_graceful_shutdown(self, *args):
+    def windows_graceful_shutdown(self, _):
         """Graceful shutdown for Windows"""
         self.loop.stop()
 
 
 class AbstractWorkerProcess(AbstractWorker, multiprocessing.Process, ABC):
     """AbstractWorkerProcess"""
```

### Comparing `granny-pliers-0.0.4/src/granny_pliers.egg-info/PKG-INFO` & `granny-pliers-0.0.5/src/granny_pliers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.4
+Version: 0.0.5
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `granny-pliers-0.0.4/src/granny_pliers.egg-info/SOURCES.txt` & `granny-pliers-0.0.5/src/granny_pliers.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,9 +11,15 @@
 src/granny_pliers/config/abstract_config.py
 src/granny_pliers/config/autowired_config.py
 src/granny_pliers/config/logger_config.py
 src/granny_pliers/config/project_environment.py
 src/granny_pliers/logger/__init__.py
 src/granny_pliers/logger/abstract_logger.py
 src/granny_pliers/logger/log_processors.py
+src/granny_pliers/orm/__init__.py
+src/granny_pliers/orm/abstract_model.py
+src/granny_pliers/orm/abstract_repository.py
+src/granny_pliers/testing/__init__.py
+src/granny_pliers/testing/abstract_test_case.py
+src/granny_pliers/testing/async_abstract_test_case.py
 src/granny_pliers/worker/__init__.py
 src/granny_pliers/worker/abstract_worker.py
```

