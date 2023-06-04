# Comparing `tmp/NREL-gaps-0.3.3.tar.gz` & `tmp/NREL-gaps-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-gaps-0.3.3.tar", last modified: Mon May 22 22:12:59 2023, max compression
+gzip compressed data, was "NREL-gaps-0.3.4.tar", last modified: Sun Jun  4 20:48:47 2023, max compression
```

## Comparing `NREL-gaps-0.3.3.tar` & `NREL-gaps-0.3.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:12:59.648186 NREL-gaps-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:12:59.644186 NREL-gaps-0.3.3/NREL_gaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 22:12:59.000000 NREL-gaps-0.3.3/NREL_gaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-22 22:12:59.648186 NREL-gaps-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:12:59.648186 NREL-gaps-0.3.3/gaps/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:12:59.648186 NREL-gaps-0.3.3/gaps/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)    29981 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/cli/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    32534 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23886 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/project_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/gaps/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 22:12:59.648186 NREL-gaps-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-22 22:12:50.000000 NREL-gaps-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:48:47.391908 NREL-gaps-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:48:47.391908 NREL-gaps-0.3.4/NREL_gaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-04 20:48:47.000000 NREL-gaps-0.3.4/NREL_gaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-04 20:48:47.000000 NREL-gaps-0.3.4/NREL_gaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:48:47.000000 NREL-gaps-0.3.4/NREL_gaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:48:47.000000 NREL-gaps-0.3.4/NREL_gaps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-04 20:48:47.000000 NREL-gaps-0.3.4/NREL_gaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 20:48:47.000000 NREL-gaps-0.3.4/NREL_gaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-04 20:48:47.391908 NREL-gaps-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:48:47.391908 NREL-gaps-0.3.4/gaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:48:47.391908 NREL-gaps-0.3.4/gaps/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32224 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/cli/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32534 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23886 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11008 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/project_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/gaps/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:48:47.391908 NREL-gaps-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-04 20:48:38.000000 NREL-gaps-0.3.4/setup.py
```

### Comparing `NREL-gaps-0.3.3/LICENSE` & `NREL-gaps-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/NREL_gaps.egg-info/PKG-INFO` & `NREL-gaps-0.3.4/NREL_gaps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-gaps
-Version: 0.3.3
+Version: 0.3.4
 Summary: National Renewable Energy Laboratory's (NREL's) Geospatial Analysis Pipelines (GAPs) framework
 Home-page: https://nrel.github.io/gaps/
 Author: Paul Pinchuk
 Maintainer-email: ppinchuk@nrel.gov
 License: BSD 3-Clause
 Keywords: gaps
 Classifier: Development Status :: 4 - Beta
```

### Comparing `NREL-gaps-0.3.3/NREL_gaps.egg-info/SOURCES.txt` & `NREL-gaps-0.3.4/NREL_gaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/PKG-INFO` & `NREL-gaps-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-gaps
-Version: 0.3.3
+Version: 0.3.4
 Summary: National Renewable Energy Laboratory's (NREL's) Geospatial Analysis Pipelines (GAPs) framework
 Home-page: https://nrel.github.io/gaps/
 Author: Paul Pinchuk
 Maintainer-email: ppinchuk@nrel.gov
 License: BSD 3-Clause
 Keywords: gaps
 Classifier: Development Status :: 4 - Beta
```

### Comparing `NREL-gaps-0.3.3/README.rst` & `NREL-gaps-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/batch.py` & `NREL-gaps-0.3.4/gaps/batch.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/cli/batch.py` & `NREL-gaps-0.3.4/gaps/cli/batch.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/cli/cli.py` & `NREL-gaps-0.3.4/gaps/cli/cli.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/cli/collect.py` & `NREL-gaps-0.3.4/gaps/cli/collect.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/cli/command.py` & `NREL-gaps-0.3.4/gaps/cli/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 GAPS_SUPPLIED_ARGS = {
     "tag",
     "command_name",
     "config_file",
     "project_dir",
     "job_name",
     "out_dir",
+    "out_fpath",
     "config",
 }
 
 
 class AbstractBaseCLICommandConfiguration(ABC):
     """Abstract Base CLI Command representation.
 
@@ -127,30 +128,44 @@
                     avoiding clashing output files with jobs on other
                     nodes. This string  contains a leading underscore,
                     so the file name can easily be generated:
                     ``f"{out_file_name}{tag}.{extension}"``.
                 command_name : str
                     Name of the command being run. This is equivalent to
                     the ``name`` input argument.
-                config_file : Path
+                config_file : str
                     Path to the configuration file specified by the
                     user.
-                project_dir : Path
+                project_dir : str
                     Path to the project directory (parent directory of
                     the configuration file).
                 job_name : str
                     Name of the job being run. This is typically a
                     combination of the project directory, the command
                     name, and a tag unique to a job. Note that the tag
                     will not be included if you request this argument
                     in a config preprocessing function, as the execution
                     has not been split into multiple jobs by that point.
-                out_dir : Path
+                out_dir : str
                     Path to output directory - typically equivalent to
                     the project directory.
+                out_fpath : str
+                    Suggested path to output file. You are not required
+                    to use this argument - it is provided purely for
+                    convenience purposes. This argument combines the
+                    ``out_dir`` with ``job_name`` to yield a unique
+                    output filepath for a given node. Note that the
+                    output filename will contain the tag if it is
+                    "requested" from a node function, but *WILL NOT*
+                    contain a tag if requested from a config
+                    pre-processing function, since the number of split
+                    nodes have not been determined at that point.
+                    Also note that this string *WILL NOT* contain a
+                    file-ending, so that will have to be added by the
+                    node function.
 
             If your function is capable of multiprocessing, you should
             also include ``max_workers`` in the function signature.
             ``gaps`` will pass an integer equal to the number of
             processes the user wants to run on a single node for this
             value. Note that the ``config`` parameter is not allowed as
             a function signature item. Please request all the required
@@ -224,30 +239,51 @@
             requirements layed out above. At minimum, this function
             should have "config" as the first parameter (which will
             receive the user configuration input as a dictionary) and
             *must* return the updated config dictionary. This function
             can also "request" the following arguments by including them
             in the function signature:
 
+                tag : str
+                    Short string unique to this job run that can be used
+                    to generate unique output filenames, thereby
+                    avoiding clashing output files with jobs on other
+                    nodes. This string  contains a leading underscore,
+                    so the file name can easily be generated:
+                    ``f"{out_file_name}{tag}.{extension}"``.
                 command_name : str
                     Name of the command being run. This is equivalent to
                     the ``name`` input above.
-                config_file : Path
+                config_file : str
                     Path to the configuration file specified by the
                     user.
-                project_dir : Path
+                project_dir : str
                     Path to the project directory (parent directory of
                     the configuration file).
                 job_name : str
                     Name of the job being run. This is typically a
                     combination of the project directory and the command
                     name.
-                out_dir : Path
+                out_dir : str
                     Path to output directory - typically equivalent to
                     the project directory.
+                out_fpath : str
+                    Suggested path to output file. You are not required
+                    to use this argument - it is provided purely for
+                    convenience purposes. This argument combines the
+                    ``out_dir`` with ``job_name`` to yield a unique
+                    output filepath for a given node. Note that the
+                    output filename will contain the tag if it is
+                    "requested" from a node function, but *WILL NOT*
+                    contain a tag if requested from a config
+                    pre-processing function, since the number of split
+                    nodes have not been determined at that point.
+                    Also note that this string *WILL NOT* contain a
+                    file-ending, so that will have to be added by the
+                    node function.
 
             These inputs will be provided by GAPs and *will not* be
             displayed to users in the template configuration files or
             documentation. See
             :func:`gaps.cli.preprocessing.preprocess_collect_config`
             for an example. Note that the ``tag`` parameter is not
             allowed as a pre-processing function signature item (the
```

### Comparing `NREL-gaps-0.3.3/gaps/cli/config.py` & `NREL-gaps-0.3.4/gaps/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,15 @@
                 {
                     "tag": tag,
                     "command_name": self.command_name,
                     "config_file": self.config_file.as_posix(),
                     "project_dir": self.project_dir.as_posix(),
                     "job_name": job_name,
                     "out_dir": self.project_dir.as_posix(),
+                    "out_fpath": (self.project_dir / job_name).as_posix(),
                     "max_workers": max_workers_per_node,
                     "run_method": getattr(
                         self.command_config, "run_method", None
                     ),
                 }
             )
```

### Comparing `NREL-gaps-0.3.3/gaps/cli/documentation.py` & `NREL-gaps-0.3.4/gaps/cli/documentation.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/cli/execution.py` & `NREL-gaps-0.3.4/gaps/cli/execution.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/cli/pipeline.py` & `NREL-gaps-0.3.4/gaps/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/cli/preprocessing.py` & `NREL-gaps-0.3.4/gaps/cli/preprocessing.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/cli/status.py` & `NREL-gaps-0.3.4/gaps/cli/status.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/cli/templates.py` & `NREL-gaps-0.3.4/gaps/cli/templates.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/collection.py` & `NREL-gaps-0.3.4/gaps/collection.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/config.py` & `NREL-gaps-0.3.4/gaps/config.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/exceptions.py` & `NREL-gaps-0.3.4/gaps/exceptions.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/hpc.py` & `NREL-gaps-0.3.4/gaps/hpc.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/legacy.py` & `NREL-gaps-0.3.4/gaps/legacy.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/log.py` & `NREL-gaps-0.3.4/gaps/log.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/pipeline.py` & `NREL-gaps-0.3.4/gaps/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/project_points.py` & `NREL-gaps-0.3.4/gaps/project_points.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/status.py` & `NREL-gaps-0.3.4/gaps/status.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/utilities.py` & `NREL-gaps-0.3.4/gaps/utilities.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/gaps/warnings.py` & `NREL-gaps-0.3.4/gaps/warnings.py`

 * *Files identical despite different names*

### Comparing `NREL-gaps-0.3.3/setup.py` & `NREL-gaps-0.3.4/setup.py`

 * *Files identical despite different names*

