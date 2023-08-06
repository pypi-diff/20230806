# Comparing `tmp/bec_device_server-0.9.1.tar.gz` & `tmp/bec_device_server-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_device_server-0.9.1.tar", last modified: Mon Jul  3 16:24:01 2023, max compression
+gzip compressed data, was "bec_device_server-0.9.2.tar", last modified: Tue Jul  4 13:48:12 2023, max compression
```

## Comparing `bec_device_server-0.9.1.tar` & `bec_device_server-0.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:24:01.017039 bec_device_server-0.9.1/
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-03 16:24:01.017039 bec_device_server-0.9.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:24:01.017039 bec_device_server-0.9.1/bec_device_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-03 16:24:00.000000 bec_device_server-0.9.1/bec_device_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-03 16:24:00.000000 bec_device_server-0.9.1/bec_device_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 16:24:00.000000 bec_device_server-0.9.1/bec_device_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-03 16:24:00.000000 bec_device_server-0.9.1/bec_device_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-03 16:24:00.000000 bec_device_server-0.9.1/bec_device_server.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:24:01.015040 bec_device_server-0.9.1/device_server/
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-28 10:41:58.000000 bec_device_server-0.9.1/device_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18508 2023-06-28 10:41:58.000000 bec_device_server-0.9.1/device_server/device_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:24:01.016039 bec_device_server-0.9.1/device_server/devices/
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-28 10:41:58.000000 bec_device_server-0.9.1/device_server/devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3473 2023-06-28 10:41:58.000000 bec_device_server-0.9.1/device_server/devices/config_update_handler.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-06-28 10:41:58.000000 bec_device_server-0.9.1/device_server/devices/device_serializer.py
--rw-r--r--   0 root         (0) root         (0)    13006 2023-06-28 10:41:58.000000 bec_device_server-0.9.1/device_server/devices/devicemanager.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-07-03 16:24:01.018039 bec_device_server-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      857 2023-06-28 14:27:03.000000 bec_device_server-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:12.336858 bec_device_server-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-04 13:48:12.336858 bec_device_server-0.9.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:12.336858 bec_device_server-0.9.2/bec_device_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-04 13:48:12.000000 bec_device_server-0.9.2/bec_device_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-04 13:48:12.000000 bec_device_server-0.9.2/bec_device_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:48:12.000000 bec_device_server-0.9.2/bec_device_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-04 13:48:12.000000 bec_device_server-0.9.2/bec_device_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-04 13:48:12.000000 bec_device_server-0.9.2/bec_device_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:12.334858 bec_device_server-0.9.2/device_server/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-06-28 10:41:58.000000 bec_device_server-0.9.2/device_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18508 2023-06-28 10:41:58.000000 bec_device_server-0.9.2/device_server/device_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:12.335858 bec_device_server-0.9.2/device_server/devices/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-28 10:41:58.000000 bec_device_server-0.9.2/device_server/devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2023-07-04 13:47:41.000000 bec_device_server-0.9.2/device_server/devices/config_update_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-06-28 10:41:58.000000 bec_device_server-0.9.2/device_server/devices/device_serializer.py
+-rw-r--r--   0 root         (0) root         (0)    13111 2023-07-04 13:47:41.000000 bec_device_server-0.9.2/device_server/devices/devicemanager.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-07-04 13:48:12.337858 bec_device_server-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-04 13:47:41.000000 bec_device_server-0.9.2/setup.py
```

### Comparing `bec_device_server-0.9.1/device_server/device_server.py` & `bec_device_server-0.9.2/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-0.9.1/device_server/devices/config_update_handler.py` & `bec_device_server-0.9.2/device_server/devices/config_update_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -58,40 +58,49 @@
             error_msg = traceback.format_exc()
             accepted = False
         finally:
             self.send_config_request_reply(
                 accepted=accepted, error_msg=error_msg, metadata=msg.metadata
             )
 
-    def send_config_request_reply(self, accepted, error_msg, metadata):
-        """send a config request reply"""
+    def send_config_request_reply(self, accepted: bool, error_msg: str, metadata: dict) -> None:
+        """
+        Sends a config request reply
+
+        Args:
+            accepted (bool): Whether the request was accepted
+            error_msg (str): Error message
+            metadata (dict): Metadata of the request
+        """
         msg = BECMessage.RequestResponseMessage(
             accepted=accepted, message=error_msg, metadata=metadata
         )
         RID = metadata.get("RID")
         self.device_manager.producer.set(
             MessageEndpoints.device_config_request_response(RID), msg.dumps(), expire=60
         )
 
-    def _update_config(self, msg):
+    def _update_config(self, msg: BECMessage.DeviceConfigMessage) -> None:
         for dev, dev_config in msg.content["config"].items():
             device = self.device_manager.devices[dev]
             if "deviceConfig" in dev_config:
                 # store old config
                 old_config = device._config["deviceConfig"].copy()
 
                 # apply config
                 try:
                     self.device_manager.update_config(device.obj, dev_config["deviceConfig"])
                 except Exception as exc:
                     self.device_manager.update_config(device.obj, old_config)
-                    raise DeviceConfigError(f"Error during object update. {exc}") from exc
+                    raise DeviceConfigError(f"Error during object update. {exc}")
 
             if "enabled" in dev_config:
+                device._config["enabled"] = dev_config["enabled"]
                 if dev_config["enabled"]:
                     # pylint:disable=protected-access
                     if device.obj._destroyed:
                         self.device_manager.initialize_device(device._config)
                     else:
                         self.device_manager.initialize_enabled_device(device)
                 else:
                     self.device_manager.disconnect_device(device.obj)
+                    self.device_manager.reset_device(device)
```

### Comparing `bec_device_server-0.9.1/device_server/devices/device_serializer.py` & `bec_device_server-0.9.2/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-0.9.1/device_server/devices/devicemanager.py` & `bec_device_server-0.9.2/device_server/devices/devicemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,18 @@
         if not obj.connected:
             return
         if hasattr(obj, "controller"):
             obj.controller.off()
             return
         obj.destroy()
 
+    def reset_device(self, obj: DSDevice):
+        """reset a device"""
+        obj.initialized = False
+
     @staticmethod
     def connect_device(obj):
         """establish a connection to a device"""
         if obj.connected:
             return
         if hasattr(obj, "controller"):
             obj.controller.on()
```

### Comparing `bec_device_server-0.9.1/setup.cfg` & `bec_device_server-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_device_server-0.9.1/setup.py` & `bec_device_server-0.9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,12 +19,13 @@
         version = res.split("=")[1]
     return version.strip().strip('"')
 
 
 if __name__ == "__main__":
     setup(
         install_requires=["numpy", "ophyd", "msgpack", "pyyaml"],
+        extras_require={"dev": ["pytest", "pytest-random-order", "coverage"]},
         version=get_version(),
     )
     local_deps = [utils, ophyd_devices]
     for dep in local_deps:
         subprocess.run(f"pip install -e {dep}", shell=True, check=True)
```

