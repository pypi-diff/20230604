# Comparing `tmp/myPackageLicensePrototype-1.1.2.tar.gz` & `tmp/myPackageLicensePrototype-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myPackageLicensePrototype-1.1.2.tar", last modified: Sun Jun  4 13:56:40 2023, max compression
+gzip compressed data, was "mypackagelicenseprototype-1.1.4.tar", last modified: Sun Jun  4 14:13:43 2023, max compression
```

## Comparing `myPackageLicensePrototype-1.1.2.tar` & `myPackageLicensePrototype-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 13:56:40.805984 myPackageLicensePrototype-1.1.2/
--rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.2/Implementation.ipynb
--rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      133 2023-06-04 13:56:40.805472 myPackageLicensePrototype-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 myPackageLicensePrototype-1.1.2/README.md
--rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.1.2/__init__.py
--rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.1.2/local_environment_installation_guide.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 13:56:40.784866 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-04 13:56:40.000000 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-06-04 13:56:40.000000 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:56:40.000000 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 13:56:40.000000 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-04 13:56:40.000000 myPackageLicensePrototype-1.1.2/myPackageLicensePrototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 myPackageLicensePrototype-1.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 13:56:40.805984 myPackageLicensePrototype-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1373 2023-06-04 13:56:22.000000 myPackageLicensePrototype-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:56:40.801047 myPackageLicensePrototype-1.1.2/src/
--rw-rw-rw-   0        0        0      140 2023-06-04 13:42:31.000000 myPackageLicensePrototype-1.1.2/src/PackageContent.py
--rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.1.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:13:43.342417 mypackagelicenseprototype-1.1.4/
+-rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 mypackagelicenseprototype-1.1.4/Implementation.ipynb
+-rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 mypackagelicenseprototype-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      133 2023-06-04 14:13:43.342417 mypackagelicenseprototype-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 mypackagelicenseprototype-1.1.4/README.md
+-rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 mypackagelicenseprototype-1.1.4/local_environment_installation_guide.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 mypackagelicenseprototype-1.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 14:13:43.350529 mypackagelicenseprototype-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1408 2023-06-04 14:13:16.000000 mypackagelicenseprototype-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:13:43.253002 mypackagelicenseprototype-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 14:13:43.342417 mypackagelicenseprototype-1.1.4/src/mypackagelicenseprototype.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-06-04 14:13:42.000000 mypackagelicenseprototype-1.1.4/src/mypackagelicenseprototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-06-04 14:13:43.000000 mypackagelicenseprototype-1.1.4/src/mypackagelicenseprototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:13:42.000000 mypackagelicenseprototype-1.1.4/src/mypackagelicenseprototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 14:13:42.000000 mypackagelicenseprototype-1.1.4/src/mypackagelicenseprototype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:13:42.000000 mypackagelicenseprototype-1.1.4/src/mypackagelicenseprototype.egg-info/top_level.txt
```

### Comparing `myPackageLicensePrototype-1.1.2/Implementation.ipynb` & `mypackagelicenseprototype-1.1.4/Implementation.ipynb`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.1.2/LICENSE` & `mypackagelicenseprototype-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.1.2/local_environment_installation_guide.txt` & `mypackagelicenseprototype-1.1.4/local_environment_installation_guide.txt`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.1.2/setup.py` & `mypackagelicenseprototype-1.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,20 @@
     with open(file, 'rb') as f:
         return chardet.detect(f.read())['encoding']
 
 encoding = get_encoding('requirements.txt')
 install_requires = codecs.open('requirements.txt', 'r', encoding=encoding).read().splitlines()
  
 setup(
-    name='myPackageLicensePrototype',
-    version='1.1.2',
+    name='mypackagelicenseprototype',
+    version='1.1.4',
     description='Description of your package',
     install_requires=install_requires,
-    packages=find_packages(),
+    package_dir={'': 'src'},
+    packages=find_packages('src'),
 )
 
 
 # from setuptools import setup, find_packages
 
 #from myPackageLicensePrototype import __version__
```

