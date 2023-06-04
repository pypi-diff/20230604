# Comparing `tmp/myPackageLicensePrototype-1.2.4.tar.gz` & `tmp/myPackageLicensePrototype-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackagelicenseprototype-1.2.4.tar", last modified: Sun Jun  4 14:48:33 2023, max compression
+gzip compressed data, was "mypackagelicenseprototype-1.2.5.tar", last modified: Sun Jun  4 14:51:34 2023, max compression
```

## Comparing `myPackageLicensePrototype-1.2.4.tar` & `myPackageLicensePrototype-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:48:33.904932 mypackagelicenseprototype-1.2.4/
--rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 mypackagelicenseprototype-1.2.4/Implementation.ipynb
--rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 mypackagelicenseprototype-1.2.4/LICENSE
--rw-rw-rw-   0        0        0      133 2023-06-04 14:48:33.903290 mypackagelicenseprototype-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 mypackagelicenseprototype-1.2.4/README.md
--rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 mypackagelicenseprototype-1.2.4/local_environment_installation_guide.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 14:48:33.830043 mypackagelicenseprototype-1.2.4/mypackagelicenseprototype/
--rw-rw-rw-   0        0        0      140 2023-06-04 14:16:31.000000 mypackagelicenseprototype-1.2.4/mypackagelicenseprototype/PackageContent.py
--rw-rw-rw-   0        0        0        0 2023-06-04 14:32:20.000000 mypackagelicenseprototype-1.2.4/mypackagelicenseprototype/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:48:33.900310 mypackagelicenseprototype-1.2.4/mypackagelicenseprototype.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-04 14:48:33.000000 mypackagelicenseprototype-1.2.4/mypackagelicenseprototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-06-04 14:48:33.000000 mypackagelicenseprototype-1.2.4/mypackagelicenseprototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:48:33.000000 mypackagelicenseprototype-1.2.4/mypackagelicenseprototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 14:48:33.000000 mypackagelicenseprototype-1.2.4/mypackagelicenseprototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-04 14:48:33.000000 mypackagelicenseprototype-1.2.4/mypackagelicenseprototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 mypackagelicenseprototype-1.2.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 14:48:33.904932 mypackagelicenseprototype-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1373 2023-06-04 14:47:31.000000 mypackagelicenseprototype-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:51:34.166744 mypackagelicenseprototype-1.2.5/
+-rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 mypackagelicenseprototype-1.2.5/Implementation.ipynb
+-rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 mypackagelicenseprototype-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0      133 2023-06-04 14:51:34.166744 mypackagelicenseprototype-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 mypackagelicenseprototype-1.2.5/README.md
+-rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 mypackagelicenseprototype-1.2.5/local_environment_installation_guide.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 14:51:34.130662 mypackagelicenseprototype-1.2.5/mypackagelicenseprototype/
+-rw-rw-rw-   0        0        0      140 2023-06-04 14:16:31.000000 mypackagelicenseprototype-1.2.5/mypackagelicenseprototype/PackageContent.py
+-rw-rw-rw-   0        0        0       28 2023-06-04 14:51:10.000000 mypackagelicenseprototype-1.2.5/mypackagelicenseprototype/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:51:34.164495 mypackagelicenseprototype-1.2.5/mypackagelicenseprototype.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-06-04 14:51:33.000000 mypackagelicenseprototype-1.2.5/mypackagelicenseprototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-06-04 14:51:33.000000 mypackagelicenseprototype-1.2.5/mypackagelicenseprototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:51:33.000000 mypackagelicenseprototype-1.2.5/mypackagelicenseprototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 14:51:33.000000 mypackagelicenseprototype-1.2.5/mypackagelicenseprototype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-04 14:51:33.000000 mypackagelicenseprototype-1.2.5/mypackagelicenseprototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 mypackagelicenseprototype-1.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 14:51:34.166744 mypackagelicenseprototype-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2023-06-04 14:51:26.000000 mypackagelicenseprototype-1.2.5/setup.py
```

### Comparing `mypackagelicenseprototype-1.2.4/Implementation.ipynb` & `mypackagelicenseprototype-1.2.5/Implementation.ipynb`

 * *Files identical despite different names*

### Comparing `mypackagelicenseprototype-1.2.4/LICENSE` & `mypackagelicenseprototype-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypackagelicenseprototype-1.2.4/local_environment_installation_guide.txt` & `mypackagelicenseprototype-1.2.5/local_environment_installation_guide.txt`

 * *Files identical despite different names*

### Comparing `mypackagelicenseprototype-1.2.4/setup.py` & `mypackagelicenseprototype-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         return chardet.detect(f.read())['encoding']
 
 encoding = get_encoding('requirements.txt')
 install_requires = codecs.open('requirements.txt', 'r', encoding=encoding).read().splitlines()
  
 setup(
     name='mypackagelicenseprototype',
-    version='1.2.4',
+    version='1.2.5',
     description='Description of your package',
     install_requires=install_requires,
     packages=find_packages(),
 )
 
 
 # from setuptools import setup, find_packages
```

