# Comparing `tmp/rmlab-0.4.0.tar.gz` & `tmp/rmlab-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmlab-0.4.0.tar", last modified: Sun Apr 16 15:04:47 2023, max compression
+gzip compressed data, was "rmlab-0.4.1.tar", last modified: Sun Jun  4 11:25:07 2023, max compression
```

## Comparing `rmlab-0.4.0.tar` & `rmlab-0.4.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.269839 rmlab-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-04-16 15:04:27.000000 rmlab-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2214 2023-04-16 15:04:47.269839 rmlab-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-04-16 15:04:27.000000 rmlab-0.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-16 15:04:27.000000 rmlab-0.4.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-16 15:04:47.270840 rmlab-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.244838 rmlab-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.250838 rmlab-0.4.0/src/rmlab/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.255838 rmlab-0.4.0/src/rmlab/_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9590 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    14244 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/fetch.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/observability.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/remove.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)    10142 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_api/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.257839 rmlab-0.4.0/src/rmlab/_data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4993 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_data/conversions.py
--rw-rw-rw-   0 root         (0) root         (0)     6286 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_data/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1937 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_data/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.257839 rmlab-0.4.0/src/rmlab/_util/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.258839 rmlab-0.4.0/src/rmlab/api/
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.259839 rmlab-0.4.0/src/rmlab/api/fetch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/fetch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11464 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/fetch/core.py
--rw-rw-rw-   0 root         (0) root         (0)     8419 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/fetch/flight_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4924 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/fetch/parametric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.260839 rmlab-0.4.0/src/rmlab/api/observability/
--rw-rw-rw-   0 root         (0) root         (0)     1180 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/observability/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.261839 rmlab-0.4.0/src/rmlab/api/operations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4951 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/operations/optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     2962 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/operations/simulation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.261839 rmlab-0.4.0/src/rmlab/api/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/persistence/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/remove.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.262839 rmlab-0.4.0/src/rmlab/api/upload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13213 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/core.py
--rw-rw-rw-   0 root         (0) root         (0)     5216 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/flight_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.264839 rmlab-0.4.0/src/rmlab/api/upload/parametric/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/parametric/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2992 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/parametric/customers.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/parametric/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     4391 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/api/upload/parametric/pricing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.266839 rmlab-0.4.0/src/rmlab/data/
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6828 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/flight.py
--rw-rw-rw-   0 root         (0) root         (0)    10309 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/items.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.269839 rmlab-0.4.0/src/rmlab/data/parametric/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/_customers_base.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/_pricing_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8670 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/customers_choice.py
--rw-rw-rw-   0 root         (0) root         (0)     5413 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/customers_request.py
--rw-rw-rw-   0 root         (0) root         (0)     7923 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/pricing_behavior.py
--rw-rw-rw-   0 root         (0) root         (0)    10954 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/pricing_optimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     3922 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/parametric/pricing_range.py
--rw-rw-rw-   0 root         (0) root         (0)     4379 2023-04-16 15:04:27.000000 rmlab-0.4.0/src/rmlab/data/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:04:47.252838 rmlab-0.4.0/src/rmlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2214 2023-04-16 15:04:47.000000 rmlab-0.4.0/src/rmlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1713 2023-04-16 15:04:47.000000 rmlab-0.4.0/src/rmlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 15:04:47.000000 rmlab-0.4.0/src/rmlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 15:04:47.000000 rmlab-0.4.0/src/rmlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-16 15:04:47.000000 rmlab-0.4.0/src/rmlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.033424 rmlab-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-04 11:24:53.000000 rmlab-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-06-04 11:25:07.033424 rmlab-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-06-04 11:24:53.000000 rmlab-0.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-04 11:24:53.000000 rmlab-0.4.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-04 11:25:07.034424 rmlab-0.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.022424 rmlab-0.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.025424 rmlab-0.4.1/src/rmlab/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.027424 rmlab-0.4.1/src/rmlab/_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9590 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14244 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_api/fetch.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_api/observability.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_api/remove.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_api/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10142 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_api/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.027424 rmlab-0.4.1/src/rmlab/_data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4993 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_data/conversions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_data/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_data/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.028424 rmlab-0.4.1/src/rmlab/_util/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.028424 rmlab-0.4.1/src/rmlab/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.029424 rmlab-0.4.1/src/rmlab/api/fetch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/fetch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11464 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/fetch/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     8419 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/fetch/flight_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4924 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/fetch/parametric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.029424 rmlab-0.4.1/src/rmlab/api/observability/
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/observability/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.029424 rmlab-0.4.1/src/rmlab/api/operations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4951 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/operations/optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2962 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/operations/simulation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.030424 rmlab-0.4.1/src/rmlab/api/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/persistence/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/remove.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.030424 rmlab-0.4.1/src/rmlab/api/upload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13213 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/upload/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     5265 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/upload/flight_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.031424 rmlab-0.4.1/src/rmlab/api/upload/parametric/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/upload/parametric/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2992 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/upload/parametric/customers.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/upload/parametric/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4391 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/api/upload/parametric/pricing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.032424 rmlab-0.4.1/src/rmlab/data/
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/flight.py
+-rw-rw-rw-   0 root         (0) root         (0)    10309 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/items.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.033424 rmlab-0.4.1/src/rmlab/data/parametric/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/parametric/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/parametric/_customers_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/parametric/_pricing_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8670 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/parametric/customers_choice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/parametric/customers_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     7923 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/parametric/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/parametric/pricing_behavior.py
+-rw-rw-rw-   0 root         (0) root         (0)    10949 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/parametric/pricing_optimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3922 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/parametric/pricing_range.py
+-rw-rw-rw-   0 root         (0) root         (0)     4379 2023-06-04 11:24:53.000000 rmlab-0.4.1/src/rmlab/data/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:25:07.025424 rmlab-0.4.1/src/rmlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-06-04 11:25:07.000000 rmlab-0.4.1/src/rmlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-06-04 11:25:07.000000 rmlab-0.4.1/src/rmlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 11:25:07.000000 rmlab-0.4.1/src/rmlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 11:25:07.000000 rmlab-0.4.1/src/rmlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-04 11:25:07.000000 rmlab-0.4.1/src/rmlab.egg-info/top_level.txt
```

### Comparing `rmlab-0.4.0/LICENSE` & `rmlab-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/PKG-INFO` & `rmlab-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmlab
-Version: 0.4.0
+Version: 0.4.1
 Summary: RMLab python client
 Home-page: https://rmlab.ai
 Author: Anton Rey
 Author-email: aanton.rv@gmail.com
 Project-URL: Bug Tracker, https://rmlab.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rmlab-0.4.0/README.md` & `rmlab-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/setup.cfg` & `rmlab-0.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rmlab
-version = 0.4.0
+version = 0.4.1
 author = Anton Rey
 author_email = aanton.rv@gmail.com
 description = RMLab python client
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://rmlab.ai
 project_urls =
```

### Comparing `rmlab-0.4.0/src/rmlab/__init__.py` & `rmlab-0.4.1/src/rmlab/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/_api/base.py` & `rmlab-0.4.1/src/rmlab/_api/base.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/_api/fetch.py` & `rmlab-0.4.1/src/rmlab/_api/fetch.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/_api/remove.py` & `rmlab-0.4.1/src/rmlab/_api/remove.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/_api/simulation.py` & `rmlab-0.4.1/src/rmlab/_api/simulation.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/_api/upload.py` & `rmlab-0.4.1/src/rmlab/_api/upload.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/_data/conversions.py` & `rmlab-0.4.1/src/rmlab/_data/conversions.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/_data/enums.py` & `rmlab-0.4.1/src/rmlab/_data/enums.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/_data/types.py` & `rmlab-0.4.1/src/rmlab/_data/types.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/_util/__init__.py` & `rmlab-0.4.1/src/rmlab/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/__init__.py` & `rmlab-0.4.1/src/rmlab/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/fetch/core.py` & `rmlab-0.4.1/src/rmlab/api/fetch/core.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/fetch/flight_data.py` & `rmlab-0.4.1/src/rmlab/api/fetch/flight_data.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/fetch/parametric.py` & `rmlab-0.4.1/src/rmlab/api/fetch/parametric.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/observability/__init__.py` & `rmlab-0.4.1/src/rmlab/api/observability/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/operations/optimization.py` & `rmlab-0.4.1/src/rmlab/api/operations/optimization.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/operations/simulation.py` & `rmlab-0.4.1/src/rmlab/api/operations/simulation.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/persistence/__init__.py` & `rmlab-0.4.1/src/rmlab/api/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/remove.py` & `rmlab-0.4.1/src/rmlab/api/remove.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/upload/core.py` & `rmlab-0.4.1/src/rmlab/api/upload/core.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/upload/flight_data.py` & `rmlab-0.4.1/src/rmlab/api/upload/flight_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,38 +22,38 @@
         citysector_id: Optional[str] = None,
         sector_id: Optional[str] = None,
     ) -> None:
         """Upload a set of flights defined in a file.
 
         Args:
             scen_id (int): Scenario ID
-            data_fn (str): Filename (.csv or .json) defining the flights
+            items (Union[str, list]): A filename (.csv or .json) or list of filenames (.json) defining the flights
             citysector_id (Optional[str], optional): A citysector ID if all flights belong to the same citysector. Defaults to None.
             sector_id (Optional[str], optional): A sector ID if all flights belong to the same sector. Defaults to None.
 
         Arguments `citysector_id` and `sector_id` are always optional. If any of them provided, concurrent uploads of flights
             files belonging to different citysectors/sectors are allowed.
 
-        Where `data_fn` can refer to:
+        Where an item can refer to:
         * a **CSV file**, for instance:
         ```csv
         Airline,Aircraft,Origin,Destination,Flight number,On sale date,Departure date,Departure time,Duration
         MyCarrier,Airbus A320-b,MAD,GVA,2277,2022-04-01,2022-05-15,T16:30,T02:00
         MyCarrier,Airbus A320-b,MAD,GVA,2277,2022-04-01,2022-05-17,T20:30,T02:00
         ```
 
         * a **JSON file**, for instance:
         ```json
         [
             {"airline": "MyCarrier", "aircraft": "Airbus A320-b", "origin": "MAD", "destination": "GVA", "flight_number": "2277", "on_sale_date": "2022-04-01", "departure_date": "2022-05-15", "departure_time": "T16:30", "duration": "T02:00", },
             {"airline": "MyCarrier", "aircraft": "Airbus A320-b", "origin": "MAD", "destination": "GVA", "flight_number": "2277", "on_sale_date": "2022-04-01", "departure_date": "2022-05-17", "departure_time": "T20:30", "duration": "T02:00", },
         ]
 
-        * a **JSON list** like the previous.
         ```
+        * a list of json filenames like the previous.
         """
 
         await self._upload_unbounded_items(
             scen_id, Flight, items, citysector_id=citysector_id, sector_id=sector_id
         )
 
     async def upload_flights_data(
```

### Comparing `rmlab-0.4.0/src/rmlab/api/upload/parametric/customers.py` & `rmlab-0.4.1/src/rmlab/api/upload/parametric/customers.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/upload/parametric/filters.py` & `rmlab-0.4.1/src/rmlab/api/upload/parametric/filters.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/api/upload/parametric/pricing.py` & `rmlab-0.4.1/src/rmlab/api/upload/parametric/pricing.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/data/__init__.py` & `rmlab-0.4.1/src/rmlab/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/data/flight.py` & `rmlab-0.4.1/src/rmlab/data/flight.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/data/items.py` & `rmlab-0.4.1/src/rmlab/data/items.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/data/parametric/customers_choice.py` & `rmlab-0.4.1/src/rmlab/data/parametric/customers_choice.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/data/parametric/customers_request.py` & `rmlab-0.4.1/src/rmlab/data/parametric/customers_request.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/data/parametric/filter.py` & `rmlab-0.4.1/src/rmlab/data/parametric/filter.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/data/parametric/pricing_behavior.py` & `rmlab-0.4.1/src/rmlab/data/parametric/pricing_behavior.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/data/parametric/pricing_optimizer.py` & `rmlab-0.4.1/src/rmlab/data/parametric/pricing_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 class OptimizerOperator:
     """Optimizer operator parameters specify the forecasting,
     aggregation and maximization algorithms and which actions are
     performed after an optimization pass finishes.
 
     Args:
       forecaster_type (OptimizationForecasterKind): Forecaster type
-      maximizer_type (OptimizationMaximizerKind): Revenue maximizer type
+      maximizer (OptimizationMaximizerKind): Revenue maximizer type
       aggregate_type (OptimizationAggregatorKind): Type of aggregation of historic input data
       aggregate_value (Optional[float]): Numeric parameter of aggregation type
       effects (str): Actions to perform after maximization
 
     **Example 1**
 
     To create an operator that:
```

### Comparing `rmlab-0.4.0/src/rmlab/data/parametric/pricing_range.py` & `rmlab-0.4.1/src/rmlab/data/parametric/pricing_range.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab/data/scenario.py` & `rmlab-0.4.1/src/rmlab/data/scenario.py`

 * *Files identical despite different names*

### Comparing `rmlab-0.4.0/src/rmlab.egg-info/PKG-INFO` & `rmlab-0.4.1/src/rmlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmlab
-Version: 0.4.0
+Version: 0.4.1
 Summary: RMLab python client
 Home-page: https://rmlab.ai
 Author: Anton Rey
 Author-email: aanton.rv@gmail.com
 Project-URL: Bug Tracker, https://rmlab.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rmlab-0.4.0/src/rmlab.egg-info/SOURCES.txt` & `rmlab-0.4.1/src/rmlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

