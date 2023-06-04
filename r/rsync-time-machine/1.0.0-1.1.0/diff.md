# Comparing `tmp/rsync-time-machine-1.0.0.tar.gz` & `tmp/rsync-time-machine-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsync-time-machine-1.0.0.tar", last modified: Sat May 13 21:59:58 2023, max compression
+gzip compressed data, was "rsync-time-machine-1.1.0.tar", last modified: Sun Jun  4 20:13:32 2023, max compression
```

## Comparing `rsync-time-machine-1.0.0.tar` & `rsync-time-machine-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-05-13 21:59:58.634504 rsync-time-machine-1.0.0/
--rw-r--r--   0 basnijholt   (501) staff       (20)    11357 2023-05-10 17:54:27.000000 rsync-time-machine-1.0.0/LICENSE
--rw-r--r--   0 basnijholt   (501) staff       (20)     9076 2023-05-13 21:59:58.634089 rsync-time-machine-1.0.0/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)     8644 2023-05-13 21:52:49.000000 rsync-time-machine-1.0.0/README.md
--rw-r--r--   0 basnijholt   (501) staff       (20)     2171 2023-05-13 21:55:13.000000 rsync-time-machine-1.0.0/pyproject.toml
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-05-13 21:59:58.632925 rsync-time-machine-1.0.0/rsync_time_machine.egg-info/
--rw-r--r--   0 basnijholt   (501) staff       (20)     9076 2023-05-13 21:59:58.000000 rsync-time-machine-1.0.0/rsync_time_machine.egg-info/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)      326 2023-05-13 21:59:58.000000 rsync-time-machine-1.0.0/rsync_time_machine.egg-info/SOURCES.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)        1 2023-05-13 21:59:58.000000 rsync-time-machine-1.0.0/rsync_time_machine.egg-info/dependency_links.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       63 2023-05-13 21:59:58.000000 rsync-time-machine-1.0.0/rsync_time_machine.egg-info/entry_points.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       54 2023-05-13 21:59:58.000000 rsync-time-machine-1.0.0/rsync_time_machine.egg-info/requires.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       19 2023-05-13 21:59:58.000000 rsync-time-machine-1.0.0/rsync_time_machine.egg-info/top_level.txt
--rwxr-xr-x   0 basnijholt   (501) staff       (20)    26482 2023-05-13 17:57:26.000000 rsync-time-machine-1.0.0/rsync_time_machine.py
--rw-r--r--   0 basnijholt   (501) staff       (20)       38 2023-05-13 21:59:58.634559 rsync-time-machine-1.0.0/setup.cfg
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-05-13 21:59:58.633419 rsync-time-machine-1.0.0/tests/
--rw-r--r--   0 basnijholt   (501) staff       (20)    14297 2023-05-13 17:57:26.000000 rsync-time-machine-1.0.0/tests/test_app.py
+drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-06-04 20:13:32.189652 rsync-time-machine-1.1.0/
+-rw-r--r--   0 basnijholt   (501) staff       (20)    11357 2023-05-10 17:54:27.000000 rsync-time-machine-1.1.0/LICENSE
+-rw-r--r--   0 basnijholt   (501) staff       (20)    12892 2023-06-04 20:13:32.189329 rsync-time-machine-1.1.0/PKG-INFO
+-rw-r--r--   0 basnijholt   (501) staff       (20)    12460 2023-06-04 20:11:35.000000 rsync-time-machine-1.1.0/README.md
+-rw-r--r--   0 basnijholt   (501) staff       (20)     2251 2023-05-28 19:34:35.000000 rsync-time-machine-1.1.0/pyproject.toml
+drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-06-04 20:13:32.184585 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/
+-rw-r--r--   0 basnijholt   (501) staff       (20)    12892 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/PKG-INFO
+-rw-r--r--   0 basnijholt   (501) staff       (20)      326 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)        1 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)       63 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/entry_points.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)       54 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/requires.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)       19 2023-06-04 20:13:32.000000 rsync-time-machine-1.1.0/rsync_time_machine.egg-info/top_level.txt
+-rwxr-xr-x   0 basnijholt   (501) staff       (20)    28867 2023-06-04 20:11:35.000000 rsync-time-machine-1.1.0/rsync_time_machine.py
+-rw-r--r--   0 basnijholt   (501) staff       (20)       38 2023-06-04 20:13:32.189724 rsync-time-machine-1.1.0/setup.cfg
+drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-06-04 20:13:32.188016 rsync-time-machine-1.1.0/tests/
+-rw-r--r--   0 basnijholt   (501) staff       (20)    14904 2023-05-28 20:38:17.000000 rsync-time-machine-1.1.0/tests/test_app.py
```

### Comparing `rsync-time-machine-1.0.0/LICENSE` & `rsync-time-machine-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rsync-time-machine-1.0.0/PKG-INFO` & `rsync-time-machine-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-Metadata-Version: 2.1
-Name: rsync-time-machine
-Version: 1.0.0
-Summary: rsync-time-machine.py is a wrapper around rsync to make it easier to create and maintain Time Machine style backups.
-Author-email: Bas Nijholt <bas@nijho.lt>
-Project-URL: Homepage, https://github.com/basnijholt/rsync-time-machine.py
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE
-
 # Rsync Time Machine 🕰️💾
 
+![Build](https://github.com/basnijholt/rsync-time-machine.py/actions/workflows/pytest.yml/badge.svg)
+[![Coverage](https://img.shields.io/codecov/c/github/basnijholt/rsync-time-machine.py)](https://codecov.io/gh/basnijholt/rsync-time-machine.py)
+[![GitHub](https://img.shields.io/github/stars/basnijholt/rsync-time-machine.py.svg?style=social)](https://github.com/basnijholt/rsync-time-machine.py/stargazers)
+[![PyPI](https://img.shields.io/pypi/v/rsync-time-machine.svg)](https://pypi.python.org/pypi/rsync-time-machine)
+[![License](https://img.shields.io/github/license/basnijholt/rsync-time-machine.py)](https://github.com/basnijholt/rsync-time-machine.py/blob/main/LICENSE)
+[![Downloads](https://img.shields.io/pypi/dm/rsync-time-machine)](https://pypi.python.org/pypi/rsync-time-machine)
+![Open Issues](https://img.shields.io/github/issues-raw/basnijholt/rsync-time-machine.py)
+
 Introducing `rsync-time-machine.py` - a Python port of the [`rsync-time-backup`](https://github.com/laurent22/rsync-time-backup) script, offering Time Machine-style backups using rsync. It creates incremental backups of files and directories to the destination of your choice. The backups are structured in a way that makes it easy to recover any file at any point in time. 🚀
 
 It works on Linux, macOS, and Windows (via WSL or Cygwin). The main advantage over Time Machine is flexibility, as it can backup from/to any filesystem and works on any platform. You can also backup to a Truecrypt drive without any problem. 😃
 
 `rsync-time-machine.py` is fully tested, has no external dependencies (only Python ≥3.7 🐍), is fully compatible with [`rsync-time-backup`](https://github.com/laurent22/rsync-time-backup), offers pretty terminal output, and is fully typed! 🎉
 
 <details><summary><b><u>[ToC]</u></b> 📚</summary>
@@ -29,14 +25,15 @@
 - [:bulb: Examples](#bulb-examples)
 - [:calendar: Backup Expiration Logic](#calendar-backup-expiration-logic)
 - [:page_facing_up: Exclusion File](#page_facing_up-exclusion-file)
 - [:lock: Built-in Lock](#lock-built-in-lock)
 - [:gear: Rsync Options](#gear-rsync-options)
 - [:no_entry_sign: No Automatic Backup Expiration](#no_entry_sign-no-automatic-backup-expiration)
 - [:arrows_counterclockwise: How to Restore](#arrows_counterclockwise-how-to-restore)
+- [:star: Featured on](#star-featured-on)
 - [:heart: Support and Contributions](#heart-support-and-contributions)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 </details>
 
 ## :star2: Features
@@ -68,24 +65,26 @@
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```bash
 usage: rsync-time-machine [-h] [-p PORT] [-i ID_RSA] [--rsync-get-flags]
                           [--rsync-set-flags RSYNC_SET_FLAGS]
                           [--rsync-append-flags RSYNC_APPEND_FLAGS]
                           [--log-dir LOG_DIR] [--strategy STRATEGY]
-                          [--no-auto-expire] [--allow-host-only] [-v]
+                          [--no-auto-expire] [--allow-host-only]
+                          [--exclude-from EXCLUDE_FROM] [-v]
                           src_folder dest_folder [exclusion_file]
 
 A script for creating and managing time-stamped backups using rsync.
 
 positional arguments:
   src_folder            Source folder for backup. Format: [USER@HOST:]SOURCE
   dest_folder           Destination folder for backup. Format:
                         [USER@HOST:]DESTINATION
-  exclusion_file        Path to the file containing exclude patterns.
+  exclusion_file        Path to the file containing exclude patterns. Cannot
+                        be used together with `--exclude-from`.
 
 options:
   -h, --help            show this help message and exit
   -p PORT, --port PORT  SSH port.
   -i ID_RSA, --id_rsa ID_RSA
                         Specify the private ssh key to use.
   --rsync-get-flags     Display the default rsync flags that are used for
@@ -112,15 +111,20 @@
                         for specifying SSH connections. When this flag is
                         used, it allows for the 'HOST' pattern without a
                         specified user. This is useful if you want to use
                         configurations from the `.ssh/config` file or rely on
                         the current username. Note: this option will not
                         enforce SSH usage, it only broadens the accepted input
                         formats.
-  -v, --verbose         Enable verbose output.
+  --exclude-from EXCLUDE_FROM
+                        Path to the file containing exclude patterns.
+                        Alternative to the positional `exclusion_file`. Not to
+                        be used with `exclusion_file`.
+  -v, --verbose         Enable verbose output. This will slow down the backup
+                        process (in simple tests by 2x).
 ```
 
 <!-- OUTPUT:END -->
 
 Please refer to the original [`rsync-time-backup`](https://github.com/laurent22/rsync-time-backup) README for a list of options, as they have been preserved in the Python port.
 
 ## :hammer_and_wrench: Installation
@@ -160,14 +164,53 @@
 
 Backup sets are automatically deleted following a simple expiration strategy defined with the `--strategy` flag. The default strategy is `1:1 30:7 365:30`. Please see the original README for a detailed explanation.
 
 ## :page_facing_up: Exclusion File
 
 An optional exclude file can be provided as a third parameter, compatible with the `--exclude-from` parameter of rsync.
 
+The `--exclude-from` option in `rsync-time-machine.py` allows you to exclude specific files or directories from the backup process. You can provide an exclusion file containing patterns for files or directories that should be excluded.
+
+<details>
+<summary>📖🔽 Click here to expand the docs on <code>--exclude-from</code> 🔽📖</summary>
+
+Here's how to use the `--exclude-from` feature in `rsync-time-machine.py`:
+
+1. Create a text file named `exclusion_file.txt` (or any other name you prefer) in your preferred location.
+2. Add the exclusion patterns to the file, one pattern per line. Patterns can be literal strings, wildcards, or character ranges.
+3. Save the file.
+
+To use this exclusion file while performing a backup with `rsync-time-machine.py`, include it as the third positional argument in your command (or with `--exclude-from exclusion_file.txt`). For example:
+
+```bash
+rsync-time-machine.py /home /mnt/backup_drive exclusion_file.txt
+```
+
+In this example, `/home` is the source folder, `/mnt/backup_drive` is the destination folder, and `exclusion_file.txt` contains the exclude patterns.
+
+Here's a sample `exclusion_file.txt`:
+
+```
++ /home/.fileA
+- /home/.*
+- /home/junk/
+```
+
+In this example:
+
+- `+ /home/.fileA`: Include the file `.fileA` from the `home` directory.
+- `- /home/.*`: Exclude all hidden files (files starting with a dot) from the `home` directory.
+- `- /home/junk/`: Exclude the entire `junk` directory from the `home` directory.
+
+Remember that the order of patterns matters, as rsync reads the file top-down and acts on the first matching pattern it encounters.
+
+See [this tutorial](https://web.archive.org/web/20230126121643/https://sites.google.com/site/rsync2u/home/rsync-tutorial/the-exclude-from-option) for more information.
+
+</details>
+
 ## :lock: Built-in Lock
 
 The script is designed so that only one backup operation can be active for a given directory, avoiding conflicts.
 
 ## :gear: Rsync Options
 
 To display, add, or remove rsync options, use the `--rsync-get-flags`, `--rsync-append-flags`, or `--rsync-set-flags` options.
@@ -184,12 +227,18 @@
 rsync -aP /path/to/last/backup/ /path/to/restore/to/
 ```
 
 Consider using the `--dry-run` option to check what exactly is going to be copied. If you want to delete files that exist in the destination but not in the backup, use the `--delete` option. Be extra cautious when using this option to avoid data loss.
 
 You can also restore files using any file explorer, including Finder on macOS or the command line.
 
+## :star: Featured on
+
+- the Real Python podcast: [Episode 158: Building Python CI With Docker & Applying for a Hacker Initiative Grant @ 00:26:28](https://realpython.com/podcasts/rpp/158/#t=1588)
+- Y Combinator Hacker News: [Python Port of 600 Line Bash Script: rsync-time-machine.py for Rsync Backups](https://news.ycombinator.com/item?id=35933238) (self-posted)
+- Reddit /rpython: [Ported a popular (untested) 600+ Line Bash Script 📜 to Python 🐍: Introducing rsync-time-machine.py for Time Machine-Style Backups Using Rsync 🔄⏰](https://www.reddit.com/r/Python/comments/13gtmz2/ported_a_popular_untested_600_line_bash_script_to/) (self-posted)
+
 ## :heart: Support and Contributions
 
 We appreciate your feedback and contributions! If you encounter any issues or have suggestions for improvements, please file an issue on the GitHub repository. We also welcome pull requests for bug fixes or new features.
 
 Happy backing up! 💾🕰️🎉
```

### Comparing `rsync-time-machine-1.0.0/README.md` & `rsync-time-machine-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,29 @@
+Metadata-Version: 2.1
+Name: rsync-time-machine
+Version: 1.1.0
+Summary: rsync-time-machine.py is a wrapper around rsync to make it easier to create and maintain Time Machine style backups.
+Author-email: Bas Nijholt <bas@nijho.lt>
+Project-URL: Homepage, https://github.com/basnijholt/rsync-time-machine.py
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: docs
+License-File: LICENSE
+
 # Rsync Time Machine 🕰️💾
 
+![Build](https://github.com/basnijholt/rsync-time-machine.py/actions/workflows/pytest.yml/badge.svg)
+[![Coverage](https://img.shields.io/codecov/c/github/basnijholt/rsync-time-machine.py)](https://codecov.io/gh/basnijholt/rsync-time-machine.py)
+[![GitHub](https://img.shields.io/github/stars/basnijholt/rsync-time-machine.py.svg?style=social)](https://github.com/basnijholt/rsync-time-machine.py/stargazers)
+[![PyPI](https://img.shields.io/pypi/v/rsync-time-machine.svg)](https://pypi.python.org/pypi/rsync-time-machine)
+[![License](https://img.shields.io/github/license/basnijholt/rsync-time-machine.py)](https://github.com/basnijholt/rsync-time-machine.py/blob/main/LICENSE)
+[![Downloads](https://img.shields.io/pypi/dm/rsync-time-machine)](https://pypi.python.org/pypi/rsync-time-machine)
+![Open Issues](https://img.shields.io/github/issues-raw/basnijholt/rsync-time-machine.py)
+
 Introducing `rsync-time-machine.py` - a Python port of the [`rsync-time-backup`](https://github.com/laurent22/rsync-time-backup) script, offering Time Machine-style backups using rsync. It creates incremental backups of files and directories to the destination of your choice. The backups are structured in a way that makes it easy to recover any file at any point in time. 🚀
 
 It works on Linux, macOS, and Windows (via WSL or Cygwin). The main advantage over Time Machine is flexibility, as it can backup from/to any filesystem and works on any platform. You can also backup to a Truecrypt drive without any problem. 😃
 
 `rsync-time-machine.py` is fully tested, has no external dependencies (only Python ≥3.7 🐍), is fully compatible with [`rsync-time-backup`](https://github.com/laurent22/rsync-time-backup), offers pretty terminal output, and is fully typed! 🎉
 
 <details><summary><b><u>[ToC]</u></b> 📚</summary>
@@ -17,14 +37,15 @@
 - [:bulb: Examples](#bulb-examples)
 - [:calendar: Backup Expiration Logic](#calendar-backup-expiration-logic)
 - [:page_facing_up: Exclusion File](#page_facing_up-exclusion-file)
 - [:lock: Built-in Lock](#lock-built-in-lock)
 - [:gear: Rsync Options](#gear-rsync-options)
 - [:no_entry_sign: No Automatic Backup Expiration](#no_entry_sign-no-automatic-backup-expiration)
 - [:arrows_counterclockwise: How to Restore](#arrows_counterclockwise-how-to-restore)
+- [:star: Featured on](#star-featured-on)
 - [:heart: Support and Contributions](#heart-support-and-contributions)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 </details>
 
 ## :star2: Features
@@ -56,24 +77,26 @@
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```bash
 usage: rsync-time-machine [-h] [-p PORT] [-i ID_RSA] [--rsync-get-flags]
                           [--rsync-set-flags RSYNC_SET_FLAGS]
                           [--rsync-append-flags RSYNC_APPEND_FLAGS]
                           [--log-dir LOG_DIR] [--strategy STRATEGY]
-                          [--no-auto-expire] [--allow-host-only] [-v]
+                          [--no-auto-expire] [--allow-host-only]
+                          [--exclude-from EXCLUDE_FROM] [-v]
                           src_folder dest_folder [exclusion_file]
 
 A script for creating and managing time-stamped backups using rsync.
 
 positional arguments:
   src_folder            Source folder for backup. Format: [USER@HOST:]SOURCE
   dest_folder           Destination folder for backup. Format:
                         [USER@HOST:]DESTINATION
-  exclusion_file        Path to the file containing exclude patterns.
+  exclusion_file        Path to the file containing exclude patterns. Cannot
+                        be used together with `--exclude-from`.
 
 options:
   -h, --help            show this help message and exit
   -p PORT, --port PORT  SSH port.
   -i ID_RSA, --id_rsa ID_RSA
                         Specify the private ssh key to use.
   --rsync-get-flags     Display the default rsync flags that are used for
@@ -100,15 +123,20 @@
                         for specifying SSH connections. When this flag is
                         used, it allows for the 'HOST' pattern without a
                         specified user. This is useful if you want to use
                         configurations from the `.ssh/config` file or rely on
                         the current username. Note: this option will not
                         enforce SSH usage, it only broadens the accepted input
                         formats.
-  -v, --verbose         Enable verbose output.
+  --exclude-from EXCLUDE_FROM
+                        Path to the file containing exclude patterns.
+                        Alternative to the positional `exclusion_file`. Not to
+                        be used with `exclusion_file`.
+  -v, --verbose         Enable verbose output. This will slow down the backup
+                        process (in simple tests by 2x).
 ```
 
 <!-- OUTPUT:END -->
 
 Please refer to the original [`rsync-time-backup`](https://github.com/laurent22/rsync-time-backup) README for a list of options, as they have been preserved in the Python port.
 
 ## :hammer_and_wrench: Installation
@@ -148,14 +176,53 @@
 
 Backup sets are automatically deleted following a simple expiration strategy defined with the `--strategy` flag. The default strategy is `1:1 30:7 365:30`. Please see the original README for a detailed explanation.
 
 ## :page_facing_up: Exclusion File
 
 An optional exclude file can be provided as a third parameter, compatible with the `--exclude-from` parameter of rsync.
 
+The `--exclude-from` option in `rsync-time-machine.py` allows you to exclude specific files or directories from the backup process. You can provide an exclusion file containing patterns for files or directories that should be excluded.
+
+<details>
+<summary>📖🔽 Click here to expand the docs on <code>--exclude-from</code> 🔽📖</summary>
+
+Here's how to use the `--exclude-from` feature in `rsync-time-machine.py`:
+
+1. Create a text file named `exclusion_file.txt` (or any other name you prefer) in your preferred location.
+2. Add the exclusion patterns to the file, one pattern per line. Patterns can be literal strings, wildcards, or character ranges.
+3. Save the file.
+
+To use this exclusion file while performing a backup with `rsync-time-machine.py`, include it as the third positional argument in your command (or with `--exclude-from exclusion_file.txt`). For example:
+
+```bash
+rsync-time-machine.py /home /mnt/backup_drive exclusion_file.txt
+```
+
+In this example, `/home` is the source folder, `/mnt/backup_drive` is the destination folder, and `exclusion_file.txt` contains the exclude patterns.
+
+Here's a sample `exclusion_file.txt`:
+
+```
++ /home/.fileA
+- /home/.*
+- /home/junk/
+```
+
+In this example:
+
+- `+ /home/.fileA`: Include the file `.fileA` from the `home` directory.
+- `- /home/.*`: Exclude all hidden files (files starting with a dot) from the `home` directory.
+- `- /home/junk/`: Exclude the entire `junk` directory from the `home` directory.
+
+Remember that the order of patterns matters, as rsync reads the file top-down and acts on the first matching pattern it encounters.
+
+See [this tutorial](https://web.archive.org/web/20230126121643/https://sites.google.com/site/rsync2u/home/rsync-tutorial/the-exclude-from-option) for more information.
+
+</details>
+
 ## :lock: Built-in Lock
 
 The script is designed so that only one backup operation can be active for a given directory, avoiding conflicts.
 
 ## :gear: Rsync Options
 
 To display, add, or remove rsync options, use the `--rsync-get-flags`, `--rsync-append-flags`, or `--rsync-set-flags` options.
@@ -172,12 +239,18 @@
 rsync -aP /path/to/last/backup/ /path/to/restore/to/
 ```
 
 Consider using the `--dry-run` option to check what exactly is going to be copied. If you want to delete files that exist in the destination but not in the backup, use the `--delete` option. Be extra cautious when using this option to avoid data loss.
 
 You can also restore files using any file explorer, including Finder on macOS or the command line.
 
+## :star: Featured on
+
+- the Real Python podcast: [Episode 158: Building Python CI With Docker & Applying for a Hacker Initiative Grant @ 00:26:28](https://realpython.com/podcasts/rpp/158/#t=1588)
+- Y Combinator Hacker News: [Python Port of 600 Line Bash Script: rsync-time-machine.py for Rsync Backups](https://news.ycombinator.com/item?id=35933238) (self-posted)
+- Reddit /rpython: [Ported a popular (untested) 600+ Line Bash Script 📜 to Python 🐍: Introducing rsync-time-machine.py for Time Machine-Style Backups Using Rsync 🔄⏰](https://www.reddit.com/r/Python/comments/13gtmz2/ported_a_popular_untested_600_line_bash_script_to/) (self-posted)
+
 ## :heart: Support and Contributions
 
 We appreciate your feedback and contributions! If you encounter any issues or have suggestions for improvements, please file an issue on the GitHub repository. We also welcome pull requests for bug fixes or new features.
 
 Happy backing up! 💾🕰️🎉
```

### Comparing `rsync-time-machine-1.0.0/pyproject.toml` & `rsync-time-machine-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     "D402",    # First line should not be the function's signature
     "PLW0603", # Using the global statement to update `X` is discouraged
     "D401",    # First line of docstring should be in imperative mood
     "SLF001",  # Private member accessed
     "PTH",     # Use pathlib.Path
     "DTZ005",  # The use of `datetime.datetime.now()` without `tz` argument is not allowed
     "PLR0913", # Too many arguments to function call
+    "S602",    # `subprocess` call with `shell=True` identified, security issue
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["SLF001"]
 ".github/*" = ["INP001"]
 
 [tool.ruff.mccabe]
```

### Comparing `rsync-time-machine-1.0.0/rsync_time_machine.egg-info/PKG-INFO` & `rsync-time-machine-1.1.0/rsync_time_machine.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: rsync-time-machine
-Version: 1.0.0
+Version: 1.1.0
 Summary: rsync-time-machine.py is a wrapper around rsync to make it easier to create and maintain Time Machine style backups.
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/rsync-time-machine.py
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 # Rsync Time Machine 🕰️💾
 
+![Build](https://github.com/basnijholt/rsync-time-machine.py/actions/workflows/pytest.yml/badge.svg)
+[![Coverage](https://img.shields.io/codecov/c/github/basnijholt/rsync-time-machine.py)](https://codecov.io/gh/basnijholt/rsync-time-machine.py)
+[![GitHub](https://img.shields.io/github/stars/basnijholt/rsync-time-machine.py.svg?style=social)](https://github.com/basnijholt/rsync-time-machine.py/stargazers)
+[![PyPI](https://img.shields.io/pypi/v/rsync-time-machine.svg)](https://pypi.python.org/pypi/rsync-time-machine)
+[![License](https://img.shields.io/github/license/basnijholt/rsync-time-machine.py)](https://github.com/basnijholt/rsync-time-machine.py/blob/main/LICENSE)
+[![Downloads](https://img.shields.io/pypi/dm/rsync-time-machine)](https://pypi.python.org/pypi/rsync-time-machine)
+![Open Issues](https://img.shields.io/github/issues-raw/basnijholt/rsync-time-machine.py)
+
 Introducing `rsync-time-machine.py` - a Python port of the [`rsync-time-backup`](https://github.com/laurent22/rsync-time-backup) script, offering Time Machine-style backups using rsync. It creates incremental backups of files and directories to the destination of your choice. The backups are structured in a way that makes it easy to recover any file at any point in time. 🚀
 
 It works on Linux, macOS, and Windows (via WSL or Cygwin). The main advantage over Time Machine is flexibility, as it can backup from/to any filesystem and works on any platform. You can also backup to a Truecrypt drive without any problem. 😃
 
 `rsync-time-machine.py` is fully tested, has no external dependencies (only Python ≥3.7 🐍), is fully compatible with [`rsync-time-backup`](https://github.com/laurent22/rsync-time-backup), offers pretty terminal output, and is fully typed! 🎉
 
 <details><summary><b><u>[ToC]</u></b> 📚</summary>
@@ -29,14 +37,15 @@
 - [:bulb: Examples](#bulb-examples)
 - [:calendar: Backup Expiration Logic](#calendar-backup-expiration-logic)
 - [:page_facing_up: Exclusion File](#page_facing_up-exclusion-file)
 - [:lock: Built-in Lock](#lock-built-in-lock)
 - [:gear: Rsync Options](#gear-rsync-options)
 - [:no_entry_sign: No Automatic Backup Expiration](#no_entry_sign-no-automatic-backup-expiration)
 - [:arrows_counterclockwise: How to Restore](#arrows_counterclockwise-how-to-restore)
+- [:star: Featured on](#star-featured-on)
 - [:heart: Support and Contributions](#heart-support-and-contributions)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 </details>
 
 ## :star2: Features
@@ -68,24 +77,26 @@
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```bash
 usage: rsync-time-machine [-h] [-p PORT] [-i ID_RSA] [--rsync-get-flags]
                           [--rsync-set-flags RSYNC_SET_FLAGS]
                           [--rsync-append-flags RSYNC_APPEND_FLAGS]
                           [--log-dir LOG_DIR] [--strategy STRATEGY]
-                          [--no-auto-expire] [--allow-host-only] [-v]
+                          [--no-auto-expire] [--allow-host-only]
+                          [--exclude-from EXCLUDE_FROM] [-v]
                           src_folder dest_folder [exclusion_file]
 
 A script for creating and managing time-stamped backups using rsync.
 
 positional arguments:
   src_folder            Source folder for backup. Format: [USER@HOST:]SOURCE
   dest_folder           Destination folder for backup. Format:
                         [USER@HOST:]DESTINATION
-  exclusion_file        Path to the file containing exclude patterns.
+  exclusion_file        Path to the file containing exclude patterns. Cannot
+                        be used together with `--exclude-from`.
 
 options:
   -h, --help            show this help message and exit
   -p PORT, --port PORT  SSH port.
   -i ID_RSA, --id_rsa ID_RSA
                         Specify the private ssh key to use.
   --rsync-get-flags     Display the default rsync flags that are used for
@@ -112,15 +123,20 @@
                         for specifying SSH connections. When this flag is
                         used, it allows for the 'HOST' pattern without a
                         specified user. This is useful if you want to use
                         configurations from the `.ssh/config` file or rely on
                         the current username. Note: this option will not
                         enforce SSH usage, it only broadens the accepted input
                         formats.
-  -v, --verbose         Enable verbose output.
+  --exclude-from EXCLUDE_FROM
+                        Path to the file containing exclude patterns.
+                        Alternative to the positional `exclusion_file`. Not to
+                        be used with `exclusion_file`.
+  -v, --verbose         Enable verbose output. This will slow down the backup
+                        process (in simple tests by 2x).
 ```
 
 <!-- OUTPUT:END -->
 
 Please refer to the original [`rsync-time-backup`](https://github.com/laurent22/rsync-time-backup) README for a list of options, as they have been preserved in the Python port.
 
 ## :hammer_and_wrench: Installation
@@ -160,14 +176,53 @@
 
 Backup sets are automatically deleted following a simple expiration strategy defined with the `--strategy` flag. The default strategy is `1:1 30:7 365:30`. Please see the original README for a detailed explanation.
 
 ## :page_facing_up: Exclusion File
 
 An optional exclude file can be provided as a third parameter, compatible with the `--exclude-from` parameter of rsync.
 
+The `--exclude-from` option in `rsync-time-machine.py` allows you to exclude specific files or directories from the backup process. You can provide an exclusion file containing patterns for files or directories that should be excluded.
+
+<details>
+<summary>📖🔽 Click here to expand the docs on <code>--exclude-from</code> 🔽📖</summary>
+
+Here's how to use the `--exclude-from` feature in `rsync-time-machine.py`:
+
+1. Create a text file named `exclusion_file.txt` (or any other name you prefer) in your preferred location.
+2. Add the exclusion patterns to the file, one pattern per line. Patterns can be literal strings, wildcards, or character ranges.
+3. Save the file.
+
+To use this exclusion file while performing a backup with `rsync-time-machine.py`, include it as the third positional argument in your command (or with `--exclude-from exclusion_file.txt`). For example:
+
+```bash
+rsync-time-machine.py /home /mnt/backup_drive exclusion_file.txt
+```
+
+In this example, `/home` is the source folder, `/mnt/backup_drive` is the destination folder, and `exclusion_file.txt` contains the exclude patterns.
+
+Here's a sample `exclusion_file.txt`:
+
+```
++ /home/.fileA
+- /home/.*
+- /home/junk/
+```
+
+In this example:
+
+- `+ /home/.fileA`: Include the file `.fileA` from the `home` directory.
+- `- /home/.*`: Exclude all hidden files (files starting with a dot) from the `home` directory.
+- `- /home/junk/`: Exclude the entire `junk` directory from the `home` directory.
+
+Remember that the order of patterns matters, as rsync reads the file top-down and acts on the first matching pattern it encounters.
+
+See [this tutorial](https://web.archive.org/web/20230126121643/https://sites.google.com/site/rsync2u/home/rsync-tutorial/the-exclude-from-option) for more information.
+
+</details>
+
 ## :lock: Built-in Lock
 
 The script is designed so that only one backup operation can be active for a given directory, avoiding conflicts.
 
 ## :gear: Rsync Options
 
 To display, add, or remove rsync options, use the `--rsync-get-flags`, `--rsync-append-flags`, or `--rsync-set-flags` options.
@@ -184,12 +239,18 @@
 rsync -aP /path/to/last/backup/ /path/to/restore/to/
 ```
 
 Consider using the `--dry-run` option to check what exactly is going to be copied. If you want to delete files that exist in the destination but not in the backup, use the `--delete` option. Be extra cautious when using this option to avoid data loss.
 
 You can also restore files using any file explorer, including Finder on macOS or the command line.
 
+## :star: Featured on
+
+- the Real Python podcast: [Episode 158: Building Python CI With Docker & Applying for a Hacker Initiative Grant @ 00:26:28](https://realpython.com/podcasts/rpp/158/#t=1588)
+- Y Combinator Hacker News: [Python Port of 600 Line Bash Script: rsync-time-machine.py for Rsync Backups](https://news.ycombinator.com/item?id=35933238) (self-posted)
+- Reddit /rpython: [Ported a popular (untested) 600+ Line Bash Script 📜 to Python 🐍: Introducing rsync-time-machine.py for Time Machine-Style Backups Using Rsync 🔄⏰](https://www.reddit.com/r/Python/comments/13gtmz2/ported_a_popular_untested_600_line_bash_script_to/) (self-posted)
+
 ## :heart: Support and Contributions
 
 We appreciate your feedback and contributions! If you encounter any issues or have suggestions for improvements, please file an issue on the GitHub repository. We also welcome pull requests for bug fixes or new features.
 
 Happy backing up! 💾🕰️🎉
```

### Comparing `rsync-time-machine-1.0.0/rsync_time_machine.py` & `rsync-time-machine-1.1.0/rsync_time_machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 """rsync-time-machine.py: A script for creating and managing time-stamped backups using rsync."""
 import argparse
+import asyncio
 import os
 import re
 import signal
-import subprocess
 import sys
 import time
 from datetime import datetime
 from types import FrameType
-from typing import Dict, List, NamedTuple, Optional, Tuple
+from typing import Callable, Dict, List, NamedTuple, Optional, Tuple
 
 APPNAME = "rsync-time-machine.py"
 VERBOSE = False
 
 
 class SSH(NamedTuple):
     """SSH connection details."""
@@ -23,67 +23,61 @@
     cmd: str
     src_folder: str
     dest_folder: str
     port: str
     id_rsa: Optional[str]
 
 
-def _bold(message: str) -> str:
-    """Return a bolded message."""
-    return f"\033[1m{message}\033[0m"
-
-
-def _green(message: str) -> str:
-    """Return a green message."""
-    return f"\033[92m{message}\033[0m"
-
-
-def _magenta(message: str) -> str:
-    """Return a magenta message."""
-    return f"\033[95m{message}\033[0m"
-
-
-def _yellow(message: str) -> str:
-    """Return a yellow message."""
-    return f"\033[93m{message}\033[0m"
-
-
-def _red(message: str) -> str:
-    """Return a red message."""
-    return f"\033[91m{message}\033[0m"
-
-
-def _orange(message: str) -> str:
-    """Return an orange message."""
-    return f"\033[33m{message}\033[0m"
+COLORS = {
+    "green": "\033[92m",
+    "magenta": "\033[95m",
+    "yellow": "\033[93m",
+    "red": "\033[91m",
+    "orange": "\033[33m",
+}
+
+
+def style(text: str, color: Optional[str] = None, *, bold: bool = False) -> str:
+    """Return styled text."""
+    color_code = COLORS.get(color, "")  # type: ignore[arg-type]
+    bold_code = "\033[1m" if bold else ""
+    reset_code = "\033[0m"
+    return f"{bold_code}{color_code}{text}{reset_code}"
+
+
+def sanitize(s: str) -> str:
+    """Return a sanitized version of the string."""
+    # See https://github.com/basnijholt/rsync-time-machine.py/issues/1
+    return s.encode("utf-8", "surrogateescape").decode("utf-8", "replace")
 
 
 def log(message: str, level: str = "info") -> None:
     """Log a message with the specified log level."""
     levels = {"info": "", "warning": "[WARNING] ", "error": "[ERROR] "}
     output = sys.stderr if level in {"warning", "error"} else sys.stdout
-    print(f"{_bold(APPNAME)}: {levels[level]}{message}", file=output)
+    message = sanitize(message)
+    print(f"{style(APPNAME, bold=True)}: {levels[level]}{message}", file=output)
 
 
 def log_info(message: str) -> None:
     """Log an info message to stdout."""
     log(message, "info")
 
 
 def log_warn(message: str) -> None:
     """Log a warning message to stderr."""
-    log(_orange(message), "warning")
+    log(style(message, "orange"), "warning")
 
 
 def log_error(message: str) -> None:
     """Log an error message to stderr."""
-    log(_red(_bold(message)), "error")
+    log(style(message, "red", bold=True), "error")
 
 
-def log_info_cmd(message: str, ssh: Optional[SSH]) -> None:
+def log_info_cmd(message: str, ssh: Optional[SSH] = None) -> None:
     """Log an info message to stdout, including the SSH command if applicable."""
     if ssh is not None:
         message = f"{ssh.cmd} '{message}'"
     log_info(message)
 
 
 def terminate_script(
@@ -149,23 +143,43 @@
     parser.add_argument(
         "dest_folder",
         help="Destination folder for backup. Format: [USER@HOST:]DESTINATION",
     )
     parser.add_argument(
         "exclusion_file",
         nargs="?",
-        help="Path to the file containing exclude patterns.",
+        help="Path to the file containing exclude patterns."
+        " Cannot be used together with `--exclude-from`.",
+    )
+    parser.add_argument(
+        "--exclude-from",
+        dest="exclude_from",
+        help="Path to the file containing exclude patterns."
+        " Alternative to the positional `exclusion_file`."
+        " Not to be used with `exclusion_file`.",
     )
     parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
-        help="Enable verbose output.",
+        help="Enable verbose output. This will slow down the backup process (in simple tests by 2x).",
     )
-    return parser.parse_args()
+    args = parser.parse_args()
+    # If both positional exclusion_file and optional --exclude-from are provided, raise an error
+    if args.exclusion_file and args.exclude_from:
+        parser.error(
+            "Both positional `exclusion_file` and `--exclude-from` were"
+            " provided. Please use only one of them.",
+        )
+
+    # If --exclude-from is provided, set exclusion_file to its value
+    if args.exclude_from:
+        args.exclusion_file = args.exclude_from
+
+    return args
 
 
 def parse_ssh_pattern(
     folder: str,
     *,
     allow_host_only: bool = False,
 ) -> Optional[Dict[str, str]]:
@@ -180,17 +194,18 @@
         return result
     return None
 
 
 def parse_ssh(
     src_folder: str,
     dest_folder: str,
+    *,
     ssh_port: str,
     id_rsa: Optional[str],
-    allow_host_only: bool,  # noqa: FBT001
+    allow_host_only: bool,
 ) -> Optional[SSH]:
     """Parse the source and destination folders for SSH usage."""
     ssh_src = parse_ssh_pattern(src_folder, allow_host_only=allow_host_only)
     ssh_dest = parse_ssh_pattern(dest_folder, allow_host_only=allow_host_only)
 
     if ssh_src or ssh_dest:
         ssh = ssh_src or ssh_dest
@@ -224,15 +239,15 @@
     # Attempt to parse the date with the format YYYY-MM-DD-HHMMSS
     dt = datetime.strptime(date_str, "%Y-%m-%d-%H%M%S")  # noqa: DTZ007
 
     # Convert the datetime object to Unix Epoch
     return int(time.mktime(dt.timetuple()))
 
 
-def find_backups(dest_folder: str, ssh: Optional[SSH]) -> List[str]:
+def find_backups(dest_folder: str, ssh: Optional[SSH] = None) -> List[str]:
     """Return a list of all available backups in the destination folder, sorted by date.
 
     (Replaces 'fn_find_backups' in the Bash script).
     """
     cmd = f"find '{dest_folder}/' -maxdepth 1 -type d -name '????-??-??-??????' -prune | sort -r"
     return run_cmd(cmd, ssh).stdout.splitlines()
 
@@ -329,88 +344,122 @@
 
 
 def backup_marker_path(folder: str) -> str:
     """Return the path to the backup marker file."""
     return os.path.join(folder, "backup.marker")
 
 
-def find_backup_marker(folder: str, ssh: Optional[SSH]) -> Optional[str]:
+def find_backup_marker(folder: str, ssh: Optional[SSH] = None) -> Optional[str]:
     """Find the backup marker file in the given folder."""
     marker_path = backup_marker_path(folder)
     output = find(marker_path, ssh)
     return marker_path if output else None
 
 
 class CmdResult(NamedTuple):
     """Command result."""
 
     stdout: str
     stderr: str
     returncode: int
 
 
-def run_cmd(
+async def async_run_cmd(
     cmd: str,
     ssh: Optional[SSH] = None,
 ) -> CmdResult:
     """Run a command locally or remotely."""
     if VERBOSE:
         log_info(
-            f"Running {'local' if ssh else 'remote'} command: {_bold(_green(cmd))}",
+            f"Running {'local' if ssh is None else 'remote'} command: {style(cmd, 'green', bold=True)}",
         )
+
     if ssh is not None:
-        result = subprocess.run(
+        process = await asyncio.create_subprocess_shell(
             f"{ssh.cmd} '{cmd}'",
-            shell=True,
-            capture_output=True,
-            text=True,
-            errors="surrogateescape",
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.PIPE,
         )
     else:
-        result = subprocess.run(
+        process = await asyncio.create_subprocess_shell(
             cmd,
-            shell=True,
-            capture_output=True,
-            text=True,
-            errors="surrogateescape",
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.PIPE,
         )
-    if VERBOSE:
-        if result.stdout:
-            log_info(f"Command output:\n{_bold(_magenta(result.stdout))}")
-        if result.stderr:
-            log_info(f"Command stderr:\n{_bold(_red(result.stderr))}")
-    return CmdResult(result.stdout.strip(), result.stderr.strip(), result.returncode)
 
+    # Should not be None because of asyncio.subprocess.PIPE
+    assert process.stdout is not None, "Process stdout is None"
+    assert process.stderr is not None, "Process stderr is None"
+
+    stdout, stderr = await asyncio.gather(
+        read_stream(process.stdout, log_info, "magenta"),
+        read_stream(process.stderr, log_info, "red"),
+    )
+
+    await process.wait()
+    assert process.returncode is not None, "Process has not returned"
+    return CmdResult(stdout, stderr, process.returncode)
+
+
+async def read_stream(
+    stream: asyncio.StreamReader,
+    callback: Callable[[str], None],
+    color: str,
+) -> str:
+    """Read each line from the stream and pass it to the callback."""
+    output = []
+    while True:
+        line = await stream.readline()
+        if line:
+            line_str = line.decode("utf-8", "replace").rstrip()
+            output.append(line_str)
+            if VERBOSE:
+                callback(f"Command output: {style(line_str, color, bold=True)}")
+        else:
+            break
+    return "\n".join(output)
+
+
+def run_cmd(
+    cmd: str,
+    ssh: Optional[SSH] = None,
+) -> CmdResult:
+    """Synchronously run a command locally or remotely."""
+    return asyncio.run(async_run_cmd(cmd, ssh))
 
-def find(path: str, ssh: Optional[SSH]) -> str:
+
+def find(path: str, ssh: Optional[SSH] = None, maxdepth: Optional[int] = None) -> str:
     """Find files in the given path, using the `find` command."""
-    return run_cmd(f"find '{path}'", ssh).stdout
+    cmd = f"find '{path}'"
+    if maxdepth is not None:
+        cmd += f" -maxdepth {maxdepth}"
+    return run_cmd(cmd, ssh).stdout
 
 
-def get_absolute_path(path: str, ssh: Optional[SSH]) -> str:
+def get_absolute_path(path: str, ssh: Optional[SSH] = None) -> str:
     """Get the absolute path of the given path."""
     return run_cmd(f"cd '{path}';pwd", ssh).stdout
 
 
-def mkdir(path: str, ssh: Optional[SSH]) -> None:
+def mkdir(path: str, ssh: Optional[SSH] = None) -> None:
     """Create a directory."""
     run_cmd(f"mkdir -p -- '{path}'", ssh)
 
 
-def rm_file(path: str, ssh: Optional[SSH]) -> None:
+def rm_file(path: str, ssh: Optional[SSH] = None) -> None:
     """Remove a file."""
     run_cmd(f"rm -f -- '{path}'", ssh)
 
 
-def rm_dir(path: str, ssh: Optional[SSH]) -> None:
+def rm_dir(path: str, ssh: Optional[SSH] = None) -> None:
     """Remove a directory."""
     run_cmd(f"rm -rf -- '{path}'", ssh)
 
 
-def ln(src: str, dest: str, ssh: Optional[SSH]) -> None:
+def ln(src: str, dest: str, ssh: Optional[SSH] = None) -> None:
     """Create a symlink."""
     run_cmd(f"ln -s -- '{src}' '{dest}'", ssh)
 
 
 def test_file_exists_src(path: str) -> bool:
     """Test if a file exists."""
     return run_cmd(f"test -e '{path}'", None).returncode == 0
@@ -428,25 +477,31 @@
     dest_folder: str,
     ssh: Optional[SSH],
 ) -> None:
     """Check if the destination is a backup folder or drive."""
     marker_path = backup_marker_path(dest_folder)
     if not find_backup_marker(dest_folder, ssh):
         log_info(
-            _yellow(
+            style(
                 "Safety check failed - the destination does not appear to be a backup folder or drive (marker file not found).",
+                "yellow",
             ),
         )
         log_info(
-            _yellow(
+            style(
                 "If it is indeed a backup folder, you may add the marker file by running the following command:",
+                "yellow",
             ),
         )
         log_info_cmd(
-            _bold(_green(f'mkdir -p -- "{dest_folder}" ; touch "{marker_path}"')),
+            style(
+                f'mkdir -p -- "{dest_folder}" ; touch "{marker_path}"',
+                "green",
+                bold=True,
+            ),
             ssh,
         )
         sys.exit(1)
 
 
 def get_link_dest_option(
     previous_dest: Optional[str],
@@ -458,32 +513,40 @@
         log_info("No previous backup - creating new one.")
     else:
         previous_dest = get_absolute_path(previous_dest, ssh)
         _full_previous_dest = (
             f"{ssh.dest_folder_prefix}{previous_dest}" if ssh else previous_dest
         )
         log_info(
-            _yellow(
-                f"Previous backup found - doing incremental backup from {_bold(_full_previous_dest)}",
+            style(
+                f"Previous backup found - doing incremental backup from {style(_full_previous_dest, bold=True)}",
+                "yellow",
             ),
         )
         link_dest_option = f"--link-dest='{previous_dest}'"
     return link_dest_option
 
 
 def handle_ssh(
     src_folder: str,
     dest_folder: str,
+    *,
     ssh_port: str,
     id_rsa: Optional[str],
     exclusion_file: str,
-    allow_host_only: bool,  # noqa: FBT001
+    allow_host_only: bool,
 ) -> Tuple[str, str, Optional[SSH]]:
     """Handle SSH-related things for in the `main` function."""
-    ssh = parse_ssh(src_folder, dest_folder, ssh_port, id_rsa, allow_host_only)
+    ssh = parse_ssh(
+        src_folder,
+        dest_folder,
+        ssh_port=ssh_port,
+        id_rsa=id_rsa,
+        allow_host_only=allow_host_only,
+    )
     if ssh is not None:
         if ssh.dest_folder:
             dest_folder = ssh.dest_folder
         if ssh.src_folder:
             src_folder = ssh.src_folder
 
     dest_folder = dest_folder.rstrip("/")
@@ -548,15 +611,15 @@
         rsync_flags.append("--modify-window=2")
 
     if ssh is not None:
         rsync_flags.append("--compress")
     return rsync_flags
 
 
-def exit_if_pid_running(running_pid: str, ssh: Optional[SSH]) -> None:
+def exit_if_pid_running(running_pid: str, ssh: Optional[SSH] = None) -> None:
     """Exit if another instance of this script is already running."""
     if sys.platform == "cygwin":
         cmd = f"procps -wwfo cmd -p {running_pid} --no-headers | grep '{APPNAME}'"
         running_cmd = run_cmd(cmd, ssh).stdout
         if running_cmd.returncode == 0:
             log_error(
                 f"Previous backup task is still active - aborting (command: {running_cmd.stdout}).",
@@ -599,16 +662,17 @@
         # Update PID to current process to avoid multiple concurrent resumes
         run_cmd(f"echo {mypid} > {inprogress_file}", ssh)
 
 
 def deal_with_no_space_left(
     log_file: str,
     dest_folder: str,
+    *,
     ssh: Optional[SSH],
-    auto_expire: bool,  # noqa: FBT001
+    auto_expire: bool,
 ) -> bool:
     """Deal with no space left on device."""
     with open(log_file) as f:
         log_data = f.read()
 
     no_space_left = re.search(
         r"No space left on device \(28\)|Result too large \(34\)",
@@ -647,15 +711,15 @@
             f"Rsync reported an error. Run this command for more details: grep -E 'rsync:|rsync error:' '{log_file}'",
         )
     elif "rsync:" in log_data:
         log_warn(
             f"Rsync reported a warning. Run this command for more details: grep -E 'rsync:|rsync error:' '{log_file}'",
         )
     else:
-        log_info(_magenta("Backup completed without errors."))
+        log_info(style("Backup completed without errors.", "magenta"))
         if auto_delete_log:
             os.remove(log_file)
 
 
 def now_str() -> str:
     """Return current date and time as string in format YYYY-MM-DD-HHMMSS."""
     return datetime.now().strftime("%Y-%m-%d-%H%M%S")
@@ -677,67 +741,68 @@
     log_file = os.path.join(
         log_dir,
         f"{now}.log",
     )
     if ssh is not None:
         src_folder = f"{ssh.src_folder_prefix}{src_folder}"
         dest = f"{ssh.dest_folder_prefix}{dest}"
-    log_info(_yellow("Starting backup..."))
-    log_info(f"From: {_bold(src_folder)}/")
-    log_info(f"To:   {_bold(dest)}/")
+    log_info(style("Starting backup...", "yellow"))
+    log_info(f"From: {style(src_folder, bold=True)}/")
+    log_info(f"To:   {style(dest, bold=True)}/")
 
     cmd = "rsync"
     if ssh is not None:
         id_rsa_option = f"-i {ssh.id_rsa} " if ssh.id_rsa else ""
         cmd = f"{cmd} -e 'ssh -p {ssh.port} {id_rsa_option}-o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null'"
 
     cmd = f"{cmd} {' '.join(rsync_flags)}"
     cmd = f"{cmd} --log-file '{log_file}'"
     if exclusion_file:
         cmd = f"{cmd} --exclude-from '{exclusion_file}'"
 
     cmd = f"{cmd} {link_dest_option}"
     cmd = f"{cmd} -- '{src_folder}/' '{dest}/'"
 
-    log_info(_bold("Running command:"))
-    log_info(_green(cmd))
+    log_info(style("Running command:", bold=True))
+    log_info(style(cmd, "green"))
 
     run_cmd(f"echo {mypid} > {inprogress_file}", ssh)
 
     run_cmd(cmd)
     return log_file
 
 
 def backup(
     src_folder: str,
     dest_folder: str,
+    *,
     exclusion_file: str,
     log_dir: str,
-    auto_delete_log: bool,  # noqa: FBT001
+    auto_delete_log: bool,
     expiration_strategy: str,
-    auto_expire: bool,  # noqa: FBT001
+    auto_expire: bool,
     port: str,
     id_rsa: str,
     rsync_set_flags: str,
     rsync_append_flags: str,
-    rsync_get_flags: bool,  # noqa: FBT001
-    allow_host_only: bool,  # noqa: FBT001
+    rsync_get_flags: bool,
+    allow_host_only: bool,
 ) -> None:
     """Perform backup of src_folder to dest_folder."""
     (
         src_folder,
         dest_folder,
         ssh,
     ) = handle_ssh(
         src_folder,
         dest_folder,
-        port,
-        id_rsa,
-        exclusion_file,
-        allow_host_only,
+        ssh_port=port,
+        id_rsa=id_rsa,
+        exclusion_file=exclusion_file,
+        allow_host_only=allow_host_only,
     )
 
     if not test_file_exists_src(src_folder):
         log_error(f"Source folder '{src_folder}' does not exist - aborting.")
         sys.exit(1)
 
     check_dest_is_backup_folder(dest_folder, ssh)
@@ -768,25 +833,25 @@
         rsync_set_flags,
         rsync_append_flags,
         ssh,
     )
 
     if rsync_get_flags:
         flags = " ".join(rsync_flags)
-        log_info(f"Rsync flags:\n{_bold(_yellow(flags))}")
+        log_info(f"Rsync flags:\n{style(flags, 'yellow', bold=True)}")
         sys.exit(0)
 
     for _ in range(100):  # max 100 retries when no space left
         link_dest_option = get_link_dest_option(
             previous_dest,
             ssh,
         )
 
-        if not find(dest, ssh):
-            _full_dest = _bold(f"{ssh.cmd if ssh else ''}{dest}")
+        if not find(dest, ssh, maxdepth=0):
+            _full_dest = style(f"{ssh.cmd if ssh else ''}{dest}", bold=True)
             log_info(f"Creating destination {_full_dest}")
             mkdir(dest, ssh)
 
         expire_backups(
             dest_folder,
             expiration_strategy,
             previous_dest if previous_dest else dest,
@@ -804,16 +869,16 @@
             mypid,
             ssh,
             now,
         )
         retry = deal_with_no_space_left(
             log_file,
             dest_folder,
-            ssh,
-            auto_expire,
+            ssh=ssh,
+            auto_expire=auto_expire,
         )
         if not retry:
             break
 
     check_rsync_errors(log_file, auto_delete_log)
 
     rm_file(os.path.join(dest_folder, "latest"), ssh)
```

### Comparing `rsync-time-machine-1.0.0/tests/test_app.py` & `rsync-time-machine-1.1.0/tests/test_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Test suite for `rsync-time-machine.py`."""
 import os
+import unicodedata
 from contextlib import contextmanager
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Iterator, Union
 from unittest.mock import Mock, patch
 
 import pytest
@@ -75,16 +76,16 @@
 
 
 def test_parse_ssh() -> None:
     """Test the parse_ssh function."""
     ssh = parse_ssh(
         "user@example.com:/path/to/src",
         "user@example.com:/path/to/dest",
-        "22",
-        None,
+        ssh_port="22",
+        id_rsa=None,
         allow_host_only=False,
     )
     assert ssh == SSH(
         "user@example.com:",
         "user@example.com:",
         "ssh -p 22 user@example.com",
         "/path/to/src",
@@ -92,16 +93,16 @@
         "22",
         None,
     )
 
     ssh = parse_ssh(
         "user@example.com:/path/to/src",
         "/path/to/dest",
-        "22",
-        None,
+        ssh_port="22",
+        id_rsa=None,
         allow_host_only=False,
     )
     assert ssh == SSH(
         "user@example.com:",
         "",
         "ssh -p 22 user@example.com",
         "/path/to/src",
@@ -109,38 +110,44 @@
         "22",
         None,
     )
 
     ssh = parse_ssh(
         "/path/to/src",
         "user@example.com:/path/to/dest",
-        "22",
-        None,
+        ssh_port="22",
+        id_rsa=None,
         allow_host_only=False,
     )
     assert ssh == SSH(
         "",
         "user@example.com:",
         "ssh -p 22 user@example.com",
         "/path/to/src",
         "/path/to/dest",
         "22",
         None,
     )
 
     assert (
-        parse_ssh("/path/to/src", "/path/to/dest", "22", None, allow_host_only=False)
+        parse_ssh(
+            "/path/to/src",
+            "/path/to/dest",
+            ssh_port="22",
+            id_rsa=None,
+            allow_host_only=False,
+        )
         is None
     )
 
     ssh = parse_ssh(
         "host:/path/to/src",
         "host:/path/to/dest",
-        "22",
-        None,
+        ssh_port="22",
+        id_rsa=None,
         allow_host_only=True,
     )
     assert ssh == SSH(
         "host:",
         "host:",
         "ssh -p 22 host",
         "/path/to/src",
@@ -149,16 +156,16 @@
         None,
     )
 
     assert (
         parse_ssh(
             "host:/path/to/src",
             "host:/path/to/dest",
-            "22",
-            None,
+            ssh_port="22",
+            id_rsa=None,
             allow_host_only=False,
         )
         is None
     )
 
 
 def test_find_backups(tmp_path: Path) -> None:
@@ -198,14 +205,15 @@
 
 
 def test_find(tmp_path: Path) -> None:
     """Test the find function."""
     path = tmp_path / "testfile.txt"
     path.touch()
     assert find(str(path), None) == str(path)
+    assert find(str(tmp_path), None, maxdepth=0) == str(tmp_path)
 
 
 def test_get_absolute_path(tmp_path: Path) -> None:
     """Test the get_absolute_path function."""
     path = tmp_path / "testfolder"
     path.mkdir()
     assert get_absolute_path(str(path), None) == str(path.resolve())
@@ -255,17 +263,17 @@
 
 
 def test_handle_ssh() -> None:
     """Test the handle_ssh function."""
     src_folder, dest_folder, ssh = handle_ssh(
         "user@example.com:/path/to/src",
         "user@example.com:/path/to/dest",
-        "22",
-        None,
-        "exclusion_file",
+        ssh_port="22",
+        id_rsa=None,
+        exclusion_file="exclusion_file",
         allow_host_only=False,
     )
     assert src_folder == "/path/to/src"
     assert dest_folder == "/path/to/dest"
     assert ssh == SSH(
         "user@example.com:",
         "user@example.com:",
@@ -275,17 +283,17 @@
         "22",
         None,
     )
 
     src_folder, dest_folder, ssh = handle_ssh(
         "/path/to/src",
         "/path/to/dest",
-        "22",
-        "",
-        "exclusion_file",
+        ssh_port="22",
+        id_rsa="",
+        exclusion_file="exclusion_file",
         allow_host_only=False,
     )
     assert src_folder == "/path/to/src"
     assert dest_folder == "/path/to/dest"
     assert ssh is None
 
 
@@ -438,19 +446,24 @@
     Reproduces https://github.com/basnijholt/rsync-time-machine.py/issues/1
     """
     src_folder = tmp_path / "src"
     dest_folder = tmp_path / "dest"
     src_folder.mkdir()
     dest_folder.mkdir()
 
-    # Create a folder and file with a non-UTF8 filename
+    # Create a folder and files with a non-UTF8 filename
     folder = "TEST-UTF8"
     (src_folder / folder).mkdir()
-    non_utf8_filename = "Mîso.rtf"
-    (src_folder / folder / non_utf8_filename).write_text("Hello, World!")
+
+    # Create composed and decomposed form of 'î'
+    composed_filename = unicodedata.normalize("NFC", "Möîso1.rtf")
+    decomposed_filename = unicodedata.normalize("NFD", "Möîso2.rtf")
+
+    (src_folder / folder / composed_filename).write_text("Hello, World!")
+    (src_folder / folder / decomposed_filename).write_text("Hello, World!")
 
     kw = {
         "src_folder": str(src_folder),
         "dest_folder": str(dest_folder),
         "exclusion_file": "",
         "log_dir": str(tmp_path / "logs"),
         "auto_delete_log": True,
@@ -467,11 +480,12 @@
     # Create a backup.marker file
     Path(backup_marker_path(str(dest_folder))).touch()
 
     # Run the backup
     backup(**kw)  # type: ignore[arg-type]
 
     # Check that the backup was created
-    assert (dest_folder / "latest" / folder / non_utf8_filename).exists()
-    assert (
-        dest_folder / "latest" / folder / non_utf8_filename
-    ).read_text() == "Hello, World!"
+    for filename in [composed_filename, decomposed_filename]:
+        assert (dest_folder / "latest" / folder / filename).exists()
+        assert (
+            dest_folder / "latest" / folder / filename
+        ).read_text() == "Hello, World!"
```

