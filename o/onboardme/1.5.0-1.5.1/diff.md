# Comparing `tmp/onboardme-1.5.0.tar.gz` & `tmp/onboardme-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.5.0.tar", max compression
+gzip compressed data, was "onboardme-1.5.1.tar", max compression
```

## Comparing `onboardme-1.5.0.tar` & `onboardme-1.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2023-06-04 12:33:10.896737 onboardme-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0    13530 2023-06-04 12:33:10.896737 onboardme-1.5.0/README.md
--rwxr-xr-x   0        0        0     7600 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/console_logging.py
--rw-r--r--   0        0        0     2095 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/constants.py
--rw-r--r--   0        0        0     5636 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     6182 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/firewall.py
--rwxr-xr-x   0        0        0     6171 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/help_text.py
--rw-r--r--   0        0        0     3085 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/misc.py
--rwxr-xr-x   0        0        0     9785 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0      233 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1738 2023-06-04 12:33:10.924738 onboardme-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    14860 1970-01-01 00:00:00.000000 onboardme-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-04 15:12:08.268515 onboardme-1.5.1/LICENSE.txt
+-rw-r--r--   0        0        0    13530 2023-06-04 15:12:08.268515 onboardme-1.5.1/README.md
+-rwxr-xr-x   0        0        0     7600 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/console_logging.py
+-rw-r--r--   0        0        0     2095 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/constants.py
+-rw-r--r--   0        0        0     5641 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     6182 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     6276 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/help_text.py
+-rw-r--r--   0        0        0     3085 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/misc.py
+-rwxr-xr-x   0        0        0     9785 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0      233 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2023-06-04 15:12:08.296515 onboardme-1.5.1/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1738 2023-06-04 15:12:08.300515 onboardme-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    14860 1970-01-01 00:00:00.000000 onboardme-1.5.1/PKG-INFO
```

### Comparing `onboardme-1.5.0/LICENSE.txt` & `onboardme-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/README.md` & `onboardme-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/__init__.py` & `onboardme-1.5.1/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/config/firewall/iptables.sh` & `onboardme-1.5.1/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/console_logging.py` & `onboardme-1.5.1/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/constants.py` & `onboardme-1.5.1/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/dot_files.py` & `onboardme-1.5.1/onboardme/dot_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     # this one needs to be allowed to fail because it might already exist
     cmds = [f"git remote add origin {git_url}"]
     subproc(cmds, error_ok=True, spinner=False, **opts)
 
     # create ~/.config/.git to get git status while editing config files
     if not path.isfile(f"{XDG_CONFIG_DIR}/.git"):
-        with open(f"{XDG_CONFIG_DIR}/.git") as config_git_config:
+        with open(f"{XDG_CONFIG_DIR}/.git", "w") as config_git_config:
             config_git_config.write(f"gitdir: {dot_files_cfg_dir}")
 
     if overwrite:
         # WARN: this command will overwrite local files with remote files
         reset_cmd = f"git reset --hard origin/{branch}"
     else:
         reset_cmd = f"git reset origin/{branch}"
```

### Comparing `onboardme-1.5.0/onboardme/env_config.py` & `onboardme-1.5.1/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/firewall.py` & `onboardme-1.5.1/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/help_text.py` & `onboardme-1.5.1/onboardme/help_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,17 @@
         'git_branch':
         'Branch to use for the git repo url. Default: main',
 
         'git_config_dir':
         'Directory to store the git configuration for your dot files. '
         'Default: ~/.config/dot_files',
 
+        'generate_screenshot':
+        'Generate a few SVGs for use in the docs and README. Undocumented.',
+
         'overwrite':
         '[b]Overwrites[/b] existing dot files with files from configured '
         "[option]--git_url[/option] repo. If you've set overwrite: true in "
         'your config, then --overwrite on the command line will act as a '
         'toggle, so it will NOT overwrite your dot files.',
 
         'pkg_managers':
@@ -129,15 +132,15 @@
                       "[cornflower_blue][OPTIONS]\n")
 
         options_table = Table(highlight=True, box=None, show_header=False,
                               row_styles=["", "dim"],
                               padding=(1, 1, 0, 0))
 
         # this used to be self.get_params(ctx)[1:] to have only one hidden option
-        for param in self.get_params(ctx)[2:]:
+        for param in self.get_params(ctx):
 
             if len(param.opts) == 2:
                 opt1 = highlighter(param.opts[1])
                 opt2 = highlighter(param.opts[0])
             else:
                 opt2 = highlighter(param.opts[0])
                 opt1 = Text("")
```

### Comparing `onboardme-1.5.0/onboardme/ide_setup.py` & `onboardme-1.5.1/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/misc.py` & `onboardme-1.5.1/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/pkg_management.py` & `onboardme-1.5.1/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/subproc.py` & `onboardme-1.5.1/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/onboardme/sudo_setup.py` & `onboardme-1.5.1/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.5.0/pyproject.toml` & `onboardme-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.5.0"
+version       = "1.5.1"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.5.0/PKG-INFO` & `onboardme-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.5.0
+Version: 1.5.1
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
```

