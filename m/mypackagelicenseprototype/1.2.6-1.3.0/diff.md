# Comparing `tmp/myPackageLicensePrototype-1.2.6.tar.gz` & `tmp/mypackagelicenseprototype-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackagelicenseprototype-1.2.6.tar", last modified: Sun Jun  4 14:53:53 2023, max compression
+gzip compressed data, was "mypackagelicenseprototype-1.3.0.tar", last modified: Sun Jun  4 15:45:26 2023, max compression
```

## Comparing `myPackageLicensePrototype-1.2.6.tar` & `mypackagelicenseprototype-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 14:53:53.362850 mypackagelicenseprototype-1.2.6/
--rw-rw-rw-   0        0        0     1026 2023-06-04 13:42:31.000000 mypackagelicenseprototype-1.2.6/Implementation.ipynb
--rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 mypackagelicenseprototype-1.2.6/LICENSE
--rw-rw-rw-   0        0        0      133 2023-06-04 14:53:53.362850 mypackagelicenseprototype-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 mypackagelicenseprototype-1.2.6/README.md
--rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 mypackagelicenseprototype-1.2.6/local_environment_installation_guide.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 14:53:53.313981 mypackagelicenseprototype-1.2.6/mypackagelicenseprototype/
--rw-rw-rw-   0        0        0      140 2023-06-04 14:16:31.000000 mypackagelicenseprototype-1.2.6/mypackagelicenseprototype/PackageContent.py
--rw-rw-rw-   0        0        0       54 2023-06-04 14:53:30.000000 mypackagelicenseprototype-1.2.6/mypackagelicenseprototype/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 14:53:53.354881 mypackagelicenseprototype-1.2.6/mypackagelicenseprototype.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-04 14:53:52.000000 mypackagelicenseprototype-1.2.6/mypackagelicenseprototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-06-04 14:53:53.000000 mypackagelicenseprototype-1.2.6/mypackagelicenseprototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 14:53:52.000000 mypackagelicenseprototype-1.2.6/mypackagelicenseprototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-04 14:53:52.000000 mypackagelicenseprototype-1.2.6/mypackagelicenseprototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-04 14:53:52.000000 mypackagelicenseprototype-1.2.6/mypackagelicenseprototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 10:24:26.000000 mypackagelicenseprototype-1.2.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 14:53:53.362850 mypackagelicenseprototype-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1373 2023-06-04 14:53:39.000000 mypackagelicenseprototype-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 15:45:26.982366 mypackagelicenseprototype-1.3.0/
+-rw-rw-rw-   0        0        0      138 2023-06-04 15:45:26.982366 mypackagelicenseprototype-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 mypackagelicenseprototype-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 15:45:26.981370 mypackagelicenseprototype-1.3.0/mypackagelicenseprototype.egg-info/
+-rw-rw-rw-   0        0        0      138 2023-06-04 15:45:26.000000 mypackagelicenseprototype-1.3.0/mypackagelicenseprototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-06-04 15:45:26.000000 mypackagelicenseprototype-1.3.0/mypackagelicenseprototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 15:45:26.000000 mypackagelicenseprototype-1.3.0/mypackagelicenseprototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 15:45:26.000000 mypackagelicenseprototype-1.3.0/mypackagelicenseprototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      233 2023-06-04 15:38:32.000000 mypackagelicenseprototype-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-06-04 15:45:26.984371 mypackagelicenseprototype-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1423 2023-06-04 15:45:12.000000 mypackagelicenseprototype-1.3.0/setup.py
```

