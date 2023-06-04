# Comparing `tmp/mkdocstrings_python-1.1.0.tar.gz` & `tmp/mkdocstrings_python-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings_python-1.1.0.tar", last modified: Fri May 26 11:01:50 2023, max compression
+gzip compressed data, was "mkdocstrings_python-1.1.1.tar", last modified: Sun Jun  4 14:01:35 2023, max compression
```

## Comparing `mkdocstrings_python-1.1.0.tar` & `mkdocstrings_python-1.1.1.tar`

### file list

```diff
@@ -1,64 +1,61 @@
--rw-r--r--   0        0        0      754 2023-05-16 10:40:20.986168 mkdocstrings_python-1.1.0/LICENSE
--rw-r--r--   0        0        0     4243 2023-05-16 10:41:07.688645 mkdocstrings_python-1.1.0/README.md
--rw-r--r--   0        0        0     2604 2023-05-26 11:01:50.845735 mkdocstrings_python-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 10:40:20.579508 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/py.typed
--rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/__init__.py
--rw-r--r--   0        0        0    18098 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/handler.py
--rw-r--r--   0        0        0     7871 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/rendering.py
--rw-r--r--   0        0        0     2532 2022-04-29 13:33:38.953329 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
--rw-r--r--   0        0        0     5036 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html
--rw-r--r--   0        0        0     4078 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html
--rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
--rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
--rw-r--r--   0        0        0     2465 2022-04-29 23:09:02.903315 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
--rw-r--r--   0        0        0      400 2022-03-01 18:29:05.585970 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
--rw-r--r--   0        0        0     2475 2022-04-29 23:09:07.859915 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
--rw-r--r--   0        0        0     3134 2022-04-29 23:09:10.543213 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
--rw-r--r--   0        0        0     2132 2022-04-29 23:09:12.233190 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
--rw-r--r--   0        0        0     3111 2022-04-29 23:09:14.279830 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
--rw-r--r--   0        0        0     3081 2022-04-29 23:09:16.163138 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
--rw-r--r--   0        0        0     2115 2022-04-29 23:09:18.059779 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
--rw-r--r--   0        0        0     3051 2022-04-29 23:09:20.759743 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
--rw-r--r--   0        0        0      674 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
--rw-r--r--   0        0        0     2436 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html
--rw-r--r--   0        0        0      245 2022-05-08 08:40:49.298304 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
--rw-r--r--   0        0        0     1852 2022-04-29 17:36:56.831573 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html
--rw-r--r--   0        0        0     2698 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/attribute.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/children.html
--rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/class.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring.html
--rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
--rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
--rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
--rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
--rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
--rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
--rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
--rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
--rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
--rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/expression.html
--rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/function.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/labels.html
--rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/module.html
--rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/signature.html
--rw-r--r--   0        0        0      703 2022-03-03 18:21:59.514950 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/style.css
--rw-r--r--   0        0        0      224 2021-10-30 13:54:10.019274 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/exceptions.html
--rw-r--r--   0        0        0      277 2021-10-30 13:54:10.202605 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/keyword_args.html
--rw-r--r--   0        0        0      293 2021-10-30 13:54:10.019274 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/parameters.html
--rw-r--r--   0        0        0      200 2021-10-30 13:54:10.092606 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/return.html
--rw-r--r--   0        0        0      137 2021-10-30 13:54:10.199272 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/style.css
--rw-r--r--   0        0        0      196 2021-10-30 13:54:10.202605 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/mkdocs/yield.html
--rw-r--r--   0        0        0      545 2021-10-30 13:54:09.842609 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/exceptions.html
--rw-r--r--   0        0        0      601 2021-11-06 17:58:09.459000 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html
--rw-r--r--   0        0        0      618 2021-11-06 17:59:12.206399 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/parameters.html
--rw-r--r--   0        0        0      494 2021-11-06 17:58:14.115000 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/returns.html
--rw-r--r--   0        0        0      600 2021-10-30 13:54:09.942608 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
--rw-r--r--   0        0        0      490 2021-11-06 17:58:20.568000 mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/yields.html
--rw-r--r--   0        0        0      174 2023-05-16 10:40:20.572842 mkdocstrings_python-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3042 2023-05-16 10:40:23.629451 mkdocstrings_python-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0     3222 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.0/tests/test_handler.py
--rw-r--r--   0        0        0     1975 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.0/tests/test_rendering.py
--rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.0/tests/test_themes.py
--rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 mkdocstrings_python-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-06-02 14:47:59.880294 mkdocstrings_python-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4243 2023-06-02 14:48:02.626927 mkdocstrings_python-1.1.1/README.md
+-rw-r--r--   0        0        0     2604 2023-06-04 14:01:35.369317 mkdocstrings_python-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 14:47:59.736962 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/py.typed
+-rw-r--r--   0        0        0      326 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/__init__.py
+-rw-r--r--   0        0        0    18098 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/handler.py
+-rw-r--r--   0        0        0     7871 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/rendering.py
+-rw-r--r--   0        0        0     2532 2022-04-29 13:33:38.953329 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
+-rw-r--r--   0        0        0     5036 2023-05-25 09:39:58.824275 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/children.html
+-rw-r--r--   0        0        0     4078 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/class.html
+-rw-r--r--   0        0        0     1740 2023-03-03 13:20:57.896481 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
+-rw-r--r--   0        0        0      274 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
+-rw-r--r--   0        0        0     2687 2023-06-04 13:03:08.238478 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
+-rw-r--r--   0        0        0      400 2022-03-01 18:29:05.585970 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
+-rw-r--r--   0        0        0     2697 2023-06-04 13:02:56.049085 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
+-rw-r--r--   0        0        0     3356 2023-06-04 13:02:13.028507 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
+-rw-r--r--   0        0        0     2346 2023-06-04 13:02:01.977392 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
+-rw-r--r--   0        0        0     3333 2023-06-04 13:01:52.305968 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
+-rw-r--r--   0        0        0     3301 2023-06-04 13:01:34.118570 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
+-rw-r--r--   0        0        0     2329 2023-06-04 13:01:20.797497 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
+-rw-r--r--   0        0        0     3273 2023-06-04 13:01:08.835791 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
+-rw-r--r--   0        0        0      674 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
+-rw-r--r--   0        0        0     2436 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/function.html
+-rw-r--r--   0        0        0      245 2022-05-08 08:40:49.298304 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
+-rw-r--r--   0        0        0     1852 2022-04-29 17:36:56.831573 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/module.html
+-rw-r--r--   0        0        0     2698 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/attribute.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/children.html
+-rw-r--r--   0        0        0       33 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/class.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring.html
+-rw-r--r--   0        0        0       48 2022-02-01 20:48:46.512716 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
+-rw-r--r--   0        0        0       46 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
+-rw-r--r--   0        0        0       54 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
+-rw-r--r--   0        0        0       48 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
+-rw-r--r--   0        0        0       44 2021-11-22 18:41:47.281610 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
+-rw-r--r--   0        0        0       46 2021-11-22 18:41:51.551545 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
+-rw-r--r--   0        0        0       45 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
+-rw-r--r--   0        0        0       43 2021-11-22 18:41:56.598136 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
+-rw-r--r--   0        0        0       44 2021-11-03 19:54:24.832142 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
+-rw-r--r--   0        0        0       38 2021-11-08 00:26:56.388000 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/expression.html
+-rw-r--r--   0        0        0       36 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/function.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/labels.html
+-rw-r--r--   0        0        0       34 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/module.html
+-rw-r--r--   0        0        0       37 2021-11-03 19:53:40.146116 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/signature.html
+-rw-r--r--   0        0        0      623 2023-06-03 23:07:22.728595 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/style.css
+-rw-r--r--   0        0        0      928 2023-06-04 13:03:39.709252 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
+-rw-r--r--   0        0        0      934 2023-06-04 13:03:43.052249 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
+-rw-r--r--   0        0        0      928 2023-06-03 22:45:13.311332 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
+-rw-r--r--   0        0        0      868 2023-06-04 13:03:48.958295 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
+-rw-r--r--   0        0        0     1058 2023-06-04 13:03:52.714552 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
+-rw-r--r--   0        0        0     1007 2023-06-04 13:03:57.017402 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
+-rw-r--r--   0        0        0      863 2023-06-04 13:04:01.126928 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
+-rw-r--r--   0        0        0     1040 2023-06-04 13:04:04.606518 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
+-rw-r--r--   0        0        0      971 2023-06-03 23:04:52.858439 mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
+-rw-r--r--   0        0        0      174 2023-06-02 14:47:59.730296 mkdocstrings_python-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3042 2023-06-02 14:48:02.626927 mkdocstrings_python-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     3222 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.1/tests/test_handler.py
+-rw-r--r--   0        0        0     1975 2023-05-11 09:36:36.899109 mkdocstrings_python-1.1.1/tests/test_rendering.py
+-rw-r--r--   0        0        0     1332 2023-05-01 15:54:09.233042 mkdocstrings_python-1.1.1/tests/test_themes.py
+-rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 mkdocstrings_python-1.1.1/PKG-INFO
```

### Comparing `mkdocstrings_python-1.1.0/LICENSE` & `mkdocstrings_python-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/README.md` & `mkdocstrings_python-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/pyproject.toml` & `mkdocstrings_python-1.1.1/pyproject.toml`

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
-version = "1.1.0"
+version = "1.1.1"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://mkdocstrings.github.io/python"
 Documentation = "https://mkdocstrings.github.io/python"
```

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/handler.py` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/rendering.py` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/rendering.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/children.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/children.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/class.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/class.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,100 @@
-{{ log.debug("Rendering attributes section") }}
+{{ log.debug("Rendering receives section") }}
 {% if config.docstring_section_style == "table" %}
   {% block table_style %}
-  <p><strong>{{ section.title or "Attributes:" }}</strong></p>
+  {% set name_column = section.value|selectattr("name")|any %}
+  <p><strong>{{ section.title or "Receives:" }}</strong></p>
   <table>
     <thead>
       <tr>
-        <th>Name</th>
+        {% if name_column %}<th>Name</th>{% endif %}
         <th>Type</th>
         <th>Description</th>
       </tr>
     </thead>
     <tbody>
-      {% for attribute in section.value %}
+      {% for receives in section.value %}
         <tr>
-          <td><code>{{ attribute.name }}</code></td>
+          {% if name_column %}<td>{% if receives.name %}<code>{{ receives.name }}</code>{% endif %}</td>{% endif %}
           <td>
-            {% if attribute.annotation %}
-              {% with expression = attribute.annotation %}
+            {% if receives.annotation %}
+              {% with expression = receives.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
-          <td>{{ attribute.description|convert_markdown(heading_level, html_id) }}</td>
+          <td>
+            <div class="doc-md-description">
+              {{ receives.description|convert_markdown(heading_level, html_id) }}
+            </div>
+          </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
-  <p>{{ section.title or "Attributes:" }}</p>
+  <p>{{ section.title or "Receives:" }}</p>
   <ul>
-    {% for attribute in section.value %}
+    {% for receives in section.value %}
       <li class="field-body">
-        <b>{{ attribute.name }}</b>
-        {% if attribute.annotation %}
-          {% with expression = attribute.annotation %}
-            (<code>{% include "expression.html" with context %}</code>)
+        {% if receives.name %}<b>{{ receives.name }}</b>{% endif %}
+        {% if receives.annotation %}
+          {% with expression = receives.annotation %}
+            {% if receives.name %}({% endif %}
+            <code>{% include "expression.html" with context %}</code>
+            {% if receives.name %}){% endif %}
           {% endwith %}
         {% endif %}
-        – {{ attribute.description|convert_markdown(heading_level, html_id) }}
+        –
+        <div class="doc-md-description">
+          {{ receives.description|convert_markdown(heading_level, html_id) }}
+        </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
     <thead>
       <tr>
-        <th><b>{{ (section.title or "ATTRIBUTE").rstrip(":").upper() }}</b></th>
+        <th><b>{{ (section.title or "RECEIVES").rstrip(":").upper() }}</b></th>
         <th><b>DESCRIPTION</b></th>
       </tr>
     </thead>
     <tbody>
-      {% for attribute in section.value %}
+      {% for receives in section.value %}
         <tr>
-          <td><code>{{ attribute.name }}</code></td>
-          <td class="doc-attribute-details">
-            {{ attribute.description|convert_markdown(heading_level, html_id) }}
-            <p>
-              {% if attribute.annotation %}
-                <span class="doc-attribute-annotation">
+          <td>
+            {% if receives.name %}
+              <code>{{ receives.name }}</code>
+            {% elif receives.annotation %}
+              <span class="doc-receives-annotation">
+                {% with expression = receives.annotation %}
+                  <code>{% include "expression.html" with context %}</code>
+                {% endwith %}
+              </span>
+            {% endif %}
+          </td>
+          <td class="doc-receives-details">
+            <div class="doc-md-description">
+              {{ receives.description|convert_markdown(heading_level, html_id) }}
+            </div>
+            {% if receives.name and receives.annotation %}
+              <p>
+                <span class="doc-receives-annotation">
                   <b>TYPE:</b>
-                  {% with expression = attribute.annotation %}
+                  {% with expression = receives.annotation %}
                     <code>{% include "expression.html" with context %}</code>
                   {% endwith %}
                 </span>
-              {% endif %}
-            </p>
+              </p>
+            {% endif %}
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock spacy_style %}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,35 +1,39 @@
-{{ log.debug("Rendering attributes section") }} {% if
-config.docstring_section_style == "table" %} {% block table_style %}
-{{ section.title or "Attributes:" }}
-Name              Type                 Description
-                  {% if
-                  attribute.annotation
-                  %} {% with
-                  expression =         {
-{{ attribute.name attribute.annotation {
-}}                %} {% include        attribute.description|convert_markdown
-                  "expression.html"    (heading_level, html_id) }}
-                  with context %} {%
-                  endwith %} {% endif
-                  %}
+{{ log.debug("Rendering receives section") }} {% if
+config.docstring_section_style == "table" %} {% block table_style %} {% set
+name_column = section.value|selectattr("name")|any %}
+{{ section.title or "Receives:" }}
+Name                Type                  Description
+                    {% if
+                    receives.annotation
+                    %} {% with expression {
+{% if receives.name = receives.annotation {
+%}{{ receives.name  %} {% include         receives.description|convert_markdown
+}}{% endif %}       "expression.html"     (heading_level, html_id) }}
+                    with context %} {%
+                    endwith %} {% endif
+                    %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
-{{ section.title or "Attributes:" }}
-    * {% for attribute in section.value %}
-    * {{ attribute.name }} {% if attribute.annotation %} {% with expression =
-      attribute.annotation %} ({% include "expression.html" with context %}) {%
-      endwith %} {% endif %} â {{ attribute.description|convert_markdown
-      (heading_level, html_id) }}
+{{ section.title or "Receives:" }}
+    * {% for receives in section.value %}
+    * {% if receives.name %}{{ receives.name }}{% endif %} {% if
+      receives.annotation %} {% with expression = receives.annotation %} {% if
+      receives.name %}({% endif %} {% include "expression.html" with context %}
+      {% if receives.name %}){% endif %} {% endwith %} {% endif %} â
+      {{ receives.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or                DESCRIPTION
-"ATTRIBUTE").rstrip(":").upper() }}
-                                    {
-                                    { attribute.description|convert_markdown
-                                    (heading_level, html_id) }}
-{{ attribute.name }}                {% if attribute.annotation %}  TYPE: {%
-                                    with expression = attribute.annotation
-                                    %} {% include "expression.html" with
-                                    context %} {% endwith %}  {% endif %}
+{{ (section.title or "RECEIVES").rstrip DESCRIPTION
+(":").upper() }}
+                                        {
+                                        { receives.description|convert_markdown
+{% if receives.name %} {{ receives.name (heading_level, html_id) }}
+}} {% elif receives.annotation %}  {%   {% if receives.name and
+with expression = receives.annotation   receives.annotation %}
+%} {% include "expression.html" with     TYPE: {% with expression =
+context %} {% endwith %}  {% endif %}   receives.annotation %} {% include
+                                        "expression.html" with context %} {%
+                                        endwith %}
+                                        {% endif %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,19 @@
           <td>
             {% if parameter.annotation %}
               {% with expression = parameter.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
-          <td>{{ parameter.description|convert_markdown(heading_level, html_id) }}</td>
+          <td>
+            <div class="doc-md-description">
+              {{ parameter.description|convert_markdown(heading_level, html_id) }}
+            </div>
+          </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
@@ -35,15 +39,18 @@
       <li class="field-body">
         <b>{{ parameter.name }}</b>
         {% if parameter.annotation %}
           {% with expression = parameter.annotation %}
             (<code>{% include "expression.html" with context %}</code>)
           {% endwith %}
         {% endif %}
-        – {{ parameter.description|convert_markdown(heading_level, html_id) }}
+        –
+        <div class="doc-md-description">
+          {{ parameter.description|convert_markdown(heading_level, html_id) }}
+        </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
@@ -54,15 +61,17 @@
       </tr>
     </thead>
     <tbody>
       {% for parameter in section.value %}
         <tr>
           <td><code>{{ parameter.name }}</code></td>
           <td class="doc-param-details">
-            {{ parameter.description|convert_markdown(heading_level, html_id) }}
+            <div class="doc-md-description">
+              {{ parameter.description|convert_markdown(heading_level, html_id) }}
+            </div>
             <p>
               {% if parameter.annotation %}
                 <span class="doc-param-annotation">
                   <b>TYPE:</b>
                   {% with expression = parameter.annotation %}
                     <code>{% include "expression.html" with context %}</code>
                   {% endwith %}
```

#### html2text {}

```diff
@@ -14,16 +14,16 @@
                   %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
 {{ section.title or "Other Parameters:" }}
     * {% for parameter in section.value %}
     * {{ parameter.name }} {% if parameter.annotation %} {% with expression =
       parameter.annotation %} ({% include "expression.html" with context %}) {%
-      endwith %} {% endif %} â {{ parameter.description|convert_markdown
-      (heading_level, html_id) }}
+      endwith %} {% endif %} â
+      {{ parameter.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
 {{ (section.title or                DESCRIPTION
 "PARAMETER").rstrip(":").upper() }}
                                     {
                                     { parameter.description|convert_markdown
```

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,19 @@
           <td>
             {% if parameter.annotation %}
               {% with expression = parameter.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
-          <td>{{ parameter.description|convert_markdown(heading_level, html_id) }}</td>
+          <td>
+            <div class="doc-md-description">
+              {{ parameter.description|convert_markdown(heading_level, html_id) }}
+            </div>
+          </td>
           <td>
             {% if parameter.default %}
               {% with expression = parameter.default %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% else %}
               <em>required</em>
@@ -45,15 +49,18 @@
       <li class="field-body">
         <b>{{ parameter.name }}</b>
         {% if parameter.annotation %}
           {% with expression = parameter.annotation %}
             (<code>{% include "expression.html" with context %}</code>)
           {% endwith %}
         {% endif %}
-        – {{ parameter.description|convert_markdown(heading_level, html_id) }}
+        –
+        <div class="doc-md-description">
+          {{ parameter.description|convert_markdown(heading_level, html_id) }}
+        </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
@@ -64,15 +71,17 @@
       </tr>
     </thead>
     <tbody>
       {% for parameter in section.value %}
         <tr>
           <td><code>{{ parameter.name }}</code></td>
           <td class="doc-param-details">
-            {{ parameter.description|convert_markdown(heading_level, html_id) }}
+            <div class="doc-md-description">
+              {{ parameter.description|convert_markdown(heading_level, html_id) }}
+            </div>
             <p>
               {% if parameter.annotation %}
                 <span class="doc-param-annotation">
                   <b>TYPE:</b>
                   {% with expression = parameter.annotation %}
                     <code>{% include "expression.html" with context %}</code>
                   {% endwith %}
```

#### html2text {}

```diff
@@ -15,16 +15,16 @@
                                                                            {% endif %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
 {{ section.title or "Parameters:" }}
     * {% for parameter in section.value %}
     * {{ parameter.name }} {% if parameter.annotation %} {% with expression =
       parameter.annotation %} ({% include "expression.html" with context %}) {%
-      endwith %} {% endif %} â {{ parameter.description|convert_markdown
-      (heading_level, html_id) }}
+      endwith %} {% endif %} â
+      {{ parameter.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
 {{ (section.title or                DESCRIPTION
 "PARAMETER").rstrip(":").upper() }}
                                     {
                                     { parameter.description|convert_markdown
```

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,19 @@
           <td>
             {% if raises.annotation %}
               {% with expression = raises.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
-          <td>{{ raises.description|convert_markdown(heading_level, html_id) }}</td>
+          <td>
+            <div class="doc-md-description">
+              {{ raises.description|convert_markdown(heading_level, html_id) }}
+            </div>
+          </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
@@ -33,15 +37,17 @@
       <li class="field-body">
         {% if raises.annotation %}
           {% with expression = raises.annotation %}
             <code>{% include "expression.html" with context %}</code>
           {% endwith %}
           –
         {% endif %}
-        {{ raises.description|convert_markdown(heading_level, html_id) }}
+        <div class="doc-md-description">
+          {{ raises.description|convert_markdown(heading_level, html_id) }}
+        </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
@@ -58,15 +64,17 @@
             <span class="doc-raises-annotation">
               {% with expression = raises.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             </span>
           </td>
           <td class="doc-raises-details">
-            {{ raises.description|convert_markdown(heading_level, html_id) }}
+            <div class="doc-md-description">
+              {{ raises.description|convert_markdown(heading_level, html_id) }}
+            </div>
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock spacy_style %}
 {% endif %}
```

#### html2text {}

```diff
@@ -7,16 +7,16 @@
 include "expression.html" with context (heading_level, html_id) }}
 %} {% endwith %} {% endif %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
 {{ section.title or "Raises:" }}
     * {% for raises in section.value %}
     * {% if raises.annotation %} {% with expression = raises.annotation %} {%
-      include "expression.html" with context %} {% endwith %} â {% endif %} {
-      { raises.description|convert_markdown(heading_level, html_id) }}
+      include "expression.html" with context %} {% endwith %} â {% endif %}
+      {{ raises.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
 {{ (section.title or "RAISES").rstrip(": DESCRIPTION
 ").upper() }}
  {% with expression = raises.annotation  {{ raises.description|convert_markdown
 %} {% include "expression.html" with     (heading_level, html_id) }}
```

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,95 @@
-{{ log.debug("Rendering receives section") }}
+{{ log.debug("Rendering returns section") }}
 {% if config.docstring_section_style == "table" %}
   {% block table_style %}
   {% set name_column = section.value|selectattr("name")|any %}
-  <p><strong>{{ section.title or "Receives:" }}</strong></p>
+  <p><strong>{{ section.title or "Returns:" }}</strong></p>
   <table>
     <thead>
       <tr>
         {% if name_column %}<th>Name</th>{% endif %}
         <th>Type</th>
         <th>Description</th>
       </tr>
     </thead>
     <tbody>
-      {% for receives in section.value %}
+      {% for returns in section.value %}
         <tr>
-          {% if name_column %}<td>{% if receives.name %}<code>{{ receives.name }}</code>{% endif %}</td>{% endif %}
+          {% if name_column %}<td>{% if returns.name %}<code>{{ returns.name }}</code>{% endif %}</td>{% endif %}
           <td>
-            {% if receives.annotation %}
-              {% with expression = receives.annotation %}
+            {% if returns.annotation %}
+              {% with expression = returns.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
-          <td>{{ receives.description|convert_markdown(heading_level, html_id) }}</td>
+          <td>
+            <div class="doc-md-description">
+              {{ returns.description|convert_markdown(heading_level, html_id) }}
+            </div>
+          </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
-  <p>{{ section.title or "Receives:" }}</p>
+  <p>{{ section.title or "Returns:" }}</p>
   <ul>
-    {% for receives in section.value %}
+    {% for returns in section.value %}
       <li class="field-body">
-        {% if receives.name %}<b>{{ receives.name }}</b>{% endif %}
-        {% if receives.annotation %}
-          {% with expression = receives.annotation %}
-            {% if receives.name %}({% endif %}
+        {% if returns.name %}<b>{{ returns.name }}</b>{% endif %}
+        {% if returns.annotation %}
+          {% with expression = returns.annotation %}
+            {% if returns.name %}({% endif %}
             <code>{% include "expression.html" with context %}</code>
-            {% if receives.name %}){% endif %}
+            {% if returns.name %}){% endif %}
           {% endwith %}
         {% endif %}
-        – {{ receives.description|convert_markdown(heading_level, html_id) }}
+        –
+        <div class="doc-md-description">
+          {{ returns.description|convert_markdown(heading_level, html_id) }}
+      </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
     <thead>
       <tr>
-        <th><b>{{ (section.title or "RECEIVES").rstrip(":").upper() }}</b></th>
+        <th><b>{{ (section.title or "RETURNS").rstrip(":").upper() }}</b></th>
         <th><b>DESCRIPTION</b></th>
       </tr>
     </thead>
     <tbody>
-      {% for receives in section.value %}
+      {% for returns in section.value %}
         <tr>
           <td>
-            {% if receives.name %}
-              <code>{{ receives.name }}</code>
-            {% elif receives.annotation %}
-              <span class="doc-receives-annotation">
-                {% with expression = receives.annotation %}
+            {% if returns.name %}
+              <code>{{ returns.name }}</code>
+            {% elif returns.annotation %}
+              <span class="doc-returns-annotation">
+                {% with expression = returns.annotation %}
                   <code>{% include "expression.html" with context %}</code>
                 {% endwith %}
               </span>
             {% endif %}
           </td>
-          <td class="doc-receives-details">
-            {{ receives.description|convert_markdown(heading_level, html_id) }}
-            {% if receives.name and receives.annotation %}
+          <td class="doc-returns-details">
+            <div class="doc-md-description">
+              {{ returns.description|convert_markdown(heading_level, html_id) }}
+            </div>
+            {% if returns.name and returns.annotation %}
               <p>
-                <span class="doc-receives-annotation">
+                <span class="doc-returns-annotation">
                   <b>TYPE:</b>
-                  {% with expression = receives.annotation %}
+                  {% with expression = returns.annotation %}
                     <code>{% include "expression.html" with context %}</code>
                   {% endwith %}
                 </span>
               </p>
             {% endif %}
           </td>
         </tr>
```

#### html2text {}

```diff
@@ -1,39 +1,38 @@
-{{ log.debug("Rendering receives section") }} {% if
+{{ log.debug("Rendering returns section") }} {% if
 config.docstring_section_style == "table" %} {% block table_style %} {% set
 name_column = section.value|selectattr("name")|any %}
-{{ section.title or "Receives:" }}
-Name                Type                  Description
-                    {% if
-                    receives.annotation
-                    %} {% with expression {
-{% if receives.name = receives.annotation {
-%}{{ receives.name  %} {% include         receives.description|convert_markdown
-}}{% endif %}       "expression.html"     (heading_level, html_id) }}
-                    with context %} {%
-                    endwith %} {% endif
-                    %}
+{{ section.title or "Returns:" }}
+Name                 Type                  Description
+                     {% if
+                     returns.annotation %}
+                     {% with expression =  {
+{% if returns.name   returns.annotation %} {
+%}{{ returns.name }} {% include            returns.description|convert_markdown
+{% endif %}          "expression.html"     (heading_level, html_id) }}
+                     with context %} {%
+                     endwith %} {% endif
+                     %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
-{{ section.title or "Receives:" }}
-    * {% for receives in section.value %}
-    * {% if receives.name %}{{ receives.name }}{% endif %} {% if
-      receives.annotation %} {% with expression = receives.annotation %} {% if
-      receives.name %}({% endif %} {% include "expression.html" with context %}
-      {% if receives.name %}){% endif %} {% endwith %} {% endif %} â {
-      { receives.description|convert_markdown(heading_level, html_id) }}
+{{ section.title or "Returns:" }}
+    * {% for returns in section.value %}
+    * {% if returns.name %}{{ returns.name }}{% endif %} {% if
+      returns.annotation %} {% with expression = returns.annotation %} {% if
+      returns.name %}({% endif %} {% include "expression.html" with context %}
+      {% if returns.name %}){% endif %} {% endwith %} {% endif %} â
+      {{ returns.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or "RECEIVES").rstrip DESCRIPTION
+{{ (section.title or "RETURNS").rstrip  DESCRIPTION
 (":").upper() }}
-                                        {
-                                        { receives.description|convert_markdown
-{% if receives.name %} {{ receives.name (heading_level, html_id) }} {% if
-}} {% elif receives.annotation %}  {%   receives.name and receives.annotation
-with expression = receives.annotation   %}
-%} {% include "expression.html" with     TYPE: {% with expression =
-context %} {% endwith %}  {% endif %}   receives.annotation %} {% include
-                                        "expression.html" with context %} {%
+                                        {{ returns.description|convert_markdown
+                                        (heading_level, html_id) }}
+{% if returns.name %} {{ returns.name   {% if returns.name and
+}} {% elif returns.annotation %}  {%    returns.annotation %}
+with expression = returns.annotation %}  TYPE: {% with expression =
+{% include "expression.html" with       returns.annotation %} {% include
+context %} {% endwith %}  {% endif %}   "expression.html" with context %} {%
                                         endwith %}
                                         {% endif %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,87 @@
-{{ log.debug("Rendering returns section") }}
+{{ log.debug("Rendering attributes section") }}
 {% if config.docstring_section_style == "table" %}
   {% block table_style %}
-  {% set name_column = section.value|selectattr("name")|any %}
-  <p><strong>{{ section.title or "Returns:" }}</strong></p>
+  <p><strong>{{ section.title or "Attributes:" }}</strong></p>
   <table>
     <thead>
       <tr>
-        {% if name_column %}<th>Name</th>{% endif %}
+        <th>Name</th>
         <th>Type</th>
         <th>Description</th>
       </tr>
     </thead>
     <tbody>
-      {% for returns in section.value %}
+      {% for attribute in section.value %}
         <tr>
-          {% if name_column %}<td>{% if returns.name %}<code>{{ returns.name }}</code>{% endif %}</td>{% endif %}
+          <td><code>{{ attribute.name }}</code></td>
           <td>
-            {% if returns.annotation %}
-              {% with expression = returns.annotation %}
+            {% if attribute.annotation %}
+              {% with expression = attribute.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
-          <td>{{ returns.description|convert_markdown(heading_level, html_id) }}</td>
+          <td>
+            <div class="doc-md-description">
+              {{ attribute.description|convert_markdown(heading_level, html_id) }}
+            </div>
+          </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
-  <p>{{ section.title or "Returns:" }}</p>
+  <p>{{ section.title or "Attributes:" }}</p>
   <ul>
-    {% for returns in section.value %}
+    {% for attribute in section.value %}
       <li class="field-body">
-        {% if returns.name %}<b>{{ returns.name }}</b>{% endif %}
-        {% if returns.annotation %}
-          {% with expression = returns.annotation %}
-            {% if returns.name %}({% endif %}
-            <code>{% include "expression.html" with context %}</code>
-            {% if returns.name %}){% endif %}
+        <b>{{ attribute.name }}</b>
+        {% if attribute.annotation %}
+          {% with expression = attribute.annotation %}
+            (<code>{% include "expression.html" with context %}</code>)
           {% endwith %}
         {% endif %}
-        – {{ returns.description|convert_markdown(heading_level, html_id) }}
+        –
+        <div class="doc-md-description">
+          {{ attribute.description|convert_markdown(heading_level, html_id) }}
+        </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
     <thead>
       <tr>
-        <th><b>{{ (section.title or "RETURNS").rstrip(":").upper() }}</b></th>
+        <th><b>{{ (section.title or "ATTRIBUTE").rstrip(":").upper() }}</b></th>
         <th><b>DESCRIPTION</b></th>
       </tr>
     </thead>
     <tbody>
-      {% for returns in section.value %}
+      {% for attribute in section.value %}
         <tr>
-          <td>
-            {% if returns.name %}
-              <code>{{ returns.name }}</code>
-            {% elif returns.annotation %}
-              <span class="doc-returns-annotation">
-                {% with expression = returns.annotation %}
-                  <code>{% include "expression.html" with context %}</code>
-                {% endwith %}
-              </span>
-            {% endif %}
-          </td>
-          <td class="doc-returns-details">
-            {{ returns.description|convert_markdown(heading_level, html_id) }}
-            {% if returns.name and returns.annotation %}
-              <p>
-                <span class="doc-returns-annotation">
+          <td><code>{{ attribute.name }}</code></td>
+          <td class="doc-attribute-details">
+            <div class="doc-md-description">
+              {{ attribute.description|convert_markdown(heading_level, html_id) }}
+            </div>
+            <p>
+              {% if attribute.annotation %}
+                <span class="doc-attribute-annotation">
                   <b>TYPE:</b>
-                  {% with expression = returns.annotation %}
+                  {% with expression = attribute.annotation %}
                     <code>{% include "expression.html" with context %}</code>
                   {% endwith %}
                 </span>
-              </p>
-            {% endif %}
+              {% endif %}
+            </p>
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock spacy_style %}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,37 +1,35 @@
-{{ log.debug("Rendering returns section") }} {% if
-config.docstring_section_style == "table" %} {% block table_style %} {% set
-name_column = section.value|selectattr("name")|any %}
-{{ section.title or "Returns:" }}
-Name                 Type                  Description
-                     {% if
-                     returns.annotation %}
-                     {% with expression =  {
-{% if returns.name   returns.annotation %} {
-%}{{ returns.name }} {% include            returns.description|convert_markdown
-{% endif %}          "expression.html"     (heading_level, html_id) }}
-                     with context %} {%
-                     endwith %} {% endif
-                     %}
+{{ log.debug("Rendering attributes section") }} {% if
+config.docstring_section_style == "table" %} {% block table_style %}
+{{ section.title or "Attributes:" }}
+Name              Type                 Description
+                  {% if
+                  attribute.annotation
+                  %} {% with
+                  expression =         {
+{{ attribute.name attribute.annotation {
+}}                %} {% include        attribute.description|convert_markdown
+                  "expression.html"    (heading_level, html_id) }}
+                  with context %} {%
+                  endwith %} {% endif
+                  %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
-{{ section.title or "Returns:" }}
-    * {% for returns in section.value %}
-    * {% if returns.name %}{{ returns.name }}{% endif %} {% if
-      returns.annotation %} {% with expression = returns.annotation %} {% if
-      returns.name %}({% endif %} {% include "expression.html" with context %}
-      {% if returns.name %}){% endif %} {% endwith %} {% endif %} â {
-      { returns.description|convert_markdown(heading_level, html_id) }}
+{{ section.title or "Attributes:" }}
+    * {% for attribute in section.value %}
+    * {{ attribute.name }} {% if attribute.annotation %} {% with expression =
+      attribute.annotation %} ({% include "expression.html" with context %}) {%
+      endwith %} {% endif %} â
+      {{ attribute.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or "RETURNS").rstrip  DESCRIPTION
-(":").upper() }}
-                                        {{ returns.description|convert_markdown
-{% if returns.name %} {{ returns.name   (heading_level, html_id) }} {% if
-}} {% elif returns.annotation %}  {%    returns.name and returns.annotation %}
-with expression = returns.annotation %}  TYPE: {% with expression =
-{% include "expression.html" with       returns.annotation %} {% include
-context %} {% endwith %}  {% endif %}   "expression.html" with context %} {%
-                                        endwith %}
-                                        {% endif %}
+{{ (section.title or                DESCRIPTION
+"ATTRIBUTE").rstrip(":").upper() }}
+                                    {
+                                    { attribute.description|convert_markdown
+                                    (heading_level, html_id) }}
+{{ attribute.name }}                {% if attribute.annotation %}  TYPE: {%
+                                    with expression = attribute.annotation
+                                    %} {% include "expression.html" with
+                                    context %} {% endwith %}  {% endif %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,19 @@
           <td>
             {% if warns.annotation %}
               {% with expression = warns.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
-          <td>{{ warns.description|convert_markdown(heading_level, html_id) }}</td>
+          <td>
+            <div class="doc-md-description">
+              {{ warns.description|convert_markdown(heading_level, html_id) }}
+            </div>
+          </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
@@ -33,15 +37,17 @@
       <li class="field-body">
         {% if warns.annotation %}
           {% with expression = warns.annotation %}
             <code>{% include "expression.html" with context %}</code>
           {% endwith %}
           –
         {% endif %}
-        {{ warns.description|convert_markdown(heading_level, html_id) }}
+        <div class="doc-md-description">
+          {{ warns.description|convert_markdown(heading_level, html_id) }}
+        </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
@@ -58,15 +64,17 @@
             <span class="doc-warns-annotation">
               {% with expression = warns.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             </span>
           </td>
           <td class="doc-warns-details">
-            {{ warns.description|convert_markdown(heading_level, html_id) }}
+            <div class="doc-md-description">
+              {{ warns.description|convert_markdown(heading_level, html_id) }}
+            </div>
           </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock spacy_style %}
 {% endif %}
```

#### html2text {}

```diff
@@ -7,16 +7,16 @@
 include "expression.html" with context %} (heading_level, html_id) }}
 {% endwith %} {% endif %}
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
 {{ section.title or "Warns:" }}
     * {% for warns in section.value %}
     * {% if warns.annotation %} {% with expression = warns.annotation %} {%
-      include "expression.html" with context %} {% endwith %} â {% endif %} {
-      { warns.description|convert_markdown(heading_level, html_id) }}
+      include "expression.html" with context %} {% endwith %} â {% endif %}
+      {{ warns.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
 {{ (section.title or "WARNS").rstrip(":   DESCRIPTION
 ").upper() }}
  {% with expression = warns.annotation %} {{ warns.description|convert_markdown
 {% include "expression.html" with context (heading_level, html_id) }}
```

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,19 @@
           <td>
             {% if yields.annotation %}
               {% with expression = yields.annotation %}
                 <code>{% include "expression.html" with context %}</code>
               {% endwith %}
             {% endif %}
           </td>
-          <td>{{ yields.description|convert_markdown(heading_level, html_id) }}</td>
+          <td>
+            <div class="doc-md-description">
+              {{ yields.description|convert_markdown(heading_level, html_id) }}
+            </div>
+          </td>
         </tr>
       {% endfor %}
     </tbody>
   </table>
   {% endblock table_style %}
 {% elif config.docstring_section_style == "list" %}
   {% block list_style %}
@@ -38,15 +42,18 @@
         {% if yields.annotation %}
           {% with expression = yields.annotation %}
             {% if yields.name %}({% endif %}
             <code>{% include "expression.html" with context %}</code>
             {% if yields.name %}){% endif %}
           {% endwith %}
         {% endif %}
-        – {{ yields.description|convert_markdown(heading_level, html_id) }}
+        –
+        <div class="doc-md-description">
+          {{ yields.description|convert_markdown(heading_level, html_id) }}
+        </div>
       </li>
     {% endfor %}
   </ul>
   {% endblock list_style %}
 {% elif config.docstring_section_style == "spacy" %}
   {% block spacy_style %}
   <table>
@@ -67,15 +74,17 @@
                 {% with expression = yields.annotation %}
                   <code>{% include "expression.html" with context %}</code>
                 {% endwith %}
               </span>
             {% endif %}
           </td>
           <td class="doc-yields-details">
-            {{ yields.description|convert_markdown(heading_level, html_id) }}
+            <div class="doc-md-description">
+              {{ yields.description|convert_markdown(heading_level, html_id) }}
+            </div>
             {% if yields.name and yields.annotation %}
               <p>
                 <span class="doc-yields-annotation">
                   <b>TYPE:</b>
                   {% with expression = yields.annotation %}
                     <code>{% include "expression.html" with context %}</code>
                   {% endwith %}
```

#### html2text {}

```diff
@@ -15,23 +15,24 @@
 {% endblock table_style %} {% elif config.docstring_section_style == "list" %}
 {% block list_style %}
 {{ section.title or "Yields:" }}
     * {% for yields in section.value %}
     * {% if yields.name %}{{ yields.name }}{% endif %} {% if yields.annotation
       %} {% with expression = yields.annotation %} {% if yields.name %}({%
       endif %} {% include "expression.html" with context %} {% if yields.name
-      %}){% endif %} {% endwith %} {% endif %} â {
-      { yields.description|convert_markdown(heading_level, html_id) }}
+      %}){% endif %} {% endwith %} {% endif %} â
+      {{ yields.description|convert_markdown(heading_level, html_id) }}
     * {% endfor %}
 {% endblock list_style %} {% elif config.docstring_section_style == "spacy" %}
 {% block spacy_style %}
-{{ (section.title or "YIELDS").rstrip(": DESCRIPTION
-").upper() }}
-                                         {{ yields.description|convert_markdown
-{% if yields.name %} {{ yields.name }}   (heading_level, html_id) }} {% if
-{% elif yields.annotation %}  {% with    yields.name and yields.annotation %}
-expression = yields.annotation %} {%      TYPE: {% with expression =
-include "expression.html" with context   yields.annotation %} {% include
-%} {% endwith %}  {% endif %}            "expression.html" with context %} {%
-                                         endwith %}
-                                         {% endif %}
+{{ (section.title or "YIELDS").rstrip   DESCRIPTION
+(":").upper() }}
+                                        {{ yields.description|convert_markdown
+                                        (heading_level, html_id) }}
+{% if yields.name %} {{ yields.name }}  {% if yields.name and yields.annotation
+{% elif yields.annotation %}  {% with   %}
+expression = yields.annotation %} {%     TYPE: {% with expression =
+include "expression.html" with context  yields.annotation %} {% include
+%} {% endwith %}  {% endif %}           "expression.html" with context %} {%
+                                        endwith %}
+                                        {% endif %}
 {% endblock spacy_style %} {% endif %}
```

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/expression.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/expression.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/function.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/function.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/module.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/module.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/_base/signature.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/_base/signature.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/material/style.css` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/material/style.css`

 * *Files 22% similar despite different names*

```diff
@@ -4,32 +4,28 @@
 }
 
 /* Avoid breaking parameters name, etc. in table cells. */
 .doc-contents td code {
   word-break: normal !important;
 }
 
-/* For pieces of Markdown rendered in table cells. */
-.doc-contents td p {
-  margin-top: 0 !important;
-  margin-bottom: 0 !important;
+/* No line break before first paragraph of descriptions. */
+.doc-md-description,
+.doc-md-description>p:first-child {
+  display: inline;
 }
 
 /* Max width for docstring sections tables. */
 .doc .md-typeset__table,
 .doc .md-typeset__table table {
   display: table !important;
   width: 100%;
 }
+
 .doc .md-typeset__table tr {
   display: table-row;
 }
 
-/* Avoid line breaks in rendered fields. */
-.field-body p {
-  display: inline;
-}
-
 /* Defaults in Spacy table style. */
 .doc-param-default {
   float: right;
-}
+}
```

### Comparing `mkdocstrings_python-1.1.0/src/mkdocstrings_handlers/python/templates/readthedocs/other_parameters.html` & `mkdocstrings_python-1.1.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html`

 * *Files 27% similar despite different names*

```diff
@@ -2,18 +2,29 @@
 <table class="field-list">
   <colgroup>
     <col class="field-name" />
     <col class="field-body" />
   </colgroup>
   <tbody valign="top">
     <tr class="field">
-      <th class="field-name">Keyword arguments:</th>
+      <th class="field-name">{{ section.title or "Attributes:" }}</th>
       <td class="field-body">
         <ul class="first simple">
-          {% for kwarg in kwargs %}
-            <li>{{ ("**" + kwarg.name + "**" + (" (`" + kwarg.annotation + "`)" if kwarg.annotation else "") + " – " + kwarg.description)|convert_markdown(heading_level, html_id) }}</li>
+          {% for attribute in section.value %}
+            <li>
+              <b>{{ attribute.name }}</b>
+              {% if attribute.annotation %}
+                {% with expression = attribute.annotation %}
+                  (<code>{% include "expression.html" with context %}</code>)
+                {% endwith %}
+              {% endif %}
+              –
+              <div class="doc-md-description">
+                {{ attribute.description|convert_markdown(heading_level, html_id) }}
+              </div>
+            </li>
           {% endfor %}
         </ul>
       </td>
     </tr>
   </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 {{ log.debug() }}
-                       * {% for kwarg in kwargs %}
-                       * {{ ("**" + kwarg.name + "**" + (" (`" +
-Keyword arguments:       kwarg.annotation + "`)" if kwarg.annotation else "") +
-                         " â " + kwarg.description)|convert_markdown
-                         (heading_level, html_id) }}
-                       * {% endfor %}
+{                 * {% for attribute in section.value %}
+{                 * {{ attribute.name }} {% if attribute.annotation %} {% with
+section.title       expression = attribute.annotation %} ({% include "expression.html"
+or                  with context %}) {% endwith %} {% endif %} â
+"Attributes:        {{ attribute.description|convert_markdown(heading_level, html_id)
+" }}                }}
+                  * {% endfor %}
```

### Comparing `mkdocstrings_python-1.1.0/tests/conftest.py` & `mkdocstrings_python-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/tests/test_handler.py` & `mkdocstrings_python-1.1.1/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/tests/test_rendering.py` & `mkdocstrings_python-1.1.1/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/tests/test_themes.py` & `mkdocstrings_python-1.1.1/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.1.0/PKG-INFO` & `mkdocstrings_python-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocstrings-python
-Version: 1.1.0
+Version: 1.1.1
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
-Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.1.0 Summary: A
+Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.1.1 Summary: A
 Python handler for mkdocstrings. Author-Email: TimothÃ©e Mazzucotelli
 pm.me> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

