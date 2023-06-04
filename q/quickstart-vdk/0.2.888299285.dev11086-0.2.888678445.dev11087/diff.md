# Comparing `tmp/quickstart-vdk-0.2.888299285.dev11086.tar.gz` & `tmp/quickstart-vdk-0.2.888678445.dev11087.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.888299285.dev11086.tar", last modified: Sat Jun  3 04:22:39 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.888678445.dev11087.tar", last modified: Sun Jun  4 04:23:00 2023, max compression
```

## Comparing `quickstart-vdk-0.2.888299285.dev11086.tar` & `quickstart-vdk-0.2.888678445.dev11087.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 04:22:39.585345 quickstart-vdk-0.2.888299285.dev11086/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-03 04:22:39.585345 quickstart-vdk-0.2.888299285.dev11086/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-03 04:19:54.000000 quickstart-vdk-0.2.888299285.dev11086/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 04:22:39.581345 quickstart-vdk-0.2.888299285.dev11086/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-03 04:22:39.000000 quickstart-vdk-0.2.888299285.dev11086/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-03 04:22:39.000000 quickstart-vdk-0.2.888299285.dev11086/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 04:22:39.000000 quickstart-vdk-0.2.888299285.dev11086/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-03 04:22:39.000000 quickstart-vdk-0.2.888299285.dev11086/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-03 04:22:39.000000 quickstart-vdk-0.2.888299285.dev11086/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 04:22:39.585345 quickstart-vdk-0.2.888299285.dev11086/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-03 04:22:29.000000 quickstart-vdk-0.2.888299285.dev11086/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 04:22:39.585345 quickstart-vdk-0.2.888299285.dev11086/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-03 04:19:54.000000 quickstart-vdk-0.2.888299285.dev11086/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:23:00.842533 quickstart-vdk-0.2.888678445.dev11087/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-04 04:23:00.838533 quickstart-vdk-0.2.888678445.dev11087/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-04 04:20:19.000000 quickstart-vdk-0.2.888678445.dev11087/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:23:00.838533 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-04 04:23:00.000000 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-04 04:23:00.000000 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 04:23:00.000000 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-04 04:23:00.000000 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-04 04:23:00.000000 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 04:23:00.842533 quickstart-vdk-0.2.888678445.dev11087/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-04 04:22:50.000000 quickstart-vdk-0.2.888678445.dev11087/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:23:00.838533 quickstart-vdk-0.2.888678445.dev11087/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-04 04:20:19.000000 quickstart-vdk-0.2.888678445.dev11087/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.888299285.dev11086/PKG-INFO` & `quickstart-vdk-0.2.888678445.dev11087/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.888299285.dev11086
+Version: 0.2.888678445.dev11087
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.888299285.dev11086/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.888299285.dev11086
+Version: 0.2.888678445.dev11087
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.888299285.dev11086/setup.py` & `quickstart-vdk-0.2.888678445.dev11087/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.888299285.dev11086"
+__version__ = "0.2.888678445.dev11087"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

