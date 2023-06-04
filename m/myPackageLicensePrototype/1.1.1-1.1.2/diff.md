# Comparing `tmp/myPackageLicensePrototype-1.1.1.tar.gz` & `tmp/myPackageLicensePrototype-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myPackageLicensePrototype-1.1.1.tar", last modified: Sun Jun  4 13:53:01 2023, max compression
+gzip compressed data, was "myPackageLicensePrototype-1.1.2.tar", last modified: Sun Jun  4 13:56:40 2023, max compression
```

## Comparing `myPackageLicensePrototype-1.1.1.tar` & `myPackageLicensePrototype-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 13:53:01.612264 myPackageLicensePrototype-1.1.1/
--rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.1/Implementation.ipynb
--rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      133 2023-06-04 13:53:01.612264 myPackageLicensePrototype-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      140 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.1/PackageContent.py
--rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 myPackageLicensePrototype-1.1.1/README.md
--rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.1.1/__init__.py
--rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.1.1/local_environment_installation_guide.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 13:53:01.612264 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-04 13:53:00.000000 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-06-04 13:53:01.000000 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:53:00.000000 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 13:53:00.000000 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-04 13:53:00.000000 myPackageLicensePrototype-1.1.1/myPackageLicensePrototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 13:53:01.616263 myPackageLicensePrototype-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-06-04 13:52:43.000000 myPackageLicensePrototype-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:56:40.805984 myPackageLicensePrototype-1.1.2/
+-rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.2/Implementation.ipynb
+-rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      133 2023-06-04 13:56:40.805472 myPackageLicensePrototype-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 myPackageLicensePrototype-1.1.2/README.md
+-rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.1.2/__init__.py
+-rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.1.2/local_environment_installation_guide.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 13:56:40.784866 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-06-04 13:56:40.000000 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-06-04 13:56:40.000000 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 13:56:40.000000 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 13:56:40.000000 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-04 13:56:40.000000 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 13:56:40.805984 myPackageLicensePrototype-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2023-06-04 13:56:22.000000 myPackageLicensePrototype-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:56:40.801047 myPackageLicensePrototype-1.1.2/src/
+-rw-rw-rw-   0        0        0      140 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.2/src/PackageContent.py
+-rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.1.2/src/__init__.py
```

### Comparing `myPackageLicensePrototype-1.1.1/Implementation.ipynb` & `myPackageLicensePrototype-1.1.2/Implementation.ipynb`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.1.1/LICENSE` & `myPackageLicensePrototype-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.1.1/local_environment_installation_guide.txt` & `myPackageLicensePrototype-1.1.2/local_environment_installation_guide.txt`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.1.1/setup.py` & `myPackageLicensePrototype-1.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 import codecs
 import chardet
 
 def get_encoding(file):
     with open(file, 'rb') as f:
         return chardet.detect(f.read())['encoding']
 
 encoding = get_encoding('requirements.txt')
 install_requires = codecs.open('requirements.txt', 'r', encoding=encoding).read().splitlines()
  
 setup(
     name='myPackageLicensePrototype',
-    version='1.1.1',
+    version='1.1.2',
     description='Description of your package',
     install_requires=install_requires,
-    ppackage_data={'': ['src/*.py']}
+    packages=find_packages(),
 )
 
 
 # from setuptools import setup, find_packages
 
 #from myPackageLicensePrototype import __version__
```

