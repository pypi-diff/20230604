# Comparing `tmp/python-selve-new-2.2.1.tar.gz` & `tmp/python-selve-new-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-selve-new-2.2.1.tar", last modified: Sat Jun  3 21:11:45 2023, max compression
+gzip compressed data, was "python-selve-new-2.2.2.tar", last modified: Sun Jun  4 13:47:23 2023, max compression
```

## Comparing `python-selve-new-2.2.1.tar` & `python-selve-new-2.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:11:45.316215 python-selve-new-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-03 21:11:45.316215 python-selve-new-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:11:45.316215 python-selve-new-2.2.1/python_selve_new.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-03 21:11:45.000000 python-selve-new-2.2.1/python_selve_new.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-03 21:11:45.000000 python-selve-new-2.2.1/python_selve_new.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 21:11:45.000000 python-selve-new-2.2.1/python_selve_new.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 21:11:45.000000 python-selve-new-2.2.1/python_selve_new.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 21:11:45.000000 python-selve-new-2.2.1/python_selve_new.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:11:45.316215 python-selve-new-2.2.1/selve/
--rw-r--r--   0 runner    (1001) docker     (123)    51216 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:11:45.316215 python-selve-new-2.2.1/selve/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/commands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/device.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:11:45.316215 python-selve-new-2.2.1/selve/util/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/selve/util/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 21:11:45.316215 python-selve-new-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-03 21:11:38.000000 python-selve-new-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:47:23.572675 python-selve-new-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-04 13:47:23.572675 python-selve-new-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:47:23.572675 python-selve-new-2.2.2/python_selve_new.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-04 13:47:23.000000 python-selve-new-2.2.2/python_selve_new.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-04 13:47:23.000000 python-selve-new-2.2.2/python_selve_new.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:47:23.000000 python-selve-new-2.2.2/python_selve_new.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-04 13:47:23.000000 python-selve-new-2.2.2/python_selve_new.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 13:47:23.000000 python-selve-new-2.2.2/python_selve_new.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:47:23.572675 python-selve-new-2.2.2/selve/
+-rw-r--r--   0 runner    (1001) docker     (123)    65992 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:47:23.572675 python-selve-new-2.2.2/selve/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/commands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:47:23.572675 python-selve-new-2.2.2/selve/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/selve/util/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 13:47:23.572675 python-selve-new-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-04 13:47:20.000000 python-selve-new-2.2.2/setup.py
```

### Comparing `python-selve-new-2.2.1/LICENSE` & `python-selve-new-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/PKG-INFO` & `python-selve-new-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.2.1/python_selve_new.egg-info/PKG-INFO` & `python-selve-new-2.2.2/python_selve_new.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.2.1/python_selve_new.egg-info/SOURCES.txt` & `python-selve-new-2.2.2/python_selve_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/__init__.py` & `python-selve-new-2.2.2/selve/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Callable
 
 import serial
 from serial.tools import list_ports
 import untangle
 
 from selve.commands import param, service
+from selve.commands import device
 from selve.commands.device import *
 from selve.commands.command import *
 from selve.commands.event import *
 from selve.commands.group import *
 from selve.commands.iveo import *
 from selve.commands.service import *
 from selve.commands.param import *
@@ -314,14 +315,18 @@
                 await self.processEventResponse(response)
             if isinstance(response, CommandResultResponse)\
                     or isinstance(response, IveoResultResponse):
                 #update device values
                 self.commandResult(response)
             if isinstance(response, DeviceGetValuesResponse):
                 self.updateCommeoDeviceValuesFromResponse(int(response.parameters[1][1]), response)
+            if isinstance(response, SenderTeachResultResponse) \
+                or isinstance(response, SensorTeachResultResponse)\
+                or isinstance(response, DeviceScanResultResponse):
+                self.processTeachResponse(response)
 
             return response
 
         except Exception as e:
             self._LOGGER.error("Error in response processing: " + str(e) + " : " + xmlstr)
             return False
 
@@ -757,101 +762,40 @@
             boundary = 7
 
         while i < boundary:
             if not self.is_id_registered(i, type):
                 return i
             i = i + 1
 
-    async def pingGateway(self):
-        cmd = service.ServicePing()
-        methodResponse = await self.executeCommandSyncWithResponse(cmd)
-        try:
-            if hasattr(methodResponse, "name"):
-                if methodResponse.name == "selve.GW.service.ping":
-                    self._LOGGER.debug("Ping back")
-                    return True
-        except:
-            self._LOGGER.debug("Error in ping")
-        self._LOGGER.debug("No ping")
-        return False
-
-
-    async def gatewayState(self):
-        cmd = service.ServiceGetState()
-        try:
-            methodResponse = await self.executeCommandSyncWithResponse(cmd)
-        except GatewayError:
-            self._LOGGER.error(str(GatewayError))
-            methodResponse = None
-
-        if hasattr(methodResponse, "name"):
-            if methodResponse.name == "selve.GW." + str(CommeoServiceCommand.GETSTATE.value):
-                if hasattr(methodResponse, "parameters"):
-                    status = ServiceState(int(methodResponse.parameters[0][1]))
-                    self._LOGGER.debug(f'Gateway state: {status}')
-                    self.state = status
-                    return status
-        return None
-
-    async def gatewayReady(self):
-        state = await self.gatewayState()
-        return state is ServiceState.READY
-
-    async def getVersionG(self):
-        cmd = service.ServiceGetVersion()
-        methodResponse = await self.executeCommandSyncWithResponse(cmd)
-        return methodResponse
-
-    async def getGatewayFirmwareVersion(self):
-        command = await self.getVersionG()
-        if hasattr(command, "version"):
-            return command.version
-        else:
-            return False
-
-    async def getGatewaySerial(self):
-        command = await self.getVersionG()
-        if hasattr(command, "serial"):
-            return command.serial
-        else:
-            return False
-
-    async def getGatewaySpec(self):
-        command = await self.getVersionG()
-        if hasattr(command, "spec"):
-            return command.spec
-        else:
-            return False
-
-    def list_devices(self):
-        """[summary]
-        Log the list of registered devices
-        """
-        for id, val in self.devices.items():
-            for ida, device in val.items():
-                self._LOGGER.info(str(device))
-
-    async def resetGateway(self):
-        command = service.ServiceReset()
-        response: ServiceResetResponse = await self.executeCommandSyncWithResponse(command)
-        if response.executed != 1:
-            self._LOGGER.info("Error: Gateway could not be reset or loads too long")
-
-        # time.sleep(2)
+    async def processTeachResponse(self, response):
+        if isinstance(response, SenderTeachResultResponse):
+            if response.senderId == -1:
+                self._LOGGER.info("No Senders found yet...")
+            else:
+                self._LOGGER.info("Sender found: " + str(response.name) + " - " + str(response.senderId))
+            self._LOGGER.info("Time left for teaching: " + str(response.timeLeft) + "s")
+            self._LOGGER.debug("Current teaching state: " + str(response.teachState.name))
+            self._LOGGER.info("Last event: " + str(response.senderEvent.name))
+        
+        if isinstance(response, SensorTeachResultResponse):
+            if response.foundId == -1:
+                self._LOGGER.info("No Senders found yet...")
+            else:
+                self._LOGGER.info("Sensor found: " + str(response.foundId))
+            self._LOGGER.info("Time left for teaching: " + str(response.timeLeft) + "s")
+            self._LOGGER.debug("Current teaching state: " + str(response.teachState.name))
+                
+        if isinstance(response, DeviceScanResultResponse):
+            if response.noNewDevices <= 0:
+                self._LOGGER.info("No Senders found yet...")
+            else:
+                self._LOGGER.info("Devices found: " + str(response.foundIds))
+            self._LOGGER.debug("Current teaching state: " + str(response.scanState.name))
 
-        start_time = time.time()
-        while await self.gatewayState() != ServiceState.READY:
-            if time.time() - start_time >= 10:
-                self._LOGGER.info("Error: Gateway could not be reset or loads too long")
-            pass
-        self._LOGGER.info("Gateway reset")
 
-    async def setEvents(self, eventDevice = False, eventSensor = False, eventSender = False, eventLogging = False, eventDuty = False):
-        command = param.ParamSetEvent(eventDevice, eventSensor, eventSender, eventLogging, eventDuty)
-        return await self.executeCommandSyncWithResponse(command)
 
     async def processEventResponse(self, response):
         if isinstance(response, CommeoDeviceEventResponse):
             # This is a commeo device response, Iveo does not generate events because it is a one way communication protocol
             if self.is_id_registered(response.id, SelveTypes.DEVICE):
                 device: SelveDevice = self.devices[SelveTypes.DEVICE.value][response.id]
             else:
@@ -926,16 +870,221 @@
             self.utilization = response.traffic
 
 
     def commandResult(self, response):
         for callback in self._callbacks:
             callback()
 
-    ##Device functions
 
+    ### Service
+
+    async def pingGateway(self):
+        cmd = ServicePing()
+        methodResponse = await self.executeCommandSyncWithResponse(cmd)
+        try:
+            if hasattr(methodResponse, "name"):
+                if methodResponse.name == "selve.GW.service.ping":
+                    self._LOGGER.debug("Ping back")
+                    return True
+        except:
+            self._LOGGER.debug("Error in ping")
+        self._LOGGER.debug("No ping")
+        return False
+
+
+    async def gatewayState(self):
+        cmd = ServiceGetState()
+        try:
+            methodResponse = await self.executeCommandSyncWithResponse(cmd)
+        except GatewayError:
+            self._LOGGER.error(str(GatewayError))
+            methodResponse = None
+
+        if hasattr(methodResponse, "name"):
+            if methodResponse.name == "selve.GW." + str(CommeoServiceCommand.GETSTATE.value):
+                if hasattr(methodResponse, "parameters"):
+                    status = ServiceState(int(methodResponse.parameters[0][1]))
+                    self._LOGGER.debug(f'Gateway state: {status}')
+                    self.state = status
+                    return status
+        return None
+
+    async def gatewayReady(self):
+        state = await self.gatewayState()
+        return state is ServiceState.READY
+
+    async def getVersionG(self):
+        cmd = ServiceGetVersion()
+        methodResponse = await self.executeCommandSyncWithResponse(cmd)
+        return methodResponse
+
+    async def getGatewayFirmwareVersion(self):
+        command = await self.getVersionG()
+        if hasattr(command, "version"):
+            return command.version
+        else:
+            return False
+
+    async def getGatewaySerial(self):
+        command = await self.getVersionG()
+        if hasattr(command, "serial"):
+            return command.serial
+        else:
+            return False
+
+    async def getGatewaySpec(self):
+        command = await self.getVersionG()
+        if hasattr(command, "spec"):
+            return command.spec
+        else:
+            return False
+
+    def list_devices(self):
+        """[summary]
+        Log the list of registered devices
+        """
+        for id, val in self.devices.items():
+            for ida, device in val.items():
+                self._LOGGER.info(str(device))
+
+    async def resetGateway(self):
+        command = ServiceReset()
+        response: ServiceResetResponse = await self.executeCommandSyncWithResponse(command)
+        if response.executed is not True:
+            self._LOGGER.info("Error: Gateway could not be reset or loads too long")
+
+        # time.sleep(2)
+
+        start_time = time.time()
+        while await self.gatewayState() != ServiceState.READY:
+            if time.time() - start_time >= 30:
+                self._LOGGER.info("Error: Gateway could not be reset or loads too long")
+            pass
+        self._LOGGER.info("Gateway reset")
+
+    async def factoryResetGateway(self):
+        command = ServiceFactoryReset()
+        response: ServiceFactoryResetResponse = await self.executeCommandSyncWithResponse(command)
+        if response.executed is not True:
+            self._LOGGER.info("Error: Gateway could not be reset or loads too long")
+
+        start_time = time.time()
+        while await self.gatewayState() != ServiceState.READY:
+            if time.time() - start_time >= 60:
+                self._LOGGER.info("Error: Gateway could not be reset or loads too long")
+            pass
+        self._LOGGER.info("Gateway factory reset")
+        return response.executed
+
+    async def setLED(self, state: bool):
+        command = ServiceSetLed(state)
+        response: ServiceSetLedResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def getLED(self):
+        command = ServiceGetLed()
+        response: ServiceGetLedResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+
+    ### Param
+    async def setForward(self, state: bool):
+        command = ParamSetForward(state)
+        response: ParamSetForwardResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
+    async def getForward(self):
+        command = ParamGetForward()
+        response: ParamGetForwardResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+
+    async def setEvents(self, eventDevice = False, eventSensor = False, eventSender = False, eventLogging = False, eventDuty = False):
+        command = ParamSetEvent(eventDevice, eventSensor, eventSender, eventLogging, eventDuty)
+        return await self.executeCommandSyncWithResponse(command)
+    
+    
+    async def getEvents(self):
+        command = ParamGetEvent()
+        response: ParamGetEventResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    
+    async def getDuty(self):
+        command = ParamGetDuty()
+        response: ParamGetDutyResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def getRF(self):
+        command = ParamGetRf()
+        response: ParamGetRfResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+
+    
+
+    ##Device functions
+    async def scanStart(self):
+        command = DeviceScanStart()
+        response: DeviceScanStartResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def scanStop(self):
+        command = DeviceScanStop()
+        response: DeviceScanStopResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def scanResult(self):
+        """ manually polls the scan state, but the states are being reported automatically by the gateway itself"""
+        command = DeviceScanResult()
+        response: DeviceScanResultResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+
+    async def deviceSave(self, id: int):
+        command = DeviceSave(id)
+        response: DeviceSaveResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def deviceGetIds(self):
+        command = DeviceGetIds()
+        response: DeviceGetIdsResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def deviceGetInfo(self, id: int):
+        command = DeviceGetInfo(id)
+        response: DeviceGetInfoResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+
+    async def deviceGetValues(self, id: int):
+        command = DeviceGetValues(id)
+        response: DeviceGetValuesResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def deviceSetFunction(self, id: int, function: DeviceFunctions):
+        command = DeviceSetFunction(id, function)
+        response: DeviceSetFunctionResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def deviceSetLabel(self, id: int, label: str):
+        command = DeviceSetLabel(id, label)
+        response: DeviceSetLabelResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
+    async def deviceSetType(self, id: int, type: DeviceType):
+        command = DeviceSetType(id, type)
+        response: DeviceSetTypeResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
+    async def deviceDelete(self, id: int):
+        command = DeviceDelete(id)
+        response: DeviceDeleteResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def deviceWriteManual(self, id: int, address: int, name: str, config: DeviceType):
+        command = DeviceWriteManual(id, address, name, config)
+        response: DeviceWriteManualResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+        
     async def updateCommeoDeviceValues(self, id: int):
         response: DeviceGetValuesResponse = await self.executeCommandSyncWithResponse(DeviceGetValues(id))
         self.updateCommeoDeviceValuesFromResponse(id, response)
 
     async def updateCommeoDeviceValuesAsync(self, id: int):
         await self.executeCommand(DeviceGetValues(id))
 
@@ -1039,15 +1188,36 @@
             await self.updateCommeoDeviceValuesAsync(device.id)
         else:
             await self.executeCommand(IveoManual(device.id, DriveCommandIveo.STOP))
             self.setDeviceState(device.id, MovementState.STOPPED_OFF, SelveTypes.IVEO)
             self.setDeviceValue(device.id, 50, SelveTypes.IVEO)
             self.setDeviceTargetValue(device.id, 50, SelveTypes.IVEO)
 
+
     ## Group
+    async def groupRead(self, id: int):
+        command = GroupRead(id)
+        response: GroupReadResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def groupWrite(self, id: int, actorIds: dict, name: str):
+        command = GroupWrite(id, actorIds, name)
+        response: GroupWriteResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def groupGetIds(self):
+        command = GroupGetIds()
+        response: GroupGetIdsResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def groupDelete(self, id: int):
+        command = GroupDelete(id)
+        response: GroupDeleteResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
     async def moveGroupUp(self, group: SelveGroup, type=DeviceCommandType.MANUAL):
         await self.executeCommand(CommandDriveUpGroup(group.id, type))
         for id in Util.b64_mask_to_list(group.mask):
             await self.updateCommeoDeviceValuesAsync(id)
 
     async def moveGroupDown(self, group: SelveGroup, type=DeviceCommandType.MANUAL):
         await self.executeCommand(CommandDriveDownGroup(group.id, type))
@@ -1056,18 +1226,206 @@
 
     async def stopGroup(self, group: SelveGroup, type=DeviceCommandType.MANUAL):
         await self.executeCommand(CommandStopGroup(group.id, type))
         for id in Util.b64bytes_to_bitlist(group.mask):
             await self.updateCommeoDeviceValuesAsync(id)
 
 
+    ### Iveo
+    async def iveoSetRepeater(self, repeaterInstalled: int):
+        """ 
+            Sets the repeater level. \n
+            repeaterInstalled: int can be \n
+            0 = no repeater installed\n
+            1 = repeater installed for 1-time forwarding\n
+            2 = multiple repeaters installed for 2-time forwarding
+        """
+        command = IveoSetRepeater(repeaterInstalled)
+        response: IveoSetRepeaterResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def iveoGetRepeater(self):
+        """ 
+            Gets the repeater level. \n
+            response.repeaterState: int can be \n
+            0 = no repeater installed\n
+            1 = repeater installed for 1-time forwarding\n
+            2 = multiple repeaters installed for 2-time forwarding
+        """
+        command = IveoGetRepeater()
+        response: IveoGetRepeaterResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def iveoSetLabel(self, id: int, label: str):
+        command = IveoSetLabel(id, label)
+        response: IveoSetLabelResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
+    async def iveoSetType(self, id: int, activity: int, type: DeviceType):
+        """
+        Sets the device configuration. \n
+        id: Iveo device id
+        activity: 0 = channel deactivated, 1 = channel active
+        type: DeviceType
+        
+        """
+        command = IveoSetConfig(id, activity, type)
+        response: IveoSetConfigResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
+    async def iveoGetType(self, id: int):
+        """
+        Gets the device configuration.
+
+        Params:
+        id: Iveo device id
+
+        Response:
+        name: Name of device
+        activity: 0 = channel deactivated, 1 = channel active
+        type: DeviceType
+        
+        """
+        command = IveoGetConfig(id)
+        response: IveoGetConfigResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+
+    async def iveoGetIds(self):
+        command = IveoGetIds()
+        response: IveoGetIdsResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def iveoFactoryReset(self):
+        command = IveoFactory()
+        response: IveoFactoryResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def iveoTeach(self):
+        command = IveoTeach()
+        response: IveoTeachResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def iveoLearn(self, id: int):
+        command = IveoLearn(id)
+        response: IveoLearnResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def iveoCommandManual(self, actorId: int, command: DriveCommandIveo):
+        command = IveoManual(actorId, command)
+        response: IveoManualResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def iveoCommandAutomatic(self, actorId: int, command: DriveCommandIveo):
+        command = IveoAutomatic(actorId, command)
+        response: IveoAutomaticResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    
+
     ### Sensor
+    async def sensorTeachStart(self):
+        command = SensorTechStart()
+        response: SensorTeachStartResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def sensorTeachStop(self):
+        command = SensorTeachStop()
+        response: SensorTeachStopResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def sensorTeachResult(self):
+        """ manually polls the teach result state, but the states are being reported automatically by the gateway itself"""
+        command = SensorTeachResult()
+        response: SensorTeachResultResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def sensorGetIds(self):
+        command = SensorGetIds()
+        response: SensorGetIdsResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def sensorGetInfo(self, id: int):
+        command = SensorGetInfo(id)
+        response: SensorGetInfoResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+
+    async def sensorGetValues(self, id: int):
+        command = SensorGetValues(id)
+        response: SensorGetValuesResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def sensorSetLabel(self, id: int, label: str):
+        command = SensorSetLabel(id, label)
+        response: SensorSetLabelResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
+    async def sensorDelete(self, id: int):
+        command = SensorDelete(id)
+        response: SensorDeleteResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
+    async def sensorWriteManual(self, id: int, address: int, name: str):
+        command = SensorWriteManual(id, address, name)
+        response: SensorWriteManualResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
     async def updateSensorValuesAsync(self, id: int):
         await self.executeCommand(SensorGetValues(id))
 
-    ### SenSim
+
+
+    ### SenSim - ToDo
     async def updateSenSimValuesAsync(self, id: int):
         await self.executeCommand(SenSimGetValues(id))
 
     ### Sender
+    async def senderTeachStart(self):
+        command = SenderTeachStart()
+        response: SenderTeachStartResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def senderTeachStop(self):
+        command = SenderTeachStop()
+        response: SenderTeachStopResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+    
+    async def senderTeachResult(self):
+        """ manually polls the teach result state, but the states are being reported automatically by the gateway itself"""
+        command = SenderTeachResult()
+        response: SenderTeachResultResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def senderGetIds(self):
+        command = SenderGetIds()
+        response: SenderGetIdsResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def senderGetInfo(self, id: int):
+        command = SenderGetInfo(id)
+        response: SenderGetInfoResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+
+    async def senderGetValues(self, id: int):
+        command = SenderGetValues(id)
+        response: SenderGetValuesResponse = await self.executeCommandSyncWithResponse(command)
+        return response
+    
+    async def senderSetLabel(self, id: int, label: str):
+        command = SenderSetLabel(id, label)
+        response: SenderSetLabelResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
+    async def senderDelete(self, id: int):
+        command = SenderDelete(id)
+        response: SenderDeleteResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
+    async def senderWriteManual(self, id: int, address: int, channel: int, resetCount: int, name: str):
+        command = SenderWriteManual(id, address, channel, resetCount, name)
+        response: SenderWriteManualResponse = await self.executeCommandSyncWithResponse(command)
+        return response.executed
+
+
+
+
     async def updateSenderValuesAsync(self, id: int):
         await self.executeCommand(SenderGetValues(id))
```

### Comparing `python-selve-new-2.2.1/selve/commands/command.py` & `python-selve-new-2.2.2/selve/commands/command.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/commands/device.py` & `python-selve-new-2.2.2/selve/commands/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
         super().__init__(CommeoDeviceCommand.SCANSTART)
 
 
 class DeviceScanStop(GatewayCommand):
     def __init__(self):
         super().__init__(CommeoDeviceCommand.SCANSTOP)
 
+class DeviceScanResult(GatewayCommand):
+    def __init__(self):
+        super().__init__(CommeoDeviceCommand.SCANRESULT)
+
 
 class DeviceSave(GatewayCommand):
     def __init__(self, id: int):
         super().__init__(CommeoDeviceCommand.SAVE, [(ParameterType.INT, id)])
 
 
 class DeviceGetIds(GatewayCommand):
```

### Comparing `python-selve-new-2.2.1/selve/commands/event.py` & `python-selve-new-2.2.2/selve/commands/event.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/commands/group.py` & `python-selve-new-2.2.2/selve/commands/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/commands/iveo.py` & `python-selve-new-2.2.2/selve/commands/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/commands/param.py` & `python-selve-new-2.2.2/selve/commands/param.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/commands/senSim.py` & `python-selve-new-2.2.2/selve/commands/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/commands/sender.py` & `python-selve-new-2.2.2/selve/commands/sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         super().__init__(CommeoSenderCommand.GETINFO, [(ParameterType.INT, id)])
         
 class SenderGetValues(GatewayCommand):
     def __init__(self, id: int):
         super().__init__(CommeoSenderCommand.GETVALUES, [(ParameterType.INT, id)])
         
 class SenderSetLabel(GatewayCommand):
-    def __init__(self, id: int):
-        super().__init__(CommeoSenderCommand.SETLABEL, [(ParameterType.INT, id)])
+    def __init__(self, id: int, name: str):
+        super().__init__(CommeoSenderCommand.SETLABEL, [(ParameterType.INT, id), (ParameterType.STRING, name)])
         
 class SenderDelete(GatewayCommand):
     def __init__(self, id: int):
         super().__init__(CommeoSenderCommand.DELETE, [(ParameterType.INT, id)])
         
 class SenderWriteManual(GatewayCommand):
     def __init__(self, id: int, adress: int, channel: int, resetCount: int, name: str):
```

### Comparing `python-selve-new-2.2.1/selve/commands/sensor.py` & `python-selve-new-2.2.2/selve/commands/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
         super().__init__(CommeoSensorCommand.TEACHSTART)
 
 
 class SensorTeachStop(GatewayCommand):
     def __init__(self):
         super().__init__(CommeoSensorCommand.TEACHSTOP)
 
+class SensorTeachResult(GatewayCommand):
+    def __init__(self):
+        super().__init__(CommeoSensorCommand.TEACHRESULT)
+
 
 class SensorGetIds(GatewayCommand):
     def __init__(self):
         super().__init__(CommeoSensorCommand.GETIDS)
 
 
 class SensorGetInfo(GatewayCommand):
```

### Comparing `python-selve-new-2.2.1/selve/commands/service.py` & `python-selve-new-2.2.2/selve/commands/service.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/device.py` & `python-selve-new-2.2.2/selve/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/group.py` & `python-selve-new-2.2.2/selve/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/iveo.py` & `python-selve-new-2.2.2/selve/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/senSim.py` & `python-selve-new-2.2.2/selve/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/sender.py` & `python-selve-new-2.2.2/selve/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/sensor.py` & `python-selve-new-2.2.2/selve/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/util/__init__.py` & `python-selve-new-2.2.2/selve/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/util/errors.py` & `python-selve-new-2.2.2/selve/util/errors.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/selve/util/protocol.py` & `python-selve-new-2.2.2/selve/util/protocol.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.1/setup.py` & `python-selve-new-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     
     name='python-selve-new',  # Required    
-    version='2.2.1',  # Required
+    version='2.2.2',  # Required
     description='Python library for interfacing with selve devices using the USB-RF controller. Written completely new.',  # Required   
     long_description=long_description,  # Optional 
     long_description_content_type="text/markdown",   
     url='https://github.com/Kannix2005/python-selve-new',  # Optional
     author='Stefan Altheimer',  # Optional
    
     author_email='me@stefan-altheimer.de',  # Optional
```

