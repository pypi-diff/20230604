# Comparing `tmp/myPackageLicensePrototype-1.1.0.tar.gz` & `tmp/myPackageLicensePrototype-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myPackageLicensePrototype-1.1.0.tar", last modified: Sun Jun  4 13:43:37 2023, max compression
+gzip compressed data, was "myPackageLicensePrototype-1.1.1.tar", last modified: Sun Jun  4 13:53:01 2023, max compression
```

## Comparing `myPackageLicensePrototype-1.1.0.tar` & `myPackageLicensePrototype-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 13:43:37.347560 myPackageLicensePrototype-1.1.0/
--rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.0/Implementation.ipynb
--rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      133 2023-06-04 13:43:37.347560 myPackageLicensePrototype-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      140 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.0/PackageContent.py
--rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 myPackageLicensePrototype-1.1.0/README.md
--rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.1.0/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:43:37.231618 myPackageLicensePrototype-1.1.0/dist/
--rw-rw-rw-   0        0        0     3154 2023-06-02 09:23:52.000000 myPackageLicensePrototype-1.1.0/dist/myPackageLicensePrototype-1.0.2.tar.gz
--rw-rw-rw-   0        0        0     7119 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.1.0/dist/myPackageLicensePrototype-1.0.3.tar.gz
--rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.1.0/local_environment_installation_guide.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 13:43:37.279487 myPackageLicensePrototype-1.1.0/myPackageLicensePrototype.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.0/myPackageLicensePrototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.0/myPackageLicensePrototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:37:21.000000 myPackageLicensePrototype-1.1.0/myPackageLicensePrototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 13:37:21.000000 myPackageLicensePrototype-1.1.0/myPackageLicensePrototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.0/myPackageLicensePrototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 13:43:37.351570 myPackageLicensePrototype-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-06-04 13:43:18.000000 myPackageLicensePrototype-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:43:37.106699 myPackageLicensePrototype-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 13:43:37.343542 myPackageLicensePrototype-1.1.0/src/myPackageLicensePrototype.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-04 13:43:36.000000 myPackageLicensePrototype-1.1.0/src/myPackageLicensePrototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      731 2023-06-04 13:43:36.000000 myPackageLicensePrototype-1.1.0/src/myPackageLicensePrototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:43:36.000000 myPackageLicensePrototype-1.1.0/src/myPackageLicensePrototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 13:43:36.000000 myPackageLicensePrototype-1.1.0/src/myPackageLicensePrototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:43:36.000000 myPackageLicensePrototype-1.1.0/src/myPackageLicensePrototype.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 13:53:01.612264 myPackageLicensePrototype-1.1.1/
+-rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.1/Implementation.ipynb
+-rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      133 2023-06-04 13:53:01.612264 myPackageLicensePrototype-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.1/PackageContent.py
+-rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 myPackageLicensePrototype-1.1.1/README.md
+-rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.1.1/__init__.py
+-rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.1.1/local_environment_installation_guide.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 13:53:01.612264 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-06-04 13:53:00.000000 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-06-04 13:53:01.000000 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 13:53:00.000000 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 13:53:00.000000 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-04 13:53:00.000000 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 13:53:01.616263 myPackageLicensePrototype-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1365 2023-06-04 13:52:43.000000 myPackageLicensePrototype-1.1.1/setup.py
```

### Comparing `myPackageLicensePrototype-1.1.0/Implementation.ipynb` & `myPackageLicensePrototype-1.1.1/Implementation.ipynb`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.1.0/LICENSE` & `myPackageLicensePrototype-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.1.0/local_environment_installation_guide.txt` & `myPackageLicensePrototype-1.1.1/local_environment_installation_guide.txt`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.1.0/setup.py` & `myPackageLicensePrototype-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         return chardet.detect(f.read())['encoding']
 
 encoding = get_encoding('requirements.txt')
 install_requires = codecs.open('requirements.txt', 'r', encoding=encoding).read().splitlines()
  
 setup(
     name='myPackageLicensePrototype',
-    version='1.1.0',
+    version='1.1.1',
     description='Description of your package',
     install_requires=install_requires,
     ppackage_data={'': ['src/*.py']}
 )
 
 
 # from setuptools import setup, find_packages
```

