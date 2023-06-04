# Comparing `tmp/netbox-contract-2.0.1.tar.gz` & `tmp/netbox-contract-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-contract-2.0.1.tar", last modified: Thu Jun  1 20:35:33 2023, max compression
+gzip compressed data, was "netbox-contract-2.0.2.tar", last modified: Sun Jun  4 08:16:25 2023, max compression
```

## Comparing `netbox-contract-2.0.1.tar` & `netbox-contract-2.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.739246 netbox-contract-2.0.1/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.1/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2641 2023-06-01 20:35:33.739246 netbox-contract-2.0.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2102 2023-05-25 21:05:55.000000 netbox-contract-2.0.1/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-06-01 20:33:56.000000 netbox-contract-2.0.1/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-01 20:35:33.739246 netbox-contract-2.0.1/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.1/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.663245 netbox-contract-2.0.1/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.687245 netbox-contract-2.0.1/src/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-06-01 20:34:32.000000 netbox-contract-2.0.1/src/netbox_contract/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.707245 netbox-contract-2.0.1/src/netbox_contract/api/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/api/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4016 2023-05-25 20:01:58.000000 netbox-contract-2.0.1/src/netbox_contract/api/serializers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-05-23 17:57:34.000000 netbox-contract-2.0.1/src/netbox_contract/api/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      955 2023-05-22 22:26:02.000000 netbox-contract-2.0.1/src/netbox_contract/api/views.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1369 2023-05-10 21:06:50.000000 netbox-contract-2.0.1/src/netbox_contract/filtersets.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5629 2023-05-16 21:07:49.000000 netbox-contract-2.0.1/src/netbox_contract/forms.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.727246 netbox-contract-2.0.1/src/netbox_contract/migrations/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0001_initial.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0006_alter_contract_circuit.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0007_invoice_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0008_invoice_comments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0009_contract_external_reference.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0010_invoice_contracts.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0011_auto_20230122_2112.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0012_remove_invoice_contract.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0014_contract_end_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-05-13 17:53:07.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/0015_contractassignement.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/migrations/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5517 2023-05-24 18:15:36.000000 netbox-contract-2.0.1/src/netbox_contract/models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1644 2023-03-12 18:00:52.000000 netbox-contract-2.0.1/src/netbox_contract/navigation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/search.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3712 2023-05-30 21:11:00.000000 netbox-contract-2.0.1/src/netbox_contract/tables.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2027 2023-06-01 20:32:56.000000 netbox-contract-2.0.1/src/netbox_contract/template_content.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.731246 netbox-contract-2.0.1/src/netbox_contract/templates/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      775 2023-05-23 19:02:53.000000 netbox-contract-2.0.1/src/netbox_contract/templates/contract_assignements_bottom.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      305 2023-05-24 18:09:51.000000 netbox-contract-2.0.1/src/netbox_contract/templates/contract_list_bottom.html
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.739246 netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4257 2023-05-23 21:01:17.000000 netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/contract.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-05-22 21:27:25.000000 netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/contract_assignement.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/invoice.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-12 14:46:55.000000 netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/serviceprovider.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3751 2023-05-23 19:01:13.000000 netbox-contract-2.0.1/src/netbox_contract/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8388 2023-05-30 21:08:13.000000 netbox-contract-2.0.1/src/netbox_contract/views.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-01 20:35:33.699245 netbox-contract-2.0.1/src/netbox_contract.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2641 2023-06-01 20:35:33.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-06-01 20:35:33.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-01 20:35:33.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-01 20:35:33.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-01 20:35:33.000000 netbox-contract-2.0.1/src/netbox_contract.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.767368 netbox-contract-2.0.2/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.2/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.2/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2895 2023-06-04 08:16:25.767368 netbox-contract-2.0.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2356 2023-06-04 08:14:44.000000 netbox-contract-2.0.2/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-06-04 08:15:08.000000 netbox-contract-2.0.2/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-04 08:16:25.767368 netbox-contract-2.0.2/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.691366 netbox-contract-2.0.2/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.715367 netbox-contract-2.0.2/src/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-06-04 08:14:58.000000 netbox-contract-2.0.2/src/netbox_contract/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.735367 netbox-contract-2.0.2/src/netbox_contract/api/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/api/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4016 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/api/serializers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/api/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      955 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/api/views.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1369 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/filtersets.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5650 2023-06-01 21:20:01.000000 netbox-contract-2.0.2/src/netbox_contract/forms.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.743367 netbox-contract-2.0.2/src/netbox_contract/migrations/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0001_initial.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0006_alter_contract_circuit.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0007_invoice_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0008_invoice_comments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0009_contract_external_reference.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0010_invoice_contracts.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0011_auto_20230122_2112.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0012_remove_invoice_contract.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0014_contract_end_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0015_contractassignement.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5517 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1644 2023-03-12 18:00:52.000000 netbox-contract-2.0.2/src/netbox_contract/navigation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/search.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3712 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/tables.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2027 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/template_content.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.743367 netbox-contract-2.0.2/src/netbox_contract/templates/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      775 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/templates/contract_assignements_bottom.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      305 2023-05-24 18:09:51.000000 netbox-contract-2.0.2/src/netbox_contract/templates/contract_list_bottom.html
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.767368 netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4257 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/contract.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/contract_assignement.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/invoice.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/serviceprovider.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3751 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8388 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/views.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.727367 netbox-contract-2.0.2/src/netbox_contract.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2895 2023-06-04 08:16:25.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-06-04 08:16:25.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-04 08:16:25.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-04 08:16:25.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-04 08:16:25.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/top_level.txt
```

### Comparing `netbox-contract-2.0.1/LICENSE` & `netbox-contract-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/PKG-INFO` & `netbox-contract-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-contract
-Version: 2.0.1
+Version: 2.0.2
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -80,7 +80,15 @@
 ```
 
 ## release notes
 
 ### version 2.0.0
 
 Add a new contract asignement model to allow the assignement of contract not only to Circuits. The support for the direct Contract to Circuit relation will be removed in version 2.1.0 . In Order to migrate existing relations contract_migration.py script is provided and can be run from the django shell.
+
+#### version 2.0.1
+
+Add support contract assignement panel to devices.
+
+#### version 2.0.2
+
+Add support for Netbox 3.5 whcih become the minimum version supported to accoodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
```

### Comparing `netbox-contract-2.0.1/README.md` & `netbox-contract-2.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -66,7 +66,15 @@
 ```
 
 ## release notes
 
 ### version 2.0.0
 
 Add a new contract asignement model to allow the assignement of contract not only to Circuits. The support for the direct Contract to Circuit relation will be removed in version 2.1.0 . In Order to migrate existing relations contract_migration.py script is provided and can be run from the django shell.
+
+#### version 2.0.1
+
+Add support contract assignement panel to devices.
+
+#### version 2.0.2
+
+Add support for Netbox 3.5 whcih become the minimum version supported to accoodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
```

### Comparing `netbox-contract-2.0.1/pyproject.toml` & `netbox-contract-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netbox-contract"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
   { name="Marc Lebreuil", email="marc@famillelebreuil.net" },
 ]
 description = "Contract management plugin for Netbox"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `netbox-contract-2.0.1/src/netbox_contract/api/serializers.py` & `netbox-contract-2.0.2/src/netbox_contract/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/api/views.py` & `netbox-contract-2.0.2/src/netbox_contract/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/filtersets.py` & `netbox-contract-2.0.2/src/netbox_contract/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/forms.py` & `netbox-contract-2.0.2/src/netbox_contract/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django import forms
 import django_filters
-from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelBulkEditForm, NetBoxModelCSVForm
-from utilities.forms.fields import CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField, MultipleChoiceField
-from utilities.forms import CSVModelChoiceField, DatePicker,SlugField
+from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelBulkEditForm, NetBoxModelImportForm
+from utilities.forms.fields import CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField, MultipleChoiceField, CSVModelChoiceField, SlugField
+from utilities.forms.widgets import DatePicker
 from extras.filters import TagFilter
 from circuits.models import Circuit
 from .models import Contract, Invoice, ServiceProvider, StatusChoices, ContractAssignement
 
 class ContractForm(NetBoxModelForm):
     comments = CommentField()
     circuit=DynamicModelMultipleChoiceField(
@@ -68,15 +68,15 @@
 class InvoiceFilterSetForm(NetBoxModelFilterSetForm):
     model = Invoice
     contracts=DynamicModelMultipleChoiceField(
         queryset=Contract.objects.all(),
         required=False
     )
 
-class ContractCSVForm(NetBoxModelCSVForm):
+class ContractCSVForm(NetBoxModelImportForm):
     circuit = CSVModelChoiceField(
         queryset=Circuit.objects.all(),
         to_field_name='name',
         help_text='Related Circuit'
     )
 
     class Meta:
@@ -110,15 +110,15 @@
     )
 
     nullable_fields = (
         'comments',
     )
     model = Contract
 
-class InvoiceCSVForm(NetBoxModelCSVForm):
+class InvoiceCSVForm(NetBoxModelImportForm):
     contracts = CSVModelChoiceField(
         queryset=Contract.objects.all(),
         to_field_name='name',
         help_text='Related Contracts'
     )
 
     class Meta:
@@ -150,15 +150,15 @@
         fields = ('name', 'slug','portal_url',
             'comments', 'tags')
 
 class ServiceProviderFilterSetForm(NetBoxModelFilterSetForm):
     model = ServiceProvider
     tag = TagFilter()
 
-class ServiceProviderCSVForm(NetBoxModelCSVForm):
+class ServiceProviderCSVForm(NetBoxModelImportForm):
     slug = SlugField()
     comments = CommentField()
     class Meta:
         model = ServiceProvider
         fields = [
             'name', 'slug','portal_url',
             'comments', 'tags'
```

### Comparing `netbox-contract-2.0.1/src/netbox_contract/migrations/0001_initial.py` & `netbox-contract-2.0.2/src/netbox_contract/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py` & `netbox-contract-2.0.2/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py` & `netbox-contract-2.0.2/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py` & `netbox-contract-2.0.2/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py` & `netbox-contract-2.0.2/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/migrations/0006_alter_contract_circuit.py` & `netbox-contract-2.0.2/src/netbox_contract/migrations/0006_alter_contract_circuit.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/migrations/0011_auto_20230122_2112.py` & `netbox-contract-2.0.2/src/netbox_contract/migrations/0011_auto_20230122_2112.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py` & `netbox-contract-2.0.2/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/migrations/0015_contractassignement.py` & `netbox-contract-2.0.2/src/netbox_contract/migrations/0015_contractassignement.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/models.py` & `netbox-contract-2.0.2/src/netbox_contract/models.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/navigation.py` & `netbox-contract-2.0.2/src/netbox_contract/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/search.py` & `netbox-contract-2.0.2/src/netbox_contract/search.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/tables.py` & `netbox-contract-2.0.2/src/netbox_contract/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/template_content.py` & `netbox-contract-2.0.2/src/netbox_contract/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/templates/contract_assignements_bottom.html` & `netbox-contract-2.0.2/src/netbox_contract/templates/contract_assignements_bottom.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/contract.html` & `netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/contract.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/contract_assignement.html` & `netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/contract_assignement.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/invoice.html` & `netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/invoice.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/templates/netbox_contract/serviceprovider.html` & `netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/serviceprovider.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/urls.py` & `netbox-contract-2.0.2/src/netbox_contract/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract/views.py` & `netbox-contract-2.0.2/src/netbox_contract/views.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.1/src/netbox_contract.egg-info/PKG-INFO` & `netbox-contract-2.0.2/src/netbox_contract.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-contract
-Version: 2.0.1
+Version: 2.0.2
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -80,7 +80,15 @@
 ```
 
 ## release notes
 
 ### version 2.0.0
 
 Add a new contract asignement model to allow the assignement of contract not only to Circuits. The support for the direct Contract to Circuit relation will be removed in version 2.1.0 . In Order to migrate existing relations contract_migration.py script is provided and can be run from the django shell.
+
+#### version 2.0.1
+
+Add support contract assignement panel to devices.
+
+#### version 2.0.2
+
+Add support for Netbox 3.5 whcih become the minimum version supported to accoodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
```

### Comparing `netbox-contract-2.0.1/src/netbox_contract.egg-info/SOURCES.txt` & `netbox-contract-2.0.2/src/netbox_contract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

