# Comparing `tmp/prefab-0.2.6.tar.gz` & `tmp/prefab-0.3.0.tar.gz`

## Comparing `prefab-0.2.6.tar` & `prefab-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 prefab-0.2.6/.gitattributes
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 prefab-0.2.6/.pylintrc
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 prefab-0.2.6/requirements.txt
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 prefab-0.2.6/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 prefab-0.2.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    69100 2020-02-02 00:00:00.000000 prefab-0.2.6/assets/logo.png
--rw-r--r--   0        0        0    67819 2020-02-02 00:00:00.000000 prefab-0.2.6/assets/promo_c.png
--rw-r--r--   0        0        0    74174 2020-02-02 00:00:00.000000 prefab-0.2.6/assets/promo_p.png
--rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/circles-inverse_512x512.png
--rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/circles_512x512.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross-inverse_16x128_256x256.png
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross-inverse_32x128_256x256.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross-inverse_64x128_256x256.png
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross_16x128_256x256.png
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross_32x128_256x256.png
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/cross_64x128_256x256.png
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/devices.gds
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_16x256_16_512x512.png
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_16x256_32_512x512.png
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_16x256_64_512x512.png
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_32x256_16_512x512.png
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_32x256_32_512x512.png
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_32x256_64_512x512.png
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_64x256_16_512x512.png
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_64x256_32_512x512.png
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/grating_64x256_64_512x512.png
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/pie_128x128_256x256.png
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/rectangle_128x128_256x256.png
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/ring_64x128_256x256.png
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 prefab-0.2.6/devices/star_128x128_256x256.png
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 prefab-0.2.6/docs/models.md
--rw-r--r--   0        0        0   232507 2020-02-02 00:00:00.000000 prefab-0.2.6/examples/example_prediction.ipynb
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 prefab-0.2.6/prefab/__init__.py
--rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 prefab-0.2.6/prefab/io.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 prefab-0.2.6/prefab/predictor.py
--rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 prefab-0.2.6/prefab/processor.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 prefab-0.2.6/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 prefab-0.2.6/LICENSE
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 prefab-0.2.6/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 prefab-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    35500 2020-02-02 00:00:00.000000 prefab-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 prefab-0.3.0/.gitattributes
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 prefab-0.3.0/.pylintrc
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 prefab-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 prefab-0.3.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 prefab-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    69100 2020-02-02 00:00:00.000000 prefab-0.3.0/assets/logo.png
+-rw-r--r--   0        0        0    67819 2020-02-02 00:00:00.000000 prefab-0.3.0/assets/promo_c.png
+-rw-r--r--   0        0        0    74174 2020-02-02 00:00:00.000000 prefab-0.3.0/assets/promo_p.png
+-rw-r--r--   0        0        0    13192 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/circles-inverse_512x512.png
+-rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/circles_512x512.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/cross-inverse_16x128_256x256.png
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/cross-inverse_32x128_256x256.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/cross-inverse_64x128_256x256.png
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/cross_16x128_256x256.png
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/cross_32x128_256x256.png
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/cross_64x128_256x256.png
+-rw-r--r--   0        0        0    87251 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/demux.png
+-rw-r--r--   0        0        0    12364 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/devices.gds
+-rw-r--r--   0        0        0   257418 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/fleur.png
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/grating_16x256_16_512x512.png
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/grating_16x256_32_512x512.png
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/grating_16x256_64_512x512.png
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/grating_32x256_16_512x512.png
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/grating_32x256_32_512x512.png
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/grating_32x256_64_512x512.png
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/grating_64x256_16_512x512.png
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/grating_64x256_32_512x512.png
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/grating_64x256_64_512x512.png
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/pie_128x128_256x256.png
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/rectangle_128x128_256x256.png
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/ring_64x128_256x256.png
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 prefab-0.3.0/devices/star_128x128_256x256.png
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 prefab-0.3.0/docs/models.md
+-rw-r--r--   0        0        0   233020 2020-02-02 00:00:00.000000 prefab-0.3.0/examples/1_prediction.ipynb
+-rw-r--r--   0        0        0   145408 2020-02-02 00:00:00.000000 prefab-0.3.0/examples/2_prediction_gds.ipynb
+-rw-r--r--   0        0        0   278518 2020-02-02 00:00:00.000000 prefab-0.3.0/examples/3_correction.ipynb
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 prefab-0.3.0/prefab/__init__.py
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 prefab-0.3.0/prefab/io.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 prefab-0.3.0/prefab/predictor.py
+-rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 prefab-0.3.0/prefab/processor.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 prefab-0.3.0/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 prefab-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 prefab-0.3.0/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 prefab-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    34470 2020-02-02 00:00:00.000000 prefab-0.3.0/PKG-INFO
```

### Comparing `prefab-0.2.6/.github/workflows/python-publish.yml` & `prefab-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/assets/logo.png` & `prefab-0.3.0/assets/logo.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/assets/promo_c.png` & `prefab-0.3.0/assets/promo_c.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/assets/promo_p.png` & `prefab-0.3.0/assets/promo_p.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/circles-inverse_512x512.png` & `prefab-0.3.0/devices/circles-inverse_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/circles_512x512.png` & `prefab-0.3.0/devices/circles_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/cross-inverse_16x128_256x256.png` & `prefab-0.3.0/devices/cross-inverse_16x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/cross-inverse_32x128_256x256.png` & `prefab-0.3.0/devices/cross-inverse_32x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/cross-inverse_64x128_256x256.png` & `prefab-0.3.0/devices/cross-inverse_64x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/cross_16x128_256x256.png` & `prefab-0.3.0/devices/cross_16x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/cross_32x128_256x256.png` & `prefab-0.3.0/devices/cross_32x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/cross_64x128_256x256.png` & `prefab-0.3.0/devices/cross_64x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/grating_16x256_16_512x512.png` & `prefab-0.3.0/devices/grating_16x256_16_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/grating_16x256_32_512x512.png` & `prefab-0.3.0/devices/grating_16x256_32_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/grating_16x256_64_512x512.png` & `prefab-0.3.0/devices/grating_16x256_64_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/grating_32x256_16_512x512.png` & `prefab-0.3.0/devices/grating_32x256_16_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/grating_32x256_32_512x512.png` & `prefab-0.3.0/devices/grating_32x256_32_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/grating_32x256_64_512x512.png` & `prefab-0.3.0/devices/grating_32x256_64_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/grating_64x256_16_512x512.png` & `prefab-0.3.0/devices/grating_64x256_16_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/grating_64x256_32_512x512.png` & `prefab-0.3.0/devices/grating_64x256_32_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/grating_64x256_64_512x512.png` & `prefab-0.3.0/devices/grating_64x256_64_512x512.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/pie_128x128_256x256.png` & `prefab-0.3.0/devices/pie_128x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/rectangle_128x128_256x256.png` & `prefab-0.3.0/devices/rectangle_128x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/ring_64x128_256x256.png` & `prefab-0.3.0/devices/ring_64x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/devices/star_128x128_256x256.png` & `prefab-0.3.0/devices/star_128x128_256x256.png`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/prefab/predictor.py` & `prefab-0.3.0/prefab/predictor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,63 @@
-"""Makes predictions of fabrication variations in photonic devices using ML
-models on the cloud.
+"""
+A module for making predictions on fabrication variations in photonic devices 
+using machine learning models deployed in the cloud.
 """
 
 import base64
 import numpy as np
 import requests
 import cv2
-from prefab.processor import binarize
+from prefab.processor import binarize_hard
 
 
 def predict(device: np.ndarray, model_name: str, model_num: str,
-            binary: bool = False) -> np.ndarray:
-    """Makes a complete prediction of a device.
+            binarize: bool = False) -> np.ndarray:
+    """
+    Generates a prediction for a photonic device using a specified cloud-based ML model.
 
-    A prediction is made by sending an image of a device to a cloud
-    function that inferences the model. If the model is a corrector (i.e.,
-    self.model_type = 'c'), the result can be interpreted as a correction
-    instead.
-
-    Args:
-        device: A binary numpy matrix representing the shape of a device.
-        model_name: A string indicating the name of the model. See
-            documentation for names of available models.
-        model_num: A string indicating the number of the model. See
-            documentation for names of available models.
-        binary: A bool indicating if the prediction will be binarized.
-
-    Returns:
-        A numpy matrix representing the shape of a predicted device. Pixel
-        values closer to 1 indicate high core material likeliness, while
-        pixel values closer to 0 indicate high cladding material
-        likeliness. Inbetween pixel values indicate uncertainty in the
-        prediction.
+    The function sends an image of the device to a cloud function, which uses the specified 
+    machine learning model to generate a prediction. If the model is a corrector (i.e., 
+    the model type is 'c'), the result can be interpreted as a correction.
+
+    Parameters
+    ----------
+    device : np.ndarray
+        A binary numpy matrix representing the shape of a device.
+
+    model_name : str
+        The name of the ML model to use for the prediction. 
+        Consult the module's documentation for available models.
+
+    model_num : str
+        The version number of the ML model. 
+        Consult the module's documentation for available versions.
+
+    binarize : bool, optional
+        If set to True, the prediction will be binarized (default is False).
+
+    Returns
+    -------
+    np.ndarray
+        A numpy matrix representing the predicted shape of the device. Pixel values closer 
+        to 1 indicate a higher likelihood of core material, while pixel values closer to 0 
+        suggest a higher likelihood of cladding material. Pixel values in between represent 
+        prediction uncertainty.
     """
     function_url = 'https://prefab-photonics--predict.modal.run'
 
     device_img = cv2.imencode('.png', 255*device)[1].tobytes()
     device_img_base64 = base64.b64encode(device_img).decode('utf-8')
     predict_data = {'device': device_img_base64,
                     'model_name': model_name,
                     'model_num': model_num}
 
-    prediction_img_base64 = requests.post(function_url, json=predict_data,
-                                          timeout=200)
+    prediction_img_base64 = requests.post(function_url, json=predict_data, timeout=200)
 
     prediction_img_data = base64.b64decode(prediction_img_base64.json())
     prediction_img = np.frombuffer(prediction_img_data, np.uint8)
-    prediction = cv2.imdecode(prediction_img, 0)/255
+    prediction = cv2.imdecode(prediction_img, 0) / 255
 
-    if binary:
-        prediction = binarize(prediction)
+    if binarize:
+        prediction = binarize_hard(prediction)
 
     return prediction
```

### Comparing `prefab-0.2.6/LICENSE` & `prefab-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefab-0.2.6/pyproject.toml` & `prefab-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "prefab"
-version = "0.2.6"
+version = "0.3.0"
 authors = [
     {name = "Dusan Gostimirovic", email="dusan@prefabphotonics.com"},
 ]
 keywords = ["photonics", "nanofabrication", "machine learning", "layout"]
 description = "Machine learning based prediction of photonic device fabrication"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `prefab-0.2.6/PKG-INFO` & `prefab-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefab
-Version: 0.2.6
+Version: 0.3.0
 Summary: Machine learning based prediction of photonic device fabrication
 Project-URL: Homepage, https://github.com/PreFab-Photonics/PreFab
 Author-email: Dusan Gostimirovic <dusan@prefabphotonics.com>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
@@ -521,77 +521,71 @@
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # PreFab
 
 ![PreFab logo](https://github.com/PreFab-Photonics/PreFab/blob/main/assets/logo.png?raw=true)
 
-`PreFab` models fabrication process induced structural variations in integrated photonic devices using **deep learning**. New insights into the capabilities of nanofabrication processes are uncovered and device design fidelity is enhanced in this *virtual nanofabrication environment*.
+`PreFab` leverages **deep learning** to model fabrication-induced structural variations in integrated photonic devices. Through this *virtual nanofabrication environment*, we uncover valuable insights into nanofabrication processes and enhance device design accuracy.
 
 ## Prediction
 
-`PreFab` predicts process-induced structural variations such as corner rounding (both over and under etching), washing away of small lines and islands, and filling of narrow holes and channels in planar photonic devices. The designer then resimulates their (predicted) design to rapidly prototype the expected performance and make any necessary corrections prior to nanofabrication.
+`PreFab` accurately predicts process-induced structural alterations such as corner rounding, washing away of small lines and islands, and filling of narrow holes in planar photonic devices. This enables designers to quickly prototype expected performance and rectify designs prior to nanofabrication.
 
-![Example of PreFab prediction](https://github.com/PreFab-Photonics/PreFab/blob/main/assets/promo_p.png?raw=true) *Predicted fabrication variation of a star structure on a silicon-on-insulator e-beam lithography process.*
+![Example of PreFab prediction](https://github.com/PreFab-Photonics/PreFab/blob/main/assets/promo_p.png?raw=true)
 
 ## Correction
 
-`PreFab` also makes automatic corrections to device designs so that the fabricated outcome is closer to the nominal design. Less structural variation generally means less performance degradation from simulation to experiment.
+`PreFab` automates corrections to device designs, ensuring the fabricated outcome aligns with the original design. This results in reduced structural variation and performance disparity from simulation to experiment.
 
-![Example of PreFab correction](https://github.com/PreFab-Photonics/PreFab/blob/main/assets/promo_c.png?raw=true) *Corrected fabrication of a star structure on a silicon-on-insulator e-beam lithography process.*
+![Example of PreFab correction](https://github.com/PreFab-Photonics/PreFab/blob/main/assets/promo_c.png?raw=true)
 
 ## Models
 
-Each photonic foundry requires its own *predictor* and *corrector* models. These models are updated regularly based on data from recent fabrication runs. The following models are currently available (see full list on [`docs/models.md`](docs/models.md)):
+`PreFab` accommodates unique *predictor* and *corrector* models for each photonic foundry, regularly updated based on recent fabrication data. Current models include (see full list on [`docs/models.md`](docs/models.md)):
 
 | Foundry | Process | Latest Version | Latest Dataset | Type | Full Name | Status | Usage |
 | ------- | ------- | -------------- | -------------- | ---- | --------- |------- | ----- |
 | ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v5 (Jun 3 2023) | v4 (Apr 12 2023) | Predictor | p_ANT_NanoSOI_v5_d4 | Beta | Open |
 | ANT | [NanoSOI](https://www.appliednt.com/nanosoi-fabrication-service/) | v5 (Jun 3 2023) | v4 (Apr 12 2023) | Corrector | c_ANT_NanoSOI_v5_d4 | Beta | Open |
 
-*This list will update over time. Usage is subject to change. Please contact us or create an issue if you would like to see a new foundry and process modelled.*
+*New models and foundries are regularly added. Usage may change. For additional foundry and process models, feel free to contact us or raise an issue.*
 
 ## Installation
 
 ### Local
 
-Install the latest version of `PreFab` locally using:
+Install `PreFab` via pip:
 
 ```sh
 pip install prefab
 ```
 
-Alternatively, you can clone this repository and then install in development mode using:
+Or clone the repository and install in development mode:
 
 ```sh
 git clone https://github.com/PreFab-Photonics/PreFab.git
 cd PreFab
 pip install -e .
 ```
 
-This will allow any changes made to the source code to be reflected in your Python module.
-
 ### Online
 
-You can also run the latest version of `PreFab` online by following:
+Use `PreFab` online through GitHub Codespaces:
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?machine=basicLinux32gb&repo=608330448&ref=main&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=EastUs)
 
 ## Getting Started
 
-Please see the notebooks in [`/examples`](https://github.com/PreFab-Photonics/PreFab/tree/main/examples) to get started with making predictions.
+Visit [`/examples`](https://github.com/PreFab-Photonics/PreFab/tree/main/examples) for usage notebooks.
 
 ## Performance and Usage
 
-Currently, `PreFab` models are accessed through a serverless cloud platform that has the following limitations to keep in mind:
-
-- 🐢 Inferencing is done on a CPU and will thus be relatively slow. GPU inferencing to come in future updates.
-- 🥶 The first prediction may be slow, as the cloud server may have to perform a cold start and load the necessary model(s). After the first prediction, the server will be "hot" for some time and the subsequent predictions will be much quicker.
-- 😊 Please be mindful of your usage. Start with small examples before scaling up to larger device designs, and please keep usage down to a reasonable amount in these early stages. Thank you!
-
-<!-- ## Documentation
+`PreFab` models are served via a serverless cloud platform. Please note:
 
-To get started with tutorials and examples, or to dive into the API reference, visit our full documentation [here](README.md). -->
+- 🐢 CPU inferencing may result in slower performance. Future updates will introduce GPU inferencing.
+- 🥶 The first prediction may take longer due to cold start server loading. Subsequent predictions will be faster.
+- 😊 Be considerate of usage. Start small and limit usage during the initial stages. Thank you!
 
 ## License
 
-This project is licensed under the terms of the LGPL-2.1 license. © 2023 PreFab Photonics.
+This project is licensed under the LGPL-2.1 license. © 2023 PreFab Photonics.
```

