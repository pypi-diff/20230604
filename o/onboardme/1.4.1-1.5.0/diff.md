# Comparing `tmp/onboardme-1.4.1.tar.gz` & `tmp/onboardme-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.4.1.tar", max compression
+gzip compressed data, was "onboardme-1.5.0.tar", max compression
```

## Comparing `onboardme-1.4.1.tar` & `onboardme-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2023-06-04 09:30:31.748637 onboardme-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0    16332 2023-06-04 09:30:31.748637 onboardme-1.4.1/README.md
--rwxr-xr-x   0        0        0     7282 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/console_logging.py
--rw-r--r--   0        0        0     2095 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/constants.py
--rw-r--r--   0        0        0     5141 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5825 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/firewall.py
--rwxr-xr-x   0        0        0     6017 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/help_text.py
--rw-r--r--   0        0        0     3085 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/misc.py
--rwxr-xr-x   0        0        0     9785 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0      233 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2023-06-04 09:30:31.776638 onboardme-1.4.1/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1792 2023-06-04 09:30:31.776638 onboardme-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    17662 1970-01-01 00:00:00.000000 onboardme-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-04 12:33:10.896737 onboardme-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0    13530 2023-06-04 12:33:10.896737 onboardme-1.5.0/README.md
+-rwxr-xr-x   0        0        0     7600 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/console_logging.py
+-rw-r--r--   0        0        0     2095 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/constants.py
+-rw-r--r--   0        0        0     5636 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     6182 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     6171 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/help_text.py
+-rw-r--r--   0        0        0     3085 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/misc.py
+-rwxr-xr-x   0        0        0     9785 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0      233 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2023-06-04 12:33:10.924738 onboardme-1.5.0/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1738 2023-06-04 12:33:10.924738 onboardme-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    14860 1970-01-01 00:00:00.000000 onboardme-1.5.0/PKG-INFO
```

### Comparing `onboardme-1.4.1/LICENSE.txt` & `onboardme-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.1/README.md` & `onboardme-1.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: onboardme
+Version: 1.5.0
+Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
+Home-page: http://github.com/jessebot/onboardme
+License: AGPL-3.0-or-later
+Keywords: onboardme,onboarding,desktop-setup,development-environment
+Author: Jesse Hitch
+Author-email: jessebot@linux.com
+Requires-Python: >=3.11,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Installation/Setup
+Requires-Dist: GitPython (>=3.1,<4.0)
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: rich (>=13.4,<14.0)
+Requires-Dist: wget (>=3.2,<4.0)
+Requires-Dist: xdg-base-dirs (>=6.0,<7.0)
+Project-URL: Bug Tracker, http://github.com/jessebot/onboardme/issues
+Project-URL: Documentation, https://jessebot.github.io/onboardme/onboardme
+Project-URL: Repository, http://github.com/jessebot/onboardme
+Description-Content-Type: text/markdown
+
 <h1 align="center">
   <img
     src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png"
     height="30"
     width="0px"
   />
   💻 onboard<i>me</i>
@@ -62,15 +91,19 @@
 If you haven't already made the switch from Vim to [NeoVim], you can try out NeoVim today with `onboardme` :D We used to support both neovim _and_ vim, but these days none of the primary developers of this repo use pure vim anymore, so we can't ensure it's up to standards. All of your knowledge from vim is still helpful in neovim though, and we highly recommend switching as neovim has a lot more features and a very active plugin community :) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/doc/user/nvim.html#nvim-from-vim). 
 
 </details>
 
 <details>
   <summary><h4>Easy <code>yaml</code> config files using XDG Base Directory Spec<h4></summary>
 
-We use use [XDG Base Directory Spec] for [config files](#configuration) so you always know where they are :)
+We use use [XDG Base Directory Spec] for config files, so you always know where they are :)
+
+Config files are in `$XDG_CONFIG_HOME/onboardme/`, <sub>or `~/.config/onboardme/` if `$XDG_CONFIG_HOME` is not defined</sub>.
+
+Learn more about configuration in the [config docs](https://jessebot.github.io/onboardme/onboardme/getting-started).
 
 </details>
 
 <details>
   <summary><h4>Docker image for an on-the-go dev workspace<h4></summary>
 
 The docker image is built nightly, and on push to `main` via GHA. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
@@ -191,21 +224,23 @@
 ```
 
 ## Using the Docker image
 
 Read more about our docker tags and how to use them at [jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme) on DockerHub.
 
 # Usage
+Learn more about configuration in the [config docs](https://jessebot.github.io/onboardme/onboardme/getting-started), but by default you can get started with:
 
-_Now_ you can run `onboardme` 🎉 
 ```bash
 # this will display the help text for onboardme
 onboardme --help
 
-# Running this won't overwrite any existing dot files, but it may add new ones.
+# Running this won't overwrite any existing dot files, but it may add new ones
+# and it may install new packages. Don't run this till you've looked at the files
+# in ~/.config/onboardme/
 onboardme
 ```
 
 From here, if you want to *completely wipe your existing dot files* for a fresh start with with `onboardme`, you can run:
 ```bash
 # WARNING: This will overwrite your local dotfiles, including your .bashrc and .bash_profile
 # can also be done with: onboardme -O
@@ -217,113 +252,14 @@
 ### Upgrades
 If you're on python 3.11, you should be able to do:
 
 ```bash
 pip3.11 install --upgrade onboardme
 ```
 
-### Configuration
-onboardme has lots of CLI options, but you can also use config files. You have to create these files for the time being.
-
-Config files are in `$XDG_CONFIG_HOME/onboardme/`, <sub>or `~/.config/onboardme/` if `$XDG_CONFIG_HOME` is not defined</sub>.
-
-| Config File                               |        Description                                  |
-|:------------------------------------------|:----------------------------------------------------|
-| `$XDG_CONFIG_HOME/onboardme/config.yml`   | For step configuration to run either all steps, or just a subset. | 
-| `$XDG_CONFIG_HOME/onboardme/packages.yml` | For adding packages with different package managers |
-
-Examples:
-<details>
-<summary><code>~/.config/onboardme/config.yml</code></summary>
-
-```yaml
----
-# ______________________________________________________________ #
-#         Config file for the onboardme cli command.             #
-# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
-#  - If this files exists as: ~/.config/onboardme/config.yaml    #
-#    then its loaded instead of the default config               #
-# -------------------------------------------------------------- #
-
-
-log:
-  # Full path to a file you'd like to log to. Creates file if it doesn't exist
-  file: ""
-  # what level of logs to output (debug, info, warn, error)
-  level: "warn"
-
-# steps refer to a specific function in the list of functions we run
-steps:
-  # these are mac specific steps
-  Darwin:
-    - dot_files
-    - packages
-    - font_setup
-    - neovim_setup
-    - sudo_setup
-  # these are linux specific steps
-  Linux:
-    - dot_files
-    - packages
-    - font_setup
-    - neovim_setup
-    - group_setup
-
-dot_files:
-  # personal git repo URL for your dot files, defaults to jessebot/dot_files
-  git_url: "https://github.com/jessebot/dot_files.git"
-  # the branch to use for the git repo above, defaults to main
-  git_branch: "main"
-  # !!CAREFUL: runs a `git reset --hard`, which will overwite/delete files in 
-  # $HOME that conflict with the above defined git repo url and branch.
-  # You should run the following to get the files that would be overwritten:
-  # onboardme -s dot_files
-  # if set to true, then using onboardme -O will toggle it back to false
-  overwrite: false
-
-# This is the basic package config.
-package:
-  # Remove any of the below pkg managers to only run the remaining pkg managers
-  managers:
-    # macOS specific steps
-    Darwin:
-      - brew
-      - pip3.11
-    # Debian/Ubuntu specific steps
-    Linux:
-      - apt
-      - brew
-      - pip3.11
-      - flatpak
-      - snap
-  # list of extra existing packages groups to install
-  groups:
-    default:
-      # basic tui stuff to have a nice time in the terminal :)
-      - default
-    # move these package.groups.default to always install them
-    optional:
-      # setting up more python data science specific tooling
-      - data_science
-      # kubernetes and docker tools
-      - devops
-      # gaming always installs gui
-      - gaming
-      # freetube and other gui applications
-      - gui
-      # this configures neomutt and offlineimap
-      - mail
-      # sets up useful music tui stuff for spotify and youtube
-      - music
-      # things like zoom and slack
-      - work
-```
-
-</details>
-
 ## Under the Hood
 Made and tested for these operating systems:
 
 [![Tested on Ventura 13.4 with a 13-inch M1 Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en)
 [![Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://www.debian.org/)
 [![Tested only on ubuntu servers](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/)
 
@@ -390,7 +326,8 @@
 [default packages]: https://github.com/jessebot/dot_files/blob/main/.config/onboardme/packages.yml "default installed packages for onboardme"
 
 <!-- external link references -->
 [dot files]: https://en.wikipedia.org/wiki/Hidden_file_and_hidden_directory#Unix_and_Unix-like_environments "wiki entry for dot file explanation"
 [XDG Base Directory Spec]: https://specifications.freedesktop.org/basedir-spec/latest/ar01s03.html
 [NeoVim]: https://neovim.io/ "neovim, vim improved"
 [lazy.nvim]: https://github.com/folke/lazy.nvim "lazy.nvim, a plugin manager for neovim"
+
```

### Comparing `onboardme-1.4.1/onboardme/__init__.py` & `onboardme-1.5.0/onboardme/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -108,14 +108,19 @@
         help=HELP['git_url'],
         default=USR_CONFIG_FILE['dot_files']['git_url'])
 @option('--git_branch',
         '-b',
         metavar='BRANCH',
         help=HELP['git_branch'],
         default=USR_CONFIG_FILE['dot_files']['git_branch'])
+@option('--git_config_dir',
+        '-d',
+        metavar='PATH',
+        help=HELP['git_config_dir'],
+        default=USR_CONFIG_FILE['dot_files']['git_config_dir'])
 @option('--overwrite',
         '-O',
         is_flag=True,
         help=HELP['overwrite'],
         default=USR_CONFIG_FILE['dot_files']['overwrite'])
 @option('--pkg_managers',
         '-p',
@@ -149,15 +154,15 @@
         is_flag=True)
 @option('--version',
         is_flag=True,
         help=HELP['version'],
         default=False)
 def main(log_level, log_file,
          steps, 
-         git_url, git_branch, overwrite,
+         git_url, git_branch, git_config_dir, overwrite,
          pkg_managers, pkg_groups,
          firewall, remote_host,
          no_upgrade,
          version) -> bool:
     """
     If run with no options on Linux, it will install brew, pip3.11, apt,
     flatpak, and snap packages. On mac, it only installs brew/pip3.11 packages.
@@ -173,31 +178,34 @@
     # before we do anything, we need to make sure this OS is supported
     check_os_support()
 
     # setup logging immediately
     log = setup_logger(log_level, log_file)
 
     # makes sure we only overwrite config file prefs if cli opts are passed in
-    usr_pref = process_configs(overwrite, git_url, git_branch, pkg_managers,
-                               pkg_groups, firewall, remote_host, steps,
+    usr_pref = process_configs(overwrite, git_url, git_branch, git_config_dir,
+                               pkg_managers, pkg_groups, 
+                               firewall, remote_host,
+                               steps,
                                log_file, log_level)
 
     if log:
         log.debug(f"User passed in the following preferences:\n{usr_pref}\n")
     else:
         logging.debug(f"User passed in the following preferences:\n{usr_pref}")
 
     # actual heavy lifting of onboardme happens in these
     for step in usr_pref['steps'][OS[0]]:
 
         if step == 'dot_files':
             # this creates a live git repo out of your home directory
             df_prefs = usr_pref['dot_files']
             setup_dot_files(OS, df_prefs['overwrite'],
-                            df_prefs['git_url'], df_prefs['git_branch'])
+                            df_prefs['git_url'], df_prefs['git_branch'],
+                            df_prefs['git_config_dir'])
 
         elif step == 'packages':
             pkg_mngrs = usr_pref['package']['managers'][OS[0]]
             pkg_groups = usr_pref['package']['groups']
             run_pkg_mngrs(pkg_mngrs, pkg_groups, no_upgrade)
 
         elif step in ['neovim_setup', 'font_setup']:
```

### Comparing `onboardme-1.4.1/onboardme/config/firewall/iptables.sh` & `onboardme-1.5.0/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.1/onboardme/console_logging.py` & `onboardme-1.5.0/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.1/onboardme/constants.py` & `onboardme-1.5.0/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.1/onboardme/dot_files.py` & `onboardme-1.5.0/onboardme/dot_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,48 +9,58 @@
 from rich.table import Table
 # custom libs
 from .constants import HOME_DIR, PWD, XDG_CONFIG_DIR
 from .console_logging import print_panel, print_msg
 from .subproc import subproc
 
 
-XDG_GIT_CFG_DIR = path.join(XDG_CONFIG_DIR, 'git')
-Path(XDG_GIT_CFG_DIR).mkdir(exist_ok=True)
-XDG_GIT_PATH = path.join(XDG_GIT_CFG_DIR, 'config')
+xdg_git_config_dir = path.join(XDG_CONFIG_DIR, 'git')
+Path(xdg_git_config_dir).mkdir(exist_ok=True)
+XDG_GIT_CONFIG = path.join(xdg_git_config_dir, 'config')
 
 
-def setup_dot_files(OS='Linux', overwrite=False,
+def setup_dot_files(OS='Linux',
+                    overwrite=False,
                     git_url="https://github.com/jessebot/dot_files.git",
-                    branch="main") -> None:
+                    branch="main",
+                    dot_files_cfg_dir=f"{XDG_CONFIG_DIR}/dot_files") -> None:
     """
     note on how we're doing things, seperate dot files repo:
     https://probablerobot.net/2021/05/keeping-'live'-dotfiles-in-a-git-repo/
+
+
     """
-    git_dir = path.join(HOME_DIR, '.git_dot_files')
-    # create ~/.git_dot_files if it does not exist
-    Path(git_dir).mkdir(exist_ok=True)
-    chdir(git_dir)
-    opts = {'quiet': True, 'cwd': git_dir}
+    # create dot_files_cfg_dir if it doesn't exist/don't complain if it does
+    # defaults to ~/.config/dot_files
+    Path(dot_files_cfg_dir).mkdir(parents=True, exist_ok=True)
+    chdir(dot_files_cfg_dir)
+    opts = {'quiet': True, 'cwd': dot_files_cfg_dir}
 
     if git_url:
         if "github.com" in git_url:
+            # get just the owner/repo_name like jessebot/dot_files
             user_repo = "/".join(git_url.split("/")[-2:]).replace(".git", "")
 
     # global: use main as default branch, always push up new remote branch
     git_raw = f"https://raw.githubusercontent.com/{user_repo}/{branch}"
 
-    cmds = [f'curl {git_raw}/.config/git/config -o {XDG_GIT_PATH}',
-            f'git --git-dir={git_dir} --work-tree={HOME_DIR} init',
+    cmds = [f'curl {git_raw}/.config/git/config -o {XDG_GIT_CONFIG}',
+            f'git --git-dir={dot_files_cfg_dir} --work-tree={HOME_DIR} init',
             'git config status.showUntrackedFiles no']
     subproc(cmds, spinner=False, **opts)
 
     # this one needs to be allowed to fail because it might already exist
     cmds = [f"git remote add origin {git_url}"]
     subproc(cmds, error_ok=True, spinner=False, **opts)
 
+    # create ~/.config/.git to get git status while editing config files
+    if not path.isfile(f"{XDG_CONFIG_DIR}/.git"):
+        with open(f"{XDG_CONFIG_DIR}/.git") as config_git_config:
+            config_git_config.write(f"gitdir: {dot_files_cfg_dir}")
+
     if overwrite:
         # WARN: this command will overwrite local files with remote files
         reset_cmd = f"git reset --hard origin/{branch}"
     else:
         reset_cmd = f"git reset origin/{branch}"
         git_action = "[b]differ[/b] from"
```

### Comparing `onboardme-1.4.1/onboardme/env_config.py` & `onboardme-1.5.0/onboardme/env_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import logging as log
 
 # rich helps pretty print everything
 from rich.prompt import Confirm
 
 # custom libs
-from .constants import OS, USR_CONFIG_FILE, DEFAULT_PKG_GROUPS
+from .constants import OS, USR_CONFIG_FILE, DEFAULT_PKG_GROUPS, HOME_DIR
 from .console_logging import print_panel
 
 
 def check_os_support():
     """
     verify we're on a supported OS and ask to quit if not.
     """
@@ -94,37 +94,48 @@
 
         if not value or always_prefer_default:
             user_config[key] = defaults[key]
 
     return user_config
 
 
-def process_configs(overwrite: bool, repo: str, git_branch: str, 
-                    pkg_mngrs: list, pkg_groups: list, firewall: bool,
-                    remote_host: str, steps: list, log_file: str,
+def process_configs(overwrite: bool,
+                    repo: str,
+                    git_branch: str,
+                    git_config_dir: str,
+                    pkg_mngrs: list,
+                    pkg_groups: list,
+                    firewall: bool,
+                    remote_host: str,
+                    steps: list,
+                    log_file: str,
                     log_level: str) -> dict:
     """
     process the config in ~/.config/onboardme/config.yml if it exists,
     then process the cli dict, and fill in defaults for anything not explicitly
     defined. Returns full final config as dict for use in script.
     """
     if remote_host:
         firewall = True
         if type(remote_host) is str:
             remote_host = [remote_host]
 
+    if "~" in git_config_dir:
+        git_config_dir = git_config_dir.replace("~", HOME_DIR)
 
     cli_dict = {'package': {'managers': {OS[0]: pkg_mngrs},
                             'groups': pkg_groups},
                 'log': {'file': log_file, 'level': log_level},
                 'remote_hosts': remote_host,
                 'firewall': firewall,
                 'steps': {OS[0]: steps},
                 'dot_files': {'overwrite': overwrite,
-                              'git_url': repo, 'git_branch': git_branch}}
+                              'git_url': repo,
+                              'git_branch': git_branch,
+                              'git_config_dir': git_config_dir}}
 
     log.debug(f"cli_dict is:\n{cli_dict}\n")
 
     if OS[0] == 'Darwin':
         try:
             USR_CONFIG_FILE['package']['managers'].pop('Linux')
             USR_CONFIG_FILE['steps'].pop('Linux')
```

### Comparing `onboardme-1.4.1/onboardme/firewall.py` & `onboardme-1.5.0/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.1/onboardme/help_text.py` & `onboardme-1.5.0/onboardme/help_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,33 +37,28 @@
     dot_file_url = '[meta]https://github.com/jessebot/dot_files[/meta]'
     step_choices = pretty_choices(STEPS)
     pkg_mngr_choices = pretty_choices(PKG_MNGRS)
     logging_choices = pretty_choices(['debug', 'info', 'warn', 'error'])
     pkg_group_choices = pretty_choices(DEFAULT_PKG_GROUPS + OPT_PKG_GROUPS)
 
     return {
-        'log_level':
-        f'Logging level. {logging_choices}\nDefault: [meta]warn[/meta]',
-
-        'log_file':
-        'Full path to file to log to, if set.',
-
-        'quiet':
-        "unstable. Don't output to stdout. ",
-
         'steps':
         f'[b]Only[/b] run [meta]STEP[/] in the script.\n{step_choices}\nExampl'
         'e: [switch]-s[/] [meta]dot_files[/] [switch]-s[/] [meta]packages',
 
         'git_url':
         f'A git repo URL for your dot files. Default: {dot_file_url}',
 
         'git_branch':
         'Branch to use for the git repo url. Default: main',
 
+        'git_config_dir':
+        'Directory to store the git configuration for your dot files. '
+        'Default: ~/.config/dot_files',
+
         'overwrite':
         '[b]Overwrites[/b] existing dot files with files from configured '
         "[option]--git_url[/option] repo. If you've set overwrite: true in "
         'your config, then --overwrite on the command line will act as a '
         'toggle, so it will NOT overwrite your dot files.',
 
         'pkg_managers':
@@ -80,15 +75,25 @@
         'remote_host':
         'Setup SSH on a random port & add [meta]IP_ADDR[/] to firewall',
 
         'firewall':
         'Setup iptables (on [i]linux[/] only).',
 
         'version':
-        f'Print the version of onboardme ({VERSION})'
+        f'Print the version of onboardme ({VERSION})',
+
+        'log_level':
+        f'Logging level. {logging_choices}\nDefault: [meta]warn[/meta]',
+
+        'log_file':
+        'Full path to file to log to, if set.',
+
+        'quiet':
+        "unstable. Don't output to stdout. "
+
     }
 
 
 class RichCommand(click.Command):
     """
     Override Clicks help with a Richer version.
 
@@ -123,16 +128,16 @@
         console.print("\n[b]Usage[/]:  [royal_blue1]onboardme[/] " +
                       "[cornflower_blue][OPTIONS]\n")
 
         options_table = Table(highlight=True, box=None, show_header=False,
                               row_styles=["", "dim"],
                               padding=(1, 1, 0, 0))
 
-        # this used to be self.get_params(ctx)[1:] and I don't know why
-        for param in self.get_params(ctx):
+        # this used to be self.get_params(ctx)[1:] to have only one hidden option
+        for param in self.get_params(ctx)[2:]:
 
             if len(param.opts) == 2:
                 opt1 = highlighter(param.opts[1])
                 opt2 = highlighter(param.opts[0])
             else:
                 opt2 = highlighter(param.opts[0])
                 opt1 = Text("")
```

### Comparing `onboardme-1.4.1/onboardme/ide_setup.py` & `onboardme-1.5.0/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.1/onboardme/misc.py` & `onboardme-1.5.0/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.1/onboardme/pkg_management.py` & `onboardme-1.5.0/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.1/onboardme/subproc.py` & `onboardme-1.5.0/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.1/onboardme/sudo_setup.py` & `onboardme-1.5.0/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.4.1/pyproject.toml` & `onboardme-1.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.4.1"
+version       = "1.5.0"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
@@ -15,16 +15,15 @@
                  "Programming Language :: Python :: 3.11",
                  "Operating System :: MacOS :: MacOS X",
                  "Operating System :: POSIX :: Linux",
                  "Intended Audience :: End Users/Desktop",
                  "Topic :: System :: Installation/Setup",
                  "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)"]
 packages      = [{include = "onboardme"}]
-include       = ["onboardme/scripts/update_apt_sources.sh",
-                 "onboardme/scripts/get_apt_list.sh"]
+include       = ["onboardme/scripts/update_apt_sources.sh"]
 
 [tool.poetry.dependencies]
 python              = "^3.11"
 click               = "^8.1"
 rich                = "^13.4"
 PyYAML              = "^6.0"
 GitPython           = "^3.1"
```

### Comparing `onboardme-1.4.1/PKG-INFO` & `onboardme-1.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: onboardme
-Version: 1.4.1
-Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
-Home-page: http://github.com/jessebot/onboardme
-License: AGPL-3.0-or-later
-Keywords: onboardme,onboarding,desktop-setup,development-environment
-Author: Jesse Hitch
-Author-email: jessebot@linux.com
-Requires-Python: >=3.11,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: System :: Installation/Setup
-Requires-Dist: GitPython (>=3.1,<4.0)
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: click (>=8.1,<9.0)
-Requires-Dist: rich (>=13.4,<14.0)
-Requires-Dist: wget (>=3.2,<4.0)
-Requires-Dist: xdg-base-dirs (>=6.0,<7.0)
-Project-URL: Bug Tracker, http://github.com/jessebot/onboardme/issues
-Project-URL: Documentation, https://jessebot.github.io/onboardme/onboardme
-Project-URL: Repository, http://github.com/jessebot/onboardme
-Description-Content-Type: text/markdown
-
 <h1 align="center">
   <img
     src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png"
     height="30"
     width="0px"
   />
   💻 onboard<i>me</i>
@@ -91,15 +62,19 @@
 If you haven't already made the switch from Vim to [NeoVim], you can try out NeoVim today with `onboardme` :D We used to support both neovim _and_ vim, but these days none of the primary developers of this repo use pure vim anymore, so we can't ensure it's up to standards. All of your knowledge from vim is still helpful in neovim though, and we highly recommend switching as neovim has a lot more features and a very active plugin community :) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/doc/user/nvim.html#nvim-from-vim). 
 
 </details>
 
 <details>
   <summary><h4>Easy <code>yaml</code> config files using XDG Base Directory Spec<h4></summary>
 
-We use use [XDG Base Directory Spec] for [config files](#configuration) so you always know where they are :)
+We use use [XDG Base Directory Spec] for config files, so you always know where they are :)
+
+Config files are in `$XDG_CONFIG_HOME/onboardme/`, <sub>or `~/.config/onboardme/` if `$XDG_CONFIG_HOME` is not defined</sub>.
+
+Learn more about configuration in the [config docs](https://jessebot.github.io/onboardme/onboardme/getting-started).
 
 </details>
 
 <details>
   <summary><h4>Docker image for an on-the-go dev workspace<h4></summary>
 
 The docker image is built nightly, and on push to `main` via GHA. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
@@ -220,21 +195,23 @@
 ```
 
 ## Using the Docker image
 
 Read more about our docker tags and how to use them at [jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme) on DockerHub.
 
 # Usage
+Learn more about configuration in the [config docs](https://jessebot.github.io/onboardme/onboardme/getting-started), but by default you can get started with:
 
-_Now_ you can run `onboardme` 🎉 
 ```bash
 # this will display the help text for onboardme
 onboardme --help
 
-# Running this won't overwrite any existing dot files, but it may add new ones.
+# Running this won't overwrite any existing dot files, but it may add new ones
+# and it may install new packages. Don't run this till you've looked at the files
+# in ~/.config/onboardme/
 onboardme
 ```
 
 From here, if you want to *completely wipe your existing dot files* for a fresh start with with `onboardme`, you can run:
 ```bash
 # WARNING: This will overwrite your local dotfiles, including your .bashrc and .bash_profile
 # can also be done with: onboardme -O
@@ -246,113 +223,14 @@
 ### Upgrades
 If you're on python 3.11, you should be able to do:
 
 ```bash
 pip3.11 install --upgrade onboardme
 ```
 
-### Configuration
-onboardme has lots of CLI options, but you can also use config files. You have to create these files for the time being.
-
-Config files are in `$XDG_CONFIG_HOME/onboardme/`, <sub>or `~/.config/onboardme/` if `$XDG_CONFIG_HOME` is not defined</sub>.
-
-| Config File                               |        Description                                  |
-|:------------------------------------------|:----------------------------------------------------|
-| `$XDG_CONFIG_HOME/onboardme/config.yml`   | For step configuration to run either all steps, or just a subset. | 
-| `$XDG_CONFIG_HOME/onboardme/packages.yml` | For adding packages with different package managers |
-
-Examples:
-<details>
-<summary><code>~/.config/onboardme/config.yml</code></summary>
-
-```yaml
----
-# ______________________________________________________________ #
-#         Config file for the onboardme cli command.             #
-# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
-#  - If this files exists as: ~/.config/onboardme/config.yaml    #
-#    then its loaded instead of the default config               #
-# -------------------------------------------------------------- #
-
-
-log:
-  # Full path to a file you'd like to log to. Creates file if it doesn't exist
-  file: ""
-  # what level of logs to output (debug, info, warn, error)
-  level: "warn"
-
-# steps refer to a specific function in the list of functions we run
-steps:
-  # these are mac specific steps
-  Darwin:
-    - dot_files
-    - packages
-    - font_setup
-    - neovim_setup
-    - sudo_setup
-  # these are linux specific steps
-  Linux:
-    - dot_files
-    - packages
-    - font_setup
-    - neovim_setup
-    - group_setup
-
-dot_files:
-  # personal git repo URL for your dot files, defaults to jessebot/dot_files
-  git_url: "https://github.com/jessebot/dot_files.git"
-  # the branch to use for the git repo above, defaults to main
-  git_branch: "main"
-  # !!CAREFUL: runs a `git reset --hard`, which will overwite/delete files in 
-  # $HOME that conflict with the above defined git repo url and branch.
-  # You should run the following to get the files that would be overwritten:
-  # onboardme -s dot_files
-  # if set to true, then using onboardme -O will toggle it back to false
-  overwrite: false
-
-# This is the basic package config.
-package:
-  # Remove any of the below pkg managers to only run the remaining pkg managers
-  managers:
-    # macOS specific steps
-    Darwin:
-      - brew
-      - pip3.11
-    # Debian/Ubuntu specific steps
-    Linux:
-      - apt
-      - brew
-      - pip3.11
-      - flatpak
-      - snap
-  # list of extra existing packages groups to install
-  groups:
-    default:
-      # basic tui stuff to have a nice time in the terminal :)
-      - default
-    # move these package.groups.default to always install them
-    optional:
-      # setting up more python data science specific tooling
-      - data_science
-      # kubernetes and docker tools
-      - devops
-      # gaming always installs gui
-      - gaming
-      # freetube and other gui applications
-      - gui
-      # this configures neomutt and offlineimap
-      - mail
-      # sets up useful music tui stuff for spotify and youtube
-      - music
-      # things like zoom and slack
-      - work
-```
-
-</details>
-
 ## Under the Hood
 Made and tested for these operating systems:
 
 [![Tested on Ventura 13.4 with a 13-inch M1 Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en)
 [![Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://www.debian.org/)
 [![Tested only on ubuntu servers](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/)
 
@@ -419,8 +297,7 @@
 [default packages]: https://github.com/jessebot/dot_files/blob/main/.config/onboardme/packages.yml "default installed packages for onboardme"
 
 <!-- external link references -->
 [dot files]: https://en.wikipedia.org/wiki/Hidden_file_and_hidden_directory#Unix_and_Unix-like_environments "wiki entry for dot file explanation"
 [XDG Base Directory Spec]: https://specifications.freedesktop.org/basedir-spec/latest/ar01s03.html
 [NeoVim]: https://neovim.io/ "neovim, vim improved"
 [lazy.nvim]: https://github.com/folke/lazy.nvim "lazy.nvim, a plugin manager for neovim"
-
```

