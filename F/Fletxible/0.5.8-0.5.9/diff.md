# Comparing `tmp/Fletxible-0.5.8.tar.gz` & `tmp/Fletxible-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.5.8.tar", last modified: Fri May 26 19:15:14 2023, max compression
+gzip compressed data, was "Fletxible-0.5.9.tar", last modified: Tue May 30 15:37:29 2023, max compression
```

## Comparing `Fletxible-0.5.8.tar` & `Fletxible-0.5.9.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 19:15:14.244223 Fletxible-0.5.8/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 19:15:14.236879 Fletxible-0.5.8/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-26 19:15:14.000000 Fletxible-0.5.8/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      714 2023-05-26 19:15:14.000000 Fletxible-0.5.8/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-26 19:15:14.000000 Fletxible-0.5.8/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       58 2023-05-26 19:15:14.000000 Fletxible-0.5.8/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-26 19:15:14.000000 Fletxible-0.5.8/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-05-26 19:15:14.000000 Fletxible-0.5.8/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.8/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-26 19:15:14.243855 Fletxible-0.5.8/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.8/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 19:15:14.237690 Fletxible-0.5.8/components/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.8/components/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-05-26 14:46:31.000000 Fletxible-0.5.8/components/block.py
--rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-05-26 14:46:31.000000 Fletxible-0.5.8/components/typography.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 19:15:14.240407 Fletxible-0.5.8/core/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.8/core/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1034 2023-05-26 14:46:31.000000 Fletxible-0.5.8/core/drawer.py
--rw-r--r--   0 ahmad      (501) staff       (20)      996 2023-05-26 14:46:31.000000 Fletxible-0.5.8/core/header.py
--rw-r--r--   0 ahmad      (501) staff       (20)      318 2023-05-26 14:46:31.000000 Fletxible-0.5.8/core/left_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)      557 2023-05-26 14:46:31.000000 Fletxible-0.5.8/core/middle_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4525 2023-05-26 14:46:31.000000 Fletxible-0.5.8/core/mobile_drop_down.py
--rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-05-26 14:46:31.000000 Fletxible-0.5.8/core/mobile_navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1874 2023-05-26 14:46:31.000000 Fletxible-0.5.8/core/navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1252 2023-05-26 14:46:31.000000 Fletxible-0.5.8/core/right_panel.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 19:15:14.241790 Fletxible-0.5.8/fletxible/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:15.000000 Fletxible-0.5.8/fletxible/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3450 2023-05-26 14:46:31.000000 Fletxible-0.5.8/fletxible/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-05-26 19:13:59.000000 Fletxible-0.5.8/fletxible/command.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2037 2023-05-26 14:46:31.000000 Fletxible-0.5.8/fletxible/fx_template.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1022 2023-05-26 16:21:14.000000 Fletxible-0.5.8/fletxible/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3319 2023-05-26 19:14:14.000000 Fletxible-0.5.8/fletxible/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-26 19:15:14.244293 Fletxible-0.5.8/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1219 2023-05-26 19:14:37.000000 Fletxible-0.5.8/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 19:15:14.242012 Fletxible-0.5.8/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.8/tests/test_route.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 19:15:14.243479 Fletxible-0.5.8/utilities/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 17:08:22.000000 Fletxible-0.5.8/utilities/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)      195 2023-05-26 16:04:02.000000 Fletxible-0.5.8/utilities/config.py
--rw-r--r--   0 ahmad      (501) staff       (20)      660 2023-05-26 14:46:31.000000 Fletxible-0.5.8/utilities/links.py
--rw-r--r--   0 ahmad      (501) staff       (20)      666 2023-05-26 14:46:31.000000 Fletxible-0.5.8/utilities/rail.py
--rw-r--r--   0 ahmad      (501) staff       (20)      366 2023-05-26 14:46:31.000000 Fletxible-0.5.8/utilities/router.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.765561 Fletxible-0.5.9/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.757663 Fletxible-0.5.9/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      727 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       58 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-05-30 15:37:29.000000 Fletxible-0.5.9/Fletxible.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.9/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-05-30 15:37:29.765346 Fletxible-0.5.9/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-05-30 15:35:48.000000 Fletxible-0.5.9/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.758381 Fletxible-0.5.9/components/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.9/components/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-05-26 14:46:31.000000 Fletxible-0.5.9/components/block.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-05-26 14:46:31.000000 Fletxible-0.5.9/components/typography.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.761611 Fletxible-0.5.9/core/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.9/core/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1193 2023-05-30 13:09:25.000000 Fletxible-0.5.9/core/drawer.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4190 2023-05-30 13:09:25.000000 Fletxible-0.5.9/core/header.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      318 2023-05-26 14:46:31.000000 Fletxible-0.5.9/core/left_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1185 2023-05-30 12:19:20.000000 Fletxible-0.5.9/core/middle_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4525 2023-05-28 17:50:12.000000 Fletxible-0.5.9/core/mobile_drop_down.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-05-26 14:46:31.000000 Fletxible-0.5.9/core/mobile_navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2022 2023-05-30 13:09:25.000000 Fletxible-0.5.9/core/navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1109 2023-05-29 09:33:45.000000 Fletxible-0.5.9/core/repo.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1252 2023-05-26 14:46:31.000000 Fletxible-0.5.9/core/right_panel.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.763158 Fletxible-0.5.9/fletxible/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:12.000000 Fletxible-0.5.9/fletxible/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4533 2023-05-30 15:36:50.000000 Fletxible-0.5.9/fletxible/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-05-30 15:36:50.000000 Fletxible-0.5.9/fletxible/command.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2066 2023-05-30 15:36:50.000000 Fletxible-0.5.9/fletxible/fx_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1089 2023-05-30 15:36:50.000000 Fletxible-0.5.9/fletxible/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4216 2023-05-30 15:36:50.000000 Fletxible-0.5.9/fletxible/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-30 15:37:29.765631 Fletxible-0.5.9/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1213 2023-05-30 15:37:03.000000 Fletxible-0.5.9/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.763411 Fletxible-0.5.9/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.9/tests/test_route.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-30 15:37:29.765008 Fletxible-0.5.9/utilities/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 17:08:22.000000 Fletxible-0.5.9/utilities/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      195 2023-05-26 16:04:02.000000 Fletxible-0.5.9/utilities/config.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      660 2023-05-29 12:14:30.000000 Fletxible-0.5.9/utilities/links.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      666 2023-05-30 09:09:24.000000 Fletxible-0.5.9/utilities/rail.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      366 2023-05-26 14:46:31.000000 Fletxible-0.5.9/utilities/router.py
```

### Comparing `Fletxible-0.5.8/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.5.9/Fletxible.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.8
+Version: 0.5.9
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
-Keywords: python web template,web application,development
+Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.
```

### Comparing `Fletxible-0.5.8/Fletxible.egg-info/SOURCES.txt` & `Fletxible-0.5.9/Fletxible.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 core/drawer.py
 core/header.py
 core/left_panel.py
 core/middle_panel.py
 core/mobile_drop_down.py
 core/mobile_navigation.py
 core/navigation.py
+core/repo.py
 core/right_panel.py
 fletxible/__init__.py
 fletxible/base.py
 fletxible/command.py
 fletxible/fx_template.py
 fletxible/main.py
 fletxible/script.py
```

### Comparing `Fletxible-0.5.8/LICENSE` & `Fletxible-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.8/PKG-INFO` & `Fletxible-0.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.8
+Version: 0.5.9
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
-Keywords: python web template,web application,development
+Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.
```

### Comparing `Fletxible-0.5.8/README.md` & `Fletxible-0.5.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,77 +3,91 @@
 
 
 
 <div align="center">
   <a href="https://github.com/LineIndent/fletxible/actions/workflows/build.yml">
     <img src="https://github.com/LineIndent/fletxible/actions/workflows/build.yml/badge.svg" alt="Build Status">
   </a>
-  <a href="https://fletxible.readthedocs.io/en/latest/?badge=latest">
+  <!-- <a href="https://fletxible.readthedocs.io/en/latest/?badge=latest">
     <img src="https://readthedocs.org/projects/fletxible/badge/?version=latest" alt="Documentation">
-  </a>
-  <a href="https://pypi.org/project/fletxible/">
+  </a> -->
+  <!-- <a href="https://pypi.org/project/fletxible/">
     <img src="https://img.shields.io/pypi/pyversions/fletxible.svg" alt="Python version">
-  </a>
+  </a> -->
   <a href="https://pypi.org/project/Fletxible/">
-    <img src="https://img.shields.io/pypi/v/Fletxible.svg" alt="PyPI version">
+    <img src="https://img.shields.io/pypi/v/Fletxible.svg" alt="PyPI version", style="background-color: blue;">
   </a>
   <a href="https://pypi.org/project/fletxible/">
     <img src="https://img.shields.io/pypi/dm/fletxible.svg" alt="PyPI downloads">
   </a>
 </div>
 
 <br>
 
 <p align="center">
 Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.</p>
 
+<img src="./assets/fletxible.png">
 
 
-## 1. Installation
+## Installation
 
 To use Fletxible, you need to have the following installed:
 
 -   Latest version of Flet
 -   Python 3.5+
 
 If you don't have Flet installed, installing Fletxible automatically installs it for you. You can install Fletxible using the following command:
-```
+```py
 $ pip install Fletxible
 ```
 
 
 
-## 2. Application Setup
+## Application Setup
 
 After installing Fletxible, you can test if it's working properly by running the following command:
 
-```
+```py
 $ fletxible-init
 ```
 
-If the package was installed correctly, a directory named ```logic``` along with a file called ```flet_config.yml``` will be generated inside the root directory.
+If the package was installed correctly, a file called ```fx_config.yml``` will be generated inside the root directory. Other directories and files will also be generated.
 
-The ```logic``` directory will contain four files:
+## 3. Quick Start
 
-1. ```__init__.py```
-2. ```main.py```
-3. ```script.py```
-4. ```utilities.py```
+Open the  ```fx_config.yml``` file and configure the document as needed. Change the site name, repository link, as well as any theme related settings.
 
-## 3. Current Algorithm Functions
+When you're ready, run the following command to generate your files/pages:
+```py
+python3 script.py
+```
+
+If successful, the script should generate files inside a directory named ```web``` corresponding to the names under the **navigation** header inside the ```fx_config.yml```. 
+
+You can then run the following command to see your application:
+
+```py
+python3 main.py
+```
+
+If the setup has no error, you can start customizing your pages by adding in your personal layout directly within the generated pages inside the ```web``` directory.
+
+
+## Current Algorithm Functions
 
 This algorithm is a script that loads and processes data from a YAML file ```flet_config.yml``` that contains navigation information for a web application. The script then updates and creates various files and directories necessary for the application to function.
 
 Here is a summary of what the algorithm does (v0.2.0):
 
 1. Import necessary libraries and functions
 2. Define a dictionary variable to hold route keys
 
 3. Define several functions to perform various tasks:
-   1. open_yaml_script(): Loads data from the "flet_config.yml" file.
+   1. open_yaml_script(): Loads data from the "fx_config.yml" file.
    2. check_pages_directory_script(): Checks if a "pages" directory exists and creates one if not.
    3. update_pages_directory_script(docs: dict): Loops over the files in the "pages" directory and deletes any files that are not listed in the navigation information.
    4. handle_navigation_routing_script(docs: dict): Loops over the navigation information and writes route strings to a temporary file.
    5. set_application_routing_script(docs: dict): Reads the temporary file created in the previous step, creates a route.py file with the appropriate routes, and deletes the temporary file.
    6. set_default_methods_script(docs: dict): Loops over the navigation information and creates default pages for each page listed, and creates a route.pickle file with information about the modules used in the application. 
    7. map_yaml(yaml_file_path, output_file_path): Reads a YAML file and writes its contents to a Python file with a specified filename.
    8. script(page: ft.Page): Main function that calls the other functions to process the data and set up the application.
@@ -83,12 +97,8 @@
 ## Contributing
 
 Contributions are highly encouraged and welcomed.
 
 
 ## License
 
-Fletxible is open-source and licensed under the [MIT License](LICENSE).
-
-
-
-
+Fletxible is open-source and licensed under the [MIT License](LICENSE).
```

#### html2text {}

```diff
@@ -1,45 +1,54 @@
                            ****** fletxible. ******
-[Build_Status] [Documentation] [Python_version] [PyPI_version] [PyPI_downloads]
+                               [Build_Status]
+                        style="background-color: blue;">
+ [PyPI_downloads]
 
    Fletxible is a Python web boilerplate project designed to provide a solid
   foundation for building web applications with Python and Flet. The project
   comes pre-configured with a range of tools and features to make it easy for
   developers to get started building their applications, without the need to
           spend time setting up infrastructure or configuring tools.
-## 1. Installation To use Fletxible, you need to have the following installed:
-- Latest version of Flet - Python 3.5+ If you don't have Flet installed,
-installing Fletxible automatically installs it for you. You can install
-Fletxible using the following command: ``` $ pip install Fletxible ``` ## 2.
-Application Setup After installing Fletxible, you can test if it's working
-properly by running the following command: ``` $ fletxible-init ``` If the
-package was installed correctly, a directory named ```logic``` along with a
-file called ```flet_config.yml``` will be generated inside the root directory.
-The ```logic``` directory will contain four files: 1. ```__init__.py``` 2.
-```main.py``` 3. ```script.py``` 4. ```utilities.py``` ## 3. Current Algorithm
-Functions This algorithm is a script that loads and processes data from a YAML
-file ```flet_config.yml``` that contains navigation information for a web
-application. The script then updates and creates various files and directories
-necessary for the application to function. Here is a summary of what the
-algorithm does (v0.2.0): 1. Import necessary libraries and functions 2. Define
-a dictionary variable to hold route keys 3. Define several functions to perform
-various tasks: 1. open_yaml_script(): Loads data from the "flet_config.yml"
-file. 2. check_pages_directory_script(): Checks if a "pages" directory exists
-and creates one if not. 3. update_pages_directory_script(docs: dict): Loops
-over the files in the "pages" directory and deletes any files that are not
-listed in the navigation information. 4. handle_navigation_routing_script(docs:
-dict): Loops over the navigation information and writes route strings to a
-temporary file. 5. set_application_routing_script(docs: dict): Reads the
-temporary file created in the previous step, creates a route.py file with the
-appropriate routes, and deletes the temporary file. 6.
-set_default_methods_script(docs: dict): Loops over the navigation information
-and creates default pages for each page listed, and creates a route.pickle file
-with information about the modules used in the application. 7. map_yaml
-(yaml_file_path, output_file_path): Reads a YAML file and writes its contents
-to a Python file with a specified filename. 8. script(page: ft.Page): Main
-function that calls the other functions to process the data and set up the
-application. Overall, the script is part of a larger application development
-process that involves reading and processing data from a YAML file, creating
-and updating various files and directories, and setting up routing information
-for a web application. ## Contributing Contributions are highly encouraged and
-welcomed. ## License Fletxible is open-source and licensed under the [MIT
-License](LICENSE).
+[./assets/fletxible.png] ## Installation To use Fletxible, you need to have the
+following installed: - Latest version of Flet - Python 3.5+ If you don't have
+Flet installed, installing Fletxible automatically installs it for you. You can
+install Fletxible using the following command: ```py $ pip install Fletxible
+``` ## Application Setup After installing Fletxible, you can test if it's
+working properly by running the following command: ```py $ fletxible-init ```
+If the package was installed correctly, a file called ```fx_config.yml``` will
+be generated inside the root directory. Other directories and files will also
+be generated. ## 3. Quick Start Open the ```fx_config.yml``` file and configure
+the document as needed. Change the site name, repository link, as well as any
+theme related settings. When you're ready, run the following command to
+generate your files/pages: ```py python3 script.py ``` If successful, the
+script should generate files inside a directory named ```web``` corresponding
+to the names under the **navigation** header inside the ```fx_config.yml```.
+You can then run the following command to see your application: ```py python3
+main.py ``` If the setup has no error, you can start customizing your pages by
+adding in your personal layout directly within the generated pages inside the
+```web``` directory. ## Current Algorithm Functions This algorithm is a script
+that loads and processes data from a YAML file ```flet_config.yml``` that
+contains navigation information for a web application. The script then updates
+and creates various files and directories necessary for the application to
+function. Here is a summary of what the algorithm does (v0.2.0): 1. Import
+necessary libraries and functions 2. Define a dictionary variable to hold route
+keys 3. Define several functions to perform various tasks: 1. open_yaml_script
+(): Loads data from the "fx_config.yml" file. 2. check_pages_directory_script
+(): Checks if a "pages" directory exists and creates one if not. 3.
+update_pages_directory_script(docs: dict): Loops over the files in the "pages"
+directory and deletes any files that are not listed in the navigation
+information. 4. handle_navigation_routing_script(docs: dict): Loops over the
+navigation information and writes route strings to a temporary file. 5.
+set_application_routing_script(docs: dict): Reads the temporary file created in
+the previous step, creates a route.py file with the appropriate routes, and
+deletes the temporary file. 6. set_default_methods_script(docs: dict): Loops
+over the navigation information and creates default pages for each page listed,
+and creates a route.pickle file with information about the modules used in the
+application. 7. map_yaml(yaml_file_path, output_file_path): Reads a YAML file
+and writes its contents to a Python file with a specified filename. 8. script
+(page: ft.Page): Main function that calls the other functions to process the
+data and set up the application. Overall, the script is part of a larger
+application development process that involves reading and processing data from
+a YAML file, creating and updating various files and directories, and setting
+up routing information for a web application. ## Contributing Contributions are
+highly encouraged and welcomed. ## License Fletxible is open-source and
+licensed under the [MIT License](LICENSE).
```

### Comparing `Fletxible-0.5.8/components/block.py` & `Fletxible-0.5.9/components/block.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.8/core/mobile_drop_down.py` & `Fletxible-0.5.9/core/mobile_drop_down.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.8/core/right_panel.py` & `Fletxible-0.5.9/core/right_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.8/fletxible/base.py` & `Fletxible-0.5.9/fletxible/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from core.mobile_drop_down import MobileDropDownNavigation
+# from core.mobile_drop_down import MobileDropDownNavigation
 from core.mobile_navigation import MobileNavigation
 from core.middle_panel import MiddlePanel
 from core.right_panel import RightPanel
 from core.navigation import Navigation
 from core.left_panel import LeftPanel
 from core.header import Header
 from core.drawer import Drawer
@@ -17,54 +17,85 @@
         self.fx_rail = fx_rail
 
         self.fx_stack = ft.Stack(expand=True)
         self.fx_row = ft.Row(expand=True, spacing=2)
 
         self.fx_drawer = Drawer()
 
-        # Bug: control is not being added to page ...
-        self.fx_drop_down = MobileDropDownNavigation(2890, [])
-        # self.fx_controls[1] = self.fx_drop_down
-
-        self.fx_left = LeftPanel()
-        self.fx_middle = MiddlePanel(controls=self.fx_controls)
-        self.fx_right = RightPanel(middle_panel=self.fx_middle, fx_rail=self.fx_rail)
-
         self.fx_max_nav = Navigation(
             page=self.page, function=lambda e: self.set_app_router(e)
         )
         self.fx_min_nav = MobileNavigation(on_click=lambda e: self.set_fx_drawer(e))
 
         self.fx_header = Header(full_nav=self.fx_max_nav, mobile_nav=self.fx_min_nav)
+        # Bug: control is not being added to page ...
+        # self.fx_drop_down = MobileDropDownNavigation(120, self.page, [])
+
+        self.fx_left = LeftPanel()
+        self.fx_middle = MiddlePanel(
+            controls=self.fx_controls,
+            function=[
+                self.set_fx_header,
+                self.set_header_navigation_row,
+            ],
+            page=self.page,
+        )
+        self.fx_right = RightPanel(middle_panel=self.fx_middle, fx_rail=self.fx_rail)
 
         super().__init__()
 
     # Method: Responsive method to set the UI for 'mobile/tablet' screens ...
     def set_application_to_mobile(self):
-        self.set_fx_max_nav(False)
+        self.set_fx_max_nav(0, False)
         self.set_fx_left(False)
         self.set_fx_right(False)
 
         self.set_fx_min_nav(True)
         # self.set_fx_drop_down(True)
 
+        self.set_fx_header(60)
+        self.set_header_repo_opacity(0, False)
+        self.set_header_navigation_row(0, False)
+
     # Method: Responsive method to set the UI for 'desktop' screens ...
     def set_application_to_desktop(self):
         self.set_fx_left(True)
         self.set_fx_right(True)
-        self.set_fx_max_nav(True)
+        self.set_fx_max_nav(1, True)
 
         self.set_fx_min_nav(False)
         # self.set_fx_drop_down(False)
 
+        self.set_fx_header(90)
+        self.set_header_repo_opacity(1, True)
+        self.set_header_navigation_row(1, True)
+
+    # Method: sets the state of the header with animations ...
+    def set_header_navigation_row(self, value: int, state: bool):
+        self.fx_header.navigation.opacity = value
+        self.fx_header.navigation.visible = state
+        self.fx_header.navigation.update()
+
+    def set_header_repo_opacity(self, value: int, state: bool):
+        self.fx_header.repo.controls[1].opacity = value
+        self.fx_header.repo.controls[1].visible = state
+        self.fx_header.repo.update()
+
+    def set_fx_header(self, height: int):
+        self.fx_header.height = height
+        self.fx_header.update()
+
     def set_fx_drop_down(self, state: bool):
         self.fx_drop_down.visible = state
         self.fx_drop_down.update()
 
-    def set_fx_max_nav(self, state: bool):
+    def set_fx_max_nav(self, value: int, state: bool):
+        self.fx_max_nav.opacity = value
+        self.fx_max_nav.update()
+
         self.fx_max_nav.visible = state
         self.fx_max_nav.update()
 
     def set_fx_min_nav(self, state: bool):
         self.fx_min_nav.visible = state
         self.fx_min_nav.update()
```

### Comparing `Fletxible-0.5.8/fletxible/command.py` & `Fletxible-0.5.9/fletxible/command.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.8/fletxible/fx_template.py` & `Fletxible-0.5.9/fletxible/fx_template.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 class FxView(ft.View):
     def __init__(
         self,
         page: ft.Page,
         route="",  # set your routes here ...
+        # bgcolor="#2e303d",
         bgcolor="#23262d",
         padding=0,
     ) -> None:
         self.page = page
         self.page.on_resize = self.fx_dynamics
         self.fx_view = FxControls(self.page, self.fx_controls(), self.fx_rail())
 
@@ -38,15 +39,15 @@
     # Method: Create your side rails(fx_right panel) here by passing in strings...
     def fx_rail(self):
         return []
 
     # Method: Create your layout here. Create your UI inside this list ...
     def fx_controls(self, fx_drop_down_placeholder=ft.Container()) -> list:
         return [
-            ft.Divider(height=15, color="transparent"),
+            ft.Divider(height=45, color="transparent"),
             # start your layout design here ...
             fx_drop_down_placeholder,  # DO NOT remove this placeholder ...
             fxType.heading(f"Hi! Welcome to Fletxible!!"),
             fxType.subtitle("Start building your website with fletxible!!"),
             ft.Divider(height=5, color="transparent"),
             fxType.paragraph(
                 "You can install Fletxible using with the following command: "
```

### Comparing `Fletxible-0.5.8/fletxible/main.py` & `Fletxible-0.5.9/fletxible/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 import importlib.util
 import flet as ft
 import os
+import yaml
+
+
+with open("fx_config.yml", "r") as file:
+    docs: dict = yaml.safe_load(file)
 
 
 def main(page: ft.Page):
     # Web theme ...
     theme = ft.Theme(
         scrollbar_theme=ft.ScrollbarTheme(
             thickness=4,
@@ -27,16 +32,15 @@
 
     for key, __ in router.items():
         page.views.append(router[key].loader.load_module().FxView(page))
 
     page.data = router
     page.update()
 
-    for view in page.views[:]:
-        if view.route:
-            view.fx_dynamics(event=None)
+    for view in page.views[1:]:
+        view.fx_dynamics(event=None)
 
     page.update()
 
 
 if __name__ == "__main__":
     ft.flet.app(target=main)
```

### Comparing `Fletxible-0.5.8/fletxible/script.py` & `Fletxible-0.5.9/fletxible/script.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import yaml
 import os
 from utilities.router import fx_router
 from utilities.links import fx_nav_links
 
 
 def open_yaml_script() -> dict:
-    # Load the YAML file
     with open("fx_config.yml", "r") as file:
         docs = yaml.safe_load(file)
 
     return docs
 
 
 def check_fweb_directory_exists():
-    # Check if "fWeb" directory exists
     _dir = None
     for root, dirs, files in os.walk("."):
         if "web" in dirs:
             _dir = os.path.join(root, "web")
             break
 
         if not _dir:
@@ -41,14 +39,44 @@
     with open("temp.txt", "w") as f:
         for page in docs["navigation"]:
             for key in page:
                 route = os.path.splitext(page[key])[0]
                 f.write(f"{fx_router(route)}")
 
 
+def set_site_name(docs: dict):
+    site_name = f"'{docs['site-name']}',"
+
+    with open("./core/header.py", "r") as fHeader:
+        header = fHeader.read()
+
+    with open("./core/drawer.py", "r") as fDrawer:
+        drawer = fDrawer.read()
+
+    header_start_idx = header.index("# start #")
+    header_end_idx = header.index("# end #")
+
+    drawer_start_idx = drawer.index("# start #")
+    drawer_end_idx = drawer.index("# end #")
+
+    header_modified_string = (
+        header[:header_start_idx] + "# start #\n" + site_name + header[header_end_idx:]
+    )
+
+    drawer_modified_string = (
+        drawer[:drawer_start_idx] + "# start #\n" + site_name + drawer[drawer_end_idx:]
+    )
+
+    with open("./core/header.py", "w") as w:
+        w.write(header_modified_string)
+
+    with open("./core/drawer.py", "w") as w:
+        w.write(drawer_modified_string)
+
+
 def create_router_file():
     with open("temp.txt", "r") as r:
         routers = r.read()
 
     with open("./core/navigation.py", "r") as r:
         pre_code = r.read()
 
@@ -123,14 +151,20 @@
     try:
         temporary_file_for_routing(docs)
 
     except Exception as e:
         print(e)
 
     try:
+        set_site_name(docs)
+
+    except Exception as e:
+        print("Site-name error: ", e)
+
+    try:
         create_router_file()
 
     except Exception as e:
         print(e)
 
     try:
         create_fx_views(docs)
```

### Comparing `Fletxible-0.5.8/setup.py` & `Fletxible-0.5.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Fletxible",
-    version="0.5.8",
+    version="0.5.9",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=[
@@ -22,9 +22,9 @@
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
             "fletxible-init=fletxible.command:init",
         ],
     },
-    keywords=["python web template", "web application", "development"],
+    keywords=["python web template", "web application", "theme"],
 )
```

### Comparing `Fletxible-0.5.8/utilities/links.py` & `Fletxible-0.5.9/utilities/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     for file in os.listdir("web"):
         # Set the path of the file to loop over folders and only include files
         path = os.path.join("web", file)
 
         # If the path is NOT a folder, continue ...
         if not os.path.isdir(path):
             filename = os.path.splitext(file)[0]
-            string = f"ft.Text(size=13, weight='bold', spans=[ft.TextSpan('{filename.capitalize()}', data='/{filename}', on_click=lambda e: self.set_app_router(e))]),"
+            string = f"ft.Text(size=11, weight='bold', spans=[ft.TextSpan('{filename.capitalize()}', data='/{filename}', on_click=lambda e: self.set_app_router(e))]),"
             links.append(string)
 
     return links
```

### Comparing `Fletxible-0.5.8/utilities/rail.py` & `Fletxible-0.5.9/utilities/rail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import flet as ft
 
 
 def create_rail(number: int, title: list, funcOne: list, funcTwo: list):
     rail_list: list = [
-        ft.Divider(height=10, color="transparent"),
+        ft.Divider(height=35, color="transparent"),
     ]
 
     if number != 0:
         for index in range(number):
             rail_list.append(
                 ft.Container(
                     content=ft.Text(
```

