# Comparing `tmp/mosaic-library-1.0.1.tar.gz` & `tmp/mosaic-library-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaic-library-1.0.1.tar", last modified: Sun May 28 16:23:50 2023, max compression
+gzip compressed data, was "mosaic-library-1.0.2.tar", last modified: Sun Jun  4 12:10:04 2023, max compression
```

## Comparing `mosaic-library-1.0.1.tar` & `mosaic-library-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/
--rw-rw-r--   0 fft       (1000) fft       (1000)     1083 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/LICENSE
--rw-rw-r--   0 fft       (1000) fft       (1000)    18654 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/PKG-INFO
--rw-rw-r--   0 fft       (1000) fft       (1000)    18072 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/README.MD
-drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/mosaic_library.egg-info/
--rw-rw-r--   0 fft       (1000) fft       (1000)    18654 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/PKG-INFO
--rw-rw-r--   0 fft       (1000) fft       (1000)      475 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/SOURCES.txt
--rw-rw-r--   0 fft       (1000) fft       (1000)        1 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/dependency_links.txt
--rw-rw-r--   0 fft       (1000) fft       (1000)       98 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/entry_points.txt
--rw-rw-r--   0 fft       (1000) fft       (1000)       86 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/requires.txt
--rw-rw-r--   0 fft       (1000) fft       (1000)       11 2023-05-28 16:23:50.000000 mosaic-library-1.0.1/mosaic_library.egg-info/top_level.txt
-drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/mosaicking/
--rw-rw-r--   0 fft       (1000) fft       (1000)        0 2023-05-19 14:29:07.000000 mosaic-library-1.0.1/mosaicking/__init__.py
--rw-rw-r--   0 fft       (1000) fft       (1000)     5067 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/calibration.py
--rw-rw-r--   0 fft       (1000) fft       (1000)    22678 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/mosaic.py
--rw-rw-r--   0 fft       (1000) fft       (1000)     6135 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/preprocessing.py
--rw-rw-r--   0 fft       (1000) fft       (1000)     2156 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/registration.py
--rw-rw-r--   0 fft       (1000) fft       (1000)    16557 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/transformations.py
--rw-rw-r--   0 fft       (1000) fft       (1000)    11706 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/mosaicking/utils.py
--rw-rw-r--   0 fft       (1000) fft       (1000)      656 2023-05-28 16:21:44.000000 mosaic-library-1.0.1/pyproject.toml
--rw-rw-r--   0 fft       (1000) fft       (1000)      427 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/setup.cfg
-drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-05-28 16:23:50.971173 mosaic-library-1.0.1/tests/
--rw-rw-r--   0 fft       (1000) fft       (1000)     2727 2023-05-28 16:07:39.000000 mosaic-library-1.0.1/tests/test_preprocessing.py
+drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-06-04 12:10:04.135498 mosaic-library-1.0.2/
+-rw-rw-r--   0 fft       (1000) fft       (1000)     1083 2023-05-28 16:07:39.000000 mosaic-library-1.0.2/LICENSE
+-rw-rw-r--   0 fft       (1000) fft       (1000)    18656 2023-06-04 12:10:04.135498 mosaic-library-1.0.2/PKG-INFO
+-rw-rw-r--   0 fft       (1000) fft       (1000)    18074 2023-05-28 17:05:15.000000 mosaic-library-1.0.2/README.MD
+drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-06-04 12:10:04.131498 mosaic-library-1.0.2/mosaic_library.egg-info/
+-rw-rw-r--   0 fft       (1000) fft       (1000)    18656 2023-06-04 12:10:04.000000 mosaic-library-1.0.2/mosaic_library.egg-info/PKG-INFO
+-rw-rw-r--   0 fft       (1000) fft       (1000)      502 2023-06-04 12:10:04.000000 mosaic-library-1.0.2/mosaic_library.egg-info/SOURCES.txt
+-rw-rw-r--   0 fft       (1000) fft       (1000)        1 2023-06-04 12:10:04.000000 mosaic-library-1.0.2/mosaic_library.egg-info/dependency_links.txt
+-rw-rw-r--   0 fft       (1000) fft       (1000)       98 2023-06-04 12:10:04.000000 mosaic-library-1.0.2/mosaic_library.egg-info/entry_points.txt
+-rw-rw-r--   0 fft       (1000) fft       (1000)       86 2023-06-04 12:10:04.000000 mosaic-library-1.0.2/mosaic_library.egg-info/requires.txt
+-rw-rw-r--   0 fft       (1000) fft       (1000)       11 2023-06-04 12:10:04.000000 mosaic-library-1.0.2/mosaic_library.egg-info/top_level.txt
+drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-06-04 12:10:04.131498 mosaic-library-1.0.2/mosaicking/
+-rw-rw-r--   0 fft       (1000) fft       (1000)        0 2023-05-19 14:29:07.000000 mosaic-library-1.0.2/mosaicking/__init__.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)     5067 2023-05-28 16:07:39.000000 mosaic-library-1.0.2/mosaicking/calibration.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)    22784 2023-06-04 11:43:46.000000 mosaic-library-1.0.2/mosaicking/mosaic.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)     6135 2023-05-28 16:07:39.000000 mosaic-library-1.0.2/mosaicking/preprocessing.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)     2745 2023-06-04 11:31:28.000000 mosaic-library-1.0.2/mosaicking/registration.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)    16557 2023-05-28 16:07:39.000000 mosaic-library-1.0.2/mosaicking/transformations.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)    11608 2023-06-04 11:48:42.000000 mosaic-library-1.0.2/mosaicking/utils.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)      656 2023-06-04 11:55:59.000000 mosaic-library-1.0.2/pyproject.toml
+-rw-rw-r--   0 fft       (1000) fft       (1000)      427 2023-06-04 12:10:04.135498 mosaic-library-1.0.2/setup.cfg
+drwxrwxr-x   0 fft       (1000) fft       (1000)        0 2023-06-04 12:10:04.135498 mosaic-library-1.0.2/tests/
+-rw-rw-r--   0 fft       (1000) fft       (1000)     2727 2023-05-28 16:07:39.000000 mosaic-library-1.0.2/tests/test_preprocessing.py
+-rw-rw-r--   0 fft       (1000) fft       (1000)     1177 2023-06-04 11:33:39.000000 mosaic-library-1.0.2/tests/test_registration.py
```

### Comparing `mosaic-library-1.0.1/LICENSE` & `mosaic-library-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaic-library-1.0.1/PKG-INFO` & `mosaic-library-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaic-library
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python library for manipulating images for underwater mosaicking applications.
 Author-email: Fletcher Thompson <fletho@dtu.dk>
 Project-URL: Homepage, https://github.com/DTUAqua-ObsTek/mosaic-library
 Project-URL: Bug Tracker, https://github.com/DTUAqua-ObsTek/mosaic-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -264,18 +264,18 @@
 $$
 
 Where $f_x$ and $f_y$ are the focal lengths in the image coordinate frame x and y directions respectively, 
 measured in pixels. $c_x$ and $c_y$ are the principle points in the image coordinate frame x and y directions respectively.
 Since focal lengths of cameras are generally reported in mm, the method for converting is as follows:
 
 $$
-\begin{align*}
+\begin{aligned}
 f_x &= \frac{f\times w}{W} \\
 f_y &= \frac{f\times h}{H}
-\end{align*}
+\end{aligned}
 $$
 
 Where $f$ is the focal length measured in mm, $w$ is the image width in pixels, $W$ is the sensor width in mm,
 $h$ is the image height in pixels, and $H$ is the sensor height in mm. Information on a variety of commonly used
 sensors are available [here](https://en.wikipedia.org/wiki/Image_sensor_format#Table_of_sensor_formats_and_sizes).
 
 Additionally, the effects of the lens can distort the path of light making objects that should be straight appear curved.
```

### Comparing `mosaic-library-1.0.1/README.MD` & `mosaic-library-1.0.2/README.MD`

 * *Files 1% similar despite different names*

```diff
@@ -250,18 +250,18 @@
 $$
 
 Where $f_x$ and $f_y$ are the focal lengths in the image coordinate frame x and y directions respectively, 
 measured in pixels. $c_x$ and $c_y$ are the principle points in the image coordinate frame x and y directions respectively.
 Since focal lengths of cameras are generally reported in mm, the method for converting is as follows:
 
 $$
-\begin{align*}
+\begin{aligned}
 f_x &= \frac{f\times w}{W} \\
 f_y &= \frac{f\times h}{H}
-\end{align*}
+\end{aligned}
 $$
 
 Where $f$ is the focal length measured in mm, $w$ is the image width in pixels, $W$ is the sensor width in mm,
 $h$ is the image height in pixels, and $H$ is the sensor height in mm. Information on a variety of commonly used
 sensors are available [here](https://en.wikipedia.org/wiki/Image_sensor_format#Table_of_sensor_formats_and_sizes).
 
 Additionally, the effects of the lens can distort the path of light making objects that should be straight appear curved.
```

### Comparing `mosaic-library-1.0.1/mosaic_library.egg-info/PKG-INFO` & `mosaic-library-1.0.2/mosaic_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaic-library
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python library for manipulating images for underwater mosaicking applications.
 Author-email: Fletcher Thompson <fletho@dtu.dk>
 Project-URL: Homepage, https://github.com/DTUAqua-ObsTek/mosaic-library
 Project-URL: Bug Tracker, https://github.com/DTUAqua-ObsTek/mosaic-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -264,18 +264,18 @@
 $$
 
 Where $f_x$ and $f_y$ are the focal lengths in the image coordinate frame x and y directions respectively, 
 measured in pixels. $c_x$ and $c_y$ are the principle points in the image coordinate frame x and y directions respectively.
 Since focal lengths of cameras are generally reported in mm, the method for converting is as follows:
 
 $$
-\begin{align*}
+\begin{aligned}
 f_x &= \frac{f\times w}{W} \\
 f_y &= \frac{f\times h}{H}
-\end{align*}
+\end{aligned}
 $$
 
 Where $f$ is the focal length measured in mm, $w$ is the image width in pixels, $W$ is the sensor width in mm,
 $h$ is the image height in pixels, and $H$ is the sensor height in mm. Information on a variety of commonly used
 sensors are available [here](https://en.wikipedia.org/wiki/Image_sensor_format#Table_of_sensor_formats_and_sizes).
 
 Additionally, the effects of the lens can distort the path of light making objects that should be straight appear curved.
```

### Comparing `mosaic-library-1.0.1/mosaicking/calibration.py` & `mosaic-library-1.0.2/mosaicking/calibration.py`

 * *Files identical despite different names*

### Comparing `mosaic-library-1.0.1/mosaicking/mosaic.py` & `mosaic-library-1.0.2/mosaicking/mosaic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import cv2
 from cv2 import fisheye
 from pathlib import Path
 import sys
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.spatial.transform import Rotation
+import warnings
+import traceback
 
 import mosaicking.transformations
 from mosaicking import preprocessing, utils, transformations, registration
-from itertools import chain
 import yaml
 
 
 def main():
     args = utils.parse_args()
 
     reader = utils.VideoPlayer(args)
@@ -20,27 +21,23 @@
     output_path = Path(args.output_directory).resolve()
     output_path.mkdir(parents=True, exist_ok=True)
 
     if args.orientation_file is not None:
         ori_path = Path(args.orientation_file).resolve()
         assert ori_path.exists(), "File not found: {}".format(str(ori_path))
         if args.sync_points is None and args.time_offset is None:
-            sys.stderr.write(
-                "Warning: No --sync_points or --time_offset argument given, assuming video and orientation file start at the same time.\n")
+            warnings.warn("No --sync_points or --time_offset argument given, assuming video and orientation file start at the same time.", UserWarning)
         orientations = utils.load_orientations(ori_path, args)
         quat_lut = interp1d(orientations.index, orientations[["qx", "qy", "qz", "qw"]], axis=0, kind='nearest')
 
     # IF DEMO SPECIFIED, THEN GENERATE THE DEMO VIDEO
     if args.demo:
         output_video = output_path.joinpath("demo.mp4")
         writer = cv2.VideoWriter(str(output_video), cv2.VideoWriter_fourcc(*"mp4v"), reader.fps, frameSize=(1920, 1080), isColor=True)
 
-    # FORMAT SPEC FOR PROGRESS
-    formatspec = "{:0" + "{}d".format(len(str(reader.n_frames))) + "}"
-
     # DISPLAY WINDOWS
     if args.show_mosaic:
         cv2.namedWindow(args.video, cv2.WINDOW_NORMAL)
     if args.show_rotation:
         cv2.namedWindow("ROTATION COMPENSATION", cv2.WINDOW_NORMAL)
     if args.show_preprocessing:
         cv2.namedWindow("PREPROCESSING RESULT", cv2.WINDOW_NORMAL)
@@ -60,23 +57,27 @@
             detectors.append(cv2.ORB_create())  # ORB detector is pretty good and is CC licensed
         if model == "SIFT":
             detectors.append(cv2.SIFT_create())
         if model == "SURF":
             try:
                 detectors.append(cv2.xfeatures2d.SURF_create())
             except cv2.error:
-                sys.stderr.write("WARNING: Trying to use non-free SURF on OpenCV built with non-free option disabled.\n")
-        # if model == "FAST":
-        #     detectors.append(cv2.FastFeatureDetector_create())
-        # if model == "BRIEF":
-        #    detectors.append(cv2.xfeatures2d.BriefDescriptorExtractor_create())
-        # if model == "FREAK":
-        #    detectors.append(cv2.xfeatures2d.FREAK_create())
-        # if model == "GFTT":
-        #    detectors.append(cv2.GFTTDetector_create())
+                warnings.warn("Trying to use non-free SURF on OpenCV built with non-free option disabled.", UserWarning)
+        if model == "FAST":
+            warnings.warn("FAST features are not yet implemented.", UserWarning)
+            #detectors.append(cv2.FastFeatureDetector_create())
+        if model == "BRIEF":
+            warnings.warn("BRIEF features are not yet implemented.", UserWarning)
+            #detectors.append(cv2.xfeatures2d.BriefDescriptorExtractor_create())
+        if model == "FREAK":
+            warnings.warn("FREAK features are not yet implemented.", UserWarning)
+            #detectors.append(cv2.xfeatures2d.FREAK_create())
+        if model == "GFTT":
+            warnings.warn("GFTT features are not yet implemented.", UserWarning)
+            #detectors.append(cv2.GFTTDetector_create())
         if model == "BRISK":
             detectors.append(cv2.BRISK_create())
         if model == "KAZE":
             detectors.append(cv2.KAZE_create())
 
     # DEFINE THE MATCHER METHOD
     # FLANN parameters
@@ -100,31 +101,35 @@
         calibration_path = Path(args.calibration).resolve()
         assert calibration_path.exists(), "File not found: {}".format(str(calibration_path))
         with open(args.calibration, "r") as f:
             calib_data = yaml.safe_load(f)
         if 'camera_matrix' in calib_data:
             K = np.array(calib_data['camera_matrix']['data']).reshape((3, 3))
         else:
-            sys.stderr.write(f"WARNING: No camera_matrix found in {str(calibration_path)}\n")
-
-    print("K: {}".format(repr(K)))
-    K_scaled = K.copy()  # A copy of K that is scaled
+            warnings.warn(f"No camera_matrix found in {str(calibration_path)}", UserWarning)
 
     # Camera Lens distortion coefficients
-    distCoeff = np.zeros((4, 1), np.float64)
+    dist_coeff = np.zeros((4, 1), np.float64)
     if args.distortion is not None:
-        distCoeff = np.array([[d] for d in args.distortion], np.float64)
+        dist_coeff = np.array([[d] for d in args.distortion], np.float64)
     if args.calibration is not None:
         if 'distortion_coefficients' in calib_data:
-            distCoeff = np.array(calib_data['distortion_coefficients']['data']).reshape((calib_data['distortion_coefficients']['rows'],
-                                                                                         calib_data['distortion_coefficients']['cols']))
+            dist_coeff = np.array(calib_data['distortion_coefficients']['data']).reshape((calib_data['distortion_coefficients']['rows'],
+                                                                                          calib_data['distortion_coefficients']['cols']))
         else:
-            sys.stderr.write(f"WARNING: No distortion_coefficients found in {str(calibration_path)}\n")
+            warnings.warn(f"No distortion_coefficients found in {str(calibration_path)}", UserWarning)
+
+    K, roi = cv2.getOptimalNewCameraMatrix(K, dist_coeff, (reader.width, reader.height), 0)
+
+    print("K:", K)
+    K_scaled = K.copy()  # A copy of K that is scaled
 
     # BEGIN MAIN LOOP #
+    img = None
+    mosaic_img = None
     init = True  # Flag to init
     nomatches = False  # Prevents consecutive tile dumps due to no match
     counter = 0  # Counter to intermittently save the output mosaic
     tile_counter = 0  # Counter for number of generated tiles.
     try:  # External try to handle any unexpected errors
         print(f"Frames available: {len(reader)}")
         print(reader)
@@ -132,19 +137,19 @@
         for img in reader:
             print(reader)
             og = img.copy()  # keep a copy for later reference
 
             # Preprocess the image
             # First rectify the image
             if args.fisheye:
-                img = fisheye.undistortImage(img, K, distCoeff)
-                image_mask = fisheye.undistortImage(255 * np.ones_like(img), K, distCoeff)[:, :, 0]
+                img = fisheye.undistortImage(img, K, dist_coeff)
+                image_mask = fisheye.undistortImage(255 * np.ones_like(img), K, dist_coeff)[:, :, 0]
             else:
-                img = cv2.undistort(img, K, distCoeff)
-                image_mask = cv2.undistort(255 * np.ones_like(img), K, distCoeff)[:, :, 0]
+                img = cv2.undistort(img, K, dist_coeff)
+                image_mask = cv2.undistort(255 * np.ones_like(img), K, dist_coeff)[:, :, 0]
             # Then apply color correction if specified
             img = preprocessing.imadjust(img) if args.imadjust else img
             # Then apply contrast balancing if specified
             img = preprocessing.equalize_color(img) if args.equalize_color else img
             # Then apply light balancing if specified
             img = preprocessing.equalize_luminance(img) if args.equalize_luminance else img
             # Enhance detail
@@ -165,18 +170,16 @@
                                              fontsize, (255, 255, 255), 3)
                 cv2.imshow("PREPROCESSING RESULT", preproc_result)
 
             # If it's the first time, then acquire keypoints and go to next frame
             if init:
                 sys.stdout.write("Initializing new mosaic.\n")
                 # Detect keypoints on the first frame
-                features = [registration.get_features(img, detector) for detector in detectors]
-                kp_prev = list(chain.from_iterable([f[0] for f in features]))
+                kp_prev, des_prev = registration.get_keypoints_descriptors(img, detectors)
                 num_features = len(kp_prev)
-                des_prev = [f[1] for f in features]
                 if num_features < args.min_features:
                     sys.stderr.write("Not Enough Features, Finding Good Frame.\n")
                     continue
                 # Apply scaling to image if specified
                 if args.scale_factor > 0.0:
                     img, kp_prev, image_mask = transformations.apply_scale(img, kp_prev, args.scale_factor,
                                                                            image_mask)
@@ -208,18 +211,16 @@
                 t = [0, 0]  # Initialize the translation to 0
                 init = False  # Initialization complete
                 sys.stdout.write("Init stage complete.\n")
                 continue
             # We are now mosaicking
             else:
                 # Detect keypoints in the new frame
-                features = [registration.get_features(img, detector) for detector in detectors]
-                kp = list(chain.from_iterable([f[0] for f in features]))
+                kp, des = registration.get_keypoints_descriptors(img, detectors)
                 num_features = len(kp)
-                des = [f[1] for f in features]
                 if num_features < args.min_features:
                     sys.stderr.write("Not Enough Features, Skipping Frame.\n")
                     continue
                 if args.scale_factor > 0.0:
                     img, kp, image_mask = transformations.apply_scale(img, kp, args.scale_factor, image_mask)
                     K_scaled = K.copy()
                     K_scaled = K_scaled * args.scale_factor
@@ -367,32 +368,33 @@
                 counter = counter + 1
                 if args.save_freq > 0 and counter % args.save_freq == 0:
                     counter = 0
                     fpath = output_path.joinpath("current_mosaic.png")
                     cv2.imwrite(str(fpath), mosaic_img)
                 if key == ord("q") or key & 0xff == 27:
                     raise KeyboardInterrupt
-    except Exception as err:
+    except KeyboardInterrupt:
+        sys.stderr.write("\nUser terminated program.\n")
+    except Exception:
         # Some strange error has occurred, write out to stderr, cleanup and rethrow the error
         sys.stderr.write("\nPipeline failed at frame {}\n".format(reader.get(cv2.CAP_PROP_POS_FRAMES) + 1))
+        traceback.print_exc()
+        fpath = output_path.joinpath("error_frame.png")
+        if img is not None:
+            cv2.imwrite(str(fpath), img)
+        fpath = output_path.joinpath("error_mosaic.png")
+        if mosaic_img is not None:
+            cv2.imwrite(str(fpath), mosaic_img)
+    finally:
+        # Cleanup actions and exit.
+        fpath = output_path.joinpath("tile_{:03d}.png".format(tile_counter))
+        if mosaic_img is not None:
+            cv2.imwrite(str(fpath), mosaic_img)
         cv2.destroyAllWindows()
-        del reader
+        reader.release()
+        #del reader
         if args.demo:
             writer.release()
-        fpath = output_path.joinpath("error_frame.png")
-        cv2.imwrite(str(fpath), img)
-        fpath = output_path.joinpath("error_mosaic.png")
-        cv2.imwrite(str(fpath), mosaic_img)
-        raise err
-        # The video exited properly, so cleanup and exit.
-    except KeyboardInterrupt:
-        sys.stderr.write("\nUser terminated program.\n")
-    fpath = output_path.joinpath("tile_{:03d}.png".format(tile_counter))
-    cv2.imwrite(str(fpath), mosaic_img)
-    cv2.destroyAllWindows()
-    del reader
-    if args.demo:
-        writer.release()
 
 
-if __name__=="__main__":
+if __name__ == "__main__":
     main()
```

### Comparing `mosaic-library-1.0.1/mosaicking/preprocessing.py` & `mosaic-library-1.0.2/mosaicking/preprocessing.py`

 * *Files identical despite different names*

### Comparing `mosaic-library-1.0.1/mosaicking/registration.py` & `mosaic-library-1.0.2/mosaicking/registration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import cv2
 import numpy as np
 from typing import Union, Tuple, List, Sequence
 from numpy import typing as npt
+from itertools import chain
 
 
-def get_matches(descriptors1: Union[npt.NDArray[float], list], descriptors2: Union[npt.NDArray[float], list], matcher: cv2.DescriptorMatcher, minmatches: int):
-    if not isinstance(descriptors1, list):
+def get_matches(descriptors1: Union[npt.NDArray[float], Sequence[npt.NDArray[float]]], descriptors2: Union[npt.NDArray[float], Sequence[npt.NDArray[float]]], matcher: cv2.DescriptorMatcher, minmatches: int):
+    if not isinstance(descriptors1, (tuple, list)):
         descriptors1 = [descriptors1]
-    if not isinstance(descriptors2, list):
+    if not isinstance(descriptors2, (tuple, list)):
         descriptors2 = [descriptors2]
     mlength = 0
     nlength = 0
     good = []
     for d1, d2 in zip(descriptors1, descriptors2):
         matches = matcher.knnMatch(d1.astype(np.float32), d2.astype(np.float32), 2)
         for m, n in matches:
@@ -22,23 +23,30 @@
             if m.distance < 0.7 * n.distance:
                 good.append(m)
         mlength += d1.shape[0]
         nlength += d2.shape[0]
     return minmatches <= len(good), good
 
 
-def get_features(img: npt.NDArray[np.uint8], fdet: cv2.Feature2D, mask: npt.NDArray[np.uint8] = None) -> Tuple[List[cv2.KeyPoint], npt.NDArray[float]]:
+def get_features(img: npt.NDArray[np.uint8], fdet: cv2.Feature2D, mask: npt.NDArray[np.uint8] = None) -> Tuple[List[cv2.KeyPoint], Union[npt.NDArray[np.float32], npt.NDArray[np.uint8]]]:
     """
-    Given a feature detector, obtain the features found in the image.
+    Given a feature detector, obtain the keypoints and descriptors found in the image.
     """
     if img.ndim > 2:
         img = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
     return fdet.detectAndCompute(img, mask)
 
 
+def get_keypoints_descriptors(img: npt.NDArray[np.uint8], detectors: Sequence[cv2.Feature2D], mask: npt.NDArray[np.uint8] = None) -> Tuple[Tuple[cv2.KeyPoint], Tuple[Union[npt.NDArray[np.float32], npt.NDArray[np.uint8]]]]:
+    features = [get_features(img, detector, mask) for detector in detectors]
+    kp = tuple(chain.from_iterable([f[0] for f in features]))
+    des = tuple(f[1] for f in features if f[1] is not None)
+    return kp, des
+
+
 def get_match_points(kp_src: Sequence[cv2.KeyPoint], kp_dst: Sequence[cv2.KeyPoint], matches: Sequence[cv2.DMatch]) -> Tuple[npt.NDArray[float], npt.NDArray[float]]:
     """
     Converts matched keypoint objects from source and destination into numpy arrays.
     """
     assert max([m.queryIdx for m in matches]) < len(kp_src), "Match indices are larger than length of src keypoints, check order of src, dst keypoint arguments."
     assert max([m.trainIdx for m in matches]) < len(kp_dst), "Match indices are larger than length of dst keypoints, check order of src, dst keypoint arguments."
     src_pts = np.float32([kp_src[m.queryIdx].pt for m in matches]).reshape(-1, 1, 2)
```

### Comparing `mosaic-library-1.0.1/mosaicking/transformations.py` & `mosaic-library-1.0.2/mosaicking/transformations.py`

 * *Files identical despite different names*

### Comparing `mosaic-library-1.0.1/mosaicking/utils.py` & `mosaic-library-1.0.2/mosaicking/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,18 +136,14 @@
         if self._finish_frame < self._start_frame:
             raise ValueError("Finishing frame is less than starting time.")
 
     def evaluate_stopping(self):
         """Return true if stopping conditions met."""
         return self._finish_frame <= self.get(cv2.CAP_PROP_POS_FRAMES)
 
-    def __del__(self):
-        print(f"Closing video {self._args.video}")
-        self.release()
-
     def __len__(self):
         return len(range(*slice(self._start_frame, self._finish_frame, self.frame_skip).indices(self.n_frames)))
 
 
 class VideoPlayerIterator:
     def __init__(self, videoplayer: VideoPlayer):
         self._videoplayer = videoplayer
```

### Comparing `mosaic-library-1.0.1/pyproject.toml` & `mosaic-library-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "mosaic-library"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Fletcher Thompson", email="fletho@dtu.dk" },
 ]
 description = "A python library for manipulating images for underwater mosaicking applications."
 readme = "README.MD"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mosaic-library-1.0.1/tests/test_preprocessing.py` & `mosaic-library-1.0.2/tests/test_preprocessing.py`

 * *Files identical despite different names*

