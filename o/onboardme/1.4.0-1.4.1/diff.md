# Comparing `tmp/onboardme-1.4.0.tar.gz` & `tmp/onboardme-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.4.0.tar", max compression
+gzip compressed data, was "onboardme-1.4.1.tar", max compression
```

## Comparing `onboardme-1.4.0.tar` & `onboardme-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2023-05-28 15:28:05.091720 onboardme-1.4.0/LICENSE.txt
--rw-r--r--   0        0        0    15601 2023-05-29 15:10:47.936626 onboardme-1.4.0/README.md
--rwxr-xr-x   0        0        0     7282 2023-05-29 15:10:47.936626 onboardme-1.4.0/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2023-05-28 15:28:05.103721 onboardme-1.4.0/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2023-05-28 15:28:05.103721 onboardme-1.4.0/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-05-28 15:28:05.103721 onboardme-1.4.0/onboardme/console_logging.py
--rw-r--r--   0        0        0     2095 2023-05-29 15:10:47.936626 onboardme-1.4.0/onboardme/constants.py
--rw-r--r--   0        0        0     5141 2023-05-28 15:28:05.103721 onboardme-1.4.0/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5825 2023-05-29 15:10:47.936626 onboardme-1.4.0/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-05-28 15:28:05.103721 onboardme-1.4.0/onboardme/firewall.py
--rwxr-xr-x   0        0        0     6017 2023-05-29 15:10:47.936626 onboardme-1.4.0/onboardme/help_text.py
--rw-r--r--   0        0        0     3085 2023-05-28 15:28:05.103721 onboardme-1.4.0/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2023-05-28 15:28:05.103721 onboardme-1.4.0/onboardme/misc.py
--rwxr-xr-x   0        0        0     9785 2023-05-29 15:10:47.936626 onboardme-1.4.0/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0      233 2023-05-28 15:28:05.103721 onboardme-1.4.0/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-05-28 15:28:05.103721 onboardme-1.4.0/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2023-05-28 15:28:05.103721 onboardme-1.4.0/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1792 2023-05-29 15:10:47.936626 onboardme-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    16931 1970-01-01 00:00:00.000000 onboardme-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-04 09:30:31.748637 onboardme-1.4.1/LICENSE.txt
+-rw-r--r--   0        0        0    16332 2023-06-04 09:30:31.748637 onboardme-1.4.1/README.md
+-rwxr-xr-x   0        0        0     7282 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/console_logging.py
+-rw-r--r--   0        0        0     2095 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/constants.py
+-rw-r--r--   0        0        0     5141 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5825 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     6017 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/help_text.py
+-rw-r--r--   0        0        0     3085 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/misc.py
+-rwxr-xr-x   0        0        0     9785 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0      233 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1792 2023-06-04 09:30:31.776638 onboardme-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    17662 1970-01-01 00:00:00.000000 onboardme-1.4.1/PKG-INFO
```

### Comparing `onboardme-1.4.0/LICENSE.txt` & `onboardme-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/README.md` & `onboardme-1.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -232,75 +232,94 @@
 | `$XDG_CONFIG_HOME/onboardme/packages.yml` | For adding packages with different package managers |
 
 Examples:
 <details>
 <summary><code>~/.config/onboardme/config.yml</code></summary>
 
 ```yaml
+---
+# ______________________________________________________________ #
+#         Config file for the onboardme cli command.             #
+# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
+#  - If this files exists as: ~/.config/onboardme/config.yaml    #
+#    then its loaded instead of the default config               #
+# -------------------------------------------------------------- #
+
+
 log:
   # Full path to a file you'd like to log to. Creates file if it doesn't exist
   file: ""
-  # what level of logs to output (DEBUG, INFO, WARN, ERROR)
-  level: "INFO"
+  # what level of logs to output (debug, info, warn, error)
+  level: "warn"
 
 # steps refer to a specific function in the list of functions we run
 steps:
   # these are mac specific steps
   Darwin:
-    # clones dot files into home dir/git fetches updates for dot files
     - dot_files
-    # install packages
     - packages
-    # adds nerdfonts
     - font_setup
-    # runs :Lazy sync to install all your plugins
     - neovim_setup
-    # sets up touchID for sudo
     - sudo_setup
   # these are linux specific steps
   Linux:
     - dot_files
     - packages
     - font_setup
     - neovim_setup
-    # add your user to the docker group
     - group_setup
 
 dot_files:
   # personal git repo URL for your dot files, defaults to jessebot/dot_files
   git_url: "https://github.com/jessebot/dot_files.git"
   # the branch to use for the git repo above, defaults to main
   git_branch: "main"
-  # !CAREFUL: runs a `git reset --hard`, which will overwite/delete local files in ~ that
-  # conflict with the above defined git repo url and branch. You should run
-  # `onboardme -s dot_files` to get the files that would be overwritten
+  # !!CAREFUL: runs a `git reset --hard`, which will overwite/delete files in 
+  # $HOME that conflict with the above defined git repo url and branch.
+  # You should run the following to get the files that would be overwritten:
+  # onboardme -s dot_files
+  # if set to true, then using onboardme -O will toggle it back to false
   overwrite: false
 
-# basic package config
+# This is the basic package config.
 package:
   # Remove any of the below pkg managers to only run the remaining pkg managers
   managers:
-    # these are macOS specific steps
+    # macOS specific steps
     Darwin:
       - brew
       - pip3.11
-    # these are linux specific steps
+    # Debian/Ubuntu specific steps
     Linux:
+      - apt
       - brew
       - pip3.11
-      - apt
-      - snap
       - flatpak
+      - snap
   # list of extra existing packages groups to install
   groups:
-    - default
-    # uncomment these to add them as default installed package groups
-    # - gui
-    # - gaming
-    # - devops
+    default:
+      # basic tui stuff to have a nice time in the terminal :)
+      - default
+    # move these package.groups.default to always install them
+    optional:
+      # setting up more python data science specific tooling
+      - data_science
+      # kubernetes and docker tools
+      - devops
+      # gaming always installs gui
+      - gaming
+      # freetube and other gui applications
+      - gui
+      # this configures neomutt and offlineimap
+      - mail
+      # sets up useful music tui stuff for spotify and youtube
+      - music
+      # things like zoom and slack
+      - work
 ```
 
 </details>
 
 ## Under the Hood
 Made and tested for these operating systems:
```

### Comparing `onboardme-1.4.0/onboardme/__init__.py` & `onboardme-1.4.1/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/config/firewall/iptables.sh` & `onboardme-1.4.1/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/console_logging.py` & `onboardme-1.4.1/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/constants.py` & `onboardme-1.4.1/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/dot_files.py` & `onboardme-1.4.1/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/env_config.py` & `onboardme-1.4.1/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/firewall.py` & `onboardme-1.4.1/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/help_text.py` & `onboardme-1.4.1/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/ide_setup.py` & `onboardme-1.4.1/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/misc.py` & `onboardme-1.4.1/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/pkg_management.py` & `onboardme-1.4.1/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/subproc.py` & `onboardme-1.4.1/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/onboardme/sudo_setup.py` & `onboardme-1.4.1/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.0/pyproject.toml` & `onboardme-1.4.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.4.0"
+version       = "1.4.1"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
@@ -21,15 +21,15 @@
 packages      = [{include = "onboardme"}]
 include       = ["onboardme/scripts/update_apt_sources.sh",
                  "onboardme/scripts/get_apt_list.sh"]
 
 [tool.poetry.dependencies]
 python              = "^3.11"
 click               = "^8.1"
-rich                = "^13.3"
+rich                = "^13.4"
 PyYAML              = "^6.0"
 GitPython           = "^3.1"
 wget                = "^3.2"
 xdg-base-dirs       = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3"
```

### Comparing `onboardme-1.4.0/PKG-INFO` & `onboardme-1.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.4.0
+Version: 1.4.1
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
@@ -15,15 +15,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Installation/Setup
 Requires-Dist: GitPython (>=3.1,<4.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1,<9.0)
-Requires-Dist: rich (>=13.3,<14.0)
+Requires-Dist: rich (>=13.4,<14.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Requires-Dist: xdg-base-dirs (>=6.0,<7.0)
 Project-URL: Bug Tracker, http://github.com/jessebot/onboardme/issues
 Project-URL: Documentation, https://jessebot.github.io/onboardme/onboardme
 Project-URL: Repository, http://github.com/jessebot/onboardme
 Description-Content-Type: text/markdown
 
@@ -261,75 +261,94 @@
 | `$XDG_CONFIG_HOME/onboardme/packages.yml` | For adding packages with different package managers |
 
 Examples:
 <details>
 <summary><code>~/.config/onboardme/config.yml</code></summary>
 
 ```yaml
+---
+# ______________________________________________________________ #
+#         Config file for the onboardme cli command.             #
+# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
+#  - If this files exists as: ~/.config/onboardme/config.yaml    #
+#    then its loaded instead of the default config               #
+# -------------------------------------------------------------- #
+
+
 log:
   # Full path to a file you'd like to log to. Creates file if it doesn't exist
   file: ""
-  # what level of logs to output (DEBUG, INFO, WARN, ERROR)
-  level: "INFO"
+  # what level of logs to output (debug, info, warn, error)
+  level: "warn"
 
 # steps refer to a specific function in the list of functions we run
 steps:
   # these are mac specific steps
   Darwin:
-    # clones dot files into home dir/git fetches updates for dot files
     - dot_files
-    # install packages
     - packages
-    # adds nerdfonts
     - font_setup
-    # runs :Lazy sync to install all your plugins
     - neovim_setup
-    # sets up touchID for sudo
     - sudo_setup
   # these are linux specific steps
   Linux:
     - dot_files
     - packages
     - font_setup
     - neovim_setup
-    # add your user to the docker group
     - group_setup
 
 dot_files:
   # personal git repo URL for your dot files, defaults to jessebot/dot_files
   git_url: "https://github.com/jessebot/dot_files.git"
   # the branch to use for the git repo above, defaults to main
   git_branch: "main"
-  # !CAREFUL: runs a `git reset --hard`, which will overwite/delete local files in ~ that
-  # conflict with the above defined git repo url and branch. You should run
-  # `onboardme -s dot_files` to get the files that would be overwritten
+  # !!CAREFUL: runs a `git reset --hard`, which will overwite/delete files in 
+  # $HOME that conflict with the above defined git repo url and branch.
+  # You should run the following to get the files that would be overwritten:
+  # onboardme -s dot_files
+  # if set to true, then using onboardme -O will toggle it back to false
   overwrite: false
 
-# basic package config
+# This is the basic package config.
 package:
   # Remove any of the below pkg managers to only run the remaining pkg managers
   managers:
-    # these are macOS specific steps
+    # macOS specific steps
     Darwin:
       - brew
       - pip3.11
-    # these are linux specific steps
+    # Debian/Ubuntu specific steps
     Linux:
+      - apt
       - brew
       - pip3.11
-      - apt
-      - snap
       - flatpak
+      - snap
   # list of extra existing packages groups to install
   groups:
-    - default
-    # uncomment these to add them as default installed package groups
-    # - gui
-    # - gaming
-    # - devops
+    default:
+      # basic tui stuff to have a nice time in the terminal :)
+      - default
+    # move these package.groups.default to always install them
+    optional:
+      # setting up more python data science specific tooling
+      - data_science
+      # kubernetes and docker tools
+      - devops
+      # gaming always installs gui
+      - gaming
+      # freetube and other gui applications
+      - gui
+      # this configures neomutt and offlineimap
+      - mail
+      # sets up useful music tui stuff for spotify and youtube
+      - music
+      # things like zoom and slack
+      - work
 ```
 
 </details>
 
 ## Under the Hood
 Made and tested for these operating systems:
```

