# Comparing `tmp/hockey_rink-1.0.1.tar.gz` & `tmp/hockey_rink-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hockey_rink-1.0.1.tar", last modified: Sat Mar 18 21:27:11 2023, max compression
+gzip compressed data, was "dist\hockey_rink-1.0.2.tar", last modified: Sat Jun  3 23:34:36 2023, max compression
```

## Comparing `hockey_rink-1.0.1.tar` & `hockey_rink-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-18 21:27:11.000000 hockey_rink-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-03-18 21:27:11.000000 hockey_rink-1.0.1/hockey_rink/
--rw-rw-rw-   0        0        0    27752 2023-03-15 01:16:54.000000 hockey_rink-1.0.1/hockey_rink/rink.py
--rw-rw-rw-   0        0        0    35015 2023-03-15 01:16:54.000000 hockey_rink-1.0.1/hockey_rink/rink_feature.py
--rw-rw-rw-   0        0        0    16226 2023-03-18 21:26:50.000000 hockey_rink-1.0.1/hockey_rink/_base_rink.py
--rw-rw-rw-   0        0        0    58582 2023-03-15 01:16:54.000000 hockey_rink-1.0.1/hockey_rink/_rink_plot.py
--rw-rw-rw-   0        0        0       50 2023-02-24 01:09:03.000000 hockey_rink-1.0.1/hockey_rink/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-18 21:27:11.000000 hockey_rink-1.0.1/hockey_rink.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-18 21:27:10.000000 hockey_rink-1.0.1/hockey_rink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-18 21:27:10.000000 hockey_rink-1.0.1/hockey_rink.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     7507 2023-03-18 21:27:10.000000 hockey_rink-1.0.1/hockey_rink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-03-18 21:27:10.000000 hockey_rink-1.0.1/hockey_rink.egg-info/requires.txt
--rw-rw-rw-   0        0        0      358 2023-03-18 21:27:11.000000 hockey_rink-1.0.1/hockey_rink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-03-18 21:27:10.000000 hockey_rink-1.0.1/hockey_rink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2021-05-12 20:26:17.000000 hockey_rink-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     7507 2023-03-18 21:27:11.000000 hockey_rink-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5591 2023-03-16 00:08:45.000000 hockey_rink-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-18 21:27:11.000000 hockey_rink-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      879 2023-03-18 21:26:50.000000 hockey_rink-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:34:36.000000 hockey_rink-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-03 23:34:36.000000 hockey_rink-1.0.2/hockey_rink/
+-rw-rw-rw-   0        0        0    27752 2023-03-15 01:16:54.000000 hockey_rink-1.0.2/hockey_rink/rink.py
+-rw-rw-rw-   0        0        0    35015 2023-03-15 01:16:54.000000 hockey_rink-1.0.2/hockey_rink/rink_feature.py
+-rw-rw-rw-   0        0        0    16226 2023-03-18 21:26:50.000000 hockey_rink-1.0.2/hockey_rink/_base_rink.py
+-rw-rw-rw-   0        0        0    58685 2023-06-03 23:31:04.000000 hockey_rink-1.0.2/hockey_rink/_rink_plot.py
+-rw-rw-rw-   0        0        0       50 2023-02-24 01:09:03.000000 hockey_rink-1.0.2/hockey_rink/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:34:36.000000 hockey_rink-1.0.2/hockey_rink.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-03 23:34:35.000000 hockey_rink-1.0.2/hockey_rink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-18 21:27:10.000000 hockey_rink-1.0.2/hockey_rink.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     7507 2023-06-03 23:34:35.000000 hockey_rink-1.0.2/hockey_rink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-06-03 23:34:35.000000 hockey_rink-1.0.2/hockey_rink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      358 2023-06-03 23:34:35.000000 hockey_rink-1.0.2/hockey_rink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-06-03 23:34:35.000000 hockey_rink-1.0.2/hockey_rink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2021-05-12 20:26:17.000000 hockey_rink-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     7507 2023-06-03 23:34:36.000000 hockey_rink-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5591 2023-03-16 00:08:45.000000 hockey_rink-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 23:34:36.000000 hockey_rink-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-06-03 23:31:04.000000 hockey_rink-1.0.2/setup.py
```

### Comparing `hockey_rink-1.0.1/hockey_rink/rink.py` & `hockey_rink-1.0.2/hockey_rink/rink.py`

 * *Files identical despite different names*

### Comparing `hockey_rink-1.0.1/hockey_rink/rink_feature.py` & `hockey_rink-1.0.2/hockey_rink/rink_feature.py`

 * *Files identical despite different names*

### Comparing `hockey_rink-1.0.1/hockey_rink/_base_rink.py` & `hockey_rink-1.0.2/hockey_rink/_base_rink.py`

 * *Files identical despite different names*

### Comparing `hockey_rink-1.0.1/hockey_rink/_rink_plot.py` & `hockey_rink-1.0.2/hockey_rink/_rink_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,18 +549,17 @@
         pre_children = ax.get_children()
 
         if is_ax_fn:
             plot_image = fn(*args, **kwargs)
         else:
             plot_image = fn(*args, **kwargs, ax=ax)
 
-        plot_features = [child for child in ax.get_children() if child not in pre_children]
-
         # Have to use set_clip_path because including clip_path in above updates axis limits.
         if clip_to_boards:
+            plot_features = [child for child in ax.get_children() if child not in pre_children]
             self.clip_plot(plot_features, ax, plot_range, plot_xlim, plot_ylim)
 
         return plot_image
 
     def scatter(
         self,
         x, y,
@@ -988,14 +987,17 @@
         img = ax.hexbin(**kwargs)
 
         # Rotate vertices and transform offsets.
         hexagon = img.get_paths()[0]
         hexagon.vertices = rotation.transform(hexagon.vertices)
         img.set_offsets(transform.transform(img.get_offsets()))
 
+        if clip_to_boards:
+            self.clip_plot(img, ax, plot_range, plot_xlim, plot_ylim)
+
         return img
 
     def heatmap(
         self,
         x, y, values=None,
         nbins=10, binsize=None,
         reduce_fn=np.mean, fill_value=np.nan,
```

### Comparing `hockey_rink-1.0.1/hockey_rink.egg-info/PKG-INFO` & `hockey_rink-1.0.2/hockey_rink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hockey-rink
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library for plotting hockey rinks with Matplotlib.
 Home-page: https://github.com/the-bucketless/hockey_rink
 Author: The Bucketless
 Author-email: thebucketless@protonmail.com
 License: GNU General Public License v3 (GPLv3)
 Description: ![](images/hockey-rink-logo.png)
```

### Comparing `hockey_rink-1.0.1/LICENSE` & `hockey_rink-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hockey_rink-1.0.1/PKG-INFO` & `hockey_rink-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hockey_rink
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library for plotting hockey rinks with Matplotlib.
 Home-page: https://github.com/the-bucketless/hockey_rink
 Author: The Bucketless
 Author-email: thebucketless@protonmail.com
 License: GNU General Public License v3 (GPLv3)
 Description: ![](images/hockey-rink-logo.png)
```

### Comparing `hockey_rink-1.0.1/README.md` & `hockey_rink-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hockey_rink-1.0.1/setup.py` & `hockey_rink-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="hockey_rink",
-    version="1.0.1",
+    version="1.0.2",
     description="A Python library for plotting hockey rinks with Matplotlib.",
     long_description_content_type="text/markdown",
     long_description=readme,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Framework :: Matplotlib",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

