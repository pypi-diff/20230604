# Comparing `tmp/google-sheet-downloader-1.0.7.tar.gz` & `tmp/google-sheet-downloader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-sheet-downloader-1.0.7.tar", last modified: Wed May 24 06:36:34 2023, max compression
+gzip compressed data, was "google-sheet-downloader-1.1.0.tar", last modified: Sun Jun  4 09:17:29 2023, max compression
```

## Comparing `google-sheet-downloader-1.0.7.tar` & `google-sheet-downloader-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:36:34.620302 google-sheet-downloader-1.0.7/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4670 2023-05-24 06:36:34.620167 google-sheet-downloader-1.0.7/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     4489 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-24 06:36:34.619937 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4670 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       74 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       24 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3206 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/google_sheet_downloader.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-24 06:36:34.620350 google-sheet-downloader-1.0.7/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      556 2023-05-24 06:36:34.000000 google-sheet-downloader-1.0.7/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-04 09:17:29.863986 google-sheet-downloader-1.1.0/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4670 2023-06-04 09:17:29.863864 google-sheet-downloader-1.1.0/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4489 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-04 09:17:29.863677 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4670 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       74 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       24 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3968 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-04 09:17:29.864026 google-sheet-downloader-1.1.0/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      556 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/setup.py
```

### Comparing `google-sheet-downloader-1.0.7/PKG-INFO` & `google-sheet-downloader-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.0.7
+Version: 1.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 積木塊：Google Sheets 下載器 by Bowen Chiu
```

### Comparing `google-sheet-downloader-1.0.7/README.md` & `google-sheet-downloader-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `google-sheet-downloader-1.0.7/google_sheet_downloader.egg-info/PKG-INFO` & `google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.0.7
+Version: 1.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 積木塊：Google Sheets 下載器 by Bowen Chiu
```

### Comparing `google-sheet-downloader-1.0.7/google_sheet_downloader.py` & `google-sheet-downloader-1.1.0/google_sheet_downloader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
-# google_sheet_downloader.py
 import argparse
 import csv
+import datetime
 import glob
 import hashlib
 import json
 import os
 
 import gspread
 from google.oauth2.service_account import Credentials
@@ -18,15 +18,15 @@
         "https://www.googleapis.com/auth/drive.file",
         "https://www.googleapis.com/auth/drive"
     ]
     with open(key_file, 'r') as f:
         dic = json.load(f)
     credentials = Credentials.from_service_account_info(dic, scopes=scopes)
     gspread_client = gspread.authorize(credentials)
-    return gspread_client
+    return gspread_client, credentials
 
 
 def get_all_values(gspread_client, sheet_id, worksheet_name=''):
     spreadsheet = gspread_client.open_by_key(sheet_id)
     if worksheet_name == '':
         worksheet = spreadsheet.worksheets()[0]
     else:
@@ -45,46 +45,63 @@
     os.makedirs(output_folder, exist_ok=True)
     sha256_digest = hashlib.sha256(f"{sheet_name}_{worksheet_name}".encode()).hexdigest()
     output_file = os.path.join(output_folder,
                                f"doc-id_{sheet_id}_sha_{sha256_digest}.csv")
     with open(output_file, 'w', newline='', encoding='utf-8') as f:
         writer = csv.writer(f)
         writer.writerows(data)
+    return output_file
+
+
+def save_to_json(metadata, output_folder, sheet_id, sha256_digest):
+    os.makedirs(output_folder, exist_ok=True)
+    output_file = os.path.join(output_folder,
+                               f"doc-id_{sheet_id}_sha_{sha256_digest}.json")
+    with open(output_file, 'w', encoding='utf-8') as f:
+        json.dump(metadata, f, indent=4, ensure_ascii=False)
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description="Google Sheet Downloader")
     parser.add_argument('--key-file', required=True, help="Google service account key JSON file path")
     parser.add_argument('--sheet-ids', required=True, help="Comma separated Google sheet IDs to download")
     parser.add_argument('--output-folder', required=True, help="Output folder path for CSV files")
     parser.add_argument('--force', action='store_true', help="Force download and ignore cache")
 
     return parser.parse_args()
 
 
 def download_google_sheets(key_file, sheet_ids, output_folder, force):
-    gspread_client = None
+    gspread_client, credentials = None, None
 
     for sheet_id in sheet_ids.split(','):
         if not force and is_downloaded(output_folder, sheet_id):
-            # print(f"Skipping: Sheet ID {sheet_id} (Already downloaded)")
             continue
 
-        if gspread_client is None:
-            gspread_client = init_gspread(key_file)
+        if gspread_client is None or credentials is None:
+            gspread_client, credentials = init_gspread(key_file)
 
         sheet = gspread_client.open_by_key(sheet_id)
         for worksheet in sheet.worksheets():
             sheet_name = sheet.title
             worksheet_name = worksheet.title
-            # print(f"Checking: {sheet_name} - {worksheet_name}")
 
             data = get_all_values(gspread_client, sheet_id, worksheet_name)
-            save_to_csv(data, output_folder, sheet_name, worksheet_name, sheet_id)
-            # print(f"Saved: {sheet_name} - {worksheet_name}")
+            csv_file_name = save_to_csv(data, output_folder, sheet_name, worksheet_name, sheet_id)
+
+            download_time = datetime.datetime.utcnow().isoformat() + "Z"
+            sha256_digest = hashlib.sha256(f"{sheet_name}_{worksheet_name}".encode()).hexdigest()
+            metadata = {
+                "sheet_id": sheet_id,
+                "sheet_name": sheet_name,
+                "worksheet_name": worksheet_name,
+                "download_time": download_time,
+                "download_filename": csv_file_name
+            }
+            save_to_json(metadata, output_folder, sheet_id, sha256_digest)
 
 
 def main():
     args = parse_arguments()
     download_google_sheets(args.key_file, args.sheet_ids, args.output_folder, args.force)
```

### Comparing `google-sheet-downloader-1.0.7/setup.py` & `google-sheet-downloader-1.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="google-sheet-downloader",
-    version="1.0.7",
+    version="1.1.0",
     packages=find_packages(),
     py_modules=['google_sheet_downloader'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'google_sheet_downloader = google_sheet_downloader:main',
         ],
```

