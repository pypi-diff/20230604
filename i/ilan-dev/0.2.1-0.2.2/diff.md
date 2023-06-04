# Comparing `tmp/ilan-dev-0.2.1.tar.gz` & `tmp/ilan-dev-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ilan-dev-0.2.1.tar", last modified: Sun Mar 26 04:46:39 2023, max compression
+gzip compressed data, was "ilan-dev-0.2.2.tar", last modified: Sun Jun  4 05:29:45 2023, max compression
```

## Comparing `ilan-dev-0.2.1.tar` & `ilan-dev-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2023-03-26 04:46:39.000000 ilan-dev-0.2.1/
--rw-r--r--   0 ilan       (501) staff       (20)      898 2023-03-26 04:46:39.000000 ilan-dev-0.2.1/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)     1448 2023-03-04 05:09:39.000000 ilan-dev-0.2.1/ilan_dev.py
--rw-r--r--   0 ilan       (501) staff       (20)      851 2023-03-03 22:48:35.000000 ilan-dev-0.2.1/setup.py
--rwxr-xr-x   0 ilan       (501) staff       (20)     2746 2023-03-03 02:14:37.000000 ilan-dev-0.2.1/cleanup
--rwxr-xr-x   0 ilan       (501) staff       (20)     5101 2023-03-24 04:53:02.000000 ilan-dev-0.2.1/tarinfo
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2023-03-26 04:46:39.000000 ilan-dev-0.2.1/ilan_dev.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)      898 2023-03-26 04:46:39.000000 ilan-dev-0.2.1/ilan_dev.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      187 2023-03-26 04:46:39.000000 ilan-dev-0.2.1/ilan_dev.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        9 2023-03-26 04:46:39.000000 ilan-dev-0.2.1/ilan_dev.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2023-03-26 04:46:39.000000 ilan-dev-0.2.1/ilan_dev.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2023-03-26 04:46:39.000000 ilan-dev-0.2.1/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      219 2023-03-03 22:47:13.000000 ilan-dev-0.2.1/README.rst
--rw-r--r--   0 ilan       (501) staff       (20)     1520 2023-02-27 03:12:59.000000 ilan-dev-0.2.1/LICENSE.txt
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2023-06-04 05:29:45.053578 ilan-dev-0.2.2/
+-rw-r--r--   0 ilan       (501) staff       (20)     1520 2023-02-27 03:12:59.000000 ilan-dev-0.2.2/LICENSE.txt
+-rw-r--r--   0 ilan       (501) staff       (20)      797 2023-06-04 05:29:45.053258 ilan-dev-0.2.2/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      219 2023-03-03 22:47:13.000000 ilan-dev-0.2.2/README.rst
+-rwxr-xr-x   0 ilan       (501) staff       (20)     2940 2023-04-13 03:50:37.000000 ilan-dev-0.2.2/cleanup
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2023-06-04 05:29:45.052754 ilan-dev-0.2.2/ilan_dev.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)      797 2023-06-04 05:29:44.000000 ilan-dev-0.2.2/ilan_dev.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      187 2023-06-04 05:29:44.000000 ilan-dev-0.2.2/ilan_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2023-06-04 05:29:44.000000 ilan-dev-0.2.2/ilan_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        9 2023-06-04 05:29:44.000000 ilan-dev-0.2.2/ilan_dev.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)     1448 2023-03-26 04:52:33.000000 ilan-dev-0.2.2/ilan_dev.py
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2023-06-04 05:29:45.053683 ilan-dev-0.2.2/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      851 2023-03-03 22:48:35.000000 ilan-dev-0.2.2/setup.py
+-rwxr-xr-x   0 ilan       (501) staff       (20)     5737 2023-05-04 20:37:21.000000 ilan-dev-0.2.2/tarinfo
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ilan-dev-0.2.1/ilan_dev.py` & `ilan-dev-0.2.2/ilan_dev.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from posixpath import dirname
 
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 
 def lcp(a):
     """
     return longest common prefix of iterable of strings,
     or None when iterable is exhausted immediately
     """
```

### Comparing `ilan-dev-0.2.1/setup.py` & `ilan-dev-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `ilan-dev-0.2.1/cleanup` & `ilan-dev-0.2.2/cleanup`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 #!/usr/bin/env python
 import os
 import string
+from argparse import ArgumentParser
+from fnmatch import fnmatch
 from os.path import basename, join, isfile, isdir
-from optparse import OptionParser
 
 
 ASCII_ONLY = False
+VERBOSE = False
 
 # file extensions which are cleaned when using the -r option
-FILE_EXT = ('.py', '.txt', '.c', '.h', '.pyx', '.pyi', '.json',
+FILE_EXT = ('.py', '.txt', '.c', '.h', '.pyx', '.pyi', '.sh',
             '.yml', '.yaml', '.md', '.rst', '.md', '.xml')
 
+# directories being ignored
+IGNORE_DIRS = ('.git', '__pycache__', '*.egg-info')
+
 
 def cleanup(data, expand_tabs=True):
     if data == '':
         return ''
 
     data = data.replace('\r', '')
     data = '\n'.join(line.rstrip() for line in data.split('\n'))
@@ -29,14 +34,16 @@
     if not data.endswith('\n'):
         data += '\n'
 
     return data
 
 
 def clean_file(path):
+    if VERBOSE:
+        print(path)
     if not isfile(path):
         print("Ignoring non-existing file: %s" % path)
         return
 
     with open(path, 'r') as fi:
         old_data = fi.read()
 
@@ -52,59 +59,60 @@
 
 def clean_dir(dir_path):
     if not isdir(dir_path):
         print("Not a directory: %s" % dir_path)
         return
 
     for root, dirs, files in os.walk(dir_path):
-        parts = root.split(os.sep)
-        if '.git' in parts:
-            continue
+        for dn in list(dirs):
+            if any(fnmatch(dn, pat) for pat in IGNORE_DIRS):
+                dirs.remove(dn)
 
         for fn in files:
             if fn.endswith(FILE_EXT):
                 path = join(root, fn)
                 clean_file(path)
 
 
 def main():
-    p = OptionParser(
-        usage="usage: %prog [options] FILE [FILE ...]",
-        description=("Cleanup whitespace in FILE, that is: "
-                     "remove carriage returns; "
-                     "remove excess whitespace at the end of each line; "
-                     "expand tabs (to 8 spaces), but not a Makefile; "
-                     "make sure file has a newline at the end"))
-
-    p.add_option("--ascii-only",
-                 action="store_true",
-                 help="allow only ASCII bytes (removes others)")
-
-    p.add_option('-r', "--recur",
-                 action="store_true",
-                 help="cleanup recursively")
+    p = ArgumentParser(description=("""
+Cleanup whitespace in FILE, that is:
+(a) remove carriage returns
+(b) remove excess whitespace at the end of each line
+(c) expand tabs (to 8 spaces), but not in a Makefile
+(d) make sure file has a newline at the end
+"""))
+    p.add_argument("--ascii-only", action="store_true",
+                   help="allow only ASCII bytes (removes others)")
+
+    p.add_argument('-r', "--recur", action="store_true",
+                   help="cleanup recursively")
+
+    p.add_argument('-v', "--verbose", action="store_true")
 
-    p.add_option("--version",
-                 action="store_true")
+    p.add_argument("--version", action="store_true")
 
-    opts, args = p.parse_args()
+    p.add_argument(dest='paths', metavar='FILE', nargs='*')
 
-    if opts.version:
+    args = p.parse_args()
+
+    if args.version:
         import ilan_dev
         print("ilan-dev: %s" % ilan_dev.__version__)
         return
 
-    global ASCII_ONLY
-    ASCII_ONLY = opts.ascii_only
-
-    if opts.recur:
-        if len(args) == 0:
-            args = ['.']
-        for path in args:
+    global ASCII_ONLY, VERBOSE
+    ASCII_ONLY = args.ascii_only
+    VERBOSE = args.verbose
+
+    if args.recur:
+        if not args.paths:
+            args.paths.append('.')
+        for path in args.paths:
             clean_dir(path)
     else:
-        for path in args:
+        for path in args.paths:
             clean_file(path)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ilan-dev-0.2.1/tarinfo` & `ilan-dev-0.2.2/tarinfo`

 * *Files 15% similar despite different names*

```diff
@@ -73,38 +73,52 @@
     print("          directories: %7d" % ndirs)
     print("           empty dirs: %7d" % len(empty))
     print("         missing dirs: %7d" % len(missing))
     print("       total archives: %7d" % len(names))
     print("           total size: %7s" % human_bytes(size))
     print("longest common prefix: %r" % lcp([name for name, _ in names]))
 
+def tar_select(name, path):
+    try:
+        with tarfile.open(path) as t:
+            data = t.extractfile(name).read()
+    except KeyError as e:
+        print("Error: %s" % e)
+        return
+    try:
+        print(data.decode())
+    except UnicodeDecodeError:
+        print("size: %d bytes" % len(data))
+        print(data[:256])
+
 def help():
     print("""\
 usage: %s [options] COMMAND [TAR ...]",
 
 display useful information about tar files
 
 Commands:
-  cext        list Python C extension imports
-  common      list archive name common in all tarballs
-  diff        show difference of two tarballs (compares archive names only)
-  empty       list empty directories
-  missing     list missing directories
-  lcp         show the longest common prefix of all archive names
-  ls          list archive members, similar to 'ls -l'
-  stat        display a useful summart of information
-  size        list file sizes of all archives (sorted by size)
+  cext          list Python C extension imports
+  common        list archive name common in all tarballs
+  diff          show difference of two tarballs (compares archive names only)
+  empty         list empty directories
+  missing       list missing directories
+  lcp           show the longest common prefix of all archive names
+  ls            list archive members, similar to 'ls -l'
+  select NAME   show content of archive NAME
+  stat          display a useful summart of information
+  size          list file sizes of all archives (sorted by size)
 
 Options:
   -h, --help  show this help message and exit
   --version
 """ % basename(sys.argv[0]))
 
 CMDS = ['cext', 'common', 'diff', 'empty', 'missing',
-        'lcp', 'ls', 'stat', 'size']
+        'lcp', 'ls', 'select', 'stat', 'size']
 
 def check_commamd(cmd):
     if cmd in CMDS:
         return
     print("no such command: %r" % cmd)
     close_matches = difflib.get_close_matches(cmd, CMDS)
     if close_matches:
@@ -136,14 +150,19 @@
 
     if cmd == 'diff':
         if len(args) != 2:
             sys.exit("'diff' requires exactly two tar archives, try --help")
         tar_diff(*args)
         return
 
+    if cmd == 'select':
+        if len(args) == 0:
+            sys.exit("'select' requires NAME, try --help")
+        archive_name, args = args[0], args[1:]
+
     for path in args:
         if not isfile(path):
             sys.exit("no such file: %r" % path)
 
         if len(args) > 1:
             print("==> %s <==" % path)
 
@@ -159,14 +178,17 @@
             if s:
                 print(s)
 
         if cmd == 'ls':
             with tarfile.open(path) as t:
                 t.list()
 
+        if cmd == 'select':
+            tar_select(archive_name, path)
+
         if cmd == 'size':
             with tarfile.open(path) as t:
                 lst = [(m.size, m.name) for m in t.getmembers()]
             for size, name in sorted(lst):
                 print("%-60s %10s" % (name, human_bytes(size)))
 
         if cmd == 'stat':
```

### Comparing `ilan-dev-0.2.1/LICENSE.txt` & `ilan-dev-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

