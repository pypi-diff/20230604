# Comparing `tmp/InternetSpeedLogger-1.1.1.tar.gz` & `tmp/InternetSpeedLogger-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternetSpeedLogger-1.1.1.tar", last modified: Sat Jun  3 13:02:15 2023, max compression
+gzip compressed data, was "InternetSpeedLogger-1.2.0.tar", last modified: Sun Jun  4 08:40:49 2023, max compression
```

## Comparing `InternetSpeedLogger-1.1.1.tar` & `InternetSpeedLogger-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 13:02:15.236197 InternetSpeedLogger-1.1.1/
--rw-r--r--   0 andreas   (1000) apache      (48)     1071 2023-06-02 15:28:30.000000 InternetSpeedLogger-1.1.1/LICENSE
--rw-r--r--   0 andreas   (1000) apache      (48)     5813 2023-06-03 13:02:15.235197 InternetSpeedLogger-1.1.1/PKG-INFO
--rw-r--r--   0 andreas   (1000) apache      (48)     3893 2023-06-03 12:11:32.000000 InternetSpeedLogger-1.1.1/README.md
--rw-r--r--   0 andreas   (1000) apache      (48)      936 2023-06-03 13:01:24.000000 InternetSpeedLogger-1.1.1/pyproject.toml
--rw-r--r--   0 andreas   (1000) apache      (48)       38 2023-06-03 13:02:15.236197 InternetSpeedLogger-1.1.1/setup.cfg
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 13:02:15.220197 InternetSpeedLogger-1.1.1/src/
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 13:02:15.225197 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger/
--rw-r--r--   0 andreas   (1000) apache      (48)     5026 2023-06-03 13:01:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger/InternetSpeedLogger.py
--rw-r--r--   0 andreas   (1000) apache      (48)        0 2023-06-03 07:33:53.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger/__init__.py
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-03 13:02:15.234197 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/
--rw-r--r--   0 andreas   (1000) apache      (48)     5813 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) apache      (48)      399 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) apache      (48)        1 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       85 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/entry_points.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       14 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/requires.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       20 2023-06-03 13:02:15.000000 InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/top_level.txt
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 08:40:49.930216 InternetSpeedLogger-1.2.0/
+-rw-r--r--   0 andreas   (1000) apache      (48)     1071 2023-06-02 15:28:30.000000 InternetSpeedLogger-1.2.0/LICENSE
+-rw-r--r--   0 andreas   (1000) apache      (48)     5809 2023-06-04 08:40:49.930216 InternetSpeedLogger-1.2.0/PKG-INFO
+-rw-r--r--   0 andreas   (1000) apache      (48)     3889 2023-06-03 13:09:41.000000 InternetSpeedLogger-1.2.0/README.md
+-rw-r--r--   0 andreas   (1000) apache      (48)      936 2023-06-04 08:33:54.000000 InternetSpeedLogger-1.2.0/pyproject.toml
+-rw-r--r--   0 andreas   (1000) apache      (48)       38 2023-06-04 08:40:49.931216 InternetSpeedLogger-1.2.0/setup.cfg
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 08:40:49.920216 InternetSpeedLogger-1.2.0/src/
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 08:40:49.925216 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger/
+-rw-r--r--   0 andreas   (1000) apache      (48)     5711 2023-06-04 08:33:35.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger/InternetSpeedLogger.py
+-rw-r--r--   0 andreas   (1000) apache      (48)       47 2023-06-03 16:58:12.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger/__init__.py
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 08:40:49.929216 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/
+-rw-r--r--   0 andreas   (1000) apache      (48)     5809 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) apache      (48)      399 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)        1 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       85 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/entry_points.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       14 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/requires.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       20 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/top_level.txt
```

### Comparing `InternetSpeedLogger-1.1.1/LICENSE` & `InternetSpeedLogger-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `InternetSpeedLogger-1.1.1/PKG-INFO` & `InternetSpeedLogger-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternetSpeedLogger
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Python script that continuously monitors and logs your internet speed.
 Author-email: Andreas Menzel <mail@andreas-menzel.com>
 License: MIT License
         
         Copyright (c) 2023 Andreas Menzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -123,12 +123,12 @@
 Remember, the best way to make successful contributions is to communicate! Feel
 free to ask questions and discuss your ideas in the issue tracker.
 
 In your pull request, provide a clear and comprehensive explanation of your
 changes and their necessity. This will help us understand the purpose of your
 contribution and expedite the review process.
 
-Thank you for your interest in improving InternetSpeedDataLogger! :heart:
+Thank you for your interest in improving InternetSpeedLogger! :heart:
 
 ## License
 
 This script is released under the MIT License.
```

### Comparing `InternetSpeedLogger-1.1.1/README.md` & `InternetSpeedLogger-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -86,12 +86,12 @@
 Remember, the best way to make successful contributions is to communicate! Feel
 free to ask questions and discuss your ideas in the issue tracker.
 
 In your pull request, provide a clear and comprehensive explanation of your
 changes and their necessity. This will help us understand the purpose of your
 contribution and expedite the review process.
 
-Thank you for your interest in improving InternetSpeedDataLogger! :heart:
+Thank you for your interest in improving InternetSpeedLogger! :heart:
 
 ## License
 
 This script is released under the MIT License.
```

### Comparing `InternetSpeedLogger-1.1.1/pyproject.toml` & `InternetSpeedLogger-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "InternetSpeedLogger"
-version = "1.1.1"
+version = "1.2.0"
 dependencies = [
     "speedtest_cli"
 ]
 authors = [
   { name="Andreas Menzel", email="mail@andreas-menzel.com" },
 ]
 description = "A Python script that continuously monitors and logs your internet speed."
```

### Comparing `InternetSpeedLogger-1.1.1/src/InternetSpeedLogger/InternetSpeedLogger.py` & `InternetSpeedLogger-1.2.0/src/InternetSpeedLogger/InternetSpeedLogger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,106 @@
 #!/usr/bin/env python3
 
-# -------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # InternetSpeedLogger
 #
 # A Python script that continuously monitors and logs your internet speed. It
 # tests both download and upload speeds at regular intervals and records the
 # data in a CSV file for easy analysis and tracking. Ideal for auditing your
 # network performance or ISP reliability over time.
 #
 # https://github.com/Andreas-Menzel/InternetSpeedLogger
 # https://pypi.org/project/InternetSpeedLogger/
-# -------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 # @author: Andreas Menzel
 # @license: MIT License
-# -------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
 
 import argparse
 import csv
 from datetime import datetime
 from pathlib import Path
 from signal import signal, SIGINT
 from speedtest import Speedtest
+from tempfile import gettempdir
 from time import sleep
 
 
-script_version = '1.1.1'
+script_version = '1.2.0'
 
 
 def argparse_check_positive(value):
     ivalue = int(value)
     if ivalue <= 0:
-        raise argparse.ArgumentTypeError("%s is an invalid positive int value" % value)
+        raise argparse.ArgumentTypeError(
+            "%s is an invalid positive int value" % value)
     return ivalue
 
+
 def setupArgumentParser():
     parser = argparse.ArgumentParser(
         prog='InternetSpeedLogger',
         description="""
 A Python script that continuously monitors and logs your internet
 speed. It tests both download and upload speeds at regular intervals
 and records the data in a CSV file for easy analysis and tracking.
 Ideal for auditing your network performance or ISP reliability over
 time.
             """,
         epilog="""
 Default location of the log-file:
     A .csv-file will be created, which will contain all logged information.
     Default Filename: "YYYY-MM-DD_HH:MM:SS_internet_speeds.csv"
-    Default Location: typically "/home/<username>" on Linux
-                      typically "C:\\Users\\<username>" on Windows
-                      typically "/Users/<username>" on macOS
+    Default Location: <tmp_dir>/InternetSpeedLogger/
+        <tmp_dir> on Windows: C:\\TEMP, C:\\TMP, \\TEMP, or \\TMP, in that order
+        <tmp_dir> on all other: /tmp, /var/tmp, or /usr/tmp, in that order
             """,
         formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('--version', action='version',
                         version='%(prog)s ' + script_version)
     parser.add_argument('-i', '--interval',
                         help='Testing interval in seconds. Make sure that the interval is not shorter than the time needed for testing. (default: %(default)s)',
                         type=argparse_check_positive,
                         default=60)
     parser.add_argument('-d', '--duration',
                         help='Duration of the entire test runs. The script will automatically end after this duration. Set to <= 0 for infinite. (default: %(default)s)',
                         type=int,
                         default=0)
     parser.add_argument('-l', '--log_file',
-                        help='Filename for the log-file. NOTE: The file will be overwritten if it already exists. NOTE: ".csv" will be automatically appended to the filename!',
+                        help='Filename for the log-file. NOTE: A similar filename will be chosen if a file with this name already exists.',
                         default='')
     return parser.parse_args()
 
 
 def main():
     args = setupArgumentParser()
 
     st = Speedtest()
 
+    datetimeString = datetime.now().strftime("%Y-%m-%d_%H:%M:%S")
     if args.log_file != '':
-        csv_file = Path(f'{args.log_file}.csv')
+        if len(args.log_file) > 4 and args.log_file[-4:] == '.csv':
+            csv_file = Path(f'{args.log_file}')
+        else:
+            csv_file = Path(f'{args.log_file}.csv')
     else:
         # Set to default/fallback location.
         csv_file = Path(
-            f'{Path.home().joinpath(datetime.now().strftime("%Y-%m-%d_%H:%M:%S"))}_internet_speeds.csv')
+            f'{Path(gettempdir(), "InternetSpeedLogger", datetimeString)}_internet_speeds.csv')
+
+    # Make sure that the log-file is unique and does not exist yet.
+    if csv_file.exists():
+        csv_file = Path(csv_file.parent, f'{csv_file.stem}_{datetimeString}{csv_file.suffix}')
+    if csv_file.exists():
+        counter = 2
+        new_csv_file = csv_file
+        while new_csv_file.exists():
+            new_csv_file = Path(csv_file.parent, f'{csv_file.stem}_{counter}{csv_file.suffix}')
+            counter = counter + 1
+        csv_file = new_csv_file
 
     print(f"""\
 InternetSpeedLogger (version {script_version})
 
 Testing interval: {args.interval} s
 Testing duration: {args.duration} s
 Log-file: "{csv_file.absolute()}"\
```

### Comparing `InternetSpeedLogger-1.1.1/src/InternetSpeedLogger.egg-info/PKG-INFO` & `InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternetSpeedLogger
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Python script that continuously monitors and logs your internet speed.
 Author-email: Andreas Menzel <mail@andreas-menzel.com>
 License: MIT License
         
         Copyright (c) 2023 Andreas Menzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -123,12 +123,12 @@
 Remember, the best way to make successful contributions is to communicate! Feel
 free to ask questions and discuss your ideas in the issue tracker.
 
 In your pull request, provide a clear and comprehensive explanation of your
 changes and their necessity. This will help us understand the purpose of your
 contribution and expedite the review process.
 
-Thank you for your interest in improving InternetSpeedDataLogger! :heart:
+Thank you for your interest in improving InternetSpeedLogger! :heart:
 
 ## License
 
 This script is released under the MIT License.
```

