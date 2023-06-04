# Comparing `tmp/presidio_image_redactor-0.0.46-py3-none-any.whl.zip` & `tmp/presidio_image_redactor-0.0.47-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 23475 bytes, number of entries: 17
--rw-r--r--  2.0 unx      784 b- defN 23-Jan-31 19:53 presidio_image_redactor/__init__.py
--rw-r--r--  2.0 unx     4970 b- defN 23-Jan-31 19:53 presidio_image_redactor/bbox.py
--rw-r--r--  2.0 unx     9991 b- defN 23-Jan-31 19:53 presidio_image_redactor/dicom_image_pii_verify_engine.py
--rw-r--r--  2.0 unx    32053 b- defN 23-Jan-31 19:53 presidio_image_redactor/dicom_image_redactor_engine.py
--rw-r--r--  2.0 unx     6921 b- defN 23-Jan-31 19:53 presidio_image_redactor/image_analyzer_engine.py
--rw-r--r--  2.0 unx     2470 b- defN 23-Jan-31 19:53 presidio_image_redactor/image_pii_verify_engine.py
--rw-r--r--  2.0 unx     1818 b- defN 23-Jan-31 19:53 presidio_image_redactor/image_redactor_engine.py
--rw-r--r--  2.0 unx      981 b- defN 23-Jan-31 19:53 presidio_image_redactor/ocr.py
--rw-r--r--  2.0 unx      615 b- defN 23-Jan-31 19:53 presidio_image_redactor/tesseract_ocr.py
--rw-r--r--  2.0 unx      216 b- defN 23-Jan-31 19:53 presidio_image_redactor/entities/__init__.py
--rw-r--r--  2.0 unx     2034 b- defN 23-Jan-31 19:53 presidio_image_redactor/entities/api_request_convertor.py
--rw-r--r--  2.0 unx     2106 b- defN 23-Jan-31 19:53 presidio_image_redactor/entities/image_recognizer_result.py
--rw-r--r--  2.0 unx      274 b- defN 23-Jan-31 19:53 presidio_image_redactor/entities/invalid_exception.py
--rw-r--r--  2.0 unx     6291 b- defN 23-Jan-31 19:53 presidio_image_redactor-0.0.46.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-31 19:53 presidio_image_redactor-0.0.46.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jan-31 19:53 presidio_image_redactor-0.0.46.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1708 b- defN 23-Jan-31 19:53 presidio_image_redactor-0.0.46.dist-info/RECORD
-17 files, 73348 bytes uncompressed, 20559 bytes compressed:  72.0%
+Zip file size: 23535 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-04 10:03 presidio_image_redactor/__init__.py
+-rw-r--r--  2.0 unx     4970 b- defN 23-Jun-04 10:03 presidio_image_redactor/bbox.py
+-rw-r--r--  2.0 unx    10224 b- defN 23-Jun-04 10:03 presidio_image_redactor/dicom_image_pii_verify_engine.py
+-rw-r--r--  2.0 unx    32055 b- defN 23-Jun-04 10:03 presidio_image_redactor/dicom_image_redactor_engine.py
+-rw-r--r--  2.0 unx     6921 b- defN 23-Jun-04 10:03 presidio_image_redactor/image_analyzer_engine.py
+-rw-r--r--  2.0 unx     2470 b- defN 23-Jun-04 10:03 presidio_image_redactor/image_pii_verify_engine.py
+-rw-r--r--  2.0 unx     1818 b- defN 23-Jun-04 10:03 presidio_image_redactor/image_redactor_engine.py
+-rw-r--r--  2.0 unx      981 b- defN 23-Jun-04 10:03 presidio_image_redactor/ocr.py
+-rw-r--r--  2.0 unx      615 b- defN 23-Jun-04 10:03 presidio_image_redactor/tesseract_ocr.py
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-04 10:03 presidio_image_redactor/entities/__init__.py
+-rw-r--r--  2.0 unx     2034 b- defN 23-Jun-04 10:03 presidio_image_redactor/entities/api_request_convertor.py
+-rw-r--r--  2.0 unx     2106 b- defN 23-Jun-04 10:03 presidio_image_redactor/entities/image_recognizer_result.py
+-rw-r--r--  2.0 unx      274 b- defN 23-Jun-04 10:03 presidio_image_redactor/entities/invalid_exception.py
+-rw-r--r--  2.0 unx     6342 b- defN 23-Jun-04 10:03 presidio_image_redactor-0.0.47.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 10:03 presidio_image_redactor-0.0.47.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-04 10:03 presidio_image_redactor-0.0.47.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1709 b- defN 23-Jun-04 10:03 presidio_image_redactor-0.0.47.dist-info/RECORD
+17 files, 73635 bytes uncompressed, 20619 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: presidio_image_redactor/entities/image_recognizer_result.py
 Comment: 
 
 Filename: presidio_image_redactor/entities/invalid_exception.py
 Comment: 
 
-Filename: presidio_image_redactor-0.0.46.dist-info/METADATA
+Filename: presidio_image_redactor-0.0.47.dist-info/METADATA
 Comment: 
 
-Filename: presidio_image_redactor-0.0.46.dist-info/WHEEL
+Filename: presidio_image_redactor-0.0.47.dist-info/WHEEL
 Comment: 
 
-Filename: presidio_image_redactor-0.0.46.dist-info/top_level.txt
+Filename: presidio_image_redactor-0.0.47.dist-info/top_level.txt
 Comment: 
 
-Filename: presidio_image_redactor-0.0.46.dist-info/RECORD
+Filename: presidio_image_redactor-0.0.47.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## presidio_image_redactor/dicom_image_pii_verify_engine.py

```diff
@@ -168,37 +168,41 @@
         """Handle when a word is detected multiple times as different types of entities.
 
         :param results: List of detected PHI with bbox info.
         :param dup_pix_tolerance: Pixel difference tolerance for identifying duplicates.
         :return: Detected PHI with no duplicate entities.
         """
         dups = []
-        results_no_dups = results.copy()
+        sorted(results, key=lambda x: x['score'], reverse=True)
+        results_no_dups = []
         dims = ["left", "top", "width", "height"]
 
         # Check for duplicates
         for i in range(len(results) - 1):
             i_dims = {dim: results[i][dim] for dim in dims}
 
             # Ignore if we've already detected this dup combination
             for other in range(i + 1, len(results)):
-                if i not in dups:
+                if i not in results_no_dups:
                     other_dims = {dim: results[other][dim] for dim in dims}
                     matching_dims = {
                         dim: abs(i_dims[dim] - other_dims[dim]) <= dup_pix_tolerance
                         for dim in dims
                     }
                     matching = list(matching_dims.values())
 
                     if all(matching):
-                        dups.append(other)
+                        lower_scored_index = other if \
+                            results[other]['score'] < results[i]['score'] else i
+                        dups.append(lower_scored_index)
 
         # Remove duplicates
-        for dup_index in sorted(dups, reverse=True):
-            del results_no_dups[dup_index]
+        for i in range(len(results)):
+            if i not in dups:
+                results_no_dups.append(results[i])
 
         return results_no_dups
 
     def _label_all_positives(
         self,
         gt_labels_dict: dict,
         ocr_results: List[dict],
@@ -231,15 +235,15 @@
             # If not, check back with OCR
             if not gt_match_found:
                 all_pos, _ = self.bbox_processor.match_with_source(
                     all_pos, ocr_results, analyzer_result, tolerance
                 )
 
         # Remove any duplicates
-        all_pos = self._remove_duplicate_entities(all_pos, 0)
+        all_pos = self._remove_duplicate_entities(all_pos)
 
         return all_pos
 
     @staticmethod
     def calculate_precision(gt: List[dict], all_pos: List[dict]) -> float:
         """Calculate precision.
```

## presidio_image_redactor/dicom_image_redactor_engine.py

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 from copy import deepcopy
 import tempfile
 from pathlib import Path
-from PIL import Image
+from PIL import Image, ImageOps
 import pydicom
 from pydicom.pixel_data_handlers.util import apply_voi_lut
 import PIL
 import png
 import numpy as np
 from matplotlib import pyplot as plt  # necessary import for PIL typing # noqa: F401
 from typing import Tuple, List, Union, Optional
@@ -331,21 +331,21 @@
         """
         # Invert colors if invert flag is True
         if invert:
             if image.mode == "RGBA":
                 # Handle transparency as needed
                 r, g, b, a = image.split()
                 rgb_image = Image.merge("RGB", (r, g, b))
-                inverted_image = PIL.ImageOps.invert(rgb_image)
+                inverted_image = ImageOps.invert(rgb_image)
                 r2, g2, b2 = inverted_image.split()
 
                 image = Image.merge("RGBA", (r2, g2, b2, a))
 
             else:
-                image = PIL.ImageOps.invert(image)
+                image = ImageOps.invert(image)
 
         # Get background color
         if is_greyscale:
             # Select most common color as color
             bg_color = int(np.bincount(list(image.getdata())).argmax())
         else:
             # Reduce size of image to 1 pixel to get dominant color
```

## Comparing `presidio_image_redactor-0.0.46.dist-info/METADATA` & `presidio_image_redactor-0.0.47.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: presidio-image-redactor
-Version: 0.0.46
+Version: 0.0.47
 Summary: Presidio image redactor package
 Home-page: https://github.com/Microsoft/presidio
 License: MIT
 Keywords: presidio_image_redactor
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Requires-Dist: pillow (>=9.0)
 Requires-Dist: pytesseract (==0.3.7)
 Requires-Dist: presidio-analyzer (>=1.9.0)
 Requires-Dist: matplotlib (==3.6.2)
 Requires-Dist: pydantic (==1.7.4)
```

## Comparing `presidio_image_redactor-0.0.46.dist-info/RECORD` & `presidio_image_redactor-0.0.47.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 presidio_image_redactor/__init__.py,sha256=A9X45d5XBrAXQAia9RYtM71fTRbdtiVRKlJxaARPrlM,784
 presidio_image_redactor/bbox.py,sha256=-am94Cthy-vUE7PgmNq-YGTTtRbO-t3ytAFLoTdsbTU,4970
-presidio_image_redactor/dicom_image_pii_verify_engine.py,sha256=ip5dNCjEDSdXXZBP9aQsscqKqLuu4Pz55rctSZdBIVM,9991
-presidio_image_redactor/dicom_image_redactor_engine.py,sha256=AQpkRaWQh67LAXDl3Gisp9mKRuxujGDYsNCTv-RU4aQ,32053
+presidio_image_redactor/dicom_image_pii_verify_engine.py,sha256=XhqLUyxj-953rJJUpzYFnIr6Mk5UiQ6mDZcU6OTjCk8,10224
+presidio_image_redactor/dicom_image_redactor_engine.py,sha256=4tzuEvcJGgIumTQ3r0jqKP-qpd3_dJEyViQfMLmdmrU,32055
 presidio_image_redactor/image_analyzer_engine.py,sha256=KuEJGE198NtPQVM-ly1viNAWvhTVMigbYdYtkFhhfuM,6921
 presidio_image_redactor/image_pii_verify_engine.py,sha256=y2o3mi9GXVBvSksebM1uGX7d4w7_imh7KnU8pO3cd1Y,2470
 presidio_image_redactor/image_redactor_engine.py,sha256=z8n1LLr54Y9z-vHANNEeYj5x0j28fiy1WhnjG8UZNhI,1818
 presidio_image_redactor/ocr.py,sha256=n7x1JtH-fkbF8fvf2kRP2848JdXI59VPW4xJ3XOHj0o,981
 presidio_image_redactor/tesseract_ocr.py,sha256=cxnjsyaL3t6C8JJQe8tOslu8DeOZicnppEhUR3YEaG0,615
 presidio_image_redactor/entities/__init__.py,sha256=RqsxcYKASoFLPqPW5EmEoSIX85vraPFaUQdILQL2K_c,216
 presidio_image_redactor/entities/api_request_convertor.py,sha256=PAgB6aBAk5h1T749W5rLbWxrA80TPyo6U4BDq7Qzn90,2034
 presidio_image_redactor/entities/image_recognizer_result.py,sha256=9MR_KCXfJHqoawOQFixHMT_h1kSGBf5WlR9jnVJD1TI,2106
 presidio_image_redactor/entities/invalid_exception.py,sha256=FDGsHC0o5R06RmboBmqhFVYBfmole9TQvjziZw2eJ4w,274
-presidio_image_redactor-0.0.46.dist-info/METADATA,sha256=j7fjfvDoQWyNOMF3XyX2vfiAtaw3-DZYKZmLS0rveko,6291
-presidio_image_redactor-0.0.46.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-presidio_image_redactor-0.0.46.dist-info/top_level.txt,sha256=exMcxj0mg3Ey4ACq-Chz4sD5_7z-Z1YqHcfmWYUr0Oo,24
-presidio_image_redactor-0.0.46.dist-info/RECORD,,
+presidio_image_redactor-0.0.47.dist-info/METADATA,sha256=bXI5pIysESdA9FVC1iXW2tZlGqTe9C9Bxj5OFSfOwT4,6342
+presidio_image_redactor-0.0.47.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+presidio_image_redactor-0.0.47.dist-info/top_level.txt,sha256=exMcxj0mg3Ey4ACq-Chz4sD5_7z-Z1YqHcfmWYUr0Oo,24
+presidio_image_redactor-0.0.47.dist-info/RECORD,,
```

