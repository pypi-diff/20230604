# Comparing `tmp/syft-0.8.1b5.tar.gz` & `tmp/syft-0.8.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.1b5.tar", last modified: Sat Jun  3 12:39:18 2023, max compression
+gzip compressed data, was "syft-0.8.1b6.tar", last modified: Sun Jun  4 12:44:27 2023, max compression
```

## Comparing `syft-0.8.1b5.tar` & `syft-0.8.1b6.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.619018 syft-0.8.1b5/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-03 12:36:52.000000 syft-0.8.1b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-03 12:36:52.000000 syft-0.8.1b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-03 12:39:18.619018 syft-0.8.1b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-06-03 12:36:51.000000 syft-0.8.1b5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-03 12:36:52.000000 syft-0.8.1b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-03 12:39:18.623018 syft-0.8.1b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-03 12:36:52.000000 syft-0.8.1b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.547017 syft-0.8.1b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.559017 syft-0.8.1b5/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-03 12:37:07.000000 syft-0.8.1b5/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-03 12:37:07.000000 syft-0.8.1b5/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.563017 syft-0.8.1b5/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.567017 syft-0.8.1b5/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24407 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.567017 syft-0.8.1b5/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.571017 syft-0.8.1b5/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.575017 syft-0.8.1b5/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    28362 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.583017 syft-0.8.1b5/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.583017 syft-0.8.1b5/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.587017 syft-0.8.1b5/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    46765 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.587017 syft-0.8.1b5/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.591018 syft-0.8.1b5/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.591018 syft-0.8.1b5/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.591018 syft-0.8.1b5/src/syft/service/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/message/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/message/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/message/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.591018 syft-0.8.1b5/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.595018 syft-0.8.1b5/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.595018 syft-0.8.1b5/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21242 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.595018 syft-0.8.1b5/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40512 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13261 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.599018 syft-0.8.1b5/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.599018 syft-0.8.1b5/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.603018 syft-0.8.1b5/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.603018 syft-0.8.1b5/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.607018 syft-0.8.1b5/src/syft/service/vpn/
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/service/vpn/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.611018 syft-0.8.1b5/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.615018 syft-0.8.1b5/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.619018 syft-0.8.1b5/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-03 12:36:52.000000 syft-0.8.1b5/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:39:18.559017 syft-0.8.1b5/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 12:39:18.000000 syft-0.8.1b5/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.013247 syft-0.8.1b6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-04 12:42:01.000000 syft-0.8.1b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-04 12:42:01.000000 syft-0.8.1b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-04 12:44:27.013247 syft-0.8.1b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-06-04 12:42:01.000000 syft-0.8.1b6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-04 12:42:01.000000 syft-0.8.1b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-04 12:44:27.017247 syft-0.8.1b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-04 12:42:01.000000 syft-0.8.1b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.957247 syft-0.8.1b6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.965247 syft-0.8.1b6/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-04 12:42:17.000000 syft-0.8.1b6/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-04 12:42:17.000000 syft-0.8.1b6/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.969246 syft-0.8.1b6/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.973246 syft-0.8.1b6/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24407 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.973246 syft-0.8.1b6/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.977247 syft-0.8.1b6/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.981247 syft-0.8.1b6/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28362 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.985247 syft-0.8.1b6/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.985247 syft-0.8.1b6/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.989246 syft-0.8.1b6/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46765 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.993247 syft-0.8.1b6/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22127 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.993247 syft-0.8.1b6/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.993247 syft-0.8.1b6/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.997247 syft-0.8.1b6/src/syft/service/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/message/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/message/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/message/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.997247 syft-0.8.1b6/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.997247 syft-0.8.1b6/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.997247 syft-0.8.1b6/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21242 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.001247 syft-0.8.1b6/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40512 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13261 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.001247 syft-0.8.1b6/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.001247 syft-0.8.1b6/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13188 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.001247 syft-0.8.1b6/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.005246 syft-0.8.1b6/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.005246 syft-0.8.1b6/src/syft/service/vpn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/service/vpn/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.009246 syft-0.8.1b6/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.009246 syft-0.8.1b6/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:27.013247 syft-0.8.1b6/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-04 12:42:01.000000 syft-0.8.1b6/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:44:26.965247 syft-0.8.1b6/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 12:44:26.000000 syft-0.8.1b6/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.1b5/LICENSE` & `syft-0.8.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/PKG-INFO` & `syft-0.8.1b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b5
+Version: 0.8.1b6
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b5 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b6 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.1b5/README.md` & `syft-0.8.1b6/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/setup.cfg` & `syft-0.8.1b6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.1-beta.5"
+version = attr: "0.8.1-beta.6"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.1b5/src/syft/VERSION` & `syft-0.8.1b6/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.1-beta.5"
+__version__ = "0.8.1-beta.6"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.1b5/src/syft/__init__.py` & `syft-0.8.1b6/src/syft/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.1-beta.5"
+__version__ = "0.8.1-beta.6"
 
 # stdlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
```

### Comparing `syft-0.8.1b5/src/syft/abstract_node.py` & `syft-0.8.1b6/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/client/api.py` & `syft-0.8.1b6/src/syft/client/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/client/client.py` & `syft-0.8.1b6/src/syft/client/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/client/connection.py` & `syft-0.8.1b6/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/client/deploy.py` & `syft-0.8.1b6/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/client/registry.py` & `syft-0.8.1b6/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/client/search.py` & `syft-0.8.1b6/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/client/user_settings.py` & `syft-0.8.1b6/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/external/__init__.py` & `syft-0.8.1b6/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/external/oblv/__init__.py` & `syft-0.8.1b6/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/external/oblv/deployment.py` & `syft-0.8.1b6/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/external/oblv/deployment_client.py` & `syft-0.8.1b6/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/external/oblv/exceptions.py` & `syft-0.8.1b6/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.1b6/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.1b6/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/external/oblv/oblv_service.py` & `syft-0.8.1b6/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/gevent_patch.py` & `syft-0.8.1b6/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/node/credentials.py` & `syft-0.8.1b6/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/node/gateway.py` & `syft-0.8.1b6/src/syft/node/gateway.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/node/node.py` & `syft-0.8.1b6/src/syft/node/node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/node/routes.py` & `syft-0.8.1b6/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/node/run.py` & `syft-0.8.1b6/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/node/server.py` & `syft-0.8.1b6/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/node/worker_settings.py` & `syft-0.8.1b6/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/array.py` & `syft-0.8.1b6/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/arrow.py` & `syft-0.8.1b6/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/deserialize.py` & `syft-0.8.1b6/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/lib_permissions.py` & `syft-0.8.1b6/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/lib_service_registry.py` & `syft-0.8.1b6/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/mock.py` & `syft-0.8.1b6/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/recursive.py` & `syft-0.8.1b6/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/recursive_primitives.py` & `syft-0.8.1b6/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/serializable.py` & `syft-0.8.1b6/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/signature.py` & `syft-0.8.1b6/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/serde/third_party.py` & `syft-0.8.1b6/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/action_data_empty.py` & `syft-0.8.1b6/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/action_graph.py` & `syft-0.8.1b6/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/action_graph_service.py` & `syft-0.8.1b6/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/action_object.py` & `syft-0.8.1b6/src/syft/service/action/action_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/action_permissions.py` & `syft-0.8.1b6/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/action_service.py` & `syft-0.8.1b6/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/action_store.py` & `syft-0.8.1b6/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/action_types.py` & `syft-0.8.1b6/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/numpy.py` & `syft-0.8.1b6/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/pandas.py` & `syft-0.8.1b6/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/plan.py` & `syft-0.8.1b6/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/action/verification.py` & `syft-0.8.1b6/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/code/unparse.py` & `syft-0.8.1b6/src/syft/service/code/unparse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/code/user_code.py` & `syft-0.8.1b6/src/syft/service/code/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/code/user_code_parse.py` & `syft-0.8.1b6/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/code/user_code_service.py` & `syft-0.8.1b6/src/syft/service/code/user_code_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/code/user_code_stash.py` & `syft-0.8.1b6/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/context.py` & `syft-0.8.1b6/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/data_subject/data_subject.py` & `syft-0.8.1b6/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.1b6/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.1b6/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.1b6/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/dataset/dataset.py` & `syft-0.8.1b6/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/dataset/dataset_service.py` & `syft-0.8.1b6/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.1b6/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/message/message_service.py` & `syft-0.8.1b6/src/syft/service/message/message_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/message/message_stash.py` & `syft-0.8.1b6/src/syft/service/message/message_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/message/messages.py` & `syft-0.8.1b6/src/syft/service/message/messages.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/metadata/node_metadata.py` & `syft-0.8.1b6/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/network/network_service.py` & `syft-0.8.1b6/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/network/node_peer.py` & `syft-0.8.1b6/src/syft/service/network/node_peer.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/network/routes.py` & `syft-0.8.1b6/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/policy/policy.py` & `syft-0.8.1b6/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/policy/policy_service.py` & `syft-0.8.1b6/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.1b6/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/project/project.py` & `syft-0.8.1b6/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/project/project_service.py` & `syft-0.8.1b6/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/project/project_stash.py` & `syft-0.8.1b6/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/queue/base_queue.py` & `syft-0.8.1b6/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/queue/queue.py` & `syft-0.8.1b6/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/queue/queue_stash.py` & `syft-0.8.1b6/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/queue/zmq_queue.py` & `syft-0.8.1b6/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/request/request.py` & `syft-0.8.1b6/src/syft/service/request/request.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/request/request_service.py` & `syft-0.8.1b6/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/request/request_stash.py` & `syft-0.8.1b6/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/response.py` & `syft-0.8.1b6/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/service.py` & `syft-0.8.1b6/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/settings/settings.py` & `syft-0.8.1b6/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/settings/settings_service.py` & `syft-0.8.1b6/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/settings/settings_stash.py` & `syft-0.8.1b6/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/user/user.py` & `syft-0.8.1b6/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/user/user_roles.py` & `syft-0.8.1b6/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/user/user_service.py` & `syft-0.8.1b6/src/syft/service/user/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/user/user_stash.py` & `syft-0.8.1b6/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/vpn/headscale_client.py` & `syft-0.8.1b6/src/syft/service/vpn/headscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.1b6/src/syft/service/vpn/tailscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/service/vpn/vpn.py` & `syft-0.8.1b6/src/syft/service/vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/store/dict_document_store.py` & `syft-0.8.1b6/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/store/document_store.py` & `syft-0.8.1b6/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/store/kv_document_store.py` & `syft-0.8.1b6/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/store/linked_obj.py` & `syft-0.8.1b6/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/store/locks.py` & `syft-0.8.1b6/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/store/mongo_client.py` & `syft-0.8.1b6/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/store/mongo_codecs.py` & `syft-0.8.1b6/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/store/mongo_document_store.py` & `syft-0.8.1b6/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/store/sqlite_document_store.py` & `syft-0.8.1b6/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/types/datetime.py` & `syft-0.8.1b6/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/types/grid_url.py` & `syft-0.8.1b6/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/types/syft_metaclass.py` & `syft-0.8.1b6/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/types/syft_object.py` & `syft-0.8.1b6/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/types/transforms.py` & `syft-0.8.1b6/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/types/twin_object.py` & `syft-0.8.1b6/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/types/uid.py` & `syft-0.8.1b6/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/util/autoreload.py` & `syft-0.8.1b6/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/util/decorators.py` & `syft-0.8.1b6/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/util/experimental_flags.py` & `syft-0.8.1b6/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/util/filterwarnings.py` & `syft-0.8.1b6/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/util/logger.py` & `syft-0.8.1b6/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/util/schema.py` & `syft-0.8.1b6/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/util/telemetry.py` & `syft-0.8.1b6/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/util/trace_decorator.py` & `syft-0.8.1b6/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/util/util.py` & `syft-0.8.1b6/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft/util/version_compare.py` & `syft-0.8.1b6/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft.egg-info/PKG-INFO` & `syft-0.8.1b6/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b5
+Version: 0.8.1b6
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b5 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b6 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.1b5/src/syft.egg-info/SOURCES.txt` & `syft-0.8.1b6/src/syft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b5/src/syft.egg-info/requires.txt` & `syft-0.8.1b6/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

