# Comparing `tmp/mkdocs-walt-0.1.0.tar.gz` & `tmp/mkdocs-walt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-walt-0.1.0.tar", last modified: Wed May 31 19:05:18 2023, max compression
+gzip compressed data, was "mkdocs-walt-0.1.1.tar", last modified: Sun Jun  4 18:23:58 2023, max compression
```

## Comparing `mkdocs-walt-0.1.0.tar` & `mkdocs-walt-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-31 19:05:18.411700 mkdocs-walt-0.1.0/
--rw-r--r--   0 sue        (501) staff       (20)      145 2023-05-30 20:37:51.000000 mkdocs-walt-0.1.0/MANIFEST.in
--rw-r--r--   0 sue        (501) staff       (20)     1495 2023-05-31 19:05:18.411593 mkdocs-walt-0.1.0/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)     1063 2023-05-31 18:19:34.000000 mkdocs-walt-0.1.0/README.md
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-31 19:05:18.410909 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/
--rw-r--r--   0 sue        (501) staff       (20)     1495 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)      361 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/SOURCES.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/dependency_links.txt
--rw-r--r--   0 sue        (501) staff       (20)       28 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/entry_points.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-29 21:29:31.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/not-zip-safe
--rw-r--r--   0 sue        (501) staff       (20)        7 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/requires.txt
--rw-r--r--   0 sue        (501) staff       (20)        5 2023-05-31 19:05:18.000000 mkdocs-walt-0.1.0/mkdocs_walt.egg-info/top_level.txt
--rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-31 19:05:18.411733 mkdocs-walt-0.1.0/setup.cfg
--rw-r--r--   0 sue        (501) staff       (20)      872 2023-05-31 19:05:08.000000 mkdocs-walt-0.1.0/setup.py
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-31 19:05:18.411436 mkdocs-walt-0.1.0/walt/
--rw-r--r--   0 sue        (501) staff       (20)       29 2023-05-29 21:22:32.000000 mkdocs-walt-0.1.0/walt/__init__.py
--rw-r--r--   0 sue        (501) staff       (20)     3383 2023-05-31 18:42:35.000000 mkdocs-walt-0.1.0/walt/base.html
--rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-30 01:55:40.000000 mkdocs-walt-0.1.0/walt/main.html
--rw-r--r--   0 sue        (501) staff       (20)      189 2023-05-31 18:05:20.000000 mkdocs-walt-0.1.0/walt/mkdocs_theme.yml
--rw-r--r--   0 sue        (501) staff       (20)     5788 2023-05-31 18:44:58.000000 mkdocs-walt-0.1.0/walt/styles.css
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-06-04 18:23:58.922241 mkdocs-walt-0.1.1/
+-rw-r--r--   0 sue        (501) staff       (20)      145 2023-05-30 20:37:51.000000 mkdocs-walt-0.1.1/MANIFEST.in
+-rw-r--r--   0 sue        (501) staff       (20)     1772 2023-06-04 18:23:58.922078 mkdocs-walt-0.1.1/PKG-INFO
+-rw-r--r--   0 sue        (501) staff       (20)     1340 2023-06-04 18:23:26.000000 mkdocs-walt-0.1.1/README.md
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-06-04 18:23:58.919002 mkdocs-walt-0.1.1/mkdocs_walt.egg-info/
+-rw-r--r--   0 sue        (501) staff       (20)     1772 2023-06-04 18:23:58.000000 mkdocs-walt-0.1.1/mkdocs_walt.egg-info/PKG-INFO
+-rw-r--r--   0 sue        (501) staff       (20)      485 2023-06-04 18:23:58.000000 mkdocs-walt-0.1.1/mkdocs_walt.egg-info/SOURCES.txt
+-rw-r--r--   0 sue        (501) staff       (20)        1 2023-06-04 18:23:58.000000 mkdocs-walt-0.1.1/mkdocs_walt.egg-info/dependency_links.txt
+-rw-r--r--   0 sue        (501) staff       (20)       28 2023-06-04 18:23:58.000000 mkdocs-walt-0.1.1/mkdocs_walt.egg-info/entry_points.txt
+-rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-29 21:29:31.000000 mkdocs-walt-0.1.1/mkdocs_walt.egg-info/not-zip-safe
+-rw-r--r--   0 sue        (501) staff       (20)        7 2023-06-04 18:23:58.000000 mkdocs-walt-0.1.1/mkdocs_walt.egg-info/requires.txt
+-rw-r--r--   0 sue        (501) staff       (20)        5 2023-06-04 18:23:58.000000 mkdocs-walt-0.1.1/mkdocs_walt.egg-info/top_level.txt
+-rw-r--r--   0 sue        (501) staff       (20)       38 2023-06-04 18:23:58.922280 mkdocs-walt-0.1.1/setup.cfg
+-rw-r--r--   0 sue        (501) staff       (20)      872 2023-06-04 17:33:36.000000 mkdocs-walt-0.1.1/setup.py
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-06-04 18:23:58.920442 mkdocs-walt-0.1.1/walt/
+-rw-r--r--   0 sue        (501) staff       (20)       29 2023-05-29 21:22:32.000000 mkdocs-walt-0.1.1/walt/__init__.py
+-rw-r--r--   0 sue        (501) staff       (20)     3386 2023-06-04 14:27:45.000000 mkdocs-walt-0.1.1/walt/base.html
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-06-04 18:23:58.921500 mkdocs-walt-0.1.1/walt/highlightjs/
+-rw-r--r--   0 sue        (501) staff       (20)     1815 2023-06-03 22:48:37.000000 mkdocs-walt-0.1.1/walt/highlightjs/catppuccin-latte.min.css
+-rw-r--r--   0 sue        (501) staff       (20)     1823 2023-06-03 22:44:47.000000 mkdocs-walt-0.1.1/walt/highlightjs/catppuccin-macchiato.min.css
+-rw-r--r--   0 sue        (501) staff       (20)   121488 2023-06-03 22:23:51.000000 mkdocs-walt-0.1.1/walt/highlightjs/highlight.min.js
+-rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-30 01:55:40.000000 mkdocs-walt-0.1.1/walt/main.html
+-rw-r--r--   0 sue        (501) staff       (20)      234 2023-06-03 23:12:42.000000 mkdocs-walt-0.1.1/walt/mkdocs_theme.yml
+-rw-r--r--   0 sue        (501) staff       (20)     4543 2023-06-04 17:28:51.000000 mkdocs-walt-0.1.1/walt/walt.min.css
```

### Comparing `mkdocs-walt-0.1.0/PKG-INFO` & `mkdocs-walt-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-walt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A minimal theme for MkDocs
 Home-page: https://github.com/codesue/walt
 Author: Suzen Fylke
 Author-email: codesue@users.noreply.github.com
 License: MIT
 Keywords: mkdocs,mkdocs-theme,walt
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,16 @@
 It has the following features:
 
 - classless styles for semantic HTML based on [writ.css](https://writ.cmcenroe.me)
 - light mode and dark mode based on system settings
 - an emoji favicon for browsers that support svg site icons
 - code syntax highlighting using highlight.js
 
+<img src="https://raw.githubusercontent.com/codesue/walt/main/assets/images/mkdocs-walt-light.png" alt="Screenshot of the Walt website" />
+
 ## Installation
 
 ```sh
 pip install mkdocs-walt
 ```
 
 ## Usage
@@ -35,27 +37,32 @@
 project's `mkdocs.yml`:
 
 ```yaml
 theme:
   name: walt
 ```
 
-See the [full usage example](https://github.com/codesue/walt/examples/mkdocs).
+See the [end to end example](https://github.com/codesue/walt/tree/main/examples/mkdocs).
 
 ## Defaults
 
 Walt sets the following configurations by default:
 
 ```yaml
 site_emoji: 🍃
 locale: en
 theme_color: "hsl(0, 0%, 100%)"
 theme_color_dark: "hsl(232, 23%, 18%)"
 include_header: true
+include_nav: true
 highlightjs: true
 ```
 
+## License
+
+Copyright &copy; 2023 [Suzen Fylke](https://suzenfylke.com). Distributed under the MIT License.
+
 ## Acknowledgements
 
 Walt uses [writ.css](https://github.com/programble/writ/tree/master) for styles
 and [Catppuccin](https://github.com/catppuccin/catppuccin) for code block syntax
 highlighting and dark mode color palettes.
```

### Comparing `mkdocs-walt-0.1.0/README.md` & `mkdocs-walt-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 It has the following features:
 
 - classless styles for semantic HTML based on [writ.css](https://writ.cmcenroe.me)
 - light mode and dark mode based on system settings
 - an emoji favicon for browsers that support svg site icons
 - code syntax highlighting using highlight.js
 
+<img src="https://raw.githubusercontent.com/codesue/walt/main/assets/images/mkdocs-walt-light.png" alt="Screenshot of the Walt website" />
+
 ## Installation
 
 ```sh
 pip install mkdocs-walt
 ```
 
 ## Usage
@@ -21,27 +23,32 @@
 project's `mkdocs.yml`:
 
 ```yaml
 theme:
   name: walt
 ```
 
-See the [full usage example](https://github.com/codesue/walt/examples/mkdocs).
+See the [end to end example](https://github.com/codesue/walt/tree/main/examples/mkdocs).
 
 ## Defaults
 
 Walt sets the following configurations by default:
 
 ```yaml
 site_emoji: 🍃
 locale: en
 theme_color: "hsl(0, 0%, 100%)"
 theme_color_dark: "hsl(232, 23%, 18%)"
 include_header: true
+include_nav: true
 highlightjs: true
 ```
 
+## License
+
+Copyright &copy; 2023 [Suzen Fylke](https://suzenfylke.com). Distributed under the MIT License.
+
 ## Acknowledgements
 
 Walt uses [writ.css](https://github.com/programble/writ/tree/master) for styles
 and [Catppuccin](https://github.com/catppuccin/catppuccin) for code block syntax
 highlighting and dark mode color palettes.
```

### Comparing `mkdocs-walt-0.1.0/mkdocs_walt.egg-info/PKG-INFO` & `mkdocs-walt-0.1.1/mkdocs_walt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-walt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A minimal theme for MkDocs
 Home-page: https://github.com/codesue/walt
 Author: Suzen Fylke
 Author-email: codesue@users.noreply.github.com
 License: MIT
 Keywords: mkdocs,mkdocs-theme,walt
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,16 @@
 It has the following features:
 
 - classless styles for semantic HTML based on [writ.css](https://writ.cmcenroe.me)
 - light mode and dark mode based on system settings
 - an emoji favicon for browsers that support svg site icons
 - code syntax highlighting using highlight.js
 
+<img src="https://raw.githubusercontent.com/codesue/walt/main/assets/images/mkdocs-walt-light.png" alt="Screenshot of the Walt website" />
+
 ## Installation
 
 ```sh
 pip install mkdocs-walt
 ```
 
 ## Usage
@@ -35,27 +37,32 @@
 project's `mkdocs.yml`:
 
 ```yaml
 theme:
   name: walt
 ```
 
-See the [full usage example](https://github.com/codesue/walt/examples/mkdocs).
+See the [end to end example](https://github.com/codesue/walt/tree/main/examples/mkdocs).
 
 ## Defaults
 
 Walt sets the following configurations by default:
 
 ```yaml
 site_emoji: 🍃
 locale: en
 theme_color: "hsl(0, 0%, 100%)"
 theme_color_dark: "hsl(232, 23%, 18%)"
 include_header: true
+include_nav: true
 highlightjs: true
 ```
 
+## License
+
+Copyright &copy; 2023 [Suzen Fylke](https://suzenfylke.com). Distributed under the MIT License.
+
 ## Acknowledgements
 
 Walt uses [writ.css](https://github.com/programble/writ/tree/master) for styles
 and [Catppuccin](https://github.com/catppuccin/catppuccin) for code block syntax
 highlighting and dark mode color palettes.
```

### Comparing `mkdocs-walt-0.1.0/setup.py` & `mkdocs-walt-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 with open('README.md', 'r') as f:
   LONG_DESCRIPTION = f.read()
 
 setup(
     name='mkdocs-walt',
     version=VERSION,
```

### Comparing `mkdocs-walt-0.1.0/walt/base.html` & `mkdocs-walt-0.1.1/walt/base.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!doctype html>
+<!DOCTYPE html>
 <html lang="{{ config.theme.locale }}">
   <head>
     {%- block site_meta %}
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>{{ page.title or config.site_name }}</title>
     {% if config.site_description %}<meta name="description" content="{{ config.site_description }}">{% endif %}
@@ -14,31 +14,31 @@
 
     <meta name="color-scheme" content="light dark">
     <meta name="theme-color" content="{{ config.theme.theme_color }}" media="(prefers-color-scheme: light)">
     <meta name="theme-color" content="{{ config.theme.theme_color_dark }}" media="(prefers-color-scheme: dark)">
     {%- endblock %}
 
     {%- block styles %}
-    <link rel="stylesheet" href="{{ "styles.css"|url }}">
+    <link rel="stylesheet" href="{{ "walt.min.css"|url }}">
     {%- if config.theme.highlightjs %}
-    <link rel="stylesheet" href="//unpkg.com/@catppuccin/highlightjs/css/catppuccin-macchiato.css" media="(prefers-color-scheme: dark)">
-    <link rel="stylesheet" href="//unpkg.com/@catppuccin/highlightjs/css/catppuccin-latte.css" media="(prefers-color-scheme: light)">
+    <link rel="stylesheet" href="{{ "highlightjs/catppuccin-macchiato.min.css"|url }}" media="(prefers-color-scheme: dark)">
+    <link rel="stylesheet" href="{{ "highlightjs/catppuccin-latte.min.css"|url }}" media="(prefers-color-scheme: light)">
     <style>
       .hljs, code.hljs { background: unset; }
       code .hljs-comment { color: var(--color-secondary-text); }
     </style>
     {%- endif %}
     {% for path in config.extra_css %}
     <link href="{{ path|url }}" rel="stylesheet">
     {% endfor %}
     {%- endblock %}
 
     {%- block libs %}
     {%- if config.theme.highlightjs %}
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/highlight.min.js"></script>
+    <script src="{{ "highlightjs/highlight.min.js"|url }}"></script>
     {%- for lang in config.theme.hljs_languages %}
       <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.5.0/languages/{{lang}}.min.js"></script>
     {%- endfor %}
     <script>hljs.initHighlightingOnLoad();</script>
     {%- endif %}
     {%- endblock %}
 
@@ -47,22 +47,24 @@
   <body>
     <a href="#skip" class="visually-hidden">Skip to main content</a>
     {%- block header %}
     {%- if config.theme.include_header %}
     <header>
       <span class="site-name">{{ config.site_name }}</span>
       {% if config.site_description %}<p>{{ config.site_description }}</p>{% endif %}
+      {%- if config.theme.include_nav %}
       <nav>
         <h2 class="visually-hidden">Top level navigation menu</h2>
         <ul>
           {%- for nav_item in nav %}
           <li><a href="{{ nav_item.url|url }}">{{ nav_item.title }}</a></li>
           {%- endfor %}
         </ul>
       </nav>
+      {%- endif %}
     </header>
     {%- endif %}
     {%- endblock %}
     {%- block main %}
     <main id="skip">
       {{ page.content }}
     </main>
```

#### html2text {}

```diff
@@ -5,29 +5,31 @@
 {% endif %} {% if page and page.canonical_url %}
 {% endif %} {% if config.site_favicon %}
  {% else %}
 {% endif %}
 
 
  {%- endblock %} {%- block styles %}
-css"|url }}"> {%- if config.theme.highlightjs %}
-
+min.css"|url }}"> {%- if config.theme.highlightjs %}
+atppuccin-macchiato.min.css"|url }}" media="(prefers-color-scheme: dark)">
+atppuccin-latte.min.css"|url }}" media="(prefers-color-scheme: light)">
  {%- endif %} {% for path in config.extra_css %}
  {% endfor %} {%- endblock %} {%- block libs %} {%- if config.theme.highlightjs
 %}
- {%- for lang in config.theme.hljs_languages %}
+ighlight.min.js"|url }}">
+{%- for lang in config.theme.hljs_languages %}
  {%- endfor %}
  {%- endif %} {%- endblock %} {%- block extrahead %} {% endblock %}
 Skip_to_main_content {%- block header %} {%- if config.theme.include_header %}
 {{ config.site_name }} {% if config.site_description %}
 {{ config.site_description }}
-{% endif %}
+{% endif %} {%- if config.theme.include_nav %}
 ***** Top level navigation menu *****
     * {%- for nav_item in nav %}
     * {{_nav_item.title_}}
     * {%- endfor %}
-  {%- endif %} {%- endblock %} {%- block main %}  {{ page.content }}  {%-
-endblock %} {%- block footer %}  {%- if config.copyright %}
+ {%- endif %}  {%- endif %} {%- endblock %} {%- block main %}  {{ page.content
+}}  {%- endblock %} {%- block footer %}  {%- if config.copyright %}
 {{ config.copyright }}
 {%- endif %}  {%- endblock %} {%- block scripts %} {% for path in
 config.extra_javascript %}
  {% endfor %} {%- endblock %}
```

