# Comparing `tmp/releasecmd-0.8.1.tar.gz` & `tmp/releasecmd-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "releasecmd-0.8.1.tar", last modified: Fri Feb 24 23:50:38 2023, max compression
+gzip compressed data, was "releasecmd-0.9.0.tar", last modified: Sun Jun  4 15:34:18 2023, max compression
```

## Comparing `releasecmd-0.8.1.tar` & `releasecmd-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-24 23:50:38.687694 releasecmd-0.8.1/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:13.000000 releasecmd-0.8.1/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      138 2021-03-20 04:14:13.000000 releasecmd-0.8.1/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     5543 2023-02-24 23:50:38.687694 releasecmd-0.8.1/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     4020 2023-02-24 23:42:57.000000 releasecmd-0.8.1/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)      696 2023-02-24 23:44:43.000000 releasecmd-0.8.1/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-24 23:50:38.687694 releasecmd-0.8.1/releasecmd/
--rw-r--r--   0 toor      (1000) toor      (1000)     9009 2023-02-24 00:19:16.000000 releasecmd-0.8.1/releasecmd/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-02-24 23:49:41.000000 releasecmd-0.8.1/releasecmd/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      971 2021-10-17 04:49:22.000000 releasecmd-0.8.1/releasecmd/_retry.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-24 23:50:38.687694 releasecmd-0.8.1/releasecmd.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     5543 2023-02-24 23:50:38.000000 releasecmd-0.8.1/releasecmd.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      293 2023-02-24 23:50:38.000000 releasecmd-0.8.1/releasecmd.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-02-24 23:50:38.000000 releasecmd-0.8.1/releasecmd.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        6 2023-02-24 23:50:38.000000 releasecmd-0.8.1/releasecmd.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       11 2023-02-24 23:50:38.000000 releasecmd-0.8.1/releasecmd.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-02-24 23:50:38.687694 releasecmd-0.8.1/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2454 2023-02-24 23:47:59.000000 releasecmd-0.8.1/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 15:34:18.889412 releasecmd-0.9.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:13.000000 releasecmd-0.9.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      138 2021-03-20 04:14:13.000000 releasecmd-0.9.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     5596 2023-06-04 15:34:18.889412 releasecmd-0.9.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     4073 2023-06-04 15:08:43.000000 releasecmd-0.9.0/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)      733 2023-06-04 06:59:24.000000 releasecmd-0.9.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 15:34:18.889412 releasecmd-0.9.0/releasecmd/
+-rw-r--r--   0 toor      (1000) toor      (1000)     9562 2023-06-04 15:19:45.000000 releasecmd-0.9.0/releasecmd/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-04 15:22:32.000000 releasecmd-0.9.0/releasecmd/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      971 2021-10-17 04:49:22.000000 releasecmd-0.9.0/releasecmd/_retry.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 15:34:18.889412 releasecmd-0.9.0/releasecmd.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5596 2023-06-04 15:34:18.000000 releasecmd-0.9.0/releasecmd.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      293 2023-06-04 15:34:18.000000 releasecmd-0.9.0/releasecmd.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-04 15:34:18.000000 releasecmd-0.9.0/releasecmd.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        6 2023-06-04 15:34:18.000000 releasecmd-0.9.0/releasecmd.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       11 2023-06-04 15:34:18.000000 releasecmd-0.9.0/releasecmd.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-04 15:34:18.889412 releasecmd-0.9.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2454 2023-06-04 14:53:15.000000 releasecmd-0.9.0/setup.py
```

### Comparing `releasecmd-0.8.1/LICENSE` & `releasecmd-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `releasecmd-0.8.1/PKG-INFO` & `releasecmd-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: releasecmd
-Version: 0.8.1
+Version: 0.9.0
 Summary: releasecmd is a release subcommand for setup.py (setuptools.setup). the subcommand create a git tag and push, and upload packages to PyPI.
 Home-page: https://github.com/thombashi/releasecmd
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Changlog, https://github.com/thombashi/releasecmd/releases
 Project-URL: Source, https://github.com/thombashi/releasecmd
@@ -148,21 +148,22 @@
 
 
 release command options
 ============================================
 ::
 
     Options for 'ReleaseCommand' command:
-        --skip-tagging    skip a git tag creation
-        --skip-uploading  skip uploading packages to PyPI
-        --dry-run         do no harm
-        --sign            make a GPG-signed tag
-        --search-dir      specify a root directory path to search a version file.
+      --skip-tagging    skip a git tag creation
+      --skip-uploading  skip uploading packages to PyPI
+      --dry-run         do no harm
+      --sign            [deprecated from PyPI] make a GPG-signed tag
+      --verbose         show verbose output
+      --search-dir      specify a root directory path to search a version file.
                         defaults to the current directory.
-        --tag-template    specify git tag format. defaults to 'v{version}'.
-        --version         specify version manually
+      --tag-template    specify git tag format. defaults to 'v{version}'.
+      --version         specify version manually
 
 
 Dependencies
 ============================================
 - Python 3.7+
 - `Git <https://git-scm.com/>`__
```

### Comparing `releasecmd-0.8.1/README.rst` & `releasecmd-0.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -115,21 +115,22 @@
 
 
 release command options
 ============================================
 ::
 
     Options for 'ReleaseCommand' command:
-        --skip-tagging    skip a git tag creation
-        --skip-uploading  skip uploading packages to PyPI
-        --dry-run         do no harm
-        --sign            make a GPG-signed tag
-        --search-dir      specify a root directory path to search a version file.
+      --skip-tagging    skip a git tag creation
+      --skip-uploading  skip uploading packages to PyPI
+      --dry-run         do no harm
+      --sign            [deprecated from PyPI] make a GPG-signed tag
+      --verbose         show verbose output
+      --search-dir      specify a root directory path to search a version file.
                         defaults to the current directory.
-        --tag-template    specify git tag format. defaults to 'v{version}'.
-        --version         specify version manually
+      --tag-template    specify git tag format. defaults to 'v{version}'.
+      --version         specify version manually
 
 
 Dependencies
 ============================================
 - Python 3.7+
 - `Git <https://git-scm.com/>`__
```

### Comparing `releasecmd-0.8.1/pyproject.toml` & `releasecmd-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
```

### Comparing `releasecmd-0.8.1/releasecmd/__init__.py` & `releasecmd-0.9.0/releasecmd/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 import errno
 import os
 import re
 import subprocess
 import sys
+import warnings
 from typing import Dict, Generator, List, Optional
 
 import setuptools
 
 from .__version__ import __author__, __copyright__, __email__, __license__, __version__
 from ._retry import Retry, sleep_before_retry
 
@@ -29,15 +30,16 @@
     description = "create a Git tag and push, and then upload packages to PyPI"
 
     # command class must provide 'user_options' attribute (a list of tuples)
     user_options = [
         ("skip-tagging", None, "skip a git tag creation"),
         ("skip-uploading", None, "skip uploading packages to PyPI"),
         ("dry-run", None, "do no harm"),
-        ("sign", None, "make a GPG-signed tag"),
+        ("sign", None, "[deprecated from PyPI] make a GPG-signed tag"),
+        ("verbose", None, "show verbose output"),
         (
             "search-dir=",
             None,
             "specify a root directory path to search a version file. "
             "defaults to the current directory.",
         ),
         ("tag-template=", None, "specify git tag format. defaults to 'v{version}'."),
@@ -48,14 +50,15 @@
     __TAG_ALREADY_EXISTS = 128
 
     def initialize_options(self) -> None:
         self.skip_tagging = False
         self.skip_uploading = False
         self.dry_run = False
         self.sign = False
+        self.verbose = False
         self.search_dir = "."
         self.tag_template = "v{version}"
         self.version: Optional[str] = None
 
     def finalize_options(self) -> None:
         pass
 
@@ -151,14 +154,17 @@
     ) -> subprocess.CompletedProcess:
         command_str = " ".join(command)
 
         if self.dry_run:
             print(f"dry run: {command_str}")
             return subprocess.CompletedProcess(args=[], returncode=0, stdout="", stderr="")
 
+        if self.verbose:
+            print(f"execute: {command_str}")
+
         result = subprocess.run(command, stderr=subprocess.PIPE, encoding="utf8")
         returncode = result.returncode
         if returncode == 0 or (retry and returncode in retry.no_retry_returncodes):
             return result
 
         if retry is None:
             self.__print_error(command_str, error_msg=result.stderr)
@@ -187,20 +193,24 @@
         print("[check existing git tags]")
         TAG_NOT_FOUND = 2
         result = self.__call(
             ["git", "ls-remote", "--exit-code", "origin", f"refs/tags/{tag}"],
             retry=Retry(no_retry_returncodes=[TAG_NOT_FOUND]),
         )
         if result.returncode == 0:
-            print("[ERROR] {} tag already exists", file=sys.stderr)
+            print(f"[ERROR] {tag} tag already exists", file=sys.stderr)
             sys.exit(1)
 
         command_items: List[str] = ["git", "tag"]
         extra_log = ""
         if self.sign:
+            warnings.warn(
+                "support for GPG signatures has been removed from PyPI", DeprecationWarning
+            )
+
             command_items.extend(["--sign", "-m", f"'GPG signed {version} tag'"])
             extra_log = " with gpg signing"
         command_items.append(tag)
         print(f"[create a git tag{extra_log}: {tag}]")
         self.__call(command_items)
 
         print("[push git tags]")
@@ -212,15 +222,18 @@
         version_regexp = re.compile(rf".+-{re.escape(version):s}.*(\.tar\.gz|\.whl)(\.asc$)?")
         upload_file_list: List[str] = []
 
         for filename in os.listdir(self.__DIST_DIR_NAME):
             if not version_regexp.search(filename):
                 continue
 
-            upload_file_list.append(os.path.join(self.__DIST_DIR_NAME, filename))
+            upload_filepath = os.path.join(self.__DIST_DIR_NAME, filename)
+            if self.verbose:
+                print(f"found a file: {os.path.abspath(upload_filepath)}")
+            upload_file_list.append(upload_filepath)
 
         return upload_file_list
 
     def __sign_package(self, version: str) -> None:
         if not self.sign:
             return
 
@@ -238,15 +251,18 @@
 
     def __upload_package(self, upload_file_list: List[str]) -> None:
         if self.skip_uploading:
             print("skip uploading packages")
             return
 
         print("[upload packages to PyPI]")
-        self.__call(["twine", "upload"] + upload_file_list, retry=Retry())
+        cmd = ["twine", "upload"]
+        if self.verbose:
+            cmd += ["--verbose"]
+        self.__call(cmd + upload_file_list, retry=Retry())
 
     def __traverse_version_file(self) -> Generator[Optional[str], None, None]:
         regexp_exclude_dirs = re.compile(
             "|".join(
                 [
                     "/build/.+",
                     re.escape("/.eggs/"),
```

### Comparing `releasecmd-0.8.1/releasecmd/_retry.py` & `releasecmd-0.9.0/releasecmd/_retry.py`

 * *Files identical despite different names*

### Comparing `releasecmd-0.8.1/releasecmd.egg-info/PKG-INFO` & `releasecmd-0.9.0/releasecmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: releasecmd
-Version: 0.8.1
+Version: 0.9.0
 Summary: releasecmd is a release subcommand for setup.py (setuptools.setup). the subcommand create a git tag and push, and upload packages to PyPI.
 Home-page: https://github.com/thombashi/releasecmd
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Changlog, https://github.com/thombashi/releasecmd/releases
 Project-URL: Source, https://github.com/thombashi/releasecmd
@@ -148,21 +148,22 @@
 
 
 release command options
 ============================================
 ::
 
     Options for 'ReleaseCommand' command:
-        --skip-tagging    skip a git tag creation
-        --skip-uploading  skip uploading packages to PyPI
-        --dry-run         do no harm
-        --sign            make a GPG-signed tag
-        --search-dir      specify a root directory path to search a version file.
+      --skip-tagging    skip a git tag creation
+      --skip-uploading  skip uploading packages to PyPI
+      --dry-run         do no harm
+      --sign            [deprecated from PyPI] make a GPG-signed tag
+      --verbose         show verbose output
+      --search-dir      specify a root directory path to search a version file.
                         defaults to the current directory.
-        --tag-template    specify git tag format. defaults to 'v{version}'.
-        --version         specify version manually
+      --tag-template    specify git tag format. defaults to 'v{version}'.
+      --version         specify version manually
 
 
 Dependencies
 ============================================
 - Python 3.7+
 - `Git <https://git-scm.com/>`__
```

### Comparing `releasecmd-0.8.1/setup.py` & `releasecmd-0.9.0/setup.py`

 * *Files identical despite different names*

