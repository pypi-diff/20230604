# Comparing `tmp/install-pybci-0.2.3b0.tar.gz` & `tmp/install-pybci-0.2.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.2.3b0.tar", last modified: Sat Jun  3 16:51:21 2023, max compression
+gzip compressed data, was "install-pybci-0.2.3b1.tar", last modified: Sun Jun  4 12:56:08 2023, max compression
```

## Comparing `install-pybci-0.2.3b0.tar` & `install-pybci-0.2.3b1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-03 16:51:21.000000 install-pybci-0.2.3b0/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-03 16:51:21.000000 install-pybci-0.2.3b0/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:51:21.000000 install-pybci-0.2.3b0/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-03 16:51:21.000000 install-pybci-0.2.3b0/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 16:51:21.000000 install-pybci-0.2.3b0/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/OptimisedDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.943371 install-pybci-0.2.3b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-04 12:56:08.943371 install-pybci-0.2.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.939371 install-pybci-0.2.3b1/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-04 12:56:08.000000 install-pybci-0.2.3b1/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-04 12:56:08.000000 install-pybci-0.2.3b1/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:56:08.000000 install-pybci-0.2.3b1/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-04 12:56:08.000000 install-pybci-0.2.3b1/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 12:56:08.000000 install-pybci-0.2.3b1/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.939371 install-pybci-0.2.3b1/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.939371 install-pybci-0.2.3b1/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.943371 install-pybci-0.2.3b1/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/OptimisedDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:56:08.943371 install-pybci-0.2.3b1/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 12:56:08.943371 install-pybci-0.2.3b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-04 12:55:33.000000 install-pybci-0.2.3b1/setup.py
```

### Comparing `install-pybci-0.2.3b0/LICENSE` & `install-pybci-0.2.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/PKG-INFO` & `install-pybci-0.2.3b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.3b0
+Version: 0.2.3b1
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `install-pybci-0.2.3b0/README.md` & `install-pybci-0.2.3b1/README.md`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.2.3b1/install_pybci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.3b0
+Version: 0.2.3b1
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `install-pybci-0.2.3b0/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.2.3b1/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/pybci/Configuration/EpochSettings.py` & `install-pybci-0.2.3b1/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.2.3b1/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.2.3b1/pybci/ThreadClasses/ClassifierThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.2.3b1/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.2.3b1/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/pybci/ThreadClasses/OptimisedDataReceiverThread.py` & `install-pybci-0.2.3b1/pybci/ThreadClasses/OptimisedDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/pybci/Utils/Classifier.py` & `install-pybci-0.2.3b1/pybci/Utils/Classifier.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.2.3b1/pybci/Utils/FeatureExtractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import antropy as ant
 import numpy as np
 from scipy.signal import welch
 from scipy.integrate import simps
 import warnings, time
-from ..Utils.Logger import Logger
 from ..Configuration.FeatureSettings import GeneralFeatureChoices
 # Filter out UserWarning messages from the scipy package, could be worth moving to init and applying printdebug print levels? (typically nans, 0 and infs causing errors)
 warnings.filterwarnings("ignore", category=UserWarning, module="scipy") # used to reduce print statements from constant signals being applied
 warnings.filterwarnings("ignore", category=UserWarning, module="antropy") # used to reduce print statements from constant signals being applied
 warnings.filterwarnings("ignore", category=RuntimeWarning, module="antropy") # used to reduce print statements from constant signals being applied
 warnings.filterwarnings("ignore", category=RuntimeWarning, module="numpy") # used to reduce print statements from constant signals being applied
 #warnings.filterwarnings("ignore", category=RuntimeWarning, module="pybci") # used to reduce print statements from constant signals being applied
 
 class GenericFeatureExtractor():
-    logger = Logger(Logger.INFO)
-
-    def __init__(self, logger = Logger(Logger.INFO), freqbands = [[1.0, 4.0], [4.0, 8.0], [8.0, 12.0], [12.0, 20.0]], featureChoices = GeneralFeatureChoices()):
+    def __init__(self, freqbands = [[1.0, 4.0], [4.0, 8.0], [8.0, 12.0], [12.0, 20.0]], featureChoices = GeneralFeatureChoices()):
         super().__init__()
         self.freqbands = freqbands
         self.featureChoices = featureChoices
         #for key, value in self.featureChoices.__dict__.items():
         #    print(f"{key} = {value}")
-        self.logger = logger
         selFeats = sum([self.featureChoices.appr_entropy,
             self.featureChoices.perm_entropy,
             self.featureChoices.spec_entropy,
             self.featureChoices.svd_entropy,
             self.featureChoices.samp_entropy,
             self.featureChoices.rms,
             self.featureChoices.meanPSD,
@@ -48,17 +44,14 @@
             target = string of received marker type
             sr = samplerate of current device
         Returns:
             features = 2D numpy array of size (chs, (len(freqbands) + sum(True in self.featureChoices)))
             target = same as input target, can be useful for using a baseline number differently
         NOTE: Any channels with a constant value will generate warnings in any frequency based features (constant level == no frequency components).
         """
-        #print(np.array(epoch).shape)
-        #print(epoch)
-        start = time.time()
         numchs = epoch.shape[1]
         features = np.zeros(numchs * self.numFeatures)
 
         for ch in range(epoch.shape[1]):
             #ch = np.isnan(ch)
             if self.featureChoices.psdBand: # get custom average power within given frequency band from freqbands
                 freqs, psd = welch(epoch[:,ch], sr)
@@ -118,17 +111,15 @@
             #if self.featureChoices.slopeSignChange: # slopeSignChange
             #    l += 1    
             #    ssc = sum([1 if (c-ch[inum+1])*(c-ch[inum+1])>=0.1 else 0 for inum, c in enumerate(ch[:-1])])
             #    features[(ch self.numFeatures)+l] = ssc
         features[np.isnan(features)] = 0 # checks for nans
         features[features == np.inf] = 0#np.iinfo(np.int32).max
         #print(features)
-        if (self.logger.level == Logger.TIMING):
-            end = time.time()
-            self.logger.log(Logger.TIMING, f" Generic Feature Extraction time {end - start}")
+        
         return features
     
 class GazeFeatureExtractor():
     def __init__(self):
         super().__init__()
 
 '''pupil channels in order
```

### Comparing `install-pybci-0.2.3b0/pybci/Utils/LSLScanner.py` & `install-pybci-0.2.3b1/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/pybci/Utils/Logger.py` & `install-pybci-0.2.3b1/pybci/Utils/Logger.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.3b0/pybci/pybci.py` & `install-pybci-0.2.3b1/pybci/pybci.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,21 +249,21 @@
                     dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
                                             self.globalEpochSettings, len(self.dataThreads),maxExpectedSampleRate = stream.info().nominal_srate())
             dt.start()
             self.dataThreads.append(dt)
             if stream.info().name() in self.streamCustomFeatureExtract.keys():
                 self.ft = FeatureProcessorThread(self.closeEvent,self.trainTestEvent, self.dataQueueTrain, self.dataQueueTest,
                                                 self.featureQueueTest,self.featureQueueTrain, len(self.dataStreams),
-                                                self.markerCountRetrieveEvent, self.markerCountQueue,
+                                                self.markerCountRetrieveEvent, self.markerCountQueue,logger=self.logger,
                                                 featureExtractor = self.streamCustomFeatureExtract[stream.info().name()],
                                                 globalEpochSettings = self.globalEpochSettings, customEpochSettings = self.customEpochSettings)
             else:
                 self.ft = FeatureProcessorThread(self.closeEvent,self.trainTestEvent, self.dataQueueTrain, self.dataQueueTest,
                                                 self.featureQueueTest,self.featureQueueTrain, len(self.dataStreams),
-                                                self.markerCountRetrieveEvent, self.markerCountQueue,
+                                                self.markerCountRetrieveEvent, self.markerCountQueue,logger=self.logger,
                                                 globalEpochSettings = self.globalEpochSettings, customEpochSettings = self.customEpochSettings)
             self.ft.start()
             self.featureThreads.append(dt)
         # marker thread requires data and feature threads to push new markers too
         self.markerThread = MarkerThread(self.closeEvent,self.trainTestEvent, self.markerStream,self.dataThreads, self.featureThreads)
         self.markerThread.start()
         self.classifierThread = ClassifierThread(self.closeEvent,self.trainTestEvent, self.featureQueueTest,self.featureQueueTrain,
```

### Comparing `install-pybci-0.2.3b0/setup.py` & `install-pybci-0.2.3b1/setup.py`

 * *Files identical despite different names*

