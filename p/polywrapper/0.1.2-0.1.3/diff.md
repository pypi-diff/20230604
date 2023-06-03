# Comparing `tmp/polywrapper-0.1.2.tar.gz` & `tmp/polywrapper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrapper-0.1.2.tar", last modified: Sat Jun  3 21:13:40 2023, max compression
+gzip compressed data, was "polywrapper-0.1.3.tar", last modified: Sat Jun  3 22:23:21 2023, max compression
```

## Comparing `polywrapper-0.1.2.tar` & `polywrapper-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 21:13:40.864127 polywrapper-0.1.2/
--rw-r--r--   0 david     (1000) david     (1000)     1065 2023-03-13 22:24:52.000000 polywrapper-0.1.2/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 21:13:40.864127 polywrapper-0.1.2/PKG-INFO
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 21:13:40.860128 polywrapper-0.1.2/polywrapper/
--rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-03 21:13:12.000000 polywrapper-0.1.2/polywrapper/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     3714 2023-06-03 20:49:10.000000 polywrapper-0.1.2/polywrapper/polywrapper.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 21:13:40.864127 polywrapper-0.1.2/polywrapper.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 21:13:40.000000 polywrapper-0.1.2/polywrapper.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 21:13:40.000000 polywrapper-0.1.2/polywrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-03 21:13:40.000000 polywrapper-0.1.2/polywrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       17 2023-06-03 21:13:40.000000 polywrapper-0.1.2/polywrapper.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       12 2023-06-03 21:13:40.000000 polywrapper-0.1.2/polywrapper.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-06-03 21:13:40.864127 polywrapper-0.1.2/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)      294 2023-06-03 21:13:39.000000 polywrapper-0.1.2/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 22:23:21.560860 polywrapper-0.1.3/
+-rw-r--r--   0 david     (1000) david     (1000)     1065 2023-03-13 22:24:52.000000 polywrapper-0.1.3/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 22:23:21.560860 polywrapper-0.1.3/PKG-INFO
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 22:23:21.560860 polywrapper-0.1.3/polywrapper/
+-rw-rw-r--   0 david     (1000) david     (1000)       46 2023-06-03 21:13:12.000000 polywrapper-0.1.3/polywrapper/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     4238 2023-06-03 22:14:37.000000 polywrapper-0.1.3/polywrapper/polywrapper.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-03 22:23:21.560860 polywrapper-0.1.3/polywrapper.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 22:23:21.000000 polywrapper-0.1.3/polywrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      241 2023-06-03 22:23:21.000000 polywrapper-0.1.3/polywrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-03 22:23:21.000000 polywrapper-0.1.3/polywrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       17 2023-06-03 22:23:21.000000 polywrapper-0.1.3/polywrapper.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       12 2023-06-03 22:23:21.000000 polywrapper-0.1.3/polywrapper.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-06-03 22:23:21.560860 polywrapper-0.1.3/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)      294 2023-06-03 22:22:33.000000 polywrapper-0.1.3/setup.py
```

### Comparing `polywrapper-0.1.2/LICENSE` & `polywrapper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polywrapper-0.1.2/polywrapper/polywrapper.py` & `polywrapper-0.1.3/polywrapper/polywrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,7 +115,25 @@
                     "location": key,
                     "action": "record",
                     "value": input_value,
                 }
             )
         )
         return json.loads(self.ws.recv())
+
+    def append(self, key: str, value: any):
+        if type(value) == dict:
+            input_value = json.dumps(value)
+        else:
+            input_value = value
+        self.ws.send(
+            json.dumps(
+                {
+                    "password": self.password,
+                    "dbname": self.db_name,
+                    "location": key,
+                    "action": "append",
+                    "value": input_value,
+                }
+            )
+        )
+        return json.loads(self.ws.recv())
```

