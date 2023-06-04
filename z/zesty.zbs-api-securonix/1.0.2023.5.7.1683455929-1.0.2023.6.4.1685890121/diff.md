# Comparing `tmp/zesty.zbs-api-securonix-1.0.2023.5.7.1683455929.tar.gz` & `tmp/zesty.zbs-api-securonix-1.0.2023.6.4.1685890121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.5.7.1683455929.tar", last modified: Sun May  7 10:38:50 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.6.4.1685890121.tar", last modified: Sun Jun  4 14:48:41 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929.tar` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1175 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13467 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3326 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     7404 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7245 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1879 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    10693 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    12497 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     6791 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1175 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13458 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3326 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7404 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7245 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    10693 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    12497 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     7199 2023-06-04 14:47:37.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-04 14:48:41.000000 zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.5.7.1683455929
+Version: 1.0.2023.6.4.1685890121
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/README.md` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/setup.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/actions.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Command Design Pattern (Behavioral Design Pattern)
 """
 import uuid as uuid_gen
-import warnings
+from abc import abstractmethod
 from typing import Dict
-from .models.hf_interface import *
-from .models.BlockDevice import BlockDevice
+
+from .models.hf_interface import IActionHF, ISpecialInstructions
 
 
 class ZBSActionData:
     mount_path = None
     device = None
     filesystem = None
     fs_type = None
@@ -130,15 +130,15 @@
         -- Actions in a list keyed to a higher order cannot start until all Actions of lower orders complete
     """
 
     def __init__(self, dev_id: str = None, size: int = None, sub_actions: Dict[int, Dict[str, IActionHF]] = None):
         self.dev_id = dev_id
         self.size = size
         self.sub_actions = sub_actions
-        
+
     def __repr__(self):
         return str(self.__dict__)
 
 
 class ZBSAction(IActionHF):
     """
     Base command class
@@ -169,21 +169,21 @@
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         cls.subclasses[cls.__name__] = cls
 
     def __repr__(self):
         special_instructions = self.get_special_instructions() if isinstance(self.get_special_instructions(),
                                                                              Dict) else self.get_special_instructions().__dict__
-        repr_dict = dict(zip(['Action Type','Action Status','SpecialInstructions'],
-                            [self.get_action_type(),
+        repr_dict = dict(zip(['Action Type', 'Action Status', 'SpecialInstructions'],
+                             [self.get_action_type(),
                              str(self.get_status().name),
                              special_instructions]))
-        
+
         return str(repr_dict)
-    
+
     def set_data(self, data: ZBSActionData):
         self.data = data
 
     def set_receiver(self, receiver: ZBSAgentReceiver):
         self.receiver = receiver
 
     def serialize(self):
@@ -234,17 +234,17 @@
         return serialized_action.get(ZBSAction.STATUS_FIELD_NAME)
 
     @staticmethod
     def deserialize_special_instructions(serialized_action):
         if not isinstance(serialized_action, dict):
             serialized_action = serialized_action.serialize()
         special_instructions = SpecialInstructions(
-            dev_id=serialized_action.get(ZBSAction.SPECIAL_INSTRUCTIONS_FIELD_NAME, {}).get('dev_id'),
-            size=serialized_action.get(ZBSAction.SPECIAL_INSTRUCTIONS_FIELD_NAME, {}).get('size'),
-            sub_actions=serialized_action.get(ZBSAction.SPECIAL_INSTRUCTIONS_FIELD_NAME, {}).get('sub_actions'),
+            dev_id = serialized_action.get(ZBSAction.SPECIAL_INSTRUCTIONS_FIELD_NAME, {}).get('dev_id'),
+            size = serialized_action.get(ZBSAction.SPECIAL_INSTRUCTIONS_FIELD_NAME, {}).get('size'),
+            sub_actions = serialized_action.get(ZBSAction.SPECIAL_INSTRUCTIONS_FIELD_NAME, {}).get('sub_actions'),
         )
         for key, val in serialized_action.get(ZBSAction.SPECIAL_INSTRUCTIONS_FIELD_NAME, {}).items():
             if key not in ['dev_id', 'size', 'sub_actions']:
                 setattr(special_instructions, str(key), val)
 
         return special_instructions
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/BlockDevice.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/FileSystem.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/ManagedFS.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/ManagedFS.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/Usage.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/agent_report.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/disk_mon.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/hf_interface.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/overview.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/protocol.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/protocol.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/step_instructions.py` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/src/step_instructions.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,25 @@
             and self.dev_size_gb is None \
             and self.dev_iops is None \
             and self.dev_throughput is None:
             raise Exception(f"Must modify at least one attribute")
 
 
 @dataclass
+class DetachDiskCloud(CloudInstruction):
+    dev_id: str
+
+
+@dataclass
+class TakeSnapshotCloud(CloudInstruction):
+    dev_id: str
+    snapshot_id: str
+
+
+@dataclass
 class ExtendDiskSizeMachine(MachineInstruction):
     # Note: this is a copy of AddDiskMachine
     fs_id: str  # will there be ability to grab this from context?
     fs_mount_path: str
     # dev_path: str  # This is necessary for Monitored disk Extend only actions
                      # Probably better to have a separate payload/step
     btrfs_dev_id: int
@@ -214,7 +225,18 @@
 
 ###### TODO: END discuss with Osher
 
 
 @dataclass
 class RemoveDiskCloud(CloudInstruction):
     volume_id: str
+
+
+@dataclass
+class StartMigrationMachine(MachineInstruction):
+    fs_id: str  # will there be ability to grab this from context?
+    account_id: str
+    action_id: str
+    fs_mount_path: str
+    volume_id: str
+    dev_path: str
+    reboot: bool
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.5.7.1683455929
+Version: 1.0.2023.6.4.1685890121
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-1.0.2023.6.4.1685890121/zesty.zbs_api_securonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

