# Comparing `tmp/skypilot-0.3.0.tar.gz` & `tmp/skypilot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zongheng/Dropbox/workspace/riselab/sky-computing/dist/.tmp-oi70v4yj/skypilot-0.3.0.tar", last modified: Tue May 30 00:13:43 2023, max compression
+gzip compressed data, was "/Users/zongheng/Dropbox/workspace/riselab/sky-computing/dist/.tmp-5lp6ozo5/skypilot-0.3.1.tar", last modified: Sun Jun  4 16:54:31 2023, max compression
```

## Comparing `skypilot-0.3.0.tar` & `skypilot-0.3.1.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/
--rw-r--r--   0 zongheng   (502) staff       (20)    12170 2022-04-03 15:38:40.000000 skypilot-0.3.0/LICENSE
--rw-r--r--   0 zongheng   (502) staff       (20)      473 2023-05-28 16:45:59.000000 skypilot-0.3.0/MANIFEST.in
--rw-r--r--   0 zongheng   (502) staff       (20)     8079 2023-05-30 00:13:43.000000 skypilot-0.3.0/PKG-INFO
--rw-r--r--   0 zongheng   (502) staff       (20)     7163 2023-05-28 16:45:59.000000 skypilot-0.3.0/README.md
--rw-r--r--   0 zongheng   (502) staff       (20)      519 2023-05-28 16:43:06.000000 skypilot-0.3.0/pyproject.toml
--rw-r--r--   0 zongheng   (502) staff       (20)       38 2023-05-30 00:13:43.000000 skypilot-0.3.0/setup.cfg
--rw-r--r--   0 zongheng   (502) staff       (20)     7159 2023-05-28 17:22:30.000000 skypilot-0.3.0/setup.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/
--rw-r--r--   0 zongheng   (502) staff       (20)     2044 2023-05-30 00:13:09.000000 skypilot-0.3.0/sky/__init__.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/adaptors/
--rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/adaptors/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)     2607 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/adaptors/aws.py
--rw-r--r--   0 zongheng   (502) staff       (20)      989 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/adaptors/azure.py
--rw-r--r--   0 zongheng   (502) staff       (20)     7725 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/adaptors/cloudflare.py
--rw-r--r--   0 zongheng   (502) staff       (20)      852 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/adaptors/docker.py
--rw-r--r--   0 zongheng   (502) staff       (20)     2194 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/adaptors/gcp.py
--rw-r--r--   0 zongheng   (502) staff       (20)     3052 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/adaptors/ibm.py
--rw-r--r--   0 zongheng   (502) staff       (20)    15703 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/authentication.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/backends/
--rw-r--r--   0 zongheng   (502) staff       (20)      414 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/backends/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)     5542 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/backends/backend.py
--rw-r--r--   0 zongheng   (502) staff       (20)   114085 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/backends/backend_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)   183288 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 zongheng   (502) staff       (20)     8321 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/backends/docker_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)    16267 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/backends/monkey_patches/
--rw-r--r--   0 zongheng   (502) staff       (20)     3410 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 zongheng   (502) staff       (20)    24421 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/backends/onprem_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)     5903 2023-01-09 22:00:08.000000 skypilot-0.3.0/sky/backends/wheel_utils.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/benchmark/
--rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/benchmark/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)     8723 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/benchmark/benchmark_state.py
--rw-r--r--   0 zongheng   (502) staff       (20)    24632 2023-04-19 13:26:02.000000 skypilot-0.3.0/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)     3505 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/check.py
--rw-r--r--   0 zongheng   (502) staff       (20)   161212 2023-05-28 17:22:59.000000 skypilot-0.3.0/sky/cli.py
--rw-r--r--   0 zongheng   (502) staff       (20)     8588 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/cloud_stores.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/clouds/
--rw-r--r--   0 zongheng   (502) staff       (20)      617 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/clouds/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)    30999 2023-05-28 16:52:14.000000 skypilot-0.3.0/sky/clouds/aws.py
--rw-r--r--   0 zongheng   (502) staff       (20)    20568 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/azure.py
--rw-r--r--   0 zongheng   (502) staff       (20)    18690 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/cloud.py
--rw-r--r--   0 zongheng   (502) staff       (20)    31458 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/gcp.py
--rw-r--r--   0 zongheng   (502) staff       (20)    18104 2023-05-28 16:52:14.000000 skypilot-0.3.0/sky/clouds/ibm.py
--rw-r--r--   0 zongheng   (502) staff       (20)    10604 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/lambda_cloud.py
--rw-r--r--   0 zongheng   (502) staff       (20)     8062 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/local.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/clouds/service_catalog/
--rw-r--r--   0 zongheng   (502) staff       (20)    13177 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)    10773 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 zongheng   (502) staff       (20)     6705 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 zongheng   (502) staff       (20)    22851 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/common.py
--rw-r--r--   0 zongheng   (502) staff       (20)     1500 2023-04-19 13:26:02.000000 skypilot-0.3.0/sky/clouds/service_catalog/config.py
--rw-r--r--   0 zongheng   (502) staff       (20)      282 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 zongheng   (502) staff       (20)        0 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)    20092 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 zongheng   (502) staff       (20)     8421 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 zongheng   (502) staff       (20)    17799 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 zongheng   (502) staff       (20)     4155 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 zongheng   (502) staff       (20)    18924 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 zongheng   (502) staff       (20)     4656 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 zongheng   (502) staff       (20)     5414 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 zongheng   (502) staff       (20)     2281 2022-12-10 11:50:57.000000 skypilot-0.3.0/sky/config.py
--rw-r--r--   0 zongheng   (502) staff       (20)    38700 2023-05-28 16:58:17.000000 skypilot-0.3.0/sky/core.py
--rw-r--r--   0 zongheng   (502) staff       (20)     2477 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/dag.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/data/
--rw-r--r--   0 zongheng   (502) staff       (20)      128 2023-01-09 22:00:08.000000 skypilot-0.3.0/sky/data/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)     7273 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/data/data_transfer.py
--rw-r--r--   0 zongheng   (502) staff       (20)     7918 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/data/data_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)     3251 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/data/mounting_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)    88757 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/data/storage.py
--rw-r--r--   0 zongheng   (502) staff       (20)     1082 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/data/storage_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)     5893 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/exceptions.py
--rw-r--r--   0 zongheng   (502) staff       (20)    36869 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/execution.py
--rw-r--r--   0 zongheng   (502) staff       (20)    27126 2023-05-28 16:58:17.000000 skypilot-0.3.0/sky/global_user_state.py
--rw-r--r--   0 zongheng   (502) staff       (20)    44909 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/optimizer.py
--rw-r--r--   0 zongheng   (502) staff       (20)    41104 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/resources.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/setup_files/
--rw-r--r--   0 zongheng   (502) staff       (20)      473 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/setup_files/MANIFEST.in
--rw-r--r--   0 zongheng   (502) staff       (20)     7159 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/setup_files/setup.py
--rw-r--r--   0 zongheng   (502) staff       (20)     3216 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/sky_logging.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/
--rw-r--r--   0 zongheng   (502) staff       (20)    12568 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/LICENSE
--rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/skylet/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)     4378 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/skylet/autostop_lib.py
--rw-r--r--   0 zongheng   (502) staff       (20)     2118 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/skylet/configs.py
--rw-r--r--   0 zongheng   (502) staff       (20)      806 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/skylet/constants.py
--rw-r--r--   0 zongheng   (502) staff       (20)     9309 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/skylet/events.py
--rw-r--r--   0 zongheng   (502) staff       (20)    27771 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/skylet/job_lib.py
--rw-r--r--   0 zongheng   (502) staff       (20)    17792 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/skylet/log_lib.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/aws/
--rw-r--r--   0 zongheng   (502) staff       (20)      110 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)    32698 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 zongheng   (502) staff       (20)    52192 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/aws/config.py
--rw-r--r--   0 zongheng   (502) staff       (20)    29406 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 zongheng   (502) staff       (20)     5917 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/azure/
--rw-r--r--   0 zongheng   (502) staff       (20)       97 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)     4344 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 zongheng   (502) staff       (20)    10633 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 zongheng   (502) staff       (20)     5756 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/azure/config.py
--rw-r--r--   0 zongheng   (502) staff       (20)    17469 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/gcp/
--rw-r--r--   0 zongheng   (502) staff       (20)       91 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)    31015 2023-04-19 03:21:35.000000 skypilot-0.3.0/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 zongheng   (502) staff       (20)     2738 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 zongheng   (502) staff       (20)    26192 2023-04-18 01:28:59.000000 skypilot-0.3.0/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 zongheng   (502) staff       (20)    14276 2023-05-14 16:35:23.000000 skypilot-0.3.0/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/ibm/
--rw-r--r--   0 zongheng   (502) staff       (20)       94 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)    38280 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 zongheng   (502) staff       (20)     1290 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)    34628 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 zongheng   (502) staff       (20)      112 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)     8518 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)    13650 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/skylet/ray_patches/
--rw-r--r--   0 zongheng   (502) staff       (20)     2783 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)      294 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 zongheng   (502) staff       (20)      391 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 zongheng   (502) staff       (20)      224 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 zongheng   (502) staff       (20)      528 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 zongheng   (502) staff       (20)      658 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 zongheng   (502) staff       (20)      289 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 zongheng   (502) staff       (20)      565 2023-05-28 17:02:51.000000 skypilot-0.3.0/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 zongheng   (502) staff       (20)      603 2023-01-09 22:00:08.000000 skypilot-0.3.0/sky/skylet/skylet.py
--rw-r--r--   0 zongheng   (502) staff       (20)     2649 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 zongheng   (502) staff       (20)     5463 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/skypilot_config.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/spot/
--rw-r--r--   0 zongheng   (502) staff       (20)     1346 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/spot/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)      561 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/spot/constants.py
--rw-r--r--   0 zongheng   (502) staff       (20)    18420 2023-05-28 16:45:59.000000 skypilot-0.3.0/sky/spot/controller.py
--rw-r--r--   0 zongheng   (502) staff       (20)    19574 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/spot/recovery_strategy.py
--rw-r--r--   0 zongheng   (502) staff       (20)    13506 2023-04-19 13:26:02.000000 skypilot-0.3.0/sky/spot/spot_state.py
--rw-r--r--   0 zongheng   (502) staff       (20)    25411 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/spot/spot_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)    35504 2023-05-28 16:58:17.000000 skypilot-0.3.0/sky/task.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/templates/
--rw-r--r--   0 zongheng   (502) staff       (20)    11434 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 zongheng   (502) staff       (20)     9373 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 zongheng   (502) staff       (20)    10844 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 zongheng   (502) staff       (20)      505 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 zongheng   (502) staff       (20)      328 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 zongheng   (502) staff       (20)     8006 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 zongheng   (502) staff       (20)     6796 2023-05-28 17:22:30.000000 skypilot-0.3.0/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 zongheng   (502) staff       (20)     1424 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/templates/local-ray.yml.j2
--rw-r--r--   0 zongheng   (502) staff       (20)     2284 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/usage/
--rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/usage/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)      633 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/usage/constants.py
--rw-r--r--   0 zongheng   (502) staff       (20)    16946 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/usage/usage_lib.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/utils/
--rw-r--r--   0 zongheng   (502) staff       (20)       25 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/utils/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)     2806 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/sky/utils/cli_utils/
--rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.0/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 zongheng   (502) staff       (20)    14464 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)    14688 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/utils/command_runner.py
--rw-r--r--   0 zongheng   (502) staff       (20)    11033 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/utils/common_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)     1853 2023-04-03 17:20:30.000000 skypilot-0.3.0/sky/utils/db_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)      852 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/utils/env_options.py
--rw-r--r--   0 zongheng   (502) staff       (20)     4962 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/utils/log_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)     6611 2023-05-28 16:43:06.000000 skypilot-0.3.0/sky/utils/schemas.py
--rw-r--r--   0 zongheng   (502) staff       (20)     4078 2023-04-19 13:26:02.000000 skypilot-0.3.0/sky/utils/subprocess_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)     3965 2023-02-24 05:01:20.000000 skypilot-0.3.0/sky/utils/timeline.py
--rw-r--r--   0 zongheng   (502) staff       (20)     4186 2023-04-19 13:26:02.000000 skypilot-0.3.0/sky/utils/tpu_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)     1125 2023-05-28 16:49:29.000000 skypilot-0.3.0/sky/utils/ux_utils.py
--rw-r--r--   0 zongheng   (502) staff       (20)      701 2022-11-22 22:28:46.000000 skypilot-0.3.0/sky/utils/validator.py
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/
--rw-r--r--   0 zongheng   (502) staff       (20)     8079 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/PKG-INFO
--rw-r--r--   0 zongheng   (502) staff       (20)     4827 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/SOURCES.txt
--rw-r--r--   0 zongheng   (502) staff       (20)        1 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/dependency_links.txt
--rw-r--r--   0 zongheng   (502) staff       (20)       36 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/entry_points.txt
--rw-r--r--   0 zongheng   (502) staff       (20)     1155 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/requires.txt
--rw-r--r--   0 zongheng   (502) staff       (20)        4 2023-05-30 00:13:43.000000 skypilot-0.3.0/skypilot.egg-info/top_level.txt
-drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-05-30 00:13:43.000000 skypilot-0.3.0/tests/
--rw-r--r--   0 zongheng   (502) staff       (20)     2574 2023-05-28 16:52:14.000000 skypilot-0.3.0/tests/test_cli.py
--rw-r--r--   0 zongheng   (502) staff       (20)     5061 2023-05-28 16:43:06.000000 skypilot-0.3.0/tests/test_config.py
--rw-r--r--   0 zongheng   (502) staff       (20)      300 2021-12-14 23:56:33.000000 skypilot-0.3.0/tests/test_file_mount_helper.py
--rw-r--r--   0 zongheng   (502) staff       (20)      260 2022-11-22 22:28:46.000000 skypilot-0.3.0/tests/test_global_user_state.py
--rw-r--r--   0 zongheng   (502) staff       (20)     1076 2023-02-24 05:01:20.000000 skypilot-0.3.0/tests/test_list_accelerators.py
--rw-r--r--   0 zongheng   (502) staff       (20)    14008 2023-02-24 05:01:20.000000 skypilot-0.3.0/tests/test_onprem.py
--rw-r--r--   0 zongheng   (502) staff       (20)    19443 2023-05-28 16:45:59.000000 skypilot-0.3.0/tests/test_optimizer_dryruns.py
--rw-r--r--   0 zongheng   (502) staff       (20)     4663 2023-04-19 13:26:02.000000 skypilot-0.3.0/tests/test_optimizer_random_dag.py
--rw-r--r--   0 zongheng   (502) staff       (20)       94 2022-02-17 10:51:09.000000 skypilot-0.3.0/tests/test_pycryptodome_version.py
--rw-r--r--   0 zongheng   (502) staff       (20)   100651 2023-05-28 17:22:30.000000 skypilot-0.3.0/tests/test_smoke.py
--rw-r--r--   0 zongheng   (502) staff       (20)     7206 2023-04-03 17:20:30.000000 skypilot-0.3.0/tests/test_spot.py
--rw-r--r--   0 zongheng   (502) staff       (20)     4048 2023-05-28 16:43:06.000000 skypilot-0.3.0/tests/test_storage.py
--rw-r--r--   0 zongheng   (502) staff       (20)     1070 2023-01-09 22:00:08.000000 skypilot-0.3.0/tests/test_wheels.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/
+-rw-r--r--   0 zongheng   (502) staff       (20)    12170 2022-04-03 15:38:40.000000 skypilot-0.3.1/LICENSE
+-rw-r--r--   0 zongheng   (502) staff       (20)      473 2023-06-04 15:57:24.000000 skypilot-0.3.1/MANIFEST.in
+-rw-r--r--   0 zongheng   (502) staff       (20)     8102 2023-06-04 16:54:31.000000 skypilot-0.3.1/PKG-INFO
+-rw-r--r--   0 zongheng   (502) staff       (20)     7186 2023-06-04 15:57:24.000000 skypilot-0.3.1/README.md
+-rw-r--r--   0 zongheng   (502) staff       (20)      519 2023-05-28 16:43:06.000000 skypilot-0.3.1/pyproject.toml
+-rw-r--r--   0 zongheng   (502) staff       (20)       38 2023-06-04 16:54:31.000000 skypilot-0.3.1/setup.cfg
+-rw-r--r--   0 zongheng   (502) staff       (20)     7354 2023-06-04 15:57:24.000000 skypilot-0.3.1/setup.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/
+-rw-r--r--   0 zongheng   (502) staff       (20)     2044 2023-06-04 16:54:02.000000 skypilot-0.3.1/sky/__init__.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/adaptors/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.1/sky/adaptors/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2607 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/adaptors/aws.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      989 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/adaptors/azure.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     7726 2023-06-04 15:58:27.000000 skypilot-0.3.1/sky/adaptors/cloudflare.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      852 2022-07-22 04:56:35.000000 skypilot-0.3.1/sky/adaptors/docker.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2194 2023-05-28 16:43:06.000000 skypilot-0.3.1/sky/adaptors/gcp.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     3052 2023-06-01 22:29:03.000000 skypilot-0.3.1/sky/adaptors/ibm.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    15703 2023-06-04 15:57:23.000000 skypilot-0.3.1/sky/authentication.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/backends/
+-rw-r--r--   0 zongheng   (502) staff       (20)      414 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/backends/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5542 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/backends/backend.py
+-rw-r--r--   0 zongheng   (502) staff       (20)   114176 2023-06-04 15:57:37.000000 skypilot-0.3.1/sky/backends/backend_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)   183549 2023-06-04 15:57:37.000000 skypilot-0.3.1/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8321 2023-05-28 16:43:06.000000 skypilot-0.3.1/sky/backends/docker_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    16267 2023-05-28 16:43:06.000000 skypilot-0.3.1/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/backends/monkey_patches/
+-rw-r--r--   0 zongheng   (502) staff       (20)     3410 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    24422 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/backends/onprem_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5903 2023-01-09 22:00:08.000000 skypilot-0.3.1/sky/backends/wheel_utils.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/benchmark/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-11-22 22:28:46.000000 skypilot-0.3.1/sky/benchmark/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8723 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    24632 2023-04-19 13:26:02.000000 skypilot-0.3.1/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     3571 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/check.py
+-rw-r--r--   0 zongheng   (502) staff       (20)   161418 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/cli.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8592 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/cloud_stores.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/clouds/
+-rw-r--r--   0 zongheng   (502) staff       (20)      617 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/clouds/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    31552 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/clouds/aws.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    20568 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/clouds/azure.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    18690 2023-06-01 22:22:35.000000 skypilot-0.3.1/sky/clouds/cloud.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    31469 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/clouds/gcp.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    18104 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/clouds/ibm.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    10604 2023-06-01 22:22:35.000000 skypilot-0.3.1/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8062 2023-06-01 22:22:35.000000 skypilot-0.3.1/sky/clouds/local.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/clouds/service_catalog/
+-rw-r--r--   0 zongheng   (502) staff       (20)    13177 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    10773 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     6705 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    22851 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1500 2023-04-19 13:26:02.000000 skypilot-0.3.1/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      282 2023-06-02 16:01:04.000000 skypilot-0.3.1/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    20092 2023-06-01 22:22:35.000000 skypilot-0.3.1/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8421 2023-05-28 16:43:06.000000 skypilot-0.3.1/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    17799 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4198 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    19389 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4656 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5414 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2281 2022-12-10 11:50:57.000000 skypilot-0.3.1/sky/config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    39673 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/core.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2477 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/dag.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/data/
+-rw-r--r--   0 zongheng   (502) staff       (20)      128 2023-01-09 22:00:08.000000 skypilot-0.3.1/sky/data/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     7273 2023-05-28 16:43:06.000000 skypilot-0.3.1/sky/data/data_transfer.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     7918 2023-05-28 16:43:06.000000 skypilot-0.3.1/sky/data/data_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     3251 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/data/mounting_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    89078 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/data/storage.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1082 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/data/storage_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     6031 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/exceptions.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    37047 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/execution.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    27126 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/global_user_state.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    44909 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/optimizer.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    41104 2023-06-01 22:29:03.000000 skypilot-0.3.1/sky/resources.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/setup_files/
+-rw-r--r--   0 zongheng   (502) staff       (20)      473 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 zongheng   (502) staff       (20)     7354 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/setup_files/setup.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     3216 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/sky_logging.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/skylet/
+-rw-r--r--   0 zongheng   (502) staff       (20)    12568 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/LICENSE
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.1/sky/skylet/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4378 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/skylet/autostop_lib.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2118 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/skylet/configs.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1173 2023-06-04 15:57:37.000000 skypilot-0.3.1/sky/skylet/constants.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     9309 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/skylet/events.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    28338 2023-06-04 15:57:37.000000 skypilot-0.3.1/sky/skylet/job_lib.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    17792 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/skylet/log_lib.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/skylet/providers/
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/skylet/providers/aws/
+-rw-r--r--   0 zongheng   (502) staff       (20)      110 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.1/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    32698 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    52192 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    29406 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5917 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/skylet/providers/azure/
+-rw-r--r--   0 zongheng   (502) staff       (20)       97 2022-07-22 04:56:35.000000 skypilot-0.3.1/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4344 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 zongheng   (502) staff       (20)    10633 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 zongheng   (502) staff       (20)     5756 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    17469 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/skylet/providers/gcp/
+-rw-r--r--   0 zongheng   (502) staff       (20)       91 2022-07-22 04:56:35.000000 skypilot-0.3.1/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    31015 2023-04-19 03:21:35.000000 skypilot-0.3.1/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2738 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    26192 2023-04-18 01:28:59.000000 skypilot-0.3.1/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    14276 2023-05-14 16:35:23.000000 skypilot-0.3.1/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/skylet/providers/ibm/
+-rw-r--r--   0 zongheng   (502) staff       (20)       94 2023-06-01 22:29:03.000000 skypilot-0.3.1/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    38280 2023-06-01 22:29:03.000000 skypilot-0.3.1/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1290 2023-06-01 22:29:03.000000 skypilot-0.3.1/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    34628 2023-06-01 22:29:03.000000 skypilot-0.3.1/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 zongheng   (502) staff       (20)      112 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     8518 2023-05-28 16:43:06.000000 skypilot-0.3.1/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    13650 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/skylet/ray_patches/
+-rw-r--r--   0 zongheng   (502) staff       (20)     2783 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      294 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      391 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      224 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      528 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      658 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      289 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      565 2023-06-03 18:06:12.000000 skypilot-0.3.1/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 zongheng   (502) staff       (20)      603 2023-01-09 22:00:08.000000 skypilot-0.3.1/sky/skylet/skylet.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2649 2023-06-04 15:46:29.000000 skypilot-0.3.1/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5654 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/skypilot_config.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/spot/
+-rw-r--r--   0 zongheng   (502) staff       (20)     1346 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/spot/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      561 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/spot/constants.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    18420 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/spot/controller.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    20897 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/spot/recovery_strategy.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    13506 2023-04-19 13:26:02.000000 skypilot-0.3.1/sky/spot/spot_state.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    25411 2023-05-28 16:43:06.000000 skypilot-0.3.1/sky/spot/spot_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    35659 2023-06-04 15:57:37.000000 skypilot-0.3.1/sky/task.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/templates/
+-rw-r--r--   0 zongheng   (502) staff       (20)    11468 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)     9407 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)    10878 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)      505 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)      328 2022-11-22 22:28:46.000000 skypilot-0.3.1/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)     8040 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)     6830 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)     1424 2022-11-22 22:28:46.000000 skypilot-0.3.1/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 zongheng   (502) staff       (20)     2356 2023-06-04 15:57:24.000000 skypilot-0.3.1/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/usage/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-11-22 22:28:46.000000 skypilot-0.3.1/sky/usage/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      633 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/usage/constants.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    16946 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/usage/usage_lib.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/utils/
+-rw-r--r--   0 zongheng   (502) staff       (20)       25 2022-11-22 22:28:46.000000 skypilot-0.3.1/sky/utils/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     2806 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/sky/utils/cli_utils/
+-rw-r--r--   0 zongheng   (502) staff       (20)        0 2022-07-22 04:56:35.000000 skypilot-0.3.1/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    14464 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    14688 2023-05-28 16:43:06.000000 skypilot-0.3.1/sky/utils/command_runner.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    11033 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/utils/common_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1853 2023-04-03 17:20:30.000000 skypilot-0.3.1/sky/utils/db_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      852 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/utils/env_options.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4962 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/utils/log_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     6611 2023-06-01 22:22:35.000000 skypilot-0.3.1/sky/utils/schemas.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4078 2023-06-01 23:01:59.000000 skypilot-0.3.1/sky/utils/subprocess_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     3965 2023-02-24 05:01:20.000000 skypilot-0.3.1/sky/utils/timeline.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4186 2023-04-19 13:26:02.000000 skypilot-0.3.1/sky/utils/tpu_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1125 2023-06-01 22:47:29.000000 skypilot-0.3.1/sky/utils/ux_utils.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      701 2022-11-22 22:28:46.000000 skypilot-0.3.1/sky/utils/validator.py
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/skypilot.egg-info/
+-rw-r--r--   0 zongheng   (502) staff       (20)     8102 2023-06-04 16:54:31.000000 skypilot-0.3.1/skypilot.egg-info/PKG-INFO
+-rw-r--r--   0 zongheng   (502) staff       (20)     4827 2023-06-04 16:54:31.000000 skypilot-0.3.1/skypilot.egg-info/SOURCES.txt
+-rw-r--r--   0 zongheng   (502) staff       (20)        1 2023-06-04 16:54:31.000000 skypilot-0.3.1/skypilot.egg-info/dependency_links.txt
+-rw-r--r--   0 zongheng   (502) staff       (20)       36 2023-06-04 16:54:31.000000 skypilot-0.3.1/skypilot.egg-info/entry_points.txt
+-rw-r--r--   0 zongheng   (502) staff       (20)     1163 2023-06-04 16:54:31.000000 skypilot-0.3.1/skypilot.egg-info/requires.txt
+-rw-r--r--   0 zongheng   (502) staff       (20)        4 2023-06-04 16:54:31.000000 skypilot-0.3.1/skypilot.egg-info/top_level.txt
+drwxr-xr-x   0 zongheng   (502) staff       (20)        0 2023-06-04 16:54:31.000000 skypilot-0.3.1/tests/
+-rw-r--r--   0 zongheng   (502) staff       (20)     2574 2023-06-01 22:47:29.000000 skypilot-0.3.1/tests/test_cli.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     5061 2023-05-28 16:43:06.000000 skypilot-0.3.1/tests/test_config.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      300 2021-12-14 23:56:33.000000 skypilot-0.3.1/tests/test_file_mount_helper.py
+-rw-r--r--   0 zongheng   (502) staff       (20)      260 2022-11-22 22:28:46.000000 skypilot-0.3.1/tests/test_global_user_state.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1076 2023-02-24 05:01:20.000000 skypilot-0.3.1/tests/test_list_accelerators.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    14008 2023-02-24 05:01:20.000000 skypilot-0.3.1/tests/test_onprem.py
+-rw-r--r--   0 zongheng   (502) staff       (20)    19443 2023-06-01 22:29:03.000000 skypilot-0.3.1/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4663 2023-04-19 13:26:02.000000 skypilot-0.3.1/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 zongheng   (502) staff       (20)       94 2022-02-17 10:51:09.000000 skypilot-0.3.1/tests/test_pycryptodome_version.py
+-rw-r--r--   0 zongheng   (502) staff       (20)   101322 2023-06-04 15:57:37.000000 skypilot-0.3.1/tests/test_smoke.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     7206 2023-04-03 17:20:30.000000 skypilot-0.3.1/tests/test_spot.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     4048 2023-06-01 22:22:35.000000 skypilot-0.3.1/tests/test_storage.py
+-rw-r--r--   0 zongheng   (502) staff       (20)     1070 2023-01-09 22:00:08.000000 skypilot-0.3.1/tests/test_wheels.py
```

### Comparing `skypilot-0.3.0/LICENSE` & `skypilot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/PKG-INFO` & `skypilot-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot
-Version: 0.3.0
+Version: 0.3.1
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
@@ -57,29 +57,29 @@
 - [March, 2023] **[Vicuna LLM chatbot](https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./llm/vicuna/) **for $300 on spot instances!** 
 - [March, 2023] *Serve* your own LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama)
 ----
 
 SkyPilot is a framework for easily and cost effectively running ML workloads<sup>[1]</sup> on any cloud. 
 
 SkyPilot abstracts away the cloud infra burden:
-- Launch jobs & clusters on any cloud (AWS, Azure, GCP, Lambda Cloud)
+- Launch jobs & clusters on any cloud (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung)
 - Find scarce resources across zones/regions/clouds
 - Queue jobs & use cloud object stores
 
 SkyPilot cuts your cloud costs:
 * [Managed Spot](https://skypilot.readthedocs.io/en/latest/examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-recovery from preemptions
 * [Autostop](https://skypilot.readthedocs.io/en/latest/reference/auto-stop.html): hands-free cleanup of idle clusters 
 * [Benchmark](https://skypilot.readthedocs.io/en/latest/reference/benchmark/index.html): find best VM types for your jobs
 * Optimizer: **2x cost savings** by auto-picking best prices across zones/regions/clouds
 
 SkyPilot supports your existing GPU, TPU, and CPU workloads, with no code changes. 
 
-Install with pip (choose your clouds) or [from source](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html):
+Install with pip or [from source](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html):
 ```
-pip install "skypilot[aws,gcp,azure,lambda]"
+pip install "skypilot[aws,gcp,azure,lambda,ibm,scp]"  # choose your clouds
 ```
 
 ## Getting Started
 You can find our documentation [here](https://skypilot.readthedocs.io/en/latest/).
 - [Installation](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html)
 - [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/quickstart.html)
 - [CLI reference](https://skypilot.readthedocs.io/en/latest/reference/cli.html)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot Version: 0.3.0 Summary: SkyPilot: An
+Metadata-Version: 2.1 Name: skypilot Version: 0.3.1 Summary: SkyPilot: An
 intercloud broker for the clouds Author: SkyPilot Team License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot Project-URL:
 Issues, https://github.com/skypilot-org/skypilot/issues Project-URL:
 Discussion, https://github.com/skypilot-org/skypilot/discussions Project-URL:
 Documentation, https://skypilot.readthedocs.io/en/latest/ Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -21,53 +21,53 @@
 Vicuna model with a single command**! - [March, 2023] **[Vicuna LLM chatbot]
 (https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./
 llm/vicuna/) **for $300 on spot instances!** - [March, 2023] *Serve* your own
 LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-
 chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama) ---- SkyPilot
 is a framework for easily and cost effectively running ML workloads[1] on any
 cloud. SkyPilot abstracts away the cloud infra burden: - Launch jobs & clusters
-on any cloud (AWS, Azure, GCP, Lambda Cloud) - Find scarce resources across
-zones/regions/clouds - Queue jobs & use cloud object stores SkyPilot cuts your
-cloud costs: * [Managed Spot](https://skypilot.readthedocs.io/en/latest/
-examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-
-recovery from preemptions * [Autostop](https://skypilot.readthedocs.io/en/
-latest/reference/auto-stop.html): hands-free cleanup of idle clusters *
-[Benchmark](https://skypilot.readthedocs.io/en/latest/reference/benchmark/
-index.html): find best VM types for your jobs * Optimizer: **2x cost savings**
-by auto-picking best prices across zones/regions/clouds SkyPilot supports your
-existing GPU, TPU, and CPU workloads, with no code changes. Install with pip
-(choose your clouds) or [from source](https://skypilot.readthedocs.io/en/
+on any cloud (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung) - Find scarce
+resources across zones/regions/clouds - Queue jobs & use cloud object stores
+SkyPilot cuts your cloud costs: * [Managed Spot](https://
+skypilot.readthedocs.io/en/latest/examples/spot-jobs.html): **3x cost savings**
+using spot VMs, with auto-recovery from preemptions * [Autostop](https://
+skypilot.readthedocs.io/en/latest/reference/auto-stop.html): hands-free cleanup
+of idle clusters * [Benchmark](https://skypilot.readthedocs.io/en/latest/
+reference/benchmark/index.html): find best VM types for your jobs * Optimizer:
+**2x cost savings** by auto-picking best prices across zones/regions/clouds
+SkyPilot supports your existing GPU, TPU, and CPU workloads, with no code
+changes. Install with pip or [from source](https://skypilot.readthedocs.io/en/
 latest/getting-started/installation.html): ``` pip install "skypilot
-[aws,gcp,azure,lambda]" ``` ## Getting Started You can find our documentation
-[here](https://skypilot.readthedocs.io/en/latest/). - [Installation](https://
-skypilot.readthedocs.io/en/latest/getting-started/installation.html) -
-[Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/
-quickstart.html) - [CLI reference](https://skypilot.readthedocs.io/en/latest/
-reference/cli.html) ## SkyPilot in 1 minute A SkyPilot task specifies: resource
-requirements, data to be synced, setup commands, and the task commands. Once
-written in this [**unified interface**](https://skypilot.readthedocs.io/en/
-latest/reference/yaml-spec.html) (YAML or Python API), the task can be launched
-on any available cloud. This avoids vendor lock-in, and allows easily moving
-jobs to a different provider. Paste the following into a file `my_task.yaml`:
-```yaml resources: accelerators: V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 #
-Number of VMs to launch # Working directory (optional) containing the project
-codebase. # Its contents are synced to ~/sky_workdir/ on the cluster. workdir:
-~/torch_examples # Commands to be run before executing the job. # Typical use:
-pip install -r requirements.txt, git clone, etc. setup: | pip install torch
-torchvision # Commands to run as a job. # Typical use: launch the main program.
-run: | cd mnist python main.py --epochs 1 ``` Prepare the workdir by cloning:
-```bash git clone https://github.com/pytorch/examples.git ~/torch_examples ```
-Launch with `sky launch` (note: [access to GPU instances](https://
-skypilot.readthedocs.io/en/latest/reference/quota.html) is needed for this
-example): ```bash sky launch my_task.yaml ``` SkyPilot then performs the heavy-
-lifting for you, including: 1. Find the lowest priced VM instance type across
-different clouds 2. Provision the VM, with auto-failover if the cloud returned
-capacity errors 3. Sync the local `workdir` to the VM 4. Run the task's `setup`
-commands to prepare the VM for running the task 5. Run the task's `run`
-commands
+[aws,gcp,azure,lambda,ibm,scp]" # choose your clouds ``` ## Getting Started You
+can find our documentation [here](https://skypilot.readthedocs.io/en/latest/).
+- [Installation](https://skypilot.readthedocs.io/en/latest/getting-started/
+installation.html) - [Quickstart](https://skypilot.readthedocs.io/en/latest/
+getting-started/quickstart.html) - [CLI reference](https://
+skypilot.readthedocs.io/en/latest/reference/cli.html) ## SkyPilot in 1 minute A
+SkyPilot task specifies: resource requirements, data to be synced, setup
+commands, and the task commands. Once written in this [**unified interface**]
+(https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html) (YAML or
+Python API), the task can be launched on any available cloud. This avoids
+vendor lock-in, and allows easily moving jobs to a different provider. Paste
+the following into a file `my_task.yaml`: ```yaml resources: accelerators:
+V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 # Number of VMs to launch # Working
+directory (optional) containing the project codebase. # Its contents are synced
+to ~/sky_workdir/ on the cluster. workdir: ~/torch_examples # Commands to be
+run before executing the job. # Typical use: pip install -r requirements.txt,
+git clone, etc. setup: | pip install torch torchvision # Commands to run as a
+job. # Typical use: launch the main program. run: | cd mnist python main.py --
+epochs 1 ``` Prepare the workdir by cloning: ```bash git clone https://
+github.com/pytorch/examples.git ~/torch_examples ``` Launch with `sky launch`
+(note: [access to GPU instances](https://skypilot.readthedocs.io/en/latest/
+reference/quota.html) is needed for this example): ```bash sky launch
+my_task.yaml ``` SkyPilot then performs the heavy-lifting for you, including:
+1. Find the lowest priced VM instance type across different clouds 2. Provision
+the VM, with auto-failover if the cloud returned capacity errors 3. Sync the
+local `workdir` to the VM 4. Run the task's `setup` commands to prepare the VM
+for running the task 5. Run the task's `run` commands
                                 [SkyPilot Demo]
 Refer to [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-
 started/quickstart.html) to get started with SkyPilot. ## Learn more -
 [Documentation](https://skypilot.readthedocs.io/en/latest/) - [Example:
 HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/
 tutorial.html) - [Tutorials](https://github.com/skypilot-org/skypilot-tutorial)
 - [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-
```

### Comparing `skypilot-0.3.0/README.md` & `skypilot-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,29 +31,29 @@
 - [March, 2023] **[Vicuna LLM chatbot](https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./llm/vicuna/) **for $300 on spot instances!** 
 - [March, 2023] *Serve* your own LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama)
 ----
 
 SkyPilot is a framework for easily and cost effectively running ML workloads[^1] on any cloud. 
 
 SkyPilot abstracts away the cloud infra burden:
-- Launch jobs & clusters on any cloud (AWS, Azure, GCP, Lambda Cloud)
+- Launch jobs & clusters on any cloud (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung)
 - Find scarce resources across zones/regions/clouds
 - Queue jobs & use cloud object stores
 
 SkyPilot cuts your cloud costs:
 * [Managed Spot](https://skypilot.readthedocs.io/en/latest/examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-recovery from preemptions
 * [Autostop](https://skypilot.readthedocs.io/en/latest/reference/auto-stop.html): hands-free cleanup of idle clusters 
 * [Benchmark](https://skypilot.readthedocs.io/en/latest/reference/benchmark/index.html): find best VM types for your jobs
 * Optimizer: **2x cost savings** by auto-picking best prices across zones/regions/clouds
 
 SkyPilot supports your existing GPU, TPU, and CPU workloads, with no code changes. 
 
-Install with pip (choose your clouds) or [from source](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html):
+Install with pip or [from source](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html):
 ```
-pip install "skypilot[aws,gcp,azure,lambda]"
+pip install "skypilot[aws,gcp,azure,lambda,ibm,scp]"  # choose your clouds
 ```
 
 ## Getting Started
 You can find our documentation [here](https://skypilot.readthedocs.io/en/latest/).
 - [Installation](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html)
 - [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/quickstart.html)
 - [CLI reference](https://skypilot.readthedocs.io/en/latest/reference/cli.html)
```

#### html2text {}

```diff
@@ -6,53 +6,53 @@
 Vicuna model with a single command**! - [March, 2023] **[Vicuna LLM chatbot]
 (https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./
 llm/vicuna/) **for $300 on spot instances!** - [March, 2023] *Serve* your own
 LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-
 chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama) ---- SkyPilot
 is a framework for easily and cost effectively running ML workloads[^1] on any
 cloud. SkyPilot abstracts away the cloud infra burden: - Launch jobs & clusters
-on any cloud (AWS, Azure, GCP, Lambda Cloud) - Find scarce resources across
-zones/regions/clouds - Queue jobs & use cloud object stores SkyPilot cuts your
-cloud costs: * [Managed Spot](https://skypilot.readthedocs.io/en/latest/
-examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-
-recovery from preemptions * [Autostop](https://skypilot.readthedocs.io/en/
-latest/reference/auto-stop.html): hands-free cleanup of idle clusters *
-[Benchmark](https://skypilot.readthedocs.io/en/latest/reference/benchmark/
-index.html): find best VM types for your jobs * Optimizer: **2x cost savings**
-by auto-picking best prices across zones/regions/clouds SkyPilot supports your
-existing GPU, TPU, and CPU workloads, with no code changes. Install with pip
-(choose your clouds) or [from source](https://skypilot.readthedocs.io/en/
+on any cloud (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung) - Find scarce
+resources across zones/regions/clouds - Queue jobs & use cloud object stores
+SkyPilot cuts your cloud costs: * [Managed Spot](https://
+skypilot.readthedocs.io/en/latest/examples/spot-jobs.html): **3x cost savings**
+using spot VMs, with auto-recovery from preemptions * [Autostop](https://
+skypilot.readthedocs.io/en/latest/reference/auto-stop.html): hands-free cleanup
+of idle clusters * [Benchmark](https://skypilot.readthedocs.io/en/latest/
+reference/benchmark/index.html): find best VM types for your jobs * Optimizer:
+**2x cost savings** by auto-picking best prices across zones/regions/clouds
+SkyPilot supports your existing GPU, TPU, and CPU workloads, with no code
+changes. Install with pip or [from source](https://skypilot.readthedocs.io/en/
 latest/getting-started/installation.html): ``` pip install "skypilot
-[aws,gcp,azure,lambda]" ``` ## Getting Started You can find our documentation
-[here](https://skypilot.readthedocs.io/en/latest/). - [Installation](https://
-skypilot.readthedocs.io/en/latest/getting-started/installation.html) -
-[Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/
-quickstart.html) - [CLI reference](https://skypilot.readthedocs.io/en/latest/
-reference/cli.html) ## SkyPilot in 1 minute A SkyPilot task specifies: resource
-requirements, data to be synced, setup commands, and the task commands. Once
-written in this [**unified interface**](https://skypilot.readthedocs.io/en/
-latest/reference/yaml-spec.html) (YAML or Python API), the task can be launched
-on any available cloud. This avoids vendor lock-in, and allows easily moving
-jobs to a different provider. Paste the following into a file `my_task.yaml`:
-```yaml resources: accelerators: V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 #
-Number of VMs to launch # Working directory (optional) containing the project
-codebase. # Its contents are synced to ~/sky_workdir/ on the cluster. workdir:
-~/torch_examples # Commands to be run before executing the job. # Typical use:
-pip install -r requirements.txt, git clone, etc. setup: | pip install torch
-torchvision # Commands to run as a job. # Typical use: launch the main program.
-run: | cd mnist python main.py --epochs 1 ``` Prepare the workdir by cloning:
-```bash git clone https://github.com/pytorch/examples.git ~/torch_examples ```
-Launch with `sky launch` (note: [access to GPU instances](https://
-skypilot.readthedocs.io/en/latest/reference/quota.html) is needed for this
-example): ```bash sky launch my_task.yaml ``` SkyPilot then performs the heavy-
-lifting for you, including: 1. Find the lowest priced VM instance type across
-different clouds 2. Provision the VM, with auto-failover if the cloud returned
-capacity errors 3. Sync the local `workdir` to the VM 4. Run the task's `setup`
-commands to prepare the VM for running the task 5. Run the task's `run`
-commands
+[aws,gcp,azure,lambda,ibm,scp]" # choose your clouds ``` ## Getting Started You
+can find our documentation [here](https://skypilot.readthedocs.io/en/latest/).
+- [Installation](https://skypilot.readthedocs.io/en/latest/getting-started/
+installation.html) - [Quickstart](https://skypilot.readthedocs.io/en/latest/
+getting-started/quickstart.html) - [CLI reference](https://
+skypilot.readthedocs.io/en/latest/reference/cli.html) ## SkyPilot in 1 minute A
+SkyPilot task specifies: resource requirements, data to be synced, setup
+commands, and the task commands. Once written in this [**unified interface**]
+(https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html) (YAML or
+Python API), the task can be launched on any available cloud. This avoids
+vendor lock-in, and allows easily moving jobs to a different provider. Paste
+the following into a file `my_task.yaml`: ```yaml resources: accelerators:
+V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 # Number of VMs to launch # Working
+directory (optional) containing the project codebase. # Its contents are synced
+to ~/sky_workdir/ on the cluster. workdir: ~/torch_examples # Commands to be
+run before executing the job. # Typical use: pip install -r requirements.txt,
+git clone, etc. setup: | pip install torch torchvision # Commands to run as a
+job. # Typical use: launch the main program. run: | cd mnist python main.py --
+epochs 1 ``` Prepare the workdir by cloning: ```bash git clone https://
+github.com/pytorch/examples.git ~/torch_examples ``` Launch with `sky launch`
+(note: [access to GPU instances](https://skypilot.readthedocs.io/en/latest/
+reference/quota.html) is needed for this example): ```bash sky launch
+my_task.yaml ``` SkyPilot then performs the heavy-lifting for you, including:
+1. Find the lowest priced VM instance type across different clouds 2. Provision
+the VM, with auto-failover if the cloud returned capacity errors 3. Sync the
+local `workdir` to the VM 4. Run the task's `setup` commands to prepare the VM
+for running the task 5. Run the task's `run` commands
                                 [SkyPilot Demo]
 Refer to [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-
 started/quickstart.html) to get started with SkyPilot. ## Learn more -
 [Documentation](https://skypilot.readthedocs.io/en/latest/) - [Example:
 HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/
 tutorial.html) - [Tutorials](https://github.com/skypilot-org/skypilot-tutorial)
 - [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-
```

### Comparing `skypilot-0.3.0/pyproject.toml` & `skypilot-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/setup.py` & `skypilot-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,16 +61,19 @@
         re.MULTILINE)
     readme = mode_re.sub(r'<img\1>', readme)
     return readme
 
 
 install_requires = [
     'wheel',
-    # NOTE: ray requires click>=7.0
-    'click>=7.0',
+    # NOTE: ray requires click>=7.0. Also, click 8.1.x makes our rendered CLI
+    # docs display weird blockquotes.
+    # TODO(zongheng): investigate how to make click 8.1.x display nicely and
+    # remove the upper bound.
+    'click<=8.0.4,>=7.0',
     # NOTE: required by awscli. To avoid ray automatically installing
     # the latest version.
     'colorama<0.4.5',
     'cryptography',
     # Jinja has a bug in older versions because of the lack of pinning
     # the version of the underlying markupsafe package. See:
     # https://github.com/pallets/jinja/issues/1585
```

### Comparing `skypilot-0.3.0/sky/__init__.py` & `skypilot-0.3.1/sky/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = '3deccb2a7360d086952601188381c28f932e118e'
-__version__ = '0.3.0'
+__commit__ = '344a70b41934265fc25a41a8b5c76350be2ca9cb'
+__version__ = '0.3.1'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-0.3.0/sky/adaptors/aws.py` & `skypilot-0.3.1/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/adaptors/azure.py` & `skypilot-0.3.1/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/adaptors/cloudflare.py` & `skypilot-0.3.1/sky/adaptors/cloudflare.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         when either of those are not set, which would hint with a
         string on unset credential.
     """
 
     hints = None
     accountid_path = os.path.expanduser(ACCOUNT_ID_PATH)
     if not r2_profile_in_aws_cred():
-        hints = f'[{R2_PROFILE_NAME}] profile is not set in {R2_CREDENTIALS_PATH}'
+        hints = f'[{R2_PROFILE_NAME}] profile is not set in {R2_CREDENTIALS_PATH}.'
     if not os.path.exists(accountid_path):
         if hints:
             hints += ' Additionally, '
         else:
             hints = ''
         hints += 'Account ID from R2 dashboard is not set.'
     if hints:
```

### Comparing `skypilot-0.3.0/sky/adaptors/docker.py` & `skypilot-0.3.1/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/adaptors/gcp.py` & `skypilot-0.3.1/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/adaptors/ibm.py` & `skypilot-0.3.1/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/authentication.py` & `skypilot-0.3.1/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/backends/backend.py` & `skypilot-0.3.1/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/backends/backend_utils.py` & `skypilot-0.3.1/sky/backends/backend_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,20 @@
 #   well as the disabling of the auto-update with apt-get.
 _RAY_YAML_KEYS_TO_RESTORE_EXCEPTIONS = [
     ('provider', 'availability_zone'),
     ('available_node_types', 'ray.head.default', 'node_config', 'UserData'),
     ('available_node_types', 'ray.worker.default', 'node_config', 'UserData'),
 ]
 
+# Command that calls `ray status` with SkyPilot's Ray port set.
+RAY_STATUS_WITH_SKY_RAY_PORT_COMMAND = (
+    'RAY_PORT=$(python -c "from sky.skylet import job_lib; '
+    'print(job_lib.get_ray_port())" 2> /dev/null || echo 6379);'
+    'RAY_ADDRESS=127.0.0.1:$RAY_PORT ray status')
+
 
 def is_ip(s: str) -> bool:
     """Returns whether this string matches IP_ADDR_REGEX."""
     return len(re.findall(IP_ADDR_REGEX, s)) == 1
 
 
 def _get_yaml_path_from_cluster_name(cluster_name: str,
@@ -855,20 +861,18 @@
         (str(cloud).lower(), 'instance_tags'), {})
     if not isinstance(instance_tags, dict):
         with ux_utils.print_exception_no_traceback():
             raise ValueError('Custom instance_tags in config.yaml should '
                              f'be a dict, but received {type(instance_tags)}.')
 
     # Dump the Ray ports to a file for Ray job submission
-    ray_port = constants.SKY_REMOTE_RAY_PORT
-    ray_dashboard_port = constants.SKY_REMOTE_RAY_DASHBOARD_PORT
-    # Note we can not use json.dumps which will add a space between ":" and its value
-    # which causes the yaml parser to fail.
-    port_dict_str = f'{{"ray_port":{ray_port}, "ray_dashboard_port":{ray_dashboard_port}}}'
-    dump_port_command = f'python -c \'import json, os; json.dump({port_dict_str}, open(os.path.expanduser("{constants.SKY_REMOTE_RAY_PORT_FILE}"), "w"))\''
+    dump_port_command = (
+        f'python -c \'import json, os; json.dump({constants.SKY_REMOTE_RAY_PORT_DICT_STR}, '
+        f'open(os.path.expanduser("{constants.SKY_REMOTE_RAY_PORT_FILE}"), "w"))\''
+    )
 
     # Use a tmp file path to avoid incomplete YAML file being re-used in the
     # future.
     tmp_yaml_path = yaml_path + '.tmp'
     fill_template(
         cluster_config_template,
         dict(
@@ -906,16 +910,16 @@
                 'resource_group': f'{cluster_name}-{region_name}',
 
                 # GCP only:
                 'gcp_project_id': gcp_project_id,
 
                 # Port of Ray (GCS server).
                 # Ray's default port 6379 is conflicted with Redis.
-                'ray_port': ray_port,
-                'ray_dashboard_port': ray_dashboard_port,
+                'ray_port': constants.SKY_REMOTE_RAY_PORT,
+                'ray_dashboard_port': constants.SKY_REMOTE_RAY_DASHBOARD_PORT,
                 'ray_temp_dir': constants.SKY_REMOTE_RAY_TEMPDIR,
                 'dump_port_command': dump_port_command,
                 # Ray version.
                 'ray_version': constants.SKY_REMOTE_RAY_VERSION,
                 # Cloud credentials for cloud storage.
                 'credentials': credentials,
                 # Sky remote utils.
@@ -1102,19 +1106,20 @@
     ssh_credentials = ssh_credential_from_yaml(cluster_config_file)
     last_nodes_so_far = 0
     start = time.time()
     runner = command_runner.SSHCommandRunner(head_ip, **ssh_credentials)
     with log_utils.console.status(
             '[bold cyan]Waiting for workers...') as worker_status:
         while True:
-            rc, output, stderr = runner.run('ray status',
-                                            log_path=log_path,
-                                            stream_logs=False,
-                                            require_outputs=True,
-                                            separate_stderr=True)
+            rc, output, stderr = runner.run(
+                RAY_STATUS_WITH_SKY_RAY_PORT_COMMAND,
+                log_path=log_path,
+                stream_logs=False,
+                require_outputs=True,
+                separate_stderr=True)
             subprocess_utils.handle_returncode(
                 rc, 'ray status', 'Failed to run ray status on head node.',
                 stderr)
             logger.debug(output)
 
             ready_head, ready_workers = _count_healthy_nodes_from_ray(
                 output, is_local_cloud=is_local_cloud)
@@ -1934,15 +1939,15 @@
         if external_ips is None or len(external_ips) == 0:
             raise exceptions.FetchIPError(
                 reason=exceptions.FetchIPError.Reason.HEAD)
         # Check if ray cluster status is healthy.
         ssh_credentials = ssh_credential_from_yaml(handle.cluster_yaml)
         runner = command_runner.SSHCommandRunner(external_ips[0],
                                                  **ssh_credentials)
-        rc, output, _ = runner.run('ray status',
+        rc, output, _ = runner.run(RAY_STATUS_WITH_SKY_RAY_PORT_COMMAND,
                                    stream_logs=False,
                                    require_outputs=True,
                                    separate_stderr=True)
         if rc:
             raise exceptions.FetchIPError(
                 reason=exceptions.FetchIPError.Reason.HEAD)
 
@@ -2283,37 +2288,40 @@
                 f'{backends.CloudVmRayBackend.NAME}.'
                 f'{reset}')
     if cluster_status != global_user_state.ClusterStatus.UP:
         if onprem_utils.check_if_local_cloud(cluster_name):
             raise exceptions.ClusterNotUpError(
                 constants.UNINITIALIZED_ONPREM_CLUSTER_MESSAGE.format(
                     cluster_name),
-                cluster_status=cluster_status)
+                cluster_status=cluster_status,
+                handle=handle)
         with ux_utils.print_exception_no_traceback():
             hint_for_init = ''
             if cluster_status == global_user_state.ClusterStatus.INIT:
                 hint_for_init = (
                     f'{reset} Wait for a launch to finish, or use this command '
                     f'to try to transition the cluster to UP: {bright}sky '
                     f'start {cluster_name}{reset}')
             raise exceptions.ClusterNotUpError(
                 f'{colorama.Fore.YELLOW}{operation.capitalize()}: skipped for '
                 f'cluster {cluster_name!r} (status: {cluster_status.value}). '
                 'It is only allowed for '
                 f'{global_user_state.ClusterStatus.UP.value} clusters.'
                 f'{hint_for_init}'
                 f'{reset}',
-                cluster_status=cluster_status)
+                cluster_status=cluster_status,
+                handle=handle)
 
     if handle.head_ip is None:
         with ux_utils.print_exception_no_traceback():
             raise exceptions.ClusterNotUpError(
                 f'Cluster {cluster_name!r} has been stopped or not properly '
                 'set up. Please re-launch it with `sky start`.',
-                cluster_status=cluster_status)
+                cluster_status=cluster_status,
+                handle=handle)
     return handle
 
 
 class CloudFilter(enum.Enum):
     # Filter for all types of clouds.
     ALL = 'all'
     # Filter for Sky's main clouds (aws, gcp, azure, docker).
```

### Comparing `skypilot-0.3.0/sky/backends/cloud_vm_ray_backend.py` & `skypilot-0.3.1/sky/backends/cloud_vm_ray_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1205,15 +1205,15 @@
     ):
         """The provision retry loop."""
         style = colorama.Style
         fore = colorama.Fore
         # Get log_path name
         log_path = os.path.join(self.log_dir, 'provision.log')
         log_abs_path = os.path.abspath(log_path)
-        os.makedirs(self.log_dir, exist_ok=True)
+        os.makedirs(os.path.expanduser(self.log_dir), exist_ok=True)
         os.system(f'touch {log_path}')
         tail_cmd = f'tail -n100 -f {log_path}'
         logger.info('To view detailed progress: '
                     f'{style.BRIGHT}{tail_cmd}{style.RESET_ALL}')
 
         # Get previous cluster status
         cluster_exists = prev_cluster_status is not None
@@ -1714,15 +1714,15 @@
             #   - for all nodes: ray stop
             #   - ray up --restart-only
             return
         backend = CloudVmRayBackend()
 
         returncode = backend.run_on_head(
             handle,
-            'ray status',
+            backend_utils.RAY_STATUS_WITH_SKY_RAY_PORT_COMMAND,
             # At this state, an erroneous cluster may not have cached
             # handle.head_ip (global_user_state.add_or_update_cluster(...,
             # ready=True)).
             use_cached_head_ip=False)
         if returncode == 0:
             return
         launched_resources = handle.launched_resources
@@ -2114,14 +2114,16 @@
     NAME = 'cloudvmray'
 
     # Backward compatibility, with the old name of the handle.
     ResourceHandle = CloudVmRayResourceHandle  # pylint: disable=invalid-name
 
     def __init__(self):
         self.run_timestamp = backend_utils.get_run_timestamp()
+        # NOTE: do not expanduser() here, as this '~/...' path is used for
+        # remote as well to be expanded on the remote side.
         self.log_dir = os.path.join(constants.SKY_LOGS_DIRECTORY,
                                     self.run_timestamp)
         # Do not make directories to avoid create folder for commands that
         # do not need it (`sky status`, `sky logs` ...)
         # os.makedirs(self.log_dir, exist_ok=True)
 
         self._dag = None
@@ -2510,15 +2512,15 @@
         num_nodes = handle.launched_nodes
         plural = 's' if num_nodes > 1 else ''
         logger.info(
             f'{fore.CYAN}Syncing workdir (to {num_nodes} node{plural}): '
             f'{style.BRIGHT}{workdir}{style.RESET_ALL}'
             f' -> '
             f'{style.BRIGHT}{SKY_REMOTE_WORKDIR}{style.RESET_ALL}')
-        os.makedirs(self.log_dir, exist_ok=True)
+        os.makedirs(os.path.expanduser(self.log_dir), exist_ok=True)
         os.system(f'touch {log_path}')
         tail_cmd = f'tail -n100 -f {log_path}'
         logger.info('To view detailed progress: '
                     f'{style.BRIGHT}{tail_cmd}{style.RESET_ALL}')
         with log_utils.safe_rich_status('[bold cyan]Syncing[/]'):
             subprocess_utils.run_in_parallel(_sync_workdir_node, runners)
 
@@ -3126,14 +3128,15 @@
             # When the cluster is not in the cluster table, we guarantee that
             # all related resources / cache / config are cleaned up, i.e. it
             # is safe to skip and return True.
             ux_utils.console_newline()
             logger.warning(
                 f'Cluster {handle.cluster_name!r} is already terminated. '
                 'Skipped.')
+            return
         log_path = os.path.join(os.path.expanduser(self.log_dir),
                                 'teardown.log')
         log_abs_path = os.path.abspath(log_path)
         cloud = handle.launched_resources.cloud
         config = common_utils.read_yaml(handle.cluster_yaml)
         cluster_name = handle.cluster_name
         use_tpu_vm = config['provider'].get('_has_tpus', False)
@@ -3522,16 +3525,18 @@
             subprocess_utils.handle_returncode(
                 returncode, cmd, 'Failed to set TPU_NAME on node.')
 
         subprocess_utils.run_in_parallel(_setup_tpu_name_on_node, runners)
 
     def _execute_file_mounts(self, handle: CloudVmRayResourceHandle,
                              file_mounts: Dict[Path, Path]):
-        """Executes file mounts - rsyncing local files and
-        copying from remote stores."""
+        """Executes file mounts.
+
+        Rsyncing local files and copying from remote stores.
+        """
         # File mounts handling for remote paths possibly without write access:
         #  (1) in 'file_mounts' sections, add <prefix> to these target paths.
         #  (2) then, create symlinks from '/.../file' to '<prefix>/.../file'.
         if file_mounts is None or not file_mounts:
             return
         symlink_commands = []
         fore = colorama.Fore
@@ -3560,15 +3565,15 @@
                         '.gitignore to exclude large files, as large sizes '
                         f'will slow down rsync. {style.RESET_ALL}')
                 if os.path.islink(full_src):
                     logger.warning(
                         f'{fore.YELLOW}Source path {src!r} is a symlink. '
                         f'Symlink contents are not uploaded.{style.RESET_ALL}')
 
-        os.makedirs(self.log_dir, exist_ok=True)
+        os.makedirs(os.path.expanduser(self.log_dir), exist_ok=True)
         os.system(f'touch {log_path}')
         tail_cmd = f'tail -n100 -f {log_path}'
         logger.info('To view detailed progress: '
                     f'{style.BRIGHT}{tail_cmd}{style.RESET_ALL}')
 
         for dst, src in file_mounts.items():
             # TODO: room for improvement.  Here there are many moving parts
```

### Comparing `skypilot-0.3.0/sky/backends/docker_utils.py` & `skypilot-0.3.1/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/backends/local_docker_backend.py` & `skypilot-0.3.1/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-0.3.1/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/backends/onprem_utils.py` & `skypilot-0.3.1/sky/backends/onprem_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
                             'P100',
                             'T4',
                             'P4',
                             'K80',
                             'A100',
                             '1080',
                             '2080',
-                            'A5000'
+                            'A5000',
                             'A6000']
         accelerators_dict = {}
         for acc in all_accelerators:
             output_str = os.popen(f'lspci | grep \\'{acc}\\'').read()
             output_lst = output_str.split('\\n')
             count = 0
             for output in output_lst:
```

### Comparing `skypilot-0.3.0/sky/backends/wheel_utils.py` & `skypilot-0.3.1/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/benchmark/benchmark_state.py` & `skypilot-0.3.1/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/benchmark/benchmark_utils.py` & `skypilot-0.3.1/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/check.py` & `skypilot-0.3.1/sky/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import click
 
 from sky import clouds
 from sky import global_user_state
 from sky.adaptors import cloudflare
 
 
+# TODO(zhwu): add check for a single cloud to improve performance
 def check(quiet: bool = False) -> None:
     echo = (lambda *_args, **_kwargs: None) if quiet else click.echo
     echo('Checking credentials to enable clouds for SkyPilot.')
 
     enabled_clouds = []
     for cloud in clouds.CLOUD_REGISTRY.values():
         if not isinstance(cloud, clouds.Local):
```

### Comparing `skypilot-0.3.0/sky/cli.py` & `skypilot-0.3.1/sky/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -3349,17 +3349,17 @@
     '--detach-run',
     '-d',
     default=False,
     is_flag=True,
     help=('If True, as soon as a job is submitted, return from this call '
           'and do not stream execution logs.'))
 @click.option(
-    '--retry-until-up',
-    '-r',
-    default=True,
+    '--retry-until-up/--no-retry-until-up',
+    '-r/-no-r',
+    default=None,
     is_flag=True,
     required=False,
     help=('(Default: True; this flag is deprecated and will be removed in a '
           'future release.) Whether to retry provisioning infinitely until the '
           'cluster is up, if unavailability errors are encountered. This '
           'applies to launching the spot clusters (both the initial and any '
           'recovery attempts), not the spot controller.'))
@@ -3425,14 +3425,26 @@
         use_spot=use_spot,
         image_id=image_id,
         env=env,
         disk_size=disk_size,
         disk_tier=disk_tier,
         spot_recovery=spot_recovery,
     )
+    # Deprecation.
+    if retry_until_up is not None:
+        flag_str = '--retry-until-up'
+        if not retry_until_up:
+            flag_str = '--no-retry-until-up'
+        click.secho(
+            f'Flag {flag_str} is deprecated and will be removed in a '
+            'future release (managed spot jobs will always be retried). '
+            'Please file an issue if this does not work for you.',
+            fg='yellow')
+    else:
+        retry_until_up = True
 
     if not yes:
         prompt = f'Launching a new spot task {name!r}. Proceed?'
         if prompt is not None:
             click.confirm(prompt, default=True, abort=True, show_default=True)
 
     # We try our best to validate the cluster name before we launch the task.
@@ -3440,22 +3452,14 @@
     # against the regex, and the cloud-specific validation will be done by
     # the spot controller when actually launching the spot cluster.
     resources = list(task.resources)[0]
     task_cloud = (resources.cloud
                   if resources.cloud is not None else clouds.Cloud)
     task_cloud.check_cluster_name_is_valid(name)
 
-    # Deprecation.
-    if not retry_until_up:
-        click.secho(
-            'Flag --retry-until-up is deprecated and will be removed in a '
-            'future release (defaults to True). Please file an issue if this '
-            'does not work for you.',
-            fg='yellow')
-
     sky.spot_launch(task,
                     name,
                     detach_run=detach_run,
                     retry_until_up=retry_until_up)
 
 
 @spot.command('queue', cls=_DocumentedCodeCommand)
```

### Comparing `skypilot-0.3.0/sky/cloud_stores.py` & `skypilot-0.3.1/sky/cloud_stores.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     """Google Cloud Storage."""
 
     # We use gsutil as a basic implementation.  One pro is that its -m
     # multi-threaded download is nice, which frees us from implementing
     # parellel workers on our end.
     # The gsutil command is part of the Google Cloud SDK, and we reuse
     # the installation logic here.
-    _GET_GSUTIL = gcp.GCLOUD_INSTALLATION_COMMAND
+    _GET_GSUTIL = gcp.GOOGLE_SDK_INSTALLATION_COMMAND
 
     _GSUTIL = ('GOOGLE_APPLICATION_CREDENTIALS='
                f'{gcp.DEFAULT_GCP_APPLICATION_CREDENTIAL_PATH} gsutil')
 
     def is_directory(self, url: str) -> bool:
         """Returns whether 'url' is a directory.
         In cloud object stores, a "directory" refers to a regular object whose
```

### Comparing `skypilot-0.3.0/sky/clouds/__init__.py` & `skypilot-0.3.1/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/aws.py` & `skypilot-0.3.1/sky/clouds/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     _regions: List[clouds.Region] = []
 
     _INDENT_PREFIX = '    '
     _STATIC_CREDENTIAL_HELP_STR = (
         'Run the following commands:'
         f'\n{_INDENT_PREFIX}  $ pip install boto3'
         f'\n{_INDENT_PREFIX}  $ aws configure'
+        f'\n{_INDENT_PREFIX}  $ aws configure list  # Ensure that this shows identity is set.'
         f'\n{_INDENT_PREFIX}For more info: '
         'https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html'  # pylint: disable=line-too-long
     )
 
     @classmethod
     def _cloud_unsupported_features(
             cls) -> Dict[clouds.CloudImplementationFeatures, str]:
@@ -563,25 +564,33 @@
             # need to identity them with each other. (There can be some cases,
             # when an IAM user is given a limited permission by the admin, we may
             # ignore that case for now, or print out a warning if the underlying
             # userid changed for a cluster).
             # 2. In the case where the multiple users belong to an organization,
             # those users will have different account id, so fallback works.
             user_ids = [user_info['UserId'], user_info['Account']]
-        except aws.botocore_exceptions().NoCredentialsError:
+        except aws.botocore_exceptions().NoCredentialsError as e:
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.CloudUserIdentityError(
-                    f'AWS credentials are not set. {cls._STATIC_CREDENTIAL_HELP_STR}'
+                    'AWS credentials are not set. '
+                    f'{cls._STATIC_CREDENTIAL_HELP_STR}\n'
+                    f'{cls._INDENT_PREFIX}Details: `aws sts '
+                    'get-caller-identity` failed with error:'
+                    f' {common_utils.format_exception(e, use_bracket=True)}.'
                 ) from None
-        except aws.botocore_exceptions().ClientError:
+        except aws.botocore_exceptions().ClientError as e:
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.CloudUserIdentityError(
                     'Failed to access AWS services with credentials. '
                     'Make sure that the access and secret keys are correct.'
-                    f' {cls._STATIC_CREDENTIAL_HELP_STR}') from None
+                    f' {cls._STATIC_CREDENTIAL_HELP_STR}\n'
+                    f'{cls._INDENT_PREFIX}Details: `aws sts '
+                    'get-caller-identity` failed with error:'
+                    f' {common_utils.format_exception(e, use_bracket=True)}.'
+                ) from None
         except aws.botocore_exceptions().InvalidConfigError as e:
             # pylint: disable=import-outside-toplevel
             import awscli
             from packaging import version
             awscli_version = version.parse(awscli.__version__)
             if (awscli_version < version.parse('1.27.10') and
                     'configured to use SSO' in str(e)):
```

### Comparing `skypilot-0.3.0/sky/clouds/azure.py` & `skypilot-0.3.1/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/cloud.py` & `skypilot-0.3.1/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/gcp.py` & `skypilot-0.3.1/sky/clouds/gcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,24 +50,24 @@
 ]
 
 _GCLOUD_INSTALLATION_LOG = '~/.sky/logs/gcloud_installation.log'
 _GCLOUD_VERSION = '424.0.0'
 # Need to be run with /bin/bash
 # We factor out the installation logic to keep it align in both spot
 # controller and cloud stores.
-GCLOUD_INSTALLATION_COMMAND = f'pushd /tmp &>/dev/null && \
-    gcloud --help > /dev/null 2>&1 || \
+GOOGLE_SDK_INSTALLATION_COMMAND = f'pushd /tmp &>/dev/null && \
+    {{ gcloud --help > /dev/null 2>&1 || \
     {{ mkdir -p {os.path.dirname(_GCLOUD_INSTALLATION_LOG)} && \
     wget --quiet https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-{_GCLOUD_VERSION}-linux-x86_64.tar.gz > {_GCLOUD_INSTALLATION_LOG} && \
     tar xzf google-cloud-sdk-{_GCLOUD_VERSION}-linux-x86_64.tar.gz >> {_GCLOUD_INSTALLATION_LOG} && \
     rm -rf ~/google-cloud-sdk >> {_GCLOUD_INSTALLATION_LOG}  && \
     mv google-cloud-sdk ~/ && \
     ~/google-cloud-sdk/install.sh -q >> {_GCLOUD_INSTALLATION_LOG} 2>&1 && \
     echo "source ~/google-cloud-sdk/path.bash.inc > /dev/null 2>&1" >> ~/.bashrc && \
-    source ~/google-cloud-sdk/path.bash.inc >> {_GCLOUD_INSTALLATION_LOG} 2>&1; }} && \
+    source ~/google-cloud-sdk/path.bash.inc >> {_GCLOUD_INSTALLATION_LOG} 2>&1; }}; }} && \
     {{ cp {GCP_CONFIG_SKY_BACKUP_PATH} {GCP_CONFIG_PATH} > /dev/null 2>&1 || true; }} && \
     popd &>/dev/null'
 
 # TODO(zhwu): Move the default AMI size to the catalog instead.
 DEFAULT_GCP_IMAGE_GB = 50
```

### Comparing `skypilot-0.3.0/sky/clouds/ibm.py` & `skypilot-0.3.1/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/lambda_cloud.py` & `skypilot-0.3.1/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/local.py` & `skypilot-0.3.1/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/__init__.py` & `skypilot-0.3.1/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-0.3.1/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-0.3.1/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/common.py` & `skypilot-0.3.1/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/config.py` & `skypilot-0.3.1/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-0.3.1/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-0.3.1/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-0.3.1/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-0.3.1/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,37 +12,40 @@
 import json
 import os
 import requests
 
 ENDPOINT = 'https://cloud.lambdalabs.com/api/v1/instance-types'
 DEFAULT_LAMBDA_KEYS_PATH = os.path.expanduser('~/.lambda_cloud/lambda_keys')
 
-# This is the list that Lambda Labs gave us.
+# List of all possible regions.
 REGIONS = [
     'australia-southeast-1',
     'europe-central-1',
     'asia-south-1',
     'me-west-1',
     'europe-south-1',
     'asia-northeast-1',
     'asia-northeast-2',
     'us-east-1',
     'us-west-2',
     'us-west-1',
     'us-south-1',
+    'us-west-3',
+    'us-midwest-1',
 ]
 
 # Source: https://lambdalabs.com/service/gpu-cloud
 GPU_TO_MEMORY = {
     'A100': 40960,
     'A100-80GB': 81920,
     'A6000': 49152,
     'A10': 24576,
     'RTX6000': 24576,
     'V100': 16384,
+    'H100': 81920,
 }
 
 
 def name_to_gpu(name: str) -> str:
     # Edge case
     if name == 'gpu_8x_a100_80gb_sxm4':
         return 'A100-80GB'
```

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-0.3.1/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files 5% similar despite different names*

```diff
@@ -328,14 +328,24 @@
     case_sensitive: bool = True,
 ) -> Dict[str, List[common.InstanceTypeInfo]]:
     """Returns all instance types in GCP offering GPUs."""
     results = common.list_accelerators_impl('GCP', _df, gpus_only, name_filter,
                                             region_filter, quantity_filter,
                                             case_sensitive)
 
+    # Remove GPUs that are unsupported by SkyPilot.
+    new_results = {}
+    for acc_name, acc_info in results.items():
+        if (acc_name.startswith('tpu') or
+                acc_name in _NUM_ACC_TO_MAX_CPU_AND_MEMORY or
+                acc_name in _A100_INSTANCE_TYPE_DICTS):
+            new_results[acc_name] = acc_info
+            new_results[acc_name] = acc_info
+    results = new_results
+
     a100_infos = results.get('A100', []) + results.get('A100-80GB', [])
     if not a100_infos:
         return results
 
     # Unlike other GPUs that can be attached to different sizes of N1 VMs,
     # A100 GPUs can only be attached to fixed-size A2 VMs.
     # Thus, we can show their exact cost including the host VM prices.
@@ -458,14 +468,15 @@
         # TODO(woosuk): Check max vCPUs and memory for each TPU type.
         assert instance_type == 'TPU-VM' or instance_type.startswith('n1-')
         return
 
     if acc_name in _A100_INSTANCE_TYPE_DICTS:
         valid_counts = list(_A100_INSTANCE_TYPE_DICTS[acc_name].keys())
     else:
+        assert acc_name in _NUM_ACC_TO_MAX_CPU_AND_MEMORY, acc_name
         valid_counts = list(_NUM_ACC_TO_MAX_CPU_AND_MEMORY[acc_name].keys())
     if acc_count not in valid_counts:
         with ux_utils.print_exception_no_traceback():
             raise exceptions.ResourcesMismatchError(
                 f'{acc_name}:{acc_count} is not launchable on GCP. '
                 f'The valid {acc_name} counts are {valid_counts}.')
```

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-0.3.1/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-0.3.1/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/config.py` & `skypilot-0.3.1/sky/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/core.py` & `skypilot-0.3.1/sky/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,21 +520,30 @@
                            f'{colorama.Style.RESET_ALL}')
     jobs = job_lib.load_job_queue(jobs_payload)
     return jobs
 
 
 @usage_lib.entrypoint
 # pylint: disable=redefined-builtin
-def cancel(cluster_name: str,
-           all: bool = False,
-           job_ids: Optional[List[int]] = None) -> None:
+def cancel(
+    cluster_name: str,
+    all: bool = False,
+    job_ids: Optional[List[int]] = None,
+    # pylint: disable=invalid-name
+    _try_cancel_if_cluster_is_init: bool = False,
+) -> None:
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
     """Cancel jobs on a cluster.
 
     Please refer to the sky.cli.cancel for the document.
+    Additional arguments:
+        _try_cancel_if_cluster_is_init: (bool) whether to try cancelling the job
+            even if the cluster is not UP, but the head node is still alive.
+            This is used by the spot controller to cancel the job when the
+            worker node is preempted in the spot cluster.
 
     Raises:
         ValueError: if arguments are invalid, or the cluster does not exist.
         sky.exceptions.ClusterNotUpError: if the cluster is not UP.
         sky.exceptions.NotSupportedError: if the specified cluster is a
           reserved cluster that does not support this operation.
         sky.exceptions.ClusterOwnerIdentityMismatchError: if the current user is
@@ -547,18 +556,31 @@
             'sky cancel requires either a job id '
             f'(see `sky queue {cluster_name} -s`) or the --all flag.')
 
     backend_utils.check_cluster_name_not_reserved(
         cluster_name, operation_str='Cancelling jobs')
 
     # Check the status of the cluster.
-    handle = backend_utils.check_cluster_available(
-        cluster_name,
-        operation='cancelling jobs',
-    )
+    try:
+        handle = backend_utils.check_cluster_available(
+            cluster_name,
+            operation='cancelling jobs',
+        )
+    except exceptions.ClusterNotUpError as e:
+        if not _try_cancel_if_cluster_is_init:
+            raise
+        assert (e.handle is None or
+                isinstance(e.handle, backends.CloudVmRayResourceHandle)), e
+        if (e.handle is None or e.handle.head_ip is None):
+            raise
+        # Even if the cluster is not UP, we can still try to cancel the job if
+        # the head node is still alive. This is useful when a spot cluster's
+        # worker node is preempted, but we can still cancel the job on the head
+        # node.
+
     backend = backend_utils.get_backend_from_handle(handle)
 
     if all:
         sky_logging.print(f'{colorama.Fore.YELLOW}'
                           f'Cancelling all jobs on cluster {cluster_name!r}...'
                           f'{colorama.Style.RESET_ALL}')
         job_ids = None
```

### Comparing `skypilot-0.3.0/sky/dag.py` & `skypilot-0.3.1/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/data/data_transfer.py` & `skypilot-0.3.1/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/data/data_utils.py` & `skypilot-0.3.1/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/data/mounting_utils.py` & `skypilot-0.3.1/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/data/storage.py` & `skypilot-0.3.1/sky/data/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import time
 import typing
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 import urllib.parse
 
 import colorama
 
+from sky import check
 from sky import clouds
 from sky.adaptors import aws
 from sky.adaptors import gcp
 from sky.adaptors import cloudflare
 from sky.backends import backend_utils
 from sky.utils import schemas
 from sky.data import data_transfer
@@ -56,14 +57,27 @@
     'your cloud credentials have access to it.')
 
 _BUCKET_EXTERNALLY_DELETED_DEBUG_MESSAGE = (
     'Bucket {bucket_name!r} does not exist. '
     'It may have been deleted externally.')
 
 
+def _is_storage_cloud_enabled(cloud_name: str,
+                              try_fix_with_sky_check: bool = True) -> bool:
+    enabled_storage_clouds = global_user_state.get_enabled_storage_clouds()
+    if cloud_name in enabled_storage_clouds:
+        return True
+    if try_fix_with_sky_check:
+        # TODO(zhwu): Only check the specified cloud to speed up.
+        check.check(quiet=True)
+        return _is_storage_cloud_enabled(cloud_name,
+                                         try_fix_with_sky_check=False)
+    return False
+
+
 class StoreType(enum.Enum):
     """Enum for the different types of stores."""
     S3 = 'S3'
     GCS = 'GCS'
     AZURE = 'AZURE'
     R2 = 'R2'
 
@@ -911,16 +925,15 @@
                 assert data_utils.verify_r2_bucket(self.name), (
                     f'Source specified as {self.source}, a R2 bucket. ',
                     'R2 Bucket should exist.')
         # Validate name
         self.name = self.validate_name(self.name)
 
         # Check if the storage is enabled
-        enabled_storage_clouds = global_user_state.get_enabled_storage_clouds()
-        if str(clouds.AWS()) not in enabled_storage_clouds:
+        if not _is_storage_cloud_enabled(str(clouds.AWS())):
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesUnavailableError(
                     'Storage \'store: s3\' specified, but ' \
                     'AWS access is disabled. To fix, enable '\
                     'AWS by running `sky check`. More info: '\
                     'https://skypilot.readthedocs.io/en/latest/getting-started/installation.html.' # pylint: disable=line-too-long
                     )
@@ -1297,16 +1310,15 @@
                            'the same as R2 bucket.')
                     assert data_utils.verify_r2_bucket(self.name), (
                         f'Source specified as {self.source}, a R2 bucket. ',
                         'R2 Bucket should exist.')
         # Validate name
         self.name = self.validate_name(self.name)
         # Check if the storage is enabled
-        enabled_storage_clouds = global_user_state.get_enabled_storage_clouds()
-        if str(clouds.GCP()) not in enabled_storage_clouds:
+        if not _is_storage_cloud_enabled(str(clouds.GCP())):
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesUnavailableError(
                     'Storage \'store: gcs\' specified, but ' \
                     'GCP access is disabled. To fix, enable '\
                     'GCP by running `sky check`. '\
                     'More info: https://skypilot.readthedocs.io/en/latest/getting-started/installation.html.' # pylint: disable=line-too-long
                     )
@@ -1711,16 +1723,15 @@
             elif self.source.startswith('r2://'):
                 assert self.name == data_utils.split_r2_path(self.source)[0], (
                     'R2 Bucket is specified as path, the name should be '
                     'the same as R2 bucket.')
         # Validate name
         self.name = S3Store.validate_name(self.name)
         # Check if the storage is enabled
-        enabled_storage_clouds = global_user_state.get_enabled_storage_clouds()
-        if cloudflare.NAME not in enabled_storage_clouds:
+        if not _is_storage_cloud_enabled(cloudflare.NAME):
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesUnavailableError(
                     'Storage \'store: r2\' specified, but ' \
                     'Cloudflare R2 access is disabled. To fix, '\
                     'enable Cloudflare R2 by running `sky check`. '\
                     'More info: https://skypilot.readthedocs.io/en/latest/getting-started/installation.html.'  # pylint: disable=line-too-long
                     )
```

### Comparing `skypilot-0.3.0/sky/data/storage_utils.py` & `skypilot-0.3.1/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/exceptions.py` & `skypilot-0.3.1/sky/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Exceptions."""
 import enum
 import typing
 from typing import List, Optional
 
 if typing.TYPE_CHECKING:
     from sky import global_user_state
+    from sky.backends import backend
 
 # Return code for keyboard interruption and SIGTSTP
 KEYBOARD_INTERRUPT_CODE = 130
 SIGTSTP_CODE = 146
 RSYNC_FILE_NOT_FOUND_CODE = 23
 # Arbitrarily chosen value. Used in SkyPilot's storage mounting scripts
 MOUNT_PATH_NON_EMPTY_CODE = 42
@@ -90,20 +91,21 @@
                    f'\n{error_msg}')
         super().__init__(message)
 
 
 class ClusterNotUpError(Exception):
     """Raised when a cluster is not up."""
 
-    def __init__(
-            self, message: str,
-            cluster_status: Optional['global_user_state.ClusterStatus']
-    ) -> None:
+    def __init__(self,
+                 message: str,
+                 cluster_status: Optional['global_user_state.ClusterStatus'],
+                 handle: Optional['backend.ResourceHandle'] = None) -> None:
         super().__init__(message)
         self.cluster_status = cluster_status
+        self.handle = handle
 
 
 class ClusterSetUpError(Exception):
     """Raised when a cluster has setup error."""
     pass
```

### Comparing `skypilot-0.3.0/sky/execution.py` & `skypilot-0.3.1/sky/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,21 +590,24 @@
             'remote_user_yaml_prefix': spot.SPOT_TASK_YAML_PREFIX,
             'user_yaml_path': f.name,
             'user_config_path': None,
             'spot_controller': controller_name,
             # Note: actual spot cluster name will be <task_name>-<spot job ID>
             'task_name': name,
             'uuid': task_uuid,
-            'gcloud_installation_commands': gcp.GCLOUD_INSTALLATION_COMMAND,
+            'google_sdk_installation_commands':
+                gcp.GOOGLE_SDK_INSTALLATION_COMMAND,
             'is_dev': env_options.Options.IS_DEVELOPER.get(),
             'is_debug': env_options.Options.SHOW_DEBUG_INFO.get(),
             'disable_logging': env_options.Options.DISABLE_LOGGING.get(),
             'logging_user_hash': common_utils.get_user_hash(),
             'retry_until_up': retry_until_up,
-            'user': os.environ.get('USER', None),
+            # Should not use $USER here, as that env var can be empty when
+            # running in a container.
+            'user': getpass.getuser(),
         }
         if skypilot_config.loaded():
             # Look up the contents of the already loaded configs via the
             # 'skypilot_config' module. Don't simply read the on-disk file as
             # it may have changed since this process started.
             #
             # Set any proxy command to None, because the controller would've
@@ -632,14 +635,15 @@
             # is not set up), but it may catch some obvious errors.
             # TODO(zhwu): hacky. We should only set the proxy command of the
             # cloud where the controller is launched (currently, only aws user
             # uses proxy_command).
             proxy_command_key = ('aws', 'ssh_proxy_command')
             ssh_proxy_command = skypilot_config.get_nested(
                 proxy_command_key, None)
+            config_dict = skypilot_config.to_dict()
             if isinstance(ssh_proxy_command, str):
                 config_dict = skypilot_config.set_nested(
                     proxy_command_key, None)
             elif isinstance(ssh_proxy_command, dict):
                 # Instead of removing the key, we set the value to empty string
                 # so that the controller will only try the regions specified by
                 # the keys.
```

### Comparing `skypilot-0.3.0/sky/global_user_state.py` & `skypilot-0.3.1/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/optimizer.py` & `skypilot-0.3.1/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/resources.py` & `skypilot-0.3.1/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/setup_files/setup.py` & `skypilot-0.3.1/sky/setup_files/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,16 +61,19 @@
         re.MULTILINE)
     readme = mode_re.sub(r'<img\1>', readme)
     return readme
 
 
 install_requires = [
     'wheel',
-    # NOTE: ray requires click>=7.0
-    'click>=7.0',
+    # NOTE: ray requires click>=7.0. Also, click 8.1.x makes our rendered CLI
+    # docs display weird blockquotes.
+    # TODO(zongheng): investigate how to make click 8.1.x display nicely and
+    # remove the upper bound.
+    'click<=8.0.4,>=7.0',
     # NOTE: required by awscli. To avoid ray automatically installing
     # the latest version.
     'colorama<0.4.5',
     'cryptography',
     # Jinja has a bug in older versions because of the lack of pinning
     # the version of the underlying markupsafe package. See:
     # https://github.com/pallets/jinja/issues/1585
```

### Comparing `skypilot-0.3.0/sky/sky_logging.py` & `skypilot-0.3.1/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/LICENSE` & `skypilot-0.3.1/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/autostop_lib.py` & `skypilot-0.3.1/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/configs.py` & `skypilot-0.3.1/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/events.py` & `skypilot-0.3.1/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/job_lib.py` & `skypilot-0.3.1/sky/skylet/job_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,15 +318,33 @@
     rows = _CURSOR.execute(f'SELECT {field} FROM jobs WHERE job_id=(?)',
                            (job_id,))
     for (timestamp,) in rows:
         return common_utils.encode_payload(timestamp)
     return common_utils.encode_payload(None)
 
 
+def get_ray_port():
+    """Get the port Skypilot-internal Ray cluster uses.
+
+    If the port file does not exist, the cluster was launched before #1790,
+    return the default port.
+    """
+    port_path = os.path.expanduser(constants.SKY_REMOTE_RAY_PORT_FILE)
+    if not os.path.exists(port_path):
+        return 6379
+    port = json.load(open(port_path))['ray_port']
+    return port
+
+
 def get_job_submission_port():
+    """Get the dashboard port Skypilot-internal Ray cluster uses.
+
+    If the port file does not exist, the cluster was launched before #1790,
+    return the default port.
+    """
     port_path = os.path.expanduser(constants.SKY_REMOTE_RAY_PORT_FILE)
     if not os.path.exists(port_path):
         return 8265
     port = json.load(open(port_path))['ray_dashboard_port']
     return port
```

### Comparing `skypilot-0.3.0/sky/skylet/log_lib.py` & `skypilot-0.3.1/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-0.3.1/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/aws/config.py` & `skypilot-0.3.1/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/aws/node_provider.py` & `skypilot-0.3.1/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/aws/utils.py` & `skypilot-0.3.1/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-0.3.1/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-0.3.1/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/azure/config.py` & `skypilot-0.3.1/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/azure/node_provider.py` & `skypilot-0.3.1/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/gcp/config.py` & `skypilot-0.3.1/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/gcp/constants.py` & `skypilot-0.3.1/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/gcp/node.py` & `skypilot-0.3.1/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/gcp/node_provider.py` & `skypilot-0.3.1/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/ibm/node_provider.py` & `skypilot-0.3.1/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/ibm/utils.py` & `skypilot-0.3.1/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-0.3.1/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-0.3.1/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-0.3.1/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/ray_patches/__init__.py` & `skypilot-0.3.1/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-0.3.1/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-0.3.1/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/ray_patches/worker.py.patch` & `skypilot-0.3.1/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/skylet.py` & `skypilot-0.3.1/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skylet/subprocess_daemon.py` & `skypilot-0.3.1/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/skypilot_config.py` & `skypilot-0.3.1/sky/skypilot_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,22 @@
             prev_value = prev[key]
             prev[key] = value
             logger.debug(f'Set the value of {keys} to {value} (previous: '
                          f'{prev_value}). Returning conf: {to_return}')
     return to_return
 
 
+def to_dict() -> Dict[str, Any]:
+    """Returns a deep-copied version of the current config."""
+    global _dict
+    if _dict is not None:
+        return copy.deepcopy(_dict)
+    return {}
+
+
 def _syntax_check_for_ssh_proxy_command(cloud: str) -> None:
     ssh_proxy_command_config = get_nested((cloud.lower(), 'ssh_proxy_command'),
                                           None)
     if ssh_proxy_command_config is None or isinstance(ssh_proxy_command_config,
                                                       str):
         return
```

### Comparing `skypilot-0.3.0/sky/spot/__init__.py` & `skypilot-0.3.1/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/spot/constants.py` & `skypilot-0.3.1/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/spot/controller.py` & `skypilot-0.3.1/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/spot/recovery_strategy.py` & `skypilot-0.3.1/sky/spot/recovery_strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,21 +126,45 @@
     def _try_cancel_all_jobs(self):
         handle = global_user_state.get_handle_from_cluster_name(
             self.cluster_name)
         if handle is None:
             return
         try:
             usage_lib.messages.usage.set_internal()
-            sky.cancel(cluster_name=self.cluster_name, all=True)
+            # Note that `sky.cancel()` may not go through for a variety of
+            # reasons:
+            # (1) head node is preempted; or
+            # (2) somehow user programs escape the cancel codepath's kill.
+            # The latter is silent and is a TODO.
+            #
+            # For the former, an exception will be thrown, in which case we
+            # fallback to terminate_cluster() in the except block below. This
+            # is because in the event of recovery on the same set of remaining
+            # worker nodes, we don't want to leave some old job processes
+            # running.
+            # TODO(zhwu): This is non-ideal and we should figure out another way
+            # to reliably cancel those processes and not have to down the
+            # remaining nodes first.
+            #
+            # In the case where the worker node is preempted, the `sky.cancel()`
+            # should be functional with the `_try_cancel_if_cluster_is_init`
+            # flag, i.e. it sends the cancel signal to the head node, which will
+            # then kill the user process on remaining worker nodes.
+            sky.cancel(cluster_name=self.cluster_name,
+                       all=True,
+                       _try_cancel_if_cluster_is_init=True)
         except Exception as e:  # pylint: disable=broad-except
-            # Ignore the failure as the cluster can be totally stopped, and the
-            # job canceling can get connection error.
-            logger.info('Ignoring the job cancellation failure; '
-                        'the spot cluster is likely completely stopped.'
-                        f'\n  Detailed exception: {e}')
+            logger.info(
+                'Failed to cancel the job on the cluster. The cluster '
+                'might be already down or the head node is preempted.'
+                '\n  Detailed exception: '
+                f'{common_utils.format_exception(e)}\n'
+                'Terminating the cluster again to make sure there is no '
+                'remaining job on the worker nodes.')
+            terminate_cluster(self.cluster_name)
 
     def _wait_until_job_starts_on_cluster(self) -> Optional[float]:
         """Wait for MAX_JOB_CHECKING_RETRY times until job starts on the cluster
 
         Returns:
             The timestamp of when the job is submitted, or None if failed to
             submit.
```

### Comparing `skypilot-0.3.0/sky/spot/spot_state.py` & `skypilot-0.3.1/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/spot/spot_utils.py` & `skypilot-0.3.1/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/task.py` & `skypilot-0.3.1/sky/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -670,32 +670,38 @@
     def get_preferred_store_type(self) -> storage_lib.StoreType:
         # TODO(zhwu, romilb): The optimizer should look at the source and
         #  destination to figure out the right stores to use. For now, we
         #  use a heuristic solution to find the store type by the following
         #  order:
         #  1. cloud decided in best_resources.
         #  2. cloud specified in the task resources.
-        #  3. the first enabled cloud.
+        #  3. if not specified or the task's cloud does not support storage,
+        #     use the first enabled storage cloud.
         # This should be refactored and moved to the optimizer.
         assert len(self.resources) == 1, self.resources
         storage_cloud = None
+
+        backend_utils.check_public_cloud_enabled()
+        enabled_storage_clouds = global_user_state.get_enabled_storage_clouds()
+        if not enabled_storage_clouds:
+            raise ValueError('No enabled cloud for storage, run: sky check')
+
         if self.best_resources is not None:
             storage_cloud = self.best_resources.cloud
         else:
             resources = list(self.resources)[0]
             storage_cloud = resources.cloud
-            if storage_cloud is None:
-                # Get the first enabled cloud.
-                backend_utils.check_public_cloud_enabled()
-                enabled_storage_clouds = \
-                    global_user_state.get_enabled_storage_clouds()
-                if enabled_storage_clouds:
-                    storage_cloud = enabled_storage_clouds[0]
+        if storage_cloud is not None:
+            if str(storage_cloud) not in enabled_storage_clouds:
+                storage_cloud = None
+
         if storage_cloud is None:
-            raise ValueError('No available cloud to mount storage.')
+            storage_cloud = clouds.CLOUD_REGISTRY.from_str(
+                enabled_storage_clouds[0])
+
         store_type = storage_lib.get_storetype_from_cloud(storage_cloud)
         return store_type
 
     def sync_storage_mounts(self) -> None:
         """(INTERNAL) Eagerly syncs storage mounts to cloud storage.
 
         After syncing up, COPY-mode storage mounts are translated into regular
```

### Comparing `skypilot-0.3.0/sky/templates/aws-ray.yml.j2` & `skypilot-0.3.1/sky/templates/aws-ray.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -204,21 +204,21 @@
 #   current num items (num SSH connections): 1
 head_start_ray_commands:
   # Start skylet daemon. (Should not place it in the head_setup_commands, otherwise it will run before sky is installed.)
   # NOTE: --disable-usage-stats in `ray start` saves 10 seconds of idle wait.
   # Line "which prlimit ..": increase the limit of the number of open files for the raylet process, as the `ulimit` may not take effect at this point, because it requires
   # all the sessions to be reloaded. This is a workaround.
   - ((ps aux | grep -v nohup | grep -v grep | grep -q -- "python3 -m sky.skylet.skylet") || nohup python3 -m sky.skylet.skylet >> ~/.sky/skylet.log 2>&1 &);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 RAY_DEDUP_LOGS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
     {{dump_port_command}};
 
 {%- if num_nodes > 1 %}
 worker_start_ray_commands:
-  - ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
+  - ray stop; RAY_SCHEDULER_EVENTS=0 RAY_DEDUP_LOGS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
 {%- else %}
 worker_start_ray_commands: []
 {%- endif %}
 
 head_node: {}
 worker_nodes: {}
```

### Comparing `skypilot-0.3.0/sky/templates/azure-ray.yml.j2` & `skypilot-0.3.1/sky/templates/azure-ray.yml.j2`

 * *Files 0% similar despite different names*

```diff
@@ -141,21 +141,21 @@
 #
 # Increment the following for catching performance bugs easier:
 #   current num items (num SSH connections): 2
 head_start_ray_commands:
   # Start skylet daemon. (Should not place it in the head_setup_commands, otherwise it will run before skypilot is installed.)
   # NOTE: --disable-usage-stats in `ray start` saves 10 seconds of idle wait.
   - ((ps aux | grep -v nohup | grep -v grep | grep -q -- "python3 -m sky.skylet.skylet") || nohup python3 -m sky.skylet.skylet >> ~/.sky/skylet.log 2>&1 &);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 RAY_DEDUP_LOGS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
     {{dump_port_command}};
 
 {%- if num_nodes > 1 %}
 worker_start_ray_commands:
-  - ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
+  - ray stop; RAY_SCHEDULER_EVENTS=0 RAY_DEDUP_LOGS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
 {%- else %}
 worker_start_ray_commands: []
 {%- endif %}
 
 head_node: {}
 worker_nodes: {}
```

### Comparing `skypilot-0.3.0/sky/templates/gcp-ray.yml.j2` & `skypilot-0.3.1/sky/templates/gcp-ray.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -188,23 +188,23 @@
 head_start_ray_commands:
   # Start skylet daemon. (Should not place it in the head_setup_commands, otherwise it will run before sky is installed.)
   # NOTE: --disable-usage-stats in `ray start` saves 10 seconds of idle wait.
   # Line "which prlimit ..": increase the limit of the number of open files for the raylet process, as the `ulimit` may not take effect at this point, because it requires
   # all the sessions to be reloaded. This is a workaround.
   - ((ps aux | grep -v nohup | grep -v grep | grep -q -- "python3 -m sky.skylet.skylet") || nohup python3 -m sky.skylet.skylet >> ~/.sky/skylet.log 2>&1 &);
     export SKYPILOT_NUM_GPUS=0 && which nvidia-smi > /dev/null && SKYPILOT_NUM_GPUS=$(nvidia-smi --query-gpu=index,name --format=csv,noheader | wc -l);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --num-gpus=$SKYPILOT_NUM_GPUS --temp-dir {{ray_temp_dir}} || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 RAY_DEDUP_LOGS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --num-gpus=$SKYPILOT_NUM_GPUS --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
     {{dump_port_command}};
 
 # Worker commands are needed for TPU VM Pods
 {%- if num_nodes > 1 or tpu_vm %}
 worker_start_ray_commands:
   - SKYPILOT_NUM_GPUS=0 && which nvidia-smi > /dev/null && SKYPILOT_NUM_GPUS=$(nvidia-smi --query-gpu=index,name --format=csv,noheader | wc -l);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --num-gpus=$SKYPILOT_NUM_GPUS --temp-dir {{ray_temp_dir}} || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 RAY_DEDUP_LOGS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --num-gpus=$SKYPILOT_NUM_GPUS --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
 {%- else %}
 worker_start_ray_commands: []
 {%- endif %}
 
 head_node: {}
 worker_nodes: {}
```

### Comparing `skypilot-0.3.0/sky/templates/ibm-ray.yml.j2` & `skypilot-0.3.1/sky/templates/ibm-ray.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -123,21 +123,21 @@
 #   current num items (num SSH connections): 1
 head_start_ray_commands:
   # Start skylet daemon. (Should not place it in the head_setup_commands, otherwise it will run before sky is installed.)
   # NOTE: --disable-usage-stats in `ray start` saves 10 seconds of idle wait.
   # Line "which prlimit ..": increase the limit of the number of open files for the raylet process, as the `ulimit` may not take effect at this point, because it requires
   # all the sessions to be reloaded. This is a workaround.
   - ((ps aux | grep -v nohup | grep -v grep | grep -q -- "python3 -m sky.skylet.skylet") || nohup python3 -m sky.skylet.skylet >> ~/.sky/skylet.log 2>&1 &);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 RAY_DEDUP_LOGS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
     {{dump_port_command}};
 
 {%- if num_nodes > 1 %}
 worker_start_ray_commands:
-  - ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
+  - ray stop; RAY_SCHEDULER_EVENTS=0 RAY_DEDUP_LOGS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
 {%- else %}
 worker_start_ray_commands: []
 {%- endif %}
 
 head_node: {}
 worker_nodes: {}
```

### Comparing `skypilot-0.3.0/sky/templates/lambda-ray.yml.j2` & `skypilot-0.3.1/sky/templates/lambda-ray.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -91,21 +91,21 @@
 # items! The same comment applies for worker_start_ray_commands.
 #
 # Increment the following for catching performance bugs easier:
 #   current num items (num SSH connections): 2
 head_start_ray_commands:
   # Start skylet daemon. (Should not place it in the head_setup_commands, otherwise it will run before skypilot is installed.)
   - ((ps aux | grep -v nohup | grep -v grep | grep -q -- "python3 -m sky.skylet.skylet") || nohup python3 -m sky.skylet.skylet >> ~/.sky/skylet.log 2>&1 &);
-    ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
+    ray stop; RAY_SCHEDULER_EVENTS=0 RAY_DEDUP_LOGS=0 ray start --disable-usage-stats --head --port={{ray_port}} --dashboard-port={{ray_dashboard_port}} --object-manager-port=8076 --autoscaling-config=~/ray_bootstrap_config.yaml {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
     {{dump_port_command}};
 
 {%- if num_nodes > 1 %}
 worker_start_ray_commands:
-  - ray stop; RAY_SCHEDULER_EVENTS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
+  - ray stop; RAY_SCHEDULER_EVENTS=0 RAY_DEDUP_LOGS=0 ray start --disable-usage-stats --address=$RAY_HEAD_IP:{{ray_port}} --object-manager-port=8076 {{"--resources='%s'" % custom_resources if custom_resources}} --temp-dir {{ray_temp_dir}} || exit 1;
     which prlimit && for id in $(pgrep -f raylet/raylet); do sudo prlimit --nofile=1048576:1048576 --pid=$id || true; done;
 {%- else %}
 worker_start_ray_commands: []
 {%- endif %}
 
 head_node: {}
 worker_nodes: {}
```

### Comparing `skypilot-0.3.0/sky/templates/local-ray.yml.j2` & `skypilot-0.3.1/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/templates/spot-controller.yaml.j2` & `skypilot-0.3.1/sky/templates/spot-controller.yaml.j2`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,24 @@
   {{remote_user_yaml_prefix}}/{{task_name}}-{{uuid}}.config_yaml: {{user_config_path}}
 {% endif %}
 
 setup: |
   # Install cli dependencies
   # Not using SkyPilot wheels because the wheel can be cleaned up by another process.
   # TODO(zhwu): Keep the dependencies align with the ones in setup.py
+  echo Check and install AWS SDK
   (pip list | grep boto3 > /dev/null 2>&1 && \
    pip list | grep google-api-python-client > /dev/null 2>&1 ) || \
    pip install boto3 awscli pycryptodome==3.12.0 google-api-python-client google-cloud-storage 2>&1 > /dev/null
 
   # We do not install azure dependencies for now since our subscription does not support spot instances.
   # pip list | grep azure-cli > /dev/null 2>&1 || \
   #  pip3 install azure-cli==2.31.0 azure-core
-
-  {{gcloud_installation_commands}}
+  echo Check and install Google SDK
+  {{google_sdk_installation_commands}}
 
   # Internal: disable logging for manually logging into the spot controller for debugging.
   {% if is_dev %}
   echo 'export SKYPILOT_DEV=1' >> ~/.bashrc
   {% endif %}
 
 run: |
```

### Comparing `skypilot-0.3.0/sky/usage/constants.py` & `skypilot-0.3.1/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/usage/usage_lib.py` & `skypilot-0.3.1/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/accelerator_registry.py` & `skypilot-0.3.1/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/cli_utils/status_utils.py` & `skypilot-0.3.1/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/command_runner.py` & `skypilot-0.3.1/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/common_utils.py` & `skypilot-0.3.1/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/db_utils.py` & `skypilot-0.3.1/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/env_options.py` & `skypilot-0.3.1/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/log_utils.py` & `skypilot-0.3.1/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/schemas.py` & `skypilot-0.3.1/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/subprocess_utils.py` & `skypilot-0.3.1/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/timeline.py` & `skypilot-0.3.1/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/tpu_utils.py` & `skypilot-0.3.1/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/ux_utils.py` & `skypilot-0.3.1/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/sky/utils/validator.py` & `skypilot-0.3.1/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/skypilot.egg-info/PKG-INFO` & `skypilot-0.3.1/skypilot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot
-Version: 0.3.0
+Version: 0.3.1
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
@@ -57,29 +57,29 @@
 - [March, 2023] **[Vicuna LLM chatbot](https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./llm/vicuna/) **for $300 on spot instances!** 
 - [March, 2023] *Serve* your own LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama)
 ----
 
 SkyPilot is a framework for easily and cost effectively running ML workloads<sup>[1]</sup> on any cloud. 
 
 SkyPilot abstracts away the cloud infra burden:
-- Launch jobs & clusters on any cloud (AWS, Azure, GCP, Lambda Cloud)
+- Launch jobs & clusters on any cloud (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung)
 - Find scarce resources across zones/regions/clouds
 - Queue jobs & use cloud object stores
 
 SkyPilot cuts your cloud costs:
 * [Managed Spot](https://skypilot.readthedocs.io/en/latest/examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-recovery from preemptions
 * [Autostop](https://skypilot.readthedocs.io/en/latest/reference/auto-stop.html): hands-free cleanup of idle clusters 
 * [Benchmark](https://skypilot.readthedocs.io/en/latest/reference/benchmark/index.html): find best VM types for your jobs
 * Optimizer: **2x cost savings** by auto-picking best prices across zones/regions/clouds
 
 SkyPilot supports your existing GPU, TPU, and CPU workloads, with no code changes. 
 
-Install with pip (choose your clouds) or [from source](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html):
+Install with pip or [from source](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html):
 ```
-pip install "skypilot[aws,gcp,azure,lambda]"
+pip install "skypilot[aws,gcp,azure,lambda,ibm,scp]"  # choose your clouds
 ```
 
 ## Getting Started
 You can find our documentation [here](https://skypilot.readthedocs.io/en/latest/).
 - [Installation](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html)
 - [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/quickstart.html)
 - [CLI reference](https://skypilot.readthedocs.io/en/latest/reference/cli.html)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot Version: 0.3.0 Summary: SkyPilot: An
+Metadata-Version: 2.1 Name: skypilot Version: 0.3.1 Summary: SkyPilot: An
 intercloud broker for the clouds Author: SkyPilot Team License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot Project-URL:
 Issues, https://github.com/skypilot-org/skypilot/issues Project-URL:
 Discussion, https://github.com/skypilot-org/skypilot/discussions Project-URL:
 Documentation, https://skypilot.readthedocs.io/en/latest/ Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -21,53 +21,53 @@
 Vicuna model with a single command**! - [March, 2023] **[Vicuna LLM chatbot]
 (https://lmsys.org/blog/2023-03-30-vicuna/) trained** [**using SkyPilot**](./
 llm/vicuna/) **for $300 on spot instances!** - [March, 2023] *Serve* your own
 LLaMA LLM chatbot (not finetuned) on any cloud: [**example**](./llm/llama-
 chatbots/), [**repo**](https://github.com/skypilot-org/sky-llama) ---- SkyPilot
 is a framework for easily and cost effectively running ML workloads[1] on any
 cloud. SkyPilot abstracts away the cloud infra burden: - Launch jobs & clusters
-on any cloud (AWS, Azure, GCP, Lambda Cloud) - Find scarce resources across
-zones/regions/clouds - Queue jobs & use cloud object stores SkyPilot cuts your
-cloud costs: * [Managed Spot](https://skypilot.readthedocs.io/en/latest/
-examples/spot-jobs.html): **3x cost savings** using spot VMs, with auto-
-recovery from preemptions * [Autostop](https://skypilot.readthedocs.io/en/
-latest/reference/auto-stop.html): hands-free cleanup of idle clusters *
-[Benchmark](https://skypilot.readthedocs.io/en/latest/reference/benchmark/
-index.html): find best VM types for your jobs * Optimizer: **2x cost savings**
-by auto-picking best prices across zones/regions/clouds SkyPilot supports your
-existing GPU, TPU, and CPU workloads, with no code changes. Install with pip
-(choose your clouds) or [from source](https://skypilot.readthedocs.io/en/
+on any cloud (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung) - Find scarce
+resources across zones/regions/clouds - Queue jobs & use cloud object stores
+SkyPilot cuts your cloud costs: * [Managed Spot](https://
+skypilot.readthedocs.io/en/latest/examples/spot-jobs.html): **3x cost savings**
+using spot VMs, with auto-recovery from preemptions * [Autostop](https://
+skypilot.readthedocs.io/en/latest/reference/auto-stop.html): hands-free cleanup
+of idle clusters * [Benchmark](https://skypilot.readthedocs.io/en/latest/
+reference/benchmark/index.html): find best VM types for your jobs * Optimizer:
+**2x cost savings** by auto-picking best prices across zones/regions/clouds
+SkyPilot supports your existing GPU, TPU, and CPU workloads, with no code
+changes. Install with pip or [from source](https://skypilot.readthedocs.io/en/
 latest/getting-started/installation.html): ``` pip install "skypilot
-[aws,gcp,azure,lambda]" ``` ## Getting Started You can find our documentation
-[here](https://skypilot.readthedocs.io/en/latest/). - [Installation](https://
-skypilot.readthedocs.io/en/latest/getting-started/installation.html) -
-[Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/
-quickstart.html) - [CLI reference](https://skypilot.readthedocs.io/en/latest/
-reference/cli.html) ## SkyPilot in 1 minute A SkyPilot task specifies: resource
-requirements, data to be synced, setup commands, and the task commands. Once
-written in this [**unified interface**](https://skypilot.readthedocs.io/en/
-latest/reference/yaml-spec.html) (YAML or Python API), the task can be launched
-on any available cloud. This avoids vendor lock-in, and allows easily moving
-jobs to a different provider. Paste the following into a file `my_task.yaml`:
-```yaml resources: accelerators: V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 #
-Number of VMs to launch # Working directory (optional) containing the project
-codebase. # Its contents are synced to ~/sky_workdir/ on the cluster. workdir:
-~/torch_examples # Commands to be run before executing the job. # Typical use:
-pip install -r requirements.txt, git clone, etc. setup: | pip install torch
-torchvision # Commands to run as a job. # Typical use: launch the main program.
-run: | cd mnist python main.py --epochs 1 ``` Prepare the workdir by cloning:
-```bash git clone https://github.com/pytorch/examples.git ~/torch_examples ```
-Launch with `sky launch` (note: [access to GPU instances](https://
-skypilot.readthedocs.io/en/latest/reference/quota.html) is needed for this
-example): ```bash sky launch my_task.yaml ``` SkyPilot then performs the heavy-
-lifting for you, including: 1. Find the lowest priced VM instance type across
-different clouds 2. Provision the VM, with auto-failover if the cloud returned
-capacity errors 3. Sync the local `workdir` to the VM 4. Run the task's `setup`
-commands to prepare the VM for running the task 5. Run the task's `run`
-commands
+[aws,gcp,azure,lambda,ibm,scp]" # choose your clouds ``` ## Getting Started You
+can find our documentation [here](https://skypilot.readthedocs.io/en/latest/).
+- [Installation](https://skypilot.readthedocs.io/en/latest/getting-started/
+installation.html) - [Quickstart](https://skypilot.readthedocs.io/en/latest/
+getting-started/quickstart.html) - [CLI reference](https://
+skypilot.readthedocs.io/en/latest/reference/cli.html) ## SkyPilot in 1 minute A
+SkyPilot task specifies: resource requirements, data to be synced, setup
+commands, and the task commands. Once written in this [**unified interface**]
+(https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html) (YAML or
+Python API), the task can be launched on any available cloud. This avoids
+vendor lock-in, and allows easily moving jobs to a different provider. Paste
+the following into a file `my_task.yaml`: ```yaml resources: accelerators:
+V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 # Number of VMs to launch # Working
+directory (optional) containing the project codebase. # Its contents are synced
+to ~/sky_workdir/ on the cluster. workdir: ~/torch_examples # Commands to be
+run before executing the job. # Typical use: pip install -r requirements.txt,
+git clone, etc. setup: | pip install torch torchvision # Commands to run as a
+job. # Typical use: launch the main program. run: | cd mnist python main.py --
+epochs 1 ``` Prepare the workdir by cloning: ```bash git clone https://
+github.com/pytorch/examples.git ~/torch_examples ``` Launch with `sky launch`
+(note: [access to GPU instances](https://skypilot.readthedocs.io/en/latest/
+reference/quota.html) is needed for this example): ```bash sky launch
+my_task.yaml ``` SkyPilot then performs the heavy-lifting for you, including:
+1. Find the lowest priced VM instance type across different clouds 2. Provision
+the VM, with auto-failover if the cloud returned capacity errors 3. Sync the
+local `workdir` to the VM 4. Run the task's `setup` commands to prepare the VM
+for running the task 5. Run the task's `run` commands
                                 [SkyPilot Demo]
 Refer to [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-
 started/quickstart.html) to get started with SkyPilot. ## Learn more -
 [Documentation](https://skypilot.readthedocs.io/en/latest/) - [Example:
 HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/
 tutorial.html) - [Tutorials](https://github.com/skypilot-org/skypilot-tutorial)
 - [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-
```

### Comparing `skypilot-0.3.0/skypilot.egg-info/SOURCES.txt` & `skypilot-0.3.1/skypilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/skypilot.egg-info/requires.txt` & `skypilot-0.3.1/skypilot.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 wheel
-click>=7.0
+click<=8.0.4,>=7.0
 colorama<0.4.5
 cryptography
 jinja2>=3.0
 jsonschema
 networkx
 oauth2client
 pandas
```

### Comparing `skypilot-0.3.0/tests/test_cli.py` & `skypilot-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/tests/test_config.py` & `skypilot-0.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/tests/test_list_accelerators.py` & `skypilot-0.3.1/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/tests/test_onprem.py` & `skypilot-0.3.1/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/tests/test_optimizer_dryruns.py` & `skypilot-0.3.1/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/tests/test_optimizer_random_dag.py` & `skypilot-0.3.1/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/tests/test_smoke.py` & `skypilot-0.3.1/tests/test_smoke.py`

 * *Files 0% similar despite different names*

```diff
@@ -1057,14 +1057,15 @@
 def test_multi_hostname(generic_cloud: str):
     name = _get_cluster_name()
     test = Test(
         'multi_hostname',
         [
             f'sky launch -y -c {name} --cloud {generic_cloud} examples/multi_hostname.yaml',
             f'sky logs {name} 1 --status',  # Ensure the job succeeded.
+            f'sky logs {name} 1 | grep "My hostname:" | wc -l | grep 2',  # Ensure there are 2 hosts.
             f'sky exec {name} examples/multi_hostname.yaml',
             f'sky logs {name} 2 --status',  # Ensure the job succeeded.
         ],
         f'sky down -y {name}',
     )
     run_one_test(test)
 
@@ -1780,14 +1781,15 @@
         f'sky down -y {name}',
         timeout=30 * 60,  # 30 mins  (it takes around ~23 mins)
     )
     run_one_test(test)
 
 
 # ---------- Testing env for disk tier ----------
+@pytest.mark.aws
 def test_aws_disk_tier():
 
     def _get_aws_query_command(region, instance_id, field, expected):
         return (f'aws ec2 describe-volumes --region {region} '
                 f'--filters Name=attachment.instance-id,Values={instance_id} '
                 f'--query Volumes[*].{field} | grep {expected} ; ')
 
@@ -1813,14 +1815,15 @@
             ],
             f'sky down -y {name}',
             timeout=10 * 60,  # 10 mins  (it takes around ~6 mins)
         )
         run_one_test(test)
 
 
+@pytest.mark.gcp
 def test_gcp_disk_tier():
     for disk_tier in ['low', 'medium', 'high']:
         type = GCP._get_disk_type(disk_tier)
         name = _get_cluster_name() + '-' + disk_tier
         region = 'us-west2'
         test = Test(
             'gcp-disk-tier',
@@ -1834,14 +1837,15 @@
             ],
             f'sky down -y {name}',
             timeout=6 * 60,  # 6 mins  (it takes around ~3 mins)
         )
         run_one_test(test)
 
 
+@pytest.mark.azure
 def test_azure_disk_tier():
     for disk_tier in ['low', 'medium']:
         type = Azure._get_disk_type(disk_tier)
         name = _get_cluster_name() + '-' + disk_tier
         region = 'westus2'
         test = Test(
             'azure-disk-tier',
@@ -1854,14 +1858,32 @@
             ],
             f'sky down -y {name}',
             timeout=20 * 60,  # 20 mins  (it takes around ~12 mins)
         )
         run_one_test(test)
 
 
+# ------- Testing user ray cluster --------
+def test_user_ray_cluster():
+    name = _get_cluster_name()
+    test = Test(
+        'user-ray-cluster',
+        [
+            f'sky launch -y -c {name} "ray start --head"',
+            f'sky exec {name} "echo hi"',
+            f'sky logs {name} 1 --status',
+            f'sky status -r | grep {name} | grep UP',
+            f'sky exec {name} "echo bye"',
+            f'sky logs {name} 2 --status',
+        ],
+        f'sky down -y {name}',
+    )
+    run_one_test(test)
+
+
 # ------- Testing the core API --------
 # Most of the core APIs have been tested in the CLI tests.
 # These tests are for testing the return value of the APIs not fully used in CLI.
 def test_core_api():
     name = _get_cluster_name()
     sky.launch
     # TODO(zhwu): Add a test for core api.
```

### Comparing `skypilot-0.3.0/tests/test_spot.py` & `skypilot-0.3.1/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/tests/test_storage.py` & `skypilot-0.3.1/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-0.3.0/tests/test_wheels.py` & `skypilot-0.3.1/tests/test_wheels.py`

 * *Files identical despite different names*

