# Comparing `tmp/rfswarm-agent-1.1.2.tar.gz` & `tmp/rfswarm-agent-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfswarm-agent-1.1.2.tar", last modified: Fri May 19 05:26:26 2023, max compression
+gzip compressed data, was "rfswarm-agent-1.1.3.tar", last modified: Sun Jun  4 05:25:59 2023, max compression
```

## Comparing `rfswarm-agent-1.1.2.tar` & `rfswarm-agent-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:26.010291 rfswarm-agent-1.1.2/
--rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-agent-1.1.2/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)     3104 2023-05-19 05:26:26.010291 rfswarm-agent-1.1.2/PKG-INFO
--rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-05-19 05:23:33.000000 rfswarm-agent-1.1.2/README.md
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:26.010291 rfswarm-agent-1.1.2/rfswarm_agent/
--rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-05-19 05:26:24.000000 rfswarm-agent-1.1.2/rfswarm_agent/__init__.py
--rw-r--r--   0 dave      (1000) dave      (1000)    49769 2023-05-19 05:26:24.000000 rfswarm-agent-1.1.2/rfswarm_agent/rfswarm_agent.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-19 05:26:26.010291 rfswarm-agent-1.1.2/rfswarm_agent.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     3104 2023-05-19 05:26:25.000000 rfswarm-agent-1.1.2/rfswarm_agent.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-19 05:26:25.000000 rfswarm-agent-1.1.2/rfswarm_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-19 05:26:25.000000 rfswarm-agent-1.1.2/rfswarm_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       71 2023-05-19 05:26:25.000000 rfswarm-agent-1.1.2/rfswarm_agent.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       44 2023-05-19 05:26:25.000000 rfswarm-agent-1.1.2/rfswarm_agent.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       14 2023-05-19 05:26:25.000000 rfswarm-agent-1.1.2/rfswarm_agent.egg-info/top_level.txt
--rw-r--r--   0 dave      (1000) dave      (1000)     1138 2023-05-19 05:26:24.000000 rfswarm-agent-1.1.2/setup-agent.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-19 05:26:26.010291 rfswarm-agent-1.1.2/setup.cfg
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.301699 rfswarm-agent-1.1.3/
+-rw-r--r--   0 dave      (1000) dave      (1000)    35149 2023-02-10 08:46:44.000000 rfswarm-agent-1.1.3/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3152 2023-06-04 05:25:59.301699 rfswarm-agent-1.1.3/PKG-INFO
+-rw-r--r--   0 dave      (1000) dave      (1000)     5809 2023-06-04 04:58:34.000000 rfswarm-agent-1.1.3/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.301699 rfswarm-agent-1.1.3/rfswarm_agent/
+-rw-r--r--   0 dave      (1000) dave      (1000)       53 2023-06-04 05:25:57.000000 rfswarm-agent-1.1.3/rfswarm_agent/__init__.py
+-rw-r--r--   0 dave      (1000) dave      (1000)    49769 2023-06-04 05:25:57.000000 rfswarm-agent-1.1.3/rfswarm_agent/rfswarm_agent.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-04 05:25:59.301699 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3152 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       71 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       44 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       14 2023-06-04 05:25:59.000000 rfswarm-agent-1.1.3/rfswarm_agent.egg-info/top_level.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)     1138 2023-06-04 05:25:57.000000 rfswarm-agent-1.1.3/setup-agent.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-04 05:25:59.301699 rfswarm-agent-1.1.3/setup.cfg
```

### Comparing `rfswarm-agent-1.1.2/LICENSE` & `rfswarm-agent-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rfswarm-agent-1.1.2/PKG-INFO` & `rfswarm-agent-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-agent
-Version: 1.1.2
+Version: 1.1.3
 Summary: rfswarm Agent
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

### Comparing `rfswarm-agent-1.1.2/README.md` & `rfswarm-agent-1.1.3/README.md`

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

### Comparing `rfswarm-agent-1.1.2/rfswarm_agent/rfswarm_agent.py` & `rfswarm-agent-1.1.3/rfswarm_agent/rfswarm_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 #
 # 	Robot Framework Swarm
 #
-#    Version 1.1.2
+#    Version 1.1.3
 #
 
 
 # https://stackoverflow.com/questions/48090535/csv-file-reading-and-find-the-value-from-nth-column-using-robot-framework
 
 import argparse
 import base64
@@ -31,15 +31,15 @@
 import pkg_resources
 import psutil
 import requests
 
 
 class RFSwarmAgent():
 
-	version = "1.1.2"
+	version = "1.1.3"
 	config = None
 	isconnected = False
 	isrunning = False
 	isstopping = False
 	runagent = True
 	run_name = None
 	swarmmanager = None
```

### Comparing `rfswarm-agent-1.1.2/rfswarm_agent.egg-info/PKG-INFO` & `rfswarm-agent-1.1.3/rfswarm_agent.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfswarm-agent
-Version: 1.1.2
+Version: 1.1.3
 Summary: rfswarm Agent
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

### Comparing `rfswarm-agent-1.1.2/setup-agent.py` & `rfswarm-agent-1.1.3/setup-agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README_PyPi.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="rfswarm-agent",
-	version="1.1.2",
+	version="1.1.3",
 	author="damies13",
 	author_email="damies13+rfswarm@gmail.com",
 	description="rfswarm Agent",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/damies13/rfswarm",
 	packages=setuptools.find_packages(exclude=["*fswarm_report*", "*rfswarm_manager*", "build/*"]),
```

