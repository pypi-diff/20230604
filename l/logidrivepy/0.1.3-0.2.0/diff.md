# Comparing `tmp/logidrivepy-0.1.3.tar.gz` & `tmp/logidrivepy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logidrivepy-0.1.3.tar", last modified: Sat May 27 10:20:39 2023, max compression
+gzip compressed data, was "logidrivepy-0.2.0.tar", last modified: Sun Jun  4 11:19:33 2023, max compression
```

## Comparing `logidrivepy-0.1.3.tar` & `logidrivepy-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 10:20:39.069082 logidrivepy-0.1.3/
--rw-rw-rw-   0        0        0     1087 2023-05-23 22:21:13.000000 logidrivepy-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3469 2023-05-27 10:20:39.068082 logidrivepy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2770 2023-05-27 10:03:51.000000 logidrivepy-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 10:20:39.036074 logidrivepy-0.1.3/logidrivepy/
--rw-rw-rw-   0        0        0      196 2023-05-27 04:08:39.000000 logidrivepy-0.1.3/logidrivepy/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-05-27 03:38:07.000000 logidrivepy-0.1.3/logidrivepy/constants.py
--rw-rw-rw-   0        0        0      760 2023-05-27 09:04:30.000000 logidrivepy-0.1.3/logidrivepy/controller.py
--rw-rw-rw-   0        0        0    16701 2023-05-27 08:42:15.000000 logidrivepy-0.1.3/logidrivepy/functions.py
--rw-rw-rw-   0        0        0     1865 2023-05-27 03:39:18.000000 logidrivepy-0.1.3/logidrivepy/structs.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:20:39.058080 logidrivepy-0.1.3/logidrivepy.egg-info/
--rw-rw-rw-   0        0        0     3469 2023-05-27 10:20:38.000000 logidrivepy-0.1.3/logidrivepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-05-27 10:20:38.000000 logidrivepy-0.1.3/logidrivepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 10:20:38.000000 logidrivepy-0.1.3/logidrivepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-27 10:20:38.000000 logidrivepy-0.1.3/logidrivepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 10:20:39.069082 logidrivepy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      957 2023-05-27 10:19:36.000000 logidrivepy-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:20:39.065081 logidrivepy-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2023-05-23 21:56:36.000000 logidrivepy-0.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0      743 2023-05-27 09:01:48.000000 logidrivepy-0.1.3/tests/run_controller_test.py
--rw-rw-rw-   0        0        0      585 2023-05-27 09:26:43.000000 logidrivepy-0.1.3/tests/spin_wheel_test.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:19:33.154628 logidrivepy-0.2.0/
+-rw-rw-rw-   0        0        0     1087 2023-05-23 22:21:13.000000 logidrivepy-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4873 2023-06-04 11:19:33.151627 logidrivepy-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4168 2023-06-04 11:15:14.000000 logidrivepy-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 11:19:33.100616 logidrivepy-0.2.0/logidrivepy/
+-rw-rw-rw-   0        0        0      196 2023-05-27 04:08:39.000000 logidrivepy-0.2.0/logidrivepy/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-05-27 03:38:07.000000 logidrivepy-0.2.0/logidrivepy/constants.py
+-rw-rw-rw-   0        0        0      760 2023-05-27 09:04:30.000000 logidrivepy-0.2.0/logidrivepy/controller.py
+-rw-rw-rw-   0        0        0    38374 2023-06-04 10:22:13.000000 logidrivepy-0.2.0/logidrivepy/functions.py
+-rw-rw-rw-   0        0        0     1865 2023-05-27 03:39:18.000000 logidrivepy-0.2.0/logidrivepy/structs.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:19:33.133624 logidrivepy-0.2.0/logidrivepy.egg-info/
+-rw-rw-rw-   0        0        0     4873 2023-06-04 11:19:32.000000 logidrivepy-0.2.0/logidrivepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-06-04 11:19:32.000000 logidrivepy-0.2.0/logidrivepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 11:19:32.000000 logidrivepy-0.2.0/logidrivepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-04 11:19:32.000000 logidrivepy-0.2.0/logidrivepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 11:19:33.154628 logidrivepy-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      963 2023-06-04 11:17:40.000000 logidrivepy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:19:33.148627 logidrivepy-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-23 21:56:36.000000 logidrivepy-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-06-04 08:55:18.000000 logidrivepy-0.2.0/tests/run_controller_test.py
+-rw-rw-rw-   0        0        0      585 2023-05-27 09:26:43.000000 logidrivepy-0.2.0/tests/spin_wheel_test.py
```

### Comparing `logidrivepy-0.1.3/LICENSE.txt` & `logidrivepy-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.3/PKG-INFO` & `logidrivepy-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,68 @@
 Metadata-Version: 2.1
 Name: logidrivepy
-Version: 0.1.3
-Summary: A Python library for interfacing with a Logitech steering wheel.
+Version: 0.2.0
+Summary: A Python module for interfacing with Logitech steering wheels.
 Home-page: https://github.com/cengizozel/logidrivepy
 Author: Cengiz Ozel
 Author-email: cozel@cs.rochester.edu
 License: MIT
-Keywords: logitech,g920,driving,wheel,controller
+Keywords: logitech,g920,driving,steering-wheel,controller
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # LogiDrivePy - Logitech Controller Python Module
 
-A Python module for interfacing with a Logitech steering wheel. This module was tested on a Logitech G920 Driving Force Racing Wheel.
+A Python module for interfacing with Logitech steering wheels. This module was tested with the Logitech G920 Driving Force Racing Wheel but should work with other Logitech devices as specified in the [Supported Devices](#supported-devices) section.
 
 ## Introduction
 
-This Python module facilitates interaction with the Logitech G920 Driving Force Racing Wheel, serving as a bridge between Python and the Logitech Steering Wheel's software components.
+This Python module facilitates interaction with Logitech steering wheels, serving as a bridge between Python and the Logitech Steering Wheel's software components.
 
-The original functionality was provided in the form of a C# implementation as part of the Logitech Steering Wheel SDK (Software Development Kit) for the Unity Game Engine, designed by Logitech's developers. The SDK includes APIs (Application Programming Interfaces), which are sets of protocols and tools that allow developers to interact with Logitech's steering wheel hardware.
+The original functionality was provided in the form of a C# implementation as part of the [Logitech Steering Wheel SDK](https://www.logitechg.com/en-us/innovation/developer-lab.html) for the [Unity Game Engine](https://assetstore.unity.com/packages/tools/integration/logitech-gaming-sdk-6630). The SDK allows developers to easily add Logitech steering wheel support to their games, using a set of predefined force feedback effects or creating custom effects by defining specific forces.
 
-Seeing the potential to extend this functionality to the Python community, this module was developed to enable the same capabilities for Python developers. By utilizing the `ctypes` Python library, the module can load and call functions from Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll), effectively enabling Python scripts to control and interact with the Logitech G920 Driving Force Racing Wheel.
+With the aim to extend these capabilities to the Python community, this module was developed as an accessible tool for Python developers. Utilizing the `ctypes` Python library, the module enables Python scripts to load and interact with Logitech steering wheels through Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll), providing a seamless integration experience for developers working with these devices.
+
+## Supported Devices
+
+This library was tested with the Logitech G920 Driving Force Racing Wheel, but according to Logitech documentation, it should also work with the following devices:
+
+### Logitech
+- G29
+- G920
+- Driving Force GT
+- G27
+- G25
+- Driving Force Pro
+- MOMO Force
+- MOMO Racing
+- Formula Force GP
+- Driving Force
+- Formula Force
+- Force 3D
+- Strike Force 3D
+- Freedom 2.4 Cordless Joystick
+- Cordless Rumblepad
+- Cordless Rumblepad 2
+- Rumblepad
+
+### Microsoft
+- Sidewinder Force Feedback 2 (Stick)
+- Sidewinder Force (Wheel)
+
+### Other (with Immersion drivers)
+- Saitek Cyborg 3D Force
+- Act-Labs Force RS Wheel
 
 ## Installation
 
 To install the package, simply use pip:
 ```
 pip install logidrivepy
 ```
@@ -78,12 +109,14 @@
 
 ## Dependencies
 
 This library uses the `ctypes` Python library to load and call functions from the Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll). The ctypes library is part of the standard Python library and should be installed by default with a standard Python installation.
 
 This library also requires `Tkinter`, a Python binding to the Tk GUI toolkit. Tkinter is part of the standard Python library for Python 3 and should be installed by default with a standard Python installation.
 
-### License
+## License
 
 This project is licensed under the terms of the MIT license. For more details, see the `LICENSE.txt` file.
 
+Please note that this project is **not** a reverse engineering of the Logitech Gaming Steering Wheel SDK. Instead, this project aims to provide an interface to Logitech steering wheels in Python by utilizing the SDK's provided DLL file (LogitechSteeringWheelEnginesWrapper.dll) without decompiling, disassembling, or otherwise altering the SDK's components. This project is designed to extend the functionality of the SDK for Python developers while respecting and complying with the original End-User License Agreement of the SDK.
+
```

### Comparing `logidrivepy-0.1.3/logidrivepy/constants.py` & `logidrivepy-0.2.0/logidrivepy/constants.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.3/logidrivepy/controller.py` & `logidrivepy-0.2.0/logidrivepy/controller.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.3/logidrivepy/structs.py` & `logidrivepy-0.2.0/logidrivepy/structs.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.3/logidrivepy.egg-info/PKG-INFO` & `logidrivepy-0.2.0/logidrivepy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,68 @@
 Metadata-Version: 2.1
 Name: logidrivepy
-Version: 0.1.3
-Summary: A Python library for interfacing with a Logitech steering wheel.
+Version: 0.2.0
+Summary: A Python module for interfacing with Logitech steering wheels.
 Home-page: https://github.com/cengizozel/logidrivepy
 Author: Cengiz Ozel
 Author-email: cozel@cs.rochester.edu
 License: MIT
-Keywords: logitech,g920,driving,wheel,controller
+Keywords: logitech,g920,driving,steering-wheel,controller
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # LogiDrivePy - Logitech Controller Python Module
 
-A Python module for interfacing with a Logitech steering wheel. This module was tested on a Logitech G920 Driving Force Racing Wheel.
+A Python module for interfacing with Logitech steering wheels. This module was tested with the Logitech G920 Driving Force Racing Wheel but should work with other Logitech devices as specified in the [Supported Devices](#supported-devices) section.
 
 ## Introduction
 
-This Python module facilitates interaction with the Logitech G920 Driving Force Racing Wheel, serving as a bridge between Python and the Logitech Steering Wheel's software components.
+This Python module facilitates interaction with Logitech steering wheels, serving as a bridge between Python and the Logitech Steering Wheel's software components.
 
-The original functionality was provided in the form of a C# implementation as part of the Logitech Steering Wheel SDK (Software Development Kit) for the Unity Game Engine, designed by Logitech's developers. The SDK includes APIs (Application Programming Interfaces), which are sets of protocols and tools that allow developers to interact with Logitech's steering wheel hardware.
+The original functionality was provided in the form of a C# implementation as part of the [Logitech Steering Wheel SDK](https://www.logitechg.com/en-us/innovation/developer-lab.html) for the [Unity Game Engine](https://assetstore.unity.com/packages/tools/integration/logitech-gaming-sdk-6630). The SDK allows developers to easily add Logitech steering wheel support to their games, using a set of predefined force feedback effects or creating custom effects by defining specific forces.
 
-Seeing the potential to extend this functionality to the Python community, this module was developed to enable the same capabilities for Python developers. By utilizing the `ctypes` Python library, the module can load and call functions from Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll), effectively enabling Python scripts to control and interact with the Logitech G920 Driving Force Racing Wheel.
+With the aim to extend these capabilities to the Python community, this module was developed as an accessible tool for Python developers. Utilizing the `ctypes` Python library, the module enables Python scripts to load and interact with Logitech steering wheels through Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll), providing a seamless integration experience for developers working with these devices.
+
+## Supported Devices
+
+This library was tested with the Logitech G920 Driving Force Racing Wheel, but according to Logitech documentation, it should also work with the following devices:
+
+### Logitech
+- G29
+- G920
+- Driving Force GT
+- G27
+- G25
+- Driving Force Pro
+- MOMO Force
+- MOMO Racing
+- Formula Force GP
+- Driving Force
+- Formula Force
+- Force 3D
+- Strike Force 3D
+- Freedom 2.4 Cordless Joystick
+- Cordless Rumblepad
+- Cordless Rumblepad 2
+- Rumblepad
+
+### Microsoft
+- Sidewinder Force Feedback 2 (Stick)
+- Sidewinder Force (Wheel)
+
+### Other (with Immersion drivers)
+- Saitek Cyborg 3D Force
+- Act-Labs Force RS Wheel
 
 ## Installation
 
 To install the package, simply use pip:
 ```
 pip install logidrivepy
 ```
@@ -78,12 +109,14 @@
 
 ## Dependencies
 
 This library uses the `ctypes` Python library to load and call functions from the Logitech's DLL (LogitechSteeringWheelEnginesWrapper.dll). The ctypes library is part of the standard Python library and should be installed by default with a standard Python installation.
 
 This library also requires `Tkinter`, a Python binding to the Tk GUI toolkit. Tkinter is part of the standard Python library for Python 3 and should be installed by default with a standard Python installation.
 
-### License
+## License
 
 This project is licensed under the terms of the MIT license. For more details, see the `LICENSE.txt` file.
 
+Please note that this project is **not** a reverse engineering of the Logitech Gaming Steering Wheel SDK. Instead, this project aims to provide an interface to Logitech steering wheels in Python by utilizing the SDK's provided DLL file (LogitechSteeringWheelEnginesWrapper.dll) without decompiling, disassembling, or otherwise altering the SDK's components. This project is designed to extend the functionality of the SDK for Python developers while respecting and complying with the original End-User License Agreement of the SDK.
+
```

### Comparing `logidrivepy-0.1.3/setup.py` & `logidrivepy-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='logidrivepy',
-    version='0.1.3',
-    description='A Python library for interfacing with a Logitech steering wheel.',
+    version='0.2.0',
+    description='A Python module for interfacing with Logitech steering wheels.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/cengizozel/logidrivepy',
     author='Cengiz Ozel',
     author_email='cozel@cs.rochester.edu',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     package_data={'logidrivepy': ['dll/*.dll']},
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
-    keywords='logitech, g920, driving, wheel, controller',
+    keywords='logitech, g920, driving, steering-wheel, controller',
     install_requires=[
     ],
 )
```

### Comparing `logidrivepy-0.1.3/tests/run_controller_test.py` & `logidrivepy-0.2.0/tests/run_controller_test.py`

 * *Files identical despite different names*

### Comparing `logidrivepy-0.1.3/tests/spin_wheel_test.py` & `logidrivepy-0.2.0/tests/spin_wheel_test.py`

 * *Files identical despite different names*

