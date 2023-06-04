# Comparing `tmp/erdgen-0.0.1rc2.tar.gz` & `tmp/erdgen-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdgen-0.0.1rc2.tar", last modified: Fri Jun  2 18:45:25 2023, max compression
+gzip compressed data, was "erdgen-0.0.1rc3.tar", last modified: Sun Jun  4 00:50:21 2023, max compression
```

## Comparing `erdgen-0.0.1rc2.tar` & `erdgen-0.0.1rc3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 18:45:25.511196 erdgen-0.0.1rc2/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1068 2023-06-02 00:24:03.000000 erdgen-0.0.1rc2/LICENSE
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      169 2023-06-02 18:44:51.000000 erdgen-0.0.1rc2/MANIFEST.in
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4495 2023-06-02 18:45:25.507196 erdgen-0.0.1rc2/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3912 2023-06-02 00:58:39.000000 erdgen-0.0.1rc2/README.md
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 18:45:25.507196 erdgen-0.0.1rc2/erdgen/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc2/erdgen/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       87 2023-06-02 00:24:03.000000 erdgen-0.0.1rc2/erdgen/__main__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      419 2023-06-02 00:24:03.000000 erdgen-0.0.1rc2/erdgen/erdgen.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 18:45:25.507196 erdgen-0.0.1rc2/erdgen/src/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3004 2023-06-02 18:44:51.000000 erdgen-0.0.1rc2/erdgen/src/_.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc2/erdgen/src/__init__.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 18:45:25.507196 erdgen-0.0.1rc2/erdgen.egg-info/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4495 2023-06-02 18:45:25.000000 erdgen-0.0.1rc2/erdgen.egg-info/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      281 2023-06-02 18:45:25.000000 erdgen-0.0.1rc2/erdgen.egg-info/SOURCES.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-02 18:45:25.000000 erdgen-0.0.1rc2/erdgen.egg-info/dependency_links.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-02 18:45:25.000000 erdgen-0.0.1rc2/erdgen.egg-info/requires.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        7 2023-06-02 18:45:25.000000 erdgen-0.0.1rc2/erdgen.egg-info/top_level.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-02 18:45:25.511196 erdgen-0.0.1rc2/setup.cfg
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      962 2023-06-02 18:44:51.000000 erdgen-0.0.1rc2/setup.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-04 00:50:21.336350 erdgen-0.0.1rc3/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1068 2023-06-02 00:24:03.000000 erdgen-0.0.1rc3/LICENSE
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      169 2023-06-02 18:44:51.000000 erdgen-0.0.1rc3/MANIFEST.in
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4546 2023-06-04 00:50:21.336350 erdgen-0.0.1rc3/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3963 2023-06-04 00:49:31.000000 erdgen-0.0.1rc3/README.md
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-04 00:50:21.332350 erdgen-0.0.1rc3/erdgen/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc3/erdgen/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       87 2023-06-02 00:24:03.000000 erdgen-0.0.1rc3/erdgen/__main__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      419 2023-06-02 00:24:03.000000 erdgen-0.0.1rc3/erdgen/erdgen.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-04 00:50:21.336350 erdgen-0.0.1rc3/erdgen/src/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     3004 2023-06-02 18:44:51.000000 erdgen-0.0.1rc3/erdgen/src/_.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-02 00:24:03.000000 erdgen-0.0.1rc3/erdgen/src/__init__.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-04 00:50:21.336350 erdgen-0.0.1rc3/erdgen.egg-info/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     4546 2023-06-04 00:50:21.000000 erdgen-0.0.1rc3/erdgen.egg-info/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      281 2023-06-04 00:50:21.000000 erdgen-0.0.1rc3/erdgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-04 00:50:21.000000 erdgen-0.0.1rc3/erdgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-04 00:50:21.000000 erdgen-0.0.1rc3/erdgen.egg-info/requires.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        7 2023-06-04 00:50:21.000000 erdgen-0.0.1rc3/erdgen.egg-info/top_level.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       38 2023-06-04 00:50:21.336350 erdgen-0.0.1rc3/setup.cfg
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      962 2023-06-04 00:48:14.000000 erdgen-0.0.1rc3/setup.py
```

### Comparing `erdgen-0.0.1rc2/LICENSE` & `erdgen-0.0.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `erdgen-0.0.1rc2/PKG-INFO` & `erdgen-0.0.1rc3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,14 +16,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `erdgen`
 
 > DBT YML ERD Generator
 
+[![pypi](https://img.shields.io/pypi/v/erdgen?style=for-the-badge)](https://pypi.org/project/erdgen/)
+
 ## Overview
 
 This Python program generates Database Markup Language (DBML) Entity Relationship Diagram's (ERD) from the relationships node in your dbt YML files. The script parses the YML files, extracts relationships and columns, and outputs a DBML schema.
 
 The program is pretty opinionated. It requires each YML file to only contain one model. Further, the "relationships" node in dbt yml is a made-up construct.
 
 This program is useful for automated ERD generation if your dbt project doesn't have referential integrity or explicit SQL relationships. If your SQL models have defined SQL relationships there are better tools for automated ERD generation.
@@ -45,43 +47,41 @@
 
 The YML files are expected to have the following structure:
 
 ```yml
 version: 2
 
 models:
- - name: Computer
-   description: beep boop beep
-   columns:
-     - name: computerId
-       description: The unique identifier of computer
-     # other non-join key columns as necessary
-   relationships:
-     - name: files
-       description: The files are in the computer!?
-       type: one_to_many
-       table: computer_files
-       join:
-         - local: computerId
-           remote: computerId
+    - name: Computer
+      description: beep boop beep
+      columns:
+          - name: computerId
+            description: The unique identifier of computer
+          # other non-join key columns as necessary
+      relationships:
+          - name: files
+            description: The files are in the computer!?
+            type: one_to_many
+            table: computer_files
+            join:
+                - local: computerId
+                  remote: computerId
 ```
 
 **note**: Each YML file should contain only one model under the `models` node.
 
 ### Relationships
 
-The `relationships` node in the YAML files represents the relationship between the current model and other models. It is composed of several sub-nodes:
+The `relationships` node in the YML files represents the relationship between the current model and other models. It is composed of several sub-nodes:
 
 - `name`: The name of the relationship.
 - `description`: A brief description of the relationship.
-- `type`: The type of the relationship. It can be one_to_one, one_to_many, many_to_one, or many_to_many.
+- `type`: The type of the relationship. It can be `one_to_one`, `one_to_many`, `many_to_one`, or `many_to_many`.
 - `table`: The name of the other model involved in the relationship.
-- `join`: A list of the columns that are used for the join between the current model and the other model. Each item in the list is composed of 'local' and - 'remote' nodes, representing the column in the current model and the column in the other model, respectively.
-
-The type value can be one of the following: `one_to_one`, `one_to_many`, `many_to_one`, and `many_to_many`.
+- `join`: A list of the columns that are used for the join between the current model and the other model. Each item in the list is composed of `local` and - `remote` nodes, representing the column in the current model and the column in the other model, respectively.
 
 ## Output
 
 The output is a DBML schema that includes the tables, columns, and references based on the relationships defined in the YML files. The output is printed to the console.
 
 ## Notes
 
@@ -132,11 +132,10 @@
 make lint
 ```
 
 ## TODO
 
 - Add better error handling and reporting
 - Perhaps add a debug/verbose mode
-- Add tests lol
 - make it less jank
```

### Comparing `erdgen-0.0.1rc2/README.md` & `erdgen-0.0.1rc3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # `erdgen`
 
 > DBT YML ERD Generator
 
+[![pypi](https://img.shields.io/pypi/v/erdgen?style=for-the-badge)](https://pypi.org/project/erdgen/)
+
 ## Overview
 
 This Python program generates Database Markup Language (DBML) Entity Relationship Diagram's (ERD) from the relationships node in your dbt YML files. The script parses the YML files, extracts relationships and columns, and outputs a DBML schema.
 
 The program is pretty opinionated. It requires each YML file to only contain one model. Further, the "relationships" node in dbt yml is a made-up construct.
 
 This program is useful for automated ERD generation if your dbt project doesn't have referential integrity or explicit SQL relationships. If your SQL models have defined SQL relationships there are better tools for automated ERD generation.
@@ -27,43 +29,41 @@
 
 The YML files are expected to have the following structure:
 
 ```yml
 version: 2
 
 models:
- - name: Computer
-   description: beep boop beep
-   columns:
-     - name: computerId
-       description: The unique identifier of computer
-     # other non-join key columns as necessary
-   relationships:
-     - name: files
-       description: The files are in the computer!?
-       type: one_to_many
-       table: computer_files
-       join:
-         - local: computerId
-           remote: computerId
+    - name: Computer
+      description: beep boop beep
+      columns:
+          - name: computerId
+            description: The unique identifier of computer
+          # other non-join key columns as necessary
+      relationships:
+          - name: files
+            description: The files are in the computer!?
+            type: one_to_many
+            table: computer_files
+            join:
+                - local: computerId
+                  remote: computerId
 ```
 
 **note**: Each YML file should contain only one model under the `models` node.
 
 ### Relationships
 
-The `relationships` node in the YAML files represents the relationship between the current model and other models. It is composed of several sub-nodes:
+The `relationships` node in the YML files represents the relationship between the current model and other models. It is composed of several sub-nodes:
 
 - `name`: The name of the relationship.
 - `description`: A brief description of the relationship.
-- `type`: The type of the relationship. It can be one_to_one, one_to_many, many_to_one, or many_to_many.
+- `type`: The type of the relationship. It can be `one_to_one`, `one_to_many`, `many_to_one`, or `many_to_many`.
 - `table`: The name of the other model involved in the relationship.
-- `join`: A list of the columns that are used for the join between the current model and the other model. Each item in the list is composed of 'local' and - 'remote' nodes, representing the column in the current model and the column in the other model, respectively.
-
-The type value can be one of the following: `one_to_one`, `one_to_many`, `many_to_one`, and `many_to_many`.
+- `join`: A list of the columns that are used for the join between the current model and the other model. Each item in the list is composed of `local` and - `remote` nodes, representing the column in the current model and the column in the other model, respectively.
 
 ## Output
 
 The output is a DBML schema that includes the tables, columns, and references based on the relationships defined in the YML files. The output is printed to the console.
 
 ## Notes
 
@@ -114,9 +114,8 @@
 make lint
 ```
 
 ## TODO
 
 - Add better error handling and reporting
 - Perhaps add a debug/verbose mode
-- Add tests lol
 - make it less jank
```

### Comparing `erdgen-0.0.1rc2/erdgen/src/_.py` & `erdgen-0.0.1rc3/erdgen/src/_.py`

 * *Files identical despite different names*

### Comparing `erdgen-0.0.1rc2/erdgen.egg-info/PKG-INFO` & `erdgen-0.0.1rc3/erdgen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdgen
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Generate a DBML ERD from DBT YML relationships
 Home-page: https://github.com/neo-andrew-moss/erdgen
 Author: Andrew Moss
 Author-email: andrew.moss@neofinancial.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,14 +16,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `erdgen`
 
 > DBT YML ERD Generator
 
+[![pypi](https://img.shields.io/pypi/v/erdgen?style=for-the-badge)](https://pypi.org/project/erdgen/)
+
 ## Overview
 
 This Python program generates Database Markup Language (DBML) Entity Relationship Diagram's (ERD) from the relationships node in your dbt YML files. The script parses the YML files, extracts relationships and columns, and outputs a DBML schema.
 
 The program is pretty opinionated. It requires each YML file to only contain one model. Further, the "relationships" node in dbt yml is a made-up construct.
 
 This program is useful for automated ERD generation if your dbt project doesn't have referential integrity or explicit SQL relationships. If your SQL models have defined SQL relationships there are better tools for automated ERD generation.
@@ -45,43 +47,41 @@
 
 The YML files are expected to have the following structure:
 
 ```yml
 version: 2
 
 models:
- - name: Computer
-   description: beep boop beep
-   columns:
-     - name: computerId
-       description: The unique identifier of computer
-     # other non-join key columns as necessary
-   relationships:
-     - name: files
-       description: The files are in the computer!?
-       type: one_to_many
-       table: computer_files
-       join:
-         - local: computerId
-           remote: computerId
+    - name: Computer
+      description: beep boop beep
+      columns:
+          - name: computerId
+            description: The unique identifier of computer
+          # other non-join key columns as necessary
+      relationships:
+          - name: files
+            description: The files are in the computer!?
+            type: one_to_many
+            table: computer_files
+            join:
+                - local: computerId
+                  remote: computerId
 ```
 
 **note**: Each YML file should contain only one model under the `models` node.
 
 ### Relationships
 
-The `relationships` node in the YAML files represents the relationship between the current model and other models. It is composed of several sub-nodes:
+The `relationships` node in the YML files represents the relationship between the current model and other models. It is composed of several sub-nodes:
 
 - `name`: The name of the relationship.
 - `description`: A brief description of the relationship.
-- `type`: The type of the relationship. It can be one_to_one, one_to_many, many_to_one, or many_to_many.
+- `type`: The type of the relationship. It can be `one_to_one`, `one_to_many`, `many_to_one`, or `many_to_many`.
 - `table`: The name of the other model involved in the relationship.
-- `join`: A list of the columns that are used for the join between the current model and the other model. Each item in the list is composed of 'local' and - 'remote' nodes, representing the column in the current model and the column in the other model, respectively.
-
-The type value can be one of the following: `one_to_one`, `one_to_many`, `many_to_one`, and `many_to_many`.
+- `join`: A list of the columns that are used for the join between the current model and the other model. Each item in the list is composed of `local` and - `remote` nodes, representing the column in the current model and the column in the other model, respectively.
 
 ## Output
 
 The output is a DBML schema that includes the tables, columns, and references based on the relationships defined in the YML files. The output is printed to the console.
 
 ## Notes
 
@@ -132,11 +132,10 @@
 make lint
 ```
 
 ## TODO
 
 - Add better error handling and reporting
 - Perhaps add a debug/verbose mode
-- Add tests lol
 - make it less jank
```

### Comparing `erdgen-0.0.1rc2/setup.py` & `erdgen-0.0.1rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Andrew Moss",
     author_email="andrew.moss@neofinancial.com",
     python_requires=">=3.6",
     name="erdgen",
-    version="0.0.1rc2",
+    version="0.0.1rc3",
     description="Generate a DBML ERD from DBT YML relationships",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

