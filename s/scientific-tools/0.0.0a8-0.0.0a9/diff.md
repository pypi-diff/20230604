# Comparing `tmp/scientific_tools-0.0.0a8-py3-none-any.whl.zip` & `tmp/scientific_tools-0.0.0a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 3593 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat        0 b- defN 22-Sep-11 09:50 graphics/__init__.py
--rw-rw-rw-  2.0 fat     3686 b- defN 22-Sep-11 09:40 graphics/graphics.py
--rw-rw-rw-  2.0 fat      172 b- defN 22-Sep-11 09:52 scientific_tools-0.0.0a8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2124 b- defN 22-Sep-11 09:52 scientific_tools-0.0.0a8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Sep-11 09:52 scientific_tools-0.0.0a8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Sep-11 09:52 scientific_tools-0.0.0a8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      590 b- defN 22-Sep-11 09:52 scientific_tools-0.0.0a8.dist-info/RECORD
-7 files, 6673 bytes uncompressed, 2531 bytes compressed:  62.1%
+Zip file size: 3812 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Sep-11 09:50 scientific_tools/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Sep-11 09:50 scientific_tools/graphics/__init__.py
+-rw-rw-rw-  2.0 fat     3686 b- defN 22-Sep-11 09:40 scientific_tools/graphics/graphics.py
+-rw-rw-rw-  2.0 fat      172 b- defN 22-Sep-11 09:58 scientific_tools-0.0.0a9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2124 b- defN 22-Sep-11 09:58 scientific_tools-0.0.0a9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Sep-11 09:58 scientific_tools-0.0.0a9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 22-Sep-11 09:58 scientific_tools-0.0.0a9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      707 b- defN 22-Sep-11 09:58 scientific_tools-0.0.0a9.dist-info/RECORD
+8 files, 6798 bytes uncompressed, 2550 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
-Filename: graphics/__init__.py
+Filename: scientific_tools/__init__.py
 Comment: 
 
-Filename: graphics/graphics.py
+Filename: scientific_tools/graphics/__init__.py
 Comment: 
 
-Filename: scientific_tools-0.0.0a8.dist-info/LICENSE
+Filename: scientific_tools/graphics/graphics.py
 Comment: 
 
-Filename: scientific_tools-0.0.0a8.dist-info/METADATA
+Filename: scientific_tools-0.0.0a9.dist-info/LICENSE
 Comment: 
 
-Filename: scientific_tools-0.0.0a8.dist-info/WHEEL
+Filename: scientific_tools-0.0.0a9.dist-info/METADATA
 Comment: 
 
-Filename: scientific_tools-0.0.0a8.dist-info/top_level.txt
+Filename: scientific_tools-0.0.0a9.dist-info/WHEEL
 Comment: 
 
-Filename: scientific_tools-0.0.0a8.dist-info/RECORD
+Filename: scientific_tools-0.0.0a9.dist-info/top_level.txt
+Comment: 
+
+Filename: scientific_tools-0.0.0a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `graphics/graphics.py` & `scientific_tools/graphics/graphics.py`

 * *Files identical despite different names*

## Comparing `scientific_tools-0.0.0a8.dist-info/METADATA` & `scientific_tools-0.0.0a9.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific-tools
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: Scientific tools is the Swiss knife for scientists and students who work with python.
 Author-email: Cyprien BONTRON <c.b.e.python@gmail.com>
 Maintainer-email: Cyprien BONTRON <c.b.e.python@gmail.com>
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License        
         Futher information at: https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode
 Project-URL: Download-URL, https://pypi.org/project/scientific_tools/
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `scientific_tools-0.0.0a8.dist-info/RECORD` & `scientific_tools-0.0.0a9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-graphics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-graphics/graphics.py,sha256=gaGTLGoYHnI3F-6qYYKy58Sl8RczcTsKXqTV_GN9u9w,3686
-scientific_tools-0.0.0a8.dist-info/LICENSE,sha256=8Efq7_9a9Gk8K4KtwX5YS8GKttL5UTRLjEzqGbLOgpY,172
-scientific_tools-0.0.0a8.dist-info/METADATA,sha256=QNL54MzORmD9Lyi1zn1zIFZYdAXYGxNumBoMptJc96g,2124
-scientific_tools-0.0.0a8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-scientific_tools-0.0.0a8.dist-info/top_level.txt,sha256=KHs_lM1QzMMzLlURkl8KxmsQQJA3o8PVFgDVXTSpK_o,9
-scientific_tools-0.0.0a8.dist-info/RECORD,,
+scientific_tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+scientific_tools/graphics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+scientific_tools/graphics/graphics.py,sha256=gaGTLGoYHnI3F-6qYYKy58Sl8RczcTsKXqTV_GN9u9w,3686
+scientific_tools-0.0.0a9.dist-info/LICENSE,sha256=8Efq7_9a9Gk8K4KtwX5YS8GKttL5UTRLjEzqGbLOgpY,172
+scientific_tools-0.0.0a9.dist-info/METADATA,sha256=IMMAP4oVkNofRWxDxXg4dW5PmD-2XS02guAgkTrc83c,2124
+scientific_tools-0.0.0a9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+scientific_tools-0.0.0a9.dist-info/top_level.txt,sha256=aUDjvOA9144J4tqwvy5S7UELW3MeAGX7dK1awQ4SxeY,17
+scientific_tools-0.0.0a9.dist-info/RECORD,,
```

