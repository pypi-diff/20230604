# Comparing `tmp/webint_posts-0.0.8.tar.gz` & `tmp/webint_posts-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_posts-0.0.8.tar", max compression
+gzip compressed data, was "webint_posts-0.0.9.tar", max compression
```

## Comparing `webint_posts-0.0.8.tar` & `webint_posts-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      900 2023-02-24 02:09:24.410034 webint_posts-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    25190 2023-02-23 00:33:49.360321 webint_posts-0.0.8/webint_posts/__init__.py
--rw-r--r--   0        0        0      250 2023-02-22 23:33:20.428459 webint_posts-0.0.8/webint_posts/templates/__init__.py
--rw-r--r--   0        0        0       85 2023-02-14 23:35:28.168637 webint_posts-0.0.8/webint_posts/templates/access_denied.html
--rw-r--r--   0        0        0      759 2023-01-27 00:43:31.455968 webint_posts-0.0.8/webint_posts/templates/activity.html
--rw-r--r--   0        0        0     1157 2023-01-27 00:43:31.463969 webint_posts-0.0.8/webint_posts/templates/card.html
--rw-r--r--   0        0        0      441 2023-01-27 00:43:31.459968 webint_posts-0.0.8/webint_posts/templates/cards.html
--rw-r--r--   0        0        0      230 2023-01-27 00:43:31.463969 webint_posts-0.0.8/webint_posts/templates/channel.html
--rw-r--r--   0        0        0      631 2023-01-27 00:43:31.459968 webint_posts-0.0.8/webint_posts/templates/channels.html
--rw-r--r--   0        0        0      251 2023-02-22 23:50:41.408426 webint_posts-0.0.8/webint_posts/templates/day.html
--rw-r--r--   0        0        0      466 2023-01-27 00:43:31.459968 webint_posts-0.0.8/webint_posts/templates/entries.html
--rw-r--r--   0        0        0     6770 2023-02-23 00:34:11.556601 webint_posts-0.0.8/webint_posts/templates/entry.html
--rw-r--r--   0        0        0       49 2023-02-14 23:35:28.168637 webint_posts-0.0.8/webint_posts/templates/entry_not_found.html
--rw-r--r--   0        0        0      241 2023-02-22 23:50:16.428113 webint_posts-0.0.8/webint_posts/templates/month.html
--rw-r--r--   0        0        0      369 2023-01-27 00:43:31.463969 webint_posts-0.0.8/webint_posts/templates/render_dict.html
--rw-r--r--   0        0        0      223 2023-01-27 00:43:31.459968 webint_posts-0.0.8/webint_posts/templates/rooms.html
--rw-r--r--   0        0        0      322 2023-01-27 00:43:31.459968 webint_posts-0.0.8/webint_posts/templates/syndication.html
--rw-r--r--   0        0        0      227 2023-02-22 23:49:39.839655 webint_posts-0.0.8/webint_posts/templates/year.html
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 webint_posts-0.0.8/setup.py
--rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 webint_posts-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-03-08 03:54:19.584246 webint_posts-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    25190 2023-02-23 00:33:49.360321 webint_posts-0.0.9/webint_posts/__init__.py
+-rw-r--r--   0        0        0      250 2023-02-22 23:33:20.428459 webint_posts-0.0.9/webint_posts/templates/__init__.py
+-rw-r--r--   0        0        0       85 2023-02-14 23:35:28.168637 webint_posts-0.0.9/webint_posts/templates/access_denied.html
+-rw-r--r--   0        0        0      745 2023-03-08 03:49:47.540320 webint_posts-0.0.9/webint_posts/templates/activity.html
+-rw-r--r--   0        0        0     1157 2023-01-27 00:43:31.463969 webint_posts-0.0.9/webint_posts/templates/card.html
+-rw-r--r--   0        0        0      441 2023-01-27 00:43:31.459968 webint_posts-0.0.9/webint_posts/templates/cards.html
+-rw-r--r--   0        0        0      230 2023-01-27 00:43:31.463969 webint_posts-0.0.9/webint_posts/templates/channel.html
+-rw-r--r--   0        0        0      631 2023-01-27 00:43:31.459968 webint_posts-0.0.9/webint_posts/templates/channels.html
+-rw-r--r--   0        0        0      251 2023-02-22 23:50:41.408426 webint_posts-0.0.9/webint_posts/templates/day.html
+-rw-r--r--   0        0        0      466 2023-01-27 00:43:31.459968 webint_posts-0.0.9/webint_posts/templates/entries.html
+-rw-r--r--   0        0        0     6770 2023-02-23 00:34:11.556601 webint_posts-0.0.9/webint_posts/templates/entry.html
+-rw-r--r--   0        0        0       49 2023-02-14 23:35:28.168637 webint_posts-0.0.9/webint_posts/templates/entry_not_found.html
+-rw-r--r--   0        0        0      241 2023-02-22 23:50:16.428113 webint_posts-0.0.9/webint_posts/templates/month.html
+-rw-r--r--   0        0        0      369 2023-01-27 00:43:31.463969 webint_posts-0.0.9/webint_posts/templates/render_dict.html
+-rw-r--r--   0        0        0      223 2023-01-27 00:43:31.459968 webint_posts-0.0.9/webint_posts/templates/rooms.html
+-rw-r--r--   0        0        0      322 2023-01-27 00:43:31.459968 webint_posts-0.0.9/webint_posts/templates/syndication.html
+-rw-r--r--   0        0        0      227 2023-02-22 23:49:39.839655 webint_posts-0.0.9/webint_posts/templates/year.html
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 webint_posts-0.0.9/setup.py
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 webint_posts-0.0.9/PKG-INFO
```

### Comparing `webint_posts-0.0.8/pyproject.toml` & `webint_posts-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-posts"
-version = "0.0.8"
+version = "0.0.9"
 description = "manage posts on your website"
 keywords = ["IndieWeb", "Micropub"]
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
 packages = [{include = "webint_posts"}]
 
 [tool.poetry.plugins."webapps"]
```

### Comparing `webint_posts-0.0.8/webint_posts/__init__.py` & `webint_posts-0.0.9/webint_posts/__init__.py`

 * *Files identical despite different names*

### Comparing `webint_posts-0.0.8/webint_posts/templates/card.html` & `webint_posts-0.0.9/webint_posts/templates/card.html`

 * *Files identical despite different names*

### Comparing `webint_posts-0.0.8/webint_posts/templates/channels.html` & `webint_posts-0.0.9/webint_posts/templates/channels.html`

 * *Files identical despite different names*

### Comparing `webint_posts-0.0.8/webint_posts/templates/entry.html` & `webint_posts-0.0.9/webint_posts/templates/entry.html`

 * *Files identical despite different names*

### Comparing `webint_posts-0.0.8/setup.py` & `webint_posts-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['micropub>=0.0', 'webint>=0.0']
 
 entry_points = \
 {'webapps': ['posts = webint_posts:app']}
 
 setup_kwargs = {
     'name': 'webint-posts',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'manage posts on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

