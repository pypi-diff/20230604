# Comparing `tmp/wombo-0.1.71.tar.gz` & `tmp/wombo-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wombo-0.1.71.tar", max compression
+gzip compressed data, was "wombo-0.1.72.tar", max compression
```

## Comparing `wombo-0.1.71.tar` & `wombo-0.1.72.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.71/LICENSE
--rw-r--r--   0        0        0     2323 2023-06-02 21:15:19.997083 wombo-0.1.71/README.md
--rw-r--r--   0        0        0      397 2023-06-04 18:30:02.713770 wombo-0.1.71/pyproject.toml
--rw-r--r--   0        0        0      143 2023-06-04 08:40:59.713656 wombo-0.1.71/wombo/__init__.py
--rw-r--r--   0        0        0     4562 2023-06-04 18:22:06.269770 wombo-0.1.71/wombo/async_dream.py
--rw-r--r--   0        0        0      664 2023-06-04 08:28:17.545656 wombo-0.1.71/wombo/base_dream.py
--rw-r--r--   0        0        0     3920 2023-06-04 18:26:03.057770 wombo-0.1.71/wombo/dream.py
--rw-r--r--   0        0        0      163 2023-06-04 08:28:17.549656 wombo-0.1.71/wombo/models/__init__.py
--rw-r--r--   0        0        0      524 2023-06-03 20:13:43.005160 wombo-0.1.71/wombo/models/check_task.py
--rw-r--r--   0        0        0      504 2023-06-04 08:28:17.549656 wombo-0.1.71/wombo/models/create_task.py
--rw-r--r--   0        0        0     3232 2023-06-04 08:28:17.549656 wombo-0.1.71/wombo/urls.py
--rw-r--r--   0        0        0     3059 1970-01-01 00:00:00.000000 wombo-0.1.71/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-02 14:02:35.382424 wombo-0.1.72/LICENSE
+-rw-r--r--   0        0        0     3567 2023-06-04 18:50:34.397770 wombo-0.1.72/README.md
+-rw-r--r--   0        0        0      397 2023-06-04 18:52:39.309770 wombo-0.1.72/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-06-04 08:40:59.713656 wombo-0.1.72/wombo/__init__.py
+-rw-r--r--   0        0        0     4562 2023-06-04 18:22:06.269770 wombo-0.1.72/wombo/async_dream.py
+-rw-r--r--   0        0        0      664 2023-06-04 08:28:17.545656 wombo-0.1.72/wombo/base_dream.py
+-rw-r--r--   0        0        0     3920 2023-06-04 18:26:03.057770 wombo-0.1.72/wombo/dream.py
+-rw-r--r--   0        0        0      163 2023-06-04 08:28:17.549656 wombo-0.1.72/wombo/models/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-03 20:13:43.005160 wombo-0.1.72/wombo/models/check_task.py
+-rw-r--r--   0        0        0      504 2023-06-04 08:28:17.549656 wombo-0.1.72/wombo/models/create_task.py
+-rw-r--r--   0        0        0     3232 2023-06-04 08:28:17.549656 wombo-0.1.72/wombo/urls.py
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 wombo-0.1.72/PKG-INFO
```

### Comparing `wombo-0.1.71/LICENSE` & `wombo-0.1.72/LICENSE`

 * *Files identical despite different names*

### Comparing `wombo-0.1.71/wombo/async_dream.py` & `wombo-0.1.72/wombo/async_dream.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.71/wombo/base_dream.py` & `wombo-0.1.72/wombo/base_dream.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.71/wombo/dream.py` & `wombo-0.1.72/wombo/dream.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.71/wombo/models/check_task.py` & `wombo-0.1.72/wombo/models/check_task.py`

 * *Files identical despite different names*

### Comparing `wombo-0.1.71/wombo/urls.py` & `wombo-0.1.72/wombo/urls.py`

 * *Files identical despite different names*

