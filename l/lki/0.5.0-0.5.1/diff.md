# Comparing `tmp/lki-0.5.0.tar.gz` & `tmp/lki-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lki-0.5.0.tar", last modified: Thu Jul 14 12:04:15 2022, max compression
+gzip compressed data, was "lki-0.5.1.tar", last modified: Sun Jun  4 07:11:44 2023, max compression
```

## Comparing `lki-0.5.0.tar` & `lki-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 12:04:15.423549 lki-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-07-14 12:03:57.000000 lki-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4113 2022-07-14 12:04:15.423549 lki-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-07-14 12:03:57.000000 lki-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 12:04:15.423549 lki-0.5.0/lki/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-14 12:03:57.000000 lki-0.5.0/lki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5515 2022-07-14 12:03:57.000000 lki-0.5.0/lki/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-07-14 12:03:57.000000 lki-0.5.0/lki/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-07-14 12:03:57.000000 lki-0.5.0/lki/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-07-14 12:03:57.000000 lki-0.5.0/lki/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 12:04:15.423549 lki-0.5.0/lki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4113 2022-07-14 12:04:14.000000 lki-0.5.0/lki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-07-14 12:04:15.000000 lki-0.5.0/lki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 12:04:14.000000 lki-0.5.0/lki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-07-14 12:04:15.000000 lki-0.5.0/lki.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-14 12:04:15.000000 lki-0.5.0/lki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-07-14 12:04:15.000000 lki-0.5.0/lki.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-07-14 12:04:15.423549 lki-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-07-14 12:03:57.000000 lki-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:11:44.327741 lki-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-04 07:11:02.000000 lki-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-04 07:11:44.327741 lki-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-04 07:11:02.000000 lki-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:11:44.327741 lki-0.5.1/lki/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-04 07:11:02.000000 lki-0.5.1/lki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-04 07:11:02.000000 lki-0.5.1/lki/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-04 07:11:02.000000 lki-0.5.1/lki/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-04 07:11:02.000000 lki-0.5.1/lki/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-04 07:11:02.000000 lki-0.5.1/lki/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:11:44.327741 lki-0.5.1/lki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-04 07:11:44.000000 lki-0.5.1/lki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-04 07:11:44.000000 lki-0.5.1/lki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 07:11:44.000000 lki-0.5.1/lki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-04 07:11:44.000000 lki-0.5.1/lki.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 07:11:44.000000 lki-0.5.1/lki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-04 07:11:44.000000 lki-0.5.1/lki.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-04 07:11:44.327741 lki-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-04 07:11:02.000000 lki-0.5.1/setup.py
```

### Comparing `lki-0.5.0/LICENSE` & `lki-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lki-0.5.0/PKG-INFO` & `lki-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lki
-Version: 0.5.0
+Version: 0.5.1
 Summary: connect Lirian's useful commands
 Home-page: https://github.com/LKI/LKI
 Author: Lirian Su
 Author-email: liriansu@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `lki-0.5.0/README.md` & `lki-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lki-0.5.0/lki/cmdline.py` & `lki-0.5.1/lki/cmdline.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         _link(".ideavimrc")
         _link(".inputrc")
         _link(".profile")
         _link(".tmux.conf")
         if is_windows:
             _link(
                 ".windows-terminal.json",
-                "~/AppData/Local/Packages/Microsoft.WindowsTerminal_8wekyb3d8bbwe/LocalState/settings.json",
+                "AppData/Local/Packages/Microsoft.WindowsTerminal_8wekyb3d8bbwe/LocalState/settings.json",
             )
         # TODO: implement `lki install --vim`
         # _link("dotvim/vimrc", ".vimrc")
         #
         # if IS_WIN32:
         #     _link("dotvim/vimrc", "_vimrc")
         #     _link("dotvim", "vimfiles", target_is_directory=True)
```

### Comparing `lki-0.5.0/lki/config.py` & `lki-0.5.1/lki/config.py`

 * *Files identical despite different names*

### Comparing `lki-0.5.0/lki/utils.py` & `lki-0.5.1/lki/utils.py`

 * *Files identical despite different names*

### Comparing `lki-0.5.0/lki.egg-info/PKG-INFO` & `lki-0.5.1/lki.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lki
-Version: 0.5.0
+Version: 0.5.1
 Summary: connect Lirian's useful commands
 Home-page: https://github.com/LKI/LKI
 Author: Lirian Su
 Author-email: liriansu@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `lki-0.5.0/setup.cfg` & `lki-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [bumpversion]
 commit = True
-current_version = 0.5.0
+current_version = 0.5.1
 message = release: {current_version} -> {new_version}
 tag = True
 
 [bumpversion:file:lki/__init__.py]
 
 [aliases]
 release = sdist bdist_wheel
```

### Comparing `lki-0.5.0/setup.py` & `lki-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from pipenv.utils.dependencies import convert_deps_to_pip
 
 import lki
 
 with io.open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
+install_requires: list[str] = convert_deps_to_pip(Project(chdir=False).parsed_pipfile["packages"])
+
 setuptools.setup(
     name="lki",
     version=lki.__version__,
     description="connect Lirian's useful commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Lirian Su",
     author_email="liriansu@gmail.com",
     url="https://github.com/LKI/LKI",
     license="MIT License",
-    install_requires=convert_deps_to_pip(Project(chdir=False).parsed_pipfile["packages"], r=False),
+    install_requires=install_requires,
     packages=setuptools.find_packages(),
     entry_points={"console_scripts": "lki = lki.cmdline:entry"},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
```

