# Comparing `tmp/myPackageLicensePrototype-1.2.0.tar.gz` & `tmp/myPackageLicensePrototype-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackagelicenseprototype-1.2.0.tar", last modified: Sun Jun  4 14:17:23 2023, max compression
+gzip compressed data, was "mypackagelicenseprototype-1.2.1.tar", last modified: Sun Jun  4 14:23:51 2023, max compression
```

## Comparing `myPackageLicensePrototype-1.2.0.tar` & `myPackageLicensePrototype-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:17:23.766410 mypackagelicenseprototype-1.2.0/
--rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 mypackagelicenseprototype-1.2.0/Implementation.ipynb
--rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 mypackagelicenseprototype-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      133 2023-06-04 14:17:23.766410 mypackagelicenseprototype-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      140 2023-06-04 14:16:31.000000 mypackagelicenseprototype-1.2.0/PackageContent.py
--rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 mypackagelicenseprototype-1.2.0/README.md
--rw-rw-rw-   0        0        0        0 2023-06-04 14:16:31.000000 mypackagelicenseprototype-1.2.0/__init__.py
--rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 mypackagelicenseprototype-1.2.0/local_environment_installation_guide.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 14:17:23.756617 mypackagelicenseprototype-1.2.0/mypackagelicenseprototype.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-04 14:17:23.000000 mypackagelicenseprototype-1.2.0/mypackagelicenseprototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-06-04 14:17:23.000000 mypackagelicenseprototype-1.2.0/mypackagelicenseprototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:17:23.000000 mypackagelicenseprototype-1.2.0/mypackagelicenseprototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 14:17:23.000000 mypackagelicenseprototype-1.2.0/mypackagelicenseprototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-04 14:17:23.000000 mypackagelicenseprototype-1.2.0/mypackagelicenseprototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 mypackagelicenseprototype-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 14:17:23.766410 mypackagelicenseprototype-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-06-04 14:17:12.000000 mypackagelicenseprototype-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:23:51.833884 mypackagelicenseprototype-1.2.1/
+-rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 mypackagelicenseprototype-1.2.1/Implementation.ipynb
+-rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 mypackagelicenseprototype-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      133 2023-06-04 14:23:51.833884 mypackagelicenseprototype-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2023-06-04 14:16:31.000000 mypackagelicenseprototype-1.2.1/PackageContent.py
+-rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 mypackagelicenseprototype-1.2.1/README.md
+-rw-rw-rw-   0        0        0       41 2023-06-04 14:20:50.000000 mypackagelicenseprototype-1.2.1/__init__.py
+-rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 mypackagelicenseprototype-1.2.1/local_environment_installation_guide.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 14:23:51.831301 mypackagelicenseprototype-1.2.1/mypackagelicenseprototype.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-06-04 14:23:51.000000 mypackagelicenseprototype-1.2.1/mypackagelicenseprototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-06-04 14:23:51.000000 mypackagelicenseprototype-1.2.1/mypackagelicenseprototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:23:51.000000 mypackagelicenseprototype-1.2.1/mypackagelicenseprototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 14:23:51.000000 mypackagelicenseprototype-1.2.1/mypackagelicenseprototype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-04 14:23:51.000000 mypackagelicenseprototype-1.2.1/mypackagelicenseprototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 mypackagelicenseprototype-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 14:23:51.833884 mypackagelicenseprototype-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1366 2023-06-04 14:23:16.000000 mypackagelicenseprototype-1.2.1/setup.py
```

### Comparing `mypackagelicenseprototype-1.2.0/Implementation.ipynb` & `mypackagelicenseprototype-1.2.1/Implementation.ipynb`

 * *Files identical despite different names*

### Comparing `mypackagelicenseprototype-1.2.0/LICENSE` & `mypackagelicenseprototype-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypackagelicenseprototype-1.2.0/local_environment_installation_guide.txt` & `mypackagelicenseprototype-1.2.1/local_environment_installation_guide.txt`

 * *Files identical despite different names*

### Comparing `mypackagelicenseprototype-1.2.0/setup.py` & `mypackagelicenseprototype-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
         return chardet.detect(f.read())['encoding']
 
 encoding = get_encoding('requirements.txt')
 install_requires = codecs.open('requirements.txt', 'r', encoding=encoding).read().splitlines()
  
 setup(
     name='mypackagelicenseprototype',
-    version='1.2.0',
+    version='1.2.1',
     description='Description of your package',
     install_requires=install_requires,
-    ppackage_data={'': ['src/*.py']}
+    #ppackage_data={'': ['src/*.py']}
 )
 
 
 # from setuptools import setup, find_packages
 
 #from myPackageLicensePrototype import __version__
```

