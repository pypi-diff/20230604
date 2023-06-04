# Comparing `tmp/ascvid-1.5.0.tar.gz` & `tmp/ascvid-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascvid-1.5.0.tar", last modified: Wed Apr 12 06:04:54 2023, max compression
+gzip compressed data, was "ascvid-1.5.1.tar", last modified: Sun Jun  4 19:33:46 2023, max compression
```

## Comparing `ascvid-1.5.0.tar` & `ascvid-1.5.1.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-12 06:04:54.671766 ascvid-1.5.0/
--rw-r--r--   0 adam      (1003) adam      (1003)    35149 2023-04-05 16:13:01.000000 ascvid-1.5.0/LICENSE
--rw-r--r--   0 adam      (1003) adam      (1003)     3522 2023-04-12 06:04:54.671766 ascvid-1.5.0/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)     2769 2023-04-12 06:00:06.000000 ascvid-1.5.0/README.rst
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-12 06:04:54.671766 ascvid-1.5.0/ascvid/
--rw-r--r--   0 adam      (1003) adam      (1003)       22 2023-04-06 09:16:15.000000 ascvid-1.5.0/ascvid/__init__.py
--rw-r--r--   0 adam      (1003) adam      (1003)       59 2023-04-05 16:35:01.000000 ascvid-1.5.0/ascvid/__main__.py
--rw-r--r--   0 adam      (1003) adam      (1003)      819 2023-04-10 19:20:07.000000 ascvid-1.5.0/ascvid/audio.py
--rw-r--r--   0 adam      (1003) adam      (1003)     3160 2023-04-12 05:41:10.000000 ascvid-1.5.0/ascvid/cli.py
--rw-r--r--   0 adam      (1003) adam      (1003)     1130 2023-04-08 09:37:55.000000 ascvid-1.5.0/ascvid/getcol.py
--rw-r--r--   0 adam      (1003) adam      (1003)      519 2023-04-06 15:39:53.000000 ascvid-1.5.0/ascvid/logger.py
--rw-r--r--   0 adam      (1003) adam      (1003)     6522 2023-04-12 05:55:59.000000 ascvid-1.5.0/ascvid/player.py
--rw-r--r--   0 adam      (1003) adam      (1003)     1314 2023-04-08 16:17:56.000000 ascvid-1.5.0/ascvid/run_terminal.py
--rw-r--r--   0 adam      (1003) adam      (1003)      641 2023-04-07 16:55:04.000000 ascvid-1.5.0/ascvid/timer.py
-drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-04-12 06:04:54.671766 ascvid-1.5.0/ascvid.egg-info/
--rw-r--r--   0 adam      (1003) adam      (1003)     3522 2023-04-12 06:04:54.000000 ascvid-1.5.0/ascvid.egg-info/PKG-INFO
--rw-r--r--   0 adam      (1003) adam      (1003)      367 2023-04-12 06:04:54.000000 ascvid-1.5.0/ascvid.egg-info/SOURCES.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-04-12 06:04:54.000000 ascvid-1.5.0/ascvid.egg-info/dependency_links.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       43 2023-04-12 06:04:54.000000 ascvid-1.5.0/ascvid.egg-info/entry_points.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       57 2023-04-12 06:04:54.000000 ascvid-1.5.0/ascvid.egg-info/requires.txt
--rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-04-12 06:04:54.000000 ascvid-1.5.0/ascvid.egg-info/top_level.txt
--rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-04-12 06:04:54.671766 ascvid-1.5.0/setup.cfg
--rw-r--r--   0 adam      (1003) adam      (1003)     3719 2023-04-12 06:02:22.000000 ascvid-1.5.0/setup.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:33:46.390354 ascvid-1.5.1/
+-rw-r--r--   0 adam      (1003) adam      (1003)    35149 2023-04-05 16:13:01.000000 ascvid-1.5.1/LICENSE
+-rw-r--r--   0 adam      (1003) adam      (1003)     3522 2023-06-04 19:33:46.390354 ascvid-1.5.1/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)     2769 2023-04-12 06:00:06.000000 ascvid-1.5.1/README.rst
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:33:46.390354 ascvid-1.5.1/ascvid/
+-rw-r--r--   0 adam      (1003) adam      (1003)       22 2023-04-06 09:16:15.000000 ascvid-1.5.1/ascvid/__init__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)       59 2023-04-05 16:35:01.000000 ascvid-1.5.1/ascvid/__main__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      819 2023-04-10 19:20:07.000000 ascvid-1.5.1/ascvid/audio.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     3160 2023-04-12 05:41:10.000000 ascvid-1.5.1/ascvid/cli.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     1130 2023-04-08 09:37:55.000000 ascvid-1.5.1/ascvid/getcol.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      519 2023-04-06 15:39:53.000000 ascvid-1.5.1/ascvid/logger.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     6641 2023-05-08 15:25:52.000000 ascvid-1.5.1/ascvid/player.py
+-rw-r--r--   0 adam      (1003) adam      (1003)     1314 2023-04-08 16:17:56.000000 ascvid-1.5.1/ascvid/run_terminal.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:33:46.390354 ascvid-1.5.1/ascvid/subs/
+-rw-r--r--   0 adam      (1003) adam      (1003)       35 2023-04-12 05:30:19.000000 ascvid-1.5.1/ascvid/subs/__init__.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      394 2023-04-12 05:44:01.000000 ascvid-1.5.1/ascvid/subs/find_format.py
+-rw-r--r--   0 adam      (1003) adam      (1003)      641 2023-04-12 16:41:51.000000 ascvid-1.5.1/ascvid/timer.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:33:46.390354 ascvid-1.5.1/ascvid/utils/
+-rw-r--r--   0 adam      (1003) adam      (1003)      701 2023-04-12 05:18:59.000000 ascvid-1.5.1/ascvid/utils/html2curses.py
+drwxr-xr-x   0 adam      (1003) adam      (1003)        0 2023-06-04 19:33:46.390354 ascvid-1.5.1/ascvid.egg-info/
+-rw-r--r--   0 adam      (1003) adam      (1003)     3522 2023-06-04 19:33:46.000000 ascvid-1.5.1/ascvid.egg-info/PKG-INFO
+-rw-r--r--   0 adam      (1003) adam      (1003)      446 2023-06-04 19:33:46.000000 ascvid-1.5.1/ascvid.egg-info/SOURCES.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        1 2023-06-04 19:33:46.000000 ascvid-1.5.1/ascvid.egg-info/dependency_links.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       43 2023-06-04 19:33:46.000000 ascvid-1.5.1/ascvid.egg-info/entry_points.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       57 2023-06-04 19:33:46.000000 ascvid-1.5.1/ascvid.egg-info/requires.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)        7 2023-06-04 19:33:46.000000 ascvid-1.5.1/ascvid.egg-info/top_level.txt
+-rw-r--r--   0 adam      (1003) adam      (1003)       38 2023-06-04 19:33:46.390354 ascvid-1.5.1/setup.cfg
+-rw-r--r--   0 adam      (1003) adam      (1003)     3748 2023-06-04 19:33:22.000000 ascvid-1.5.1/setup.py
```

### Comparing `ascvid-1.5.0/LICENSE` & `ascvid-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.0/PKG-INFO` & `ascvid-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascvid
-Version: 1.5.0
+Version: 1.5.1
 Summary: ASCII Video player.
 Home-page: https://github.com/jenca-adam/ascvid
 Author: Adam Jenca
 Author-email: jenca.a@gjh.sk
 Keywords: Video,ASCII,Terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `ascvid-1.5.0/README.rst` & `ascvid-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.0/ascvid/audio.py` & `ascvid-1.5.1/ascvid/audio.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.0/ascvid/cli.py` & `ascvid-1.5.1/ascvid/cli.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.0/ascvid/getcol.py` & `ascvid-1.5.1/ascvid/getcol.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.0/ascvid/logger.py` & `ascvid-1.5.1/ascvid/logger.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.0/ascvid/player.py` & `ascvid-1.5.1/ascvid/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     if use_ascii:
         return get_character(color,colored,truecolor)
     if truecolor:
         r,g,b=color
         return f"\x1b[38;2;{r};{g};{b}m{char}"
     return f"{closest(color)}{char}"
 
-def show_frame(fr,char,colored,truecolor,use_ascii,resize,hast,tit,out,fps,nfps,deb,subs,ttt,dur):
+def show_frame(fr,char,colored,truecolor,use_ascii,resize,hast,tit,out,fps,nfps,deb,subs,ttt,dur,avg):
     ts=os.get_terminal_size()
     tw=ts.columns
     th=ts.lines
     if deb:
         th-=1
    
  
@@ -107,15 +107,15 @@
             r,g,b,*foo=pix[x,y]
             line+=get_pixel((r,g,b),colored,truecolor,use_ascii,char)
         lines.append(line+'\x1b[0m')
     clear(out)
     if hast:
         print(tit,file=out,flush=True)
     if deb:
-        print(f"{ttt:.2f}/{dur}@ {fps:.2f} FPS  => {nfps} FPS",flush=True,file=out)
+        print(f"{ttt:.2f}/{dur}@ {fps:.2f} FPS ({avg} AVG)  => {nfps} FPS",flush=True,file=out)
     print('\n'.join(lines),end="",file=out)
     if subs:
         print("\n"+subs.get_sub(ttt),end="",file=out)
 def mkpos(a):
     if a<0:
         return 0
     return a
@@ -141,15 +141,15 @@
     q=queue.Queue()
     dur=vid.get_meta_data().get("duration",float("inf"))
     settings=None
     if sys.platform.lower().startswith("linux"):
         import tty
         import termios
         settings=termios.tcgetattr(sys.stdin)
-
+    fpsum=0
     if fast:
         frame_count=vid.count_frames()
         if frame_count>=10000:
             response=print_warning(f"{file!r} has {frame_count} frames.",ask="Are you sure you want to resize them all at once [y*]")
             if response!="y":
                 sys.exit(1)
         tw=os.get_terminal_size().columns
@@ -206,18 +206,20 @@
                         audio_stream.pause()
                     while q.get()!=" ":
                         pass
                     if audio_stream is not None:
                         audio_stream.resume()
                     frame_timer.start()
             current_fps=frindex/frame_timer.curtime
-            show_frame(frame,char,colored,truecolor,use_ascii,not fast,show_title,title,out,current_fps,fps,show_dbg,subs,frame_timer.curtime,dur)
+            avgfps=0 if frindex==0 else fpsum/frindex
+            show_frame(frame,char,colored,truecolor,use_ascii,not fast,show_title,title,out,current_fps,fps,show_dbg,subs,frame_timer.curtime,dur,avgfps)
             if fps!="max" and current_fps>fps:
                 time.sleep(mkpos(1/fps))
             frindex+=1
+            fpsum+=current_fps
     except KeyboardInterrupt:
         clear(out)
     finally:
         cursor.show()
         out.write("\x1b[0m")
         out.flush()
         if settings is not None:
```

### Comparing `ascvid-1.5.0/ascvid/run_terminal.py` & `ascvid-1.5.1/ascvid/run_terminal.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.0/ascvid/timer.py` & `ascvid-1.5.1/ascvid/timer.py`

 * *Files identical despite different names*

### Comparing `ascvid-1.5.0/ascvid.egg-info/PKG-INFO` & `ascvid-1.5.1/ascvid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascvid
-Version: 1.5.0
+Version: 1.5.1
 Summary: ASCII Video player.
 Home-page: https://github.com/jenca-adam/ascvid
 Author: Adam Jenca
 Author-email: jenca.a@gjh.sk
 Keywords: Video,ASCII,Terminal
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `ascvid-1.5.0/setup.py` & `ascvid-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-setuptools.setup(name="ascvid",version="1.5.0",description="ASCII Video player.", long_description=
+setuptools.setup(name="ascvid",version="1.5.1",description="ASCII Video player.", long_description=
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
-                 packages=["ascvid"],
+                 packages=["ascvid","ascvid.subs","ascvid.utils"],
                  classifiers=["Development Status :: 4 - Beta","Environment :: Console","Intended Audience :: End Users/Desktop","License :: OSI Approved :: GNU General Public License v3 (GPLv3)","Operating System :: Microsoft :: Windows","Operating System :: POSIX :: Linux","Operating System :: Unix","Programming Language :: Python :: 3.10","Topic :: Multimedia :: Video :: Display"],keywords="Video,ASCII,Terminal",author="Adam Jenca",author_email="jenca.a@gjh.sk",url="https://github.com/jenca-adam/ascvid",entry_points={"console_scripts":["ascvid = ascvid.cli:main"]})
```

