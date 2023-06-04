# Comparing `tmp/cdktf-gke-auth-1.0.1.tar.gz` & `tmp/cdktf-gke-auth-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-gke-auth-1.0.1.tar", last modified: Sun Jun  4 00:39:19 2023, max compression
+gzip compressed data, was "cdktf-gke-auth-1.1.0.tar", last modified: Sun Jun  4 13:16:17 2023, max compression
```

## Comparing `cdktf-gke-auth-1.0.1.tar` & `cdktf-gke-auth-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:39:19.086163 cdktf-gke-auth-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-04 00:39:02.000000 cdktf-gke-auth-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-04 00:39:02.000000 cdktf-gke-auth-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-04 00:39:19.086163 cdktf-gke-auth-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-04 00:39:02.000000 cdktf-gke-auth-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-04 00:39:02.000000 cdktf-gke-auth-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 00:39:19.086163 cdktf-gke-auth-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-04 00:39:02.000000 cdktf-gke-auth-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:39:19.086163 cdktf-gke-auth-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:39:19.086163 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth/
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-06-04 00:39:02.000000 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:39:19.086163 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-04 00:39:02.000000 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-06-04 00:39:02.000000 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth/_jsii/cdktf-gke-auth@1.0.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 00:39:02.000000 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:39:19.086163 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-04 00:39:19.000000 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-04 00:39:19.000000 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 00:39:19.000000 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-04 00:39:19.000000 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 00:39:19.000000 cdktf-gke-auth-1.0.1/src/cdktf_gke_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:16:17.148796 cdktf-gke-auth-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/_jsii/cdktf-gke-auth@1.1.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-04 13:16:17.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-04 13:16:17.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:16:17.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-04 13:16:17.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 13:16:17.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/top_level.txt
```

### Comparing `cdktf-gke-auth-1.0.1/LICENSE` & `cdktf-gke-auth-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-gke-auth-1.0.1/PKG-INFO` & `cdktf-gke-auth-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-gke-auth
-Version: 1.0.1
+Version: 1.1.0
 Summary: cdktf-gke-auth
 Home-page: https://github.com/01walid/cdktf-gke-auth.git
 Author: Walid Ziouche<hi@walid.dev>
 License: Apache-2.0
 Project-URL: Source, https://github.com/01walid/cdktf-gke-auth.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -20,24 +20,28 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg" alt="Apache 2.0 License"></a>
+  <a href="https://gitpod.io/#https://github.com/01walid/cdktf-gke-auth"><img src="https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod" alt="Gitpod ready-to-code"></a>
   <a href="https://www.npmjs.com/package/cdktf-gke-auth"><img src="https://badge.fury.io/js/cdktf-gke-auth.svg" alt="npm version"></a>
+  <a href="https://pypi.org/project/cdktf-gke-auth/"><img src="https://badge.fury.io/py/cdktf-gke-auth.svg" alt="PyPI version"></a>
   <a href="https://github.com/01walid/cdktf-gke-auth/actions/workflows/build.yml"><img src="https://github.com/01walid/cdktf-gke-auth/actions/workflows/build.yml/badge.svg" alt="Build badge"></a>
   <a href="https://github.com/01walid/cdktf-gke-auth/actions/workflows/release.yml"><img src="https://github.com/01walid/cdktf-gke-auth/actions/workflows/release.yml/badge.svg" alt="Release badge"></a>
 </p>
 
 # cdktf-gke-auth
 
 Easily authenticate against a Google Kubernetes Engine (GKE) within your CDK for Terraform stack. Without the need to
 resort to [Google's terraform GKE auth](https://github.com/terraform-google-modules/terraform-google-kubernetes-engine/tree/v26.1.1/modules/auth) module. You can avoid running `cdktf get` as pre-synth step.
 
+This project uses [projen](https://github.com/projen/projen) and [jsii](https://github.com/aws/jsii) to compile the construct to Typescript, Python, Go and .Net (Java upon request).
+
 ## Example usage (Typescript)
 
 Install the construct with: `yarn install cdktf-gke-auth`.
 
 ```python
 import { GoogleProvider } from "@cdktf/provider-google/lib/provider";
 import { TerraformOutput, TerraformStack } from "cdktf";
@@ -53,21 +57,23 @@
     const auth = new GKEAuth(this, "gke-auth", {
       clusterName: "my-cluster",
       location: "europe-west1",
       projectId: "my-project",
     });
 
     // init the Kubernetes provider like so:
-    // new KubernetesProvider(this, "kubernetes", {
-    //   ...auth.authCredentials
-    // });
+    new KubernetesProvider(this, "kubernetes", {
+      ...auth.authCredentials
+    });
 
     // Or a helm provider like so:
-    //  new HelmProvider(this, "helm", {
-    //   kubernetes: auth.authCredentials,
-    // });
+     new HelmProvider(this, "helm", {
+      kubernetes: auth.authCredentials,
+    });
   }
 }
 ```
 
 The `GKEAuth` instance expose `host`, `clusterCaCertificate`, `clusterCaCertificatePEM`, and `token` you can use to authenticate using
 any of the kubernetes popular cdktf providers.
+
+For other languages examples, checkout this construct on [ConstructHub](https://constructs.dev/packages/cdktf-gke-auth/).
```

### Comparing `cdktf-gke-auth-1.0.1/README.md` & `cdktf-gke-auth-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 <p align="center">
   <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg" alt="Apache 2.0 License"></a>
+  <a href="https://gitpod.io/#https://github.com/01walid/cdktf-gke-auth"><img src="https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod" alt="Gitpod ready-to-code"></a>
   <a href="https://www.npmjs.com/package/cdktf-gke-auth"><img src="https://badge.fury.io/js/cdktf-gke-auth.svg" alt="npm version"></a>
+  <a href="https://pypi.org/project/cdktf-gke-auth/"><img src="https://badge.fury.io/py/cdktf-gke-auth.svg" alt="PyPI version"></a>
   <a href="https://github.com/01walid/cdktf-gke-auth/actions/workflows/build.yml"><img src="https://github.com/01walid/cdktf-gke-auth/actions/workflows/build.yml/badge.svg" alt="Build badge"></a>
   <a href="https://github.com/01walid/cdktf-gke-auth/actions/workflows/release.yml"><img src="https://github.com/01walid/cdktf-gke-auth/actions/workflows/release.yml/badge.svg" alt="Release badge"></a>
 </p>
 
 # cdktf-gke-auth
 
 Easily authenticate against a Google Kubernetes Engine (GKE) within your CDK for Terraform stack. Without the need to
 resort to [Google's terraform GKE auth](https://github.com/terraform-google-modules/terraform-google-kubernetes-engine/tree/v26.1.1/modules/auth) module. You can avoid running `cdktf get` as pre-synth step.
 
+This project uses [projen](https://github.com/projen/projen) and [jsii](https://github.com/aws/jsii) to compile the construct to Typescript, Python, Go and .Net (Java upon request).
+
 ## Example usage (Typescript)
 
 Install the construct with: `yarn install cdktf-gke-auth`.
 
 ```python
 import { GoogleProvider } from "@cdktf/provider-google/lib/provider";
 import { TerraformOutput, TerraformStack } from "cdktf";
@@ -29,21 +33,23 @@
     const auth = new GKEAuth(this, "gke-auth", {
       clusterName: "my-cluster",
       location: "europe-west1",
       projectId: "my-project",
     });
 
     // init the Kubernetes provider like so:
-    // new KubernetesProvider(this, "kubernetes", {
-    //   ...auth.authCredentials
-    // });
+    new KubernetesProvider(this, "kubernetes", {
+      ...auth.authCredentials
+    });
 
     // Or a helm provider like so:
-    //  new HelmProvider(this, "helm", {
-    //   kubernetes: auth.authCredentials,
-    // });
+     new HelmProvider(this, "helm", {
+      kubernetes: auth.authCredentials,
+    });
   }
 }
 ```
 
 The `GKEAuth` instance expose `host`, `clusterCaCertificate`, `clusterCaCertificatePEM`, and `token` you can use to authenticate using
 any of the kubernetes popular cdktf providers.
+
+For other languages examples, checkout this construct on [ConstructHub](https://constructs.dev/packages/cdktf-gke-auth/).
```

### Comparing `cdktf-gke-auth-1.0.1/setup.py` & `cdktf-gke-auth-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-gke-auth",
-    "version": "1.0.1",
+    "version": "1.1.0",
     "description": "cdktf-gke-auth",
     "license": "Apache-2.0",
     "url": "https://github.com/01walid/cdktf-gke-auth.git",
     "long_description_content_type": "text/markdown",
     "author": "Walid Ziouche<hi@walid.dev>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_gke_auth",
         "cdktf_gke_auth._jsii"
     ],
     "package_data": {
         "cdktf_gke_auth._jsii": [
-            "cdktf-gke-auth@1.0.1.jsii.tgz"
+            "cdktf-gke-auth@1.1.0.jsii.tgz"
         ],
         "cdktf_gke_auth": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-gke-auth-1.0.1/src/cdktf_gke_auth/__init__.py` & `cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 '''
 <p align="center">
   <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg" alt="Apache 2.0 License"></a>
+  <a href="https://gitpod.io/#https://github.com/01walid/cdktf-gke-auth"><img src="https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod" alt="Gitpod ready-to-code"></a>
   <a href="https://www.npmjs.com/package/cdktf-gke-auth"><img src="https://badge.fury.io/js/cdktf-gke-auth.svg" alt="npm version"></a>
+  <a href="https://pypi.org/project/cdktf-gke-auth/"><img src="https://badge.fury.io/py/cdktf-gke-auth.svg" alt="PyPI version"></a>
   <a href="https://github.com/01walid/cdktf-gke-auth/actions/workflows/build.yml"><img src="https://github.com/01walid/cdktf-gke-auth/actions/workflows/build.yml/badge.svg" alt="Build badge"></a>
   <a href="https://github.com/01walid/cdktf-gke-auth/actions/workflows/release.yml"><img src="https://github.com/01walid/cdktf-gke-auth/actions/workflows/release.yml/badge.svg" alt="Release badge"></a>
 </p>
 
 # cdktf-gke-auth
 
 Easily authenticate against a Google Kubernetes Engine (GKE) within your CDK for Terraform stack. Without the need to
 resort to [Google's terraform GKE auth](https://github.com/terraform-google-modules/terraform-google-kubernetes-engine/tree/v26.1.1/modules/auth) module. You can avoid running `cdktf get` as pre-synth step.
 
+This project uses [projen](https://github.com/projen/projen) and [jsii](https://github.com/aws/jsii) to compile the construct to Typescript, Python, Go and .Net (Java upon request).
+
 ## Example usage (Typescript)
 
 Install the construct with: `yarn install cdktf-gke-auth`.
 
 ```python
 import { GoogleProvider } from "@cdktf/provider-google/lib/provider";
 import { TerraformOutput, TerraformStack } from "cdktf";
@@ -30,28 +34,30 @@
     const auth = new GKEAuth(this, "gke-auth", {
       clusterName: "my-cluster",
       location: "europe-west1",
       projectId: "my-project",
     });
 
     // init the Kubernetes provider like so:
-    // new KubernetesProvider(this, "kubernetes", {
-    //   ...auth.authCredentials
-    // });
+    new KubernetesProvider(this, "kubernetes", {
+      ...auth.authCredentials
+    });
 
     // Or a helm provider like so:
-    //  new HelmProvider(this, "helm", {
-    //   kubernetes: auth.authCredentials,
-    // });
+     new HelmProvider(this, "helm", {
+      kubernetes: auth.authCredentials,
+    });
   }
 }
 ```
 
 The `GKEAuth` instance expose `host`, `clusterCaCertificate`, `clusterCaCertificatePEM`, and `token` you can use to authenticate using
 any of the kubernetes popular cdktf providers.
+
+For other languages examples, checkout this construct on [ConstructHub](https://constructs.dev/packages/cdktf-gke-auth/).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -128,14 +134,77 @@
 
     def __repr__(self) -> str:
         return "AuthCredentials(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="cdktf-gke-auth.ClusterInfo",
+    jsii_struct_bases=[],
+    name_mapping={
+        "cluster_name": "clusterName",
+        "location": "location",
+        "project_id": "projectId",
+    },
+)
+class ClusterInfo:
+    def __init__(
+        self,
+        *,
+        cluster_name: builtins.str,
+        location: builtins.str,
+        project_id: builtins.str,
+    ) -> None:
+        '''
+        :param cluster_name: 
+        :param location: 
+        :param project_id: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b934b88fa4ac34cda3f71ae8f1a0a22b11f51e21a86a39607bb7bb32ad38bf2b)
+            check_type(argname="argument cluster_name", value=cluster_name, expected_type=type_hints["cluster_name"])
+            check_type(argname="argument location", value=location, expected_type=type_hints["location"])
+            check_type(argname="argument project_id", value=project_id, expected_type=type_hints["project_id"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "cluster_name": cluster_name,
+            "location": location,
+            "project_id": project_id,
+        }
+
+    @builtins.property
+    def cluster_name(self) -> builtins.str:
+        result = self._values.get("cluster_name")
+        assert result is not None, "Required property 'cluster_name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def location(self) -> builtins.str:
+        result = self._values.get("location")
+        assert result is not None, "Required property 'location' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def project_id(self) -> builtins.str:
+        result = self._values.get("project_id")
+        assert result is not None, "Required property 'project_id' is missing"
+        return typing.cast(builtins.str, result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "ClusterInfo(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.implements(_cdktf_9a9027ec.ITerraformDependable)
 class GKEAuth(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdktf-gke-auth.GKEAuth",
 ):
     def __init__(
@@ -154,15 +223,15 @@
         :param location: 
         :param project_id: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__71514e77038348f5442dde297a2d25dd17d9df0eabb64fc9c335dc5902ded582)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        props = GkeControlPlaneProps(
+        props = ClusterInfo(
             cluster_name=cluster_name, location=location, project_id=project_id
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="authCredentials")
@@ -215,106 +284,43 @@
 
     @builtins.property
     @jsii.member(jsii_name="token")
     def token(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "token"))
 
 
-@jsii.data_type(
-    jsii_type="cdktf-gke-auth.GkeControlPlaneProps",
-    jsii_struct_bases=[],
-    name_mapping={
-        "cluster_name": "clusterName",
-        "location": "location",
-        "project_id": "projectId",
-    },
-)
-class GkeControlPlaneProps:
-    def __init__(
-        self,
-        *,
-        cluster_name: builtins.str,
-        location: builtins.str,
-        project_id: builtins.str,
-    ) -> None:
-        '''
-        :param cluster_name: 
-        :param location: 
-        :param project_id: 
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__89ff4487bf931715058231b7757c5544cdc0826cb62ded6e7e2bca28c1dc6b8f)
-            check_type(argname="argument cluster_name", value=cluster_name, expected_type=type_hints["cluster_name"])
-            check_type(argname="argument location", value=location, expected_type=type_hints["location"])
-            check_type(argname="argument project_id", value=project_id, expected_type=type_hints["project_id"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "cluster_name": cluster_name,
-            "location": location,
-            "project_id": project_id,
-        }
-
-    @builtins.property
-    def cluster_name(self) -> builtins.str:
-        result = self._values.get("cluster_name")
-        assert result is not None, "Required property 'cluster_name' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def location(self) -> builtins.str:
-        result = self._values.get("location")
-        assert result is not None, "Required property 'location' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def project_id(self) -> builtins.str:
-        result = self._values.get("project_id")
-        assert result is not None, "Required property 'project_id' is missing"
-        return typing.cast(builtins.str, result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "GkeControlPlaneProps(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
 __all__ = [
     "AuthCredentials",
+    "ClusterInfo",
     "GKEAuth",
-    "GkeControlPlaneProps",
 ]
 
 publication.publish()
 
 def _typecheckingstub__ba90e7c257be36144934039cc0a19d9ef6cf64b1c94e73ca1a7334437127b3ac(
     *,
     cluster_ca_certificate: builtins.str,
     host: builtins.str,
     token: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__71514e77038348f5442dde297a2d25dd17d9df0eabb64fc9c335dc5902ded582(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
+def _typecheckingstub__b934b88fa4ac34cda3f71ae8f1a0a22b11f51e21a86a39607bb7bb32ad38bf2b(
     *,
     cluster_name: builtins.str,
     location: builtins.str,
     project_id: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__89ff4487bf931715058231b7757c5544cdc0826cb62ded6e7e2bca28c1dc6b8f(
+def _typecheckingstub__71514e77038348f5442dde297a2d25dd17d9df0eabb64fc9c335dc5902ded582(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
     *,
     cluster_name: builtins.str,
     location: builtins.str,
     project_id: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-gke-auth-1.0.1/src/cdktf_gke_auth.egg-info/PKG-INFO` & `cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-gke-auth
-Version: 1.0.1
+Version: 1.1.0
 Summary: cdktf-gke-auth
 Home-page: https://github.com/01walid/cdktf-gke-auth.git
 Author: Walid Ziouche<hi@walid.dev>
 License: Apache-2.0
 Project-URL: Source, https://github.com/01walid/cdktf-gke-auth.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -20,24 +20,28 @@
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg" alt="Apache 2.0 License"></a>
+  <a href="https://gitpod.io/#https://github.com/01walid/cdktf-gke-auth"><img src="https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod" alt="Gitpod ready-to-code"></a>
   <a href="https://www.npmjs.com/package/cdktf-gke-auth"><img src="https://badge.fury.io/js/cdktf-gke-auth.svg" alt="npm version"></a>
+  <a href="https://pypi.org/project/cdktf-gke-auth/"><img src="https://badge.fury.io/py/cdktf-gke-auth.svg" alt="PyPI version"></a>
   <a href="https://github.com/01walid/cdktf-gke-auth/actions/workflows/build.yml"><img src="https://github.com/01walid/cdktf-gke-auth/actions/workflows/build.yml/badge.svg" alt="Build badge"></a>
   <a href="https://github.com/01walid/cdktf-gke-auth/actions/workflows/release.yml"><img src="https://github.com/01walid/cdktf-gke-auth/actions/workflows/release.yml/badge.svg" alt="Release badge"></a>
 </p>
 
 # cdktf-gke-auth
 
 Easily authenticate against a Google Kubernetes Engine (GKE) within your CDK for Terraform stack. Without the need to
 resort to [Google's terraform GKE auth](https://github.com/terraform-google-modules/terraform-google-kubernetes-engine/tree/v26.1.1/modules/auth) module. You can avoid running `cdktf get` as pre-synth step.
 
+This project uses [projen](https://github.com/projen/projen) and [jsii](https://github.com/aws/jsii) to compile the construct to Typescript, Python, Go and .Net (Java upon request).
+
 ## Example usage (Typescript)
 
 Install the construct with: `yarn install cdktf-gke-auth`.
 
 ```python
 import { GoogleProvider } from "@cdktf/provider-google/lib/provider";
 import { TerraformOutput, TerraformStack } from "cdktf";
@@ -53,21 +57,23 @@
     const auth = new GKEAuth(this, "gke-auth", {
       clusterName: "my-cluster",
       location: "europe-west1",
       projectId: "my-project",
     });
 
     // init the Kubernetes provider like so:
-    // new KubernetesProvider(this, "kubernetes", {
-    //   ...auth.authCredentials
-    // });
+    new KubernetesProvider(this, "kubernetes", {
+      ...auth.authCredentials
+    });
 
     // Or a helm provider like so:
-    //  new HelmProvider(this, "helm", {
-    //   kubernetes: auth.authCredentials,
-    // });
+     new HelmProvider(this, "helm", {
+      kubernetes: auth.authCredentials,
+    });
   }
 }
 ```
 
 The `GKEAuth` instance expose `host`, `clusterCaCertificate`, `clusterCaCertificatePEM`, and `token` you can use to authenticate using
 any of the kubernetes popular cdktf providers.
+
+For other languages examples, checkout this construct on [ConstructHub](https://constructs.dev/packages/cdktf-gke-auth/).
```

