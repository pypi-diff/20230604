# Comparing `tmp/django-hostutils-0.0.5.tar.gz` & `tmp/django-hostutils-0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hostutils-0.0.5.tar", last modified: Sat Jun  3 22:18:42 2023, max compression
+gzip compressed data, was "django-hostutils-0.0.dev3.tar", last modified: Tue Apr 25 00:40:22 2023, max compression
```

## Comparing `django-hostutils-0.0.5.tar` & `django-hostutils-0.0.dev3.tar`

### file list

```diff
@@ -1,47 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.551202 django-hostutils-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44965 2023-06-03 22:18:42.551202 django-hostutils-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 22:18:42.551202 django-hostutils-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.547202 django-hostutils-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 22:18:42.000000 django-hostutils-0.0.5/src/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.547202 django-hostutils-0.0.5/src/django_hostutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44965 2023-06-03 22:18:42.000000 django-hostutils-0.0.5/src/django_hostutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-03 22:18:42.000000 django-hostutils-0.0.5/src/django_hostutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:18:42.000000 django-hostutils-0.0.5/src/django_hostutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-03 22:18:42.000000 django-hostutils-0.0.5/src/django_hostutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 22:18:42.000000 django-hostutils-0.0.5/src/django_hostutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.547202 django-hostutils-0.0.5/src/djangoaddicts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.547202 django-hostutils-0.0.5/src/djangoaddicts/hostutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.543202 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.543202 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.547202 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.547202 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.547202 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_cpu_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_interface_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_partition_stats.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_process_stats.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.551202 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card_swap.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_results_timestamp.htm
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:18:42.551202 django-hostutils-0.0.5/src/djangoaddicts/hostutils/views/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/views/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-06-03 22:18:27.000000 django-hostutils-0.0.5/src/djangoaddicts/hostutils/views/htmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/django_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   133744 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/cpu.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/cpu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/disk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/host.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/memory.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/_static/process.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   131317 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/cpu.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   124420 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/disk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   161082 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/host.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   100187 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/memory.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   154714 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   122738 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/images/process.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/docs/source/version_history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:40:22.000000 django-hostutils-0.0.dev3/src/django_hostutils.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_partition_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.509207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card_swap.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_results_timestamp.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/htmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.505207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_cpu_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_interface_stats.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_partition_usage.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_process_details.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/core/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:22.513207 django-hostutils-0.0.dev3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-25 00:40:08.000000 django-hostutils-0.0.dev3/tests/unit/test_htmx.py
```

### Comparing `django-hostutils-0.0.5/LICENSE` & `django-hostutils-0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.5/README.md` & `django-hostutils-0.0.dev3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: django-hostutils
+Version: 0.0.dev3
+Summary: host utilities for django projects
+Home-page: https://github.com/davidslusser/django-hostutils
+Author: David Slusser
+Author-email: dbslusser@gmail.com
+License: GNU GENERAL PUBLIC LICENSE
+Platform: any
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # django-hostutils
 Host utilities package for django projects. Bootstrap 5 templates are provided.  Host metric data includes:
 - Host OS, release, uptime
 - CPU count and utilization
 - Memory usage
 - Disk partations and utilization
 - Processes running, idle, sleeping
@@ -14,46 +27,27 @@
 |--------------|------|
 | Author       | David Slusser |
 | Description  | Host utilities package for django projects. |
 | Requirements | `Python 3.x` +<br>`Django 3.2.x` + |
 
 <br/>
 
-## Code Quality
-| Workflow | Description             | Status                                                                       |
-|----------|-------------------------|------------------------------------------------------------------------------|
-|Bandit|security checks|![Bandit](https://github.com/djangoaddicts/django-hostutils/actions/workflows/bandit.yaml/badge.svg)|
-|Black|code formatting|![Black](https://github.com/djangoaddicts/django-hostutils/actions/workflows/black.yaml/badge.svg)|
-|Coveralls|code coverage status|[![Coverage Status](https://coveralls.io/repos/github/djangoaddicts/django-hostutils/badge.svg?branch=coveralls)](https://coveralls.io/github/djangoaddicts/django-hostutils?branch=coveralls)|
-|Mypy|static type checking|![Mypy](https://github.com/djangoaddicts/django-hostutils/actions/workflows/mypy.yaml/badge.svg)|
-|Ruff|static code analysis|![Ruff](https://github.com/djangoaddicts/django-hostutils/actions/workflows/ruff.yaml/badge.svg)|
-|Pytest|unit testing|![Pytest](https://github.com/djangoaddicts/django-hostutils/actions/workflows/pytest.yaml/badge.svg)|
-
-<br/>
-
-### Code Coverage Dashboard:
-https://coveralls.io/github/djangoaddicts/django-hostutils
-
-<br/>
-
-## Documentation
+## Code Quality Checks
 | Workflow | Description             | Status                                                                       |
 |----------|-------------------------|------------------------------------------------------------------------------|
-|Docs|ReadTheDocs Build|[![Documentation Status](https://readthedocs.org/projects/django-hostutils/badge/?version=latest)](https://django-hostutils.readthedocs.io/en/latest/?badge=latest)|
-
-Full documentation is available here:
-
-https://django-hostutils.readthedocs.io/en/latest/index.html 
+|Bandit|security checks|![Bandit](https://github.com/davidslusser/workflow_tests/actions/workflows/bandit.yaml/badge.svg)|
+|Black|code formatting|![Black](https://github.com/davidslusser/workflow_tests/actions/workflows/black.yaml/badge.svg)|
+|Mypy|static type checking|![Mypy](https://github.com/davidslusser/workflow_tests/actions/workflows/mypy.yaml/badge.svg)|
+|Pylint|static code analysis|![Pylint](https://github.com/davidslusser/workflow_tests/actions/workflows/pylint.yaml/badge.svg)|
+|Pytest|unit testing|![Pytest](https://github.com/davidslusser/workflow_tests/actions/workflows/pytest.yaml/badge.svg)|
 
 <br/>
 
 ## License
-django-hostutils is licensed under the GNU-3 license (see the LICENSE file for details).
-
-https://github.com/davidslusser/django-hostutils/blob/docs/LICENSE 
+django-userextensions is licensed under the GNU-3 license (see the LICENSE file for details).
 
 <br/>
 
 ## Installation 
 - pip install django-hostutils
 - add the following to your INSTALLED_APPS
 
@@ -62,68 +56,51 @@
     ```
 - add the following to your project-level urls.py:
    
    ```python
    path("hostutils/", include("djangoaddicts.hostutils.urls"), ),
    ```
 
-<br/>
-
 ## Usage
-
-### Included Views
 Several pages are available. If you have a Bootstrap 5 nav-menu you can add the following snippet in your navbar where appropriate:
 
-```python
-{% include 'hostutils/bs5/snippets/hostutils_nav_menu.htm' %}
-```
+    ```
+    {% include 'hostutils/bs5/snippets/hostutils_nav_menu.htm' %}
+    ```
 
-Individual pages can also be linked directly:
+Alternatively, individual pages can linked directly:
 
 - Host overview page: 
 
-    ```python
+    ```
     {% url 'hostutils:host_details' %}
     ```
 
 - CPU stats page: 
 
-    ```python
+    ```
     {% url 'hostutils:host_cpu' %}
     ```
 
 - Disk stats page: 
 
-    ```python
+    ```
     {% url 'hostutils:host_disk' %}
     ```
 
 - Memory stats page: 
 
-    ```python
+    ```
     {% url 'hostutils:host_memory' %}
     ```
 
 - Network stats page: 
 
-    ```python
+    ```
     {% url 'hostutils:host_network' %}
     ```
 
 - Process stats page: 
 
-    ```python
-    {% url 'hostutils:host_process' %}
     ```
-
-### Custom Views
-Custom views/templates can be used to override the Bootstrap 5 templates provided by default for GUI views. In your views, import the desired views(s) from hostutils and create a class that inherits the desired hostutils view.
-
-Here is an example of creating a custom view using ShowHost:
-
-    ```python
-    from djangoaddicts.hostutils.views import ShowHost
-
-    class MyCustomShowHostView(ShowHost):
-        template_name = "my_custom_template.html"
-        title = "My Custom Title"
+    {% url 'hostutils:host_process' %}
     ```
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/forms.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/forms.py`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/cpu.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 {% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %}
 {% load static %}
 {% load handyhelper_tags %}
 
 {% block local_head %}
+    {% include 'handyhelpers/component/chartjs_components.htm' %}
     <style>
         .card .card-header {
             color: var(--primary);
             font-weight: bold;
             font-size: 1.25rem;
         }
         .key {
@@ -153,15 +154,15 @@
     <div class="container-fluid mt-5">
         <div class="card shadow">
             <div class="card-header">CPUs <span class="small">({{ logical_count }})</span></div>
                 <div class="card-body" style="overflow-y: auto; overflow-x: hidden; max-height: 50vh">
                     <ul class="list-group mx-auto justify-content-center" style="max-width: 93%; margin-top: .5%; margin-bottom: .5%">
                         {% for cpu, data in cpu_data.items %}
                         <li class="list-group-item bg-light shadow-sm hvr-grow mb-3">
-                            <a href="#" hx-get="{% url 'hostutils:get_cpu_stats' cpu %}" hx-target="#modal_wrapper">
+                            <a href="#" onClick="showInfo('{% url "hostutils:get_cpu_stats" %}', '{{cpu}}', 'CPU Stats: <small><i>{{cpu}}</i></small>', true);">
                                 <div class="row">
                                     <div class="col-xs-12 col-md-2"><span class="key">CPU:</span><span class="value">{{ cpu }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Percent:</span><span class="value">{{ data.percent }}%</span></div>
                                     <div class="col-xs-12 col-md-3"><span class="key">System:</span><span class="value">{{ data.time_percent.system }}%</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Idle:</span><span class="value">{{ data.time_percent.idle }}%</span></div>
                                     <div class="col-xs-12 col-md-3"><span class="key">Frequency:</span><span class="value">{{ data.frequency.current }}</span></div>
                                 </div>
@@ -171,9 +172,9 @@
                     </ul>
                 </div>
             </div>
         </div>
     </div>
 </section>
 
-{% include 'handyhelpers/htmx/bs5/generic_modal.htm' %}
+{% include 'handyhelpers/component/bs5/modals.htm' %}
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends BASE_TEMPLATE|default:"handyhelpers/handyhelpers_base_bs5.htm" %} {%
-load static %} {% load handyhelper_tags %} {% block local_head %}
+load static %} {% load handyhelper_tags %} {% block local_head %} {% include
+'handyhelpers/component/chartjs_components.htm' %}
  {% endblock %} {% block content %}  {% if title or subtitle %}
 {{ title }}
 {{ subtitle|safe }}
 {% endif %}
 {{ physical_count }}
 Physical
 {{ logical_count }}
@@ -21,14 +22,15 @@
 {{ load_avg_5 }}%
 5 minute load average
 {{ load_avg_15 }}%
 15 minute load average
 
 CPUs ({{ logical_count }})
     * {% for cpu, data in cpu_data.items %}
-    * CPU:{{_cpu_}}
-      Percent:{{_data.percent_}}%
-      System:{{_data.time_percent.system_}}%
-      Idle:{{_data.time_percent.idle_}}%
-      Frequency:{{_data.frequency.current_}}
-    * {% endfor %}
- {% include 'handyhelpers/htmx/bs5/generic_modal.htm' %} {% endblock content %}
+    *  %}', '{{cpu}}', 'CPU Stats: {{cpu}}', true);">
+      CPU:{{ cpu }}
+      Percent:{{ data.percent }}%
+      System:{{ data.time_percent.system }}%
+      Idle:{{ data.time_percent.idle }}%
+      Frequency:{{ data.frequency.current }}
+{% endfor %}
+ {% include 'handyhelpers/component/bs5/modals.htm' %} {% endblock content %}
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/detail_host.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/disk.html`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
             justify-content: center;
         }
         .titlecard-container > * {
             flex: 1;
         }
         .titlecard {
             height: 6rem;
+<!--            min-width: 148px;-->
+<!--            max-width: 475;-->
         }
         .titlecard .icon {
             color: var(--primary);
             font-size: 2.5rem;
             text-align: left;
             margin-top: -.5rem;
         }
@@ -131,15 +133,15 @@
     <div class="container-fluid mt-5">
         <div class="card shadow">
             <div class="card-header">Partitions <span class="small">({{ partition_lists|length }})</span></div>
                 <div class="card-body" style="overflow-y: auto; overflow-x: hidden; max-height: 50vh">
                     <ul class="list-group mx-auto justify-content-center" style="max-width: 93%; margin-top: .5%; margin-bottom: .5%">
                         {% for item in partition_lists %}
                         <li class="list-group-item bg-light shadow-sm hvr-grow mb-3">
-                            <a href="#" hx-get="{% url 'hostutils:get_partition_stats' %}?part={{ item.mountpoint }}" hx-target="#modal_wrapper">
+                            <a href="#" onClick="showInfo('{% url "hostutils:get_partition_stats" %}', '{{item.mountpoint}}', 'Partition Disk Usage: <small><i>{{item.mountpoint}}</i></small>', true);">
                                 <div class="row mb-1">
                                     <div class="col-xs-12 col-md-3"><span class="key">Device:</span><span class="value">{{ item.device }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Filesystem:</span><span class="value">{{ item.fstype }}</span></div>
                                     <div class="col-xs-12 col-md-3"><span class="key">Mount Point:</span><span class="value">{{ item.mountpoint }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Max File:</span><span class="value">{{ item.maxfile }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Max Path:</span><span class="value">{{ item.maxpath }}</span></div>
                                 </div>
@@ -221,9 +223,9 @@
               }
           }
         }
     }
 });
 </script>
 
-{% include 'handyhelpers/htmx/bs5/generic_modal.htm' %}
+{% include 'handyhelpers/component/bs5/modals.htm' %}
 {% endblock content %}
```

#### html2text {}

```diff
@@ -12,15 +12,17 @@
 {{ io_counters.read_bytes|byte_size }}
 Read Bytes
 {{ io_counters.write_bytes|byte_size }}
 Write Bytes
 
 Partitions ({{ partition_lists|length }})
     * {% for item in partition_lists %}
-    * Device:{{_item.device_}}
-      Filesystem:{{_item.fstype_}}
-      Mount_Point:{{_item.mountpoint_}}
-      Max_File:{{_item.maxfile_}}
-      Max_Path:{{_item.maxpath_}}
-      Options:{{_item.opts_}}
-    * {% endfor %}
- {% include 'handyhelpers/htmx/bs5/generic_modal.htm' %} {% endblock content %}
+    *  %}', '{{item.mountpoint}}', 'Partition Disk Usage: {{item.mountpoint}}',
+      true);">
+      Device:{{ item.device }}
+      Filesystem:{{ item.fstype }}
+      Mount Point:{{ item.mountpoint }}
+      Max File:{{ item.maxfile }}
+      Max Path:{{ item.maxpath }}
+      Options:{{ item.opts }}
+{% endfor %}
+ {% include 'handyhelpers/component/bs5/modals.htm' %} {% endblock content %}
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/memory.html`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/network.html`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     <div class="container-fluid mt-5">
         <div class="card shadow">
             <div class="card-header">Network Interfaces <span class="small">({{ interface_list|length }})</span></div>
                 <div class="card-body" style="overflow-y: auto; overflow-x: hidden; height: 200px">
                     <ul class="list-group mx-auto justify-content-center" style="max-width: 93%; margin-top: .5%; margin-bottom: .5%">
                         {% for k,v in interface_list.items %}
                         <li class="list-group-item bg-light shadow-sm hvr-grow mb-3">
-                            <a href="#" hx-get="{% url 'hostutils:get_interface_stats' k %}" hx-target="#modal_wrapper">
+                            <a href="#" onClick="showInfo('{% url "hostutils:get_interface_stats" %}', '{{k}}', 'Network Stats: <small><i>{{k}}</i></small>', false);">
                                 <div class="row">
                                     <div class="key h5">{{ k }}:</div>
                                     {% for item in v %}
                                     <div class="col-xs-12 col-md-3"><span class="key">address:</span><span class="value">{{ item.address }}</span></div>
                                     <div class="col-xs-12 col-md-3"><span class="key">netmask:</span><span class="value">{{ item.netmask }}</span></div>
                                     <div class="col-xs-12 col-md-3"><span class="key">broadcast:</span><span class="value">{{ item.broadcast }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">family:</span><span class="value">{{ item.family.name }}</span></div>
@@ -185,9 +185,9 @@
                     </ul>
                 </div>
             </div>
         </div>
     </div>
 </section>
 
-{% include 'handyhelpers/htmx/bs5/generic_modal.htm' %}
+{% include 'handyhelpers/component/bs5/modals.htm' %}
 {% endblock content %}
```

#### html2text {}

```diff
@@ -19,30 +19,31 @@
 {{ counters.dropin }}
 Drops In
 {{ counters.dropout }}
 Drops Out
 
 Network Interfaces ({{ interface_list|length }})
     * {% for k,v in interface_list.items %}
-    * {{_k_}}:
-      {%_for_item_in_v_%}
-      address:{{_item.address_}}
-      netmask:{{_item.netmask_}}
-      broadcast:{{_item.broadcast_}}
-      family:{{_item.family.name_}}
-      ptp:{{_item.ptp_}}
-      {%_endfor_%}
-    * {% endfor %}
+    *  %}', '{{k}}', 'Network Stats: {{k}}', false);">
+      {{ k }}:
+      {% for item in v %}
+      address:{{ item.address }}
+      netmask:{{ item.netmask }}
+      broadcast:{{ item.broadcast }}
+      family:{{ item.family.name }}
+      ptp:{{ item.ptp }}
+      {% endfor %}
+{% endfor %}
 
 Network Connections ({{ connection_list|length }})
     * {% for connection in connection_list %}
     * laddr:{{ connection.laddr.ip }}
       lport:{{ connection.laddr.port }}
       family:{{ connection.family.name }}
       fd:{{ connection.fd }}
       status:{{ connection.status }}
       raddr:{{ connection.raddr.ip }}
       rport:{{ connection.raddr.port }}
       type:{{ connection.type }}
       pid:{{ connection.pid }}
       {% endfor %}
- {% include 'handyhelpers/htmx/bs5/generic_modal.htm' %} {% endblock content %}
+ {% include 'handyhelpers/component/bs5/modals.htm' %} {% endblock content %}
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/detail/processes.html`

 * *Files 1% similar despite different names*

```diff
@@ -131,13 +131,13 @@
 
 <section class="mb-5 animated fadeIn" style="animation-delay: .35s;">
     <div class="container-fluid mt-5" id="id_process_list_container">
         {% include 'hostutils/bs5/snippets/host_process_card.htm' %}
     </div>
 </section>
 
-{% include 'handyhelpers/htmx/bs5/generic_modal.htm' %}
+{% include 'handyhelpers/component/bs5/modals.htm' %}
 {% with filter_form as form_data %}
     {% include 'handyhelpers/generic/bs5/generic_modal_form_htmx.htm' %}
 {% endwith %}
 
 {% endblock content %}
```

#### html2text {}

```diff
@@ -16,10 +16,10 @@
 {{ counts.zombie }}
 Zombie
 {{ counts.dead }}
 Dead
 
 
 {% include 'hostutils/bs5/snippets/host_process_card.htm' %}
- {% include 'handyhelpers/htmx/bs5/generic_modal.htm' %} {% with filter_form as
+ {% include 'handyhelpers/component/bs5/modals.htm' %} {% with filter_form as
 form_data %} {% include 'handyhelpers/generic/bs5/generic_modal_form_htmx.htm'
 %} {% endwith %} {% endblock content %}
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_cpu_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_cpu_stats.htm`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,81 @@
+{% if data %}
 <div class="container-fluid">
     <br/>
     <div class="row">
         <div class="col-7">
             <div class="h3 font-weight-bold text-primary">CPU Times</div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">System: </div>
-                <div class="col-2 text-secondary">{{ time_percent.system }}%</div>
-                <div class="col-6 text-secondary">{{ time.system }}</div>
+                <div class="col-3 text-primary font-weight-bold">System: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.system }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.system }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Idle: </div>
-                <div class="col-2 text-secondary">{{ time_percent.idle }}%</div>
-                <div class="col-6 text-secondary">{{ time.idle }}</div>
+                <div class="col-3 text-primary font-weight-bold">Idle: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.idle }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.idle }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">User: </div>
-                <div class="col-2 text-secondary">{{ time_percent.user }}%</div>
-                <div class="col-6 text-secondary">{{ time.user }}</div>
+                <div class="col-3 text-primary font-weight-bold">User: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.user }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.user }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Nice: </div>
-                <div class="col-2 text-secondary">{{ time_percent.nice }}%</div>
-                <div class="col-6 text-secondary">{{ time.nice }}</div>
+                <div class="col-3 text-primary font-weight-bold">Nice: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.nice }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.nice }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">IO Wait: </div>
-                <div class="col-2 text-secondary">{{ time_percent.iowait }}%</div>
-                <div class="col-6 text-secondary">{{ time.iowait }}</div>
+                <div class="col-3 text-primary font-weight-bold">IO Wait: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.iowait }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.iowait }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">IRQ: </div>
-                <div class="col-2 text-secondary">{{ time_percent.irq }}%</div>
-                <div class="col-6 text-secondary">{{ time.irq }}</div>
+                <div class="col-3 text-primary font-weight-bold">IRQ: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.irq }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.irq }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Soft IRQ: </div>
-                <div class="col-2 text-secondary">{{ time_percent.softirq }}%</div>
-                <div class="col-6 text-secondary">{{ time.system }}</div>
+                <div class="col-3 text-primary font-weight-bold">Soft IRQ: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.softirq }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.system }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Steal: </div>
-                <div class="col-2 text-secondary">{{ time_percent.steal }}%</div>
-                <div class="col-6 text-secondary">{{ time.steal }}</div>
+                <div class="col-3 text-primary font-weight-bold">Steal: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.steal }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.steal }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Guest: </div>
-                <div class="col-2 text-secondary">{{ time_percent.guest }}%</div>
-                <div class="col-6 text-secondary">{{ time.guest }}</div>
+                <div class="col-3 text-primary font-weight-bold">Guest: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.guest }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.guest }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-4 text-primary font-weight-bold">Guest Nice: </div>
-                <div class="col-2 text-secondary">{{ time_percent.guest_nice }}%</div>
-                <div class="col-6 text-secondary">{{ time.guest_nice }}</div>
+                <div class="col-3 text-primary font-weight-bold">Guest Nice: </div>
+                <div class="col-2 text-secondary">{{ data.time_percent.guest_nice }}%</div>
+                <div class="col-7 text-secondary">{{ data.time.guest_nice }}</div>
             </div>
 
         </div>
 
         <div class="col-5">
             <div class="h3 font-weight-bold text-primary">CPU Frequencies</div>
             <div class="row m-3">
-                <div class="col-5 text-primary font-weight-bold">Current: </div>
-                <div class="col-7 text-secondary">{{ frequency.current }}</div>
+                <div class="col-6 text-primary font-weight-bold">Current: </div>
+                <div class="col-6 text-secondary">{{ data.frequency.current }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-5 text-primary font-weight-bold">Min: </div>
-                <div class="col-7 text-secondary">{{ frequency.min }}</div>
+                <div class="col-6 text-primary font-weight-bold">Min: </div>
+                <div class="col-6 text-secondary">{{ data.frequency.min }}</div>
             </div>
             <div class="row m-3">
-                <div class="col-5 text-primary font-weight-bold">Max: </div>
-                <div class="col-7 text-secondary">{{ frequency.max }}</div>
+                <div class="col-6 text-primary font-weight-bold">Max: </div>
+                <div class="col-6 text-secondary">{{ data.frequency.max }}</div>
             </div>
         </div>
     </div>
 </div>
+{% else %}
+<div class="container-fluid">
+    data not available for this partition
+</div>
+{% endif %}
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_interface_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_interface_stats.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_partition_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/templates/hostutils/bs5/ajax/host_interface_stats.htm`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,28 @@
-{% load handyhelper_tags %}
+{% if data %}
 <div class="container-fluid">
     <div class="row m-3">
-        <div class="col-3 text-primary font-weight-bold">Total: </div>
-        <div class="col-9 text-secondary">{{ data.total|byte_size }}</div>
+        <div class="col-3 text-primary font-weight-bold">Up: </div>
+        <div class="col-9 text-secondary">{{ data.isup }}</div>
     </div>
     <div class="row m-3">
-        <div class="col-3 text-primary font-weight-bold">Used:</div>
-        <div class="col-9 text-secondary">{{ data.used|byte_size }}</div>
+        <div class="col-3 text-primary font-weight-bold">Duplex:</div>
+        <div class="col-9 text-secondary">{{ data.duplex.name }}</div>
     </div>
     <div class="row m-3">
-        <div class="col-3 text-primary font-weight-bold">Free:</div>
-        <div class="col-9 text-secondary">{{ data.free|byte_size }}</div>
+        <div class="col-3 text-primary font-weight-bold">Speed:</div>
+        <div class="col-9 text-secondary">{{ data.speed }}</div>
     </div>
     <div class="row m-3">
-        <div class="col-3 text-primary font-weight-bold">Percent:</div>
-        <div class="col-9 text-secondary">{{ data.percent }}%</div>
+        <div class="col-3 text-primary font-weight-bold">MTU:</div>
+        <div class="col-9 text-secondary">{{ data.mtu }}</div>
     </div>
+    <div class="row m-3">
+        <div class="col-3 text-primary font-weight-bold">Flags:</div>
+        <div class="col-9 text-secondary">{{ data.flags }}</div>
+    </div>
+</div>
+{% else %}
+<div class="container-fluid">
+    data not available for this partition
 </div>
+{% endif %}
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/htmx/get_process_stats.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/ajax/get_process_stats.htm`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 {% load handyhelper_tags %}
+{% if data %}
 <div class="container-fluid">
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">PID: </div>
-        <div class="col-9 text-secondary">{{ pid }}</div>
+        <div class="col-9 text-secondary">{{ data.pid }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">PPID: </div>
-        <div class="col-9 text-secondary">{{ ppid }}</div>
+        <div class="col-9 text-secondary">{{ data.ppid }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Name:</div>
-        <div class="col-9 text-secondary">{{ name }}</div>
+        <div class="col-9 text-secondary">{{ data.name }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Status:</div>
-        <div class="col-9 text-secondary">{{ status }}</div>
+        <div class="col-9 text-secondary">{{ data.status }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Stated At:</div>
-        <div class="col-9 text-secondary">{{ create_time|to_datetime }}</div>
+        <div class="col-9 text-secondary">{{ data.create_time|to_datetime }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Username:</div>
-        <div class="col-9 text-secondary">{{ username }}</div>
+        <div class="col-9 text-secondary">{{ data.username }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Command:</div>
-        <div class="col-9 text-secondary">{{ cmdline|join:" " }}</div>
+        <div class="col-9 text-secondary">{{ data.cmdline|join:" " }}</div>
     </div>
-    {% if exe %}
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Executable:</div>
-        <div class="col-9 text-secondary">{{ exe }}</div>
+        <div class="col-9 text-secondary">{{ data.exe }}</div>
     </div>
-    {% endif %}
-    {% if cwd %}
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Working Directory:</div>
-        <div class="col-9 text-secondary">{{ cwd }}</div>
+        <div class="col-9 text-secondary">{{ data.cwd }}</div>
     </div>
-    {% endif %}
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">CPU:</div>
-        <div class="col-9 text-secondary">{{ cpu_num }}</div>
+        <div class="col-9 text-secondary">{{ data.cpu_num }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">CPU Percent:</div>
-        <div class="col-9 text-secondary">{{ cpu_percent }}%</div>
+        <div class="col-9 text-secondary">{{ data.cpu_percent }}%</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Memory Percent:</div>
-        <div class="col-9 text-secondary">{{ memory_percent|percentage }}</div>
+        <div class="col-9 text-secondary">{{ data.memory_percent|percentage }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Thread Count:</div>
-        <div class="col-9 text-secondary">{{ num_threads }}</div>
+        <div class="col-9 text-secondary">{{ data.num_threads }}</div>
     </div>
     <div class="row m-3">
         <div class="col-3 text-primary font-weight-bold">Threads:</div>
-        <div class="col-9 text-secondary">{% for thread in threads%}{{ thread }}<br>{% endfor %}</div>
+        <div class="col-9 text-secondary">{{ data.threads|join:", " }}</div>
     </div>
 </div>
+{% else %}
+<div class="container-fluid">
+    data not available for this process
+</div>
+{% endif %}
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/host_process_card.htm`

 * *Files 18% similar despite different names*

```diff
@@ -17,16 +17,15 @@
                     </div>
                 </div>
             </div>
                 <div class="card-body" style="overflow-y: auto; overflow-x: hidden; max-height: 50vh; cursor: pointer;">
                     <ul class="list-group mx-auto justify-content-center" style="max-width: 93%; margin-top: .5%; margin-bottom: .5%">
                         {% for item in process_list %}
                         <li class="list-group-item bg-light shadow-sm hvr-grow mb-3">
-                            {% comment %} <div onClick="showInfo('{% url "hostutils:get_process_stats" %}', '{{item.pid}}', 'Process Details: <small><i>{{item.name}}</i></small>', true);"> {% endcomment %}
-                            <div hx-get="{% url 'hostutils:get_process_stats' item.pid %}" hx-target="#modal_wrapper">
+                            <div onClick="showInfo('{% url "hostutils:get_process_stats" %}', '{{item.pid}}', 'Process Details: <small><i>{{item.name}}</i></small>', true);">
                                 <div class="row">
                                     <div class="col-xs-12 col-md-2"><span class="key">PID:</span><span class="value">{{ item.pid }}</span></div>
                                     <div class="col-xs-12 col-md-4"><span class="key">Name:</span><span class="value">{{ item.name }}</span></div>
                                     <div class="col-xs-12 col-md-2"><span class="key">Status:</span><span class="value">{{ item.status }}</span></div>
                                     <div class="col-xs-12 col-md-4"><span class="key">Started At:</span><span class="value">{{ item.create_time|to_datetime }}</span></div>
                                 </div>
                             </div>
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/hostutils_nav_menu.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/templates/hostutils/bs5/snippets/processes_title_cards.htm`

 * *Files identical despite different names*

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/urls.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from django.urls import path
+from djangoaddicts.hostutils.views import ajax
 from djangoaddicts.hostutils.views import gui
 from djangoaddicts.hostutils.views import htmx
 
 app_name = "hostutils"
 
 urlpatterns = [
     # host views
     path("host_cpu/", gui.ShowHostCpu.as_view(), name="host_cpu"),
     path("host_details/", gui.ShowHost.as_view(), name="host_details"),
     path("host_disk/", gui.ShowHostDisk.as_view(), name="host_disk"),
     path("host_memory/", gui.ShowHostMemory.as_view(), name="host_memory"),
     path("host_network/", gui.ShowHostNetwork.as_view(), name="host_network"),
     path("host_process/", gui.ShowHostProcesses.as_view(), name="host_process"),
+    # ajax views
+    path("get_cpu_stats/", ajax.GetHostCpuStats.as_view(), name="get_cpu_stats"),
+    path("get_interface_stats/", ajax.GetHostNetworkStats.as_view(), name="get_interface_stats"),
+    path("get_partition_stats/", ajax.GetHostParitionStats.as_view(), name="get_partition_stats"),
+    path("get_process_stats/", ajax.GetHostProcessStats.as_view(), name="get_process_stats"),
     # htmx views
     path("get_host_processes/", htmx.GetHostProcesses.as_view(), name="get_host_processes"),
-    path("get_cpu_stats/<int:cpu>/", htmx.GetHostCpuStats.as_view(), name="get_cpu_stats"),
-    path("get_interface_stats/<str:interface>/", htmx.GetHostNetworkStats.as_view(), name="get_interface_stats"),
-    path("get_partition_stats/", htmx.GetHostParitionStats.as_view(), name="get_partition_stats"),
-    path("get_process_stats/<int:pid>/", htmx.GetHostProcessStats.as_view(), name="get_process_stats"),
-
 ]
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/views/__init__.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from djangoaddicts.hostutils.views.ajax import (
+    GetHostCpuStats,
+    GetHostNetworkStats,
+    GetHostParitionStats,
+    GetHostProcessStats,
+)
 from djangoaddicts.hostutils.views.gui import (
     ShowHost,
     ShowHostCpu,
     ShowHostDisk,
     ShowHostMemory,
     ShowHostNetwork,
     ShowHostProcesses,
 )
-from djangoaddicts.hostutils.views.htmx import (
-    GetHostProcesses,
-    GetHostCpuStats,
-    GetHostNetworkStats,
-    GetHostParitionStats,
-    GetHostProcessStats,
-)
+from djangoaddicts.hostutils.views.htmx import GetHostProcesses
+
 
 __all__ = [
     "GetHostCpuStats",
     "GetHostNetworkStats",
     "GetHostParitionStats",
     "GetHostProcessStats",
     "GetHostProcesses",
```

### Comparing `django-hostutils-0.0.5/src/djangoaddicts/hostutils/views/gui.py` & `django-hostutils-0.0.dev3/src/djangoaddicts/hostutils/views/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 from djangoaddicts.hostutils.forms import HostProcessFilterForm
 
 
 class ShowHost(View):
     """Display dashboard like page showing an overview of host data"""
 
     template_name = "hostutils/bs5/detail/detail_host.html"
-    title = "Host Dashboard"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         now = datetime.datetime.now()
         context = {}
-        context["title"] = self.title
+        context["title"] = "Host Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
         context["cpu_count"] = psutil.cpu_count(logical=False)
         context["memory"] = psutil.virtual_memory()
         context["disk_usage"] = psutil.disk_usage("/")
         context["disk_io_counters"] = psutil.disk_io_counters()
         context["network"] = psutil.net_connections()
         context["pids"] = psutil.pids()
@@ -37,128 +36,123 @@
         )
 
         context["platform"] = psutil.os.uname()
 
         return render(request, self.template_name, context=context)
 
 
-class ShowHostCpu(View):
-    """Display dashboard like page showing host cpu data"""
+class ShowHostProcesses(View):
+    """Display dashboard like page showing host process data"""
 
-    template_name = "hostutils/bs5/detail/cpu.html"
-    title = "CPU Dashboard"
+    template_name = "hostutils/bs5/detail/processes.html"
 
     def get(self, request, *args, **kwargs):
-        """CPU Dashboard"""
+        """allow get method"""
         context = {}
-        context["title"] = self.title
+        context["title"] = "Host Processes"
+        context["now"] = datetime.datetime.now()
         context["subtitle"] = psutil.os.uname()[1]
-        context["stats"] = psutil.cpu_stats()
-        context["physical_count"] = psutil.cpu_count(logical=False)
-        context["logical_count"] = psutil.cpu_count(logical=True)
-        context["percent"] = psutil.cpu_percent(interval=None)
-        context["times_list"] = psutil.cpu_times(percpu=True)
-        context["times_percent_list"] = psutil.cpu_times_percent(percpu=True)
-        context["percent_list"] = psutil.cpu_percent(interval=None, percpu=True)
-        context["frequency_list"] = psutil.cpu_freq(percpu=True)
-        context["cpu_range"] = list(range(psutil.cpu_count(logical=True)))
-        cpu_data = {}
-        for i in range(context["logical_count"]):
-            cpu_data[i] = {
-                "times": context["times_list"][i],
-                "time_percent": context["times_percent_list"][i],
-                "percent": context["percent_list"][i],
-                "frequency": context["frequency_list"][i],
-            }
-        context["cpu_data"] = cpu_data
-        context["load_avg_1"], context["load_avg_5"], context["load_avg_15"] = [
-            round(x / psutil.cpu_count() * 100, 2) for x in psutil.getloadavg()
-        ]
+        process_list = list(psutil.process_iter())
+        context["process_list"] = process_list
+        counts = {
+            "running": len([i for i in process_list if i.status() == "running"]),
+            "sleeping": len([i for i in process_list if i.status() == "sleeping"]),
+            "idle": len([i for i in process_list if i.status() == "idle"]),
+            "stopped": len([i for i in process_list if i.status() == "stopped"]),
+            "zombie": len([i for i in process_list if i.status() == "zombie"]),
+            "dead": len([i for i in process_list if i.status() == "dead"]),
+        }
+        context["counts"] = counts
+        filter_form = {}
+        filter_form["form"] = HostProcessFilterForm(request.GET or None)
+        filter_form["modal_name"] = "filter_processes"
+        filter_form["modal_size"] = "modal-lg"
+        filter_form["modal_title"] = "Filter Host Processes"
+        filter_form["hx_method"] = "hx-get"
+        filter_form["hx_url"] = "/hostutils/get_host_processes"
+        filter_form["hx_target"] = "id_process_list_container"
+        filter_form["method"] = "GET"
+        filter_form["action"] = "Filter"
+        context["filter_form"] = filter_form
+        return render(request, self.template_name, context=context)
+
+
+class ShowHostNetwork(View):
+    """Display dashboard like page showing host network data"""
+
+    template_name = "hostutils/bs5/detail/network.html"
+
+    def get(self, request, *args, **kwargs):
+        """allow get method"""
+        context = {}
+        context["title"] = "Network Dashboard"
+        context["subtitle"] = psutil.os.uname()[1]
+        context["connection_list"] = psutil.net_connections()
+        context["interface_list"] = psutil.net_if_addrs()
+        context["stats_list"] = psutil.net_if_stats()
+        context["counters"] = psutil.net_io_counters()
         return render(request, self.template_name, context=context)
 
 
 class ShowHostDisk(View):
     """Display dashboard like page showing host disk data"""
 
     template_name = "hostutils/bs5/detail/disk.html"
-    title = "Disk Dashboard"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         context = {}
-        context["title"] = self.title
+        context["title"] = "Disk Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
         context["usage"] = psutil.disk_usage("/")
         context["io_counters"] = psutil.disk_io_counters()
         context["partition_lists"] = psutil.disk_partitions()
         return render(request, self.template_name, context=context)
 
 
 class ShowHostMemory(View):
     """Display dashboard like page showing host memory data"""
 
     template_name = "hostutils/bs5/detail/memory.html"
-    title = "Memory Dashboard"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         context = {}
-        context["title"] = self.title
+        context["title"] = "Memory Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
         context["virtual"] = psutil.virtual_memory()
         context["swap"] = psutil.swap_memory()
         return render(request, self.template_name, context=context)
 
 
-class ShowHostNetwork(View):
-    """Display dashboard like page showing host network data"""
-
-    template_name = "hostutils/bs5/detail/network.html"
-    title = "Network Dashboard"
-
-    def get(self, request, *args, **kwargs):
-        """allow get method"""
-        context = {}
-        context["title"] = self.title
-        context["subtitle"] = psutil.os.uname()[1]
-        context["connection_list"] = psutil.net_connections()
-        context["interface_list"] = psutil.net_if_addrs()
-        context["stats_list"] = psutil.net_if_stats()
-        context["counters"] = psutil.net_io_counters()
-        return render(request, self.template_name, context=context)
-
-
-class ShowHostProcesses(View):
-    """Display dashboard like page showing host process data"""
+class ShowHostCpu(View):
+    """Display dashboard like page showing host cpu data"""
 
-    template_name = "hostutils/bs5/detail/processes.html"
-    title = "Process Dashboard"
+    template_name = "hostutils/bs5/detail/cpu.html"
 
     def get(self, request, *args, **kwargs):
         """allow get method"""
         context = {}
-        context["title"] = self.title
-        context["now"] = datetime.datetime.now()
+        context["title"] = "CPU Dashboard"
         context["subtitle"] = psutil.os.uname()[1]
-        process_list = list(psutil.process_iter())
-        context["process_list"] = process_list
-        counts = {
-            "running": len([i for i in process_list if i.status() == "running"]),
-            "sleeping": len([i for i in process_list if i.status() == "sleeping"]),
-            "idle": len([i for i in process_list if i.status() == "idle"]),
-            "stopped": len([i for i in process_list if i.status() == "stopped"]),
-            "zombie": len([i for i in process_list if i.status() == "zombie"]),
-            "dead": len([i for i in process_list if i.status() == "dead"]),
-        }
-        context["counts"] = counts
-        filter_form = {}
-        filter_form["form"] = HostProcessFilterForm(request.GET or None)
-        filter_form["modal_name"] = "filter_processes"
-        filter_form["modal_size"] = "modal-lg"
-        filter_form["modal_title"] = "Filter Host Processes"
-        filter_form["hx_method"] = "hx-get"
-        filter_form["hx_url"] = "/hostutils/get_host_processes"
-        filter_form["hx_target"] = "id_process_list_container"
-        filter_form["method"] = "GET"
-        filter_form["action"] = "Filter"
-        context["filter_form"] = filter_form
+        context["stats"] = psutil.cpu_stats()
+        context["physical_count"] = psutil.cpu_count(logical=False)
+        context["logical_count"] = psutil.cpu_count(logical=True)
+        context["percent"] = psutil.cpu_percent(interval=None)
+        context["times_list"] = psutil.cpu_times(percpu=True)
+        context["times_percent_list"] = psutil.cpu_times_percent(percpu=True)
+        context["percent_list"] = psutil.cpu_percent(interval=None, percpu=True)
+        context["frequency_list"] = psutil.cpu_freq(percpu=True)
+        context["cpu_range"] = list(range(psutil.cpu_count(logical=True)))
+        cpu_data = {}
+        for i in range(context["logical_count"]):
+            cpu_data[i] = {
+                "times": context["times_list"][i],
+                "time_percent": context["times_percent_list"][i],
+                "percent": context["percent_list"][i],
+                "frequency": context["frequency_list"][i],
+            }
+        context["cpu_data"] = cpu_data
+        context["load_avg_1"], context["load_avg_5"], context["load_avg_15"] = [
+            round(x / psutil.cpu_count() * 100, 2) for x in psutil.getloadavg()
+        ]
         return render(request, self.template_name, context=context)
```

