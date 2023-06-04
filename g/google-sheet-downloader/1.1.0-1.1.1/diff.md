# Comparing `tmp/google-sheet-downloader-1.1.0.tar.gz` & `tmp/google-sheet-downloader-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-sheet-downloader-1.1.0.tar", last modified: Sun Jun  4 09:17:29 2023, max compression
+gzip compressed data, was "google-sheet-downloader-1.1.1.tar", last modified: Sun Jun  4 12:17:35 2023, max compression
```

## Comparing `google-sheet-downloader-1.1.0.tar` & `google-sheet-downloader-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-04 09:17:29.863986 google-sheet-downloader-1.1.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4670 2023-06-04 09:17:29.863864 google-sheet-downloader-1.1.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     4489 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-04 09:17:29.863677 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     4670 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       74 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       24 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3968 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/google_sheet_downloader.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-04 09:17:29.864026 google-sheet-downloader-1.1.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      556 2023-06-04 09:17:29.000000 google-sheet-downloader-1.1.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-04 12:17:35.566151 google-sheet-downloader-1.1.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4670 2023-06-04 12:17:35.566036 google-sheet-downloader-1.1.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4489 2023-06-04 12:17:35.000000 google-sheet-downloader-1.1.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-04 12:17:35.565856 google-sheet-downloader-1.1.1/google_sheet_downloader.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     4670 2023-06-04 12:17:35.000000 google-sheet-downloader-1.1.1/google_sheet_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      329 2023-06-04 12:17:35.000000 google-sheet-downloader-1.1.1/google_sheet_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-04 12:17:35.000000 google-sheet-downloader-1.1.1/google_sheet_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       74 2023-06-04 12:17:35.000000 google-sheet-downloader-1.1.1/google_sheet_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       75 2023-06-04 12:17:35.000000 google-sheet-downloader-1.1.1/google_sheet_downloader.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       24 2023-06-04 12:17:35.000000 google-sheet-downloader-1.1.1/google_sheet_downloader.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3996 2023-06-04 12:17:35.000000 google-sheet-downloader-1.1.1/google_sheet_downloader.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-04 12:17:35.566186 google-sheet-downloader-1.1.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      556 2023-06-04 12:17:35.000000 google-sheet-downloader-1.1.1/setup.py
```

### Comparing `google-sheet-downloader-1.1.0/PKG-INFO` & `google-sheet-downloader-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 積木塊：Google Sheets 下載器 by Bowen Chiu
```

### Comparing `google-sheet-downloader-1.1.0/README.md` & `google-sheet-downloader-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `google-sheet-downloader-1.1.0/google_sheet_downloader.egg-info/PKG-INFO` & `google-sheet-downloader-1.1.1/google_sheet_downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheet-downloader
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # 積木塊：Google Sheets 下載器 by Bowen Chiu
```

### Comparing `google-sheet-downloader-1.1.0/google_sheet_downloader.py` & `google-sheet-downloader-1.1.1/google_sheet_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,21 @@
 def is_downloaded(output_folder, sheet_id):
     pattern = os.path.join(output_folder, f"doc-id_{sheet_id}*.csv")
     matching_files = glob.glob(pattern)
 
     return len(matching_files) > 0
 
 
+def short_sha(str1):
+    return hashlib.sha256(str1.encode()).hexdigest()[:8]
+
+
 def save_to_csv(data, output_folder, sheet_name, worksheet_name, sheet_id):
     os.makedirs(output_folder, exist_ok=True)
-    sha256_digest = hashlib.sha256(f"{sheet_name}_{worksheet_name}".encode()).hexdigest()
+    sha256_digest = short_sha(f"{sheet_name}_{worksheet_name}")
     output_file = os.path.join(output_folder,
                                f"doc-id_{sheet_id}_sha_{sha256_digest}.csv")
     with open(output_file, 'w', newline='', encoding='utf-8') as f:
         writer = csv.writer(f)
         writer.writerows(data)
     return output_file
 
@@ -85,15 +89,15 @@
             sheet_name = sheet.title
             worksheet_name = worksheet.title
 
             data = get_all_values(gspread_client, sheet_id, worksheet_name)
             csv_file_name = save_to_csv(data, output_folder, sheet_name, worksheet_name, sheet_id)
 
             download_time = datetime.datetime.utcnow().isoformat() + "Z"
-            sha256_digest = hashlib.sha256(f"{sheet_name}_{worksheet_name}".encode()).hexdigest()
+            sha256_digest = short_sha(f"{sheet_name}_{worksheet_name}")
             metadata = {
                 "sheet_id": sheet_id,
                 "sheet_name": sheet_name,
                 "worksheet_name": worksheet_name,
                 "download_time": download_time,
                 "download_filename": csv_file_name
             }
```

### Comparing `google-sheet-downloader-1.1.0/setup.py` & `google-sheet-downloader-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="google-sheet-downloader",
-    version="1.1.0",
+    version="1.1.1",
     packages=find_packages(),
     py_modules=['google_sheet_downloader'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'google_sheet_downloader = google_sheet_downloader:main',
         ],
```

