# Comparing `tmp/myPackageLicensePrototype-1.0.7.tar.gz` & `tmp/myPackageLicensePrototype-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myPackageLicensePrototype-1.0.7.tar", last modified: Sun Jun  4 13:35:18 2023, max compression
+gzip compressed data, was "myPackageLicensePrototype-1.0.8.tar", last modified: Sun Jun  4 13:37:22 2023, max compression
```

## Comparing `myPackageLicensePrototype-1.0.7.tar` & `myPackageLicensePrototype-1.0.8.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 13:35:18.856000 myPackageLicensePrototype-1.0.7/
--rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      133 2023-06-04 13:35:18.851985 myPackageLicensePrototype-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 myPackageLicensePrototype-1.0.7/README.md
--rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.0.7/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:35:18.763929 myPackageLicensePrototype-1.0.7/dist/
--rw-rw-rw-   0        0        0     3154 2023-06-02 09:23:52.000000 myPackageLicensePrototype-1.0.7/dist/myPackageLicensePrototype-1.0.2.tar.gz
--rw-rw-rw-   0        0        0     7119 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.0.7/dist/myPackageLicensePrototype-1.0.3.tar.gz
--rw-rw-rw-   0        0        0    14524 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.0.7/dist/myPackageLicensePrototype-1.0.4.tar.gz
--rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.0.7/local_environment_installation_guide.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 13:35:18.838806 myPackageLicensePrototype-1.0.7/myPackageLicensePrototype.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-04 13:35:18.000000 myPackageLicensePrototype-1.0.7/myPackageLicensePrototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-06-04 13:35:18.000000 myPackageLicensePrototype-1.0.7/myPackageLicensePrototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:35:18.000000 myPackageLicensePrototype-1.0.7/myPackageLicensePrototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 13:35:18.000000 myPackageLicensePrototype-1.0.7/myPackageLicensePrototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-04 13:35:18.000000 myPackageLicensePrototype-1.0.7/myPackageLicensePrototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 13:35:18.856000 myPackageLicensePrototype-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1373 2023-06-04 13:35:09.000000 myPackageLicensePrototype-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:35:18.847971 myPackageLicensePrototype-1.0.7/src/
--rw-rw-rw-   0        0        0     1026 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.0.7/src/Implementation.ipynb
--rw-rw-rw-   0        0        0      140 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.0.7/src/PackageContent.py
--rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.0.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:37:22.179899 myPackageLicensePrototype-1.0.8/
+-rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      133 2023-06-04 13:37:22.175424 myPackageLicensePrototype-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 myPackageLicensePrototype-1.0.8/README.md
+-rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.0.8/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:37:22.098049 myPackageLicensePrototype-1.0.8/dist/
+-rw-rw-rw-   0        0        0     3154 2023-06-02 09:23:52.000000 myPackageLicensePrototype-1.0.8/dist/myPackageLicensePrototype-1.0.2.tar.gz
+-rw-rw-rw-   0        0        0     7119 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.0.8/dist/myPackageLicensePrototype-1.0.3.tar.gz
+-rw-rw-rw-   0        0        0    14524 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.0.8/dist/myPackageLicensePrototype-1.0.4.tar.gz
+-rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.0.8/local_environment_installation_guide.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 13:37:22.158836 myPackageLicensePrototype-1.0.8/myPackageLicensePrototype.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-06-04 13:37:21.000000 myPackageLicensePrototype-1.0.8/myPackageLicensePrototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2023-06-04 13:37:21.000000 myPackageLicensePrototype-1.0.8/myPackageLicensePrototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 13:37:21.000000 myPackageLicensePrototype-1.0.8/myPackageLicensePrototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 13:37:21.000000 myPackageLicensePrototype-1.0.8/myPackageLicensePrototype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-04 13:37:21.000000 myPackageLicensePrototype-1.0.8/myPackageLicensePrototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 13:37:22.179899 myPackageLicensePrototype-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2023-06-04 13:37:12.000000 myPackageLicensePrototype-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:37:22.171424 myPackageLicensePrototype-1.0.8/src/
+-rw-rw-rw-   0        0        0     1026 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.0.8/src/Implementation.ipynb
+-rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.0.8/src/__init__.py
```

### Comparing `myPackageLicensePrototype-1.0.7/LICENSE` & `myPackageLicensePrototype-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.0.7/dist/myPackageLicensePrototype-1.0.2.tar.gz` & `myPackageLicensePrototype-1.0.8/dist/myPackageLicensePrototype-1.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.0.7/dist/myPackageLicensePrototype-1.0.3.tar.gz` & `myPackageLicensePrototype-1.0.8/dist/myPackageLicensePrototype-1.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.0.7/dist/myPackageLicensePrototype-1.0.4.tar.gz` & `myPackageLicensePrototype-1.0.8/dist/myPackageLicensePrototype-1.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.0.7/local_environment_installation_guide.txt` & `myPackageLicensePrototype-1.0.8/local_environment_installation_guide.txt`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.0.7/setup.py` & `myPackageLicensePrototype-1.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         return chardet.detect(f.read())['encoding']
 
 encoding = get_encoding('requirements.txt')
 install_requires = codecs.open('requirements.txt', 'r', encoding=encoding).read().splitlines()
  
 setup(
     name='myPackageLicensePrototype',
-    version='1.0.7',
+    version='1.0.8',
     description='Description of your package',
     install_requires=install_requires,
     packages=find_packages(),
 )
 
 
 # from setuptools import setup, find_packages
```

### Comparing `myPackageLicensePrototype-1.0.7/src/Implementation.ipynb` & `myPackageLicensePrototype-1.0.8/src/Implementation.ipynb`

 * *Files identical despite different names*

