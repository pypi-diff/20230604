# Comparing `tmp/inegm.staff-0.2.2.tar.gz` & `tmp/inegm.staff-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inegm.staff-0.2.2.tar", last modified: Sun Jun  4 09:50:33 2023, max compression
+gzip compressed data, was "inegm.staff-0.2.3.tar", last modified: Sun Jun  4 11:54:13 2023, max compression
```

## Comparing `inegm.staff-0.2.2.tar` & `inegm.staff-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.075904 inegm.staff-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-04 09:50:33.075904 inegm.staff-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 09:50:33.075904 inegm.staff-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.071903 inegm.staff-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.071903 inegm.staff-0.2.2/src/inegm.staff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-04 09:50:33.000000 inegm.staff-0.2.2/src/inegm.staff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-04 09:50:33.000000 inegm.staff-0.2.2/src/inegm.staff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 09:50:33.000000 inegm.staff-0.2.2/src/inegm.staff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 09:50:33.000000 inegm.staff-0.2.2/src/inegm.staff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 09:50:33.000000 inegm.staff-0.2.2/src/inegm.staff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.071903 inegm.staff-0.2.2/src/staff/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/numerical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.071903 inegm.staff-0.2.2/src/staff/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/patterns/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/patterns/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    15313 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/pitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.071903 inegm.staff-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/tests/test_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/tests/test_pitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:54:13.593951 inegm.staff-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-04 11:54:13.593951 inegm.staff-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 11:54:13.593951 inegm.staff-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:54:13.585951 inegm.staff-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:54:13.589951 inegm.staff-0.2.3/src/inegm.staff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-04 11:54:13.000000 inegm.staff-0.2.3/src/inegm.staff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-04 11:54:13.000000 inegm.staff-0.2.3/src/inegm.staff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:54:13.000000 inegm.staff-0.2.3/src/inegm.staff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 11:54:13.000000 inegm.staff-0.2.3/src/inegm.staff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 11:54:13.000000 inegm.staff-0.2.3/src/inegm.staff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:54:13.589951 inegm.staff-0.2.3/src/staff/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/src/staff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/src/staff/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/src/staff/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/src/staff/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:54:13.589951 inegm.staff-0.2.3/src/staff/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/src/staff/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/src/staff/patterns/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/src/staff/patterns/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/src/staff/pitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:54:13.589951 inegm.staff-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/tests/test_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-04 11:53:39.000000 inegm.staff-0.2.3/tests/test_pitch.py
```

### Comparing `inegm.staff-0.2.2/LICENSE` & `inegm.staff-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.2/PKG-INFO` & `inegm.staff-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inegm.staff
-Version: 0.2.2
+Version: 0.2.3
 Summary: Utilities for computer assisted composition
 Author: Ismail Negm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `inegm.staff-0.2.2/pyproject.toml` & `inegm.staff-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.2/src/inegm.staff.egg-info/PKG-INFO` & `inegm.staff-0.2.3/src/inegm.staff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inegm.staff
-Version: 0.2.2
+Version: 0.2.3
 Summary: Utilities for computer assisted composition
 Author: Ismail Negm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `inegm.staff-0.2.2/src/staff/duration.py` & `inegm.staff-0.2.3/src/staff/duration.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.2/src/staff/patterns/duration.py` & `inegm.staff-0.2.3/src/staff/patterns/duration.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.2/src/staff/patterns/pattern.py` & `inegm.staff-0.2.3/src/staff/patterns/pattern.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.2/src/staff/pitch.py` & `inegm.staff-0.2.3/src/staff/pitch.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,14 +415,27 @@
         if (self.number < 0) or (self.number > 127):
             raise ValueError(f"number must be between 0 and 127. Got {self.number}")
 
     def __repr__(self):
         return f"MIDIPitch(number={self.number}, bend={self.bend})"
 
     @property
+    def number_precise(self) -> float:
+        """The MIDI number with the bend as the fractional part of a float.
+
+        Returns:
+            The precise MIDI number including the bend.
+
+        Examples:
+            >>> MIDIPitch(60, bend=MIDIBend(100, bend_range=200)).number_precise
+            60.5
+        """
+        return self.number + (self.bend.bend / self.bend.bend_range)
+
+    @property
     def frequency(self) -> Frequency:
         """Convert MIDIPitch to Frequency.
 
         Returns:
             The MIDIPitch frequency
         """
         fhz = Frequency(
```

### Comparing `inegm.staff-0.2.2/tests/test_duration.py` & `inegm.staff-0.2.3/tests/test_duration.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.2/tests/test_pitch.py` & `inegm.staff-0.2.3/tests/test_pitch.py`

 * *Files identical despite different names*

