# Comparing `tmp/ascvid-1.5.2.tar.gz` & `tmp/ascvid-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascvid-1.5.2.tar", last modified: Sun Jun  4 19:36:10 2023, max compression
+gzip compressed data, was "ascvid-1.5.3.tar", last modified: Sun Jun  4 19:37:07 2023, max compression
```

## Comparing `ascvid-1.5.2.tar` & `ascvid-1.5.3.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:36:10.963504 ascvid-1.5.2/
--rw-r--r--   0 adam      (1003) adam      (1003)    35149 2023-04-05 16:13:01.000000 ascvid-1.5.2/LICENSE
--rw-r--r--   0 adam      (1003) adam      (1003)     3522 2023-06-04 19:36:10.963504 ascvid-1.5.2/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)     2769 2023-04-12 06:00:06.000000 ascvid-1.5.2/README.rst
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:36:10.960171 ascvid-1.5.2/ascvid/
--rw-r--r--   0 adam      (1003) adam      (1003)       22 2023-04-06 09:16:15.000000 ascvid-1.5.2/ascvid/__init__.py
--rw-r--r--   0 adam      (1003) adam      (1003)       59 2023-04-05 16:35:01.000000 ascvid-1.5.2/ascvid/__main__.py
--rw-r--r--   0 adam      (1003) adam      (1003)      819 2023-04-10 19:20:07.000000 ascvid-1.5.2/ascvid/audio.py
--rw-r--r--   0 adam      (1003) adam      (1003)     3160 2023-04-12 05:41:10.000000 ascvid-1.5.2/ascvid/cli.py
--rw-r--r--   0 adam      (1003) adam      (1003)     1130 2023-04-08 09:37:55.000000 ascvid-1.5.2/ascvid/getcol.py
--rw-r--r--   0 adam      (1003) adam      (1003)      519 2023-04-06 15:39:53.000000 ascvid-1.5.2/ascvid/logger.py
--rw-r--r--   0 adam      (1003) adam      (1003)     6641 2023-05-08 15:25:52.000000 ascvid-1.5.2/ascvid/player.py
--rw-r--r--   0 adam      (1003) adam      (1003)     1314 2023-04-08 16:17:56.000000 ascvid-1.5.2/ascvid/run_terminal.py
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:36:10.963504 ascvid-1.5.2/ascvid/subs/
--rw-r--r--   0 adam      (1003) adam      (1003)       35 2023-04-12 05:30:19.000000 ascvid-1.5.2/ascvid/subs/__init__.py
--rw-r--r--   0 adam      (1003) adam      (1003)      394 2023-04-12 05:44:01.000000 ascvid-1.5.2/ascvid/subs/find_format.py
--rw-r--r--   0 adam      (1003) adam      (1003)      641 2023-04-12 16:41:51.000000 ascvid-1.5.2/ascvid/timer.py
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:36:10.963504 ascvid-1.5.2/ascvid/utils/
--rw-r--r--   0 adam      (1003) adam      (1003)      701 2023-04-12 05:18:59.000000 ascvid-1.5.2/ascvid/utils/html2curses.py
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:36:10.963504 ascvid-1.5.2/ascvid.egg-info/
--rw-r--r--   0 adam      (1003) adam      (1003)     3522 2023-06-04 19:36:10.000000 ascvid-1.5.2/ascvid.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)      446 2023-06-04 19:36:10.000000 ascvid-1.5.2/ascvid.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-06-04 19:36:10.000000 ascvid-1.5.2/ascvid.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       43 2023-06-04 19:36:10.000000 ascvid-1.5.2/ascvid.egg-info/entry_points.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       57 2023-06-04 19:36:10.000000 ascvid-1.5.2/ascvid.egg-info/requires.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-06-04 19:36:10.000000 ascvid-1.5.2/ascvid.egg-info/top_level.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-06-04 19:36:10.963504 ascvid-1.5.2/setup.cfg
--rw-r--r--   0 adam      (1003) adam      (1003)     3748 2023-06-04 19:35:51.000000 ascvid-1.5.2/setup.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:37:07.450092 ascvid-1.5.3/
+-rw-r--r--   0 adam      (1003) adam      (1003)    35149 2023-04-05 16:13:01.000000 ascvid-1.5.3/LICENSE
+-rw-r--r--   0 adam      (1003) adam      (1003)     3522 2023-06-04 19:37:07.450092 ascvid-1.5.3/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)     2769 2023-04-12 06:00:06.000000 ascvid-1.5.3/README.rst
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:37:07.446759 ascvid-1.5.3/ascvid/
+-rw-r--r--   0 adam      (1003) adam      (1003)       22 2023-04-06 09:16:15.000000 ascvid-1.5.3/ascvid/__init__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)       59 2023-04-05 16:35:01.000000 ascvid-1.5.3/ascvid/__main__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      819 2023-04-10 19:20:07.000000 ascvid-1.5.3/ascvid/audio.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     3160 2023-04-12 05:41:10.000000 ascvid-1.5.3/ascvid/cli.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     1130 2023-04-08 09:37:55.000000 ascvid-1.5.3/ascvid/getcol.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      519 2023-04-06 15:39:53.000000 ascvid-1.5.3/ascvid/logger.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     6641 2023-05-08 15:25:52.000000 ascvid-1.5.3/ascvid/player.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     1314 2023-04-08 16:17:56.000000 ascvid-1.5.3/ascvid/run_terminal.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:37:07.446759 ascvid-1.5.3/ascvid/subs/
+-rw-r--r--   0 adam      (1003) adam      (1003)       35 2023-04-12 05:30:19.000000 ascvid-1.5.3/ascvid/subs/__init__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      394 2023-04-12 05:44:01.000000 ascvid-1.5.3/ascvid/subs/find_format.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:37:07.450092 ascvid-1.5.3/ascvid/subs/srt/
+-rw-r--r--   0 adam      (1003) adam      (1003)     3169 2023-04-12 05:50:45.000000 ascvid-1.5.3/ascvid/subs/srt/__init__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      641 2023-04-12 16:41:51.000000 ascvid-1.5.3/ascvid/timer.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:37:07.450092 ascvid-1.5.3/ascvid/utils/
+-rw-r--r--   0 adam      (1003) adam      (1003)      701 2023-04-12 05:18:59.000000 ascvid-1.5.3/ascvid/utils/html2curses.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:37:07.446759 ascvid-1.5.3/ascvid.egg-info/
+-rw-r--r--   0 adam      (1003) adam      (1003)     3522 2023-06-04 19:37:07.000000 ascvid-1.5.3/ascvid.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)      474 2023-06-04 19:37:07.000000 ascvid-1.5.3/ascvid.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-06-04 19:37:07.000000 ascvid-1.5.3/ascvid.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       43 2023-06-04 19:37:07.000000 ascvid-1.5.3/ascvid.egg-info/entry_points.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       57 2023-06-04 19:37:07.000000 ascvid-1.5.3/ascvid.egg-info/requires.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-06-04 19:37:07.000000 ascvid-1.5.3/ascvid.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-06-04 19:37:07.450092 ascvid-1.5.3/setup.cfg
+-rw-r--r--   0 adam      (1003) adam      (1003)     3766 2023-06-04 19:37:02.000000 ascvid-1.5.3/setup.py
```

### Comparing `ascvid-1.5.2/LICENSE` & `ascvid-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.2/PKG-INFO` & `ascvid-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascvid
-Version: 1.5.2
+Version: 1.5.3
 Summary: ASCII Video player.
 Home-page: https://github.com/jenca-adam/ascvid
 Author: Adam Jenca
 Author-email: jenca.a@gjh.sk
 Keywords: Video,ASCII,Terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `ascvid-1.5.2/README.rst` & `ascvid-1.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.2/ascvid/audio.py` & `ascvid-1.5.3/ascvid/audio.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.2/ascvid/cli.py` & `ascvid-1.5.3/ascvid/cli.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.2/ascvid/getcol.py` & `ascvid-1.5.3/ascvid/getcol.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.2/ascvid/logger.py` & `ascvid-1.5.3/ascvid/logger.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.2/ascvid/player.py` & `ascvid-1.5.3/ascvid/player.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.2/ascvid/run_terminal.py` & `ascvid-1.5.3/ascvid/run_terminal.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.2/ascvid/timer.py` & `ascvid-1.5.3/ascvid/timer.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.2/ascvid/utils/html2curses.py` & `ascvid-1.5.3/ascvid/utils/html2curses.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.2/ascvid.egg-info/PKG-INFO` & `ascvid-1.5.3/ascvid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascvid
-Version: 1.5.2
+Version: 1.5.3
 Summary: ASCII Video player.
 Home-page: https://github.com/jenca-adam/ascvid
 Author: Adam Jenca
 Author-email: jenca.a@gjh.sk
 Keywords: Video,ASCII,Terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `ascvid-1.5.2/setup.py` & `ascvid-1.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-setuptools.setup(name="ascvid",version="1.5.2",description="ASCII Video player.", long_description=
+setuptools.setup(name="ascvid",version="1.5.3",description="ASCII Video player.", long_description=
                  """
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/asc.png
 
 ``ascvid`` is an ASCII video player with quite exact results. It is mostly advised to be used under Linux, but it might work on Windows too (its behavior under Mac is untested, and it will likely not work well).
 Here is a little showcase of what it can do: 
 
 .. image:: https://raw.githubusercontent.com/jenca-adam/ascvid/main/rick.gif
@@ -57,15 +57,15 @@
       -d, --debug             Debug mode: show current/target fps
       -s, --subs              Subtitle file to use
 
       --help                  Show this message and exit.
    
     """,
                  install_requires=["pillow","moviepy","cursor","numpy","click","sounddevice","av","imageio"],
-                 packages=["ascvid","ascvid.subs","ascvid.utils"],
+                 packages=["ascvid","ascvid.subs","ascvid.utils","ascvid.subs.srt"],
                  classifiers=["Development Status :: 4 - Beta","Environment :: Console","Intended Audience :: End Users/Desktop","License :: OSI Approved :: GNU General Public License v3 (GPLv3)","Operating System :: Microsoft :: Windows","Operating System :: POSIX :: Linux","Operating System :: Unix","Programming Language :: Python :: 3.10","Topic :: Multimedia :: Video :: Display"],keywords="Video,ASCII,Terminal",author="Adam Jenca",author_email="jenca.a@gjh.sk",url="https://github.com/jenca-adam/ascvid",entry_points={"console_scripts":["ascvid = ascvid.cli:main"]})
```

