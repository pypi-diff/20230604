# Comparing `tmp/logmaster-1.2.tar.gz` & `tmp/logmaster-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logmaster-1.2.tar", last modified: Sun May 21 18:07:36 2023, max compression
+gzip compressed data, was "logmaster-1.3.tar", last modified: Sun Jun  4 21:21:45 2023, max compression
```

## Comparing `logmaster-1.2.tar` & `logmaster-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 18:07:36.857575 logmaster-1.2/
--rw-rw-rw-   0        0        0     1083 2023-05-08 22:14:25.000000 logmaster-1.2/LICENSE
--rw-rw-rw-   0        0        0     1337 2023-05-21 18:07:36.865564 logmaster-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1034 2023-05-21 14:11:16.000000 logmaster-1.2/README.md
--rw-rw-rw-   0        0        0      109 2023-05-09 16:02:47.000000 logmaster-1.2/pyproject.toml
--rw-rw-rw-   0        0        0      430 2023-05-21 18:07:36.873599 logmaster-1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 18:07:36.769567 logmaster-1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 18:07:36.825569 logmaster-1.2/src/logmaster/
--rw-rw-rw-   0        0        0      993 2023-05-14 14:45:28.000000 logmaster-1.2/src/logmaster/__init__.py
--rw-rw-rw-   0        0        0       73 2023-05-14 15:04:18.000000 logmaster-1.2/src/logmaster/errors.py
--rw-rw-rw-   0        0        0     1938 2023-05-21 18:05:34.000000 logmaster-1.2/src/logmaster/logger.py
-drwxrwxrwx   0        0        0        0 2023-05-21 18:07:36.857575 logmaster-1.2/src/logmaster.egg-info/
--rw-rw-rw-   0        0        0     1337 2023-05-21 18:07:36.000000 logmaster-1.2/src/logmaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-21 18:07:36.000000 logmaster-1.2/src/logmaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 18:07:36.000000 logmaster-1.2/src/logmaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-21 18:07:36.000000 logmaster-1.2/src/logmaster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 21:21:45.542171 logmaster-1.3/
+-rw-rw-rw-   0        0        0     1083 2023-05-08 22:14:25.000000 logmaster-1.3/LICENSE
+-rw-rw-rw-   0        0        0     1337 2023-06-04 21:21:45.543171 logmaster-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1034 2023-05-21 14:11:16.000000 logmaster-1.3/README.md
+-rw-rw-rw-   0        0        0      109 2023-05-09 16:02:47.000000 logmaster-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      430 2023-06-04 21:21:45.546172 logmaster-1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 21:21:45.454173 logmaster-1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 21:21:45.498174 logmaster-1.3/src/logmaster/
+-rw-rw-rw-   0        0        0      993 2023-05-14 14:45:28.000000 logmaster-1.3/src/logmaster/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-05-14 15:04:18.000000 logmaster-1.3/src/logmaster/errors.py
+-rw-rw-rw-   0        0        0     2102 2023-06-04 21:20:50.000000 logmaster-1.3/src/logmaster/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:21:45.540171 logmaster-1.3/src/logmaster.egg-info/
+-rw-rw-rw-   0        0        0     1337 2023-06-04 21:21:45.000000 logmaster-1.3/src/logmaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-04 21:21:45.000000 logmaster-1.3/src/logmaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 21:21:45.000000 logmaster-1.3/src/logmaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 21:21:45.000000 logmaster-1.3/src/logmaster.egg-info/top_level.txt
```

### Comparing `logmaster-1.2/LICENSE` & `logmaster-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logmaster-1.2/PKG-INFO` & `logmaster-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logmaster
-Version: 1.2
+Version: 1.3
 Summary: A simple logging library for Python
 Home-page: https://github.com/W1L7dev/logmaster
 Author: W1L7dev
 Author-email: w1l7dev@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `logmaster-1.2/README.md` & `logmaster-1.3/README.md`

 * *Files identical despite different names*

### Comparing `logmaster-1.2/src/logmaster/__init__.py` & `logmaster-1.3/src/logmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `logmaster-1.2/src/logmaster/logger.py` & `logmaster-1.3/src/logmaster/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
+import inspect
+import os
 from typing import Optional
 
-import os
 from .errors import *
 
 
 class Colors:
     def __init__(self):
         self.colors_levels = {
             "success": "\033[92m",
@@ -48,20 +49,24 @@
             raise InvalidLevel(f"Invalid level: {level}")
 
         self.color = self.colors_levels[level]
 
         if show_datetime:
             output += f"{self.color}[{datetime.datetime.now()}] "
         if show_filename:
-            output += f"{self.color}[{os.path.basename(__file__)}] "
+            frame = inspect.currentframe().f_back
+            file = inspect.getframeinfo(frame).filename
+            file = os.path.basename(file)
+            output += f"{self.color}[{file}] "
         if show_type:
             output += f"{self.color}[{level.upper()}] "
 
         output += f"{self.color}{self.bold}{message}{self.reset}"
         if additional_info:
             output += f"{self.color}[{additional_info}]{self.reset}"
         if self.filename:
             with open(self.filename, "a") as f:
                 f.write(output + "\n")
         print(output)
 
-Logger().log(level="info", message="This is an info message.", additional_info="additional info")
+    def __repr__(self):
+        return f"<Logger" + (f" filename={self.filename}" if self.filename else "") + ">"
```

### Comparing `logmaster-1.2/src/logmaster.egg-info/PKG-INFO` & `logmaster-1.3/src/logmaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logmaster
-Version: 1.2
+Version: 1.3
 Summary: A simple logging library for Python
 Home-page: https://github.com/W1L7dev/logmaster
 Author: W1L7dev
 Author-email: w1l7dev@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

