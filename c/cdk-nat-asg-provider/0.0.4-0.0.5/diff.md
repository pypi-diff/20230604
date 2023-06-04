# Comparing `tmp/cdk-nat-asg-provider-0.0.4.tar.gz` & `tmp/cdk-nat-asg-provider-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-nat-asg-provider-0.0.4.tar", last modified: Tue Feb 21 01:22:42 2023, max compression
+gzip compressed data, was "cdk-nat-asg-provider-0.0.5.tar", last modified: Sun Jun  4 21:06:47 2023, max compression
```

## Comparing `cdk-nat-asg-provider-0.0.4.tar` & `cdk-nat-asg-provider-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:22:42.109632 cdk-nat-asg-provider-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-21 01:22:28.000000 cdk-nat-asg-provider-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-21 01:22:28.000000 cdk-nat-asg-provider-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-02-21 01:22:42.109632 cdk-nat-asg-provider-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-02-21 01:22:28.000000 cdk-nat-asg-provider-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-21 01:22:28.000000 cdk-nat-asg-provider-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:22:42.109632 cdk-nat-asg-provider-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-21 01:22:28.000000 cdk-nat-asg-provider-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:22:42.105632 cdk-nat-asg-provider-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:22:42.105632 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider/
--rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-02-21 01:22:28.000000 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:22:42.105632 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-21 01:22:28.000000 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34658 2023-02-21 01:22:28.000000 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider/_jsii/cdk-nat-asg-provider@0.0.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:22:28.000000 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:22:42.105632 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-02-21 01:22:42.000000 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-21 01:22:42.000000 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:22:42.000000 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-21 01:22:42.000000 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:22:42.000000 cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:06:47.406078 cdk-nat-asg-provider-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-04 21:06:33.000000 cdk-nat-asg-provider-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-04 21:06:33.000000 cdk-nat-asg-provider-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-04 21:06:47.406078 cdk-nat-asg-provider-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-04 21:06:33.000000 cdk-nat-asg-provider-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-04 21:06:33.000000 cdk-nat-asg-provider-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 21:06:47.406078 cdk-nat-asg-provider-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 21:06:33.000000 cdk-nat-asg-provider-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:06:47.402078 cdk-nat-asg-provider-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:06:47.402078 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-06-04 21:06:33.000000 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:06:47.406078 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-04 21:06:33.000000 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-06-04 21:06:33.000000 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider/_jsii/cdk-nat-asg-provider@0.0.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:06:33.000000 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:06:47.406078 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-04 21:06:47.000000 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-04 21:06:47.000000 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:06:47.000000 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-04 21:06:47.000000 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-04 21:06:47.000000 cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider.egg-info/top_level.txt
```

### Comparing `cdk-nat-asg-provider-0.0.4/LICENSE` & `cdk-nat-asg-provider-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-nat-asg-provider-0.0.4/PKG-INFO` & `cdk-nat-asg-provider-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-nat-asg-provider
-Version: 0.0.4
+Version: 0.0.5
 Summary: An AWS CDK library providing NAT instances that are each placed in their own auto scaling group to improve fault tolerance and availability.
 Home-page: https://github.com/fonzcastellanos/cdk-nat-asg-provider.git
 Author: Alfonso Castellanos<dev@alfonsocastellanos.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/fonzcastellanos/cdk-nat-asg-provider.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 # CDK NAT ASG Provider
 
 ![npm version](https://img.shields.io/npm/v/cdk-nat-asg-provider)
 ![PyPi version](https://img.shields.io/pypi/v/cdk-nat-asg-provider)
 ![Release](https://github.com/fonzcastellanos/cdk-nat-asg-provider/workflows/release/badge.svg)
 ![License](https://img.shields.io/github/license/fonzcastellanos/cdk-nat-asg-provider)
 
-Use this [AWS Cloud Development Kit (CDK)](https://docs.aws.amazon.com/cdk/v2/guide/home.html) library to configure and deploy [Network Address Translation (NAT) instances](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_NAT_Instance.html) that are each in their own [auto scaling group (ASG)](https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-groups.html) to improve fault tolerance and availability.
+Use this [AWS Cloud Development Kit (CDK)](https://docs.aws.amazon.com/cdk/v2/guide/home.html) library to configure and deploy [network address translation (NAT) instances](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_NAT_Instance.html) individually within their own [auto scaling group (ASG)](https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-groups.html) to improve reliability and availability.
 
 Works with AWS CDK <strong>v2</strong>.
 
 ## Problem
 
 Although the [NAT gateways](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-gateway.html) offered by AWS have high availability, high bandwidth scalability, and minimal administration needs, they can be too expensive for small scale applications. A cheaper alternative, one that AWS mentions in its documentation but does not recommend, is to configure and manage your own NAT instances. One way of doing this is with the CDK using [`NatInstanceProvider`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.NatInstanceProvider.html).
```

### Comparing `cdk-nat-asg-provider-0.0.4/README.md` & `cdk-nat-asg-provider-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # CDK NAT ASG Provider
 
 ![npm version](https://img.shields.io/npm/v/cdk-nat-asg-provider)
 ![PyPi version](https://img.shields.io/pypi/v/cdk-nat-asg-provider)
 ![Release](https://github.com/fonzcastellanos/cdk-nat-asg-provider/workflows/release/badge.svg)
 ![License](https://img.shields.io/github/license/fonzcastellanos/cdk-nat-asg-provider)
 
-Use this [AWS Cloud Development Kit (CDK)](https://docs.aws.amazon.com/cdk/v2/guide/home.html) library to configure and deploy [Network Address Translation (NAT) instances](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_NAT_Instance.html) that are each in their own [auto scaling group (ASG)](https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-groups.html) to improve fault tolerance and availability.
+Use this [AWS Cloud Development Kit (CDK)](https://docs.aws.amazon.com/cdk/v2/guide/home.html) library to configure and deploy [network address translation (NAT) instances](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_NAT_Instance.html) individually within their own [auto scaling group (ASG)](https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-groups.html) to improve reliability and availability.
 
 Works with AWS CDK <strong>v2</strong>.
 
 ## Problem
 
 Although the [NAT gateways](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-gateway.html) offered by AWS have high availability, high bandwidth scalability, and minimal administration needs, they can be too expensive for small scale applications. A cheaper alternative, one that AWS mentions in its documentation but does not recommend, is to configure and manage your own NAT instances. One way of doing this is with the CDK using [`NatInstanceProvider`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.NatInstanceProvider.html).
```

### Comparing `cdk-nat-asg-provider-0.0.4/setup.py` & `cdk-nat-asg-provider-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-nat-asg-provider",
-    "version": "0.0.4",
+    "version": "0.0.5",
     "description": "An AWS CDK library providing NAT instances that are each placed in their own auto scaling group to improve fault tolerance and availability.",
     "license": "Apache-2.0",
     "url": "https://github.com/fonzcastellanos/cdk-nat-asg-provider.git",
     "long_description_content_type": "text/markdown",
     "author": "Alfonso Castellanos<dev@alfonsocastellanos.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_nat_asg_provider",
         "cdk_nat_asg_provider._jsii"
     ],
     "package_data": {
         "cdk_nat_asg_provider._jsii": [
-            "cdk-nat-asg-provider@0.0.4.jsii.tgz"
+            "cdk-nat-asg-provider@0.0.5.jsii.tgz"
         ],
         "cdk_nat_asg_provider": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider/__init__.py` & `cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # CDK NAT ASG Provider
 
 ![npm version](https://img.shields.io/npm/v/cdk-nat-asg-provider)
 ![PyPi version](https://img.shields.io/pypi/v/cdk-nat-asg-provider)
 ![Release](https://github.com/fonzcastellanos/cdk-nat-asg-provider/workflows/release/badge.svg)
 ![License](https://img.shields.io/github/license/fonzcastellanos/cdk-nat-asg-provider)
 
-Use this [AWS Cloud Development Kit (CDK)](https://docs.aws.amazon.com/cdk/v2/guide/home.html) library to configure and deploy [Network Address Translation (NAT) instances](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_NAT_Instance.html) that are each in their own [auto scaling group (ASG)](https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-groups.html) to improve fault tolerance and availability.
+Use this [AWS Cloud Development Kit (CDK)](https://docs.aws.amazon.com/cdk/v2/guide/home.html) library to configure and deploy [network address translation (NAT) instances](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_NAT_Instance.html) individually within their own [auto scaling group (ASG)](https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-groups.html) to improve reliability and availability.
 
 Works with AWS CDK <strong>v2</strong>.
 
 ## Problem
 
 Although the [NAT gateways](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-gateway.html) offered by AWS have high availability, high bandwidth scalability, and minimal administration needs, they can be too expensive for small scale applications. A cheaper alternative, one that AWS mentions in its documentation but does not recommend, is to configure and manage your own NAT instances. One way of doing this is with the CDK using [`NatInstanceProvider`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.NatInstanceProvider.html).
```

### Comparing `cdk-nat-asg-provider-0.0.4/src/cdk_nat_asg_provider.egg-info/PKG-INFO` & `cdk-nat-asg-provider-0.0.5/src/cdk_nat_asg_provider.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-nat-asg-provider
-Version: 0.0.4
+Version: 0.0.5
 Summary: An AWS CDK library providing NAT instances that are each placed in their own auto scaling group to improve fault tolerance and availability.
 Home-page: https://github.com/fonzcastellanos/cdk-nat-asg-provider.git
 Author: Alfonso Castellanos<dev@alfonsocastellanos.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/fonzcastellanos/cdk-nat-asg-provider.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 # CDK NAT ASG Provider
 
 ![npm version](https://img.shields.io/npm/v/cdk-nat-asg-provider)
 ![PyPi version](https://img.shields.io/pypi/v/cdk-nat-asg-provider)
 ![Release](https://github.com/fonzcastellanos/cdk-nat-asg-provider/workflows/release/badge.svg)
 ![License](https://img.shields.io/github/license/fonzcastellanos/cdk-nat-asg-provider)
 
-Use this [AWS Cloud Development Kit (CDK)](https://docs.aws.amazon.com/cdk/v2/guide/home.html) library to configure and deploy [Network Address Translation (NAT) instances](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_NAT_Instance.html) that are each in their own [auto scaling group (ASG)](https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-groups.html) to improve fault tolerance and availability.
+Use this [AWS Cloud Development Kit (CDK)](https://docs.aws.amazon.com/cdk/v2/guide/home.html) library to configure and deploy [network address translation (NAT) instances](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_NAT_Instance.html) individually within their own [auto scaling group (ASG)](https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-groups.html) to improve reliability and availability.
 
 Works with AWS CDK <strong>v2</strong>.
 
 ## Problem
 
 Although the [NAT gateways](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-gateway.html) offered by AWS have high availability, high bandwidth scalability, and minimal administration needs, they can be too expensive for small scale applications. A cheaper alternative, one that AWS mentions in its documentation but does not recommend, is to configure and manage your own NAT instances. One way of doing this is with the CDK using [`NatInstanceProvider`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_ec2.NatInstanceProvider.html).
```

