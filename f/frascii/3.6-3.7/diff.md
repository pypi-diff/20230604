# Comparing `tmp/frascii-3.6.tar.gz` & `tmp/frascii-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-3.6.tar", last modified: Sun Jun  4 20:49:11 2023, max compression
+gzip compressed data, was "frascii-3.7.tar", last modified: Sun Jun  4 20:53:56 2023, max compression
```

## Comparing `frascii-3.6.tar` & `frascii-3.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-06-04 20:49:11.965336 frascii-3.6/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    15243 2023-06-04 20:49:11.965336 frascii-3.6/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    13129 2023-05-09 09:13:45.000000 frascii-3.6/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-06-04 20:49:11.957336 frascii-3.6/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2134 2023-06-04 20:48:46.000000 frascii-3.6/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7940 2023-05-01 12:48:57.000000 frascii-3.6/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-06-04 20:49:11.965336 frascii-3.6/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-3.6/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-3.6/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-3.6/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-3.6/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-3.6/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3926 2023-06-04 20:46:32.000000 frascii-3.6/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-3.6/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     4110 2023-04-29 14:01:04.000000 frascii-3.6/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3766 2023-06-04 20:45:43.000000 frascii-3.6/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-3.6/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-3.6/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-3.6/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-3.6/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-06-04 20:49:11.961336 frascii-3.6/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    15243 2023-06-04 20:49:11.000000 frascii-3.6/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-06-04 20:49:11.000000 frascii-3.6/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-06-04 20:49:11.000000 frascii-3.6/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-06-04 20:49:11.000000 frascii-3.6/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-06-04 20:49:11.000000 frascii-3.6/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-06-04 20:49:11.965336 frascii-3.6/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      572 2023-06-04 20:49:09.000000 frascii-3.6/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-06-04 20:53:56.814739 frascii-3.7/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    15243 2023-06-04 20:53:56.818739 frascii-3.7/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    13129 2023-05-09 09:13:45.000000 frascii-3.7/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-06-04 20:53:56.814739 frascii-3.7/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2134 2023-06-04 20:53:47.000000 frascii-3.7/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7940 2023-05-01 12:48:57.000000 frascii-3.7/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-06-04 20:53:56.814739 frascii-3.7/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-3.7/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-3.7/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-3.7/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-3.7/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-3.7/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3928 2023-06-04 20:52:58.000000 frascii-3.7/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-3.7/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     4110 2023-04-29 14:01:04.000000 frascii-3.7/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3766 2023-06-04 20:52:43.000000 frascii-3.7/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-3.7/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-3.7/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-3.7/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-3.7/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-06-04 20:53:56.814739 frascii-3.7/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    15243 2023-06-04 20:53:56.000000 frascii-3.7/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-06-04 20:53:56.000000 frascii-3.7/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-06-04 20:53:56.000000 frascii-3.7/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-06-04 20:53:56.000000 frascii-3.7/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-06-04 20:53:56.000000 frascii-3.7/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-06-04 20:53:56.818739 frascii-3.7/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      572 2023-06-04 20:49:09.000000 frascii-3.7/setup.py
```

### Comparing `frascii-3.6/PKG-INFO` & `frascii-3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frascii
-Version: 3.6
+Version: 3.7
 Summary: UNKNOWN
 Home-page: https://github.com/LuggiStruggi/Frascii.git
 Author: Lukas König
 Author-email: lukasmkoenig@gmx.net
 License: UNKNOWN
 Description: # Frascii
         ASCII-visualizations of Fractals for the Ubuntu (or other) Terminal
```

### Comparing `frascii-3.6/README.md` & `frascii-3.7/README.md`

 * *Files identical despite different names*

### Comparing `frascii-3.6/frascii/__init__.py` & `frascii-3.7/frascii/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
 from frascii.fractals.l_system import l_system_string, l_system_animate
 
-__version__ = '3.6'
+__version__ = '3.7'
 
 def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
 	if explore:
 		x, y, x_radius, y_radius, stepsize, max_iter, style, grid = mandelbrot_explore(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
 def julia(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
```

### Comparing `frascii-3.6/frascii/commands.py` & `frascii-3.7/frascii/commands.py`

 * *Files identical despite different names*

### Comparing `frascii-3.6/frascii/fractals/dragon_curve.py` & `frascii-3.7/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.6/frascii/fractals/fibonacci.py` & `frascii-3.7/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-3.6/frascii/fractals/hilbert_curve.py` & `frascii-3.7/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.6/frascii/fractals/julia.py` & `frascii-3.7/frascii/fractals/julia.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,20 +63,20 @@
 		nonlocal grid
 		nonlocal i
 		nonlocal f
 		styles = ["non-repeating", "repeating"]
 		si = 0 if style == "non-repeating" else 1
  	
 		while True:
-			stdscr.clear()
+			#stdscr.clear()
 			rows, cols = stdscr.getmaxyx()
 			y_rad = min(y_radius, rows//2-1)
 			x_rad = min(x_radius, cols//(2 if grid == "rect" else 4)-1)
 			stdscr.addstr(0, 0, julia_string(f, x, y, x_rad, y_rad, s, i, styles[si], grid))
-			stdscr.refresh()
+			#stdscr.refresh()
 			key = stdscr.getch()
 			curses.flushinp()
 			if key == curses.KEY_RIGHT:
 				x += 5*s
 			elif key == curses.KEY_LEFT:
 				x -= 5*s
 			elif key == curses.KEY_UP:
```

### Comparing `frascii-3.6/frascii/fractals/koch.py` & `frascii-3.7/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-3.6/frascii/fractals/l_system.py` & `frascii-3.7/frascii/fractals/l_system.py`

 * *Files identical despite different names*

### Comparing `frascii-3.6/frascii/fractals/mandelbrot.py` & `frascii-3.7/frascii/fractals/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `frascii-3.6/frascii/fractals/peano_curve.py` & `frascii-3.7/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.6/frascii/fractals/sierpinski_carpet.py` & `frascii-3.7/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-3.6/frascii.egg-info/PKG-INFO` & `frascii-3.7/frascii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frascii
-Version: 3.6
+Version: 3.7
 Summary: UNKNOWN
 Home-page: https://github.com/LuggiStruggi/Frascii.git
 Author: Lukas König
 Author-email: lukasmkoenig@gmx.net
 License: UNKNOWN
 Description: # Frascii
         ASCII-visualizations of Fractals for the Ubuntu (or other) Terminal
```

### Comparing `frascii-3.6/frascii.egg-info/SOURCES.txt` & `frascii-3.7/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frascii-3.6/setup.py` & `frascii-3.7/setup.py`

 * *Files identical despite different names*

