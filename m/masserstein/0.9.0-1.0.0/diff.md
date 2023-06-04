# Comparing `tmp/masserstein-0.9.0.tar.gz` & `tmp/masserstein-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/masserstein-0.9.0.tar", last modified: Sun Dec  6 16:25:04 2020, max compression
+gzip compressed data, was "masserstein-1.0.0.tar", last modified: Sun Jun  4 10:29:19 2023, max compression
```

## Comparing `masserstein-0.9.0.tar` & `masserstein-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,22 @@
-drwxr-xr-x   0 mist      (1000) users      (100)        0 2020-12-06 16:25:04.000000 masserstein-0.9.0/
--rw-r--r--   0 mist      (1000) users      (100)     1070 2020-07-09 22:31:14.000000 masserstein-0.9.0/LICENSE
--rw-r--r--   0 mist      (1000) users      (100)      940 2020-12-06 16:25:04.000000 masserstein-0.9.0/PKG-INFO
--rw-r--r--   0 mist      (1000) users      (100)     5450 2020-12-06 15:53:24.000000 masserstein-0.9.0/README.md
-drwxr-xr-x   0 mist      (1000) users      (100)        0 2020-12-06 16:25:04.000000 masserstein-0.9.0/Tutorials/
--rw-r--r--   0 mist      (1000) users      (100)  2857080 2020-12-06 15:53:24.000000 masserstein-0.9.0/Tutorials/Analysis of Mass Spectrometry Imaging data.ipynb
--rw-r--r--   0 mist      (1000) users      (100)   544199 2020-12-06 15:53:24.000000 masserstein-0.9.0/Tutorials/Package presentation.ipynb
-drwxr-xr-x   0 mist      (1000) users      (100)        0 2020-12-06 16:25:04.000000 masserstein-0.9.0/examples/
--rw-r--r--   0 mist      (1000) users      (100)      154 2020-07-09 22:31:14.000000 masserstein-0.9.0/examples/acetic_acid.txt
--rw-r--r--   0 mist      (1000) users      (100)      148 2020-07-09 22:31:14.000000 masserstein-0.9.0/examples/ethanol.txt
--rw-r--r--   0 mist      (1000) users      (100)      145 2020-07-09 22:31:14.000000 masserstein-0.9.0/examples/propane.txt
--rw-r--r--   0 mist      (1000) users      (100)      334 2020-07-09 22:31:14.000000 masserstein-0.9.0/examples/protein_molecule_list.txt
--rw-r--r--   0 mist      (1000) users      (100)  5367118 2020-07-09 22:31:14.000000 masserstein-0.9.0/examples/protein_spectrum.txt
--rw-r--r--   0 mist      (1000) users      (100)      415 2020-07-09 22:31:14.000000 masserstein-0.9.0/examples/small_molecule_list.txt
--rw-r--r--   0 mist      (1000) users      (100)     1543 2020-07-09 22:31:14.000000 masserstein-0.9.0/examples/small_molecule_spectrum.txt
-drwxr-xr-x   0 mist      (1000) users      (100)        0 2020-12-06 16:25:04.000000 masserstein-0.9.0/masserstein/
--rwxr-xr-x   0 mist      (1000) users      (100)    12376 2020-07-09 22:31:14.000000 masserstein-0.9.0/masserstein/WSDeconv.py
--rwxr-xr-x   0 mist      (1000) users      (100)     4092 2020-07-09 22:31:14.000000 masserstein-0.9.0/masserstein/WSDistance.py
--rw-r--r--   0 mist      (1000) users      (100)       54 2020-07-09 22:31:14.000000 masserstein-0.9.0/masserstein/__init__.py
--rw-r--r--   0 mist      (1000) users      (100)    17467 2020-12-06 15:53:24.000000 masserstein-0.9.0/masserstein/deconv_simplex.py
--rw-r--r--   0 mist      (1000) users      (100)     2195 2020-12-06 15:53:19.000000 masserstein-0.9.0/masserstein/peptides.py
--rw-r--r--   0 mist      (1000) users      (100)    29066 2020-12-06 15:53:24.000000 masserstein-0.9.0/masserstein/spectrum.py
-drwxr-xr-x   0 mist      (1000) users      (100)        0 2020-12-06 16:25:04.000000 masserstein-0.9.0/masserstein.egg-info/
--rw-r--r--   0 mist      (1000) users      (100)      940 2020-12-06 16:25:04.000000 masserstein-0.9.0/masserstein.egg-info/PKG-INFO
--rw-r--r--   0 mist      (1000) users      (100)      688 2020-12-06 16:25:04.000000 masserstein-0.9.0/masserstein.egg-info/SOURCES.txt
--rw-r--r--   0 mist      (1000) users      (100)        1 2020-12-06 16:25:04.000000 masserstein-0.9.0/masserstein.egg-info/dependency_links.txt
--rw-r--r--   0 mist      (1000) users      (100)       97 2020-12-06 16:25:04.000000 masserstein-0.9.0/masserstein.egg-info/entry_points.txt
--rw-r--r--   0 mist      (1000) users      (100)       50 2020-12-06 16:25:04.000000 masserstein-0.9.0/masserstein.egg-info/requires.txt
--rw-r--r--   0 mist      (1000) users      (100)       12 2020-12-06 16:25:04.000000 masserstein-0.9.0/masserstein.egg-info/top_level.txt
--rw-r--r--   0 mist      (1000) users      (100)       38 2020-12-06 16:25:04.000000 masserstein-0.9.0/setup.cfg
--rw-r--r--   0 mist      (1000) users      (100)     9254 2020-12-06 15:53:24.000000 masserstein-0.9.0/setup.py
+drwxr-xr-x   0 mist       (501) staff       (20)        0 2023-06-04 10:29:19.152190 masserstein-1.0.0/
+-rw-r--r--   0 mist       (501) staff       (20)     1134 2023-06-02 17:52:10.000000 masserstein-1.0.0/LICENSE
+-rw-r--r--   0 mist       (501) staff       (20)     1022 2023-06-04 10:29:19.152051 masserstein-1.0.0/PKG-INFO
+-rw-r--r--   0 mist       (501) staff       (20)     2096 2023-06-01 17:08:34.000000 masserstein-1.0.0/README.md
+drwxr-xr-x   0 mist       (501) staff       (20)        0 2023-06-04 10:29:19.147332 masserstein-1.0.0/masserstein/
+-rwxr-xr-x   0 mist       (501) staff       (20)    12376 2023-06-01 17:08:34.000000 masserstein-1.0.0/masserstein/WSDeconv.py
+-rwxr-xr-x   0 mist       (501) staff       (20)     4092 2023-06-01 17:08:34.000000 masserstein-1.0.0/masserstein/WSDistance.py
+-rw-r--r--   0 mist       (501) staff       (20)       77 2023-06-02 17:55:15.000000 masserstein-1.0.0/masserstein/__init__.py
+-rw-r--r--   0 mist       (501) staff       (20)    43976 2023-06-04 10:25:21.000000 masserstein-1.0.0/masserstein/deconv_simplex.py
+-rw-r--r--   0 mist       (501) staff       (20)      912 2023-06-01 17:08:34.000000 masserstein-1.0.0/masserstein/misc.py
+-rw-r--r--   0 mist       (501) staff       (20)     3088 2023-06-01 17:08:34.000000 masserstein-1.0.0/masserstein/model_selection.py
+-rw-r--r--   0 mist       (501) staff       (20)     2195 2023-06-01 17:08:34.000000 masserstein-1.0.0/masserstein/peptides.py
+-rw-r--r--   0 mist       (501) staff       (20)    33310 2023-06-02 17:41:00.000000 masserstein-1.0.0/masserstein/spectrum.py
+drwxr-xr-x   0 mist       (501) staff       (20)        0 2023-06-04 10:29:19.151840 masserstein-1.0.0/masserstein.egg-info/
+-rw-r--r--   0 mist       (501) staff       (20)     1022 2023-06-04 10:29:19.000000 masserstein-1.0.0/masserstein.egg-info/PKG-INFO
+-rw-r--r--   0 mist       (501) staff       (20)      441 2023-06-04 10:29:19.000000 masserstein-1.0.0/masserstein.egg-info/SOURCES.txt
+-rw-r--r--   0 mist       (501) staff       (20)        1 2023-06-04 10:29:19.000000 masserstein-1.0.0/masserstein.egg-info/dependency_links.txt
+-rw-r--r--   0 mist       (501) staff       (20)       96 2023-06-04 10:29:19.000000 masserstein-1.0.0/masserstein.egg-info/entry_points.txt
+-rw-r--r--   0 mist       (501) staff       (20)       55 2023-06-04 10:29:19.000000 masserstein-1.0.0/masserstein.egg-info/requires.txt
+-rw-r--r--   0 mist       (501) staff       (20)       12 2023-06-04 10:29:19.000000 masserstein-1.0.0/masserstein.egg-info/top_level.txt
+-rw-r--r--   0 mist       (501) staff       (20)       38 2023-06-04 10:29:19.152237 masserstein-1.0.0/setup.cfg
+-rw-r--r--   0 mist       (501) staff       (20)     9393 2023-06-02 17:51:41.000000 masserstein-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `masserstein-0.9.0/LICENSE` & `masserstein-1.0.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MIT License
 
-Copyright (c) 2019 Michał Ciach
+Copyright (c) 2019-2023 Michał Ciach, Michał Startek, Grzegorz Skoraczyński,
+Barbara Domżał
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `masserstein-0.9.0/PKG-INFO` & `masserstein-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: masserstein
-Version: 0.9.0
+Version: 1.0.0
 Summary: A library for analysis of Mass Spectrometry data using the Wasserstein metric
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: UNKNOWN
-Keywords: mass spectrrometry spectral deconvolution
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Keywords: mass spectrometry spectral deconvolution
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >2.7, >=3.6, <4
 Provides-Extra: graphics
+License-File: LICENSE
```

### Comparing `masserstein-0.9.0/masserstein/WSDeconv.py` & `masserstein-1.0.0/masserstein/WSDeconv.py`

 * *Files identical despite different names*

### Comparing `masserstein-0.9.0/masserstein/WSDistance.py` & `masserstein-1.0.0/masserstein/WSDistance.py`

 * *Files identical despite different names*

### Comparing `masserstein-0.9.0/masserstein/peptides.py` & `masserstein-1.0.0/masserstein/peptides.py`

 * *Files identical despite different names*

### Comparing `masserstein-0.9.0/masserstein/spectrum.py` & `masserstein-1.0.0/masserstein/spectrum.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import random
 import heapq
 import re
 from collections import Counter
 import numpy.random as rd
 from scipy.signal import argrelmax
 from .peptides import get_protein_formula
+from warnings import warn
+from copy import deepcopy
 
 class Spectrum:
     def __init__(self, formula='', threshold=0.001, total_prob=None,
                  charge=1, adduct=None, confs=None, label=None, **other):
         """Initialize a Spectrum class.
 
         Initialization can be done either by simulating a spectrum of an ion
@@ -138,14 +140,20 @@
     def average_mass(self):
         """
         Returns the average mass.
         """
         norm = float(sum(x[1] for x in self.confs))
         return sum(x[0]*x[1]/norm for x in self.confs)
 
+    def copy(self):
+        """
+        Return a (deep) copy of self
+        """
+        return deepcopy(self)
+
     # def copy(self):
     #     isospec = self.isospec
     #     self.isospec = None
     #     ret = deepcopy(self)
     #     ret.isospec = isospec
     #     self.isospec = isospec
     #     return ret
@@ -162,33 +170,37 @@
         """
         self.confs.sort(key = lambda x: x[0])
 
     def merge_confs(self):
         """
         Merges configurations with an identical mass, summing their intensities.
         """
-        cmass = self.confs[0][0]
-        cprob = 0.0
-        ret = []
-        for mass, prob in self.confs + [(-1, 0)]:
-            if mass != cmass:
-                ret.append((cmass, cprob))
-                cmass = mass
-                cprob = 0.0
-            cprob += prob
-        ### TODO3: for profile spectra, set a margin of max. 5 zero intensities
-        ### around any observed intensity to preserve peak shape
-        ### For centroid spectra, remove all zero intensities.
-        #self.confs = [x for x in ret if x[1] > 1e-12]
-        self.confs = ret
+        if not self.empty:
+            cmass = self.confs[0][0]
+            cprob = 0.0
+            ret = []
+            for mass, prob in self.confs + [(-1, 0)]:
+                if mass != cmass:
+                    ret.append((cmass, cprob))
+                    cmass = mass
+                    cprob = 0.0
+                cprob += prob
+            ### TODO3: for profile spectra, set a margin of max. 5 zero intensities
+            ### around any observed intensity to preserve peak shape
+            ### For centroid spectra, remove all zero intensities.
+            #self.confs = [x for x in ret if x[1] > 1e-12]
+            self.confs = ret
 
     def set_confs(self, confs):
         self.confs = confs
-        self.sort_confs()
-        self.merge_confs()
+        if len(self.confs) > 0:
+            self.sort_confs()
+            self.merge_confs()
+        else:
+            self.empty = True
 
     def __add__(self, other):
         res = Spectrum()
         res.confs = self.confs + other.confs
         res.sort_confs()
         res.merge_confs()
         res.label = self.label + ' + ' + other.label
@@ -283,32 +295,53 @@
     def coarse_bin(self, nb_of_digits):
         """
         Rounds the m/z to a given number of decimal digits
         """
         self.confs = [(round(x[0], nb_of_digits), x[1]) for x in self.confs]
         self.merge_confs()
 
-    def add_chemical_noise(self, nb_of_noise_peaks, noise_fraction):
+    def add_chemical_noise(self, nb_of_noise_peaks, noise_fraction, span=1.2):
+        """
+        Add additional peaks that simulate chemical noise.
+
+        The method adds additional peaks with uniform distribution in the m/z
+        domain and gamma distribution in the intensity domain. The spectrum
+        does NOT need to be normalized. Accordingly, the method does not
+        normalize the intensity afterwards! Works in-situ (on self).
+
+        Parameters
+        ----------
+        nb_of_noise_peaks : int
+            The number of added peaks.
+        noise_fraction : float
+            The amount of noise signal in the spectrum, >= 0 and <= 1.
+        span: float or 2-tuple of floats
+           If float, then `span` specifies a factor by which the m/z range is
+           increased. If 2-tuple, then `span` specifies m/z range, which is
+           noised.
+
+        Returns
+        -------
+        None
         """
-        Adds additional peaks with uniform distribution in the m/z domain
-        and gamma distribution in the intensity domain. The spectrum does NOT need
-        to be normalized. Accordingly, the method does not normalize the intensity afterwards!
-        noise_fraction controls the amount of noise signal in the spectrum.
-        nb_of_noise_peaks controls the number of peaks added.
-        """
-        span = min(x[0] for x in self.confs), max(x[0] for x in self.confs)
-        span_increase = 1.2  # increase the mass range by a factor of 1.2
-        span = [span_increase*x + (1-span_increase)*sum(span)/2 for x in span]
-        noisex = uniform.rvs(loc=span[0], scale=span[1]-span[0], size=nb_of_noise_peaks)
+        if isinstance(span, (float, int)):
+            span_increase = span
+            prev_span = (min(x[0] for x in self.confs),
+                         max(x[0] for x in self.confs))
+            span_move = 0.5 * (span_increase - 1) * (prev_span[1] - prev_span[0])
+            span = (max(prev_span[0] - span_move, 0),
+                    prev_span[1] + span_move)
+        noisex = uniform.rvs(loc=span[0], scale=span[1]-span[0],
+                             size=nb_of_noise_peaks)
         noisey = gamma.rvs(a=2, scale=2, size=nb_of_noise_peaks)
         noisey /= sum(noisey)
         signal = sum(x[1] for x in self.confs)
-        noisey *=  signal*noise_fraction /(1-noise_fraction)
+        noisey *=  signal * noise_fraction / (1 - noise_fraction)
         noise = [(x, y) for x,y in zip(noisex, noisey)]
-        self.confs += noise
+        self.confs.extend(noise)
         self.sort_confs()
         self.merge_confs()
 
     def add_gaussian_noise(self, sd):
         """
         Adds gaussian noise to each peak, simulating
         electronic noise.
@@ -391,41 +424,54 @@
         is advised in order to avoid detection of noise.
         """
         diffs = [n[1]-p[1] for n,p in zip(self.confs[1:], self.confs[:-1])]
         is_max = [nd <0 and pd > 0 for nd, pd in zip(diffs[1:], diffs[:-1])]
         peaks = [x for x, p in zip(self.confs[1:-1], is_max) if p]
         return peaks
 
+    def trim_negative_intensities(self):
+        """
+        Detects negative intensity measurements and sets them to 0.
+        """
+        self.confs = [(mz, intsy if intsy >= 0 else 0.) for mz, intsy in self.confs]
+
     def centroid(self, max_width, peak_height_fraction=0.5):
         """Return confs of a centroided spectrum.
 
         The function identifies local maxima of intensity and integrates peaks in the regions
         delimited by peak_height_fraction of the apex intensity.
         By default, for each peak the function will integrate the region delimited by the full width at half maximum.
         If the detected region is wider than max_width, the peak is considered as noise and discarded.
         Small values of max_width tend to miss peaks, while large ones increase computational complexity
         and may lead to false positives.
-        
+
         Note that this function should only be applied to profile spectra - the result
         does not make sense for centroided spectrum.
         Applying a gaussian or Savitzky-Golay filter prior to peak picking
         is advised in order to avoid detection of noise.
 
         Returns
         -----------------
             A tuple of two peak lists that can be used to construct a new Spectrum object.
             The first list contains configurations of centroids (i.e. centers of mass and areas of peaks).
             The second list contains configurations of peak apices corresponding to the centroids
             (i.e. locations and heights of the local maxima of intensity.)
         """
         ### TODO: change max_width to be in ppm?
+        # Validate the input:
+        if any(intsy < 0 for mz, intsy in self.confs):
+            warn("""
+                 The spectrum contains negative intensities!
+                 It is advised to use Spectrum.trim_negative_intensities() before any processing
+                 (unless you know what you're doing).
+                 """)
 
         # Transpose the confs list to get an array of masses and an array of intensities:
         mz, intsy = np.array(self.confs).T
-        
+
         # Find the local maxima of intensity:
         peak_indices = argrelmax(intsy)[0]
 
         peak_mz = []
         peak_intensity = []
         centroid_mz = []
         centroid_intensity = []
@@ -438,39 +484,44 @@
             target_intsy = peak_height_fraction*current_intsy
             right_shift = 1
             left_shift = 1
             # Get the mz points bounding the peak fragment to integrate.
             # First, go to the right from the detected apex until one of the four conditions are met:
             # 1. we exceed the mz range of the spectrum
             # 2. we exceed the maximum distance from the apex given by max_dist
-            # 3. the intensity exceeds the apex intensity (meaning that we've reached another peak) 
+            # 3. the intensity exceeds the apex intensity (meaning that we've reached another peak)
             # 4. we go below the threshold intensity (the desired stopping condition)
             # Note: in step 3, an alternative is to check if the intensity simply starts to increase w.r.t. the previous inspected point.
             # Such an approach may give less false positive peaks, but is very sensitive to electronic noise and to overlapping peaks.
             # When we check if the intensity has not exceeded the apex intensity, and we encounter a cluster of overlapping peaks,
             # then we will effectively consider the highest one as the true apex of the cluster and integrate the whole cluster only once.
             while p + right_shift < n-1 and mz[p+right_shift] - mz[p] < max_dist and intsy[p+right_shift] <= current_intsy and intsy[p+right_shift] > target_intsy:
                 right_shift += 1
-            if intsy[p+right_shift] > target_intsy:
+            # Get the mz values of points around left mz value of the peak boundary (which will be interpolated):
+            rx1, rx2 = mz[p+right_shift-1], mz[p+right_shift]
+            ry1, ry2 = intsy[p+right_shift-1], intsy[p+right_shift]
+            if not ry1 >= target_intsy >= ry2:
+                # warn('Failed to find the right boundary of the peak at %f (probably found an overlapping peak)' % current_mz)
                 continue
+            # Find the left boundary of the peak:
             while p - left_shift > 1 and mz[p] - mz[p-left_shift] < max_dist and intsy[p-left_shift] <= current_intsy and intsy[p-left_shift] > target_intsy:
                 left_shift += 1
-            if intsy[p-left_shift] > target_intsy:
-                continue
-            # Get the mz value actually corresponding to peak_height_fraction*current_intsy:
-            lx1, lx2 = mz[p-left_shift], mz[p-left_shift+1]  # x coordinates of points around left mz value we're looking for
+            lx1, lx2 = mz[p-left_shift], mz[p-left_shift+1]
             ly1, ly2 = intsy[p-left_shift], intsy[p-left_shift+1]
-            assert ly1 <= target_intsy <= ly2
-            rx1, rx2 = mz[p+right_shift-1], mz[p+right_shift] 
-            ry1, ry2 = intsy[p+right_shift-1], intsy[p+right_shift]
-            assert ry1 >= target_intsy >= ry2
+            if not ly1 <= target_intsy <= ly2:
+                # warn('Failed to find the left boundary of the peak at %f (probably found an overlapping peak)' % current_mz)
+                continue
+            # Interpolate the mz values actually corresponding to peak_height_fraction*current_intsy:
             lx = (target_intsy-ly1)*(lx2-lx1)/(ly2-ly1) + lx1
-            assert lx1 <= lx <= lx2
+            if not lx1 <= lx <= lx2:
+                raise RuntimeError('Failed to interpolate the left boundary mz value of the peak at %f' % current_mz)
             rx = (target_intsy-ry1)*(rx2-rx1)/(ry2-ry1) + rx1
-            assert rx1 <= rx <= rx2
+            if not rx1 <= rx <= rx2:
+                raise RuntimeError('Failed to interpolate the right boundary mz value of the peak at %f' % current_mz)
+            # Join the interpolated boundary with the actual measurements:
             x = np.hstack((lx, mz[(p-left_shift+1):(p+right_shift)], rx))
             y = np.hstack((target_intsy, intsy[(p-left_shift+1):(p+right_shift)], target_intsy))
             # Integrate the area:
             cint = np.trapz(y, x)
             cmz = np.trapz(y*x, x)/cint
             if cmz not in centroid_mz:  # intensity errors may introduce artificial peaks
                 centroid_mz.append(cmz)
@@ -481,22 +532,22 @@
         return(list(zip(centroid_mz, centroid_intensity)), list(zip(peak_mz, peak_intensity)))
 
     def resample(self, target_mz, mz_distance_threshold=0.05):
         """
         Returns a resampled spectrum with intensity values approximated
         at points given by a sorted iterable target_mz.
         The approximation is performed by a piecewise linear interpolation
-        of the spectrum intensities. The spectrum needs to be in profile mode 
+        of the spectrum intensities. The spectrum needs to be in profile mode
         in order for this procedure to work properly.
-        The spectrum is interpolated only if two target mz values closest to a 
+        The spectrum is interpolated only if two target mz values closest to a
         given target mz are closer than the specified threshold
-        This is done in order to interpolate the intensity only within peaks, not between them. 
+        This is done in order to interpolate the intensity only within peaks, not between them.
         If the surrounding mz values are further away than the threshold,
         it is assumed that the given target mz corresponds to the background and
-        there is no intensity at that point. 
+        there is no intensity at that point.
         A rule-of-thumb is to set threshold as twice the distance between
         neighboring m/z measurements.
         Large thresholds may lead to non-zero resampled intensity in the background,
         low thresholds might cause bad interpolation due to missing intensity values.
         """
         mz = [mz for mz, intsy in self.confs]
         intsy = [intsy for mz, intsy in self.confs]
@@ -519,41 +570,70 @@
             ti += 1
             y0 = y1
             y1 = intsy[ti]
             x0 = x1
             x1 = mz[ti]
             while qi < lenx and target_mz[qi] <= mz[ti]:
                 # note: maybe in this case set one of the values to zero to get a better interpolation of edges
-                if x1-x0 < mz_distance_threshold:  
+                if x1-x0 < mz_distance_threshold:
                     y[qi] = y1 + (target_mz[qi]-x1)*(y0-y1)/(x0-x1)
                 qi += 1
         return Spectrum(confs = list(zip(target_mz, y)))
 
 
     def fuzzify_peaks(self, sd, step):
         """
+        LEGACY FUNCTION. USE SELF.GAUSSIAN_SMOOTING INSTEAD.   
         Applies a gaussian filter to the peaks, effectively broadening them
         and simulating low resolution. Works in place, modifying self.
         The parameter step gives the distance between samples in m/z axis.
-        Note that after the filtering, the area below curve is equal to 1,
-        instead of the sum of 'peak' intensities!
+        After the filtering, the area below curve (not the sum of intensities!)
+        is equal to the sum of the input peak intensities.
         """
         new_mass = np.arange(self.confs[0][0] - 4*sd, self.confs[-1][0] + 4*sd, step)
-        new_intensity = np.zeros(len(new_mass))
-        lb = new_mass[0]
-        for x, y in self.confs:
-            xrnb = int((x-lb)//step)  # x's index in new_mass
-            xr = lb + step*xrnb
-            lnb = int((xr-x+4*sd)//step)   # nb of steps left of x to add gauss
-            xlb = xr - step*lnb
-            xrb = xr + step*lnb
-            xv = np.array([xlb + i*step for i in range(2*lnb + 2)])
-            nv = y*norm.pdf(xv, x, sd)
-            new_intensity[(xrnb-lnb):(xrnb+lnb+2)] += nv
-        self.confs = [(x, y) for x, y in zip(new_mass, new_intensity)]
+        A = new_mass[:,np.newaxis] - np.array([m for m,i in self.confs])
+        # we don't need to evaluate gaussians to far from their mean,
+        # from our perspective 4 standard deviations from the mean is the same
+        # as the infinity; this allows to avoid overflow as well:
+        A[np.abs(A) > 4*sd] = np.inf
+        A **= 2
+        A /= (-2*sd**2)
+        A = np.exp(A)
+        new_intensity = A @ np.array([i for m,i in self.confs])  # matrix multiplication
+        new_intensity /= (np.sqrt(2*np.pi)*sd)
+        self.set_confs(list(zip(new_mass, new_intensity)))
+
+
+    def gaussian_smoothing(self, sd=0.01, new_mz=0.01):
+        """
+        Applies a gaussian filter to the mass spectrum in order to smooth
+        it out and decrease the electronic noise.
+        Technically, each intensity measurement is replaced by a Gaussian weighted average
+        of the neighbouring intensities.  
+        As a consequence, the resolution gets decreased.
+        Parameter sd (float) controls the width of the gaussian filter.
+        Parameter new_mz (float or np.array) is the mass axis of the resulting smoothed spectrum.
+        Setting it to float generates an equally spaced mass axis with new_mz being the step length.
+        Setting it to np.array sets it as the resulting mass axis.  
+        Note that after filtering, the area below curve (not the sum of intensities!)
+        is equal to the area of the original spectrum in profile mode,
+        or the sum of the input peak intensities in centroid mode.
+        """
+        if isinstance(new_mz, float):
+            new_mz = np.arange(self.confs[0][0] - 4*sd, self.confs[-1][0] + 4*sd, new_mz)
+        assert np.all(new_mz[1:] >= new_mz[:-1]), 'The new mz axis needs to be sorted!'
+        smooth_intensity = np.zeros(new_mz.shape)
+        for mz, intsy in self.confs:
+            # smooth_intensity += intsy*np.exp(-(mz - new_mz)**2)**(1/(2*sd**2))
+            lpid, rpid = np.searchsorted(new_mz, (mz - 4*sd, mz + 4*sd))
+            peak_mz = new_mz[lpid:rpid]
+            smooth_intensity[lpid:rpid] += intsy*np.exp(-(mz - peak_mz)**2)**(1/(2*sd**2))
+        smooth_intensity /= np.sqrt(2*np.pi)*sd
+        self.set_confs(list(zip(new_mz, smooth_intensity)))
+
 
     def cut_smallest_peaks(self, removed_proportion=0.001):
         """
         Removes smallest peaks until the total removed intensity amounts
         to the given proportion of the total ion current in the spectrum.
         """
         self.confs.sort(key = lambda x: x[1], reverse=True)
@@ -584,61 +664,62 @@
         merged_bounds = []
         c_low, c_up = bounds[0]
         for b in bounds:
             if b[0] <= c:
                 pass # to be finished
 
 
-    @staticmethod
-    def filter_against_theoretical(experimental, theoreticals, margin=0.15):
+    def filter_against_other(self, others, margin=0.15):
         """
-        Remove signal from the empirical spectra which is far from theoretical.
+        Remove signal from the spectrum which is far from other spectra signal.
 
-        This method removes peaks from experimental spectrum which are outside
-        theoretical peaks +/- margin.
+        This method removes peaks from self spectrum which m/z is outside the
+        area of any peak of other spectra +/- margin. The method does not
+        modify self spectrum and returns a new instance of the filtered
+        spectrum.
 
         Parameters
         ----------
-        experimental
-            Empirical spectrum.
-        theoreticals:
-            One instance of theoretical or iterable of instances of theoretical
-            spectra.
+        self
+            Spectrum to be filtered.
+        others:
+            One instance of the spectrum against self is filtered or iterable of
+            instances of other spectra.
         margin
-            m/z radius within empirical spectrum should be left.
+            m/z radius within signal should be left.
 
         Returns
         -------
         Spectrum
-            An empirical spectrum with filtered out peaks.
+            A new spectrum with filtered out peaks.
+
         """
         try:
-            th_confs = []
-            for theoretical_spectrum in theoreticals:
-                th_confs.extend(theoretical_spectrum.confs)
-            theoretical = Spectrum()
-            theoretical.set_confs(th_confs)
+            other_confs = []
+            for other_spectrum in others:
+                other_confs.extend(other_spectrum.confs)
+            other = Spectrum(confs=other_confs)
         except TypeError:
-            theoretical = theoreticals
-        experimental_confs = experimental.confs
-        theoretical_masses = [i[0] for i in theoretical.confs]
+            other = others
+        other_masses = [i[0] for i in other.confs]
+
 
         result_confs = []
         index = 0
-        for mz, abund in experimental_confs:
-            while (index + 1 < len(theoretical_masses) and
-                   theoretical_masses[index + 1] < mz):
+        for mz, abund in self.confs:
+            while (index + 1 < len(other_masses) and
+                   other_masses[index + 1] < mz):
                 index += 1
-            if abs(mz - theoretical_masses[index]) <= margin or (
-                    index + 1 < len(theoretical_masses) and
-                    abs(mz - theoretical_masses[index + 1]) <= margin):
+            if abs(mz - other_masses[index]) <= margin or (
+                    index + 1 < len(other_masses) and
+                    abs(mz - other_masses[index + 1]) <= margin):
                 result_confs.append((mz, abund))
-        new_spectrum = Spectrum(label=experimental.label)
-        new_spectrum.confs = result_confs
-        return new_spectrum
+
+        result_spectrum = Spectrum(confs=result_confs, label=self.label)
+        return result_spectrum
 
     def plot(self, show = True, profile=False, linewidth=1, **plot_kwargs):
         """
         Plots the spectrum.
         The keyword argument show is retained for backwards compatibility.
         """
         import matplotlib.pyplot as plt
@@ -651,15 +732,15 @@
                        linewidth=linewidth, **plot_kwargs)
         if show:
             plt.show()
 
     @staticmethod
     def plot_all(spectra, show=True, profile=False, cmap=None, **plot_kwargs):
         """
-        Shows the supplied list of spectra on a single plot. 
+        Shows the supplied list of spectra on a single plot.
         """
         import matplotlib.pyplot as plt
         import matplotlib.cm as cm
         if not cmap:
             colors = cm.rainbow(np.linspace(0, 1, len(spectra)))
             colors =  [[0, 0, 0, 0.8]] + [list(x[:3]) + [0.6] for x in colors]
         else:
@@ -676,19 +757,38 @@
         plt.legend(loc=0, ncol=1)
         if show:
             plt.show()
 
 
 if __name__=="__main__":
     import matplotlib.pyplot as plt
-    S = Spectrum(formula="C2H5OH", threshold=0.)
+    from copy import deepcopy
+    S = Spectrum(formula="C2H5OH", threshold=0.01)
+
+    S.add_chemical_noise(4, 0.2)
     S.plot()
-    S.fuzzify_peaks(0.1, 0.01)
-    S.plot(profile=True)
-    
+
+    sd = 0.01
+    C = deepcopy(S)
+    C = C*(np.sqrt(2*np.pi)*sd)**-1
+    S1 = deepcopy(S)
+    S.gaussian_smoothing(0.01,  0.001)
+    S1.fuzzify_peaks(0.01, 0.001)
+    S.plot(profile=True, show=False)
+    S1.plot(profile=True, show=False)
+    C.plot(show=False)
+    plt.show()
+
+    T = Spectrum(confs=[(1, 1)])
+    T.gaussian_smoothing(0.01, np.array([0.96, 0.97, 0.98, 0.99, 1, 1.01, 1.02]))
+    T.plot(profile=True, show=False)
+    T = Spectrum(confs=[(1, 1)])
+    T.gaussian_smoothing(0.01, 0.001)
+    T.plot(profile=True)
+
     target_mz = np.linspace(45, 56, num=100)
     R = S.resample(target_mz)
     plt.subplot(221)
     S.plot(show=False, profile=True)
     plt.subplot(222)
     R.plot(show=False, profile=True)
     plt.subplot(223)
```

### Comparing `masserstein-0.9.0/masserstein.egg-info/PKG-INFO` & `masserstein-1.0.0/masserstein.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: masserstein
-Version: 0.9.0
+Version: 1.0.0
 Summary: A library for analysis of Mass Spectrometry data using the Wasserstein metric
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: UNKNOWN
-Keywords: mass spectrrometry spectral deconvolution
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Keywords: mass spectrometry spectral deconvolution
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >2.7, >=3.6, <4
 Provides-Extra: graphics
+License-File: LICENSE
```

### Comparing `masserstein-0.9.0/setup.py` & `masserstein-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.9.0',  # Required
+    version='1.0.0',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='A library for analysis of Mass Spectrometry data using the Wasserstein metric',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -93,15 +93,15 @@
     #
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
 
         # Indicate who your project is intended for
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
@@ -112,21 +112,25 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+
+        'License :: OSI Approved :: MIT License',
     ],
 
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a string of words separated by whitespace, not a list.
-    keywords='mass spectrrometry spectral deconvolution',  # Optional
+    keywords='mass spectrometry spectral deconvolution',  # Optional
 
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
@@ -137,23 +141,23 @@
     packages = ['masserstein'],
 
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. If you
     # do not support Python 2, you can simplify this to '>=3.5' or similar, see
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, <4',
+    python_requires='>2.7, >=3.6, <4',
 
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['IsoSpecPy', 'numpy', 'scipy', 'pulp'],  
+    install_requires=['IsoSpecPy', 'numpy', 'scipy', 'pulp', 'tqdm'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

