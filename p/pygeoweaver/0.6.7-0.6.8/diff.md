# Comparing `tmp/pygeoweaver-0.6.7.tar.gz` & `tmp/pygeoweaver-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.6.7.tar", last modified: Wed May 31 17:41:58 2023, max compression
+gzip compressed data, was "pygeoweaver-0.6.8.tar", last modified: Sun Jun  4 15:31:47 2023, max compression
```

## Comparing `pygeoweaver-0.6.7.tar` & `pygeoweaver-0.6.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_resetpassword.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-31 17:41:58.000000 pygeoweaver-0.6.7/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-31 17:41:58.000000 pygeoweaver-0.6.7/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:41:58.000000 pygeoweaver-0.6.7/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 17:41:58.000000 pygeoweaver-0.6.7/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:41:58.520155 pygeoweaver-0.6.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/test/test_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-31 17:41:42.000000 pygeoweaver-0.6.7/test/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_resetpassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-04 15:31:47.000000 pygeoweaver-0.6.8/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-04 15:31:47.000000 pygeoweaver-0.6.8/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:31:47.000000 pygeoweaver-0.6.8/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-04 15:31:47.000000 pygeoweaver-0.6.8/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:31:47.036620 pygeoweaver-0.6.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/test/test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-04 15:31:36.000000 pygeoweaver-0.6.8/test/test_server.py
```

### Comparing `pygeoweaver-0.6.7/LICENSE` & `pygeoweaver-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.7/PKG-INFO` & `pygeoweaver-0.6.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.7
+Version: 0.6.8
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.7/README.md` & `pygeoweaver-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.7/pygeoweaver/__main__.py` & `pygeoweaver-0.6.8/pygeoweaver/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 The main function of pygeoweaver
 To run in CLI mode. 
 """
 from pygeoweaver import detail_host, detail_process, detail_workflow, export_workflow, \
     show_history, import_workflow, list_hosts, list_processes, list_workflows, \
-    start, stop, reset_password, run_process, run_worklfow, helpwith, ui
+    start, stop, reset_password, run_process, run_worklfow, helpwith
 from pygeoweaver.server import show
+from pygeoweaver.utils import check_java
+
 
 def main():
     # start geoweaver
     # start()
     # stop geoweaver
     # stop()
     # list resources
@@ -36,11 +38,12 @@
 
     # run workflow by folder path
 
     # reset localhost password for Geoweaver
     # reset_password()
     show()
     # helpwith()
+    # check_java()
 
 
 if __name__ == "__main__":
      main()
```

### Comparing `pygeoweaver-0.6.7/pygeoweaver/sc_detail.py` & `pygeoweaver-0.6.8/pygeoweaver/sc_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.7/pygeoweaver/sc_export.py` & `pygeoweaver-0.6.8/pygeoweaver/sc_export.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.7/pygeoweaver/sc_help.py` & `pygeoweaver-0.6.8/pygeoweaver/sc_help.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.7/pygeoweaver/sc_import.py` & `pygeoweaver-0.6.8/pygeoweaver/sc_import.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.7/pygeoweaver/sc_list.py` & `pygeoweaver-0.6.8/pygeoweaver/sc_list.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.7/pygeoweaver/sc_run.py` & `pygeoweaver-0.6.8/pygeoweaver/sc_run.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.7/pygeoweaver/server.py` & `pygeoweaver-0.6.8/pygeoweaver/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 import os
 import subprocess
 import webbrowser
 from pygeoweaver.constants import GEOWEAVER_DEFAULT_ENDPOINT_URL
-from pygeoweaver.utils import checkIPython, checkOS, download_geoweaver_jar, get_logger, get_module_absolute_path, get_root_dir
+from pygeoweaver.utils import check_ipython, check_os, download_geoweaver_jar, get_logger, get_module_absolute_path, \
+    get_root_dir
 
 """
 This module provides function to start and stop Geoweaver server.
 If it detects the current environment is Jupyter notebook, it will 
 open Geoweaver GUI in the output cell (if gui is not disabld.)
 
 """
 
 logger = get_logger(__name__)
 
+
 def start(force=False):
     download_geoweaver_jar(overwrite=force)
-    if checkOS() == 3:
-        raise RuntimeError("windows is not supported yet")
+    if check_os() == 3:
+        subprocess.run([f'{get_module_absolute_path()}/start.bat'], cwd=f"{get_root_dir()}/")
     else:
-        result = subprocess.run([f'{get_module_absolute_path()}/start.sh'], cwd=f"{get_root_dir()}/")
-    
+        subprocess.run([f'{get_module_absolute_path()}/start.sh'], cwd=f"{get_root_dir()}/")
 
 
 def stop():
-    if checkOS() == 3:
-        raise RuntimeError("Windows is not supported yet")
+    if check_os() == 3:
+        subprocess.run([f'{get_module_absolute_path()}/stop.bat'], cwd=f"{get_root_dir()}/", shell=True)
     else:
-        result = subprocess.run([f'{get_module_absolute_path()}/stop.sh'], cwd=f"{get_root_dir()}/", shell=True)
-    
+        subprocess.run([f'{get_module_absolute_path()}/stop.sh'], cwd=f"{get_root_dir()}/", shell=True)
+
 
-def show(geoweaver_url = GEOWEAVER_DEFAULT_ENDPOINT_URL):
+def show(geoweaver_url=GEOWEAVER_DEFAULT_ENDPOINT_URL):
     download_geoweaver_jar()  # check if geoweaver is initialized
-    if checkIPython():
+    if check_ipython():
         logger.info("enter ipython block")
         from IPython.display import IFrame
         return IFrame(src=geoweaver_url, width='100%', height='500px')
     else:
         logger.info("enter self opening block")
         webbrowser.open(geoweaver_url)
-
-
```

### Comparing `pygeoweaver-0.6.7/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.6.8/pygeoweaver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.7
+Version: 0.6.8
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.7/pygeoweaver.egg-info/SOURCES.txt` & `pygeoweaver-0.6.8/pygeoweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.7/pyproject.toml` & `pygeoweaver-0.6.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "pytest-cov"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.6.7"
+version = "0.6.8"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,15 +18,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry]
 name = "pygeoweaver"
-version = "0.6.7"
+version = "0.6.8"
 description = "This is a wrapper package of the Geoweaver app."
 authors = ["Geoweaver team <geoweaver.app@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
```

### Comparing `pygeoweaver-0.6.7/test/test_detail.py` & `pygeoweaver-0.6.8/test/test_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.7/test/test_server.py` & `pygeoweaver-0.6.8/test/test_server.py`

 * *Files identical despite different names*

