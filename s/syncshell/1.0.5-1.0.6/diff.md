# Comparing `tmp/syncshell-1.0.5.tar.gz` & `tmp/syncshell-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncshell-1.0.5.tar", max compression
+gzip compressed data, was "syncshell-1.0.6.tar", max compression
```

## Comparing `syncshell-1.0.5.tar` & `syncshell-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1072 2022-06-16 10:22:30.000000 syncshell-1.0.5/LICENSE.txt
--rw-r--r--   0        0        0     3998 2022-07-27 09:12:57.117690 syncshell-1.0.5/README.md
--rw-r--r--   0        0        0      693 2022-07-27 09:20:40.508989 syncshell-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-18 15:23:24.855682 syncshell-1.0.5/syncshell/__init__.py
--rw-r--r--   0        0        0      158 2022-06-23 08:51:02.379245 syncshell-1.0.5/syncshell/__main__.py
--rw-r--r--   0        0        0     6625 2022-07-26 19:34:34.299826 syncshell-1.0.5/syncshell/cli.py
--rw-r--r--   0        0        0     2606 2022-07-27 08:23:49.381176 syncshell-1.0.5/syncshell/config.py
--rw-r--r--   0        0        0        0 2022-06-23 08:51:02.381314 syncshell-1.0.5/syncshell/utils/__init__.py
--rw-r--r--   0        0        0      964 2022-07-27 08:15:14.248748 syncshell-1.0.5/syncshell/utils/constants.py
--rw-r--r--   0        0        0      567 2022-06-23 08:51:02.382500 syncshell-1.0.5/syncshell/utils/spinner.py
--rw-r--r--   0        0        0     4928 2022-07-27 09:28:17.377110 syncshell-1.0.5/setup.py
--rw-r--r--   0        0        0     4891 2022-07-27 09:28:17.377454 syncshell-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-06-16 10:22:30.000000 syncshell-1.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     3702 2023-04-22 13:57:36.633541 syncshell-1.0.6/README.md
+-rw-r--r--   0        0        0      746 2023-06-04 21:42:58.091907 syncshell-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-18 15:23:24.855682 syncshell-1.0.6/syncshell/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-20 23:42:21.663528 syncshell-1.0.6/syncshell/__main__.py
+-rw-r--r--   0        0        0     7316 2023-06-04 21:32:02.267513 syncshell-1.0.6/syncshell/cli.py
+-rw-r--r--   0        0        0     2268 2023-06-04 21:32:02.269075 syncshell-1.0.6/syncshell/config.py
+-rw-r--r--   0        0        0        0 2022-06-23 08:51:02.381314 syncshell-1.0.6/syncshell/utils/__init__.py
+-rw-r--r--   0        0        0      964 2022-07-27 08:15:14.248748 syncshell-1.0.6/syncshell/utils/constants.py
+-rw-r--r--   0        0        0      567 2022-06-23 08:51:02.382500 syncshell-1.0.6/syncshell/utils/spinner.py
+-rw-r--r--   0        0        0     4596 1970-01-01 00:00:00.000000 syncshell-1.0.6/PKG-INFO
```

### Comparing `syncshell-1.0.5/LICENSE.txt` & `syncshell-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `syncshell-1.0.5/README.md` & `syncshell-1.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,93 @@
-<h1 align="center">SyncShell</h1>
+# SyncShell
+<!-- License -->
+<a href="https://mit-license.org/msudgh">
+  <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"
+    alt="MIT License" />
+</a>
+<!-- Build Status -->
+<a href="https://github.com/msudgh/syncshell/actions/workflows/test.yaml">
+  <img src="https://github.com/msudgh/syncshell/actions/workflows/test.yaml/badge.svg?branch=main"
+    alt="Build Status" />
+</a>
+<!-- Releases -->
+<a href="https://github.com/msudgh/syncshell/releases">
+  <img src="https://img.shields.io/github/release/msudgh/syncshell.svg"
+    alt="PyPi" />
+</a>
+<!-- PyPi -->
+<a href="https://pypi.org/project/syncshell/">
+  <img src="https://img.shields.io/pypi/v/syncshell.svg"
+    alt="PyPi" />
+</a>
+
+SyncShell as a simple and secure tool allows to synchronize machine's shell history across devices. It's built on top of Github Gist and written in Python (CLI). With SyncShell, you no longer have to worry about manually syncing your office and home machine's shell history and let continue where the terminal session left.
+
+## Features
+
+- Sync your shell history across all your devices
+- Securely store your shell history on Github Gist
+- Support for `zsh` and `bash` shells
+- Easy to install and use
 
-<div align="center">
-  <strong>Yet another tool for laziness</strong>
-</div>
-<div align="center">
-  Keep your machine's shell history synchronized
-</div>
-<br/>
-<div align="center">
-  <!-- Build Status -->
-  <a href="https://github.com/msudgh/syncshell/actions/workflows/test.yaml">
-    <img src="https://github.com/msudgh/syncshell/actions/workflows/test.yaml/badge.svg?branch=main"
-      alt="Build Status" />
-  </a>
-  <!-- License -->
-  <a href="https://mit-license.org/msudgh">
-    <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"
-      alt="MIT License" />
-  </a>
-  <!-- Release -->
-  <a href="https://github.com/msudgh/syncshell/releases">
-    <img src="https://img.shields.io/github/release/msudgh/syncshell.svg"
-      alt="PyPi" />
-  </a>
-  <!-- PyPi -->
-  <a href="https://pypi.org/project/syncshell/">
-    <img src="https://img.shields.io/pypi/v/syncshell.svg"
-      alt="PyPi" />
-  </a>
-</div>
-<br/>
+## Installation
+To install SyncShell, simply run the following command:
 
-## Get SyncShell
-Currently, `SyncShell` is just available on `PyPi` and by the following command install the latest version:
 ```bash
-$ pip install syncshell # Maybe sudo need
-```
-```bash
-$ syncshell -- --help
-Type:        Application
-String form: <syncshell.cli.Application object at 0x1035f51c0>
-Docstring:   SyncShell CLI Application
-
-Usage:       syncshell 
-             syncshell auth
-             syncshell download
-             syncshell upload
+$ pip install syncshell
 ```
 
-## How it Works
-The actual idea of SyncShell is synchronization of your all device's shell history, it means you don't need to have concerns when you want to sync your office and home machine's shell history. Application integrated and built on top of Github Gist, and written in Python (CLI).
-
-According to Github API, you can generate a token key with `gist` scope to access to Gist. 
-Gists have two **`public`**, **`secret`** type which syncshell while executing `syncshell upload` command will upload your history file and store them on Github Gist securely (**private**).
-
-On the others machine, by executing `syncshell download` after entering your token key and created Gist ID you can download the gist and sync your shell's history.
-
-  > Gists will be secret until you don't share it with someone else, In other words, It'll be secret and safe until you only have the Github Token and Gist ID.
-
 ## Usage
-  > Currently, `SyncShell` just support `zsh` and supporting other shells is in WIP.
+To use SyncShell, It first needs to set up a Github token key by following these steps:
 
-Before SyncShell can be useful you need to setup your Github token key:
+1. Open [**Github personal access tokens**](https://github.com/settings/tokens) page, [**Generate a new token**](https://github.com/settings/tokens/new) with `gist` scope feature.
+2. Execute the **`syncshell auth`** command, Enter the token key to validate and confirm it.
 
-  1. Open [**Github personal access tokens**](https://github.com/settings/tokens) page, [**Generate a new token**](https://github.com/settings/tokens/new) with `gist` scope feature.
-  2. Execute the **`syncshell auth`** command, Enter your token key to validate and confirm it.
-  3. Done :wink:
-
-Now you can try to upload your shell history by the following command:
+Once finished, try to upload shell history by the following command:
 
 ```bash
 $ syncshell upload
 ```
 
-After the uploading process, you'll take a Gist ID that by this ID and your Github token, you can download history on the others machine by executing the following command:
+After uploading, the download command lets to sync and pull changes on the other machines:
+
 ```bash
 $ syncshell download
 ```
 
-## Todo
-- [ ] Write more test cases
-- [x] Support `zsh`, `bash`
-
-## Contributing
-So nice you wanna contribute to this repository. Thank you. You may contribute in several ways consists of:
 
-* Creating new features
-* Fixing bugs
+### Synopsis
 
-#### Installing dependencies
-[Poetry Installation](https://python-poetry.org/docs/#installation) is straightforward walkthough to setup a versatile package manager.
-
-By the following command install syncshell dependencies
 ```bash
-# Clone syncshell repository
-$ git clone git@github.com:msudgh/syncshell.git
-$ cd syncshell
-$ poetry install
-```
+$ syncshell
+Type:        Application
+String form: <syncshell.cli.Application object at 0x101b1ff10>
+Docstring:   SyncShell CLI Application
 
-#### Tests
-Before submiting your PR, Execute the below command to be sure about passing test cases.
-```bash
-$ poetry run pytest -c pytest.ini -s
+Usage:       syncshell 
+             syncshell auth
+             syncshell download
+             syncshell upload
 ```
 
-Done :wink:
+## How it Works
+
+SyncShell is a tool that synchronizes shell history across all devices by securely storing the history file on Github Gist. Github Gist provides two types of Gists, `public` and `secret`. When the `syncshell upload` command is executed, the shell history file is uploaded and stored securely on Github Gist as a secret Gist. To download the uploaded shell history on other devices, the `syncshell download` command is used. This command retrieves the previously uploaded Gist, allowing the user to access their shell history on any device.
+
+**Security:** A Gist will be secret until it's not shared and will be secret and safe until you only have the Github Token and Gist ID.
+
+**Privacy:** In case of having password or secret in a history file, Its suggested to first have a alignment with privacy policies for any usecase.
+
+## Contributing
+Appreciate the contribution to this repository.
+
+To contribute, you need to follow the below steps for suggesting a change or a new feature:
+
+1. Install [poetry](https://python-poetry.org/docs/#installation) as a dependency manager
+2. Install dependencies by running ```poetry install```
+3. Make your changes
+4. Run and debug your changes by running ```poetry run python syncshell```
+5. Run tests by running ```poetry run pytest -c pytest.ini -s```
+6. Submit a pull request
 
 ## License
 The code is licensed under the MIT License. See the data's [LICENSE](https://github.com/msudgh/syncshell/blob/main/LICENSE) file for more information.
```

#### html2text {}

```diff
@@ -1,45 +1,40 @@
-                            ****** SyncShell ******
-                         Yet another tool for laziness
-                Keep your machine's shell history synchronized
-
-                 [Build_Status]  [MIT_License]  [PyPi]  [PyPi]
-
-## Get SyncShell Currently, `SyncShell` is just available on `PyPi` and by the
-following command install the latest version: ```bash $ pip install syncshell #
-Maybe sudo need ``` ```bash $ syncshell -- --help Type: Application String
-form:
-cli.Application object at 0x1035f51c0> Docstring: SyncShell CLI Application
+# SyncShell  [MIT_License]  [Build_Status]  [PyPi]  [PyPi] SyncShell as a
+simple and secure tool allows to synchronize machine's shell history across
+devices. It's built on top of Github Gist and written in Python (CLI). With
+SyncShell, you no longer have to worry about manually syncing your office and
+home machine's shell history and let continue where the terminal session left.
+## Features - Sync your shell history across all your devices - Securely store
+your shell history on Github Gist - Support for `zsh` and `bash` shells - Easy
+to install and use ## Installation To install SyncShell, simply run the
+following command: ```bash $ pip install syncshell ``` ## Usage To use
+SyncShell, It first needs to set up a Github token key by following these
+steps: 1. Open [**Github personal access tokens**](https://github.com/settings/
+tokens) page, [**Generate a new token**](https://github.com/settings/tokens/
+new) with `gist` scope feature. 2. Execute the **`syncshell auth`** command,
+Enter the token key to validate and confirm it. Once finished, try to upload
+shell history by the following command: ```bash $ syncshell upload ``` After
+uploading, the download command lets to sync and pull changes on the other
+machines: ```bash $ syncshell download ``` ### Synopsis ```bash $ syncshell
+Type: Application String form:
+cli.Application object at 0x101b1ff10> Docstring: SyncShell CLI Application
 Usage: syncshell syncshell auth syncshell download syncshell upload ``` ## How
-it Works The actual idea of SyncShell is synchronization of your all device's
-shell history, it means you don't need to have concerns when you want to sync
-your office and home machine's shell history. Application integrated and built
-on top of Github Gist, and written in Python (CLI). According to Github API,
-you can generate a token key with `gist` scope to access to Gist. Gists have
-two **`public`**, **`secret`** type which syncshell while executing `syncshell
-upload` command will upload your history file and store them on Github Gist
-securely (**private**). On the others machine, by executing `syncshell
-download` after entering your token key and created Gist ID you can download
-the gist and sync your shell's history. > Gists will be secret until you don't
-share it with someone else, In other words, It'll be secret and safe until you
-only have the Github Token and Gist ID. ## Usage > Currently, `SyncShell` just
-support `zsh` and supporting other shells is in WIP. Before SyncShell can be
-useful you need to setup your Github token key: 1. Open [**Github personal
-access tokens**](https://github.com/settings/tokens) page, [**Generate a new
-token**](https://github.com/settings/tokens/new) with `gist` scope feature. 2.
-Execute the **`syncshell auth`** command, Enter your token key to validate and
-confirm it. 3. Done :wink: Now you can try to upload your shell history by the
-following command: ```bash $ syncshell upload ``` After the uploading process,
-you'll take a Gist ID that by this ID and your Github token, you can download
-history on the others machine by executing the following command: ```bash $
-syncshell download ``` ## Todo - [ ] Write more test cases - [x] Support `zsh`,
-`bash` ## Contributing So nice you wanna contribute to this repository. Thank
-you. You may contribute in several ways consists of: * Creating new features *
-Fixing bugs #### Installing dependencies [Poetry Installation](https://python-
-poetry.org/docs/#installation) is straightforward walkthough to setup a
-versatile package manager. By the following command install syncshell
-dependencies ```bash # Clone syncshell repository $ git clone git@github.com:
-msudgh/syncshell.git $ cd syncshell $ poetry install ``` #### Tests Before
-submiting your PR, Execute the below command to be sure about passing test
-cases. ```bash $ poetry run pytest -c pytest.ini -s ``` Done :wink: ## License
-The code is licensed under the MIT License. See the data's [LICENSE](https://
-github.com/msudgh/syncshell/blob/main/LICENSE) file for more information.
+it Works SyncShell is a tool that synchronizes shell history across all devices
+by securely storing the history file on Github Gist. Github Gist provides two
+types of Gists, `public` and `secret`. When the `syncshell upload` command is
+executed, the shell history file is uploaded and stored securely on Github Gist
+as a secret Gist. To download the uploaded shell history on other devices, the
+`syncshell download` command is used. This command retrieves the previously
+uploaded Gist, allowing the user to access their shell history on any device.
+**Security:** A Gist will be secret until it's not shared and will be secret
+and safe until you only have the Github Token and Gist ID. **Privacy:** In case
+of having password or secret in a history file, Its suggested to first have a
+alignment with privacy policies for any usecase. ## Contributing Appreciate the
+contribution to this repository. To contribute, you need to follow the below
+steps for suggesting a change or a new feature: 1. Install [poetry](https://
+python-poetry.org/docs/#installation) as a dependency manager 2. Install
+dependencies by running ```poetry install``` 3. Make your changes 4. Run and
+debug your changes by running ```poetry run python syncshell``` 5. Run tests by
+running ```poetry run pytest -c pytest.ini -s``` 6. Submit a pull request ##
+License The code is licensed under the MIT License. See the data's [LICENSE]
+(https://github.com/msudgh/syncshell/blob/main/LICENSE) file for more
+information.
```

### Comparing `syncshell-1.0.5/pyproject.toml` & `syncshell-1.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 [tool.poetry]
 name = "syncshell"
-version = "1.0.5"
+version = "1.0.6"
 description = "Keep your machine's shell history synchronized."
 
 license = "MIT"
 
-authors = [
-    "Masoud Ghorbani <msud.ghorbani@gmail.com>"
-]
+authors = ["Masoud Ghorbani <msud.ghorbani@gmail.com>"]
 
 readme = "README.md"
 
 repository = "https://github.com/msudgh/syncshell"
 homepage = "https://github.com/msudgh/syncshell"
 
 keywords = ["sync", "shell", "history", "bash", "zsh"]
 
 [tool.poetry.dependencies]
-python = "^3.7.13"
+python = "^3.8.16"
 black = "22.3.0"
 fire = "0.1.3"
-flake8 = "4.0.1"
+flake8 = "6.0.0"
 halo = "0.0.12"
 PyGithub = "1.55"
-pytest = "7.1.2"
+pytest = "7.3.1"
 pytest-testdox = "^3.0.1"
 
-[tool.poetry.dev-dependencies]
-pre-commit = "^2.19.0"
-
 [tool.black]
 py36 = true
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
     | dist
 )/
 '''
+
+# Ref: https://python-poetry.org/docs/pyproject/#scripts
+[project.scripts]
+syncshell = "syncshell.__main__:main"
```

### Comparing `syncshell-1.0.5/syncshell/cli.py` & `syncshell-1.0.6/syncshell/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,25 @@
 
 def prepare_payload():
     """Prepare history and config file for upload"""
 
     files = {}
     config_path = constants.CONFIG_PATH
 
-    with open(constants.SHELL_HISTORY_PATH, mode="r") as history_file:
-        files[os.path.basename(history_file.name)] = InputFileContent(
-            history_file.read()
-        )
+    with open(constants.SHELL_HISTORY_PATH, "r") as history_file:
+        history_file_path = os.path.basename(history_file.name)
+        try:
+            content = history_file.read()
+            files[history_file_path] = InputFileContent(content)
+        except UnicodeDecodeError:
+            with open(
+                constants.SHELL_HISTORY_PATH, "r", encoding="latin-1"
+            ) as history_file_latin_1:
+                content = history_file_latin_1.read()
+                files[history_file_path] = InputFileContent(content)
 
     with open(config_path, mode="r") as config_file:
         # Remove token key on uplaod
         lines = config_file.readlines()
         lines.pop(1)
 
         files[os.path.basename(config_file.name)] = InputFileContent(
@@ -55,37 +62,45 @@
             # Promte token key
             prompt_token = input("Enter your Github token key: ")
             config.parser["Auth"]["token"] = str(prompt_token)
 
             # Set new token key
             config.gist = Github(config.parser["Auth"]["token"])
 
+            spinner = Spinner.NewTask("Check authentication...")
+
             # Write config file if Github user alreaded authorized
-            if config.is_logged_in(False):
+            if config.is_logged_in():
+                spinner.succeed("Your Github token key is authenticated.")
                 config.write()
+            else:
+                spinner.fail("Your Github token key is not valid.")
+                sys.exit(1)
         except KeyboardInterrupt:
             sys.exit(0)
 
     def upload(self):
         """Upload current history"""
         spinner = Spinner.NewTask("Uploading ...")
 
         # Exit process if not logged in
         if not config.is_logged_in():
+            spinner.fail("Your Github token key is not valid. Authenticate first.")
             sys.exit(1)
 
         try:
             if config.parser["Auth"]["gist_id"]:
                 gist = config.gist.get_gist(config.parser["Auth"]["gist_id"])
 
                 # Set upload date
                 config.parser["Upload"]["last_date"] = str(int(time.time()))
                 config.write()
 
                 files = prepare_payload()
+
                 gist.edit(files=files)
 
                 spinner.succeed(f"Gist ID ({gist.id}) updated.")
             else:
                 description = "SyncShell Gist"
 
                 user = config.gist.get_user()
```

### Comparing `syncshell-1.0.5/syncshell/config.py` & `syncshell-1.0.6/syncshell/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import sys
 import os
 from shutil import copy
 from configparser import ConfigParser, Error as ConfigParserError
 from github import Github, GithubException
-from syncshell.utils import constants, spinner as Spinner
+from syncshell.utils import constants
 
 
 class SyncShellConfig:
     """Config class consits of fundamental methods to read, write and validate
     config file for different scenarios of syncshell.
     """
 
@@ -63,25 +63,18 @@
 
             return True
         except IOError:
             print("Unable to set config file.")
             sys.exit(1)
             return False
 
-    def is_logged_in(self, in_background=True):
+    def is_logged_in(self):
         """Check user exists in config file"""
-
         try:
             user = self.gist.get_user()
+
             if not user.login:
                 return False
 
-            if not in_background:
-                spinner = Spinner.NewTask("Check authenticated ...")
-                spinner.succeed("Your Github token key is authenticated.")
-
             return True
         except GithubException:
-            fail_text = "Your Github token key is not valid. Authenticate first."
-            spinner.fail(fail_text)
-
             return False
```

### Comparing `syncshell-1.0.5/syncshell/utils/constants.py` & `syncshell-1.0.6/syncshell/utils/constants.py`

 * *Files identical despite different names*

### Comparing `syncshell-1.0.5/syncshell/utils/spinner.py` & `syncshell-1.0.6/syncshell/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `syncshell-1.0.5/setup.py` & `syncshell-1.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,119 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: syncshell
+Version: 1.0.6
+Summary: Keep your machine's shell history synchronized.
+Home-page: https://github.com/msudgh/syncshell
+License: MIT
+Keywords: sync,shell,history,bash,zsh
+Author: Masoud Ghorbani
+Author-email: msud.ghorbani@gmail.com
+Requires-Python: >=3.8.16,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyGithub (==1.55)
+Requires-Dist: black (==22.3.0)
+Requires-Dist: fire (==0.1.3)
+Requires-Dist: flake8 (==6.0.0)
+Requires-Dist: halo (==0.0.12)
+Requires-Dist: pytest (==7.3.1)
+Requires-Dist: pytest-testdox (>=3.0.1,<4.0.0)
+Project-URL: Repository, https://github.com/msudgh/syncshell
+Description-Content-Type: text/markdown
+
+# SyncShell
+<!-- License -->
+<a href="https://mit-license.org/msudgh">
+  <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"
+    alt="MIT License" />
+</a>
+<!-- Build Status -->
+<a href="https://github.com/msudgh/syncshell/actions/workflows/test.yaml">
+  <img src="https://github.com/msudgh/syncshell/actions/workflows/test.yaml/badge.svg?branch=main"
+    alt="Build Status" />
+</a>
+<!-- Releases -->
+<a href="https://github.com/msudgh/syncshell/releases">
+  <img src="https://img.shields.io/github/release/msudgh/syncshell.svg"
+    alt="PyPi" />
+</a>
+<!-- PyPi -->
+<a href="https://pypi.org/project/syncshell/">
+  <img src="https://img.shields.io/pypi/v/syncshell.svg"
+    alt="PyPi" />
+</a>
+
+SyncShell as a simple and secure tool allows to synchronize machine's shell history across devices. It's built on top of Github Gist and written in Python (CLI). With SyncShell, you no longer have to worry about manually syncing your office and home machine's shell history and let continue where the terminal session left.
+
+## Features
+
+- Sync your shell history across all your devices
+- Securely store your shell history on Github Gist
+- Support for `zsh` and `bash` shells
+- Easy to install and use
+
+## Installation
+To install SyncShell, simply run the following command:
+
+```bash
+$ pip install syncshell
+```
+
+## Usage
+To use SyncShell, It first needs to set up a Github token key by following these steps:
+
+1. Open [**Github personal access tokens**](https://github.com/settings/tokens) page, [**Generate a new token**](https://github.com/settings/tokens/new) with `gist` scope feature.
+2. Execute the **`syncshell auth`** command, Enter the token key to validate and confirm it.
+
+Once finished, try to upload shell history by the following command:
+
+```bash
+$ syncshell upload
+```
+
+After uploading, the download command lets to sync and pull changes on the other machines:
+
+```bash
+$ syncshell download
+```
+
+
+### Synopsis
+
+```bash
+$ syncshell
+Type:        Application
+String form: <syncshell.cli.Application object at 0x101b1ff10>
+Docstring:   SyncShell CLI Application
+
+Usage:       syncshell 
+             syncshell auth
+             syncshell download
+             syncshell upload
+```
+
+## How it Works
+
+SyncShell is a tool that synchronizes shell history across all devices by securely storing the history file on Github Gist. Github Gist provides two types of Gists, `public` and `secret`. When the `syncshell upload` command is executed, the shell history file is uploaded and stored securely on Github Gist as a secret Gist. To download the uploaded shell history on other devices, the `syncshell download` command is used. This command retrieves the previously uploaded Gist, allowing the user to access their shell history on any device.
+
+**Security:** A Gist will be secret until it's not shared and will be secret and safe until you only have the Github Token and Gist ID.
+
+**Privacy:** In case of having password or secret in a history file, Its suggested to first have a alignment with privacy policies for any usecase.
+
+## Contributing
+Appreciate the contribution to this repository.
+
+To contribute, you need to follow the below steps for suggesting a change or a new feature:
+
+1. Install [poetry](https://python-poetry.org/docs/#installation) as a dependency manager
+2. Install dependencies by running ```poetry install```
+3. Make your changes
+4. Run and debug your changes by running ```poetry run python syncshell```
+5. Run tests by running ```poetry run pytest -c pytest.ini -s```
+6. Submit a pull request
 
-packages = \
-['syncshell', 'syncshell.utils']
+## License
+The code is licensed under the MIT License. See the data's [LICENSE](https://github.com/msudgh/syncshell/blob/main/LICENSE) file for more information.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyGithub==1.55',
- 'black==22.3.0',
- 'fire==0.1.3',
- 'flake8==4.0.1',
- 'halo==0.0.12',
- 'pytest-testdox>=3.0.1,<4.0.0',
- 'pytest==7.1.2']
-
-setup_kwargs = {
-    'name': 'syncshell',
-    'version': '1.0.5',
-    'description': "Keep your machine's shell history synchronized.",
-    'long_description': '<h1 align="center">SyncShell</h1>\n\n<div align="center">\n  <strong>Yet another tool for laziness</strong>\n</div>\n<div align="center">\n  Keep your machine\'s shell history synchronized\n</div>\n<br/>\n<div align="center">\n  <!-- Build Status -->\n  <a href="https://github.com/msudgh/syncshell/actions/workflows/test.yaml">\n    <img src="https://github.com/msudgh/syncshell/actions/workflows/test.yaml/badge.svg?branch=main"\n      alt="Build Status" />\n  </a>\n  <!-- License -->\n  <a href="https://mit-license.org/msudgh">\n    <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"\n      alt="MIT License" />\n  </a>\n  <!-- Release -->\n  <a href="https://github.com/msudgh/syncshell/releases">\n    <img src="https://img.shields.io/github/release/msudgh/syncshell.svg"\n      alt="PyPi" />\n  </a>\n  <!-- PyPi -->\n  <a href="https://pypi.org/project/syncshell/">\n    <img src="https://img.shields.io/pypi/v/syncshell.svg"\n      alt="PyPi" />\n  </a>\n</div>\n<br/>\n\n## Get SyncShell\nCurrently, `SyncShell` is just available on `PyPi` and by the following command install the latest version:\n```bash\n$ pip install syncshell # Maybe sudo need\n```\n```bash\n$ syncshell -- --help\nType:        Application\nString form: <syncshell.cli.Application object at 0x1035f51c0>\nDocstring:   SyncShell CLI Application\n\nUsage:       syncshell \n             syncshell auth\n             syncshell download\n             syncshell upload\n```\n\n## How it Works\nThe actual idea of SyncShell is synchronization of your all device\'s shell history, it means you don\'t need to have concerns when you want to sync your office and home machine\'s shell history. Application integrated and built on top of Github Gist, and written in Python (CLI).\n\nAccording to Github API, you can generate a token key with `gist` scope to access to Gist. \nGists have two **`public`**, **`secret`** type which syncshell while executing `syncshell upload` command will upload your history file and store them on Github Gist securely (**private**).\n\nOn the others machine, by executing `syncshell download` after entering your token key and created Gist ID you can download the gist and sync your shell\'s history.\n\n  > Gists will be secret until you don\'t share it with someone else, In other words, It\'ll be secret and safe until you only have the Github Token and Gist ID.\n\n## Usage\n  > Currently, `SyncShell` just support `zsh` and supporting other shells is in WIP.\n\nBefore SyncShell can be useful you need to setup your Github token key:\n\n  1. Open [**Github personal access tokens**](https://github.com/settings/tokens) page, [**Generate a new token**](https://github.com/settings/tokens/new) with `gist` scope feature.\n  2. Execute the **`syncshell auth`** command, Enter your token key to validate and confirm it.\n  3. Done :wink:\n\nNow you can try to upload your shell history by the following command:\n\n```bash\n$ syncshell upload\n```\n\nAfter the uploading process, you\'ll take a Gist ID that by this ID and your Github token, you can download history on the others machine by executing the following command:\n```bash\n$ syncshell download\n```\n\n## Todo\n- [ ] Write more test cases\n- [x] Support `zsh`, `bash`\n\n## Contributing\nSo nice you wanna contribute to this repository. Thank you. You may contribute in several ways consists of:\n\n* Creating new features\n* Fixing bugs\n\n#### Installing dependencies\n[Poetry Installation](https://python-poetry.org/docs/#installation) is straightforward walkthough to setup a versatile package manager.\n\nBy the following command install syncshell dependencies\n```bash\n# Clone syncshell repository\n$ git clone git@github.com:msudgh/syncshell.git\n$ cd syncshell\n$ poetry install\n```\n\n#### Tests\nBefore submiting your PR, Execute the below command to be sure about passing test cases.\n```bash\n$ poetry run pytest -c pytest.ini -s\n```\n\nDone :wink:\n\n## License\nThe code is licensed under the MIT License. See the data\'s [LICENSE](https://github.com/msudgh/syncshell/blob/main/LICENSE) file for more information.\n',
-    'author': 'Masoud Ghorbani',
-    'author_email': 'msud.ghorbani@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/msudgh/syncshell',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.13,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,62 +1,51 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['syncshell',
-'syncshell.utils'] package_data = \ {'': ['*']} install_requires = \
-['PyGithub==1.55', 'black==22.3.0', 'fire==0.1.3', 'flake8==4.0.1',
-'halo==0.0.12', 'pytest-testdox>=3.0.1,<4.0.0', 'pytest==7.1.2'] setup_kwargs =
-{ 'name': 'syncshell', 'version': '1.0.5', 'description': "Keep your machine's
-shell history synchronized.", 'long_description': '
-                            ****** SyncShell ******
-\n\n
-                      \n Yet another tool for laziness\n
-\n
-             \n Keep your machine\'s shell history synchronized\n
-\n
-\n
- \n \n \n_n_alt="Build_Status"_/>\n\n \n \n_n_alt="MIT_License"_/>\n\n \n \n_n
-                  alt="PyPi"_/>\n\n \n \n_n_alt="PyPi"_/>\n\n
-\n
-\n\n## Get SyncShell\nCurrently, `SyncShell` is just available on `PyPi` and by
-the following command install the latest version:\n```bash\n$ pip install
-syncshell # Maybe sudo need\n```\n```bash\n$ syncshell -- --help\nType:
-Application\nString form:
-cli.Application object at 0x1035f51c0>\nDocstring: SyncShell CLI
-Application\n\nUsage: syncshell \n syncshell auth\n syncshell download\n
-syncshell upload\n```\n\n## How it Works\nThe actual idea of SyncShell is
-synchronization of your all device\'s shell history, it means you don\'t need
-to have concerns when you want to sync your office and home machine\'s shell
-history. Application integrated and built on top of Github Gist, and written in
-Python (CLI).\n\nAccording to Github API, you can generate a token key with
-`gist` scope to access to Gist. \nGists have two **`public`**, **`secret`**
-type which syncshell while executing `syncshell upload` command will upload
-your history file and store them on Github Gist securely (**private**).\n\nOn
-the others machine, by executing `syncshell download` after entering your token
-key and created Gist ID you can download the gist and sync your shell\'s
-history.\n\n > Gists will be secret until you don\'t share it with someone
-else, In other words, It\'ll be secret and safe until you only have the Github
-Token and Gist ID.\n\n## Usage\n > Currently, `SyncShell` just support `zsh`
-and supporting other shells is in WIP.\n\nBefore SyncShell can be useful you
-need to setup your Github token key:\n\n 1. Open [**Github personal access
+Metadata-Version: 2.1 Name: syncshell Version: 1.0.6 Summary: Keep your
+machine's shell history synchronized. Home-page: https://github.com/msudgh/
+syncshell License: MIT Keywords: sync,shell,history,bash,zsh Author: Masoud
+Ghorbani Author-email: msud.ghorbani@gmail.com Requires-Python: >=3.8.16,<4.0.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: PyGithub (==1.55) Requires-Dist:
+black (==22.3.0) Requires-Dist: fire (==0.1.3) Requires-Dist: flake8 (==6.0.0)
+Requires-Dist: halo (==0.0.12) Requires-Dist: pytest (==7.3.1) Requires-Dist:
+pytest-testdox (>=3.0.1,<4.0.0) Project-URL: Repository, https://github.com/
+msudgh/syncshell Description-Content-Type: text/markdown # SyncShell  [MIT
+License]  [Build_Status]  [PyPi]  [PyPi] SyncShell as a simple and secure tool
+allows to synchronize machine's shell history across devices. It's built on top
+of Github Gist and written in Python (CLI). With SyncShell, you no longer have
+to worry about manually syncing your office and home machine's shell history
+and let continue where the terminal session left. ## Features - Sync your shell
+history across all your devices - Securely store your shell history on Github
+Gist - Support for `zsh` and `bash` shells - Easy to install and use ##
+Installation To install SyncShell, simply run the following command: ```bash $
+pip install syncshell ``` ## Usage To use SyncShell, It first needs to set up a
+Github token key by following these steps: 1. Open [**Github personal access
 tokens**](https://github.com/settings/tokens) page, [**Generate a new token**]
-(https://github.com/settings/tokens/new) with `gist` scope feature.\n 2.
-Execute the **`syncshell auth`** command, Enter your token key to validate and
-confirm it.\n 3. Done :wink:\n\nNow you can try to upload your shell history by
-the following command:\n\n```bash\n$ syncshell upload\n```\n\nAfter the
-uploading process, you\'ll take a Gist ID that by this ID and your Github
-token, you can download history on the others machine by executing the
-following command:\n```bash\n$ syncshell download\n```\n\n## Todo\n- [ ] Write
-more test cases\n- [x] Support `zsh`, `bash`\n\n## Contributing\nSo nice you
-wanna contribute to this repository. Thank you. You may contribute in several
-ways consists of:\n\n* Creating new features\n* Fixing bugs\n\n#### Installing
-dependencies\n[Poetry Installation](https://python-poetry.org/docs/
-#installation) is straightforward walkthough to setup a versatile package
-manager.\n\nBy the following command install syncshell dependencies\n```bash\n#
-Clone syncshell repository\n$ git clone git@github.com:msudgh/syncshell.git\n$
-cd syncshell\n$ poetry install\n```\n\n#### Tests\nBefore submiting your PR,
-Execute the below command to be sure about passing test cases.\n```bash\n$
-poetry run pytest -c pytest.ini -s\n```\n\nDone :wink:\n\n## License\nThe code
-is licensed under the MIT License. See the data\'s [LICENSE](https://
-github.com/msudgh/syncshell/blob/main/LICENSE) file for more information.\n',
-'author': 'Masoud Ghorbani', 'author_email': 'msud.ghorbani@gmail.com',
-'maintainer': None, 'maintainer_email': None, 'url': 'https://github.com/
-msudgh/syncshell', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.7.13,<4.0.0', }
-setup(**setup_kwargs)
+(https://github.com/settings/tokens/new) with `gist` scope feature. 2. Execute
+the **`syncshell auth`** command, Enter the token key to validate and confirm
+it. Once finished, try to upload shell history by the following command:
+```bash $ syncshell upload ``` After uploading, the download command lets to
+sync and pull changes on the other machines: ```bash $ syncshell download ```
+### Synopsis ```bash $ syncshell Type: Application String form:
+cli.Application object at 0x101b1ff10> Docstring: SyncShell CLI Application
+Usage: syncshell syncshell auth syncshell download syncshell upload ``` ## How
+it Works SyncShell is a tool that synchronizes shell history across all devices
+by securely storing the history file on Github Gist. Github Gist provides two
+types of Gists, `public` and `secret`. When the `syncshell upload` command is
+executed, the shell history file is uploaded and stored securely on Github Gist
+as a secret Gist. To download the uploaded shell history on other devices, the
+`syncshell download` command is used. This command retrieves the previously
+uploaded Gist, allowing the user to access their shell history on any device.
+**Security:** A Gist will be secret until it's not shared and will be secret
+and safe until you only have the Github Token and Gist ID. **Privacy:** In case
+of having password or secret in a history file, Its suggested to first have a
+alignment with privacy policies for any usecase. ## Contributing Appreciate the
+contribution to this repository. To contribute, you need to follow the below
+steps for suggesting a change or a new feature: 1. Install [poetry](https://
+python-poetry.org/docs/#installation) as a dependency manager 2. Install
+dependencies by running ```poetry install``` 3. Make your changes 4. Run and
+debug your changes by running ```poetry run python syncshell``` 5. Run tests by
+running ```poetry run pytest -c pytest.ini -s``` 6. Submit a pull request ##
+License The code is licensed under the MIT License. See the data's [LICENSE]
+(https://github.com/msudgh/syncshell/blob/main/LICENSE) file for more
+information.
```

