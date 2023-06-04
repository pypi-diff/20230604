# Comparing `tmp/rfswarm-manager-1.1.2.tar.gz` & `tmp/rfswarm-manager-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-manager-1.1.2.tar", last modified: Fri May 19 05:26:25 2023, max compression
+gzip compressed data, was "rfswarm-manager-1.1.3.tar", last modified: Sun Jun  4 05:25:58 2023, max compression
```

## Comparing `rfswarm-manager-1.1.2.tar` & `rfswarm-manager-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:25.374287 rfswarm-manager-1.1.2/
--rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-manager-1.1.2/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)     3108 2023-05-19 05:26:25.374287 rfswarm-manager-1.1.2/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-05-19 05:23:33.000000 rfswarm-manager-1.1.2/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:25.374287 rfswarm-manager-1.1.2/rfswarm_manager/
--rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-05-19 05:26:24.000000 rfswarm-manager-1.1.2/rfswarm_manager/__init__.py
--rw-r--r--   0 dave      (1000) dave      (1000)   314437 2023-05-19 05:26:24.000000 rfswarm-manager-1.1.2/rfswarm_manager/rfswarm.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:25.374287 rfswarm-manager-1.1.2/rfswarm_manager.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3108 2023-05-19 05:26:25.000000 rfswarm-manager-1.1.2/rfswarm_manager.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      325 2023-05-19 05:26:25.000000 rfswarm-manager-1.1.2/rfswarm_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-19 05:26:25.000000 rfswarm-manager-1.1.2/rfswarm_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      111 2023-05-19 05:26:25.000000 rfswarm-manager-1.1.2/rfswarm_manager.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       78 2023-05-19 05:26:25.000000 rfswarm-manager-1.1.2/rfswarm_manager.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       16 2023-05-19 05:26:25.000000 rfswarm-manager-1.1.2/rfswarm_manager.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     1419 2023-05-19 05:26:24.000000 rfswarm-manager-1.1.2/setup-manager.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-19 05:26:25.374287 rfswarm-manager-1.1.2/setup.cfg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:58.609713 rfswarm-manager-1.1.3/
+-rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-manager-1.1.3/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3156 2023-06-04 05:25:58.609713 rfswarm-manager-1.1.3/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-06-04 04:58:34.000000 rfswarm-manager-1.1.3/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:58.605713 rfswarm-manager-1.1.3/rfswarm_manager/
+-rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-06-04 05:25:57.000000 rfswarm-manager-1.1.3/rfswarm_manager/__init__.py
+-rw-r--r--   0 dave      (1000) dave      (1000)   314437 2023-06-04 05:25:57.000000 rfswarm-manager-1.1.3/rfswarm_manager/rfswarm.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:58.609713 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3156 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      325 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      111 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       78 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       16 2023-06-04 05:25:58.000000 rfswarm-manager-1.1.3/rfswarm_manager.egg-info/top_level.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)     1419 2023-06-04 05:25:57.000000 rfswarm-manager-1.1.3/setup-manager.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-04 05:25:58.609713 rfswarm-manager-1.1.3/setup.cfg
```

### Comparing `rfswarm-manager-1.1.2/LICENSE` & `rfswarm-manager-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-manager-1.1.2/PKG-INFO` & `rfswarm-manager-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-manager
-Version: 1.1.2
+Version: 1.1.3
 Summary: rfswarm manager
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
@@ -41,15 +41,15 @@
 ### Community Support
 
 - [rfswarm Documentation](https://github.com/damies13/rfswarm/blob/master/Doc/README.md)
 - [Discord](https://discord.gg/jJfCMrqCsT)
 - [Reporting Issues / Known Issues](https://github.com/damies13/rfswarm/issues)
 
 <kbd align="centre">
-<img align="centre" height="350" src="Doc/Images/Manager&Agent_Example.png">
+<img align="centre" height="350" src="https://github.com/damies13/rfswarm/blob/master/Doc/Images/Manager&Agent_Example.png">
 </kbd><br>
 An example of how your rfswarm setup might look.
 
 ### Commercial Support
 - The easiest way to get commercial support is to sponsor this project on [GitHub](https://github.com/sponsors/damies13?frequency=recurring&sponsor=damies13)
```

### Comparing `rfswarm-manager-1.1.2/README.md` & `rfswarm-manager-1.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 |Version|Manager|Agent|Reporter|
 |---|---|---|---|
 |[![Latest PyPI version](https://img.shields.io/pypi/v/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Manager PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-manager.svg)](https://pypi.python.org/pypi/rfswarm-manager/) | [![Number of Agent PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-agent.svg)](https://pypi.python.org/pypi/rfswarm-agent/) | [![Number of Reporter PyPI downloads](https://img.shields.io/pypi/dm/rfswarm-reporter.svg)](https://pypi.python.org/pypi/rfswarm-reporter/) |
 
 | Master | Branch |
 | -- | -- |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.2&label=Linter) |
-| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.2&label=Regression%20Tests) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=master&label=Linter)](https://github.com/damies13/rfswarm/actions/workflows/superlinter.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/superlinter.yml?branch=v1.1.3&label=Linter) |
+| [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=master&label=Regression%20Tests)](https://github.com/damies13/rfswarm/actions/workflows/Regression_Tests.yml) | ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/damies13/rfswarm/Regression_Tests.yml?branch=v1.1.3&label=Regression%20Tests) |
 
 <img align="right" src="Doc/Images/Icon_Information.png">
 
 ## About
 rfswarm is a testing tool that allows you use [Robot Framework](https://robotframework.org/) test cases for performance or load testing.
 
 > _Swarm being the collective noun for Robots, just as Flock is for Birds and Herd for Sheep, so it made sense to use swarm for a performance testing tool using Robot Framework, hence rfswarm_
```

### Comparing `rfswarm-manager-1.1.2/rfswarm_manager/rfswarm.py` & `rfswarm-manager-1.1.3/rfswarm_manager/rfswarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 # 		Manager
-#    Version 1.1.2
+#    Version 1.1.3
 #
 
 # 	Helpful links
 #
 #
 
 import argparse
@@ -443,15 +443,15 @@
 	# 	log_request is here to stop BaseHTTPRequestHandler logging to the console
 	# 		https://stackoverflow.com/questions/10651052/how-to-quiet-simplehttpserver/10651257#10651257
 	def log_request(self, code='-', size='-'):
 		pass
 
 
 class RFSwarmBase:
-	version = "1.1.2"
+	version = "1.1.3"
 	debuglvl = 0
 
 	config = None
 	manager_ini = None
 
 	save_ini = True
```

### Comparing `rfswarm-manager-1.1.2/rfswarm_manager.egg-info/PKG-INFO` & `rfswarm-manager-1.1.3/rfswarm_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-manager
-Version: 1.1.2
+Version: 1.1.3
 Summary: rfswarm manager
 Home-page: https://github.com/damies13/rfswarm
 Author: damies13
 Author-email: damies13+rfswarm@gmail.com
 License: UNKNOWN
 Project-URL: Getting Help, https://github.com/damies13/rfswarm#getting-help
 Project-URL: Say Thanks!, https://github.com/damies13/rfswarm#donations
@@ -41,15 +41,15 @@
 ### Community Support
 
 - [rfswarm Documentation](https://github.com/damies13/rfswarm/blob/master/Doc/README.md)
 - [Discord](https://discord.gg/jJfCMrqCsT)
 - [Reporting Issues / Known Issues](https://github.com/damies13/rfswarm/issues)
 
 <kbd align="centre">
-<img align="centre" height="350" src="Doc/Images/Manager&Agent_Example.png">
+<img align="centre" height="350" src="https://github.com/damies13/rfswarm/blob/master/Doc/Images/Manager&Agent_Example.png">
 </kbd><br>
 An example of how your rfswarm setup might look.
 
 ### Commercial Support
 - The easiest way to get commercial support is to sponsor this project on [GitHub](https://github.com/sponsors/damies13?frequency=recurring&sponsor=damies13)
```

### Comparing `rfswarm-manager-1.1.2/setup-manager.py` & `rfswarm-manager-1.1.3/setup-manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-manager",
-	version="1.1.2",
+	version="1.1.3",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm manager",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_report*", "*fswarm_agen*", "build/*"]),
```

