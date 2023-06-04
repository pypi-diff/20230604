# Comparing `tmp/test-class-0.0.1.tar.gz` & `tmp/test-class-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-class-0.0.1.tar", last modified: Fri Jun  2 19:11:49 2023, max compression
+gzip compressed data, was "test-class-0.0.2.tar", last modified: Sun Jun  4 15:49:59 2023, max compression
```

## Comparing `test-class-0.0.1.tar` & `test-class-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:11:49.311036 test-class-0.0.1/
--rw-rw-rw-   0        0        0      292 2023-06-02 19:11:49.310037 test-class-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-02 19:11:16.000000 test-class-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 19:11:49.311036 test-class-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-02 19:11:49.299036 test-class-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 19:11:49.306037 test-class-0.0.1/src/test_class.egg-info/
--rw-rw-rw-   0        0        0      292 2023-06-02 19:11:49.000000 test-class-0.0.1/src/test_class.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-02 19:11:49.000000 test-class-0.0.1/src/test_class.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:11:49.000000 test-class-0.0.1/src/test_class.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 19:11:49.000000 test-class-0.0.1/src/test_class.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 19:11:49.309036 test-class-0.0.1/src/test_package/
--rw-rw-rw-   0        0        0        0 2023-06-02 19:05:30.000000 test-class-0.0.1/src/test_package/__init__.py
--rw-rw-rw-   0        0        0      174 2023-06-02 19:09:13.000000 test-class-0.0.1/src/test_package/test_module.py
+drwxrwxrwx   0        0        0        0 2023-06-04 15:49:59.396748 test-class-0.0.2/
+-rw-rw-rw-   0        0        0      292 2023-06-04 15:49:59.396748 test-class-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-04 15:49:34.000000 test-class-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 15:49:59.397748 test-class-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 15:49:59.382748 test-class-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 15:49:59.392752 test-class-0.0.2/src/test_class.egg-info/
+-rw-rw-rw-   0        0        0      292 2023-06-04 15:49:59.000000 test-class-0.0.2/src/test_class.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-04 15:49:59.000000 test-class-0.0.2/src/test_class.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 15:49:59.000000 test-class-0.0.2/src/test_class.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-04 15:49:59.000000 test-class-0.0.2/src/test_class.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 15:49:59.394747 test-class-0.0.2/src/test_package/
+-rw-rw-rw-   0        0        0        0 2023-06-02 19:05:30.000000 test-class-0.0.2/src/test_package/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-06-04 15:49:26.000000 test-class-0.0.2/src/test_package/test_module.py
```

