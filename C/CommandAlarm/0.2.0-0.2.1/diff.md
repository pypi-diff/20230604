# Comparing `tmp/CommandAlarm-0.2.0.tar.gz` & `tmp/CommandAlarm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommandAlarm-0.2.0.tar", last modified: Sat Jun  3 22:00:42 2023, max compression
+gzip compressed data, was "CommandAlarm-0.2.1.tar", last modified: Sun Jun  4 13:55:43 2023, max compression
```

## Comparing `CommandAlarm-0.2.0.tar` & `CommandAlarm-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-03 22:00:42.000595 CommandAlarm-0.2.0/
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-03 22:00:41.996595 CommandAlarm-0.2.0/CommandAlarm.egg-info/
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2829 2023-06-03 22:00:41.000000 CommandAlarm-0.2.0/CommandAlarm.egg-info/PKG-INFO
--rw-r--r--   0 testuser  (1002) testuser  (1003)      263 2023-06-03 22:00:41.000000 CommandAlarm-0.2.0/CommandAlarm.egg-info/SOURCES.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)        1 2023-06-03 22:00:41.000000 CommandAlarm-0.2.0/CommandAlarm.egg-info/dependency_links.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)       64 2023-06-03 22:00:41.000000 CommandAlarm-0.2.0/CommandAlarm.egg-info/entry_points.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)       13 2023-06-03 22:00:41.000000 CommandAlarm-0.2.0/CommandAlarm.egg-info/top_level.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)    35149 2017-09-30 07:16:26.000000 CommandAlarm-0.2.0/LICENSE
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2829 2023-06-03 22:00:42.000595 CommandAlarm-0.2.0/PKG-INFO
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2306 2023-06-03 21:58:23.000000 CommandAlarm-0.2.0/README.md
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-03 22:00:42.000595 CommandAlarm-0.2.0/commandalarm/
--rw-r--r--   0 testuser  (1002) testuser  (1003)       46 2023-06-03 20:03:07.000000 CommandAlarm-0.2.0/commandalarm/__init__.py
--rw-r--r--   0 testuser  (1002) testuser  (1003)     7486 2023-06-03 21:44:46.000000 CommandAlarm-0.2.0/commandalarm/commandalarm.py
--rw-r--r--   0 testuser  (1002) testuser  (1003)       38 2023-06-03 22:00:42.000595 CommandAlarm-0.2.0/setup.cfg
--rw-r--r--   0 testuser  (1002) testuser  (1003)      863 2023-06-03 20:02:47.000000 CommandAlarm-0.2.0/setup.py
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-04 13:55:43.722021 CommandAlarm-0.2.1/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      321 2023-06-04 10:08:34.000000 CommandAlarm-0.2.1/CHANGELOG.md
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-04 13:55:43.698021 CommandAlarm-0.2.1/CommandAlarm.egg-info/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2829 2023-06-04 13:55:43.000000 CommandAlarm-0.2.1/CommandAlarm.egg-info/PKG-INFO
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      288 2023-06-04 13:55:43.000000 CommandAlarm-0.2.1/CommandAlarm.egg-info/SOURCES.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)        1 2023-06-04 13:55:43.000000 CommandAlarm-0.2.1/CommandAlarm.egg-info/dependency_links.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       64 2023-06-04 13:55:43.000000 CommandAlarm-0.2.1/CommandAlarm.egg-info/entry_points.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       13 2023-06-04 13:55:43.000000 CommandAlarm-0.2.1/CommandAlarm.egg-info/top_level.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)    35149 2017-09-30 07:16:26.000000 CommandAlarm-0.2.1/LICENSE
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       29 2023-06-04 13:17:50.000000 CommandAlarm-0.2.1/MANIFEST.in
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2829 2023-06-04 13:55:43.722021 CommandAlarm-0.2.1/PKG-INFO
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2306 2023-06-03 22:05:16.000000 CommandAlarm-0.2.1/README.md
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-04 13:55:43.710021 CommandAlarm-0.2.1/commandalarm/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       46 2023-06-04 10:11:11.000000 CommandAlarm-0.2.1/commandalarm/__init__.py
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     7202 2023-06-04 10:51:58.000000 CommandAlarm-0.2.1/commandalarm/commandalarm.py
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       38 2023-06-04 13:55:43.722021 CommandAlarm-0.2.1/setup.cfg
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      863 2023-06-04 13:17:35.000000 CommandAlarm-0.2.1/setup.py
```

### Comparing `CommandAlarm-0.2.0/CommandAlarm.egg-info/PKG-INFO` & `CommandAlarm-0.2.1/CommandAlarm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommandAlarm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple command line program that allows users to set an alarm with a custom command.
 Home-page: https://github.com/alofgren/commandalarm
 Author: alofgren
 Author-email: drelofren@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `CommandAlarm-0.2.0/LICENSE` & `CommandAlarm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CommandAlarm-0.2.0/PKG-INFO` & `CommandAlarm-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommandAlarm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple command line program that allows users to set an alarm with a custom command.
 Home-page: https://github.com/alofgren/commandalarm
 Author: alofgren
 Author-email: drelofren@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `CommandAlarm-0.2.0/README.md` & `CommandAlarm-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `CommandAlarm-0.2.0/commandalarm/commandalarm.py` & `CommandAlarm-0.2.1/commandalarm/commandalarm.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         "--repeat",
         action="store_true",
         help="repeat indefinitely",
     )
     parser.add_argument("-s",
                         "--shell",
                         action="store_true",
+                        default=False,
                         help="run command with shell")
     parser.add_argument("-n",
                         "--no-check",
                         action="store_false",
                         default=True,
                         help="don't check the command return code",
                         dest="check")
@@ -174,30 +175,23 @@
         while True:
             while not ALARM_FIRED:
                 signal.pause()
             print("Time is up!")
             command_str = " ".join(args.command)
             print("Running command:", command_str)
             try:
-                if args.shell:
-                    result = subprocess.run(command_str,
-                                            capture_output=True,
-                                            shell=True,
-                                            timeout=args.timeout,
-                                            check=args.check,
-                                            text=True)
-                else:
-                    result = subprocess.run(args.command,
-                                            capture_output=True,
-                                            shell=False,
-                                            timeout=args.timeout,
-                                            check=args.check,
-                                            text=True)
-                if result.returncode == 0:
-                    print(result.stdout)
+                command = command_str if args.shell else args.command
+                result = subprocess.run(command,
+                                        capture_output=True,
+                                        shell=args.shell,
+                                        timeout=args.timeout,
+                                        check=args.check,
+                                        text=True)
+                output = result.stdout if result.returncode == 0 and args.check else result.stdout
+                print(output)
             except FileNotFoundError:
                 print("Command not found")
             except subprocess.CalledProcessError as called_process_err:
                 print(
                     f"Command returned non-zero exit status {called_process_err.returncode}"
                 )
                 print(f"stderr: {called_process_err.stderr}")
```

### Comparing `CommandAlarm-0.2.0/setup.py` & `CommandAlarm-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CommandAlarm",
-    version="0.2.0",
+    version="0.2.1",
     author="alofgren",
     author_email="drelofren@outlook.com",
     description="A simple command line program that allows users to set an alarm with a custom command.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alofgren/commandalarm",
     packages=setuptools.find_packages(),
```

