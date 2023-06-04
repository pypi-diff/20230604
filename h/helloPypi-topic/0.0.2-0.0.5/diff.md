# Comparing `tmp/helloPypi-topic-0.0.2.tar.gz` & `tmp/helloPypi-topic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helloPypi-topic-0.0.2.tar", last modified: Sat Jun  3 18:24:38 2023, max compression
+gzip compressed data, was "helloPypi-topic-0.0.5.tar", last modified: Sun Jun  4 20:11:37 2023, max compression
```

## Comparing `helloPypi-topic-0.0.2.tar` & `helloPypi-topic-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-03 18:24:38.043587 helloPypi-topic-0.0.2/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      168 2023-06-03 18:24:38.043587 helloPypi-topic-0.0.2/PKG-INFO
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-03 18:24:38.043587 helloPypi-topic-0.0.2/helloPypi_topic.egg-info/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      168 2023-06-03 18:24:37.000000 helloPypi-topic-0.0.2/helloPypi_topic.egg-info/PKG-INFO
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      241 2023-06-03 18:24:37.000000 helloPypi-topic-0.0.2/helloPypi_topic.egg-info/SOURCES.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)        1 2023-06-03 18:24:37.000000 helloPypi-topic-0.0.2/helloPypi_topic.egg-info/dependency_links.txt
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       15 2023-06-03 18:24:37.000000 helloPypi-topic-0.0.2/helloPypi_topic.egg-info/top_level.txt
-drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-03 18:24:38.043587 helloPypi-topic-0.0.2/myhellopackage/
--rw-rw-r--   0 caleb     (1000) caleb     (1000)        0 2023-06-03 18:23:37.000000 helloPypi-topic-0.0.2/myhellopackage/__init__.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       79 2023-06-03 18:20:29.000000 helloPypi-topic-0.0.2/myhellopackage/channel.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       41 2023-06-03 18:17:55.000000 helloPypi-topic-0.0.2/myhellopackage/hello.py
--rw-rw-r--   0 caleb     (1000) caleb     (1000)       38 2023-06-03 18:24:38.043587 helloPypi-topic-0.0.2/setup.cfg
--rw-rw-r--   0 caleb     (1000) caleb     (1000)      218 2023-06-03 18:24:29.000000 helloPypi-topic-0.0.2/setup.py
+drwxr-sr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 20:11:37.869241 helloPypi-topic-0.0.5/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      104 2023-06-04 20:11:37.869241 helloPypi-topic-0.0.5/PKG-INFO
+drwxr-sr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 20:11:37.865241 helloPypi-topic-0.0.5/helloPypi_topic.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      104 2023-06-04 20:11:37.000000 helloPypi-topic-0.0.5/helloPypi_topic.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      241 2023-06-04 20:11:37.000000 helloPypi-topic-0.0.5/helloPypi_topic.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-04 20:11:37.000000 helloPypi-topic-0.0.5/helloPypi_topic.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       15 2023-06-04 20:11:37.000000 helloPypi-topic-0.0.5/helloPypi_topic.egg-info/top_level.txt
+drwxr-sr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 20:11:37.865241 helloPypi-topic-0.0.5/myhellopackage/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2023-06-04 20:09:53.000000 helloPypi-topic-0.0.5/myhellopackage/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       79 2023-06-04 20:09:53.000000 helloPypi-topic-0.0.5/myhellopackage/channel.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       41 2023-06-04 20:09:53.000000 helloPypi-topic-0.0.5/myhellopackage/hello.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2023-06-04 20:11:37.869241 helloPypi-topic-0.0.5/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      218 2023-06-04 20:09:53.000000 helloPypi-topic-0.0.5/setup.py
```

