# Comparing `tmp/image_frequency_analysis-0.2.4.tar.gz` & `tmp/image_frequency_analysis-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_frequency_analysis-0.2.4.tar", last modified: Wed May 17 14:15:40 2023, max compression
+gzip compressed data, was "image_frequency_analysis-0.2.5.tar", max compression
```

## Comparing `image_frequency_analysis-0.2.4.tar` & `image_frequency_analysis-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 14:15:40.196978 image_frequency_analysis-0.2.4/
--rw-rw-rw-   0        0        0     1086 2023-04-15 11:42:59.000000 image_frequency_analysis-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     1495 2023-05-17 14:15:40.195845 image_frequency_analysis-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1209 2023-05-17 14:11:55.000000 image_frequency_analysis-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 14:15:40.174733 image_frequency_analysis-0.2.4/image_frequency_analysis/
--rw-rw-rw-   0        0        0       92 2023-05-10 12:59:14.000000 image_frequency_analysis-0.2.4/image_frequency_analysis/__init__.py
--rw-rw-rw-   0        0        0     6520 2023-05-17 14:13:41.000000 image_frequency_analysis-0.2.4/image_frequency_analysis/frequency_analysis.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:15:40.191848 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/
--rw-rw-rw-   0        0        0     1495 2023-05-17 14:15:39.000000 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-05-17 14:15:39.000000 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 14:15:39.000000 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-17 14:15:39.000000 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-17 14:15:39.000000 image_frequency_analysis-0.2.4/image_frequency_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 14:15:40.198003 image_frequency_analysis-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      562 2023-05-17 14:13:41.000000 image_frequency_analysis-0.2.4/setup.py
+-rw-r--r--   0        0        0     1065 2023-06-04 11:25:19.929417 image_frequency_analysis-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1854 2023-06-04 11:25:19.929417 image_frequency_analysis-0.2.5/README.md
+-rw-r--r--   0        0        0       87 2023-06-04 11:25:19.929417 image_frequency_analysis-0.2.5/image_frequency_analysis/__init__.py
+-rw-r--r--   0        0        0     6317 2023-06-04 11:25:19.929417 image_frequency_analysis-0.2.5/image_frequency_analysis/frequency_analysis.py
+-rw-r--r--   0        0        0      890 2023-06-04 11:25:19.929417 image_frequency_analysis-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 image_frequency_analysis-0.2.5/PKG-INFO
```

### Comparing `image_frequency_analysis-0.2.4/PKG-INFO` & `image_frequency_analysis-0.2.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,52 @@
-Metadata-Version: 2.1
-Name: image_frequency_analysis
-Version: 0.2.4
-Summary: A package to perform image frequency analysis using the Fourier Transform method
-Author: M Thivagar
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Image Frequency Analysis
-
-This package is build to combine all the steps that are done as part of the
-frequency analysis using the Fourier transform approach.
-
-
-
-## Install the Package
-You can install the package using the pip command
-
-`!pip install image_frequency_analysis` - when installing through jupyter notebook
-
-`pip install image_frequency_analysis` - when installing through a command prompt
-
-
-## Using the package
-Once you have installed you can use the package by importing the image_frequency_analysis method from the package
-
-` import image_frequency_analysis as ifa `
-
-You can then pass the image path to the function which is a required argument, to get the plot 
-of comparison between the original image and the filtered image
-
-**Example:**
-
-` ifa.FrequencyAnalysis('sandstone.tif') `
-
-By default the package uses the high pass filter to perform the filtering of the image. This option can be overridden using
-the optional parameters that can be sent to the function.
-
-You can find the various optional parameters and their usage in the package using the help command.
-
-` help(ifa.FrequencyAnalysis) ` or looking through the docstring directly in the IDE
-
+<div align="center">
+
+<h1> Image Frequency Analysis </h1>
+  
+[![PyPI version](https://badge.fury.io/py/image-frequency-analysis.svg)](https://pypi.org/project/image-frequency-analysis/)
+[![PyPI stats](https://img.shields.io/pypi/dm/image-frequency-analysis.svg)](https://pypistats.org/packages/image-frequency-analysis)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/image-frequency-analysis.svg)](https://pypi.org/project/image-frequency-analysis/)
+
+</div>
+
+This package is build to combine all the steps that are done as part of the
+frequency analysis using the Fourier transform approach.
+
+
+
+## Install the Package
+You can install the package using the pip command
+
+`!pip install image_frequency_analysis` - when installing through jupyter notebook
+
+`pip install image_frequency_analysis` - when installing through a command prompt
+
+
+## Using the package
+Once you have installed you can use the package by importing the image_frequency_analysis method from the package
+
+` import image_frequency_analysis as ifa `
+
+You can then pass the image path to the function which is a required argument, to get the plot 
+of comparison between the original image and the filtered image
+
+**Example:**
+
+` ifa.FrequencyAnalysis('sandstone.tif') `
+
+By default the package uses the high pass filter to perform the filtering of the image. This option can be overridden using
+the optional parameters that can be sent to the function.
+
+You can find the various optional parameters and their usage in the package using the help command.
+
+` help(ifa.FrequencyAnalysis) ` or looking through the docstring directly in the IDE
+
+## Sample Output
+
+**Output with default parameters**
+
+![Default Parameter Output](sampleOutput/Default_Param_Image.jpg)
+
+
+**Output with Modified Parameters**
+
+![Modified_Parameter_Output](sampleOutput/Parameterised_Image.jpg)
```

### Comparing `image_frequency_analysis-0.2.4/image_frequency_analysis/frequency_analysis.py` & `image_frequency_analysis-0.2.5/image_frequency_analysis/frequency_analysis.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-import cv2
-import numpy as np
-import matplotlib.pyplot as plt
-import os
-
-
-class FrequencyAnalysis:
-    """
-    This definition invokes the Frequency Analysis class
-    to apply the Transformation on the image based on the
-    attributes passed to the class
-
-    Attributes:
-
-    image_path - This is the file path for the image on which the transformation needs to be applied
-
-    filter_radius - This property defines to what extent the low or high frequency value needs to be allowed to
-                    pass through in the filtering process. Default value = 80
-
-    high_pass_filter - This is a boolean value which indicates to use the default high pass filter mask on the image.
-                    Default value = False
-
-    low_pass_filter - This is a boolean value which indicates to use the default low pass filter mask on the image.
-                    Default value = False
-
-    When both the high_pass_filter and low_pass_filter is False, by default high pass filter mask is applied on the image.
-
-    Throws value error when both high_pass_filter and low_pass_filter value are set to be True.
-
-    """
-    def __init__(
-        self,
-        image_path,
-        filter_radius=80,
-        high_pass_filter=False,
-        low_pass_filter=False,
-    ):
-        self.mask_area = None
-        self.fft_image = None
-        self.dft_image = None
-        self.column_center = None
-        self.row_center = None
-        self.rows = None
-        self.columns = None
-        self.image_path = image_path
-        self.radius = filter_radius
-        self.high_pass_filter = high_pass_filter
-        self.low_pass_filter = low_pass_filter
-        self.image = self.load_image(self.image_path)
-
-        self.perform_image_frequency_analysis()
-
-    """
-    Definition to load the image into the
-    image object which will be used for further
-    processing
-    """
-
-    def load_image(self, image_path):
-        if os.path.exists(self.image_path):
-            return cv2.imread(f"{image_path}", 0)
-        else:
-            raise FileNotFoundError(f"File not found: {image_path}")
-
-    """
-    Definition to find the discrete fourier
-    transform value for the given image
-    """
-
-    def calculate_dft_of_image(self):
-        self.dft_image = cv2.dft(np.float32(self.image), flags=cv2.DFT_COMPLEX_OUTPUT)
-
-    """
-    Definition to perform the frequency shifting
-    inorder to migrate the low frequency values to 
-    the center and the high frequency values to the 
-    edges
-    """
-
-    def perform_frequency_shifting(self):
-        self.fft_image = np.fft.fftshift(self.dft_image)
-
-    """
-    To visualize the frequency shifted value
-    of the image
-    """
-
-    def get_magnitude_spectrum(self):
-        return 20 * np.log(
-            cv2.magnitude(self.fft_image[:, :, 0], self.fft_image[:, :, 1])
-        )
-
-    """
-    To get the rows and column information about the
-    image matrix
-    """
-
-    def set_rows_columns_details(self):
-        self.rows, self.columns = self.image.shape
-
-        self.row_center, self.column_center = int(self.rows / 2), int(self.columns / 2)
-
-    """
-    To get the high pass filter mask
-    """
-
-    def get_high_pass_filter_mask_matrix(self):
-        return np.ones((self.rows, self.columns, 2), np.uint8)
-
-    """
-    To get the low pass filter mask
-    """
-
-    def get_low_pass_filter_mask_matrix(self):
-        return np.zeros((self.rows, self.columns, 2), np.uint8)
-
-    """
-    To calculate the mask area based on the 
-    the rows and column information of the image
-    """
-
-    def calculate_mask_area(self):
-        center = [self.row_center, self.column_center]
-        x_value, y_value = np.ogrid[: self.rows, : self.columns]
-
-        self.mask_area = (x_value - center[0]) ** 2 + (y_value - center[1]) ** 2 <= (
-            self.radius * self.radius
-        )
-
-    def plot_graph(self, frequency_shift_magnitude, image):
-        plt.figure(figsize=(20, 10))
-
-        plt.subplot(1, 3, 1)
-        plt.title("Original Image")
-        plt.imshow(self.image, cmap="gray")
-
-        plt.subplot(1, 3, 2)
-        plt.title("Frequency Shifted Mask")
-        plt.imshow(frequency_shift_magnitude, cmap="gray")
-
-        plt.subplot(1, 3, 3)
-        filter_type = "Low Pass filter" if self.low_pass_filter else "High Pass Filter"
-        plt.title(f"Image post applying the {filter_type} mask")
-        plt.imshow(image, cmap="gray")
-
-    def perform_filtering_and_inverse_transform(self, mask):
-        frequency_shift = self.fft_image * mask
-
-        frequency_mask_magnitude = 20 * np.log(
-            cv2.magnitude(frequency_shift[:, :, 0], frequency_shift[:, :, 1]) + 1
-        )
-
-        frequency_shift_inverse = np.fft.ifftshift(frequency_shift)
-
-        inverse_discrete_transform = cv2.idft(frequency_shift_inverse)
-
-        original_image = cv2.magnitude(
-            inverse_discrete_transform[:, :, 0], inverse_discrete_transform[:, :, 1]
-        )
-
-        self.plot_graph(frequency_mask_magnitude, original_image)
-
-        return original_image
-
-    def perform_high_pass_filter_analysis(self):
-        hpf_mask = self.get_high_pass_filter_mask_matrix()
-        hpf_mask[self.mask_area] = 0
-
-        return self.perform_filtering_and_inverse_transform(hpf_mask)
-
-    def perform_low_pass_filter_analysis(self):
-        lpf_mask = self.get_low_pass_filter_mask_matrix()
-        lpf_mask[self.mask_area] = 1
-
-        return self.perform_filtering_and_inverse_transform(lpf_mask)
-
-    def perform_image_frequency_analysis(self):
-        if self.high_pass_filter and self.low_pass_filter:
-            raise ValueError(
-                        "Both high_pass_filter and low_pass_filter flag cannot be True. Please choose only one type "
-                        "of filter"
-                    )
-
-        if not self.high_pass_filter and not self.low_pass_filter:
-            self.high_pass_filter = True
-
-        self.calculate_dft_of_image()
-
-        self.perform_frequency_shifting()
-
-        self.set_rows_columns_details()
-
-        self.calculate_mask_area()
-
-        if self.high_pass_filter:
-            final_image = self.perform_high_pass_filter_analysis()
-        else:
-            final_image = self.perform_low_pass_filter_analysis()
-
-        final_image = (final_image / final_image.max() * 255).astype("uint8")
-
-        return final_image
-
+import cv2
+import numpy as np
+import matplotlib.pyplot as plt
+import os
+
+
+class FrequencyAnalysis:
+    """
+    This definition invokes the Frequency Analysis class
+    to apply the Transformation on the image based on the
+    attributes passed to the class
+
+    Attributes:
+
+    image_path - This is the file path for the image on which the transformation needs to be applied
+
+    filter_radius - This property defines to what extent the low or high frequency value needs to be allowed to
+                    pass through in the filtering process. Default value = 80
+
+    high_pass_filter - This is a boolean value which indicates to use the default high pass filter mask on the image.
+                    Default value = False
+
+    low_pass_filter - This is a boolean value which indicates to use the default low pass filter mask on the image.
+                    Default value = False
+
+    When both the high_pass_filter and low_pass_filter is False, by default high pass filter mask is applied on the image.
+
+    Throws value error when both high_pass_filter and low_pass_filter value are set to be True.
+
+    """
+    def __init__(
+        self,
+        image_path,
+        filter_radius=80,
+        high_pass_filter=False,
+        low_pass_filter=False,
+    ):
+        self.mask_area = None
+        self.fft_image = None
+        self.dft_image = None
+        self.column_center = None
+        self.row_center = None
+        self.rows = None
+        self.columns = None
+        self.image_path = image_path
+        self.radius = filter_radius
+        self.high_pass_filter = high_pass_filter
+        self.low_pass_filter = low_pass_filter
+        self.image = self.load_image(self.image_path)
+
+        self.perform_image_frequency_analysis()
+
+    """
+    Definition to load the image into the
+    image object which will be used for further
+    processing
+    """
+
+    def load_image(self, image_path):
+        if os.path.exists(self.image_path):
+            return cv2.imread(f"{image_path}", 0)
+        else:
+            raise FileNotFoundError(f"File not found: {image_path}")
+
+    """
+    Definition to find the discrete fourier
+    transform value for the given image
+    """
+
+    def calculate_dft_of_image(self):
+        self.dft_image = cv2.dft(np.float32(self.image), flags=cv2.DFT_COMPLEX_OUTPUT)
+
+    """
+    Definition to perform the frequency shifting
+    inorder to migrate the low frequency values to 
+    the center and the high frequency values to the 
+    edges
+    """
+
+    def perform_frequency_shifting(self):
+        self.fft_image = np.fft.fftshift(self.dft_image)
+
+    """
+    To visualize the frequency shifted value
+    of the image
+    """
+
+    def get_magnitude_spectrum(self):
+        return 20 * np.log(
+            cv2.magnitude(self.fft_image[:, :, 0], self.fft_image[:, :, 1])
+        )
+
+    """
+    To get the rows and column information about the
+    image matrix
+    """
+
+    def set_rows_columns_details(self):
+        self.rows, self.columns = self.image.shape
+
+        self.row_center, self.column_center = int(self.rows / 2), int(self.columns / 2)
+
+    """
+    To get the high pass filter mask
+    """
+
+    def get_high_pass_filter_mask_matrix(self):
+        return np.ones((self.rows, self.columns, 2), np.uint8)
+
+    """
+    To get the low pass filter mask
+    """
+
+    def get_low_pass_filter_mask_matrix(self):
+        return np.zeros((self.rows, self.columns, 2), np.uint8)
+
+    """
+    To calculate the mask area based on the 
+    the rows and column information of the image
+    """
+
+    def calculate_mask_area(self):
+        center = [self.row_center, self.column_center]
+        x_value, y_value = np.ogrid[: self.rows, : self.columns]
+
+        self.mask_area = (x_value - center[0]) ** 2 + (y_value - center[1]) ** 2 <= (
+            self.radius * self.radius
+        )
+
+    def plot_graph(self, frequency_shift_magnitude, image):
+        plt.figure(figsize=(20, 10))
+
+        plt.subplot(1, 3, 1)
+        plt.title("Original Image")
+        plt.imshow(self.image, cmap="gray")
+
+        plt.subplot(1, 3, 2)
+        plt.title("Frequency Shifted Mask")
+        plt.imshow(frequency_shift_magnitude, cmap="gray")
+
+        plt.subplot(1, 3, 3)
+        filter_type = "Low Pass filter" if self.low_pass_filter else "High Pass Filter"
+        plt.title(f"Image post applying the {filter_type} mask")
+        plt.imshow(image, cmap="gray")
+
+    def perform_filtering_and_inverse_transform(self, mask):
+        frequency_shift = self.fft_image * mask
+
+        frequency_mask_magnitude = 20 * np.log(
+            cv2.magnitude(frequency_shift[:, :, 0], frequency_shift[:, :, 1]) + 1
+        )
+
+        frequency_shift_inverse = np.fft.ifftshift(frequency_shift)
+
+        inverse_discrete_transform = cv2.idft(frequency_shift_inverse)
+
+        original_image = cv2.magnitude(
+            inverse_discrete_transform[:, :, 0], inverse_discrete_transform[:, :, 1]
+        )
+
+        self.plot_graph(frequency_mask_magnitude, original_image)
+
+        return original_image
+
+    def perform_high_pass_filter_analysis(self):
+        hpf_mask = self.get_high_pass_filter_mask_matrix()
+        hpf_mask[self.mask_area] = 0
+
+        return self.perform_filtering_and_inverse_transform(hpf_mask)
+
+    def perform_low_pass_filter_analysis(self):
+        lpf_mask = self.get_low_pass_filter_mask_matrix()
+        lpf_mask[self.mask_area] = 1
+
+        return self.perform_filtering_and_inverse_transform(lpf_mask)
+
+    def perform_image_frequency_analysis(self):
+        if self.high_pass_filter and self.low_pass_filter:
+            raise ValueError(
+                        "Both high_pass_filter and low_pass_filter flag cannot be True. Please choose only one type "
+                        "of filter"
+                    )
+
+        if not self.high_pass_filter and not self.low_pass_filter:
+            self.high_pass_filter = True
+
+        self.calculate_dft_of_image()
+
+        self.perform_frequency_shifting()
+
+        self.set_rows_columns_details()
+
+        self.calculate_mask_area()
+
+        if self.high_pass_filter:
+            final_image = self.perform_high_pass_filter_analysis()
+        else:
+            final_image = self.perform_low_pass_filter_analysis()
+
+        final_image = (final_image / final_image.max() * 255).astype("uint8")
+
+        return final_image
+
```

