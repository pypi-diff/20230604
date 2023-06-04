# Comparing `tmp/policyuniverse-1.5.1.20230531.tar.gz` & `tmp/policyuniverse-1.5.1.20230603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyuniverse-1.5.1.20230531.tar", last modified: Wed May 31 17:21:54 2023, max compression
+gzip compressed data, was "policyuniverse-1.5.1.20230603.tar", last modified: Sun Jun  4 03:23:38 2023, max compression
```

## Comparing `policyuniverse-1.5.1.20230531.tar` & `policyuniverse-1.5.1.20230603.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:21:54.715176 policyuniverse-1.5.1.20230531/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-31 17:21:54.715176 policyuniverse-1.5.1.20230531/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:21:54.711176 policyuniverse-1.5.1.20230531/policyuniverse/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/action_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/arn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/common.py
--rw-r--r--   0 runner    (1001) docker     (123)  7793680 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/data.json
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/expander_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/policyuniverse/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:21:54.715176 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 17:21:54.000000 policyuniverse-1.5.1.20230531/policyuniverse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 17:21:54.715176 policyuniverse-1.5.1.20230531/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-31 17:21:43.000000 policyuniverse-1.5.1.20230531/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 03:23:38.872851 policyuniverse-1.5.1.20230603/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-04 03:23:38.872851 policyuniverse-1.5.1.20230603/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 03:23:38.872851 policyuniverse-1.5.1.20230603/policyuniverse/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/action_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/arn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7810249 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/expander_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 03:23:38.872851 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-04 03:23:38.872851 policyuniverse-1.5.1.20230603/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/setup.py
```

### Comparing `policyuniverse-1.5.1.20230531/LICENSE` & `policyuniverse-1.5.1.20230603/LICENSE`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/PKG-INFO` & `policyuniverse-1.5.1.20230603/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230531
+Version: 1.5.1.20230603
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230531/README.md` & `policyuniverse-1.5.1.20230603/README.md`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse/__init__.py` & `policyuniverse-1.5.1.20230603/policyuniverse/__init__.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse/action.py` & `policyuniverse-1.5.1.20230603/policyuniverse/action.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse/action_categories.py` & `policyuniverse-1.5.1.20230603/policyuniverse/action_categories.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse/arn.py` & `policyuniverse-1.5.1.20230603/policyuniverse/arn.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse/common.py` & `policyuniverse-1.5.1.20230603/policyuniverse/common.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse/data.json` & `policyuniverse-1.5.1.20230603/policyuniverse/data.json`

 * *Files 0% similar despite different names*

```diff
@@ -7109,14 +7109,27 @@
       "concepts_doc_root": "https://docs.aws.amazon.com/appconfig/latest/userguide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/appconfig/latest/userguide/getting-started-with-appconfig-permissions.html"
     },
     "prefix": "appconfig"
   },
   "AppFlow": {
     "actions": {
+      "CancelFlowExecutions": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to cancel in-progress executions of an Amazon AppFlow flow",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/appflow/1.0/APIReference/API_CancelFlowExecutions.html"
+        }
+      },
       "CreateConnectorProfile": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a login profile to be used with Amazon AppFlow flows",
@@ -7519,15 +7532,15 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to use a connector profile while creating a flow in Amazon AppFlow",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": ""
+          "doc_page_rel": "https://docs.aws.amazon.com/appflow/1.0/APIReference/API_UseConnectorProfile.html"
         }
       }
     },
     "arn_format": "arn:${Partition}:appflow:${Region}:${Account}:${ResourceType}/${ResourceName}",
     "arn_regex": "^arn:${Partition}:appflow:.+:.+:.+",
     "description": "Amazon AppFlow",
     "docs": {
@@ -10744,14 +10757,27 @@
         "description": "Grants permission to create a workgroup",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/athena/latest/APIReference/API_CreateWorkGroup.html"
         }
       },
+      "DeleteCapacityReservation": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a capacity reservation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/athena/latest/APIReference/API_DeleteCapacityReservation.html"
+        }
+      },
       "DeleteDataCatalog": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete a datacatalog",
@@ -27507,14 +27533,27 @@
         "description": "Grants permission to restore an event data store",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awscloudtrail/latest/APIReference/API_RestoreEventDataStore.html"
         }
       },
+      "StartEventDataStoreIngestion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start ingestion on an event data store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/awscloudtrail/latest/APIReference/API_StartEventDataStoreIngestion.html"
+        }
+      },
       "StartImport": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to start an import of logged trail events from a source S3 bucket to a destination event data store",
@@ -27546,14 +27585,27 @@
         "description": "Grants permission to start a new query on a specified event data store",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/awscloudtrail/latest/APIReference/API_StartQuery.html"
         }
       },
+      "StopEventDataStoreIngestion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to stop ingestion on an event data store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/awscloudtrail/latest/APIReference/API_StopEventDataStoreIngestion.html"
+        }
+      },
       "StopImport": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to stop a specified import",
@@ -47765,14 +47817,31 @@
         "description": "Grants permission to cancel a single premigration assessment run",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_CancelReplicationTaskAssessmentRun.html"
         }
       },
+      "CreateDataMigration": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys",
+          "dms:req-tag/${TagKey}"
+        ],
+        "description": "Grants permission to create a database migration using the provided settings",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "CreateDataProvider": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -47863,14 +47932,31 @@
         "description": "Grants permission to create an migration project using the provided settings",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
+      "CreateReplicationConfig": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys",
+          "dms:req-tag/${TagKey}"
+        ],
+        "description": "Grants permission to create a replication config using the provided settings",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "CreateReplicationInstance": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -47940,14 +48026,27 @@
         "description": "Grants permission to delete the specified connection between a replication instance and an endpoint",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_DeleteConnection.html"
         }
       },
+      "DeleteDataMigration": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete the specified database migration",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "DeleteDataProvider": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete the specified data provider",
@@ -48031,14 +48130,27 @@
         "description": "Grants permission to delete the specified migration project",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
+      "DeleteReplicationConfig": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete the specified replication config",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "DeleteReplicationInstance": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete the specified replication instance",
@@ -48139,14 +48251,28 @@
         "description": "Grants permission to describe the status of the connections that have been made between the replication instance and an endpoint",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_DescribeConnections.html"
         }
       },
+      "DescribeDataMigrations": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to return information about database migrations for your account in the specified region",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "DescribeEndpointSettings": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -48363,14 +48489,28 @@
         "description": "Grants permission to returns the status of the RefreshSchemas operation",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_DescribeRefreshSchemasStatus.html"
         }
       },
+      "DescribeReplicationConfigs": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe replication configs",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "DescribeReplicationInstanceTaskLogs": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
@@ -48408,14 +48548,28 @@
         "description": "Grants permission to return information about the replication subnet groups",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_DescribeReplicationSubnetGroups.html"
         }
       },
+      "DescribeReplicationTableStatistics": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe replication table statistics",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "DescribeReplicationTaskAssessmentResults": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -48464,14 +48618,28 @@
         "description": "Grants permission to return information about replication tasks for your account in the current region",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_DescribeReplicationTasks.html"
         }
       },
+      "DescribeReplications": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe replications",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "DescribeSchemas": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -48674,14 +48842,27 @@
         "description": "Grants permission to list all tags for an AWS DMS resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_ListTagsForResource.html"
         }
       },
+      "ModifyDataMigration": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to modify the specified database migration",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "ModifyEndpoint": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to modify the specified endpoint",
@@ -48726,14 +48907,27 @@
         "description": "Grants permission to modify the status of the specified Fleet Advisor collector",
         "docs": {
           "api_doc": "",
           "doc_page": "${DocHomeURL}dms/latest/APIReference/Welcome.html",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
+      "ModifyReplicationConfig": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to modify the specified replication config",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "ModifyReplicationInstance": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to modify the replication instance to apply new settings",
@@ -48804,14 +48998,27 @@
         "description": "Grants permission to populate the schema for the specified endpoint",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_RefreshSchemas.html"
         }
       },
+      "ReloadReplicationTables": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to reload the target database table with the source for a replication",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "ReloadTables": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to reload the target database table with the source data",
@@ -48846,14 +49053,27 @@
         "description": "Grants permission to run a large-scale assessment (LSA) analysis on every Fleet Advisor collector in your account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_RunFleetAdvisorLsaAnalysis.html"
         }
       },
+      "StartDataMigration": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start the database migration",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "StartMetadataModelAssessment": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to start a new assessment of metadata model",
@@ -48924,14 +49144,27 @@
         "description": "Grants permission to start the analysis of your source database to provide recommendations of target engines",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_StartRecommendations.html"
         }
       },
+      "StartReplication": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start a replication",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "StartReplicationTask": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to start the replication task",
@@ -48963,14 +49196,40 @@
         "description": "Grants permission to start a new premigration assessment run for one or more individual assessments of a migration task",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTaskAssessmentRun.html"
         }
       },
+      "StopDataMigration": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to stop the database migration",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
+      "StopReplication": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to stop a replication",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
+        }
+      },
       "StopReplicationTask": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to stop the replication task",
@@ -134852,96 +135111,204 @@
       "concepts_doc_root": "https://docs.aws.amazon.com/grafana/latest/userguide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/grafana/latest/userguide/"
     },
     "prefix": "grafana"
   },
   "Marketplace Portal": {
     "actions": {
+      "GetAdditionalSellerNotificationRecipients": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to view additional seller notification recipients",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
+        }
+      },
+      "GetBankAccountVerificationDetails": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to view bank account verification status",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
+        }
+      },
+      "GetSecondaryUserVerificationDetails": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to view secondary user account verification status",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
+        }
+      },
+      "GetSellerVerificationDetails": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to view account verification status",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
+        }
+      },
+      "PutAdditionalSellerNotificationRecipients": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update additional seller notification recipients",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
+        }
+      },
+      "PutBankAccountVerificationDetails": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update bank account verification status",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
+        }
+      },
+      "PutSecondaryUserVerificationDetails": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update secondary user account verification status",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
+        }
+      },
+      "PutSellerVerificationDetails": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update account verification status",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
+        }
+      },
       "uploadFiles": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Allows access to the File Upload page inside the AWS Marketplace Management Portal.",
+        "description": "Allows access to the File Upload page inside the AWS Marketplace Management Portal",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
         }
       },
       "viewMarketing": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Allows access to the Marketing page inside the AWS Marketplace Management Portal.",
+        "description": "Allows access to the Marketing page inside the AWS Marketplace Management Portal",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
         }
       },
       "viewReports": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Allows access to the Reports page inside the AWS Marketplace Management Portal.",
+        "description": "Allows access to the Reports page inside the AWS Marketplace Management Portal",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
         }
       },
       "viewSettings": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Allows access to the Settings page inside the AWS Marketplace Management Portal.",
+        "description": "Allows access to the Settings page inside the AWS Marketplace Management Portal",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
         }
       },
       "viewSupport": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Allows access to the Customer Support Eligibility page inside the AWS Marketplace Management Portal.",
+        "description": "Allows access to the Customer Support Eligibility page inside the AWS Marketplace Management Portal",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/marketplace/latest/userguide/detailed-management-portal-permissions.html#seller-ammp-permissions"
         }
       }
     },
-    "arn_format": "",
-    "arn_regex": "",
+    "arn_format": "arn:${Partition}:Marketplace:${Region}:${Account}:${Resource}",
+    "arn_regex": "^arn:${Partition}:Marketplace:.+",
     "description": "AWS Marketplace Management Portal",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/marketplace/latest/userguide/",
       "api_detail_root": "",
       "api_doc_root": "",
-      "api_reference_doc_page": "",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/marketplace/latest/userguide/",
       "authz_doc_page": "https://docs.aws.amazon.com/marketplace/latest/userguide/marketplace-management-portal-user-access.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/marketplace/latest/userguide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/marketplace/latest/userguide/"
     },
     "prefix": "aws-marketplace-management"
   },
   "MechanicalTurk": {
@@ -215521,14 +215888,27 @@
         "description": "Grants permission to associate browser settings to web portals",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_AssociateBrowserSettings.html"
         }
       },
+      "AssociateIpAccessSettings": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to associate ip access settings with web portals",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_AssociateIpAccessSettings.html"
+        }
+      },
       "AssociateNetworkSettings": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to associate network settings to web portals",
@@ -215602,14 +215982,30 @@
         "description": "Grants permission to create identity providers",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_CreateIdentityProvider.html"
         }
       },
+      "CreateIpAccessSettings": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create ip access settings",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_CreateIpAccessSettings.html"
+        }
+      },
       "CreateNetworkSettings": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -215708,14 +216104,27 @@
         "description": "Grants permission to delete identity providers",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_DeleteIdentityProvider.html"
         }
       },
+      "DeleteIpAccessSettings": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete ip access settings",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_DeleteIpAccessSettings.html"
+        }
+      },
       "DeleteNetworkSettings": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete network settings",
@@ -215786,14 +216195,27 @@
         "description": "Grants permission to disassociate browser settings from web portals",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_DisassociateBrowserSettings.html"
         }
       },
+      "DisassociateIpAccessSettings": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to disassociate ip access logging from web portals",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_DisassociateIpAccessSettings.html"
+        }
+      },
       "DisassociateNetworkSettings": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to disassociate network settings from web portals",
@@ -215866,14 +216288,28 @@
         "description": "Grants permission to get details on identity providers",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_GetIdentityProvider.html"
         }
       },
+      "GetIpAccessSettings": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get details on ip access settings",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_GetIpAccessSettings.html"
+        }
+      },
       "GetNetworkSettings": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -215992,14 +216428,28 @@
         "description": "Grants permission to list identity providers",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_ListIdentityProviders.html"
         }
       },
+      "ListIpAccessSettings": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to list ip access settings",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_ListIpAccessSettings.html"
+        }
+      },
       "ListNetworkSettings": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -216150,14 +216600,27 @@
         "description": "Grants permission to update identity provider",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_UpdateIdentityProvider.html"
         }
       },
+      "UpdateIpAccessSettings": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update ip access settings",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/workspaces-web/latest/APIReference/API_UpdateIpAccessSettings.html"
+        }
+      },
       "UpdateNetworkSettings": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update network settings",
```

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse/expander_minimizer.py` & `policyuniverse-1.5.1.20230603/policyuniverse/expander_minimizer.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse/organization.py` & `policyuniverse-1.5.1.20230603/policyuniverse/organization.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse/policy.py` & `policyuniverse-1.5.1.20230603/policyuniverse/policy.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse/statement.py` & `policyuniverse-1.5.1.20230603/policyuniverse/statement.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse.egg-info/PKG-INFO` & `policyuniverse-1.5.1.20230603/policyuniverse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230531
+Version: 1.5.1.20230603
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230531/policyuniverse.egg-info/SOURCES.txt` & `policyuniverse-1.5.1.20230603/policyuniverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230531/setup.py` & `policyuniverse-1.5.1.20230603/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ROOT = os.path.realpath(os.path.join(os.path.dirname(__file__)))
 
 tests_require = ["pytest", "coveralls", "bandit"]
 dev_require = ["pre-commit", "black"]
 
 setup(
     name="policyuniverse",
-    version="1.5.1.20230531",
+    version="1.5.1.20230603",
     description="Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.",
     long_description=open(os.path.join(ROOT, "README.md")).read(),
     long_description_content_type="text/markdown",
     author="Patrick Kelley",
     author_email="patrickbarrettkelley@gmail.com",
     url="https://github.com/Netflix-Skunkworks/policyuniverse",
     keywords=[
```

