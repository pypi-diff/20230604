# Comparing `tmp/volare-0.7.3.tar.gz` & `tmp/volare-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/volare-0.7.3.tar", last modified: Wed May 24 15:16:24 2023, max compression
+gzip compressed data, was "dist/volare-0.8.0.tar", last modified: Sun Jun  4 12:33:37 2023, max compression
```

## Comparing `volare-0.7.3.tar` & `volare-0.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:16:24.000000 volare-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 15:16:24.000000 volare-0.7.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      931 2023-05-24 15:16:04.000000 volare-0.7.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-05-24 15:16:24.000000 volare-0.7.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:16:24.000000 volare-0.7.3/volare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-24 15:16:23.000000 volare-0.7.3/volare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-24 15:16:23.000000 volare-0.7.3/volare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 15:16:23.000000 volare-0.7.3/volare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-05-24 15:16:23.000000 volare-0.7.3/volare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-24 15:16:23.000000 volare-0.7.3/volare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-05-24 15:16:24.000000 volare-0.7.3/volare.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:16:24.000000 volare-0.7.3/volare/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 15:16:24.000000 volare-0.7.3/volare/build/
--rw-r--r--   0 runner    (1001) docker     (122)     7450 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/git_multi_clone.py
--rw-r--r--   0 runner    (1001) docker     (122)     9219 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/gf180mcu.py
--rw-r--r--   0 runner    (1001) docker     (122)     4931 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/asap7.py
--rw-r--r--   0 runner    (1001) docker     (122)    13938 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/sky130.py
--rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-05-24 15:16:04.000000 volare-0.7.3/volare/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2023-05-24 15:16:04.000000 volare-0.7.3/volare/families.py
--rw-r--r--   0 runner    (1001) docker     (122)    13864 2023-05-24 15:16:04.000000 volare-0.7.3/volare/manage.py
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-05-24 15:16:04.000000 volare-0.7.3/volare/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 15:16:04.000000 volare-0.7.3/volare/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     7777 2023-05-24 15:16:04.000000 volare-0.7.3/volare/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3289 2023-05-24 15:16:04.000000 volare-0.7.3/volare/click_common.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1667 2023-05-24 15:16:04.000000 volare-0.7.3/volare/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-05-24 15:16:04.000000 volare-0.7.3/volare/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-04 12:33:37.000000 volare-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-06-04 12:33:37.000000 volare-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-04 12:33:37.000000 volare-0.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)      931 2023-06-04 12:33:15.000000 volare-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-04 12:33:37.000000 volare-0.8.0/volare/
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-06-04 12:33:15.000000 volare-0.8.0/volare/click_common.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-04 12:33:37.000000 volare-0.8.0/volare/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-06-04 12:33:15.000000 volare-0.8.0/volare/build/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4908 2023-06-04 12:33:15.000000 volare-0.8.0/volare/build/asap7.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9215 2023-06-04 12:33:15.000000 volare-0.8.0/volare/build/gf180mcu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13832 2023-06-04 12:33:15.000000 volare-0.8.0/volare/build/sky130.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7450 2023-06-04 12:33:15.000000 volare-0.8.0/volare/build/git_multi_clone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6478 2023-06-04 12:33:15.000000 volare-0.8.0/volare/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15559 2023-06-04 12:33:15.000000 volare-0.8.0/volare/manage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10818 2023-06-04 12:33:15.000000 volare-0.8.0/volare/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-06-04 12:33:15.000000 volare-0.8.0/volare/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1489 2023-06-04 12:33:15.000000 volare-0.8.0/volare/families.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1673 2023-06-04 12:33:15.000000 volare-0.8.0/volare/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-04 12:33:15.000000 volare-0.8.0/volare/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-04 12:33:15.000000 volare-0.8.0/volare/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-04 12:33:37.000000 volare-0.8.0/volare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-04 12:33:37.000000 volare-0.8.0/volare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-04 12:33:37.000000 volare-0.8.0/volare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-06-04 12:33:37.000000 volare-0.8.0/volare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-06-04 12:33:37.000000 volare-0.8.0/volare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-04 12:33:37.000000 volare-0.8.0/volare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-04 12:33:37.000000 volare-0.8.0/volare.egg-info/requires.txt
```

### Comparing `volare-0.7.3/setup.py` & `volare-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.3/PKG-INFO` & `volare-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volare
-Version: 0.7.3
+Version: 0.8.0
 Summary: An open_pdks PDK builder/version manager
 Home-page: UNKNOWN
 Author: Efabless Corporation
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">⛰️ Volare</h1>
         <p align="center">
@@ -72,15 +72,15 @@
         
         |sky130|gf180mcu|
         |-|-|
         |sky130_fd_io|gf180mcu_fd_io|
         |sky130_fd_pr|gf180mcu_fd_pr|
         |sky130_fd_sc_hd|gf180mcu_fd_sc_mcu7t5v0|
         |sky130_fd_sc_hvl|gf180mcu_fd_sc_mcu9t5v0|
-        |sky130 sram modules|gf180mcu_fd_bd_sram|
+        |sky130 sram modules|gf180mcu_fd_ip_sram|
         
         All builds are identified by their **open_pdks** commit hash.
         
         # Usage
         Volare requires a so-called **PDK Root**. This PDK root can be anywhere on your computer, but by default it's the folder `~/.volare` in your home directory. If you have the variable `PDK_ROOT` set, volare will use that instead. You can also manually override both values by supplying the `--pdk-root` commandline argument.
         
         ## Listing All Available PDKs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volare Version: 0.7.3 Summary: An open_pdks PDK
+Metadata-Version: 2.1 Name: volare Version: 0.8.0 Summary: An open_pdks PDK
 builder/version manager Home-page: UNKNOWN Author: Efabless Corporation Author-
 email: donn@efabless.com License: UNKNOWN Description:
                           ****** â°ï¸ Volare ******
   [License:_Apache_2.0] [CI Status] [Invite_to_the_Skywater_PDK_Slack] [Code
                                  Style:_Black]
 Volare is a version manager (and builder) for builds of Google_open-source_PDKs
                                using open_pdks.
@@ -26,15 +26,15 @@
 `sudo` (absolutely not recommended) or not, so ensure that you actually read
 the warning and add the correct path. # About the builds In its current
 inception, volare supports builds of **sky130** and **gf180mcu** PDKs using
 [Open_PDKs](https://github.com/efabless/open_pdks), including the following
 libraries: |sky130|gf180mcu| |-|-| |sky130_fd_io|gf180mcu_fd_io|
 |sky130_fd_pr|gf180mcu_fd_pr| |sky130_fd_sc_hd|gf180mcu_fd_sc_mcu7t5v0|
 |sky130_fd_sc_hvl|gf180mcu_fd_sc_mcu9t5v0| |sky130 sram
-modules|gf180mcu_fd_bd_sram| All builds are identified by their **open_pdks**
+modules|gf180mcu_fd_ip_sram| All builds are identified by their **open_pdks**
 commit hash. # Usage Volare requires a so-called **PDK Root**. This PDK root
 can be anywhere on your computer, but by default it's the folder `~/.volare` in
 your home directory. If you have the variable `PDK_ROOT` set, volare will use
 that instead. You can also manually override both values by supplying the `--
 pdk-root` commandline argument. ## Listing All Available PDKs To list all
 available pre-built PDKs hosted in this repository, you can just invoke `volare
 ls-remote --pdk `. If you omit the `--pdk` argument, `sky130` will be used as a
```

### Comparing `volare-0.7.3/volare.egg-info/PKG-INFO` & `volare-0.8.0/volare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volare
-Version: 0.7.3
+Version: 0.8.0
 Summary: An open_pdks PDK builder/version manager
 Home-page: UNKNOWN
 Author: Efabless Corporation
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">⛰️ Volare</h1>
         <p align="center">
@@ -72,15 +72,15 @@
         
         |sky130|gf180mcu|
         |-|-|
         |sky130_fd_io|gf180mcu_fd_io|
         |sky130_fd_pr|gf180mcu_fd_pr|
         |sky130_fd_sc_hd|gf180mcu_fd_sc_mcu7t5v0|
         |sky130_fd_sc_hvl|gf180mcu_fd_sc_mcu9t5v0|
-        |sky130 sram modules|gf180mcu_fd_bd_sram|
+        |sky130 sram modules|gf180mcu_fd_ip_sram|
         
         All builds are identified by their **open_pdks** commit hash.
         
         # Usage
         Volare requires a so-called **PDK Root**. This PDK root can be anywhere on your computer, but by default it's the folder `~/.volare` in your home directory. If you have the variable `PDK_ROOT` set, volare will use that instead. You can also manually override both values by supplying the `--pdk-root` commandline argument.
         
         ## Listing All Available PDKs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volare Version: 0.7.3 Summary: An open_pdks PDK
+Metadata-Version: 2.1 Name: volare Version: 0.8.0 Summary: An open_pdks PDK
 builder/version manager Home-page: UNKNOWN Author: Efabless Corporation Author-
 email: donn@efabless.com License: UNKNOWN Description:
                           ****** â°ï¸ Volare ******
   [License:_Apache_2.0] [CI Status] [Invite_to_the_Skywater_PDK_Slack] [Code
                                  Style:_Black]
 Volare is a version manager (and builder) for builds of Google_open-source_PDKs
                                using open_pdks.
@@ -26,15 +26,15 @@
 `sudo` (absolutely not recommended) or not, so ensure that you actually read
 the warning and add the correct path. # About the builds In its current
 inception, volare supports builds of **sky130** and **gf180mcu** PDKs using
 [Open_PDKs](https://github.com/efabless/open_pdks), including the following
 libraries: |sky130|gf180mcu| |-|-| |sky130_fd_io|gf180mcu_fd_io|
 |sky130_fd_pr|gf180mcu_fd_pr| |sky130_fd_sc_hd|gf180mcu_fd_sc_mcu7t5v0|
 |sky130_fd_sc_hvl|gf180mcu_fd_sc_mcu9t5v0| |sky130 sram
-modules|gf180mcu_fd_bd_sram| All builds are identified by their **open_pdks**
+modules|gf180mcu_fd_ip_sram| All builds are identified by their **open_pdks**
 commit hash. # Usage Volare requires a so-called **PDK Root**. This PDK root
 can be anywhere on your computer, but by default it's the folder `~/.volare` in
 your home directory. If you have the variable `PDK_ROOT` set, volare will use
 that instead. You can also manually override both values by supplying the `--
 pdk-root` commandline argument. ## Listing All Available PDKs To list all
 available pre-built PDKs hosted in this repository, you can just invoke `volare
 ls-remote --pdk `. If you omit the `--pdk` argument, `sky130` will be used as a
```

### Comparing `volare-0.7.3/volare/build/git_multi_clone.py` & `volare-0.8.0/volare/build/git_multi_clone.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.3/volare/build/gf180mcu.py` & `volare-0.8.0/volare/build/gf180mcu.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,15 +117,17 @@
 
 
 LIB_FLAG_MAP = {
     "gf180mcu_fd_pr": "--enable-primitive-gf180mcu",
     "gf180mcu_fd_sc_mcu7t5v0": "--enable-sc-7t5v0-gf180mcu",
     "gf180mcu_fd_sc_mcu9t5v0": "--enable-sc-9t5v0-gf180mcu",
     "gf180mcu_fd_io": "--enable-io-gf180mcu",
-    "gf180mcu_fd_bd_sram": "--enable-sram-gf180mcu",
+    "gf180mcu_fd_ip_sram": "--enable-sram-gf180mcu",
+    "gf180mcu_osu_sc_gp12t3v3": "--enable-osu-sc-gf180mcu",
+    "gf180mcu_osu_sc_gp9t3v3": "--enable-osu-sc-gf180mcu",
 }
 
 
 def build_variants(
     magic_bin, include_libraries, build_directory, open_pdks_path, log_dir, jobs=1
 ):
 
@@ -145,15 +147,15 @@
                 )
             except subprocess.CalledProcessError as e:
                 console.log(
                     f"An error occurred while building the PDK. Check {log_to} for more information."
                 )
                 raise e
 
-        library_flags = [LIB_FLAG_MAP[library] for library in include_libraries]
+        library_flags = set([LIB_FLAG_MAP[library] for library in include_libraries])
         magic_dirname = os.path.dirname(magic_bin)
 
         with console.status("Configuring open_pdks…"):
             run_sh(
                 f"""
                     set -e
                     export PATH="{magic_dirname}:$PATH"
@@ -226,30 +228,23 @@
     console.log("Done.")
 
 
 def build(
     pdk_root: str,
     version: str,
     jobs: int = 1,
-    sram: bool = True,
     clear_build_artifacts: bool = True,
     include_libraries: Optional[List[str]] = None,
     using_repos: Optional[Dict[str, str]] = None,
     build_magic: bool = False,
 ):
-    if include_libraries is None or len(include_libraries) == 0:
-        include_libraries = [
-            "gf180mcu_fd_sc_mcu7t5v0",
-            "gf180mcu_fd_sc_mcu9t5v0",
-            "gf180mcu_fd_io",
-            "gf180mcu_fd_pr",
-        ]
-
-    if sram:
-        include_libraries.append("gf180mcu_fd_bd_sram")
+    if include_libraries is None:
+        include_libraries = Family.by_name["gf180mcu"].default_includes.copy()
+    if "all" in include_libraries:
+        include_libraries = list(LIB_FLAG_MAP.keys())
 
     if using_repos is None:
         using_repos = {}
 
     timestamp = datetime.now().strftime("build_gf180mcu-%Y-%m-%d-%H-%M-%S")
     log_dir = os.path.join(get_logs_dir(), timestamp)
     mkdirp(log_dir)
@@ -263,15 +258,15 @@
     open_pdks_path, _, magic_tag = get_open_pdks(
         version, build_directory, jobs, using_repos.get("open_pdks")
     )
     with_magic(
         magic_tag,
         lambda magic_bin: build_variants(
             magic_bin,
-            include_libraries,
+            list(include_libraries),
             build_directory,
             open_pdks_path,
             log_dir,
             jobs,
         ),
         build_magic=build_magic,
     )
```

### Comparing `volare-0.7.3/volare/build/asap7.py` & `volare-0.8.0/volare/build/asap7.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,14 @@
     console.log("Done.")
 
 
 def build(
     pdk_root: str,
     version: str,
     jobs: int = 1,
-    sram: bool = True,
     clear_build_artifacts: bool = True,
     include_libraries: Optional[List[str]] = None,
     using_repos: Optional[Dict[str, str]] = None,
     build_magic: bool = False,
 ):
     if using_repos is None:
         using_repos = {}
```

### Comparing `volare-0.7.3/volare/build/sky130.py` & `volare-0.8.0/volare/build/sky130.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,27 +362,21 @@
     console.log("Done.")
 
 
 def build(
     pdk_root: str,
     version: str,
     jobs: int = 1,
-    sram: bool = True,
     clear_build_artifacts: bool = True,
     include_libraries: Optional[List[str]] = None,
     using_repos: Optional[Dict[str, str]] = None,
     build_magic: bool = False,
 ):
-    if include_libraries is None or len(include_libraries) == 0:
-        include_libraries = [
-            "sky130_fd_sc_hd",
-            "sky130_fd_sc_hvl",
-            "sky130_fd_io",
-            "sky130_fd_pr",
-        ]
+    if include_libraries is None:
+        include_libraries = Family.by_name["sky130"].default_includes
 
     if using_repos is None:
         using_repos = {}
 
     timestamp = datetime.now().strftime("build_sky130-%Y-%m-%d-%H-%M-%S")
     log_dir = os.path.join(get_logs_dir(), timestamp)
     mkdirp(log_dir)
@@ -399,15 +393,15 @@
     )
     build_sky130_timing(build_directory, sky130_path, log_dir, jobs)
 
     with_magic(
         magic_tag,
         lambda magic_bin: build_variants(
             magic_bin,
-            sram,
+            "sky130_sram_macros" in include_libraries,
             build_directory,
             open_pdks_path,
             sky130_path,
             log_dir,
             jobs,
         ),
         build_magic=build_magic,
```

### Comparing `volare-0.7.3/volare/build/magic.py` & `volare-0.8.0/volare/build/magic.py`

 * *Files identical despite different names*

### Comparing `volare-0.7.3/volare/build/__init__.py` & `volare-0.8.0/volare/build/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import tarfile
 import tempfile
 import importlib
 import subprocess
 from typing import Optional, List
 
 import click
+import zstandard as zstd
 from rich.console import Console
 from rich.progress import Progress
 
 from ..common import (
     mkdirp,
     check_version,
     get_version_dir,
@@ -42,15 +43,15 @@
 
 
 def build(
     pdk_root: str,
     pdk: str,
     version: str,
     jobs: int = 1,
-    sram: bool = True,
+    sram: bool = True,  # Deprecated
     clear_build_artifacts: bool = True,
     include_libraries: Optional[List[str]] = None,
     use_repo_at: Optional[List[str]] = None,
     build_magic: bool = False,
 ):
     use_repos = {}
     if use_repo_at is not None:
@@ -61,15 +62,14 @@
     if pdk not in Family.by_name:
         raise Exception(f"Unsupported PDK family '{pdk}'.")
 
     kwargs = {
         "pdk_root": pdk_root,
         "version": version,
         "jobs": jobs,
-        "sram": sram,
         "clear_build_artifacts": clear_build_artifacts,
         "include_libraries": include_libraries,
         "using_repos": use_repos,
         "build_magic": build_magic,
     }
 
     build_module = importlib.import_module(f".{pdk}", package=__name__)
@@ -87,15 +87,14 @@
     default=None,
     help="Explicitly define a tool metadata file instead of searching for a metadata file",
 )
 @click.argument("version", required=False)
 def build_cmd(
     include_libraries,
     jobs,
-    sram,
     pdk_root,
     pdk,
     clear_build_artifacts,
     tool_metadata_file_path,
     version,
     use_repo_at,
     build_magic,
@@ -105,22 +104,23 @@
 
     Parameters: <version> (Optional)
 
     If a version is not given, and you run this in the top level directory of
     tools with a tool_metadata.yml file, for example OpenLane or DFFRAM,
     the appropriate version will be enabled automatically.
     """
+    if include_libraries == ():
+        include_libraries = None
 
     version = check_version(version, tool_metadata_file_path, Console())
     build(
         pdk_root=pdk_root,
         pdk=pdk,
         version=version,
         jobs=jobs,
-        sram=sram,
         clear_build_artifacts=clear_build_artifacts,
         include_libraries=include_libraries,
         use_repo_at=use_repo_at,
         build_magic=build_magic,
     )
 
 
@@ -140,57 +140,76 @@
         console.print("[red]Version not found.")
         exit(os.EX_NOINPUT)
 
     tempdir = tempfile.gettempdir()
     tarball_directory = os.path.join(tempdir, "volare", f"{uuid.uuid4()}", version)
     mkdirp(tarball_directory)
 
-    tarball_path = os.path.join(tarball_directory, "default.tar.xz")
+    final_tarballs = []
 
     with Progress() as progress:
+        collections = {"common": []}
         path_it = pathlib.Path(version_directory).glob("**/*")
-        files = [str(path) for path in path_it if path.is_file()]
-        task = progress.add_task("Compressing…", total=len(files))
-        with tarfile.open(tarball_path, mode="w:xz") as tf:
-            for i, file in enumerate(files):
-                progress.update(task, completed=i + 1)
-                path_in_tarball = os.path.relpath(file, version_directory)
-                tf.add(file, arcname=path_in_tarball)
-    console.log(f"Compressed to {tarball_path}.")
+        for path in path_it:
+            if not path.is_file():
+                continue
+            relative = os.path.relpath(path, version_directory)
+            path_components = relative.split(os.sep)
+            if path_components[1] == "libs.ref":
+                lib = path_components[2]
+                collections[lib] = collections.get(lib) or []
+                collections[lib].append(str(path))
+            else:
+                collections["common"].append(str(path))
+
+        for name, files in collections.items():
+            tarball_path = os.path.join(tarball_directory, f"{name}.tar.zst")
+            task = progress.add_task(f"Compressing {name}…", total=len(files))
+            with zstd.open(tarball_path, mode="wb") as stream:
+                with tarfile.TarFile(fileobj=stream, mode="w") as tf:
+                    for i, file in enumerate(files):
+                        progress.update(task, completed=i + 1)
+                        path_in_tarball = os.path.relpath(file, version_directory)
+                        tf.add(file, arcname=path_in_tarball)
+            console.log(f"\nCompressed to {tarball_path}.")
+            progress.remove_task(task)
+            final_tarballs.append(tarball_path)
 
     tag = f"{pdk}-{version}"
 
     # If someone wants to rewrite this to not use ghr, please, by all means.
     console.log("Starting upload…")
 
     body = f"{pdk} variants built using volare"
     date = get_date_of(version)
     if date is not None:
         body = f"{pdk} variants built using open_pdks {version} (released on {date_to_iso8601(date)})"
-    subprocess.check_call(
-        [
-            "ghr",
-            "-owner",
-            owner,
-            "-repository",
-            repository,
-            "-token",
-            token,
-            "-body",
-            body,
-            "-commitish",
-            "releases",
-            "-replace",
-        ]
-        + (["-prerelease"] if pre else [])
-        + [
-            tag,
-            tarball_path,
-        ]
-    )
+
+    for tarball_path in final_tarballs:
+        subprocess.check_call(
+            [
+                "ghr",
+                "-owner",
+                owner,
+                "-repository",
+                repository,
+                "-token",
+                token,
+                "-body",
+                body,
+                "-commitish",
+                "releases",
+                "-replace",
+            ]
+            + (["-prerelease"] if pre else [])
+            + [
+                tag,
+                tarball_path,
+            ]
+        )
     console.log("Done.")
 
 
 @click.command("push", hidden=True)
 @opt_pdk_root
 @opt_push
 @click.argument("version")
```

### Comparing `volare-0.7.3/volare/families.py` & `volare-0.8.0/volare/__version__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,22 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List, Dict
+__version__ = "0.8.0"
 
-
-class Family(object):
-    by_name: Dict[str, "Family"] = {}
-
-    def __init__(self, name: str, variants: List[str]):
-        self.name = name
-        self.variants = variants
-
-
-Family.by_name = {}
-Family.by_name["sky130"] = Family("sky130", ["sky130A", "sky130B"])
-Family.by_name["gf180mcu"] = Family("gf180mcu", ["gf180mcuA", "gf180mcuB", "gf180mcuC"])
-Family.by_name["asap7"] = Family("asap7", ["asap7"])
+if __name__ == "__main__":
+    print(__version__, end="")
```

### Comparing `volare-0.7.3/volare/manage.py` & `volare-0.8.0/volare/manage.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,31 +14,30 @@
 import os
 import sys
 import json
 import shutil
 import tarfile
 import requests
 import tempfile
-from typing import List, Optional
+from typing import Any, List, Optional
 
 import rich
 import click
 import rich.tree
 import rich.progress
+import zstandard as zstd
 from rich.console import Console
 
 from .build.git_multi_clone import mkdirp
 from .common import (
     Version,
-    get_link_of,
     check_version,
+    get_release_links,
     get_versions_dir,
-    get_version_dir,
     get_volare_dir,
-    get_current_version,
     get_installed_list,
 )
 from .click_common import (
     opt,
     opt_build,
     opt_push,
     opt_pdk_root,
@@ -88,27 +87,25 @@
 
 
 def print_remote_list(
     pdk_root: str, pdk: str, console: Console, pdk_list: List[Version]
 ):
     installed_list = get_installed_list(pdk_root, pdk)
 
-    version = get_current_version(pdk_root, pdk)
-
     tree = rich.tree.Tree(f"Pre-built {pdk} PDK versions")
     for remote_version in pdk_list:
         name = remote_version.name
         assert (
             remote_version.commit_date is not None
         ), f"Remote version {name} has no commit date"
         day = remote_version.commit_date.strftime("%Y.%m.%d")
         desc = f"[green]{name} ({day})"
         if remote_version.prerelease:
             desc = f"[red]PRE-RELEASE {desc}"
-        if name == version:
+        if remote_version.is_current(pdk_root):
             tree.add(f"[bold]{desc} (enabled)")
         elif name in installed_list:
             tree.add(f"{desc} (installed)")
         else:
             tree.add(desc)
     console.print(tree)
 
@@ -120,56 +117,77 @@
     """Outputs the currently enabled PDK version.
 
     If not outputting to a tty, the output is either the version string
     unembellished, or, if no current version is enabled, an empty output with an
     exit code of 1.
     """
 
-    version = get_current_version(pdk_root, pdk)
+    version = Version.get_current(pdk_root, pdk)
     if sys.stdout.isatty():
-        if version == "":
+        if version is None:
             print(f"No version of the PDK {pdk} is currently enabled at {pdk_root}.")
             print(
                 "Invoke volare --help for assistance installing and enabling versions."
             )
             exit(1)
         else:
-            print(f"Installed: {pdk} v{version}")
+            print(f"Installed: {pdk} v{version.name}")
             print(
                 "Invoke volare --help for assistance installing and enabling versions."
             )
     else:
-        if version == "":
+        if version is None:
             exit(1)
         else:
-            print(version, end="")
+            print(version.name, end="")
 
 
 @click.command("prune")
 @opt_pdk_root
 @click.option(
     "--yes",
     is_flag=True,
     callback=lambda c, _, v: not v and c.abort(),
     expose_value=False,
-    prompt="Are you sure? This will delete all non-current versions of the PDK from your computer.",
+    prompt="Are you sure? This will delete all non-enabled versions of the PDK from your computer.",
 )
 def prune_cmd(pdk_root, pdk):
     """Removes all PDKs other than, if it exists, the one currently in use."""
     pdk_versions = get_installed_list(pdk_root, pdk)
     for version in pdk_versions:
         if version.is_current(pdk_root):
             continue
         try:
-            shutil.rmtree(version.path)
+            version.uninstall()
             print(f"Deleted {version}.")
         except Exception as e:
             print(f"Failed to delete {version}: {e}", file=sys.stderr)
 
 
+@click.command("rm")
+@opt_pdk_root
+@click.option(
+    "--yes",
+    is_flag=True,
+    callback=lambda c, _, v: not v and c.abort(),
+    expose_value=False,
+    prompt="Are you sure? This will delete this version of the PDK from your computer.",
+)
+@click.argument("version", required=False)
+def rm_cmd(pdk_root, pdk, version):
+    """Removes the PDK version specified."""
+    version_object = Version(version, pdk)
+    try:
+        version_object.uninstall(pdk_root)
+        print(f"Deleted {version}.")
+    except Exception as e:
+        print(f"Failed to delete: {e}", file=sys.stderr)
+        exit(1)
+
+
 @click.command("ls")
 @opt_pdk_root
 def list_cmd(pdk_root, pdk):
     """Lists PDK versions that are locally installed. JSON if not outputting to a tty."""
 
     pdk_versions = get_installed_list(pdk_root, pdk)
 
@@ -206,107 +224,123 @@
 
 
 @click.command("path")
 @opt_pdk_root
 @click.argument("version", required=False)
 def path_cmd(pdk_root, pdk, version):
     """Prints the path of a specific pdk version installation."""
-    path_to_print = pdk_root
-    if version is not None:
-        path_to_print = os.path.join(get_versions_dir(pdk_root, pdk), version)
-    print(path_to_print, end="")
+    version = Version(version, pdk)
+    print(version.get_dir(pdk_root), end="")
 
 
 def enable(
     pdk_root: str,
     pdk: str,
     version: str,
     build_if_not_found=False,
     also_push=False,
     build_kwargs: dict = {},
     push_kwargs: dict = {},
+    include_libraries: Optional[List[str]] = None,
 ):
     console = Console()
 
     current_file = os.path.join(get_volare_dir(pdk_root, pdk), "current")
     current_file_dir = os.path.dirname(current_file)
     mkdirp(current_file_dir)
 
-    version_directory = get_version_dir(pdk_root, pdk, version)
+    version_object = Version(version, pdk)
+
+    version_directory = version_object.get_dir(pdk_root)
 
     pdk_family = Family.by_name.get(pdk)
     if pdk_family is None:
         print(f"Unsupported PDK family '{pdk}'.", file=sys.stderr)
         exit(os.EX_USAGE)
 
     variants = pdk_family.variants
 
     version_paths = [os.path.join(version_directory, variant) for variant in variants]
     final_paths = [os.path.join(pdk_root, variant) for variant in variants]
 
     if not os.path.exists(version_directory):
-        link = get_link_of(version, pdk)
-        status = requests.head(link).status_code
-        if status == 404:
-            console.print(f"Version {version} not found either locally or remotely.")
+        release_link_list = get_release_links(version, pdk, include_libraries)
+
+        if release_link_list is None:
             if build_if_not_found:
-                console.print("Attempting to build…")
+                console.print(f"Version {version} not found, attempting to build…")
                 build(pdk_root=pdk_root, pdk=pdk, version=version, **build_kwargs)
                 if also_push:
                     push(pdk_root=pdk_root, pdk=pdk, version=version, **push_kwargs)
             else:
                 console.print(
                     f"[red]Version {version} not found either locally or remotely.\nTry volare build {version}."
                 )
                 exit(1)
         else:
-            with tempfile.TemporaryDirectory(suffix=".volare") as tarball_directory:
-                tarball_path = os.path.join(tarball_directory, f"{version}.tar.xz")
-                with requests.get(link, stream=True) as r:
-                    assert isinstance(r, requests.Response)
-                    with rich.progress.Progress() as p:
+            try:
+                tarball_directory = tempfile.TemporaryDirectory(suffix=".volare")
+                for name, link in release_link_list:
+                    tarball_path = os.path.join(tarball_directory.name, name)
+                    r = requests.get(link, stream=True)
+                    with rich.progress.Progress(console=console) as p:
                         task = p.add_task(
-                            f"Downloading pre-built tarball for {version}…",
+                            f"Downloading {name}…",
                             total=int(r.headers["Content-length"]),
                         )
                         r.raise_for_status()
                         with open(tarball_path, "wb") as f:
                             for chunk in r.iter_content(chunk_size=8192):
                                 p.advance(task, advance=len(chunk))
                                 f.write(chunk)
 
-                        task = p.add_task("Unpacking…")
-                        with tarfile.open(tarball_path, mode="r:*") as tf:
-                            p.update(task, total=len(tf.getmembers()))
-                            for i, file in enumerate(tf.getmembers()):
-                                p.update(task, completed=i + 1)
+                    with console.status(f"Unpacking {name}…"):
+                        stream: Any = None
+                        if name.endswith(".tar.zst"):
+                            stream = zstd.open(tarball_path, mode="rb")
+                        else:
+                            try:
+                                import lzma
+
+                                stream = lzma.open(tarball_path, mode="rb")
+                            except ImportError:
+                                raise OSError(
+                                    "Your Python installation does not support xz compression. Either reinstall Python or try a newer PDK version."
+                                )
+                        with tarfile.TarFile(fileobj=stream, mode="r") as tf:
+                            for file in tf:
                                 if file.isdir():
                                     continue
                                 final_path = os.path.join(version_directory, file.name)
                                 final_dir = os.path.dirname(final_path)
                                 mkdirp(final_dir)
                                 io = tf.extractfile(file)
                                 if io is None:
-                                    console.print("[red]Failed to unpack tarball.")
-                                    exit(1)
+                                    raise ValueError(
+                                        f"Failed to unpack tarball for {name}."
+                                    )
                                 with open(final_path, "wb") as f:
                                     f.write(io.read())
+            except Exception as e:
+                shutil.rmtree(version_directory, ignore_errors=True)
+                console.print(f"[red]Error: {e}")
+                exit(-1)
+            except KeyboardInterrupt:
+                console.print("Interrupted.")
+                shutil.rmtree(version_directory, ignore_errors=True)
+                exit(-1)
+
+            for variant in variants:
+                variant_install_path = os.path.join(version_directory, variant)
+                variant_sources_file = os.path.join(variant_install_path, "SOURCES")
+                if not os.path.isfile(variant_sources_file):
+                    with open(variant_sources_file, "w") as f:
+                        print(f"open_pdks {version}", file=f)
 
-                        for variant in variants:
-                            variant_install_path = os.path.join(
-                                version_directory, variant
-                            )
-                            variant_sources_file = os.path.join(
-                                variant_install_path, "SOURCES"
-                            )
-                            if not os.path.isfile(variant_sources_file):
-                                with open(variant_sources_file, "w") as f:
-                                    print(f"open_pdks {version}", file=f)
-
-                        os.unlink(tarball_path)
+            os.unlink(tarball_path)
 
     with console.status(f"Enabling version {version}…"):
         for path in final_paths:
             if os.path.exists(path):
                 if os.path.islink(path):
                     os.unlink(path)
                 else:
@@ -330,28 +364,43 @@
 @click.option(
     "-f",
     "--metadata-file",
     "tool_metadata_file_path",
     default=None,
     help="Explicitly define a tool metadata file instead of searching for a metadata file",
 )
+@click.option(
+    "-l",
+    "--include-libraries",
+    multiple=True,
+    default=None,
+    help="Libraries to include. You can use -l multiple times to include multiple libraries. Pass 'all' to include all of them. A default of 'None' uses a default set for the particular PDK.",
+)
 @click.argument("version", required=False)
-def enable_cmd(pdk_root, pdk, tool_metadata_file_path, version):
+def enable_cmd(pdk_root, pdk, tool_metadata_file_path, version, include_libraries):
     """
     Activates a given installed PDK version.
 
     Parameters: <version> (Optional)
 
     If a version is not given, and you run this in the top level directory of
     tools with a tool_metadata.yml file, for example OpenLane or DFFRAM,
     the appropriate version will be enabled automatically.
     """
+    if include_libraries == ():
+        include_libraries = None
+
     console = Console()
     version = check_version(version, tool_metadata_file_path, console)
-    enable(pdk_root=pdk_root, pdk=pdk, version=version)
+    enable(
+        pdk_root=pdk_root,
+        pdk=pdk,
+        version=version,
+        include_libraries=include_libraries,
+    )
 
 
 @click.command("enable_or_build", hidden=True)
 @opt_pdk_root
 @opt_push
 @opt_build
 @opt("--also-push/--dont-push", default=False, help="Also push.")
@@ -362,15 +411,14 @@
     default=None,
     help="Explicitly define a tool metadata file instead of searching for a metadata file",
 )
 @click.argument("version")
 def enable_or_build_cmd(
     include_libraries,
     jobs,
-    sram,
     pdk_root,
     pdk,
     owner,
     repository,
     token,
     pre,
     clear_build_artifacts,
@@ -382,30 +430,33 @@
 ):
     """
     Attempts to activate a given PDK version. If the version is not found locally or remotely,
     it will instead attempt to build said version.
 
     Parameters: <version>
     """
+    if include_libraries == ():
+        include_libraries = None
+
     console = Console()
     version = check_version(version, tool_metadata_file_path, console)
     enable(
         pdk_root=pdk_root,
         pdk=pdk,
         version=version,
         build_if_not_found=True,
         also_push=also_push,
         build_kwargs={
             "include_libraries": include_libraries,
             "jobs": jobs,
-            "sram": sram,
             "clear_build_artifacts": clear_build_artifacts,
             "use_repo_at": use_repo_at,
             "build_magic": build_magic,
         },
         push_kwargs={
             "owner": owner,
             "repository": repository,
             "token": token,
             "pre": pre,
         },
+        include_libraries=include_libraries,
     )
```

### Comparing `volare-0.7.3/volare/common.py` & `volare-0.8.0/volare/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,22 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import re
 import json
+import shutil
 import pathlib
 from datetime import datetime
 from dataclasses import dataclass
-from typing import Optional, List, Dict, Union
+from typing import Optional, List, Dict, Tuple, Union
 
 import requests
 from rich.console import Console
 
+from .families import Family
+
 # Datetime Helpers
 ISO8601_FMT = "%Y-%m-%dT%H:%M:%SZ"
 
 
 def date_to_iso8601(date: datetime) -> str:
     return date.strftime(ISO8601_FMT)
 
@@ -61,32 +64,96 @@
 class RepoMetadata(object):
     def __init__(self, repo, default_commit, default_branch="main"):
         self.repo = repo
         self.default_commit = default_commit
         self.default_branch = default_branch
 
 
+def _get_current_version(pdk_root: str, pdk: str) -> Optional[str]:
+    current_file = os.path.join(get_volare_dir(pdk_root, pdk), "current")
+    current_file_dir = os.path.dirname(current_file)
+    mkdirp(current_file_dir)
+    version = None
+    try:
+        version = open(current_file).read().strip()
+    except FileNotFoundError:
+        pass
+
+    return version
+
+
 @dataclass
 class Version(object):
     name: str
     pdk: str
     commit_date: Optional[datetime] = None
     upload_date: Optional[datetime] = None
     prerelease: bool = False
-    path: Optional[str] = None
 
     def __lt__(self, rhs: "Version"):
         return (self.commit_date or datetime.min) < (rhs.commit_date or datetime.min)
 
-    def is_current(self, pdk_root: str) -> bool:
-        return self.name == get_current_version(pdk_root, self.pdk)
-
     def __str__(self) -> str:
         return self.name
 
+    def is_installed(self, pdk_root: str) -> bool:
+        version_dir = get_version_dir(pdk_root, self.pdk, self.name)
+        return os.path.isdir(version_dir)
+
+    def is_current(self, pdk_root: str) -> bool:
+        return self.name == _get_current_version(pdk_root, self.pdk)
+
+    def get_dir(self, pdk_root: str) -> str:
+        return get_version_dir(pdk_root, self.pdk, self.name)
+
+    def unset_current(self, pdk_root: str):
+        if not self.is_installed(pdk_root):
+            return
+        if not self.is_current(pdk_root):
+            return
+
+        for variant in Family.by_name[self.pdk].variants:
+            os.unlink(os.path.join(pdk_root, variant))
+
+        current_file = os.path.join(get_volare_dir(pdk_root, self.pdk), "current")
+        os.unlink(current_file)
+
+    def uninstall(self, pdk_root: str):
+        if not self.is_installed(pdk_root):
+            raise ValueError(
+                f"Version {self.name} of the {self.pdk} PDK is not installed."
+            )
+
+        self.unset_current(pdk_root)
+
+        version_dir = self.get_dir(pdk_root)
+
+        shutil.rmtree(version_dir)
+
+    @classmethod
+    def get_current(Self, pdk_root: str, pdk: str) -> Optional["Version"]:
+        current_version = _get_current_version(pdk_root, pdk)
+        if current_version is None:
+            return None
+
+        return Version(current_version, pdk)
+
+    @classmethod
+    def get_all_installed(Self, pdk_root: str, pdk: str) -> List["Version"]:
+        versions_dir = get_versions_dir(pdk_root, pdk)
+        mkdirp(versions_dir)
+        return [
+            Version(
+                name=version,
+                pdk=pdk,
+            )
+            for version in os.listdir(versions_dir)
+            if os.path.isdir(os.path.join(versions_dir, version))
+        ]
+
     @classmethod
     def _from_github(Self) -> Dict[str, List["Version"]]:
         response_str = requests.get(
             f"{VOLARE_REPO_API}/releases", params={"per_page": 100}
         ).content.decode("utf8")
 
         releases = json.loads(response_str)
@@ -196,16 +263,56 @@
     return os.path.join(get_volare_dir(pdk_root, pdk), "versions")
 
 
 def get_version_dir(pdk_root: str, pdk: str, version: Union[str, Version]) -> str:
     return os.path.join(get_versions_dir(pdk_root, pdk), str(version))
 
 
-def get_link_of(version: str, pdk: str) -> str:
-    return f"{VOLARE_REPO_HTTPS}/releases/download/{pdk}-{version}/default.tar.xz"
+def get_link_of(version: str, pdk: str, classic: bool = False) -> str:
+    if classic:
+        return f"{VOLARE_REPO_HTTPS}/releases/download/{pdk}-{version}/default.tar.xz"
+    else:
+        return f"{VOLARE_REPO_HTTPS}/releases/download/{pdk}-{version}/common.tar.zst"
+
+
+def get_release_links(
+    version: str,
+    pdk: str,
+    scl_filter: Optional[List[str]] = None,
+) -> Optional[List[Tuple[str, str]]]:
+    default_filter = False
+    if scl_filter is None:
+        default_filter = True
+        scl_filter = Family.by_name[pdk].default_includes
+
+    release_api_link = f"{VOLARE_REPO_API}/releases/tags/{pdk}-{version}"
+    releases = requests.get(release_api_link, json=True)
+    if releases.status_code >= 400:
+        return None
+    assets = releases.json()["assets"]
+    zst_files = []
+    xz_file = None
+    for asset in assets:
+        if default_filter and asset["name"] == "default.tar.xz":
+            xz_file = (asset["name"], asset["browser_download_url"])
+        elif asset["name"].endswith(".tar.zst"):
+            asset_scl = asset["name"][:-8]
+            if asset_scl == "common" or "all" in scl_filter or asset_scl in scl_filter:
+                zst_files.append((asset["name"], asset["browser_download_url"]))
+
+    if len(zst_files):
+        return zst_files
+    if xz_file is not None:
+        return [xz_file]
+    if scl_filter is not None:
+        raise ValueError(f"No files found for standard cell libraries: {scl_filter}.")
+
+    raise Exception(
+        f"The release for {pdk}-{version} is malformed. Please file a bug report."
+    )
 
 
 def get_logs_dir() -> str:
     if os.getenv("VOLARE_LOGS") is not None:
         return os.environ["VOLARE_LOGS"]
     else:
         return os.path.join(VOLARE_RESOLVED_HOME, "volare", "logs")
@@ -224,30 +331,12 @@
     response = json.loads(response_str)
     date = response["commit"]["author"]["date"]
     commit_date = datetime.strptime(date, "%Y-%m-%dT%H:%M:%SZ")
     return commit_date
 
 
 def get_installed_list(pdk_root: str, pdk: str) -> List[Version]:
-    versions_dir = get_versions_dir(pdk_root, pdk)
-    mkdirp(versions_dir)
-    return [
-        Version(
-            name=version,
-            pdk=pdk,
-            path=os.path.join(versions_dir, version),
-        )
-        for version in os.listdir(versions_dir)
-    ]
-
+    return Version.get_all_installed(pdk_root, pdk)
 
-def get_current_version(pdk_root: str, pdk: str) -> str:
-    current_file = os.path.join(get_volare_dir(pdk_root, pdk), "current")
-    current_file_dir = os.path.dirname(current_file)
-    mkdirp(current_file_dir)
-    version = ""
-    try:
-        version = open(current_file).read().strip()
-    except FileNotFoundError:
-        pass
 
-    return version
+def get_current_version(pdk_root: str, pdk: str) -> Optional[str]:
+    return _get_current_version(pdk_root, pdk)
```

### Comparing `volare-0.7.3/volare/click_common.py` & `volare-0.8.0/volare/click_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,28 @@
 
 def opt_build(function: Callable):
     function = opt(
         "-l",
         "--include-libraries",
         multiple=True,
         default=None,
-        help="Libraries to include in the build. You can use -l multiple times to include multiple libraries. Pass 'all' to include all of them. A default of 'None' uses a default set for the particular PDK.",
+        help="Libraries to include. You can use -l multiple times to include multiple libraries. Pass 'all' to include all of them. A default of 'None' uses a default set for the particular PDK.",
     )(function)
     function = opt(
         "-j",
         "--jobs",
         default=1,
         help="Specifies the number of commands to run simultaneously.",
     )(function)
-    function = opt("--sram/--no-sram", default=True, help="Enable or disable sram")(
-        function
-    )
+    function = opt(
+        "--sram/--no-sram",
+        default=True,
+        hidden=True,
+        expose_value=False,
+    )(function)
     function = opt(
         "--clear-build-artifacts/--keep-build-artifacts",
         default=False,
         help="Whether or not to remove the build artifacts. Keeping the build artifacts is useful when testing.",
     )(function)
     function = opt(
         "-r",
```

### Comparing `volare-0.7.3/volare/__main__.py` & `volare-0.8.0/volare/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import click
 
 from . import __version__
 from .build import build_cmd, push_cmd
 from .manage import (
     output_cmd,
     prune_cmd,
+    rm_cmd,
     path_cmd,
     list_cmd,
     list_remote_cmd,
     enable_cmd,
     enable_or_build_cmd,
 )
 
@@ -31,24 +32,24 @@
 @click.version_option(__version__)
 def cli():
     pass
 
 
 cli.add_command(output_cmd)
 cli.add_command(prune_cmd)
+cli.add_command(rm_cmd)
 cli.add_command(build_cmd)
 cli.add_command(push_cmd)
 cli.add_command(path_cmd)
 cli.add_command(list_cmd)
 cli.add_command(list_remote_cmd)
 cli.add_command(enable_cmd)
 cli.add_command(enable_or_build_cmd)
 
 try:
-    import lzma  # noqa: F401
     import ssl  # noqa: F401
 except ModuleNotFoundError as e:
     print(
         f"Your version of Python 3 was not built with a required module: '{e.name}'",
         file=sys.stderr,
     )
     print(
```

### Comparing `volare-0.7.3/volare/__init__.py` & `volare-0.8.0/volare/__init__.py`

 * *Files identical despite different names*

