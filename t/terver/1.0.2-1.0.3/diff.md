# Comparing `tmp/terver-1.0.2.tar.gz` & `tmp/terver-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\terver-1.0.2.tar", last modified: Sun Jun  4 11:47:03 2023, max compression
+gzip compressed data, was "dist\terver-1.0.3.tar", last modified: Sun Jun  4 20:28:13 2023, max compression
```

## Comparing `terver-1.0.2.tar` & `terver-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 11:47:03.000000 terver-1.0.2/
--rw-rw-rw-   0        0        0        0 2023-06-04 10:55:11.000000 terver-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      386 2023-06-04 11:47:03.000000 terver-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-04 10:55:23.000000 terver-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-04 11:47:03.000000 terver-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      615 2023-06-04 11:47:00.000000 terver-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:47:03.000000 terver-1.0.2/terver/
--rw-rw-rw-   0        0        0       19 2023-06-04 11:46:49.000000 terver-1.0.2/terver/__init__.py
--rw-rw-rw-   0        0        0     3031 2023-06-04 11:30:12.000000 terver-1.0.2/terver/main.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:47:03.000000 terver-1.0.2/terver.egg-info/
--rw-rw-rw-   0        0        0      386 2023-06-04 11:47:02.000000 terver-1.0.2/terver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-06-04 11:47:02.000000 terver-1.0.2/terver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 11:47:02.000000 terver-1.0.2/terver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-04 11:47:02.000000 terver-1.0.2/terver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-04 11:47:02.000000 terver-1.0.2/terver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 20:28:13.000000 terver-1.0.3/
+-rw-rw-rw-   0        0        0        0 2023-06-04 10:55:11.000000 terver-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      386 2023-06-04 20:28:13.000000 terver-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-04 10:55:23.000000 terver-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 20:28:13.000000 terver-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      615 2023-06-04 20:27:52.000000 terver-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:28:13.000000 terver-1.0.3/terver/
+-rw-rw-rw-   0        0        0       19 2023-06-04 11:46:49.000000 terver-1.0.3/terver/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-06-04 20:27:40.000000 terver-1.0.3/terver/main.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:28:13.000000 terver-1.0.3/terver.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-06-04 20:28:13.000000 terver-1.0.3/terver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-06-04 20:28:13.000000 terver-1.0.3/terver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 20:28:13.000000 terver-1.0.3/terver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-04 20:28:13.000000 terver-1.0.3/terver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-04 20:28:13.000000 terver-1.0.3/terver.egg-info/top_level.txt
```

### Comparing `terver-1.0.2/setup.py` & `terver-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='terver',
-  version='1.0.2',
+  version='1.0.3',
   author='qdzzzxc',
   author_email='nikitstp@gmail.com',
   description='xD',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['pyperclip>=1.8.2'],
```

