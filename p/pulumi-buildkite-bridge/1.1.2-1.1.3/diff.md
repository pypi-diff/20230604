# Comparing `tmp/pulumi_buildkite_bridge-1.1.2.tar.gz` & `tmp/pulumi_buildkite_bridge-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_buildkite_bridge-1.1.2.tar", last modified: Sun Jun  4 15:44:01 2023, max compression
+gzip compressed data, was "pulumi_buildkite_bridge-1.1.3.tar", last modified: Sun Jun  4 16:00:59 2023, max compression
```

## Comparing `pulumi_buildkite_bridge-1.1.2.tar` & `pulumi_buildkite_bridge-1.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:44:01.264527 pulumi_buildkite_bridge-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-04 15:44:01.264527 pulumi_buildkite_bridge-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:44:01.260527 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:44:01.260527 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/agent/agent_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:44:01.260527 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/get_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:44:01.260527 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/organization/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/organization/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:44:01.260527 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/get_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59582 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:44:01.264527 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/team/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/team/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/team/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/team/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/team/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:44:01.260527 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 15:44:01.264527 pulumi_buildkite_bridge-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-04 15:44:01.000000 pulumi_buildkite_bridge-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:00:59.644353 pulumi_buildkite_bridge-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-04 16:00:59.644353 pulumi_buildkite_bridge-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:00:59.640353 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:00:59.640353 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/agent/agent_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:00:59.640353 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/get_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:00:59.640353 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/organization/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/organization/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:00:59.644353 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/get_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59582 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:00:59.644353 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/team/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/team/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/team/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/team/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/team/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:00:59.640353 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 16:00:59.644353 pulumi_buildkite_bridge-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-04 16:00:59.000000 pulumi_buildkite_bridge-1.1.3/setup.py
```

### Comparing `pulumi_buildkite_bridge-1.1.2/PKG-INFO` & `pulumi_buildkite_bridge-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_buildkite_bridge
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Pulumi package for creating and managing Buildkite resources.
 Home-page: https://github.com/muhlba91/pulumi-buildkite
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-buildkite
 Keywords: pulumi buildkite
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_buildkite_bridge-1.1.2/README.md` & `pulumi_buildkite_bridge-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/__init__.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/_utilities.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/agent/agent_token.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/agent/agent_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/config/vars.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/get_meta.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/get_meta.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/organization/get_organization.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/organization/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/organization/settings.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/organization/settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/_inputs.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/get_pipeline.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/get_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/outputs.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/pipeline.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/pipeline/schedule.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/pipeline/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/provider.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/team/get_team.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/team/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/team/member.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/team/member.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge/team/team.py` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge/team/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge.egg-info/PKG-INFO` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-buildkite-bridge
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Pulumi package for creating and managing Buildkite resources.
 Home-page: https://github.com/muhlba91/pulumi-buildkite
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-buildkite
 Keywords: pulumi buildkite
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_buildkite_bridge-1.1.2/pulumi_buildkite_bridge.egg-info/SOURCES.txt` & `pulumi_buildkite_bridge-1.1.3/pulumi_buildkite_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_buildkite_bridge-1.1.2/setup.py` & `pulumi_buildkite_bridge-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.1.2"
-PLUGIN_VERSION = "1.1.2"
+VERSION = "1.1.3"
+PLUGIN_VERSION = "1.1.3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'buildkite', PLUGIN_VERSION, '--server', 'github://api.github.com/muhlba91/pulumi-buildkite'])
         except OSError as error:
```

