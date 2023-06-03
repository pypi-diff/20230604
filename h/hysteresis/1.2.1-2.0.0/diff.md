# Comparing `tmp/hysteresis-1.2.1.tar.gz` & `tmp/hysteresis-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hysteresis-1.2.1.tar", last modified: Sun Oct 30 08:09:37 2022, max compression
+gzip compressed data, was "hysteresis-2.0.0.tar", last modified: Sat Jun  3 23:07:41 2023, max compression
```

## Comparing `hysteresis-1.2.1.tar` & `hysteresis-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2022-10-30 08:09:37.263130 hysteresis-1.2.1/
-drwxrwxrwx   0        0        0        0 2022-10-30 08:09:37.263130 hysteresis-1.2.1/Hysteresis/
--rw-rw-rw-   0        0        0      541 2022-10-02 03:48:05.000000 hysteresis-1.2.1/Hysteresis/__init__.py
--rw-rw-rw-   0        0        0    40161 2022-10-02 05:39:23.000000 hysteresis-1.2.1/Hysteresis/baseClass.py
--rw-rw-rw-   0        0        0     5766 2022-10-30 08:08:02.000000 hysteresis-1.2.1/Hysteresis/baseFuncs.py
--rw-rw-rw-   0        0        0     4152 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/climate.py
--rw-rw-rw-   0        0        0     2732 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/compare.py
--rw-rw-rw-   0        0        0    13248 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/data.py
--rw-rw-rw-   0        0        0     4606 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/defaultDataFuncs.py
--rw-rw-rw-   0        0        0     4888 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/defaultPlotFuncs.py
--rw-rw-rw-   0        0        0     1166 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/env.py
--rw-rw-rw-   0        0        0    12009 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/envelope.py
-drwxrwxrwx   0        0        0        0 2022-10-30 08:09:37.263130 hysteresis-1.2.1/Hysteresis/plotSpecial/
--rw-rw-rw-   0        0        0       75 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/plotSpecial/__init__.py
--rw-rw-rw-   0        0        0    12440 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/plotSpecial/animate.py
--rw-rw-rw-   0        0        0    15115 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/plotSpecial/core.py
--rw-rw-rw-   0        0        0     5584 2022-06-19 02:48:59.000000 hysteresis-1.2.1/Hysteresis/plotSpecial/guiPlot.py
--rw-rw-rw-   0        0        0     7301 2022-10-02 06:10:12.000000 hysteresis-1.2.1/Hysteresis/protocol.py
--rw-rw-rw-   0        0        0    12105 2022-10-30 07:00:17.000000 hysteresis-1.2.1/Hysteresis/resample.py
-drwxrwxrwx   0        0        0        0 2022-10-30 08:09:37.263130 hysteresis-1.2.1/Hysteresis.egg-info/
--rw-rw-rw-   0        0        0     6067 2022-10-30 08:09:37.000000 hysteresis-1.2.1/Hysteresis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2022-10-30 08:09:37.000000 hysteresis-1.2.1/Hysteresis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-30 08:09:37.000000 hysteresis-1.2.1/Hysteresis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-10-30 08:09:37.000000 hysteresis-1.2.1/Hysteresis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-10-30 08:09:37.000000 hysteresis-1.2.1/Hysteresis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6067 2022-10-30 08:09:37.263130 hysteresis-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     5609 2022-04-04 00:12:03.000000 hysteresis-1.2.1/README.md
--rw-rw-rw-   0        0        0     1096 2020-05-27 03:09:59.000000 hysteresis-1.2.1/license.txt
--rw-rw-rw-   0        0        0       42 2022-10-30 08:09:37.263130 hysteresis-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      795 2022-10-30 08:09:00.000000 hysteresis-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:07:41.111264 hysteresis-2.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-03 23:07:41.077264 hysteresis-2.0.0/Hysteresis/
+-rw-rw-rw-   0        0        0      393 2023-05-29 06:58:48.000000 hysteresis-2.0.0/Hysteresis/__init__.py
+-rw-rw-rw-   0        0        0     5762 2023-05-29 06:59:11.000000 hysteresis-2.0.0/Hysteresis/baseFuncs.py
+-rw-rw-rw-   0        0        0     4128 2023-05-29 06:57:38.000000 hysteresis-2.0.0/Hysteresis/climate.py
+-rw-rw-rw-   0        0        0     2727 2023-05-29 06:57:27.000000 hysteresis-2.0.0/Hysteresis/compare.py
+-rw-rw-rw-   0        0        0    42368 2023-06-03 22:27:08.000000 hysteresis-2.0.0/Hysteresis/curve.py
+-rw-rw-rw-   0        0        0    13244 2023-05-29 05:23:43.000000 hysteresis-2.0.0/Hysteresis/data.py
+-rw-rw-rw-   0        0        0     4542 2023-05-28 01:22:30.000000 hysteresis-2.0.0/Hysteresis/defaultDataFuncs.py
+-rw-rw-rw-   0        0        0     4879 2023-05-29 05:00:45.000000 hysteresis-2.0.0/Hysteresis/defaultPlotFuncs.py
+-rw-rw-rw-   0        0        0     1133 2023-05-25 07:01:28.000000 hysteresis-2.0.0/Hysteresis/env.py
+-rw-rw-rw-   0        0        0    11795 2023-05-29 07:00:47.000000 hysteresis-2.0.0/Hysteresis/envelope.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:07:41.109262 hysteresis-2.0.0/Hysteresis/plotSpecial/
+-rw-rw-rw-   0        0        0       75 2022-10-30 07:42:02.000000 hysteresis-2.0.0/Hysteresis/plotSpecial/__init__.py
+-rw-rw-rw-   0        0        0    12531 2023-06-03 21:17:34.000000 hysteresis-2.0.0/Hysteresis/plotSpecial/animate.py
+-rw-rw-rw-   0        0        0    14981 2023-05-29 07:14:01.000000 hysteresis-2.0.0/Hysteresis/plotSpecial/core.py
+-rw-rw-rw-   0        0        0     5584 2022-10-30 07:42:02.000000 hysteresis-2.0.0/Hysteresis/plotSpecial/guiPlot.py
+-rw-rw-rw-   0        0        0     7017 2023-05-29 07:00:30.000000 hysteresis-2.0.0/Hysteresis/protocol.py
+-rw-rw-rw-   0        0        0    12094 2023-05-29 07:00:04.000000 hysteresis-2.0.0/Hysteresis/resample.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:07:41.083302 hysteresis-2.0.0/Hysteresis.egg-info/
+-rw-rw-rw-   0        0        0     6075 2023-06-03 23:07:40.000000 hysteresis-2.0.0/Hysteresis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      943 2023-06-03 23:07:40.000000 hysteresis-2.0.0/Hysteresis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 23:07:40.000000 hysteresis-2.0.0/Hysteresis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-03 23:07:40.000000 hysteresis-2.0.0/Hysteresis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 23:07:40.000000 hysteresis-2.0.0/Hysteresis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6075 2023-06-03 23:07:41.111264 hysteresis-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5609 2022-04-04 00:12:03.000000 hysteresis-2.0.0/README.md
+-rw-rw-rw-   0        0        0     1096 2020-05-27 03:09:59.000000 hysteresis-2.0.0/license.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 23:07:41.111264 hysteresis-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-06-03 23:06:34.000000 hysteresis-2.0.0/setup.py
```

### Comparing `hysteresis-1.2.1/Hysteresis/baseClass.py` & `hysteresis-2.0.0/Hysteresis/curve.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,275 @@
 import numpy as np
 from hysteresis import data
 import hysteresis.env as env
 import matplotlib.pyplot as plt
 
 
-
-# =============================================================================
-# Curve objects
-# =============================================================================
-
-class CurveBase:
-    
-    __array_ufunc__ = None
+class CurvePlotter:
+    """
+    The Curve plotter class is used to define plotting behaviour that is common 
+    to all types of curves. It is generally ment to be inherited from and not
+    used directly. 
     """
-    The curve base object represents a generic xy curve with no limitations.
     
-    All other curves inherit from the CurveBase class. It has access to methods
-    all other curves should have access to. This uncludes plotting 
-    functionality, slope functions, area functions, and displacement functions.
     
-    """
+    def plot(self, showReversals = False, showPeaks = False, labelReversals = None,
+             **kwargs):
+        """
+        Used the plot function to make a xy plot of the curve. The default 
+        plot function uses matplotlib for plotting, and returns the plotted
+        line.
+        
+        Parameters
+        ----------
+        showReversals : bool
+            A switch that specifics if cycle reversal points should be plotted.
+        showPeaks : bool
+            A switch that specifics if the detected peak values should be plotted.
+        labelReversals : list or 'all', optional
+            A list of the cycles to be labled. 
+            A value of 'all' can also be specified, in which case all cucles will be plotted.
+            The default is [], which labels no cycles    
+        kwargs : list, optional
+            Any additional keyword arguements will be passed to the matplotlib
+            plot function. This can be used to custize char appearance.            
+
+        Outputs
+        -------
+        Matplotlib Line
+
+        """
+        
+        if labelReversals is None:
+            labelReversals = []
+
+        return self.plotFunction(self.xy, showReversals, showPeaks, self.peakIndexes, 
+                                 self.reversalIndexes, labelReversals,
+                                 **kwargs)
+                
+    def plotVsIndex(self, showReversals = False, showPeaks = False, 
+                     labelReversals = None, **kwargs):
+        """
+        Used the plot function to make a plot of each x point vs. it's index.
+        This can be useful for understanding how x values change over time.
+        The default plot function uses matplotlib for plotting, and returns 
+        the plotted line.
+        
+        Parameters
+        ----------
+        showReversals : bool
+            A switch that specifics if cycle reversal points should be plotted.
+        showPeaks : bool
+            A switch that specifics if the detected peak values should be plotted.
+        labelReversals : list or 'all', optional
+            A list of the cycles to be labled. 
+            A value of 'all' can also be specified, in which case all cucles will be plotted.
+            The default is [], which labels no cycles     
+        kwargs : list, optional
+            Any additional keyword arguements will be passed to the matplotlib
+            plot function. This can be used to custize char appearance.
+            
+        """           
+        
+        if labelReversals is None:
+            labelReversals = []
+                
+        x = np.arange(0,len(self.xy[:,0]))
+        y = self.xy[:,0]
+        
+        xy = np.column_stack([x,y])
+                    
+        return self.plotFunction(xy, showReversals, showPeaks, self.peakIndexes, 
+                                 self.reversalIndexes, labelReversals, **kwargs)
+
+    def plotLoadProtocol(self, comparisonProtocol = [], **kwargs):
+        """
+        Plots the peak x values for each cycle in a curve.
+        An additional load protocol can be provided, so the user can comapare the
+        curves peak x points against an expected load protocol.
+        
+        The default plot function uses matplotlib for plotting, and returns 
+        the plotted line.
+        
+        Parameters
+        ----------
+        comparisonProtocol : array
+            A load protocol that will be plotted on the same figure. Useful
+            for comparing the curves load protcol to the input protocol.
+        kwargs : list, optional
+            Any additional keyword arguements will be passed to the matplotlib
+            plot function. This can be used to custize char appearance.
+        """           
+        showReversals = False
+        showPeaks = False
+        labelCycles = []
+        y = self.loadProtocol
+        x = np.arange(0,len(y))
+        xy = np.column_stack([x,y])
+        
+        line = self.plotFunction(xy, showReversals, showPeaks, labelCycles, **kwargs)
+        
+        if len(comparisonProtocol) != 0:
+            line2 = plt.plot(comparisonProtocol)
+            return [line, line2]
+
+        return line
     
-    def __init__(self, XYData, xunit = '', yunit = ''):
+    def plotSlope(self,  showReversals = False, showPeaks = False, 
+                  labelReversals = None, **kwargs):
         """
+        Used the plot function to make a xy plot of the slope at each point of 
+        the curve. The slope is calcualted using the slope function, which
+        uses a centeral finite difference scheme by default.
+        plot function uses matplotlib for plotting, and returns the plotted
+        line.
+        
         Parameters
         ----------
-        XYData : array
-            The input array of XY date for the curve. A list [x,y] can also be 
-            passed into the function.
-        xunit : str, optional
-            The units on the x axis. The default is ''.
-        yunit : str, optional
-            The units on the y axis. The default is ''.
+        showReversals : bool
+            A switch that specifics if cycle reversal points should be plotted.
+        showPeaks : bool
+            A switch that specifics if the detected peak values should be plotted.
 
+        labelReversals : list or 'all', optional
+            A list of the cycles to be labled. 
+            A value of 'all' can also be specified, in which case all cucles will be plotted.
+            The default is [], which labels no cycles  
+        kwargs : list, optional
+            Any additional keyword arguements will be passed to the matplotlib
+            plot function. This can be used to custize char appearance.
+        """          
+        
+        xy = np.column_stack([self.xy[:,0], self.slope])
+        
+        if labelReversals is None:
+            labelReversals = []
+    
+        return self.plotFunction(xy, showReversals, showPeaks, self.peakIndexes, 
+                                 self.reversalIndexes, labelReversals,
+                                 **kwargs)    
+    
+    def plotArea(self,  showReversals = False, showPeaks = False, 
+                 labelReversals = None, **kwargs):
         """
+        Used the plot function to make a xy plot of the area under each point of 
+        the curve. The area is calculated using the area function, which
+        uses the midpoint rule by default.
+        The plot function uses matplotlib for plotting, and returns the plotted
+        line.
         
-        self.xy = self._parseXY(XYData)
-        self.Npoints = len(self.xy[:,0])
+        Parameters
+        ----------
+        showReversals : bool
+            A switch that specifics if cycle reversal points should be plotted.
+        showPeaks : bool
+            A switch that specifics if the detected peak values should be plotted.
+
+        labelReversals : list or 'all', optional
+            A list of the cycles to be labled. 
+            A value of 'all' can also be specified, in which case all cucles 
+            will be plotted.
+            The default is [], which labels no cycles
+        kwargs : list, optional
+            Any additional keyword arguements will be passed to the matplotlib
+            plot function. This can be used to custize char appearance.            
+            
+        """       
         
-        # The function to be used to calcualte area. These can be overwritten
-        self.areaFunction = env.environment.fArea
-        self.slopeFunction = env.environment.fslope
-        self.lengthFunction = env.environment.flength
-        self.plotFunction = env.environment.fplot
+        if labelReversals is None:
+            labelReversals = []
+            
+        xy = np.column_stack([self.xy[:,0], self.area])
+
+        return self.plotFunction(xy, showReversals, showPeaks, self.peakIndexes, 
+                                 self.reversalIndexes, labelReversals,
+                                 **kwargs)    
+                        
+    def plotCumArea(self,  showReversals = False, showPeaks = False, 
+                    labelReversals = None, cumulativeDisp = True, **kwargs):
+        """
+        Used the plot function to make a xy plot of cumulative area at each
+        point of the curve. The cumulative area is a summation of the areas up
+        to the point in question.
+        The area is calculated using the area function, which uses the midpoint 
+        rule by default.
+        The plot function uses matplotlib for plotting, and returns the plotted
+        line.
         
-        self.initializeFig = env.environment.finit
-        self.showCycles = env.environment.fcycles
+        Parameters
+        ----------
+        showReversals : bool
+            A switch that specifics if cycle reversal points should be plotted.
+        showPeaks : bool
+            A switch that specifics if the detected peak values should be plotted.
+        labelReversals : list or 'all', optional
+            A list of the cycles to be labled. 
+            A value of 'all' can also be specified, in which case all cucles will be plotted.
+            The default is [], which labels no cycles
+        kwargs : list, optional
+            Any additional keyword arguements will be passed to the matplotlib
+            plot function. This can be used to custize char appearance.
         
-        self.colorDict = {0:'C0', 1:'C1', 2:'C3'}
+        """   
         
-        self.xunit = xunit
-        self.yunit = yunit
+        if labelReversals is None:
+            labelReversals = []
+            
+        # We get the cumulative displacement and area
+        if cumulativeDisp:
+            x = self.getCumDisp()
+        else:
+            x = self.xy[:,0]
+        y = self.getCumArea()
+        xy = np.column_stack([x,y])
+
+        return self.plotFunction(xy, showReversals, showPeaks, self.peakIndexes, 
+                                 self.reversalIndexes, labelReversals,
+                                 **kwargs)    
+             
+    def initFig(self, xlims = None, ylims = None):
+        """       
+        Initializes the plot using the default rules.
+        """
         
-        self.peakIndexes = None
+        if xlims is None:
+            xlims = []
+        
+        if ylims is None:
+            ylims = []
+            
+        return self.initializeFig(xlims, ylims)
+
+
+    def _plot_curves(self, curves, curveInds, colorCycles, **kwargs):
+        """
+        Used by plotCycles and plotSubCycles
+        """
+        Ncolor = len(colorCycles) 
+        lines = []
+        # If the list has content, get the cycles to plot, otherwise plot everything
+        if curveInds is not None:
+            curves = [curves[ii] for ii in curveInds]
+            
+        for ii, curve in enumerate(curves):
+            c = colorCycles[int(ii % Ncolor)]
+            line, = plt.plot(curve.xy[:,0], curve.xy[:,1], c=c, **kwargs)
+            lines.append(line)
+        return lines     
+
+class CurveOperations:
+    
+    """
+    The Curve operations class is used to define operations that all curves
+    will have. This includes features such iteration, mathematical operations
+    like addition or multiplaction, and setting/getting items.
+    """
+    
+    __array_ufunc__ = None
+
     
     @property
     def y(self):
         return self.xy[:,1]
     
     @property
     def x(self):
@@ -83,15 +296,15 @@
         return type(self)
     
     def _convertToCurve(self, other):
         """
         Converts non-hysteresis datatypes 
         """
         if isinstance(other, np.ndarray):
-            return CurveBase(other)
+            return Curve(other)
 
     def __add__(self, other):
         """ Enables addition of curve x values"""
         Instance = self._getInstance()
         operand = _getOperand(other)
         x = self.xy[:,0]
         y = self.xy[:,1]+operand        
@@ -109,14 +322,20 @@
     def __rsub__(self, other):
         Instance = self._getInstance()
         operand = _getOperand(other)
         x = self.xy[:,0]
         y = operand - self.xy[:,1]   
         
         return Instance(np.column_stack([x,y]))
+
+    def __neg__(self):
+        Instance = self._getInstance()
+        x =  self.xy[:,0]
+        y = -self.xy[:,1]           
+        return Instance(np.column_stack([x,y]))
     
     def __mul__(self, other):
         """
         It would be useful of having a hystresis base state, then copying that over.
         """
         # Get the current instance of curve
         Instance = self._getInstance()
@@ -139,15 +358,61 @@
         # Get the current instance of curve
         Instance = self._getInstance()
         operand = _getOperand(other)    
         x = self.xy[:,0]
         y = operand / self.xy[:,1]
         
         return Instance(np.column_stack([x,y]))
+
+class Curve(CurveOperations, CurvePlotter):
     
+    """
+    The curve base object represents a generic xy curve with no limitations.
+    
+    All other curves inherit from the CurveBase class. It has access to methods
+    all other curves should have access to. This uncludes plotting 
+    functionality, slope functions, area functions, and displacement functions.
+    
+    """
+    
+    colorCycles = ['C0', 'C0', 'C1', 'C1']
+    reversalIndexes = np.array([0,-1])
+    
+    
+    def __init__(self, XYData, xunit = '', yunit = ''):
+        """
+        Parameters
+        ----------
+        XYData : array
+            The input array of XY date for the curve. A list [x,y] can also be 
+            passed into the function.
+        xunit : str, optional
+            The units on the x axis. The default is ''.
+        yunit : str, optional
+            The units on the y axis. The default is ''.
+
+        """
+        
+        self.xy = self._parseXY(XYData)
+        self.Npoints = len(self.xy[:,0])
+        
+        # The function to be used to calcualte area. These can be overwritten
+        self.areaFunction = env.environment.fArea
+        self.slopeFunction = env.environment.fslope
+        self.lengthFunction = env.environment.flength
+        self.plotFunction = env.environment.fplot
+        
+        self.initializeFig = env.environment.finit
+        self.showCycles = env.environment.fcycles
+        
+        self.xunit = xunit
+        self.yunit = yunit
+        
+        self.peakIndexes = None
+        
     def setArea(self):
         """ sets the area under each point of the curve using the area function"""
         self.area = self.areaFunction(self.xy)
         return self.area
     
     def getCumDisp(self):
         """ 
@@ -218,15 +483,15 @@
 
     def setPeaks(self, peakDist = 2, peakWidth = None, peakProminence = None):
         """
         Finds the indexes of max and min points, then stores them.
         """
         
         y = self.xy[:,1]
-        peakIndexes = data.getCycleIndicies(y, peakDist, peakWidth, peakProminence)        
+        peakIndexes = data.getCycleIndexes(y, peakDist, peakWidth, peakProminence)        
         self.peakIndexes = peakIndexes
         
         xy = self.xy
         if xy[peakIndexes[0],1] < xy[peakIndexes[1],1]:
             self.minIndexes = peakIndexes[0::2]
             self.maxIndexes = peakIndexes[1::2]
         else:
@@ -236,210 +501,14 @@
     def getPeakxy(self,):
         
         if self.peakIndexes is not None:
             return self.xy[self.peakIndexes]
         else:
             raise Exception('No peaks have been set')
         
-    
-    def plot(self, plotCycles = False, plotPeaks = False, labelCycles = [],
-             **kwargs):
-        """
-        Used the plot function to make a xy plot of the curve. The default 
-        plot function uses matplotlib for plotting, and returns the plotted
-        line.
-        
-        Parameters
-        ----------
-        plotCycles : bool
-            A switch that specifics if cycle reversal points should be plotted.
-        plotPeaks : bool
-            A switch that specifics if the detected peak values should be plotted.
-        labelCycles : list or 'all', optional
-            A list of the cycles to be labled. 
-            A value of 'all' can also be specified, in which case all cucles will be plotted.
-            The default is [], which labels no cycles    
-        kwargs : list, optional
-            Any additional keyword arguements will be passed to the matplotlib
-            plot function. This can be used to custize char appearance.            
-
-
-
-        Outputs
-        -------
-        Matplotlib Line
-
-        """        
-        x = self.xy[:,0]
-        y = self.xy[:,1]
-                    
-        return self.plotFunction(self, x ,y, plotCycles, plotPeaks, labelCycles,
-                                 **kwargs)
-                
-    def plotVsIndex(self, plotCycles = False, plotPeaks = False, 
-                     labelCycles = [], **kwargs):
-        """
-        Used the plot function to make a plot of each x point vs. it's index.
-        This can be useful for understanding how x values change over time.
-        The default plot function uses matplotlib for plotting, and returns 
-        the plotted line.
-        
-        Parameters
-        ----------
-        plotCycles : bool
-            A switch that specifics if cycle reversal points should be plotted.
-        plotPeaks : bool
-            A switch that specifics if the detected peak values should be plotted.
-
-        labelCycles : list or 'all', optional
-            A list of the cycles to be labled. 
-            A value of 'all' can also be specified, in which case all cucles will be plotted.
-            The default is [], which labels no cycles     
-        kwargs : list, optional
-            Any additional keyword arguements will be passed to the matplotlib
-            plot function. This can be used to custize char appearance.
-            
-        """           
-        
-        x = np.arange(0,len(self.xy[:,0]))
-        y = self.xy[:,0]
-                    
-        return self.plotFunction(self, x ,y, plotCycles, plotPeaks, labelCycles, **kwargs)
-
-    def plotLoadProtocol(self, comparisonProtocol = [], **kwargs):
-        """
-        Plots the peak x values for each cycle in a curve.
-        An additional load protocol can be provided, so the user can comapare the
-        curves peak x points against an expected load protocol.
-        
-        The default plot function uses matplotlib for plotting, and returns 
-        the plotted line.
-        
-        Parameters
-        ----------
-        comparisonProtocol : array
-            A load protocol that will be plotted on the same figure. Useful
-            for comparing the curves load protcol to the input protocol.
-        kwargs : list, optional
-            Any additional keyword arguements will be passed to the matplotlib
-            plot function. This can be used to custize char appearance.
-        """           
-        plotCycles = False
-        plotPeaks = False
-        labelCycles = []
-        y = self.loadProtocol
-        x = np.arange(0,len(y))
-                
-        line = self.plotFunction(self, x ,y, plotCycles, plotPeaks, labelCycles, **kwargs)
-        
-        if len(comparisonProtocol) != 0:
-            line2 = plt.plot(comparisonProtocol)
-            return [line, line2]
-
-        return line
-    
-    def plotSlope(self,  plotCycles = False, plotPeaks = False, 
-                  labelCycles = [], **kwargs):
-        """
-        Used the plot function to make a xy plot of the slope at each point of 
-        the curve. The slope is calcualted using the slope function, which
-        uses a centeral finite difference scheme by default.
-        plot function uses matplotlib for plotting, and returns the plotted
-        line.
-        
-        Parameters
-        ----------
-        plotCycles : bool
-            A switch that specifics if cycle reversal points should be plotted.
-        plotPeaks : bool
-            A switch that specifics if the detected peak values should be plotted.
-
-        labelCycles : list or 'all', optional
-            A list of the cycles to be labled. 
-            A value of 'all' can also be specified, in which case all cucles will be plotted.
-            The default is [], which labels no cycles  
-        kwargs : list, optional
-            Any additional keyword arguements will be passed to the matplotlib
-            plot function. This can be used to custize char appearance.
-        """          
-        
-        x = self.xy[:,0]
-        y = self.slope
-
-        return self.plotFunction(self, x ,y, plotCycles, plotPeaks, labelCycles, **kwargs)
-                
-    def plotArea(self,  plotCycles = False, plotPeaks = False, labelCycles = [], **kwargs):
-        """
-        Used the plot function to make a xy plot of the area under each point of 
-        the curve. The area is calculated using the area function, which
-        uses the midpoint rule by default.
-        The plot function uses matplotlib for plotting, and returns the plotted
-        line.
-        
-        Parameters
-        ----------
-        plotCycles : bool
-            A switch that specifics if cycle reversal points should be plotted.
-        plotPeaks : bool
-            A switch that specifics if the detected peak values should be plotted.
-
-        labelCycles : list or 'all', optional
-            A list of the cycles to be labled. 
-            A value of 'all' can also be specified, in which case all cucles will be plotted.
-            The default is [], which labels no cycles
-        kwargs : list, optional
-            Any additional keyword arguements will be passed to the matplotlib
-            plot function. This can be used to custize char appearance.            
-            
-        """       
-        
-        x = self.xy[:,0]
-        y = self.area
-
-        return self.plotFunction(self, x ,y, plotCycles, plotPeaks, labelCycles, **kwargs)  
-                        
-    def plotCumArea(self,  plotCycles = False, plotPeaks = False, labelCycles = [], **kwargs):
-        """
-        Used the plot function to make a xy plot of cumulative area at each
-        point of the curve. The cumulative area is a summation of the areas up
-        to the point in question.
-        The area is calculated using the area function, which uses the midpoint 
-        rule by default.
-        The plot function uses matplotlib for plotting, and returns the plotted
-        line.
-        
-        Parameters
-        ----------
-        plotCycles : bool
-            A switch that specifics if cycle reversal points should be plotted.
-        plotPeaks : bool
-            A switch that specifics if the detected peak values should be plotted.
-        labelCycles : list or 'all', optional
-            A list of the cycles to be labled. 
-            A value of 'all' can also be specified, in which case all cucles will be plotted.
-            The default is [], which labels no cycles
-        kwargs : list, optional
-            Any additional keyword arguements will be passed to the matplotlib
-            plot function. This can be used to custize char appearance.
-        
-        """   
-        
-        # We get the cumulative displacement and area
-        x = self.getCumDisp()
-        y = self.getCumArea()
-
-        self.plotFunction(self, x ,y, plotCycles, plotPeaks, labelCycles, **kwargs)  
-             
-    def initFig(self, xlims = [], ylims = []):
-        """       
-        Initializes the plot using the default rules.
-        """        
-        
-        return self.initializeFig(xlims, ylims)
-
 def _getOperand(curve):
     """
     Gets the operand (what data the function acts on) for operation functions
     (+,-,*,/)
     The data used in these functions depends on the input given.
     
     """
@@ -452,21 +521,15 @@
             operand = curve
         elif 2 == len(curve.shape) and curve.shape[-1] == 2: # if 2D array
             operand = curve[:,1]
         else: # if 1D array
             raise Exception(f'{curve.shape[-1]}D curve give, only 1 or 2D supported')
     return operand
 
-
-# =============================================================================
-# 
-# =============================================================================
-
-
-class Hysteresis(CurveBase):
+class Hysteresis(Curve):
     """
     Hysteresis objects are those that have at least one reversal point in 
     their data. Reversal points are those where the x axis changes direction.
     
     The hysteresis object has a number of functions that help find the reversal
     points in the x data of the curve.
     
@@ -506,21 +569,21 @@
         Can be turned off for performance reasons.    
         
     """
     
     def __init__(self, XYData, revDist = 2, revWidth = None, revProminence = None,
                  setCycles = True, setArea = True, setSlope = True, **kwargs):
  
-        CurveBase.__init__(self, XYData, **kwargs)
+        Curve.__init__(self, XYData, **kwargs)
         # self.setReversalPropreties(revDist, revWidth, revProminence)
         self._setStatePropreties(revDist, revWidth, revProminence,
                                  setCycles, setArea, setSlope)
         
         #TODO Create warning if cycles don't make sense.
-        self.cycles = None
+        self.cycles:list[SimpleCurve] = None
         if setCycles == True:
             self.setReversalIndexes(revDist, revWidth, revProminence)
             self.setCycles()
         
         if setArea ==True:
             self.setArea()
         if setSlope ==True:
@@ -555,27 +618,24 @@
         Sets the propreties that are used to caculate where reversal points occur.
         These are used if we want to copy new classes using the same parameters.
         """
         
         return [self.revDist, self.revWidth, self.revProminence,
                 self._setCycles, self._setArea, self._setSlope]
         
-        
     def setReversalIndexes(self, revDist = 2, revWidth = None, 
                            revProminence = None, **kwargs):
-        """ Finds the location of the reversal points
+        """ 
+        Finds the location of the reversal points
         """
-        
-        # Deprication waring
-        findPeakKwargs(**kwargs)
        
         self.setReversalPropreties(revDist, revWidth, revProminence)
         
         x = self.xy[:,0]
-        self.reversalIndexes = data.getCycleIndicies(x, revDist, revWidth, revProminence)
+        self.reversalIndexes = data.getCycleIndexes(x, revDist, revWidth, revProminence)
         self.loadProtocol = x[self.reversalIndexes]
 
     def getReversalxy(self):
         """
         Gets the reversal xy indexes
         """
         return self.xy[self.reversalIndexes]
@@ -586,23 +646,23 @@
         xy = self.xy
         indices = self.reversalIndexes
         NIndex = len(indices) - 1
         
         Cycles = [None]*NIndex
         for ii in range(NIndex):
             # I forget why we overshoot the cycles here by one
-            Cycles[ii] = SimpleCycle(xy[indices[ii]:(indices[ii+1]+1), :])
+            Cycles[ii] = SimpleCurve(xy[indices[ii]:(indices[ii+1]+1), :])
                        
-        self.cycles = Cycles
+        self.cycles:list[SimpleCurve] = Cycles
         self.NCycles = NIndex
         self.NCycles = len(Cycles)
     
-    def getCycles(self, Indicies):
-        """ Returns a list of cycles given a list of indicies"""
-        Cycles = [self.cycles[index] for index in Indicies]
+    def getCycles(self, Indexes):
+        """ Returns a list of cycles given a list of indexes"""
+        Cycles = [self.cycles[index] for index in Indexes]
         return Cycles      
     
     def getCycle(self, Index):
         """ Returns a list of cycles given a input index"""
         return self.cycles[Index]
 
     def setCycleNetAreas(self):
@@ -614,15 +674,15 @@
             
         self.CycleAreas = areas
 
     def setNetArea(self):
         """ Sets the net area of the whole Hysteresis """
         self.NetArea = np.sum(self.area)
 
-    def plotCycle(self, Index, plotPeaks = False, **kwargs):
+    def plotCycle(self, Index, showPeaks = False, **kwargs):
         
         """
         Plots the xy values of a single cycle.
         
         Parameters
         ----------
         Index : int
@@ -631,65 +691,56 @@
             A switch that specifics if the detected peak values should be plotted.
         kwargs : list, optional
             Any additional keyword arguements will be passed to the matplotlib
             plot function. This can be used to custize char appearance.            
         """
         
         Cycle = self.cycles[Index]
-        return Cycle.plot(plotPeaks = plotPeaks, **kwargs)
+        return Cycle.plot(showPeaks = showPeaks, **kwargs)
 
-    def plotCycles(self, cycleIndexes = [], plotCycles = False, plotPeaks = False, 
-                    labelCycles = [], Cycles = [], **kwargs):
+    def plotCycles(self, cycleIndexes:list = None, showReversals = False, showPeaks = False, 
+                    labelReversals:list = None, colorCycles:list = None, **kwargs):
         """
         Plots the xy values of a several cycles on the same figure.
         If no list is provided, every cycle will be plotted.
         
         Parameters
         ----------
         cycleIndexes : list of int
-            A list of the cycles to be plotted.
-        plotCycles : bool
+            A list of the cycles to be plotted. By default everything is plotted.
+        showReversals : bool
             A switch that specifics if cycle reversal points should be plotted.            
-        plotPeaks : bool
+        showPeaks : bool
             A switch that specifics if the detected peak values should be plotted.
+        labelReversals : list of int, or 'all'
+            A list of the integers which can be used to label certain reversal points
+            on the graph. If no lis is provided then no reversal points are labeled.
+            If 'all' is provided, then all points will be labeled
+        colorCycles : list of str
+            A list of matplotlib color labels to use for the cycle color. The cycles
+            will follow the colours used, the wrap back to the start of the list if there
+            are more cycles than entries provided in the color Cycles.            
         kwargs : list, optional
             Any additional keyword arguements will be passed to the matplotlib
             plot function. This can be used to custize char appearance.            
-        """
-        if len(Cycles) !=0:
-            cycleIndexes = Cycles
-            print('Deprication warning: the "Cycles" key word arguement has been replaced by "cycleIndexes", and will return an error in future versions.')
-        
+        """        
         
         xyHys = self.xy
-        Vectors = self.cycles
         
-        self.showCycles(self, xyHys[:,0], xyHys[:,1], plotCycles, plotPeaks, labelCycles, Cycles, **kwargs)
+        if not colorCycles:
+            colorCycles = self.colorCycles
         
-        colorDict = self.colorDict
-        
-        lines = []
-        # If the list is empty, plot everything
-        if len(cycleIndexes) == 0:
-            for ii, vector in enumerate(Vectors):
-                # c = colorDict[int(np.floor((ii + 1)/2) % 3)]
-                c = colorDict[int(np.floor((ii + 1)/2) % 2)]
-                line, = plt.plot(vector.xy[:,0], vector.xy[:,1], c=c)
-                # plt.plot(vector.xy[:,0], vector.xy[:,1])
-                lines.append(line)
-
-        else:
-            for ii, vector in enumerate(Vectors):
-                if ii in Cycles:
-                    # c = colorDict[int(np.floor((ii + 1)/2) % 3)]
-                    # plt.plot(vector.xy[:,0], vector.xy[:,1], c=c)
-                    line = plt.plot(vector.xy[:,0], vector.xy[:,1])
-                    lines.append(line)
+        self.showCycles(xyHys, showReversals, showPeaks, self.peakIndexes, 
+                        self.reversalIndexes, labelReversals, cycleIndexes)
+                    
+        return self._plot_curves(self.cycles, cycleIndexes, colorCycles, **kwargs)
+    
+     
+    
 
-       
     def recalculateCycles(self, revDist = 2, revWidth = None, revProminence = None, **kwargs):
         """
         Calcualtes the cycles again, using the input parameters for distance 
         (number of indexes), width (distance on the x axis), and prominence
         (distance in the y axis).
         
         Peaks are calculated using scipy's find_peaks function.
@@ -715,17 +766,14 @@
         
         Returns
         -------
         None.
 
         """
         
-        # Deprication waring, remove later
-        findPeakKwargs(**kwargs)
-        
         self.setReversalIndexes(revDist, revWidth, revProminence)
         self.setCycles()
         self.setArea()
         
         
     def recalculateCycles_like(self, sampleHysteresis):
         """
@@ -789,27 +837,26 @@
         
         
         try:
             dxy = self.length
         except:
             raise Exception('Length not set yet, set length using .setLength')
                         
-        self.reversalIndexes = data.getMaxIndicies(dxy, revDist, revWidth, revProminence)
+        self.reversalIndexes = data.getMaxIndexes(dxy, revDist, revWidth, revProminence)
         self.loadProtocol = self.xy[self.reversalIndexes,0]
         
         self.setCycles()
         self.setArea()           
 
-    def RemoveCycles():
-        pass
-
-class SimpleCycle(CurveBase):
-    """ A curve that doesn't change direction on the X axis, but can change
-    Y direction. The data has a number of peaks, each of which is the largest
-    y value in relation to other points on the curve. This point canbe 
+class SimpleCurve(Curve):
+    """ 
+    A simple cycle is a curve that doesn't change direction on the X axis, but 
+    can change direction in it's Y wzis. The data has a number of peaks, each 
+    of which is the largest y value in relation to other points on the curve. 
+    This point canbe 
     
     
     Parameters
     ----------
     XYData : array
         The input array of XY date for the curve. A list [x,y] can also be 
         passed into the function.
@@ -838,25 +885,27 @@
         Can be turned off for performance reasons.
     setSlope : Boolean, optional
         Used to turn on or off setting the slopeby default. 
         Can be turned off for performance reasons.   
     
     """
     
+    colorCycles = ['C0', 'C1'] # applies to subcycles here
+    
     def __init__(self, XYData, findPeaks = False, setSlope = False, setArea = False,
                  peakDist = 2, peakWidth = None, peakProminence = None, **kwargs):
-        CurveBase.__init__(self, XYData, **kwargs)
+        Curve.__init__(self, XYData, **kwargs)
         
         self._setDirection()
         self._setStatePropreties(findPeaks, setSlope, setArea, 
                                  peakDist, peakWidth, peakProminence)
                
         self.subCycles = None
         if findPeaks == True:
-            self.setPeaks(peakDist, peakWidth, peakProminence)
+            self.setPeaks()
             self.setSubCycles()
     
         if setSlope == True:
             self.setSlope()
         if setArea == True:
             self.setArea()      
 
@@ -879,127 +928,150 @@
         """
         Sets the propreties that are used to caculate where reversal points occur.
         These are used if we want to copy new classes using the same parameters.
         """
         return [self._findPeaks,self._setSlope,self._setArea,
                 self.peakDist, self.peakWidth, self.peakProminence]
 
-
-
     def _setDirection(self):
         """
          1 = left to right. -1 = to is right to left
 
         """
         xdata = self.xy[:,0]
         if xdata[0] <= xdata[-1]:
             self.direction =  1
         else:
             self.direction = -1
            
                 
-    def setSubCycles(self):
+    def setSubCycles(self, peakDist = 2, peakWidth = None, peakProminence = None):
         """
         Finds monotonic "sub-sycles" within each cycle.
         Peaks must be set before subcyles can be set.
 
         """
 
         xy = self.xy
+        if self.peakIndexes is None:
+            self.setPeaks(peakDist, peakWidth, peakProminence)
         indices = self.peakIndexes
         NIndex = len(indices) - 1
         
         SubCycles = [None]*NIndex
         for ii in range(NIndex):
             SubCycles[ii] = MonotonicCurve(xy[indices[ii]:(indices[ii+1]+1), :])
                        
         self.subCycles = SubCycles
         self.NsubCycles = len(SubCycles)
-        
-        
+                
     def setSubCyclesArea(self):
         """
-        Sets the net area for all SubCycles
+        Sets the net area for all SubCycles.
         """
         try:
             SubCycles = self.subCycles
         except:
             raise Exception('No SubCycles not yet set')
             
         for subCycle in SubCycles:
             subCycle._setNetArea        
 
     def setSubCyclesSlope(self):
         """
-        Sets the net area for all MonotonicCurves
+        Sets the net slope for all MonotonicCurves.
         """
         try:
             SubCycles = self.subCycles
         except:
             raise Exception('SubCycles not yet set')
             
         for SubCycle in SubCycles:
             SubCycle.setSlope()       
       
-    def getSubCycles(self, indicies):
+    def getSubCycles(self, indexes):
         """
-        returns a list of subcycles with the input indicies.
+        returns a list of subcycles with the input indexes.
 
         Parameters
         ----------
         Index : list of int
             The integer index of the sub-cycle you want to return.
 
         Returns
         -------
         Subcycle
             The output subcycle.
 
         """        
         
-        SubCycles = [self.subCycles[index] for index in indicies]
+        SubCycles = [self.subCycles[index] for index in indexes]
         return SubCycles      
     
     def getSubCycle(self, index):
         """
-        Gets the subcycle with a partcular index
+        Gets the subcycle with a partcular index.
 
         Parameters
         ----------
         Index : int
             The integer index of the sub-cycle you want to return.
 
         Returns
         -------
         Subcycle
             The output subcycle.
 
         """
         return self.subCycles[index]
-     
-    def plotSubCycles(self, SubCyclesIndicies = [], plotCycles = False, plotPeaks = False):
+    
+    def plotSubCycles(self, subCyclesIndexes:list = None, showReversals = False, showPeaks = False,
+                      colorCycles:list = None, **kwargs):
+        """
+        Plots the xy values of a several subcycles on the same figure.
+        If no list is provided, every subcycle will be plotted.
+        
+        Parameters
+        ----------
+        subCyclesIndexes : list of int
+            A list of the subcycles to be plotted.
+        showReversals : bool
+            A switch that specifics if subcycle reversal points should be plotted.
+            It's expected that there are no reveral points in each subcycles'            
+        showPeaks : bool
+            A switch that specifics if the detected peak values should be plotted.
+            
+        kwargs : list, optional
+            Any additional keyword arguements will be passed to the matplotlib
+            plot function. This can be used to custize char appearance.            
+        """  
         
         xyMono = self.xy
-        Vectors = self.subCycles
         
-        self.showCycles(self, xyMono[:,0], xyMono[:,1], plotCycles, plotPeaks)
+        if not colorCycles:
+            colorCycles = self.colorCycles
+        
+        self.showCycles(xyMono, showReversals, showPeaks, self.peakIndexes, 
+                        self.reversalIndexes, None, subCyclesIndexes)
+ 
+        # lines = []
+        # # If the list has content, get the cycles to plot, otherwise plot everything
+        # if subCyclesIndexes is not  None:
+        #     vectors = [self.subCycles[ii] for ii in subCyclesIndexes]
+        
+        # for ii, vector in enumerate(vectors):
+        #     c = colorCycles[int(ii % Ncolor)]
+        #     line, = plt.plot(vector.xy[:,0], vector.xy[:,1], c=c, **kwargs)
+        #     lines.append(line)        
+        # return lines
+    
+        return self._plot_curves(self.subCycles, subCyclesIndexes, colorCycles, **kwargs)
+    
+    
         
-        colorDict = self.colorDict
-        if len(SubCyclesIndicies) == 0:
-            for ii, vector in enumerate(Vectors):
-                c = colorDict[ii%2]
-                plt.plot(vector.xy[:,0], vector.xy[:,1], c = c)
-
-        else:
-            for ii, vector in enumerate(self.SimpleCycles):
-                if ii in SubCyclesIndicies:
-                    c = colorDict[ii%2]
-                    plt.plot(vector.xy[:,0], vector.xy[:,1], c = c)
-            
-            
     def recalculatePeaks(self, peakDist = 2, peakWidth = None, peakProminence = None):
         """
         Peaks are calculated using scipy's find_peaks function
         
         Parameters
         ----------
             
@@ -1024,61 +1096,29 @@
         None.
 
         """
         self.setPeaks(peakDist, peakWidth, peakProminence)
         self.setSubCycles()
         self.setArea()  
 
-class MonotonicCurve(CurveBase):
+class MonotonicCurve(Curve):
     """
     A curve that has no changes in it's x axis direction, as well as no changes
     in it's y axis direction.
     """   
     def __init__(self, XYData, **kwargs):
-        CurveBase.__init__(self, XYData, **kwargs)
+        Curve.__init__(self, XYData, **kwargs)
         
         self._setDirection()
             
     def _setDirection(self):
         """
          1 = neg to pos. -1 = pos to neg
         """
         ydata = self.xy[:,1]
         if ydata[0] <= ydata[-1]:
             self.direction =  1
         else:
             self.direction = -1
 
 
-# =============================================================================
-# Deprication warnings
-# =============================================================================
-
-def findPeakKwargs(**kwargs):
-    if 'peakDist' in kwargs.keys():
-        raise Exception('Use of "peakDist" has been depricated. Instead use "revDist".')
-    if 'peakDist' in kwargs.keys():
-        print('Use of "peakWidth" has been depricated. Instead use "revWidth".')
-    if 'peakProminence' in kwargs.keys():
-        print('Use of "peakProminence" has been depricated. Instead use "revProminence".')    
-    
-    # pass
-
-
-"""
-TODO:
-    For Monotonic curves:
-    Find and time between peaks is optional.
-    Find interesections
-    FInd area nearest to current peak
-"""
-
-
-"""
-TODO:
-    Allow for custom headings:
-    Perhaps a style object?
-
-    Add limitts to the style object?    
-    Make the limits part of the hysteresis object, so they don't need
-    to continually be passed to each funciton.
-"""
+
```

### Comparing `hysteresis-1.2.1/Hysteresis/baseFuncs.py` & `hysteresis-2.0.0/Hysteresis/baseFuncs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from scipy.interpolate import interp1d
-from .baseClass import Hysteresis, SimpleCycle, MonotonicCurve
+from .curve import Hysteresis, SimpleCurve, MonotonicCurve
 
 
 
 # This is kind of unorganized right now...
 
 
 # Todo:
@@ -155,20 +155,20 @@
     """
 
     
     
     # Get sample parameters, then pass those to the new curve.
     
     # if the curve is a SimpleCycle
-    if isinstance(Curve, SimpleCycle):
+    if isinstance(Curve, SimpleCurve):
     
         x = Curve.xy[:,0]
         y = Curve.xy[:,1]
         direction = Curve.direction
-        Output = SimpleCycle(_RemoveNeg(x, y, direction))    
+        Output = SimpleCurve(_RemoveNeg(x, y, direction))    
        
     # if the curve is a hysteresis, we recursively create a series of Cycles
     elif isinstance(Curve, Hysteresis):
         outputCycles = [None]*Curve.NCycles
         for ii, Cycle in enumerate(Curve.Cycles):
             outputCycles[ii] = removeNegative(Cycle)
         Output = concatenateHys(*outputCycles)    # If Curve
```

### Comparing `hysteresis-1.2.1/Hysteresis/climate.py` & `hysteresis-2.0.0/Hysteresis/climate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 
-from .baseClass import CurveBase
+from .curve import Curve
 
 import matplotlib.pyplot as plt
 from scipy.optimize import curve_fit
 
 
 
 # =============================================================================
@@ -50,29 +50,25 @@
     """
     
     coef, correlation = curve_fit(f, xy[:,0], xy[:,1], **kwargs)
     
     return coef, correlation
 
 
-
-
-
-
-class SeasonalCurve(CurveBase):
+class SeasonalCurve(Curve):
     """
     The input XY data is assumed to be evenly spaced in time.
     
     The curve will be closed so that the first point is equal to the final
     point.
     """
     
     
     def __init__(self, xy, period = 1, n = 1, m = 1):
-        CurveBase.__init__(self, xy)
+        Curve.__init__(self, xy)
         
         self.time = np.arange(0, self.Npoints)/self.Npoints
         self.period = period
         self.n = n
         self.m = m
         
         self.tempFunction = getTemp
```

### Comparing `hysteresis-1.2.1/Hysteresis/compare.py` & `hysteresis-2.0.0/Hysteresis/compare.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-
+from .curve import Curve, Hysteresis
 import hysteresis.env as env
-# from .defaultDataFuncs import defaultSampleFunction, defaultCombineDiff
 from .resample import resample
 
 
 # =============================================================================
 # Compare
 # =============================================================================
 # TODO: consider storing the sample function within the class itself.
 
-def compareCycle(Curve1, Curve2, Nsample = 10):
+def compareCycle(Curve1:Curve, Curve2:Curve, Nsample = 10):
     """
     Compares two Curve objects by resampling them using linear interplation,
     then comparing the distance between both cycles in a comon domain.
 
     Parameters
     ----------
     Curve1 : Curve
@@ -45,15 +44,15 @@
     xy2 = resample(xy2, Nsample)
     
     
     diff = sampleFunction(xy1, xy2)
 
     return diff
 
-def compareHys(Hys1, Hys2):
+def compareHys(Hys1:Hysteresis, Hys2:Hysteresis):
     """
     
 
     Parameters
     ----------
     Hys1 : Hysteresis Object
         The first Hysteresis object.
```

### Comparing `hysteresis-1.2.1/Hysteresis/data.py` & `hysteresis-2.0.0/Hysteresis/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     
     InterpFunction = interp1d(TempDataX, TempDataY)
     ySample = InterpFunction(xSample)
           
     return xSample,ySample
 
 
-def getMaxIndicies(VectorX, peakDist = 2, peakWidth = None, 
+def getMaxIndexes(VectorX, peakDist = 2, peakWidth = None, 
                      peakProminence = None, **kwargs):
     MaxIndexes,_ = find_peaks(VectorX, height = (None, None), distance = peakDist, 
                             width = peakWidth, prominence = peakProminence, **kwargs)
 
     Nindex = len(MaxIndexes) + 2
     Indexes = np.zeros(Nindex, dtype = int)
     Indexes[0] = 0
@@ -88,15 +88,15 @@
         order = 1
     else:
         order = 2
     return order
 
 
 
-def getCycleIndicies(VectorX, peakDist = 2, peakWidth = None, 
+def getCycleIndexes(VectorX, peakDist = 2, peakWidth = None, 
                      peakProminence = None, **kwargs):
     """
     This function finds the index where there is areversal in the XY data. 
     You may need to adjust the find peaks factor to get satisfactory results.
     Built on the scipy find peaks funciton
     
 
@@ -232,16 +232,16 @@
     Rnet : float
         Returns a the sampled value 
 
     """
        
     # We get the indicies where the reversal happens.
     
-    ExperimentIndicies = getCycleIndicies(ExperimentX, Nsample, peakDist, peakwidth, ExperimentY)
-    AnalysisIndicies = getCycleIndicies(AnalysisX, Nsample, peakDist, peakwidth, AnalysisY)
+    ExperimentIndicies = getCycleIndexes(ExperimentX, Nsample, peakDist, peakwidth, ExperimentY)
+    AnalysisIndicies = getCycleIndexes(AnalysisX, Nsample, peakDist, peakwidth, AnalysisY)
     
     # We check that both curves have the same number of indicies
     NIndex = len(ExperimentIndicies) - 1
     NIndex_2 = len(AnalysisIndicies) - 1
     R= np.zeros(NIndex)
     
     # If they don't we create a error
```

### Comparing `hysteresis-1.2.1/Hysteresis/defaultDataFuncs.py` & `hysteresis-2.0.0/Hysteresis/defaultDataFuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import numpy as np
-from numpy import trapz
 
 from scipy.interpolate import interp1d
 from hysteresis import data
 
-import matplotlib.pyplot as plt
-
-
-
 
 def defaultSlopeFunction(xy):
     """
     The standard slope function. The slope is undefined for reversal indexes.
     
     For middle points, a centeral finite difference scheme is used, which is 
     O(h**2) accurate for constant steps h.
```

### Comparing `hysteresis-1.2.1/Hysteresis/defaultPlotFuncs.py` & `hysteresis-2.0.0/Hysteresis/defaultPlotFuncs.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         ax.set_xlim(xlim[0], xlim[1])
 
     if len(ylim) != 0 :
         ax.set_ylim(ylim[0], ylim[1])
                
     return fig, ax
 
-def defaultShowCycles(self, x, y, plotCycles, plotPeaks, labelCycles = [], Cycles = []):
+def defaultShowCycles(xy, showReversals, showPeaks, peakIndexes = None, 
+                      reversalIndexes=None,  labelCycles = None, cycleIndicies = None):
     """
     A function that plots the location of the reversal points and peaks for a
     curve object.
 
     Parameters
     ----------
     x : array
@@ -43,100 +44,107 @@
         A switch that specifics if peak values should be plotted.
     labelCycles : list or 'all', optional
         A list of the cycles to be labled. 
         A value of 'all' can also be specified, in which case all cucles will be plotted.
         The default is [], which labels no cycles
     Cycles : kist, optional
         A list of the cycles to be plotted. If not specified, all values will 
-        be plotted. The default is [], which plots all cycles.
+        be plotted. The default is NOne, which plots no labels cycles.
 
     """
     
+    x = xy[:,0]
+    y = xy[:,1]
+    
+    if labelCycles is None:
+        labelCycles = []
     
+    if cycleIndicies is None:
+        cycleIndicies = []    
+        
     # Plot cycles as x only
-    if plotPeaks == True:
-        try:
-            Indexes = self.peakIndexes
-        except:
+    if showPeaks == True:
+        
+        inds = peakIndexes
+        if peakIndexes is None:
             raise Exception('No peaks have been set')
-        PeakX = x[Indexes]
-        PeakY = y[Indexes]
+            
+        PeakX = x[inds]
+        PeakY = y[inds]
 
         line2  = plt.plot(PeakX, PeakY, "+")
         # plt.title('Peak Index y values')    # Plot cycles as x only
         
-    if plotCycles == True:
-        try:
-            reversalIndexes = self.reversalIndexes        
-        except:
-            raise Exception("Object has no Cycles to display. Try setting cycles.")
+    if showReversals == True:
+        
+        if reversalIndexes is None:
+            raise Exception('No peaks have been set')
         # TODO: update marker based on direction?
         
         # if only certain cycles have been asked for we remove all indexes other indexes
-        if Cycles != []:
-            markerIndexes = reversalIndexes[Cycles]
+        if cycleIndicies != []:
+            markerIndexes = reversalIndexes[cycleIndicies]
             # only label Cycles that are in the cycles asked for
-            labelCycles = np.array([label for label in labelCycles if label in Cycles])
+            labelCycles = np.array([label for label in labelCycles if label in cycleIndicies])
         else:
             # Otherwise we plot all
             markerIndexes = reversalIndexes
         
         # Indexes = Indexes[]
         markerX = x[markerIndexes]
         markerY = y[markerIndexes]         
 
         # Plot the desired indexes
         line2  = plt.plot(markerX, markerY, "x")        
 
         # If the cycles need to be labeled,
-        # if labelCycles is 'all':
         if str(labelCycles) == 'all':
             # skip the first and last cycles
             labelIndexes = np.arange(0,len(markerIndexes))
             labelX = x[reversalIndexes]
             labelY = y[reversalIndexes]
         else:
             labelIndexes = labelCycles
             labelX = x[reversalIndexes[labelCycles]]
             labelY = y[reversalIndexes[labelCycles]] 
 
             
         for ii in range(len(labelIndexes)):
             Annotate = plt.annotate(labelIndexes[ii], [labelX[ii],labelY[ii]], xytext=(-1, 5), textcoords = 'offset points')
-            
-            
-            # Annotate = plt.annotate(int(ii), xy=(ReversalX[ii], ReversalY[ii]),xytext=(-10, 10), arrowprops=dict(arrowstyle="->"))
-            # Annotate = plt.annotate(int(Cycle), xy=(ReversalX[ii], ReversalY[ii]), xytext=(-1, 5), textcoords = 'offset points', fontsize=12)
-            # Annotate = plt.annotate(int(ii), xy=(ReversalX[ii], ReversalY[ii]))
 
-def defaultPlotFunction(self, x, y, plotCycles, plotPeaks, labelCycles = [], **kwargs):
+
+def defaultPlotFunction(xy, showReversals, showPeaks, peakIndexes = None, 
+                      reversalIndexes=None, labelCycles = None, **kwargs):
     """
     Parameters
     ----------
-    x : array
-        The input x values as an numpy array.
+    xy : 2D array [Npoints, 2]
+        The input x/y values as an numpy array, in order x,y and shape [Npoints, 2].
+        e.g. x = xy[:,0]
     y : array
         The input y values as an numpy array.
     plotCycles : bool
         A switch that specifics if cycle reversal points should be plotted.
     plotPeaks : bool
         A switch that specifics if peak values should be plotted.
     labelCycles : list or 'all', optional
         A list of the cycles to be labled. 
         A value of 'all' can also be specified, in which case all cucles will be plotted.
         The default is [], which labels no cycles
     Cycles : kist, optional
         A list of the cycles to be plotted. If not specified, all values will 
         be plotted. The default is [], which plots all cycles.
     """
-
+    
+    x = xy[:,0]
+    y = xy[:,1]
           
     line, = plt.plot(x, y, **kwargs)
        
-    defaultShowCycles(self, x, y, plotCycles, plotPeaks, labelCycles)
+    defaultShowCycles(xy, showReversals, showPeaks, peakIndexes, reversalIndexes, labelCycles)
     
     return line
```

### Comparing `hysteresis-1.2.1/Hysteresis/env.py` & `hysteresis-2.0.0/Hysteresis/env.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,14 +27,13 @@
         self.finit = initializeFig
         self.fplot = defaultPlotFunction
         self.fcycles = defaultShowCycles
         
         self.fSample = defaultSampleFunction
         self.fCombineDiff = defaultCombineDiff
         
-        
     def restart(self):
         self.__init__()
 
 
 environment = HYSTERESIS_ENVIRONMENT()
-# environment.restart()
+
```

### Comparing `hysteresis-1.2.1/Hysteresis/envelope.py` & `hysteresis-2.0.0/Hysteresis/envelope.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from numpy import trapz
 # import matplotlib.pyplot as plt
 
 from scipy.interpolate import interp1d
 from hysteresis import data
 
 from .data import linearInterpolation
-from .baseClass import Hysteresis, SimpleCycle
+from .curve import Hysteresis, SimpleCurve
 from .defaultDataFuncs import defaultAreaFunction, defaultSlopeFunction
 from .defaultPlotFuncs import initializeFig, defaultPlotFunction, defaultShowCycles
 
 
 
  
 # =============================================================================
@@ -160,15 +160,15 @@
     
         
     # Remove repeated points
     xPos = xyPos[:,0]
     _, indexes = np.unique(xPos,True)
     xyPos = xyPos[indexes]   
     
-    return SimpleCycle(xyPos, True)
+    return SimpleCurve(xyPos, True)
 
 
 def _averageBackbones(backBonePos,backBoneNeg):
     xPos = backBonePos.xy[:,0]
     xNeg = backBoneNeg.xy[:,0]
     
     f1 =  interp1d(backBonePos.xy[:,0], backBonePos.xy[:,1], fill_value = 'extrapolate')
@@ -179,15 +179,15 @@
     
     ypos = f1(x)
     yneg = f2(x)
     
     yavg = (ypos + yneg) / 2
     
     xy = np.column_stack([x, yavg])
-    backBoneAvg = SimpleCycle(xy, True)
+    backBoneAvg = SimpleCurve(xy, True)
     
     return backBoneAvg
 
 
 def getAvgBackbone(hystersis, LPsteps = [], returnPeaks = False,  returnEnd = False,
                    skipStart = 0, skipEnd =0):
     
@@ -295,15 +295,15 @@
     # add the new point, then find the index
     xy       = np.concatenate([xy, [[dUult, Pult]]])
     order    = np.argsort(xy[:,0])
     xy       = xy[order]
     endIndex = np.where(xy[:,0] == dUult)[0][0] + 1
     
     # make a new curve that ends at the failure load. 
-    backbone = SimpleCycle(xy[:endIndex])
+    backbone = SimpleCurve(xy[:endIndex])
     
     return Pult, dUult, backbone
 
 def _getIntersection(xy, Ppeak, intersection):
     # Find the elastic intercept and slope.
     Pinter  = intersection*Ppeak
     index   = np.argmin(xy[:,1] < Pinter)
@@ -354,29 +354,24 @@
         Pult, dUult = _get_ult_1(Pend, dUend)
     else:           # If the final point is less than 0.8Ppeak, find the intercept.
         Pult, dUult, backbone = _get_ult_2(Plim, xy, xyFail)
     
     backbone.setArea()    
     Anet = backbone.getNetArea()    
     
-    # Find the elastic intercept and slope.
-    # Pinter  = 0.4*Ppeak
-    # index   = np.argmin(xy[:,1] < Pinter)
-    # dUinter = _linInterpolateY(xy, Pinter, index)
-    # _getIntersection(xy, Ppeak, 0.4)
     Ke      = _getIntersection(xy, Ppeak, 0.4)
         
     radicand = dUult**2 - 2*Anet/Ke
     
     if 0 < radicand:
         Py = Ke*(dUult - (radicand)**0.5)
     else:
         Py = 0.85*Ppeak
     
     curvexy = np.column_stack([[0, Py/Ke, dUult], [0,Py,Py]])
-    curve = SimpleCycle(curvexy)
+    curve = SimpleCurve(curvexy)
     curve.setArea()
     
     return curve
```

### Comparing `hysteresis-1.2.1/Hysteresis/plotSpecial/animate.py` & `hysteresis-2.0.0/Hysteresis/plotSpecial/animate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri May  7 20:15:19 2021
 
 @author: Christian
 
+Notes, currently an experimentla feature. In the future I'd like to
+    Add arrow key functionality
+    Add bliting to speed up rendering.
 
-TODO:
-    Add arrow key functionality?
-    Add bliting
-    Make ABC and make update an abstract method.
 """
 
-# import hysteresis as hys
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation
-# from dataclasses import dataclass
 from matplotlib.widgets import Button, Slider
 import numpy as np
 
 # Add this function to somewhere else
 def init_Animation():
     fig, ax = plt.subplots()
     
     return fig, ax
     
-
-
 def getAnixy(rawFrames, skipFrames):
     xyAni = rawFrames[::skipFrames,:]
     
     return xyAni
 
 def getAniFrames(x:list, targetdx:float):
     """
-    given a input array of positive nu x, return a new array 
+    This function is used to get a set of animation frames from a input vector.
+    For the input vector x, a single frame will be pulled from every region
+    dx. Assumes that x is monotonically increasing.
     
-    Returns a frame every target dx. Can be useful for pre-processing data
-    if input data has a variable timestep.
+    This can be useful for pre-processing dataif input data has a variable timestep.
     
-    No linearl inerpolatin is used for intermediate frames.
+    No linear inerpolatin is used for intermediate frames.
     
     Parameters
     ----------
     x : list
-        DESCRIPTION.
+        the array of input values.
     targetdx : float
-        DESCRIPTION.
+        the dx for the output animation..
 
     Returns
     -------
-    TYPE
-        DESCRIPTION.
+    np.array
+        the output np array of points, with one frame every dx from the 
+        target dx.
 
     """
 
     NFrames = len(x)   
     NframesOut = []
     
     jj = 0
@@ -198,29 +195,30 @@
         else:
             update = self.update
         
         self.ani = FuncAnimation(self.fig, update, self.frames,  
                                  interval=self.interval, blit=False)
 
 
-# @dataclass
 class Animation(AnimationBase):
         
     def __init__(self, Curve, pointsPerFrame = 1, skipFrames = 1, 
                  skipStart = 0, skipEnd = 0, interval = 50, widgets = True):
         """
-        Creates a animation of the input curve object
+        Creates a animation of the input curve object.
+        This is still an experimental feature and may not work as intended 
+        for large datasets.
 
         Parameters
         ----------
         Curve : Hysteresis Curve
             The curve to animate.
         pointsPerFrame : int, optional
             The number of data points to draw per frame. The default is 1.
-        skipFrames : TYPE, optional
+        skipFrames : int, optional
             THe number of animation frames to skip per input. This reduces
             can be used to reduce the size of large data arrays. The default is
             1, which shows all frames.
         skipStart : int, optional
             Allows the user to skip this many frames at the start.
             Skipped frames are applied after the other frame filters are applied.
             The default is 0, which skips no start frames.
@@ -258,16 +256,14 @@
         
         if skipEnd == 0:
             return xyAni[skipStart:, :]
         else: 
             skipEnd *= -1 
         return xyAni[skipStart:skipEnd, :]
 
-
-    
     def update(self, frame):
         """
         Updates the canvas at the given frame.
 
         """
         points = int(frame*self.pointsPerFrame)
         newXY  = self.xyAni[:points,:]
@@ -360,35 +356,27 @@
             xyAni = getAnixy(xy, self.skipFrames)
             
             self.xyCurves[ii] = xyAni
             line = plt.plot(xyAni[:,0], xyAni[:,1])[0]
             self.lines.append(line)    # def initAnimation(self):        
             
     def update(self, frame):
-        
-        # print(frame)
         points = int(frame*self.pointsPerFrame)
-        # print(points)
         lines = [None]*self.Ncurves
         for ii in range(self.Ncurves):
 
             tempXY = self.xyCurves[ii]
             # print()
             
             newXY = tempXY[:points,:]
             line = self.lines[ii]
             line.set_data(newXY[:,0], newXY[:,1])
             lines[ii] = line
         
         self.aniArtists = lines
-        # self.aniArtists
-            # lines[ii] = line
-        # lines = self.lines
-        
-        # return lines
         return self.aniArtists
     
     # def animate(self):
     #     self.initAnimation()
     #     if self.widgets == True:        
     #         self.connectWidgets()
     #         update = self.update_slider_widget
```

### Comparing `hysteresis-1.2.1/Hysteresis/plotSpecial/core.py` & `hysteresis-2.0.0/Hysteresis/plotSpecial/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri May  7 20:15:19 2021
 
 @author: Christian
 """
 
-import hysteresis as hys
 import matplotlib.pyplot as plt
 import matplotlib.animation as animation
 from matplotlib.widgets import Button
 
-# from matplotlib.animation import FuncAnimation
 import numpy as np
 
-import openseespy.postprocessing.Get_Rendering
-
-
-
 # Add this function to somewhere else
 def init_Animation():
     fig, ax = plt.subplots()
     
     return fig, ax
     
 
@@ -45,16 +39,14 @@
         
         while jj*targetdx < x[ii]:
             NframesOut.append(x[ii])
             jj+=1
 
     return np.array(NframesOut)
 
-
-
 class AnimationBase:    
     
     def __init__(self):
         self.play = True
         
         # Replace with imported function
         fig, ax = init_Animation()
```

### Comparing `hysteresis-1.2.1/Hysteresis/plotSpecial/guiPlot.py` & `hysteresis-2.0.0/Hysteresis/plotSpecial/guiPlot.py`

 * *Files identical despite different names*

### Comparing `hysteresis-1.2.1/Hysteresis/protocol.py` & `hysteresis-2.0.0/Hysteresis/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,13 @@
 import numpy as np
 
-from .baseClass import SimpleCycle
+from .curve import SimpleCurve
 from .baseFuncs import concatenateHys
 
 
-
-
-
-# def getProtcol(loadProtcol,Nrepeats):
-#     pass
-
-
-# def getTimeseries(loadProtcol:list, dx:float, halfCycle=True, ):
-    
-    
-    
-    
-#     pass
-
-
-# def getTimeseries(loadProtcol:list, Nrepeat, halfCycle=True):
-    
-    
-    
-    
-#     pass
-
-
-
-
 def getReturnCycle(cycleStart, cycleReturn):
     """
     This function finds the return cycle that closes a hystresis Full cycle
 
     """
     
     xy1 = cycleStart.xy
@@ -45,15 +20,15 @@
     TransitonIndex = np.argmax(x2 < x1max)
     TransitonIndex = np.argmin(x2 < x1max)
     
     xyOut = np.zeros([TransitonIndex + 1, 2])
     xyOut[:TransitonIndex,:] = xy2[:TransitonIndex,:]
     xyOut[-1,:] = xy1[0,:]
     
-    return SimpleCycle(xyOut)
+    return SimpleCurve(xyOut)
 
 
 
 
 def exandHysTrace(hysteresis, loadProtocolNcycles, skipStart = 1, 
                   skipEnd = 1):
     """
```

### Comparing `hysteresis-1.2.1/Hysteresis/resample.py` & `hysteresis-2.0.0/Hysteresis/resample.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from .baseClass import Hysteresis, SimpleCycle, MonotonicCurve
+from .curve import Hysteresis, SimpleCurve, MonotonicCurve
 from .baseFuncs import (concatenateHys, concatenate, _linInterp, 
                         _linInterpSample, _getNsamples)
        
 # =============================================================================
 # concatenate and resample
 # =============================================================================
            
@@ -37,31 +37,31 @@
         An object of the input type with a number of points equal to Nsamples
 
     """  
         
     # We recursively resample by calling the function again for sub-cycle objects
     
     # if the curve is a SimpleCycle
-    if isinstance(curve, SimpleCycle):
+    if isinstance(curve, SimpleCurve):
         x = curve.xy[:,0]
         y = curve.xy[:,1]
         
         # If the simple cycle has subcycles, resample at the level of those.
         if curve.subCycles:
             outputSubcycles = [None]*curve.NsubCycles
             for ii, subcycle in enumerate(curve.subCycles):
                 outputSubcycles[ii] = resample(subcycle, Nsamples)    
                 
-            tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCycle)
+            tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCurve)
             tmpProps    = curve._getStatePropreties()
-            Output      = SimpleCycle(tmpOut.xy, *tmpProps)
+            Output      = SimpleCurve(tmpOut.xy, *tmpProps)
                         
         # Otherwise, resample the curve directly
         else:
-            Output = SimpleCycle(_linInterp(x,y, Nsamples))    
+            Output = SimpleCurve(_linInterp(x,y, Nsamples))    
        
     # if the curve is a hysteresis, we recursively create a series of Cycles
     elif isinstance(curve, Hysteresis):
         outputCycles = [None]*curve.NCycles
         for ii, cycle in enumerate(curve.cycles):
             outputCycles[ii] = resample(cycle, Nsamples)
         Output = concatenateHys(outputCycles)    # If curve
@@ -100,17 +100,17 @@
     For each curve, a number of points will be chosen based on some target
     displacement value in the x direction. If the value overshoots, 
     the last point will instead be used.
     For example, if the start = 2.5, end = 7.5 and dx = 2, points will be 
     placed at 2.5, 4.5, 6.5, 7.5 
     
     Linear interpolation is used to find the y value of intermediate points.
-    In the case of a Hysteresis, every SimpleCycle curve will be resampled with
+    In the case of a Hysteresis, every SimpleCurve will be resampled with
     an amount of points equal to Nsamples.
-    In the case of a SimpleCycle, each monotonic curve will be resampled.
+    In the case of a SimpleCurve, each monotonicCurve will be resampled.
 
     Parameters
     ----------
     curve : Hysteresis, Monotonic Cycle, or numpy array
         The curve to be resampled.
 
     Targetdx : float
@@ -122,25 +122,25 @@
         An object of the input type, with points approximately at Targetdx.
 
     """  
 
 
     # the logic in these functions is getting a little nasty, in the future
     # consider pulling these out into class methods.
-    if isinstance(curve, SimpleCycle):
+    if isinstance(curve, SimpleCurve):
                
         if curve.subCycles: # if subsycles are set, resample those
             outputSubcycles = [None]*curve.NsubCycles
             for ii, subcycle in enumerate(curve.subCycles):
                 outputSubcycles[ii] = resampleDx(subcycle, Targetdx)
-            # Output = concatenate(*outputSubcycles, outputClass = SimpleCycle)    # If curve        
+            # Output = concatenate(*outputSubcycles, outputClass = SimpleCurve)    # If curve        
         
-            tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCycle)
+            tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCurve)
             tmpProps    = curve._getStatePropreties()
-            Output      = SimpleCycle(tmpOut.xy, *tmpProps)        
+            Output      = SimpleCurve(tmpOut.xy, *tmpProps)        
         
         else: # if subsycles aren't set, resample those
             x = curve.xy[:,0]
             dxNet = x[-1] - x[0]
             Nsamples = _getNsamples(Targetdx, dxNet)
             Output = resample(curve, Nsamples)    
         
@@ -257,31 +257,31 @@
     """
     
     
     regions = _parseRegions(regions) # these get interpolated
     allRegions, isInside = _getOutsideRegions(regions) # these get left alone  
     
     
-    if isinstance(curve, SimpleCycle):
+    if isinstance(curve, SimpleCurve):
 
         if curve.subCycles: # if subsycles are set, resample those
             outputSubcycles = [None]*curve.NsubCycles
             for ii, subcycle in enumerate(curve.subCycles):
                 outputSubcycles[ii] = resampleRegion(subcycle, Nsamples, regions)
                 
-            tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCycle)
+            tmpOut      =  concatenate(outputSubcycles, outputClass = SimpleCurve)
             tmpProps    = curve._getStatePropreties()
-            output      = SimpleCycle(tmpOut.xy, *tmpProps)        
+            output      = SimpleCurve(tmpOut.xy, *tmpProps)        
         
         else: # if subsycles aren't set, resample at level of xy
         
             x = curve.xy[:,0]
             y = curve.xy[:,1]
             xy = np.column_stack([x, y])
-            output = SimpleCycle(resampleRegion(xy, Nsamples, regions))        
+            output = SimpleCurve(resampleRegion(xy, Nsamples, regions))        
     
     elif isinstance(curve, Hysteresis):
         outputCycles = [None]*curve.NCycles
         for ii, cycle in enumerate(curve.cycles):
             outputCycles[ii] = resampleRegion(cycle, Nsamples, regions)
         tmpOut = concatenateHys(outputCycles)
         tmpProps = curve._getStatePropreties()
```

### Comparing `hysteresis-1.2.1/Hysteresis.egg-info/PKG-INFO` & `hysteresis-2.0.0/Hysteresis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hysteresis
-Version: 1.2.1
+Version: 2.0.0
 Summary: Hysteresis data processing tools
 Home-page: https://github.com/cslotboom/Hysteresis
 Author: Christian Slotboom
-Author-email: cslotboom@yahoo.com
+Author-email: christia.slotboom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 <h1 align = "Left">Hysteresis: Tools for Non-functional Curves.</h1>
 
 Hysteresis is a Python library made for analyzing non-functional curves, with an emphasis on force-deformation hystereses.
 While functions only have one direction, non-functional curves change direction, and each 'x' can be is mapped to more than one 'y'.
```

### Comparing `hysteresis-1.2.1/Hysteresis.egg-info/SOURCES.txt` & `hysteresis-2.0.0/Hysteresis.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 README.md
 license.txt
 setup.py
-Hysteresis/baseClass.py
 Hysteresis/baseFuncs.py
 Hysteresis/climate.py
 Hysteresis/compare.py
 Hysteresis/data.py
 Hysteresis/defaultDataFuncs.py
 Hysteresis/defaultPlotFuncs.py
 Hysteresis/protocol.py
 Hysteresis/resample.py
 Hysteresis.egg-info/PKG-INFO
 Hysteresis.egg-info/SOURCES.txt
 Hysteresis.egg-info/dependency_links.txt
 Hysteresis.egg-info/top_level.txt
 hysteresis/__init__.py
-hysteresis/baseClass.py
 hysteresis/baseFuncs.py
 hysteresis/climate.py
 hysteresis/compare.py
+hysteresis/curve.py
 hysteresis/data.py
 hysteresis/defaultDataFuncs.py
 hysteresis/defaultPlotFuncs.py
 hysteresis/env.py
 hysteresis/envelope.py
 hysteresis/protocol.py
 hysteresis/resample.py
```

### Comparing `hysteresis-1.2.1/PKG-INFO` & `hysteresis-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hysteresis
-Version: 1.2.1
+Version: 2.0.0
 Summary: Hysteresis data processing tools
 Home-page: https://github.com/cslotboom/Hysteresis
 Author: Christian Slotboom
-Author-email: cslotboom@yahoo.com
+Author-email: christia.slotboom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 <h1 align = "Left">Hysteresis: Tools for Non-functional Curves.</h1>
 
 Hysteresis is a Python library made for analyzing non-functional curves, with an emphasis on force-deformation hystereses.
 While functions only have one direction, non-functional curves change direction, and each 'x' can be is mapped to more than one 'y'.
```

### Comparing `hysteresis-1.2.1/README.md` & `hysteresis-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hysteresis-1.2.1/license.txt` & `hysteresis-2.0.0/license.txt`

 * *Files identical despite different names*

### Comparing `hysteresis-1.2.1/setup.py` & `hysteresis-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hysteresis",
-    version="1.2.1",
+    version="2.0.0",
     author="Christian Slotboom",
-    author_email="cslotboom@yahoo.com",
+    author_email="christia.slotboom@gmail.com",
     description="Hysteresis data processing tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cslotboom/Hysteresis",
     packages=setuptools.find_packages(),
     # package_dir = {'': 'Hysteresis'},
     classifiers=[
@@ -20,9 +20,9 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
     'numpy',
     'matplotlib',
     'scipy'
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.9',
 )
```

