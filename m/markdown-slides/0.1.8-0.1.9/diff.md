# Comparing `tmp/markdown-slides-0.1.8.tar.gz` & `tmp/markdown-slides-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-slides-0.1.8.tar", last modified: Mon Mar 20 19:36:12 2023, max compression
+gzip compressed data, was "markdown-slides-0.1.9.tar", last modified: Wed Mar 22 20:57:43 2023, max compression
```

## Comparing `markdown-slides-0.1.8.tar` & `markdown-slides-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:36:12.681844 markdown-slides-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-03-20 19:36:12.681844 markdown-slides-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:36:12.681844 markdown-slides-0.1.8/markdown_slides.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-03-20 19:36:12.000000 markdown-slides-0.1.8/markdown_slides.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-20 19:36:12.000000 markdown-slides-0.1.8/markdown_slides.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:36:12.000000 markdown-slides-0.1.8/markdown_slides.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-20 19:36:12.000000 markdown-slides-0.1.8/markdown_slides.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-20 19:36:12.000000 markdown-slides-0.1.8/markdown_slides.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-20 19:36:12.000000 markdown-slides-0.1.8/markdown_slides.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-20 19:36:12.685844 markdown-slides-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:36:12.681844 markdown-slides-0.1.8/slides/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/slides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/slides/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:36:12.681844 markdown-slides-0.1.8/slides/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/slides/demo/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/slides/demo/figure.png
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/slides/frontmatter.schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:36:12.681844 markdown-slides-0.1.8/slides/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:36:12.681844 markdown-slides-0.1.8/slides/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/slides/static/css/harvard.css
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/slides/static/css/slides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:36:12.681844 markdown-slides-0.1.8/slides/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/slides/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/slides/templates/slides.html
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-20 19:35:59.000000 markdown-slides-0.1.8/slides/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:57:43.316291 markdown-slides-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-03-22 20:57:43.316291 markdown-slides-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:57:43.316291 markdown-slides-0.1.9/markdown_slides.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-03-22 20:57:43.000000 markdown-slides-0.1.9/markdown_slides.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-22 20:57:43.000000 markdown-slides-0.1.9/markdown_slides.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 20:57:43.000000 markdown-slides-0.1.9/markdown_slides.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 20:57:43.000000 markdown-slides-0.1.9/markdown_slides.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-22 20:57:43.000000 markdown-slides-0.1.9/markdown_slides.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-22 20:57:43.000000 markdown-slides-0.1.9/markdown_slides.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-22 20:57:43.316291 markdown-slides-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:57:43.316291 markdown-slides-0.1.9/slides/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/slides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/slides/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:57:43.316291 markdown-slides-0.1.9/slides/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/slides/demo/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/slides/demo/figure.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/slides/frontmatter.schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:57:43.312291 markdown-slides-0.1.9/slides/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:57:43.316291 markdown-slides-0.1.9/slides/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/slides/static/css/harvard.css
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/slides/static/css/slides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 20:57:43.316291 markdown-slides-0.1.9/slides/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/slides/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/slides/templates/slides.html
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-22 20:57:30.000000 markdown-slides-0.1.9/slides/util.py
```

### Comparing `markdown-slides-0.1.8/LICENSE` & `markdown-slides-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-slides-0.1.8/PKG-INFO` & `markdown-slides-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-slides
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
 css: static/css/harvard.css
 title: Markdown Slides Demo
 ---
@@ -136,12 +136,22 @@
 | ---------- | -------------------------------------------------------- |
 | `$n$`      | Number of samples                                        |
 | `$x_{ij}$` | `$j^\text{th}$` covariate for the `$i^\text{th}$` sample |
 | `$y_i$`    | target for the `$i^\text{th}$` sample                    |
 
 ---
 
+- important
+- bullets
+
+and
+
+1. numbered
+2. items
+
+---
+
 [Jekyll-style frontmatter](https://jekyllrb.com/docs/front-matter/) can be used to configure the presentation. See [`slides/frontmatter.schema.yaml`](slides/frontmatter.schema.yaml) for details.
 
 ---
 
 Visit the [reveal.js website](https://revealjs.com/markdown/) for further information.
```

### Comparing `markdown-slides-0.1.8/README.md` & `markdown-slides-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -130,12 +130,22 @@
 | ---------- | -------------------------------------------------------- |
 | `$n$`      | Number of samples                                        |
 | `$x_{ij}$` | `$j^\text{th}$` covariate for the `$i^\text{th}$` sample |
 | `$y_i$`    | target for the `$i^\text{th}$` sample                    |
 
 ---
 
+- important
+- bullets
+
+and
+
+1. numbered
+2. items
+
+---
+
 [Jekyll-style frontmatter](https://jekyllrb.com/docs/front-matter/) can be used to configure the presentation. See [`slides/frontmatter.schema.yaml`](slides/frontmatter.schema.yaml) for details.
 
 ---
 
 Visit the [reveal.js website](https://revealjs.com/markdown/) for further information.
```

### Comparing `markdown-slides-0.1.8/markdown_slides.egg-info/PKG-INFO` & `markdown-slides-0.1.9/markdown_slides.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-slides
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
 css: static/css/harvard.css
 title: Markdown Slides Demo
 ---
@@ -136,12 +136,22 @@
 | ---------- | -------------------------------------------------------- |
 | `$n$`      | Number of samples                                        |
 | `$x_{ij}$` | `$j^\text{th}$` covariate for the `$i^\text{th}$` sample |
 | `$y_i$`    | target for the `$i^\text{th}$` sample                    |
 
 ---
 
+- important
+- bullets
+
+and
+
+1. numbered
+2. items
+
+---
+
 [Jekyll-style frontmatter](https://jekyllrb.com/docs/front-matter/) can be used to configure the presentation. See [`slides/frontmatter.schema.yaml`](slides/frontmatter.schema.yaml) for details.
 
 ---
 
 Visit the [reveal.js website](https://revealjs.com/markdown/) for further information.
```

### Comparing `markdown-slides-0.1.8/markdown_slides.egg-info/SOURCES.txt` & `markdown-slides-0.1.9/markdown_slides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `markdown-slides-0.1.8/setup.py` & `markdown-slides-0.1.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as fp:
     long_description = fp.read()
 
 
 setup(
     name="markdown-slides",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     install_requires=[
         "flask",
         "jsonschema",
         "python-frontmatter",
         "pyyaml",
     ],
```

### Comparing `markdown-slides-0.1.8/slides/__init__.py` & `markdown-slides-0.1.9/slides/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown-slides-0.1.8/slides/__main__.py` & `markdown-slides-0.1.9/slides/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown-slides-0.1.8/slides/demo/README.md` & `markdown-slides-0.1.9/slides/demo/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -130,12 +130,22 @@
 | ---------- | -------------------------------------------------------- |
 | `$n$`      | Number of samples                                        |
 | `$x_{ij}$` | `$j^\text{th}$` covariate for the `$i^\text{th}$` sample |
 | `$y_i$`    | target for the `$i^\text{th}$` sample                    |
 
 ---
 
+- important
+- bullets
+
+and
+
+1. numbered
+2. items
+
+---
+
 [Jekyll-style frontmatter](https://jekyllrb.com/docs/front-matter/) can be used to configure the presentation. See [`slides/frontmatter.schema.yaml`](slides/frontmatter.schema.yaml) for details.
 
 ---
 
 Visit the [reveal.js website](https://revealjs.com/markdown/) for further information.
```

### Comparing `markdown-slides-0.1.8/slides/demo/figure.png` & `markdown-slides-0.1.9/slides/demo/figure.png`

 * *Files identical despite different names*

### Comparing `markdown-slides-0.1.8/slides/frontmatter.schema.yaml` & `markdown-slides-0.1.9/slides/frontmatter.schema.yaml`

 * *Files identical despite different names*

### Comparing `markdown-slides-0.1.8/slides/static/css/harvard.css` & `markdown-slides-0.1.9/slides/static/css/harvard.css`

 * *Files 6% similar despite different names*

```diff
@@ -51,7 +51,19 @@
     border: #D6D6D7 solid;
     border-radius: 10px;
     /* needed for borders to show: https://stackoverflow.com/a/4932321/1150961 */
     border-collapse: separate;
     /* needed to avoid the child clipping the border: https://stackoverflow.com/a/3724210/1150961 */
     overflow: hidden;
 }
+
+.reveal ul {
+    list-style: none;
+}
+
+.reveal ul li::before {
+    color: var(--brand-color);
+    content: "⏵";
+    display: inline-block;
+    width: 1em;
+    margin-left: -1em;
+}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `markdown-slides-0.1.8/slides/templates/index.html` & `markdown-slides-0.1.9/slides/templates/index.html`

 * *Files identical despite different names*

### Comparing `markdown-slides-0.1.8/slides/templates/slides.html` & `markdown-slides-0.1.9/slides/templates/slides.html`

 * *Files identical despite different names*

### Comparing `markdown-slides-0.1.8/slides/util.py` & `markdown-slides-0.1.9/slides/util.py`

 * *Files identical despite different names*

