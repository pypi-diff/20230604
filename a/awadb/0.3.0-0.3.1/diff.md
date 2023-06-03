# Comparing `tmp/awadb-0.3.0-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/awadb-0.3.1-cp37-cp37m-macosx_10_16_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2436783 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx  7044712 b- defN 23-May-29 08:01 awa.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx    25016 b- defN 23-May-19 10:31 awadb/__init__.py
--rw-r--r--  2.0 unx      816 b- defN 23-May-07 14:27 awadb/llm_embedding/__init__.py
--rw-r--r--  2.0 unx    15759 b- defN 23-May-29 08:01 awadb-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      415 b- defN 23-May-29 08:01 awadb-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-May-29 08:01 awadb-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-29 08:01 awadb-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      633 b- defN 23-May-29 08:01 awadb-0.3.0.dist-info/RECORD
-8 files, 7087469 bytes uncompressed, 2435691 bytes compressed:  65.6%
+Zip file size: 792107 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx  1982048 b- defN 23-Jun-03 23:01 awa.cpython-37m-darwin.so
+-rw-r--r--  2.0 unx    26165 b- defN 23-Jun-03 22:50 awadb/__init__.py
+-rw-r--r--  2.0 unx      816 b- defN 23-Jun-03 22:50 awadb/llm_embedding/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-03 23:01 awadb-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-03 23:01 awadb-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-03 23:01 awadb-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-03 23:01 awadb-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      624 b- defN 23-Jun-03 23:01 awadb-0.3.1.dist-info/RECORD
+8 files, 2021469 bytes uncompressed, 791033 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: awa.cpython-39-x86_64-linux-gnu.so
+Filename: awa.cpython-37m-darwin.so
 Comment: 
 
 Filename: awadb/__init__.py
 Comment: 
 
 Filename: awadb/llm_embedding/__init__.py
 Comment: 
 
-Filename: awadb-0.3.0.dist-info/LICENSE
+Filename: awadb-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: awadb-0.3.0.dist-info/METADATA
+Filename: awadb-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: awadb-0.3.0.dist-info/WHEEL
+Filename: awadb-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: awadb-0.3.0.dist-info/top_level.txt
+Filename: awadb-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: awadb-0.3.0.dist-info/RECORD
+Filename: awadb-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awadb/__init__.py

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import struct
 import json
 import io
 
 from enum import Enum
 
+from typing import Optional
 import awa
 
 
 class FieldDataType(Enum):
     INT = 1
     FLOAT = 2 
     STRING = 3 
@@ -219,35 +220,64 @@
                     table_info.AddVectorInfo(vec_info)
 
                 table_info.SetIndexingSize(10000)
                 table_info.SetRetrievalType("IVFPQ")
                 table_info.SetRetrievalParam('{"ncentroids" : 256, "nsubvector" : 16}')
                 self.tables_attr[table_name] = table_info
 
-    def Create(self, name):
-        if name in self.tables:
-            print('Table %s exist! Please directly Use(%s)' % (name, name))
+    def Create(self, table_name):
+        if table_name in self.tables:
+            print('Table %s exist! Please directly Use(%s)' % (table_name, table_name))
             return False
         log_dir = self.root_dir + '/log/'
-        log_dir = log_dir + name 
+        log_dir = log_dir + table_name 
         data_dir = self.root_dir + '/data/'
-        data_dir = data_dir + name
+        data_dir = data_dir + table_name
         new_table = awa.Init(log_dir, data_dir)
-        self.tables[name] = new_table
-        self.using_table_name = name
+        self.tables[table_name] = new_table
+        self.using_table_name = table_name
         self.using_table_engine = new_table
-        self.tables_fields_check[name] = False
-        self.tables_have_obvious_primary_key[name] = False
-        self.tables_primary_key_fid_no[name] = None
-        self.tables_doc_count[name] = 0
- 
+        self.tables_fields_check[table_name] = False
+        self.tables_have_obvious_primary_key[table_name] = False
+        self.tables_primary_key_fid_no[table_name] = None
+        self.tables_doc_count[table_name] = 0
+
+    def Close(self, table_name: Optional[str] = None):
+        if table_name is None:
+            if self.using_table_engine is None:
+                return False
+            if awa.Close(self.using_table_engine) == 0:
+                return True
+            return False
+
+        if table_name is not None and (not table_name  in self.tables):
+            print('Table %s not exist!' % table_name)
+            return False
+        self.using_table_engine = self.tables[table_name]
+        if self.using_table_engine is None:
+            return False
+        if awa.Close(self.using_table_engine) == 0:
+            return True
+        return False
+
+
+    def Load(self, table_name):
+        if not table_name in self.tables:
+            self.Create(table_name)
+
+        self.using_table_name = table_name
+        self.using_table_engine = self.tables[table_name]
+        if not awa.LoadFromLocal(self.using_table_engine):
+            print('Table %s can not be loaded!' % self.using_table_name)
+            return False
+        return True
 
     def Use(self, table_name):
         if not table_name in self.tables:
-            print('Table %s not exist! Please create first!')
+            print('Table %s not exist! Please create first!' % table_name)
             return False
         self.using_table_name = table_name 
         self.using_table_engine = self.tables[table_name]
 
 
     def __FieldCheck(self, field_idx, field_name, field_data, fields_type):
         if not self.tables_fields_check[self.using_table_name]:
@@ -408,16 +438,14 @@
                             field_value = field['embedding_text']
                         else:
                             continue
                     doc.append(self.llm.Embedding(field_value))
                     
             field_no = field_no + 1
 
-
-
     '''
     primary_key : format @name
     is_index :  format !province
     '''
     def Add(self, doc):
         if not isinstance(doc, list):
             error_msg = Exception("Incorrect argument, list type is needed for Add!!!")
```

