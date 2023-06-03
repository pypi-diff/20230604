# Comparing `tmp/CommandAlarm-0.1.0.tar.gz` & `tmp/CommandAlarm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommandAlarm-0.1.0.tar", last modified: Fri Jun  2 22:24:48 2023, max compression
+gzip compressed data, was "CommandAlarm-0.2.0.tar", last modified: Sat Jun  3 22:00:42 2023, max compression
```

## Comparing `CommandAlarm-0.1.0.tar` & `CommandAlarm-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-02 22:24:48.227383 CommandAlarm-0.1.0/
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-02 22:24:48.223383 CommandAlarm-0.1.0/CommandAlarm.egg-info/
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2442 2023-06-02 22:24:47.000000 CommandAlarm-0.1.0/CommandAlarm.egg-info/PKG-INFO
--rw-r--r--   0 testuser  (1002) testuser  (1003)      263 2023-06-02 22:24:48.000000 CommandAlarm-0.1.0/CommandAlarm.egg-info/SOURCES.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)        1 2023-06-02 22:24:47.000000 CommandAlarm-0.1.0/CommandAlarm.egg-info/dependency_links.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)       64 2023-06-02 22:24:47.000000 CommandAlarm-0.1.0/CommandAlarm.egg-info/entry_points.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)       13 2023-06-02 22:24:47.000000 CommandAlarm-0.1.0/CommandAlarm.egg-info/top_level.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)    35149 2017-09-30 07:16:26.000000 CommandAlarm-0.1.0/LICENSE
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2442 2023-06-02 22:24:48.223383 CommandAlarm-0.1.0/PKG-INFO
--rw-r--r--   0 testuser  (1002) testuser  (1003)     1919 2023-06-02 21:29:01.000000 CommandAlarm-0.1.0/README.md
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-02 22:24:48.223383 CommandAlarm-0.1.0/commandalarm/
--rw-r--r--   0 testuser  (1002) testuser  (1003)       46 2023-05-24 13:26:33.000000 CommandAlarm-0.1.0/commandalarm/__init__.py
--rw-r--r--   0 testuser  (1002) testuser  (1003)     5645 2023-06-02 20:52:02.000000 CommandAlarm-0.1.0/commandalarm/commandalarm.py
--rw-r--r--   0 testuser  (1002) testuser  (1003)       38 2023-06-02 22:24:48.227383 CommandAlarm-0.1.0/setup.cfg
--rw-r--r--   0 testuser  (1002) testuser  (1003)      863 2023-06-02 20:02:40.000000 CommandAlarm-0.1.0/setup.py
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-03 22:00:42.000595 CommandAlarm-0.2.0/
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-03 22:00:41.996595 CommandAlarm-0.2.0/CommandAlarm.egg-info/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2829 2023-06-03 22:00:41.000000 CommandAlarm-0.2.0/CommandAlarm.egg-info/PKG-INFO
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      263 2023-06-03 22:00:41.000000 CommandAlarm-0.2.0/CommandAlarm.egg-info/SOURCES.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)        1 2023-06-03 22:00:41.000000 CommandAlarm-0.2.0/CommandAlarm.egg-info/dependency_links.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       64 2023-06-03 22:00:41.000000 CommandAlarm-0.2.0/CommandAlarm.egg-info/entry_points.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       13 2023-06-03 22:00:41.000000 CommandAlarm-0.2.0/CommandAlarm.egg-info/top_level.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)    35149 2017-09-30 07:16:26.000000 CommandAlarm-0.2.0/LICENSE
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2829 2023-06-03 22:00:42.000595 CommandAlarm-0.2.0/PKG-INFO
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2306 2023-06-03 21:58:23.000000 CommandAlarm-0.2.0/README.md
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-03 22:00:42.000595 CommandAlarm-0.2.0/commandalarm/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       46 2023-06-03 20:03:07.000000 CommandAlarm-0.2.0/commandalarm/__init__.py
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     7486 2023-06-03 21:44:46.000000 CommandAlarm-0.2.0/commandalarm/commandalarm.py
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       38 2023-06-03 22:00:42.000595 CommandAlarm-0.2.0/setup.cfg
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      863 2023-06-03 20:02:47.000000 CommandAlarm-0.2.0/setup.py
```

### Comparing `CommandAlarm-0.1.0/CommandAlarm.egg-info/PKG-INFO` & `CommandAlarm-0.2.0/CommandAlarm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommandAlarm
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple command line program that allows users to set an alarm with a custom command.
 Home-page: https://github.com/alofgren/commandalarm
 Author: alofgren
 Author-email: drelofren@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -31,40 +31,49 @@
 cd commandalarm
 pip install .
 ```
 
 ## Usage Output
 
 ```bash
-usage: commandalarm.py [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] time command [command ...]
+usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [command ...]
 
 Set an alarm with a custom command.
 
 positional arguments:
   time                  the time in the format HH:MM:SS
-  command               the command to be executed
+  command               the command to run
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -d {1,2,3,4,5,6,7}, --day {1,2,3,4,5,6,7}
                         the day of the week as an integer from 1 to 7, where 1 represents Monday
   -r, --repeat          repeat indefinitely
+  -s, --shell           run command with shell
+  -n, --no-check        don't check the command return code
+  -t TIMEOUT, --timeout TIMEOUT
+                        timeout in seconds for the command to complete
 ```
 
 ## Examples
 
 To set an alarm for 2:00 PM on Tuesday, and play a sound when the alarm goes off:
 ```bash
-commandalarm -d 2 14:00:00 afplay alarm_sound.mp3
+commandalarm -d 2 14:00:00 aplay alarm_sound.wav
 ```
 
-To set an alarm for 6:30 AM, and run the ls command with the -l option when the alarm goes off:
+To set an alarm for 10:00 PM to run a command with shell and repeat indefinitely: 
 ```bash
-commandalarm 06:30:00 -- ls -l
+commandalarm 22:00:00 -r -s 'echo "Hello, world!"'
+```
+
+To set an alarm for 9:15 AM on Wednesday to run a Python script with a timeout of 30 seconds: 
+```bash
+commandalarm 09:15:00 -d 3 -t 30 python3 script.py
 ```
 
 ## Contributing
 
 If you would like to contribute to CommandAlarm, please feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/alofgren/commandalarm).
 
 ## Donate
```

### Comparing `CommandAlarm-0.1.0/LICENSE` & `CommandAlarm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CommandAlarm-0.1.0/PKG-INFO` & `CommandAlarm-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommandAlarm
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple command line program that allows users to set an alarm with a custom command.
 Home-page: https://github.com/alofgren/commandalarm
 Author: alofgren
 Author-email: drelofren@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -31,40 +31,49 @@
 cd commandalarm
 pip install .
 ```
 
 ## Usage Output
 
 ```bash
-usage: commandalarm.py [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] time command [command ...]
+usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [command ...]
 
 Set an alarm with a custom command.
 
 positional arguments:
   time                  the time in the format HH:MM:SS
-  command               the command to be executed
+  command               the command to run
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -d {1,2,3,4,5,6,7}, --day {1,2,3,4,5,6,7}
                         the day of the week as an integer from 1 to 7, where 1 represents Monday
   -r, --repeat          repeat indefinitely
+  -s, --shell           run command with shell
+  -n, --no-check        don't check the command return code
+  -t TIMEOUT, --timeout TIMEOUT
+                        timeout in seconds for the command to complete
 ```
 
 ## Examples
 
 To set an alarm for 2:00 PM on Tuesday, and play a sound when the alarm goes off:
 ```bash
-commandalarm -d 2 14:00:00 afplay alarm_sound.mp3
+commandalarm -d 2 14:00:00 aplay alarm_sound.wav
 ```
 
-To set an alarm for 6:30 AM, and run the ls command with the -l option when the alarm goes off:
+To set an alarm for 10:00 PM to run a command with shell and repeat indefinitely: 
 ```bash
-commandalarm 06:30:00 -- ls -l
+commandalarm 22:00:00 -r -s 'echo "Hello, world!"'
+```
+
+To set an alarm for 9:15 AM on Wednesday to run a Python script with a timeout of 30 seconds: 
+```bash
+commandalarm 09:15:00 -d 3 -t 30 python3 script.py
 ```
 
 ## Contributing
 
 If you would like to contribute to CommandAlarm, please feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/alofgren/commandalarm).
 
 ## Donate
```

### Comparing `CommandAlarm-0.1.0/README.md` & `CommandAlarm-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,40 +17,49 @@
 cd commandalarm
 pip install .
 ```
 
 ## Usage Output
 
 ```bash
-usage: commandalarm.py [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] time command [command ...]
+usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [command ...]
 
 Set an alarm with a custom command.
 
 positional arguments:
   time                  the time in the format HH:MM:SS
-  command               the command to be executed
+  command               the command to run
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -d {1,2,3,4,5,6,7}, --day {1,2,3,4,5,6,7}
                         the day of the week as an integer from 1 to 7, where 1 represents Monday
   -r, --repeat          repeat indefinitely
+  -s, --shell           run command with shell
+  -n, --no-check        don't check the command return code
+  -t TIMEOUT, --timeout TIMEOUT
+                        timeout in seconds for the command to complete
 ```
 
 ## Examples
 
 To set an alarm for 2:00 PM on Tuesday, and play a sound when the alarm goes off:
 ```bash
-commandalarm -d 2 14:00:00 afplay alarm_sound.mp3
+commandalarm -d 2 14:00:00 aplay alarm_sound.wav
 ```
 
-To set an alarm for 6:30 AM, and run the ls command with the -l option when the alarm goes off:
+To set an alarm for 10:00 PM to run a command with shell and repeat indefinitely: 
 ```bash
-commandalarm 06:30:00 -- ls -l
+commandalarm 22:00:00 -r -s 'echo "Hello, world!"'
+```
+
+To set an alarm for 9:15 AM on Wednesday to run a Python script with a timeout of 30 seconds: 
+```bash
+commandalarm 09:15:00 -d 3 -t 30 python3 script.py
 ```
 
 ## Contributing
 
 If you would like to contribute to CommandAlarm, please feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/alofgren/commandalarm).
 
 ## Donate
```

### Comparing `CommandAlarm-0.1.0/setup.py` & `CommandAlarm-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CommandAlarm",
-    version="0.1.0",
+    version="0.2.0",
     author="alofgren",
     author_email="drelofren@outlook.com",
     description="A simple command line program that allows users to set an alarm with a custom command.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alofgren/commandalarm",
     packages=setuptools.find_packages(),
```

