# Comparing `tmp/mkdocstrings_python-1.1.1.tar.gz` & `tmp/mkdocstrings_python-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings_python-1.1.1.tar", last modified: Sun Jun  4 14:01:35 2023, max compression
+gzip compressed data, was "mkdocstrings_python-1.1.2.tar", last modified: Sun Jun  4 16:19:11 2023, max compression
```

## Comparing `mkdocstrings_python-1.1.1.tar` & `mkdocstrings_python-1.1.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      754 2023-06-02 14:47:59.880294 mkdocstrings_python-1.1.1/LICENSE
--rw-r--r--   0        0        0     4243 2023-06-02 14:48:02.626927 mkdocstrings_python-1.1.1/README.md
--rw-r--r--   0        0        0     2604 2023-06-04 14:01:35.369317 mkdocstrings_python-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-02 14:47:59.736962 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/py.typed
--rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/__init__.py
--rw-r--r--   0        0        0    18098 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/handler.py
--rw-r--r--   0        0        0     7871 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/rendering.py
--rw-r--r--   0        0        0     2532 2022-04-29 13:33:38.953329 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
--rw-r--r--   0        0        0     5036 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/children.html
--rw-r--r--   0        0        0     4078 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/class.html
--rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
--rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
--rw-r--r--   0        0        0     2687 2023-06-04 13:03:08.238478 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
--rw-r--r--   0        0        0      400 2022-03-01 18:29:05.585970 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
--rw-r--r--   0        0        0     2697 2023-06-04 13:02:56.049085 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
--rw-r--r--   0        0        0     3356 2023-06-04 13:02:13.028507 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
--rw-r--r--   0        0        0     2346 2023-06-04 13:02:01.977392 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
--rw-r--r--   0        0        0     3333 2023-06-04 13:01:52.305968 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
--rw-r--r--   0        0        0     3301 2023-06-04 13:01:34.118570 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
--rw-r--r--   0        0        0     2329 2023-06-04 13:01:20.797497 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
--rw-r--r--   0        0        0     3273 2023-06-04 13:01:08.835791 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
--rw-r--r--   0        0        0      674 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
--rw-r--r--   0        0        0     2436 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/function.html
--rw-r--r--   0        0        0      245 2022-05-08 08:40:49.298304 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
--rw-r--r--   0        0        0     1852 2022-04-29 17:36:56.831573 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/module.html
--rw-r--r--   0        0        0     2698 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/attribute.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/children.html
--rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/class.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring.html
--rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
--rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
--rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
--rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
--rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
--rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
--rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
--rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
--rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/expression.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/function.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/labels.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/module.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/signature.html
--rw-r--r--   0        0        0      623 2023-06-03 23:07:22.728595 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/style.css
--rw-r--r--   0        0        0      928 2023-06-04 13:03:39.709252 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
--rw-r--r--   0        0        0      934 2023-06-04 13:03:43.052249 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
--rw-r--r--   0        0        0      928 2023-06-03 22:45:13.311332 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
--rw-r--r--   0        0        0      868 2023-06-04 13:03:48.958295 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
--rw-r--r--   0        0        0     1058 2023-06-04 13:03:52.714552 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
--rw-r--r--   0        0        0     1007 2023-06-04 13:03:57.017402 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
--rw-r--r--   0        0        0      863 2023-06-04 13:04:01.126928 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
--rw-r--r--   0        0        0     1040 2023-06-04 13:04:04.606518 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
--rw-r--r--   0        0        0      971 2023-06-03 23:04:52.858439 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
--rw-r--r--   0        0        0      174 2023-06-02 14:47:59.730296 mkdocstrings_python-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3042 2023-06-02 14:48:02.626927 mkdocstrings_python-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0     3222 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.1/tests/test_handler.py
--rw-r--r--   0        0        0     1975 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.1/tests/test_rendering.py
--rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.1/tests/test_themes.py
--rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 mkdocstrings_python-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-06-02 14:47:59.880294 mkdocstrings_python-1.1.2/LICENSE
+-rw-r--r--   0        0        0     4243 2023-06-02 14:48:02.626927 mkdocstrings_python-1.1.2/README.md
+-rw-r--r--   0        0        0     2604 2023-06-04 16:19:11.833706 mkdocstrings_python-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 14:47:59.736962 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/py.typed
+-rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/__init__.py
+-rw-r--r--   0        0        0    18098 2023-06-04 16:11:57.811980 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/handler.py
+-rw-r--r--   0        0        0     7871 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/rendering.py
+-rw-r--r--   0        0        0     2532 2022-04-29 13:33:38.953329 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
+-rw-r--r--   0        0        0     5036 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/children.html
+-rw-r--r--   0        0        0     4078 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/class.html
+-rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
+-rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
+-rw-r--r--   0        0        0     2687 2023-06-04 13:03:08.238478 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
+-rw-r--r--   0        0        0      400 2022-03-01 18:29:05.585970 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
+-rw-r--r--   0        0        0     2697 2023-06-04 13:02:56.049085 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
+-rw-r--r--   0        0        0     3356 2023-06-04 13:02:13.028507 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
+-rw-r--r--   0        0        0     2346 2023-06-04 13:02:01.977392 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
+-rw-r--r--   0        0        0     3333 2023-06-04 13:01:52.305968 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
+-rw-r--r--   0        0        0     3301 2023-06-04 13:01:34.118570 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
+-rw-r--r--   0        0        0     2329 2023-06-04 13:01:20.797497 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
+-rw-r--r--   0        0        0     3273 2023-06-04 13:01:08.835791 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
+-rw-r--r--   0        0        0      674 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
+-rw-r--r--   0        0        0     2436 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/function.html
+-rw-r--r--   0        0        0      245 2022-05-08 08:40:49.298304 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
+-rw-r--r--   0        0        0     1852 2022-04-29 17:36:56.831573 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/module.html
+-rw-r--r--   0        0        0     2698 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/attribute.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/children.html
+-rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/class.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring.html
+-rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
+-rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
+-rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
+-rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
+-rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
+-rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
+-rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
+-rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
+-rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/expression.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/function.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/labels.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/module.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/signature.html
+-rw-r--r--   0        0        0      999 2023-06-04 16:06:08.029138 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/style.css
+-rw-r--r--   0        0        0      928 2023-06-04 13:03:39.709252 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
+-rw-r--r--   0        0        0      934 2023-06-04 13:03:43.052249 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
+-rw-r--r--   0        0        0      928 2023-06-03 22:45:13.311332 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
+-rw-r--r--   0        0        0      868 2023-06-04 13:03:48.958295 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
+-rw-r--r--   0        0        0     1058 2023-06-04 13:03:52.714552 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
+-rw-r--r--   0        0        0     1007 2023-06-04 13:03:57.017402 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
+-rw-r--r--   0        0        0      863 2023-06-04 13:04:01.126928 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
+-rw-r--r--   0        0        0     1040 2023-06-04 13:04:04.606518 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
+-rw-r--r--   0        0        0      971 2023-06-03 23:04:52.858439 mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
+-rw-r--r--   0        0        0      174 2023-06-02 14:47:59.730296 mkdocstrings_python-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     3042 2023-06-02 14:48:02.626927 mkdocstrings_python-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     3222 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.2/tests/test_handler.py
+-rw-r--r--   0        0        0     1975 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.2/tests/test_rendering.py
+-rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.2/tests/test_themes.py
+-rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 mkdocstrings_python-1.1.2/PKG-INFO
```

### Comparing `mkdocstrings_python-1.1.1/LICENSE` & `mkdocstrings_python-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/README.md` & `mkdocstrings_python-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/pyproject.toml` & `mkdocstrings_python-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "mkdocstrings>=0.20",
     "griffe>=0.24",
 ]
-version = "1.1.1"
+version = "1.1.2"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://mkdocstrings.github.io/python"
 Documentation = "https://mkdocstrings.github.io/python"
```

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/handler.py` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/rendering.py` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/rendering.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/children.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/children.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/class.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/class.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/expression.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/expression.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/function.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/function.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/module.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/module.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/signature.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/material/_base/signature.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/style.css` & `mkdocstrings_python-1.1.2/src/mkdocstrings_handlers/python/templates/readthedocs/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/tests/conftest.py` & `mkdocstrings_python-1.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/tests/test_handler.py` & `mkdocstrings_python-1.1.2/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/tests/test_rendering.py` & `mkdocstrings_python-1.1.2/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/tests/test_themes.py` & `mkdocstrings_python-1.1.2/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.1/PKG-INFO` & `mkdocstrings_python-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocstrings-python
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python handler for mkdocstrings.
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.1.1 Summary: A
+Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.1.2 Summary: A
 Python handler for mkdocstrings. Author-Email: TimothÃ©e Mazzucotelli
 pm.me> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

